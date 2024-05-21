# Comparing `tmp/appxf-0.0.1.tar.gz` & `tmp/appxf-0.0.2.tar.gz`

## Comparing `appxf-0.0.1.tar` & `appxf-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 appxf-0.0.1/requirements.txt
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 appxf-0.0.1/src/appxf/__init__.py
--rw-r--r--   0        0        0     7545 2020-02-02 00:00:00.000000 appxf-0.0.1/src/appxf/fileversions.py
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 appxf-0.0.1/src/appxf/logging.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 appxf-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 appxf-0.0.1/LICENSE
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 appxf-0.0.1/README.md
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 appxf-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 appxf-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 appxf-0.0.2/requirements.txt
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 appxf-0.0.2/src/appxf/__init__.py
+-rw-r--r--   0        0        0     7545 2020-02-02 00:00:00.000000 appxf-0.0.2/src/appxf/fileversions.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 appxf-0.0.2/src/appxf/logging.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 appxf-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 appxf-0.0.2/LICENSE
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 appxf-0.0.2/README.md
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 appxf-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 appxf-0.0.2/PKG-INFO
```

### Comparing `appxf-0.0.1/src/appxf/fileversions.py` & `appxf-0.0.2/src/appxf/fileversions.py`

 * *Files identical despite different names*

### Comparing `appxf-0.0.1/src/appxf/logging.py` & `appxf-0.0.2/src/appxf/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         '%H:%M:%S')
 
 console_handler = logging.StreamHandler(stream=sys.stdout)
 console_handler.setLevel(logging.DEBUG)
 console_handler.setFormatter(console_formatter)
 
 
-def activate_logging(app_scope: str | None = None,
+def activate_logging(app_scope: list[str] | str | None = None,
                      directory: str = './data',
                      n_files: int = 5):
     ''' Activate logging for application
 
     It sets up logging to console and file logging (default: into
     ./data/log_yyyyMMdd_00.log). For appxf and the scope of your application
     down to debug level, for the root logger only warning and info.
@@ -77,23 +77,26 @@
     logging.getLogger('root').addHandler(file_handler)
 
     appxf_logger = logging.getLogger('appxf')
     appxf_logger.addHandler(console_handler)
     appxf_logger.addHandler(file_handler)
     appxf_logger.setLevel(logging.DEBUG)
     appxf_logger.propagate = False
-    appxf_logger.debug('start logging')
+    appxf_logger.debug('start logging (appxf)')
 
     if app_scope is not None:
-        app_logger = logging.getLogger(app_scope)
-        app_logger.addHandler(console_handler)
-        app_logger.addHandler(file_handler)
-        app_logger.setLevel(logging.DEBUG)
-        app_logger.propagate = False
-        app_logger.debug('start logging')
+        if isinstance(app_scope, str):
+            app_scope = [app_scope]
+        for this_scope in app_scope:
+            app_logger = logging.getLogger(this_scope)
+            app_logger.addHandler(console_handler)
+            app_logger.addHandler(file_handler)
+            app_logger.setLevel(logging.DEBUG)
+            app_logger.propagate = False
+            app_logger.debug(f'start logging ({this_scope})')
 
 
 def cleanup(directory: str, n_files: int = 5):
     ''' Cleanup log files
 
     This function is executed everytime you run activate_logging(). You should
     not need to call it yourself.
```

### Comparing `appxf-0.0.1/LICENSE` & `appxf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `appxf-0.0.1/pyproject.toml` & `appxf-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "appxf"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name = "alexander-rd", email="mail@alexander-rd.de" }
 ]
 description = "APPXF assists python applications (APP) by delivering the cross functional (XF) concerns "
 readme = "README.md"
 requires-python = ">=3.10"
 license_file = "LICENSE"
```

### Comparing `appxf-0.0.1/PKG-INFO` & `appxf-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.3
 Name: appxf
-Version: 0.0.1
+Version: 0.0.2
 Summary: APPXF assists python applications (APP) by delivering the cross functional (XF) concerns 
 Author-email: alexander-rd <mail@alexander-rd.de>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # APPXF
 
 APPXF covers cross functional concerns like configuration, persisting data,
 logging or security to limit the effort writing simple applications.
 
+__What it is:__ I transfer reusable parts into this package with a strong intend of
+the content being useful for others.
+
+__What it could be:__ With support from you, it could start closing a gap anyone
+needs to cross when writing even a small application to support small
+associations or non-profits.
+
 In Construction
 ===============
 The package is currently "in construction". Main concerns:
   * split from private sources to clarify licensing before publication
   * in the middle of a core feature increase to settle further interfaces
 Versions 0.0.x will cover this transitional phase. Target is a preliminary
 release as 0.1.0 where interfaces may still be unstable.
```

