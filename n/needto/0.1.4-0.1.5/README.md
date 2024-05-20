# Comparing `tmp/needto-0.1.4.tar.gz` & `tmp/needto-0.1.5.tar.gz`

## Comparing `needto-0.1.4.tar` & `needto-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 needto-0.1.4/needto/__about__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 needto-0.1.4/needto/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 needto-0.1.4/needto/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 needto-0.1.4/needto/src/__init__.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 needto-0.1.4/needto/src/ai_client.py
--rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 needto-0.1.4/needto/src/cli.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 needto-0.1.4/needto/src/config.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 needto-0.1.4/needto/src/utils.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 needto-0.1.4/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 needto-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 needto-0.1.4/README.md
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 needto-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 needto-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 needto-0.1.5/needto/__about__.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 needto-0.1.5/needto/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 needto-0.1.5/needto/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 needto-0.1.5/needto/src/__init__.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 needto-0.1.5/needto/src/ai_client.py
+-rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 needto-0.1.5/needto/src/cli.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 needto-0.1.5/needto/src/config.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 needto-0.1.5/needto/src/utils.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 needto-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 needto-0.1.5/LICENSE.txt
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 needto-0.1.5/README.md
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 needto-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 needto-0.1.5/PKG-INFO
```

### Comparing `needto-0.1.4/needto/src/ai_client.py` & `needto-0.1.5/needto/src/ai_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import time
 import sys
 import rich.console
 import rich.prompt
 from .config import config_manager
 
 import rich.console
 import json
@@ -41,28 +40,38 @@
             console.print("Got this from stdin:")
             console.print(stdin)
             messages.append(
                 {"role": "user", "content": f"Additional information:\n{stdin}"}
             )
         self.messages = messages
 
+        if not config_manager.values.groq_api_key:
+            console.print(
+                "No GROQ API key found. Please run `needto config` to add it."
+            )
+            sys.exit(1)
+
         self.client = groq.Groq(
             api_key=config_manager.values.groq_api_key,
         )
 
     def ask(self, prompt: str, print_prompt=False, output_limit: int = 2000):
         prompt = prompt.strip()[:output_limit]
         console = rich.console.Console()
         if print_prompt:
             print()
             console.print(prompt)
             print()
 
         self.messages.append({"role": "user", "content": prompt})
 
+        if not config_manager.values.model_name:
+            console.print("No model name found. Please run `needto config` to add it.")
+            sys.exit(1)
+
         retry_count = 3
         for _ in range(retry_count):
             chat_completion = self.client.chat.completions.create(
                 messages=self.messages,
                 model=config_manager.values.model_name,
                 # response_format={"type": "json_object"},
             )
```

### Comparing `needto-0.1.4/needto/src/cli.py` & `needto-0.1.5/needto/src/cli.py`

 * *Files identical despite different names*

### Comparing `needto-0.1.4/needto/src/config.py` & `needto-0.1.5/needto/src/config.py`

 * *Files identical despite different names*

### Comparing `needto-0.1.4/needto/src/utils.py` & `needto-0.1.5/needto/src/utils.py`

 * *Files identical despite different names*

### Comparing `needto-0.1.4/.gitignore` & `needto-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `needto-0.1.4/LICENSE.txt` & `needto-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `needto-0.1.4/README.md` & `needto-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `needto-0.1.4/pyproject.toml` & `needto-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `needto-0.1.4/PKG-INFO` & `needto-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: needto
-Version: 0.1.4
+Version: 0.1.5
 Summary: Ask AI for help you in your terminal.
 Project-URL: Documentation, https://github.com/danialkeimasi/needto#readme
 Project-URL: Issues, https://github.com/danialkeimasi/needto/issues
 Project-URL: Source, https://github.com/danialkeimasi/needto
 Author-email: Danial Keimasi <danialkeimasi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

