# Comparing `tmp/needto-0.1.6.tar.gz` & `tmp/needto-0.1.7.tar.gz`

## Comparing `needto-0.1.6.tar` & `needto-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 needto-0.1.6/needto/__about__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 needto-0.1.6/needto/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 needto-0.1.6/needto/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 needto-0.1.6/needto/src/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 needto-0.1.6/needto/src/ai_client.py
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 needto-0.1.6/needto/src/cli.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 needto-0.1.6/needto/src/config.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 needto-0.1.6/needto/src/utils.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 needto-0.1.6/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 needto-0.1.6/LICENSE.txt
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 needto-0.1.6/README.md
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 needto-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 needto-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 needto-0.1.7/needto/__about__.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 needto-0.1.7/needto/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 needto-0.1.7/needto/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 needto-0.1.7/needto/src/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 needto-0.1.7/needto/src/ai_client.py
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 needto-0.1.7/needto/src/cli.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 needto-0.1.7/needto/src/config.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 needto-0.1.7/needto/src/utils.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 needto-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 needto-0.1.7/LICENSE.txt
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 needto-0.1.7/README.md
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 needto-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 needto-0.1.7/PKG-INFO
```

### Comparing `needto-0.1.6/needto/src/ai_client.py` & `needto-0.1.7/needto/src/ai_client.py`

 * *Files identical despite different names*

### Comparing `needto-0.1.6/needto/src/cli.py` & `needto-0.1.7/needto/src/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,21 +95,21 @@
                         + (
                             f"stderr:\n{command_output.stderr.decode()}"
                             if command_output.stderr
                             else ""
                         ),
                         print_prompt=True,
                     )
-            else:
-                console.print("Leave blank to end conversation", style="blue bold")
-                if user_prompt := input("> "):
-                    print()
-                    parsed_answer = ai_client.ask(user_prompt)
-                else:
-                    break
+
+                continue
+
+        console.print("Leave blank to end conversation", style="blue bold")
+        if user_prompt := input("> "):
+            print()
+            parsed_answer = ai_client.ask(user_prompt)
         else:
             break
 
 
 @app.command(help="Write code.")
 def write(prompt_list: list[str]):
     prompt = " ".join(prompt_list)
```

### Comparing `needto-0.1.6/needto/src/config.py` & `needto-0.1.7/needto/src/config.py`

 * *Files identical despite different names*

### Comparing `needto-0.1.6/needto/src/utils.py` & `needto-0.1.7/needto/src/utils.py`

 * *Files identical despite different names*

### Comparing `needto-0.1.6/.gitignore` & `needto-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `needto-0.1.6/LICENSE.txt` & `needto-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `needto-0.1.6/README.md` & `needto-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `needto-0.1.6/pyproject.toml` & `needto-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `needto-0.1.6/PKG-INFO` & `needto-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: needto
-Version: 0.1.6
+Version: 0.1.7
 Summary: Ask AI for help you in your terminal.
 Project-URL: Documentation, https://github.com/danialkeimasi/needto#readme
 Project-URL: Issues, https://github.com/danialkeimasi/needto/issues
 Project-URL: Source, https://github.com/danialkeimasi/needto
 Author-email: Danial Keimasi <danialkeimasi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

