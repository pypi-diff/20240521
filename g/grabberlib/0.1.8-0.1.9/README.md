# Comparing `tmp/grabberlib-0.1.8.tar.gz` & `tmp/grabberlib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grabberlib-0.1.8.tar", max compression
+gzip compressed data, was "grabberlib-0.1.9.tar", max compression
```

## Comparing `grabberlib-0.1.8.tar` & `grabberlib-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.755675 grabberlib-0.1.8/README.md
--rw-r--r--   0        0        0        1 2024-04-20 14:47:15.755675 grabberlib-0.1.8/assets/pages.txt
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.8/grabber/__init__.py
--rw-r--r--   0        0        0     1690 2024-04-20 14:47:15.759675 grabberlib-0.1.8/grabber/__main__.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.8/grabber/controllers/__init__.py
--rw-r--r--   0        0        0     5403 2024-05-14 12:31:46.304901 grabberlib-0.1.8/grabber/controllers/base.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.8/grabber/core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 14:35:12.060596 grabberlib-0.1.8/grabber/core/bot/__init__.py
--rw-r--r--   0        0        0     1287 2024-05-10 12:20:10.885923 grabberlib-0.1.8/grabber/core/bot/core.py
--rw-r--r--   0        0        0       65 2024-04-20 14:47:15.759675 grabberlib-0.1.8/grabber/core/exc.py
--rw-r--r--   0        0        0      772 2024-05-09 12:59:39.317729 grabberlib-0.1.8/grabber/core/settings.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.8/grabber/core/sources/__init__.py
--rw-r--r--   0        0        0     3320 2024-05-10 14:42:57.044880 grabberlib-0.1.8/grabber/core/sources/common.py
--rw-r--r--   0        0        0     3653 2024-05-09 13:30:04.157477 grabberlib-0.1.8/grabber/core/sources/everia.py
--rw-r--r--   0        0        0     2698 2024-05-10 12:33:08.173014 grabberlib-0.1.8/grabber/core/sources/graph.py
--rw-r--r--   0        0        0     4156 2024-05-14 12:33:33.314298 grabberlib-0.1.8/grabber/core/sources/hotgirl_asia.py
--rw-r--r--   0        0        0     3290 2024-05-14 12:17:41.832296 grabberlib-0.1.8/grabber/core/sources/khd.py
--rw-r--r--   0        0        0     3409 2024-05-13 15:57:32.514304 grabberlib-0.1.8/grabber/core/sources/nudecosplay.py
--rw-r--r--   0        0        0     2818 2024-05-09 12:59:39.317729 grabberlib-0.1.8/grabber/core/sources/xasiat.py
--rw-r--r--   0        0        0     2950 2024-05-10 12:23:01.737325 grabberlib-0.1.8/grabber/core/sources/xiuren.py
--rw-r--r--   0        0        0        1 2024-04-20 14:47:15.759675 grabberlib-0.1.8/grabber/core/sources/yellow.py
--rw-r--r--   0        0        0    19475 2024-05-14 12:31:08.197949 grabberlib-0.1.8/grabber/core/utils.py
--rw-r--r--   0        0        0      175 2024-05-14 12:37:11.872860 grabberlib-0.1.8/grabber/core/version.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.8/grabber/templates/__init__.py
--rw-r--r--   0        0        0     1036 2024-05-14 12:37:16.236749 grabberlib-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 grabberlib-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.755675 grabberlib-0.1.9/README.md
+-rw-r--r--   0        0        0        1 2024-04-20 14:47:15.755675 grabberlib-0.1.9/assets/pages.txt
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.9/grabber/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-20 14:47:15.759675 grabberlib-0.1.9/grabber/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.9/grabber/controllers/__init__.py
+-rw-r--r--   0        0        0     5601 2024-05-15 12:59:42.473190 grabberlib-0.1.9/grabber/controllers/base.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.9/grabber/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 14:35:12.060596 grabberlib-0.1.9/grabber/core/bot/__init__.py
+-rw-r--r--   0        0        0     1287 2024-05-10 12:20:10.885923 grabberlib-0.1.9/grabber/core/bot/core.py
+-rw-r--r--   0        0        0       65 2024-04-20 14:47:15.759675 grabberlib-0.1.9/grabber/core/exc.py
+-rw-r--r--   0        0        0      772 2024-05-09 12:59:39.317729 grabberlib-0.1.9/grabber/core/settings.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.9/grabber/core/sources/__init__.py
+-rw-r--r--   0        0        0     3320 2024-05-10 14:42:57.044880 grabberlib-0.1.9/grabber/core/sources/common.py
+-rw-r--r--   0        0        0     3653 2024-05-09 13:30:04.157477 grabberlib-0.1.9/grabber/core/sources/everia.py
+-rw-r--r--   0        0        0     2698 2024-05-10 12:33:08.173014 grabberlib-0.1.9/grabber/core/sources/graph.py
+-rw-r--r--   0        0        0     4157 2024-05-15 13:05:53.794301 grabberlib-0.1.9/grabber/core/sources/hotgirl_asia.py
+-rw-r--r--   0        0        0     3293 2024-05-15 12:44:50.560562 grabberlib-0.1.9/grabber/core/sources/khd.py
+-rw-r--r--   0        0        0     2866 2024-05-15 12:59:07.846099 grabberlib-0.1.9/grabber/core/sources/kup.py
+-rw-r--r--   0        0        0     3409 2024-05-13 15:57:32.514304 grabberlib-0.1.9/grabber/core/sources/nudecosplay.py
+-rw-r--r--   0        0        0     2695 2024-05-15 12:50:26.711771 grabberlib-0.1.9/grabber/core/sources/xasiat.py
+-rw-r--r--   0        0        0     2950 2024-05-10 12:23:01.737325 grabberlib-0.1.9/grabber/core/sources/xiuren.py
+-rw-r--r--   0        0        0        1 2024-04-20 14:47:15.759675 grabberlib-0.1.9/grabber/core/sources/yellow.py
+-rw-r--r--   0        0        0    19529 2024-05-15 13:00:35.923585 grabberlib-0.1.9/grabber/core/utils.py
+-rw-r--r--   0        0        0      175 2024-05-15 13:21:09.413050 grabberlib-0.1.9/grabber/core/version.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.9/grabber/templates/__init__.py
+-rw-r--r--   0        0        0     1036 2024-05-15 13:21:16.132868 grabberlib-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 grabberlib-0.1.9/PKG-INFO
```

### Comparing `grabberlib-0.1.8/grabber/__main__.py` & `grabberlib-0.1.9/grabber/__main__.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.8/grabber/controllers/base.py` & `grabberlib-0.1.9/grabber/controllers/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 from grabber.core.settings import TELEGRAPH_TOKEN
 from grabber.core.sources.common import get_sources_for_common
 from grabber.core.sources.everia import get_sources_for_everia
 from grabber.core.sources.graph import get_for_telegraph
 from grabber.core.sources.hotgirl_asia import get_sources_for_hotgirl_asia
 from grabber.core.sources.khd import get_sources_for_4khd
+from grabber.core.sources.kup import get_sources_for_4kup
 from grabber.core.sources.nudecosplay import get_sources_for_nudecosplay
+from grabber.core.sources.xasiat import get_for_xasiat
 from grabber.core.sources.xiuren import get_sources_for_xiuren
 from grabber.core.utils import upload_folders_to_telegraph
 
 from ..core.version import get_version
 
 VERSION_BANNER = f"""
 A beautiful CLI utility to download images from the web! {get_version()}
@@ -135,25 +137,27 @@
             "nudebird": get_sources_for_nudecosplay,
             "hotgirl": get_sources_for_nudecosplay,
             "everia": get_sources_for_everia,
             "bestgirlsexy": get_sources_for_common,
             "asigirl": get_sources_for_common,
             "cosplaytele": get_sources_for_common,
             "hotgirl.asia": get_sources_for_hotgirl_asia,
+            "xasiat": get_for_xasiat,
+            "4kup": get_sources_for_4kup,
         }
 
         if upload:
             upload_folders_to_telegraph(
                 folder_name=folder,
                 limit=limit,
                 send_to_channel=send_to_telegram,
                 telegraph_client=telegraph_client,
             )
         else:
-            getter_images = getter_mapping.get(entity, get_for_telegraph)
+            getter_images = getter_mapping.get(entity, get_sources_for_common)
             getter_images(
                 sources=sources,
                 entity=entity,
                 telegraph_client=telegraph_client,
                 final_dest=folder,
                 save_to_telegraph=publish,
                 is_tag=is_tag,
```

### Comparing `grabberlib-0.1.8/grabber/core/bot/core.py` & `grabberlib-0.1.9/grabber/core/bot/core.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.8/grabber/core/settings.py` & `grabberlib-0.1.9/grabber/core/settings.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.8/grabber/core/sources/common.py` & `grabberlib-0.1.9/grabber/core/sources/common.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.8/grabber/core/sources/everia.py` & `grabberlib-0.1.9/grabber/core/sources/everia.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.8/grabber/core/sources/graph.py` & `grabberlib-0.1.9/grabber/core/sources/graph.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.8/grabber/core/sources/hotgirl_asia.py` & `grabberlib-0.1.9/grabber/core/sources/hotgirl_asia.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         source_urls.add(url)
         return source_urls
 
     first_page = soup.select(pages_count_query)[0]
     last_page = soup.select(pages_count_query)[-1]
     first_page_number = int(first_page.text)
     last_page_number = int(last_page.text)
-    base_url, _, = url.rsplit("?", 2)
+    base_url, *_, = url.rsplit("?", 2)
     pagination_base_url = "{base_url}/?num={page_number}&stype=showall"
     
     for index in range(first_page_number, last_page_number + 1):
         if index == 1:
             continue
         
         target_url = pagination_base_url.format(
```

### Comparing `grabberlib-0.1.8/grabber/core/sources/khd.py` & `grabberlib-0.1.9/grabber/core/sources/khd.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 query=query,
             )
             image_tags.extend(tags or [])
 
             if index == 0:
                 folder_name = soup.select("title")[0].get_text()  # type: ignore
                 page_title = folder_name.strip().rstrip()
-                titles.add(page_title)
+                titles.append(page_title)
 
         if page_title is None:
             page_title = soup.find('title').get_text(strip=True)
             titles.append(page_title)
 
         unique_img_urls = set()
         for idx, img_tag in enumerate(image_tags):
```

### Comparing `grabberlib-0.1.8/grabber/core/sources/nudecosplay.py` & `grabberlib-0.1.9/grabber/core/sources/nudecosplay.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.8/grabber/core/sources/xasiat.py` & `grabberlib-0.1.9/grabber/core/sources/kup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,93 +1,92 @@
 import pathlib
-from typing import List
+from typing import List, Optional
 
 from telegraph import Telegraph
 from tqdm import tqdm
 
-from grabber.core.settings import get_media_root
 from grabber.core.utils import (
     downloader,
     query_mapping,
     headers_mapping,
     get_tags,
     telegraph_uploader,
 )
 
 
-def get_for_xasiat(
+def get_images_from_pagination(url: str, headers: Optional[dict] = None) -> List[str]:
+    page_nav_query = "div.page-link-box li a.page-numbers"
+    tags, _ = get_tags(url, headers=headers, query=page_nav_query)
+    return [a.attrs["href"] for a in tags if tags]
+
+
+def get_sources_for_4kup(
     sources: List[str],
     entity: str,
-    telegraph_client: Telegraph,
+    telegraph_client: Optional[Telegraph] = None,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
-    **kwargs,
+    is_tag: Optional[bool] = False,
+    limit: Optional[int] = None,
 ) -> None:
-    send_to_telegram = kwargs.get("send_to_telegram", False)
-    titles = set()
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
+        desc="Retrieving URLs...",
     )
     query, src_attr = query_mapping[entity]
     headers = headers_mapping.get(entity, None)
-    folders = set()
-    titles_and_folders = set()
+    page_title = None
     title_folder_mapping = {}
+    posts_sent_counter = 0
+    titles = []
 
     if final_dest:
-        final_dest_folder = get_media_root() / final_dest
-        if not final_dest_folder.exists():
-            final_dest_folder.mkdir(parents=True, exist_ok=True)
-            final_dest = final_dest_folder
+        final_dest = pathlib.Path(final_dest)
+        if not final_dest.exists():
+            final_dest.mkdir(parents=True, exist_ok=True)
 
     for idx, source_url in tqdm_sources_iterable:
-        folder_name = ""
-        tqdm_sources_iterable.set_description(f"Retrieving URLs from {source_url}")
-        tags, soup = get_tags(
+        image_tags, soup = get_tags(
             source_url,
             headers=headers,
             query=query,
         )
 
-        title_tag = soup.select("title")[0]  # type: ignore
-        folder_name = title_tag.get_text().strip().rstrip()
-        title = folder_name
-        titles.add(title)
-        titles_and_folders.add((title, folder_name))
-
-        if final_dest:
-            new_folder = get_media_root() / final_dest / folder_name
-        else:
-            new_folder = get_media_root() / folder_name
-
-        if not new_folder.exists():
-            new_folder.mkdir(parents=True, exist_ok=True)
+        if page_title is None:
+            page_title = soup.find("title").get_text(separator=" ", strip=True).split("- Beautiful")[0].rstrip()
+            titles.append(page_title)
 
-        folders.add(new_folder)
         unique_img_urls = set()
-
-        for idx, img_tag in enumerate(tags or []):
+        for idx, img_tag in enumerate(image_tags):
             img_src = img_tag.attrs[src_attr]
+            img_name: str = img_src.split("/")[-1].split("?")[0]
+            img_name = img_name.strip().rstrip()
+            unique_img_urls.add((f"{idx + 1}-{img_name}", img_src))
 
-            if "xasiat" in img_src:
-                img_name: str = img_src.split("/")[-2]
-                img_name = img_name.strip().rstrip()
-                img_extension: str = img_name.split(".")[-1]
-            else:
-                img_name: str = img_src.split("/")[-1]
-                img_name = img_name.strip().rstrip()
-                img_extension: str = img_name.split(".")[-1]
+        tqdm_sources_iterable.set_description(f"Finished retrieving images for {page_title}")
 
-            unique_img_urls.add(
-                (title, f"{idx + 1}.{img_extension}", img_src),
+        if final_dest:
+            folder_name = page_title
+            title_dest = final_dest / folder_name
+            if not title_dest.exists():
+                title_dest.mkdir(parents=True, exist_ok=True)
+            title_folder_mapping[page_title] = (unique_img_urls, title_dest)
+
+        if save_to_telegraph:
+            telegraph_uploader(
+                unique_img_urls=unique_img_urls,
+                page_title=page_title,
+                posts_sent_counter=posts_sent_counter,
+                telegraph_client=telegraph_client,
+                tqdm_iterable=tqdm_sources_iterable,
             )
+            posts_sent_counter += 1
+        page_title = None
 
-        title_folder_mapping[title] = (unique_img_urls, new_folder)
+    if final_dest:
+        downloader(
+            titles=titles,
+            title_folder_mapping=title_folder_mapping,
+            headers=headers,
+        )
 
-    downloader(title_folder_mapping, headers)
-    telegraph_uploader(
-        title_folder_mapping=title_folder_mapping,
-        send_to_telegram=send_to_telegram,
-        save_to_telegraph=save_to_telegraph,
-        telegraph_client=telegraph_client,
-    )
```

### Comparing `grabberlib-0.1.8/grabber/core/sources/xiuren.py` & `grabberlib-0.1.9/grabber/core/sources/xiuren.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.8/grabber/core/utils.py` & `grabberlib-0.1.9/grabber/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         "href",
     ),
     "everia": ("div.entry-content img", "src"),
     "bestgirlsexy": ("div.elementor-widget-container p img", "data-src"),
     "asigirl": ("a.asigirl-item", "href"),
     "cosplaytele": ("img.attachment-full.size-full", "src"),
     "hotgirl.asia": ("div.galeria_img img", "src"),
+    "4kup": ("div#gallery div.caption a.cp", "href"),
 }
 
 
 @dataclass(kw_only=True)
 class PaginationXPath:
     pagination_query: str
     pages_count_query: str
```

### Comparing `grabberlib-0.1.8/pyproject.toml` & `grabberlib-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grabberlib"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["grabber"]
 readme = "README.md"
 packages = [
     { include = "grabber/**/*.py" },
     { include = "assets/pages.txt" },
 ]
```

### Comparing `grabberlib-0.1.8/PKG-INFO` & `grabberlib-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grabberlib
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: grabber
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

