# Comparing `tmp/flask_vite-0.3.9.tar.gz` & `tmp/flask_vite-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_vite-0.3.9.tar", max compression
+gzip compressed data, was "flask_vite-0.4.0.tar", max compression
```

## Comparing `flask_vite-0.3.9.tar` & `flask_vite-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      144 2023-10-27 14:41:44.670623 flask_vite-0.3.9/AUTHORS.rst
--rw-r--r--   0        0        0     1074 2023-10-27 14:31:08.285369 flask_vite-0.3.9/LICENSE
--rw-r--r--   0        0        0     4335 2023-10-27 14:33:46.572110 flask_vite-0.3.9/README.md
--rw-r--r--   0        0        0      999 2024-04-26 16:36:34.001504 flask_vite-0.3.9/pyproject.toml
--rw-r--r--   0        0        0      157 2024-04-26 16:16:57.467495 flask_vite-0.3.9/src/flask_vite/__init__.py
--rw-r--r--   0        0        0     1653 2024-04-26 16:25:38.956462 flask_vite-0.3.9/src/flask_vite/cli.py
--rw-r--r--   0        0        0     1974 2024-04-26 16:31:01.388966 flask_vite-0.3.9/src/flask_vite/extension.py
--rw-r--r--   0        0        0     1263 2024-04-26 16:34:32.184328 flask_vite-0.3.9/src/flask_vite/npm.py
--rw-r--r--   0        0        0       50 2023-07-04 09:13:43.637994 flask_vite-0.3.9/src/flask_vite/starter/.gitignore
--rwxr-xr-t   0        0        0    52227 2024-01-10 18:30:13.543461 flask_vite-0.3.9/src/flask_vite/starter/bun.lockb
--rw-r--r--   0        0        0      280 2023-07-04 08:57:59.573627 flask_vite-0.3.9/src/flask_vite/starter/index.html
--rw-r--r--   0        0        0       27 2023-07-04 09:14:53.281846 flask_vite-0.3.9/src/flask_vite/starter/main.js
--rw-r--r--   0        0        0      360 2024-01-10 18:30:05.609248 flask_vite-0.3.9/src/flask_vite/starter/package.json
--rw-r--r--   0        0        0       82 2023-07-04 09:05:39.738914 flask_vite-0.3.9/src/flask_vite/starter/postcss.config.js
--rw-r--r--   0        0        0       59 2023-07-04 08:17:31.233442 flask_vite-0.3.9/src/flask_vite/starter/src/styles.css
--rw-r--r--   0        0        0      157 2023-07-04 09:03:39.209131 flask_vite-0.3.9/src/flask_vite/starter/tailwind.config.js
--rw-r--r--   0        0        0      131 2023-07-04 08:17:31.234222 flask_vite-0.3.9/src/flask_vite/starter/vite.config.js
--rw-r--r--   0        0        0     1014 2024-04-26 16:27:24.908127 flask_vite-0.3.9/src/flask_vite/tags.py
--rw-r--r--   0        0        0      113 2024-04-26 16:14:35.052843 flask_vite-0.3.9/tests/__init__.py
--rw-r--r--   0        0        0     1317 2024-04-26 16:35:17.584356 flask_vite-0.3.9/tests/test_flask_vite.py
--rw-r--r--   0        0        0     5000 1970-01-01 00:00:00.000000 flask_vite-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0      144 2023-10-27 14:41:44.670623 flask_vite-0.4.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1074 2023-10-27 14:31:08.285369 flask_vite-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4335 2023-10-27 14:33:46.572110 flask_vite-0.4.0/README.md
+-rw-r--r--   0        0        0      999 2024-05-21 14:38:47.470982 flask_vite-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      157 2024-04-26 16:16:57.467495 flask_vite-0.4.0/src/flask_vite/__init__.py
+-rw-r--r--   0        0        0     1653 2024-04-26 16:25:38.956462 flask_vite-0.4.0/src/flask_vite/cli.py
+-rw-r--r--   0        0        0     1975 2024-05-21 14:35:58.177514 flask_vite-0.4.0/src/flask_vite/extension.py
+-rw-r--r--   0        0        0     1263 2024-04-26 16:34:32.184328 flask_vite-0.4.0/src/flask_vite/npm.py
+-rw-r--r--   0        0        0       50 2023-07-04 09:13:43.637994 flask_vite-0.4.0/src/flask_vite/starter/.gitignore
+-rwxr-xr-t   0        0        0    52227 2024-01-10 18:30:13.543461 flask_vite-0.4.0/src/flask_vite/starter/bun.lockb
+-rw-r--r--   0        0        0      280 2023-07-04 08:57:59.573627 flask_vite-0.4.0/src/flask_vite/starter/index.html
+-rw-r--r--   0        0        0       27 2023-07-04 09:14:53.281846 flask_vite-0.4.0/src/flask_vite/starter/main.js
+-rw-r--r--   0        0        0      360 2024-01-10 18:30:05.609248 flask_vite-0.4.0/src/flask_vite/starter/package.json
+-rw-r--r--   0        0        0       82 2023-07-04 09:05:39.738914 flask_vite-0.4.0/src/flask_vite/starter/postcss.config.js
+-rw-r--r--   0        0        0       59 2023-07-04 08:17:31.233442 flask_vite-0.4.0/src/flask_vite/starter/src/styles.css
+-rw-r--r--   0        0        0      157 2023-07-04 09:03:39.209131 flask_vite-0.4.0/src/flask_vite/starter/tailwind.config.js
+-rw-r--r--   0        0        0      131 2023-07-04 08:17:31.234222 flask_vite-0.4.0/src/flask_vite/starter/vite.config.js
+-rw-r--r--   0        0        0     1014 2024-04-26 16:27:24.908127 flask_vite-0.4.0/src/flask_vite/tags.py
+-rw-r--r--   0        0        0      113 2024-04-26 16:14:35.052843 flask_vite-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1317 2024-04-26 16:35:17.584356 flask_vite-0.4.0/tests/test_flask_vite.py
+-rw-r--r--   0        0        0     5000 1970-01-01 00:00:00.000000 flask_vite-0.4.0/PKG-INFO
```

### Comparing `flask_vite-0.3.9/LICENSE` & `flask_vite-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_vite-0.3.9/README.md` & `flask_vite-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `flask_vite-0.3.9/pyproject.toml` & `flask_vite-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask-vite"
-version = "0.3.9"
+version = "0.4.0"
 homepage = "https://github.com/abilian/flask-vite"
 description = "Flask+Vite integration."
 authors = ["Abilian SAS <contact@abilian.com>"]
 readme = "README.md"
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

### Comparing `flask_vite-0.3.9/src/flask_vite/cli.py` & `flask_vite-0.4.0/src/flask_vite/cli.py`

 * *Files identical despite different names*

### Comparing `flask_vite-0.3.9/src/flask_vite/extension.py` & `flask_vite-0.4.0/src/flask_vite/extension.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             raise RuntimeError(
                 "This extension is already registered on this Flask app."
             )
 
         app.extensions["vite"] = self
 
         config = app.config
-        if config.get("VITE_AUTO_INSERT", True):
+        if config.get("VITE_AUTO_INSERT", False):
             app.after_request(self.after_request)
 
         npm_bin_path = config.get("VITE_NPM_BIN_PATH", "npm")
         self.npm = NPM(cwd=str(self._get_root()), npm_bin_path=npm_bin_path)
 
         app.route("/_vite/<path:filename>")(self.vite_static)
         app.template_global("vite_tags")(make_tag)
```

### Comparing `flask_vite-0.3.9/src/flask_vite/npm.py` & `flask_vite-0.4.0/src/flask_vite/npm.py`

 * *Files identical despite different names*

### Comparing `flask_vite-0.3.9/src/flask_vite/starter/bun.lockb` & `flask_vite-0.4.0/src/flask_vite/starter/bun.lockb`

 * *Files identical despite different names*

### Comparing `flask_vite-0.3.9/src/flask_vite/tags.py` & `flask_vite-0.4.0/src/flask_vite/tags.py`

 * *Files identical despite different names*

### Comparing `flask_vite-0.3.9/tests/test_flask_vite.py` & `flask_vite-0.4.0/tests/test_flask_vite.py`

 * *Files identical despite different names*

### Comparing `flask_vite-0.3.9/PKG-INFO` & `flask_vite-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-vite
-Version: 0.3.9
+Version: 0.4.0
 Summary: Flask+Vite integration.
 Home-page: https://github.com/abilian/flask-vite
 Author: Abilian SAS
 Author-email: contact@abilian.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

