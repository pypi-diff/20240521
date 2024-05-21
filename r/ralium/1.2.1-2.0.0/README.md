# Comparing `tmp/ralium-1.2.1.tar.gz` & `tmp/ralium-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralium-1.2.1.tar", last modified: Tue May 21 06:13:44 2024, max compression
+gzip compressed data, was "ralium-2.0.0.tar", last modified: Tue May 21 07:25:22 2024, max compression
```

## Comparing `ralium-1.2.1.tar` & `ralium-2.0.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 06:13:44.260386 ralium-1.2.1/
--rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-1.2.1/LICENSE
--rw-rw-rw-   0        0        0    41897 2024-05-21 06:13:44.258313 ralium-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-1.2.1/README.md
--rw-rw-rw-   0        0        0      970 2024-05-21 06:12:52.000000 ralium-1.2.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-21 06:13:44.236102 ralium-1.2.1/ralium/
--rw-rw-rw-   0        0        0      357 2024-05-21 05:00:06.000000 ralium-1.2.1/ralium/__init__.py
--rw-rw-rw-   0        0        0     2965 2024-05-21 06:12:56.000000 ralium-1.2.1/ralium/_util.py
--rw-rw-rw-   0        0        0     1170 2024-05-21 00:26:03.000000 ralium-1.2.1/ralium/_util.pyi
--rw-rw-rw-   0        0        0     7555 2024-05-21 04:21:31.000000 ralium-1.2.1/ralium/api.py
--rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-1.2.1/ralium/api.pyi
--rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-1.2.1/ralium/builtins.py
--rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-1.2.1/ralium/builtins.pyi
--rw-rw-rw-   0        0        0     8231 2024-05-21 06:11:47.000000 ralium-1.2.1/ralium/bundle.py
--rw-rw-rw-   0        0        0     1581 2024-05-21 00:26:03.000000 ralium-1.2.1/ralium/bundle.pyi
--rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-1.2.1/ralium/config.py
--rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-1.2.1/ralium/config.pyi
--rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-1.2.1/ralium/element.py
--rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-1.2.1/ralium/element.pyi
--rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-1.2.1/ralium/engine.py
--rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-1.2.1/ralium/engine.pyi
--rw-rw-rw-   0        0        0     1191 2024-05-21 00:26:03.000000 ralium-1.2.1/ralium/errors.py
--rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-1.2.1/ralium/listener.py
--rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-1.2.1/ralium/listener.pyi
--rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-1.2.1/ralium/navigation.py
--rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-1.2.1/ralium/navigation.pyi
--rw-rw-rw-   0        0        0     7851 2024-05-21 05:23:35.000000 ralium-1.2.1/ralium/setuptools.py
--rw-rw-rw-   0        0        0      965 2024-05-21 05:19:13.000000 ralium-1.2.1/ralium/setuptools.pyi
--rw-rw-rw-   0        0        0     6936 2024-05-21 00:26:03.000000 ralium-1.2.1/ralium/webpage.py
--rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-1.2.1/ralium/webpage.pyi
--rw-rw-rw-   0        0        0     6031 2024-05-21 00:25:27.000000 ralium-1.2.1/ralium/window.py
--rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-1.2.1/ralium/window.pyi
-drwxrwxrwx   0        0        0        0 2024-05-21 06:13:44.257244 ralium-1.2.1/ralium.egg-info/
--rw-rw-rw-   0        0        0    41897 2024-05-21 06:13:44.000000 ralium-1.2.1/ralium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      657 2024-05-21 06:13:44.000000 ralium-1.2.1/ralium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 06:13:44.000000 ralium-1.2.1/ralium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 06:13:44.000000 ralium-1.2.1/ralium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 06:13:44.000000 ralium-1.2.1/ralium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 06:13:44.260386 ralium-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 07:25:22.488338 ralium-2.0.0/
+-rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0    41897 2024-05-21 07:25:22.486256 ralium-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-2.0.0/README.md
+-rw-rw-rw-   0        0        0      970 2024-05-21 07:24:39.000000 ralium-2.0.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-21 07:25:22.464574 ralium-2.0.0/ralium/
+-rw-rw-rw-   0        0        0      357 2024-05-21 05:00:06.000000 ralium-2.0.0/ralium/__init__.py
+-rw-rw-rw-   0        0        0     2600 2024-05-21 07:24:48.000000 ralium-2.0.0/ralium/_util.py
+-rw-rw-rw-   0        0        0     1194 2024-05-21 06:24:20.000000 ralium-2.0.0/ralium/_util.pyi
+-rw-rw-rw-   0        0        0     7555 2024-05-21 04:21:31.000000 ralium-2.0.0/ralium/api.py
+-rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-2.0.0/ralium/api.pyi
+-rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-2.0.0/ralium/builtins.py
+-rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-2.0.0/ralium/builtins.pyi
+-rw-rw-rw-   0        0        0     8231 2024-05-21 06:11:47.000000 ralium-2.0.0/ralium/bundle.py
+-rw-rw-rw-   0        0        0     1581 2024-05-21 00:26:03.000000 ralium-2.0.0/ralium/bundle.pyi
+-rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-2.0.0/ralium/config.py
+-rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-2.0.0/ralium/config.pyi
+-rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-2.0.0/ralium/element.py
+-rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-2.0.0/ralium/element.pyi
+-rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-2.0.0/ralium/engine.py
+-rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-2.0.0/ralium/engine.pyi
+-rw-rw-rw-   0        0        0     1233 2024-05-21 06:18:29.000000 ralium-2.0.0/ralium/errors.py
+-rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-2.0.0/ralium/listener.py
+-rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-2.0.0/ralium/listener.pyi
+-rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-2.0.0/ralium/navigation.py
+-rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-2.0.0/ralium/navigation.pyi
+-rw-rw-rw-   0        0        0     4804 2024-05-21 07:20:43.000000 ralium-2.0.0/ralium/pyhtml.py
+-rw-rw-rw-   0        0        0      531 2024-05-21 07:20:26.000000 ralium-2.0.0/ralium/pyhtml.pyi
+-rw-rw-rw-   0        0        0     7851 2024-05-21 05:23:35.000000 ralium-2.0.0/ralium/setuptools.py
+-rw-rw-rw-   0        0        0      965 2024-05-21 05:19:13.000000 ralium-2.0.0/ralium/setuptools.pyi
+-rw-rw-rw-   0        0        0     6936 2024-05-21 00:26:03.000000 ralium-2.0.0/ralium/webpage.py
+-rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-2.0.0/ralium/webpage.pyi
+-rw-rw-rw-   0        0        0     6078 2024-05-21 06:47:26.000000 ralium-2.0.0/ralium/window.py
+-rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-2.0.0/ralium/window.pyi
+drwxrwxrwx   0        0        0        0 2024-05-21 07:25:22.484251 ralium-2.0.0/ralium.egg-info/
+-rw-rw-rw-   0        0        0    41897 2024-05-21 07:25:22.000000 ralium-2.0.0/ralium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2024-05-21 07:25:22.000000 ralium-2.0.0/ralium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 07:25:22.000000 ralium-2.0.0/ralium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 07:25:22.000000 ralium-2.0.0/ralium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 07:25:22.000000 ralium-2.0.0/ralium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 07:25:22.488338 ralium-2.0.0/setup.cfg
```

### Comparing `ralium-1.2.1/LICENSE` & `ralium-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/PKG-INFO` & `ralium-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 1.2.1
+Version: 2.0.0
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-1.2.1/pyproject.toml` & `ralium-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools >= 69.5.0", "wheel >= 0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ralium"
-version = "1.2.1"
+version = "2.0.0"
 description = "An easy to use wrapper for pywebview."
 readme = "README.md"
 authors = [{ name = "Isaiah Coroama", email = "coroamaisaiah@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

### Comparing `ralium-1.2.1/ralium/_util.py` & `ralium-2.0.0/ralium/_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 import http.server
-
 import platform
 import ctypes
 import winreg
 import sys
 import os
 
 __all__ = [
-    "__version__",
-    "BasicHTTPServer", "_get_http_server_handler", "_get_bundle", "_norm_url", "_check_exists", 
-    "_check_is_dir", "_get_path_limit", "_read_file", "_get_path", "_is_markup_filelike"
+    "__version__", "BasicHTTPServer", "NamedDict", "_get_http_server_handler", "_get_bundle", 
+    "_norm_url", "_check_exists",  "_check_is_dir", "_get_path_limit", "_read_file", "_get_path"
 ]
 
-__version__ = "1.2.1"
+__version__ = "2.0.0"
 
 SYS_BUNDLE_ATTRIBUTE = "bundled"
 
 class BasicHTTPServer(http.server.SimpleHTTPRequestHandler):
     pass
 
+class NamedDict(dict):
+    def __init__(self, iterable):
+        for key, value in iterable.items():
+            if isinstance(value, dict):
+                self[key] = NamedDict(value)
+                continue
+
+            self[key] = value
+
 def _get_bundle():
     return getattr(sys, SYS_BUNDLE_ATTRIBUTE, None)
 
 def _get_http_server_handler():
     if _get_bundle() is not None:
         import ralium.bundle
         return ralium.bundle.BundledHTTPServer
@@ -83,24 +90,8 @@
 
     if bundle is not None:
         return os.path.normpath(path)
 
     if getattr(sys, "frozen", False):
         return os.path.abspath(os.path.join(sys._MEIPASS, path))
 
-    return os.path.abspath(path)
-
-# A copy of the 'BeautifulSoup._markup_resembles_filename' function
-def _is_markup_filelike(markup):
-    path_characters = '/\\'
-    extensions = ['.html', '.htm', '.xml', '.xhtml', '.txt']
-    if isinstance(markup, bytes):
-        path_characters = path_characters.encode("utf8")
-        extensions = [x.encode('utf8') for x in extensions]
-    filelike = False
-    if any(x in markup for x in path_characters):
-        filelike = True
-    else:
-        lower = markup.lower()
-        if any(lower.endswith(ext) for ext in extensions):
-            filelike = True
-    return filelike
+    return os.path.abspath(path)
```

### Comparing `ralium-1.2.1/ralium/_util.pyi` & `ralium-2.0.0/ralium/_util.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -13,31 +13,32 @@
     FunctionType, 
     ModuleType
 )
 
 import http.server
 
 __all__ = [
-    "__version__",
-    "BasicHTTPServer", "_get_http_server_handler", "_get_bundle", "_norm_url", "_check_exists", 
-    "_check_is_dir", "_get_path_limit", "_read_file", "_get_path", "_is_markup_filelike"
+    "__version__", "BasicHTTPServer", "NamedDict", "_get_http_server_handler", "_get_bundle", 
+    "_norm_url", "_check_exists",  "_check_is_dir", "_get_path_limit", "_read_file", "_get_path"
 ]
 
 __version__: str
 
 _RT = TypeVar("_RT") # Return Type
 ClassType: TypeAlias = object
 DirPathStr: TypeAlias = str
 FilePathStr: TypeAlias = str
 
 class BasicHTTPServer(http.server.SimpleHTTPRequestHandler): ...
 
+class NamedDict(dict):
+    def __init__(self, iterable: dict[str, Any]) -> None: ...
+
 def _get_bundle() -> FileSystem | None: ...
 def _get_http_server_handler() -> BasicHTTPServer | BundledHTTPServer: ...
 def _check_exists(path: str) -> bool: ...
 def _check_is_dir(path: str) -> bool: ...
 def _norm_url(path: str) -> str: ...
 def _get_path_limit_winreg() -> int: ...
 def _get_path_limit() -> int: ...
 def _read_file(path: str, encoding: str = "UTF-8") -> str: ...
-def _get_path(path: str) -> str: ...
-def _is_markup_filelike(markup: str) -> bool: ...
+def _get_path(path: str) -> str: ...
```

### Comparing `ralium-1.2.1/ralium/api.py` & `ralium-2.0.0/ralium/api.py`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/api.pyi` & `ralium-2.0.0/ralium/api.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/builtins.py` & `ralium-2.0.0/ralium/builtins.py`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/builtins.pyi` & `ralium-2.0.0/ralium/builtins.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/bundle.py` & `ralium-2.0.0/ralium/bundle.py`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/bundle.pyi` & `ralium-2.0.0/ralium/bundle.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/config.py` & `ralium-2.0.0/ralium/config.py`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/element.py` & `ralium-2.0.0/ralium/element.py`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/element.pyi` & `ralium-2.0.0/ralium/element.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/engine.py` & `ralium-2.0.0/ralium/engine.py`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/engine.pyi` & `ralium-2.0.0/ralium/engine.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/errors.py` & `ralium-2.0.0/ralium/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 global __RALIUM_WARNING_MESSAGES__
 __RALIUM_WARNING_MESSAGES__ = True
 
 class SetupError(Exception): pass
 class WindowLoadError(Exception): pass
 class BridgeEventError(Exception): pass
+class PyHTMLSyntaxError(Exception): pass
 class FilePathLimitError(Exception): pass
 class RegistryNotFoundError(Exception): pass
 class WindowNotRunningError(Exception): pass
 
 class WebFunctionApiError(Exception): pass
 
 class WebHookNotFoundError(Exception): pass
```

### Comparing `ralium-1.2.1/ralium/listener.py` & `ralium-2.0.0/ralium/listener.py`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/listener.pyi` & `ralium-2.0.0/ralium/listener.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/navigation.py` & `ralium-2.0.0/ralium/navigation.py`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/setuptools.py` & `ralium-2.0.0/ralium/setuptools.py`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/setuptools.pyi` & `ralium-2.0.0/ralium/setuptools.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/webpage.py` & `ralium-2.0.0/ralium/webpage.py`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/webpage.pyi` & `ralium-2.0.0/ralium/webpage.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium/window.py` & `ralium-2.0.0/ralium/window.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ralium.navigation import WindowNavigation
 from ralium.listener import ClassListener
 from ralium.webpage import WebHookDict, HTML_TEMPLATE
 from ralium.config import WindowConfig
 from ralium.engine import WebEngine
+from ralium.pyhtml import PyHTML
 import ralium.builtins
 
 from ralium.errors import (
     WebHookHomepageError, 
     WindowNotRunningError
 )
 
@@ -144,15 +145,15 @@
         
         for namespace in webhook.namespaces:
             self.engine.bridge.new(namespace)
 
             for function in namespace.values():
                 self.engine.functions.add_function(function)
         
-        html = BeautifulSoup(webhook.html, features="lxml")
+        html = BeautifulSoup(PyHTML(webhook).compile(), features="lxml")
         webhook.elements = [create_ralium_id(element) for element in html.body.find_all()]
 
         create_element(html, "base", {"href": str(self.engine)})
         create_element(html, "script", string=str(self.engine.bridge))
         create_element(html, "style", string=webhook.css)
 
         self.render(html)
```

### Comparing `ralium-1.2.1/ralium/window.pyi` & `ralium-2.0.0/ralium/window.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.2.1/ralium.egg-info/PKG-INFO` & `ralium-2.0.0/ralium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 1.2.1
+Version: 2.0.0
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-1.2.1/ralium.egg-info/SOURCES.txt` & `ralium-2.0.0/ralium.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 ralium/engine.py
 ralium/engine.pyi
 ralium/errors.py
 ralium/listener.py
 ralium/listener.pyi
 ralium/navigation.py
 ralium/navigation.pyi
+ralium/pyhtml.py
+ralium/pyhtml.pyi
 ralium/setuptools.py
 ralium/setuptools.pyi
 ralium/webpage.py
 ralium/webpage.pyi
 ralium/window.py
 ralium/window.pyi
 ralium.egg-info/PKG-INFO
```

