# Comparing `tmp/html_summary-0.2.1-py3-none-any.whl.zip` & `tmp/html_summary-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3650 bytes, number of entries: 8
+Zip file size: 3706 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 html_summary/__init__.py
--rw-r--r--  2.0 unx      831 b- defN 80-Jan-01 00:00 html_summary/cli.py
--rw-r--r--  2.0 unx     1282 b- defN 80-Jan-01 00:00 html_summary/summary.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 html_summary-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      751 b- defN 80-Jan-01 00:00 html_summary-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 html_summary-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 html_summary-0.2.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      646 b- defN 16-Jan-01 00:00 html_summary-0.2.1.dist-info/RECORD
-8 files, 4718 bytes uncompressed, 2514 bytes compressed:  46.7%
+-rw-r--r--  2.0 unx      998 b- defN 80-Jan-01 00:00 html_summary/cli.py
+-rw-r--r--  2.0 unx     1406 b- defN 80-Jan-01 00:00 html_summary/summary.py
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 html_summary-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      789 b- defN 80-Jan-01 00:00 html_summary-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 html_summary-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 html_summary-0.3.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      646 b- defN 16-Jan-01 00:00 html_summary-0.3.0.dist-info/RECORD
+8 files, 5047 bytes uncompressed, 2570 bytes compressed:  49.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: html_summary/cli.py
 Comment: 
 
 Filename: html_summary/summary.py
 Comment: 
 
-Filename: html_summary-0.2.1.dist-info/LICENSE
+Filename: html_summary-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: html_summary-0.2.1.dist-info/METADATA
+Filename: html_summary-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: html_summary-0.2.1.dist-info/WHEEL
+Filename: html_summary-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: html_summary-0.2.1.dist-info/entry_points.txt
+Filename: html_summary-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: html_summary-0.2.1.dist-info/RECORD
+Filename: html_summary-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## html_summary/cli.py

```diff
@@ -3,15 +3,17 @@
 
 import click
 import httpx
 from dotenv import find_dotenv
 from dotenv import load_dotenv
 from loguru import logger
 
-from .summary import summarize_html
+from .summary import load_html
+from .summary import load_pdf
+from .summary import summarize
 
 
 def fetch_content(path: str) -> str:
     if path.startswith("http"):
         resp = httpx.get(url=path)
         resp.raise_for_status()
 
@@ -22,16 +24,18 @@
         f = path
     return f
 
 
 @click.command()
 @click.argument("path", type=click.STRING)
 @click.option("-l", "--lang", type=click.STRING, default="English")
-def main(path: str, lang: str) -> None:
+@click.option("--pdf", is_flag=True, type=click.BOOL)
+def main(path: str, lang: str, pdf: bool) -> None:
     load_dotenv(find_dotenv())
 
     lang = os.getenv("HTML_SUMMARY_LANG", lang)
 
     f = fetch_content(path)
 
-    s = summarize_html(f, lang)
+    text = load_pdf(f) if pdf else load_html(f)
+    s = summarize(text, lang)
     logger.info("summarization:\n{}", s)
```

## html_summary/summary.py

```diff
@@ -1,19 +1,18 @@
 import functools
 from pathlib import Path
 
-from langchain.chains.llm import LLMChain
 from langchain.globals import set_llm_cache
 from langchain_community.cache import SQLiteCache
 from langchain_community.document_loaders.html_bs import BSHTMLLoader
+from langchain_community.document_loaders.pdf import PyPDFLoader
 from langchain_core.messages import AIMessage
 from langchain_core.prompts import PromptTemplate
 from langchain_core.runnables import RunnableSerializable
 from langchain_openai import ChatOpenAI
-from loguru import logger
 
 database_path = Path.home() / ".cache" / ".langchain.db"
 cache = SQLiteCache(database_path.as_posix())
 set_llm_cache(cache)
 
 
 PROMPT_TEMPLATE = """Write a concise summary in bullet points using {lang} for the following article:
@@ -26,18 +25,23 @@
 def get_chain() -> RunnableSerializable:
     llm = ChatOpenAI(temperature=0, model="gpt-4-turbo")
     prompt = PromptTemplate.from_template(PROMPT_TEMPLATE)
     chain = prompt | llm
     return chain
 
 
-def summarize_html(f: str, lang: str = "English") -> str:
-    logger.info("summarize html: {}", f)
-
+def load_html(f: str) -> str:
     loader = BSHTMLLoader(f)
     docs = loader.load()
+    return "\n".join([doc.page_content for doc in docs])
+
+
+def load_pdf(f: str) -> str:
+    loader = PyPDFLoader(f)
+    docs = loader.load()
+    return "\n".join([doc.page_content for doc in docs])
 
-    text = "\n".join([doc.page_content for doc in docs])
 
+def summarize(text: str, lang: str = "English") -> str:
     chain = get_chain()
     ai_message: AIMessage = chain.invoke({"text": text, "lang": lang})
     return ai_message.pretty_repr()
```

## Comparing `html_summary-0.2.1.dist-info/LICENSE` & `html_summary-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `html_summary-0.2.1.dist-info/METADATA` & `html_summary-0.3.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html_summary
-Version: 0.2.1
+Version: 0.3.0
 Summary: 
 Author: narumi
 Author-email: toucans-cutouts0f@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -13,8 +13,9 @@
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: langchain (>=0.1.17,<0.2.0)
 Requires-Dist: langchain-openai (>=0.1.6,<0.2.0)
 Requires-Dist: langchain-text-splitters (>=0.0.1,<0.0.2)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: lxml (>=5.2.1,<6.0.0)
+Requires-Dist: pypdf (>=4.2.0,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
```

## Comparing `html_summary-0.2.1.dist-info/RECORD` & `html_summary-0.3.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 html_summary/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-html_summary/cli.py,sha256=C07FIO7FaJl0YRDoUi-XD-EoM4sfAx7RTeCMCljZZ64,831
-html_summary/summary.py,sha256=bazLgK_0czECoC9TRqYKWGgDfAmDJAnjorsKlOj_pEw,1282
-html_summary-0.2.1.dist-info/LICENSE,sha256=H2T3_RTgmcngMeC7p_SXT3GwBLkd2DaNgAZuxulcfiA,1066
-html_summary-0.2.1.dist-info/METADATA,sha256=gk1Mp017OtPnVhW2WTRLDvMVmyFyuzYaoaCbbijyNnE,751
-html_summary-0.2.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-html_summary-0.2.1.dist-info/entry_points.txt,sha256=oUHajPykJSfIzQR2yTXw3M9HasZCYyG4unSL2lkkies,54
-html_summary-0.2.1.dist-info/RECORD,,
+html_summary/cli.py,sha256=YQ8HL5itdHUy3dZVKnjsgGhTqxbtaoMDC6ycVjSI070,998
+html_summary/summary.py,sha256=lsJ_xi5roXS1uK7m_m8Ofk_nAOY2L-jNvsUPpJTqz2E,1406
+html_summary-0.3.0.dist-info/LICENSE,sha256=H2T3_RTgmcngMeC7p_SXT3GwBLkd2DaNgAZuxulcfiA,1066
+html_summary-0.3.0.dist-info/METADATA,sha256=JHhtAUznq6DMJ_Z-VzYrVjuqgRDjTo73s9JjB1UL3aU,789
+html_summary-0.3.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+html_summary-0.3.0.dist-info/entry_points.txt,sha256=oUHajPykJSfIzQR2yTXw3M9HasZCYyG4unSL2lkkies,54
+html_summary-0.3.0.dist-info/RECORD,,
```

