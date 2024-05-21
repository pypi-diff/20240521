# Comparing `tmp/ralium-0.3.7.tar.gz` & `tmp/ralium-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralium-0.3.7.tar", last modified: Sun May 19 04:57:36 2024, max compression
+gzip compressed data, was "ralium-1.0.0.tar", last modified: Tue May 21 00:37:45 2024, max compression
```

## Comparing `ralium-0.3.7.tar` & `ralium-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 04:57:36.213642 ralium-0.3.7/
--rw-rw-rw-   0        0        0    35823 2024-04-24 23:35:07.000000 ralium-0.3.7/LICENSE
--rw-rw-rw-   0        0        0    41876 2024-05-19 04:57:36.212642 ralium-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0       52 2024-04-24 23:35:07.000000 ralium-0.3.7/README.md
--rw-rw-rw-   0        0        0     1018 2024-05-19 04:56:57.000000 ralium-0.3.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-19 04:57:36.196455 ralium-0.3.7/ralium/
--rw-rw-rw-   0        0        0      185 2024-05-13 23:24:25.000000 ralium-0.3.7/ralium/__init__.py
--rw-rw-rw-   0        0        0     1816 2024-05-14 21:40:48.000000 ralium-0.3.7/ralium/_util.py
--rw-rw-rw-   0        0        0      634 2024-05-14 21:32:03.000000 ralium-0.3.7/ralium/_util.pyi
--rw-rw-rw-   0        0        0     6579 2024-05-17 21:27:36.000000 ralium-0.3.7/ralium/api.py
--rw-rw-rw-   0        0        0     1066 2024-05-13 23:23:35.000000 ralium-0.3.7/ralium/api.pyi
--rw-rw-rw-   0        0        0      680 2024-05-02 17:00:29.000000 ralium-0.3.7/ralium/builtins.py
--rw-rw-rw-   0        0        0      541 2024-05-13 23:23:27.000000 ralium-0.3.7/ralium/builtins.pyi
--rw-rw-rw-   0        0        0     3332 2024-05-13 22:21:52.000000 ralium-0.3.7/ralium/config.py
--rw-rw-rw-   0        0        0      467 2024-05-01 22:26:47.000000 ralium-0.3.7/ralium/config.pyi
--rw-rw-rw-   0        0        0     6425 2024-05-19 04:49:38.000000 ralium-0.3.7/ralium/element.py
--rw-rw-rw-   0        0        0     1472 2024-05-19 04:55:59.000000 ralium-0.3.7/ralium/element.pyi
--rw-rw-rw-   0        0        0     4401 2024-05-13 21:17:30.000000 ralium-0.3.7/ralium/engine.py
--rw-rw-rw-   0        0        0     1389 2024-05-13 23:23:13.000000 ralium-0.3.7/ralium/engine.pyi
--rw-rw-rw-   0        0        0     1086 2024-05-16 17:41:03.000000 ralium-0.3.7/ralium/errors.py
--rw-rw-rw-   0        0        0     2387 2024-05-16 15:25:16.000000 ralium-0.3.7/ralium/listener.py
--rw-rw-rw-   0        0        0      890 2024-05-16 14:59:59.000000 ralium-0.3.7/ralium/listener.pyi
--rw-rw-rw-   0        0        0      804 2024-05-14 21:31:14.000000 ralium-0.3.7/ralium/navigation.py
--rw-rw-rw-   0        0        0      376 2024-04-29 20:44:02.000000 ralium-0.3.7/ralium/navigation.pyi
--rw-rw-rw-   0        0        0     3959 2024-05-17 20:30:24.000000 ralium-0.3.7/ralium/setup.py
--rw-rw-rw-   0        0        0      599 2024-05-17 20:30:43.000000 ralium-0.3.7/ralium/setup.pyi
--rw-rw-rw-   0        0        0     5738 2024-05-14 21:32:26.000000 ralium-0.3.7/ralium/webpage.py
--rw-rw-rw-   0        0        0     1250 2024-05-13 23:22:49.000000 ralium-0.3.7/ralium/webpage.pyi
--rw-rw-rw-   0        0        0     6031 2024-05-17 19:51:41.000000 ralium-0.3.7/ralium/window.py
--rw-rw-rw-   0        0        0      693 2024-05-16 17:42:01.000000 ralium-0.3.7/ralium/window.pyi
-drwxrwxrwx   0        0        0        0 2024-05-19 04:57:36.211631 ralium-0.3.7/ralium.egg-info/
--rw-rw-rw-   0        0        0    41876 2024-05-19 04:57:36.000000 ralium-0.3.7/ralium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2024-05-19 04:57:36.000000 ralium-0.3.7/ralium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 04:57:36.000000 ralium-0.3.7/ralium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-19 04:57:36.000000 ralium-0.3.7/ralium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-19 04:57:36.000000 ralium-0.3.7/ralium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 04:57:36.213642 ralium-0.3.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 00:37:45.942921 ralium-1.0.0/
+-rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0    41876 2024-05-21 00:37:45.940917 ralium-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-1.0.0/README.md
+-rw-rw-rw-   0        0        0     1018 2024-05-21 00:37:01.000000 ralium-1.0.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-21 00:37:45.916088 ralium-1.0.0/ralium/
+-rw-rw-rw-   0        0        0      383 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/__init__.py
+-rw-rw-rw-   0        0        0     2947 2024-05-21 00:30:56.000000 ralium-1.0.0/ralium/_util.py
+-rw-rw-rw-   0        0        0     1170 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/_util.pyi
+-rw-rw-rw-   0        0        0     7547 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/api.py
+-rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/api.pyi
+-rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/builtins.py
+-rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/builtins.pyi
+-rw-rw-rw-   0        0        0     8293 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/bundle.py
+-rw-rw-rw-   0        0        0     1581 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/bundle.pyi
+-rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/config.py
+-rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/config.pyi
+-rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/element.py
+-rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/element.pyi
+-rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/engine.py
+-rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/engine.pyi
+-rw-rw-rw-   0        0        0     1191 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/errors.py
+-rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/listener.py
+-rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/listener.pyi
+-rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/navigation.py
+-rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/navigation.pyi
+-rw-rw-rw-   0        0        0     5434 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/setup.py
+-rw-rw-rw-   0        0        0      699 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/setup.pyi
+-rw-rw-rw-   0        0        0     6936 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/webpage.py
+-rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/webpage.pyi
+-rw-rw-rw-   0        0        0     6031 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/window.py
+-rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/window.pyi
+drwxrwxrwx   0        0        0        0 2024-05-21 00:37:45.938830 ralium-1.0.0/ralium.egg-info/
+-rw-rw-rw-   0        0        0    41876 2024-05-21 00:37:45.000000 ralium-1.0.0/ralium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      647 2024-05-21 00:37:45.000000 ralium-1.0.0/ralium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 00:37:45.000000 ralium-1.0.0/ralium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-21 00:37:45.000000 ralium-1.0.0/ralium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 00:37:45.000000 ralium-1.0.0/ralium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 00:37:45.942921 ralium-1.0.0/setup.cfg
```

### Comparing `ralium-0.3.7/LICENSE` & `ralium-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ralium-0.3.7/PKG-INFO` & `ralium-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 0.3.7
+Version: 1.0.0
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-0.3.7/pyproject.toml` & `ralium-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools >= 69.5.0", "wheel >= 0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ralium"
-version = "0.3.7"
+version = "1.0.0"
 description = "An easy to use wrapper for pywebview."
 readme = "README.md"
 authors = [{ name = "Isaiah Coroama", email = "coroamaisaiah@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

### Comparing `ralium-0.3.7/ralium/_util.pyi` & `ralium-1.0.0/ralium/_util.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,43 @@
-from typing import TypeAlias, TypeVar, Callable, Any, Self, Literal
-from types import FunctionType, ModuleType
+from ralium.bundle import BundledHTTPServer, FileSystem
+
+from typing import (
+    TypeAlias, 
+    Callable, 
+    TypeVar, 
+    Literal,
+    Self, 
+    Any, 
+)
+
+from types import (
+    FunctionType, 
+    ModuleType
+)
+
 import http.server
 
-__all__ = ["BasicHTTPServer", "_norm_url", "_get_path_limit", "_get_path", "_is_markup_filelike"]
+__all__ = [
+    "__version__",
+    "BasicHTTPServer", "_get_http_server_handler", "_get_bundle", "_norm_url", "_check_exists", 
+    "_check_is_dir", "_get_path_limit", "_read_file", "_get_path", "_is_markup_filelike"
+]
+
+__version__: str
 
 _RT = TypeVar("_RT") # Return Type
 ClassType: TypeAlias = object
 DirPathStr: TypeAlias = str
 FilePathStr: TypeAlias = str
 
 class BasicHTTPServer(http.server.SimpleHTTPRequestHandler): ...
 
+def _get_bundle() -> FileSystem | None: ...
+def _get_http_server_handler() -> BasicHTTPServer | BundledHTTPServer: ...
+def _check_exists(path: str) -> bool: ...
+def _check_is_dir(path: str) -> bool: ...
 def _norm_url(path: str) -> str: ...
 def _get_path_limit_winreg() -> int: ...
 def _get_path_limit() -> int: ...
+def _read_file(path: str, encoding: str = "UTF-8") -> str: ...
 def _get_path(path: str) -> str: ...
 def _is_markup_filelike(markup: str) -> bool: ...
```

### Comparing `ralium-0.3.7/ralium/api.py` & `ralium-1.0.0/ralium/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,87 @@
 from ralium.webpage import WebHook, WebHookNamespace
 from ralium.config import WindowConfig
 from ralium.window import Window
 from ralium.errors import *
-from ralium._util import _get_path, _norm_url
+from ralium._util import (
+    _get_path, 
+    _norm_url, 
+    _read_file,
+    _check_exists,
+    _check_is_dir
+)
 
 from types import FunctionType, MethodType
 
 import inspect
+import sys
 import os
 
 RALIUM_API_REGISTRY_IDENTIFIER = "__ralium_registry__"
     
 def _check_web_folder(webfolder):
-    if not os.path.exists(webfolder):
+    if not _check_exists(webfolder):
         raise WebFolderNotFoundError("Web folder path does not exist.")
     
-    if not os.path.isdir(webfolder):
+    if not _check_is_dir(webfolder):
         raise WebFolderDirectoryError("Web folder must be a directory.")
 
 def _check_web_routes(webroutes):
-    if not os.path.exists(webroutes):
+    if not _check_exists(webroutes):
         raise WebRoutesNotFoundError("Web folder must contain a routes directory.")
     
-    if not os.path.isdir(webroutes):
+    if not _check_is_dir(webroutes):
         raise WebRoutesDirectoryError("Web folder routes must be a directory.")
 
 def _collect_global_css_files(webfolder):
     cssfiles = []
     cssfolder = os.path.join(webfolder, "styles")
 
-    if os.path.exists(cssfolder) and os.path.isdir(cssfolder):
+    if _check_exists(cssfolder) and _check_is_dir(cssfolder):
         for root, _, files in os.walk(webfolder):
             cssfiles.extend([os.path.join(root, file) for file in files if os.path.splitext(file)[-1] == ".css"])
     
     return cssfiles
 
 def _get_registry_contents(pyfile):
-    with open(pyfile, "r") as f:
-        content = f.read()
-    
     _globals = {}
-    exec(content, _globals)
+    exec(_read_file(pyfile), _globals)
 
     return _globals.get(RALIUM_API_REGISTRY_IDENTIFIER, [])
 
+def _bundle_collect_webhooks():
+    filesystem = getattr(sys, "bundled")
+
+    styles = [str(style) for style in filesystem.styles]
+    webhooks = []
+
+    for bundle in filesystem.bundles:
+        _styles = [str(style) for style in bundle.styles]
+        _styles.extend(styles)
+
+        _functions = []
+        _namespaces = []
+
+        if bundle.server is not None:
+            for item in _get_registry_contents(bundle.server.relpath):
+                if isinstance(item, WebHookNamespace):
+                    _namespaces.append(item)
+                    continue
+                
+                if isinstance(item, (FunctionType, MethodType,)):
+                    _functions.append(item)
+
+        webhooks.append(WebHook(bundle.url, str(bundle.page), _styles, _functions, _namespaces, (bundle.url == "/")))
+    
+    return webhooks
+
 def _collect_webhooks(webfolder, webroutes):
+    if getattr(sys, "bundled", None) is not None:
+        return _bundle_collect_webhooks()
+
     webhooks = []
     global_css = _collect_global_css_files(webfolder)
     root_split_string = os.path.join(os.path.basename(webfolder), "routes")
 
     for root, _, files in os.walk(webroutes):
         url = _norm_url(f"{root.split(root_split_string)[-1]}")
 
@@ -121,15 +154,15 @@
     webroutes = os.path.join(webfolder, "routes")
 
     _check_web_folder(webfolder)
     _check_web_routes(webroutes)
 
     webhooks = _collect_webhooks(webfolder, webroutes)
 
-    return Window(webhooks, config or WindowConfig())
+    return Window(webhooks, config)
 
 def register():
     """
     Creates a registry list to expose functions and namespaces for use within JavaScript.
 
     :returns: A decorator for exposing Python functions to JavaScript.
     """
```

### Comparing `ralium-0.3.7/ralium/api.pyi` & `ralium-1.0.0/ralium/api.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.7/ralium/builtins.py` & `ralium-1.0.0/ralium/builtins.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.7/ralium/builtins.pyi` & `ralium-1.0.0/ralium/builtins.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.7/ralium/config.py` & `ralium-1.0.0/ralium/config.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.7/ralium/element.py` & `ralium-1.0.0/ralium/element.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.7/ralium/element.pyi` & `ralium-1.0.0/ralium/element.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -14,19 +14,14 @@
     html: BeautifulSoup, 
     tag: HTMLElementStr, 
     setitems: dict[str] | None = None, 
     **setattrs: dict[str, Any]
 ) -> None: ...
 
 class JS:
-    class _RawStr(str): pass
-
-    @staticmethod
-    def raw(__value: str) -> _RawStr: ...
-
     @staticmethod
     def str(__value: str) -> str: ...
 
     true: Literal['"true"']
     false: Literal['"false"']
 
     @staticmethod
```

### Comparing `ralium-0.3.7/ralium/engine.py` & `ralium-1.0.0/ralium/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,18 @@
             new_calldata.append(HTMLElement(window, element_id, element))
             continue
 
         new_calldata.append(data)
     
     return new_calldata
 
+class WebApiFunctionDict(dict):
+    def add_function(self, function):
+        self[str(function)] = function
+
 class WebBridge:
     def __init__(self, *functions):
         self.bridges = []
         self.initial = "function bridge(func) {pywebview.api.bridge(func)};"
 
         for function in functions:
             self.new(function)
@@ -64,18 +68,14 @@
     def new(self, obj):
         if inspect.isfunction(obj) or inspect.ismethod(obj):
             return self.bridges.append(self._function_template(obj.__name__, str(obj)))
         
         if isinstance(obj, WebHookNamespace):
             return self.bridges.append(self._namespace_template(obj.name, **dict(obj.items())))
     
-class WebApiFunctionDict(dict):
-    def add_function(self, function):
-        self[str(function)] = function
-    
 class WebEngine:
     def __init__(self, window):
         self.port, worker = self._init_server()
         
         self.server = threading.Thread(target=worker, daemon=True)
         self.__running = threading.Event()
 
@@ -92,15 +92,15 @@
         return f"http://localhost:{self.port}/"
 
     @property
     def running(self):
         return not self.__running.is_set()
 
     def _init_server(self):
-        httpd = socketserver.TCPServer(("", 0,), _util.BasicHTTPServer)
+        httpd = socketserver.TCPServer(("", 0,), _util._get_http_server_handler())
         port = httpd.socket.getsockname()[1]
 
         def worker():
             while self.running:
                 httpd.handle_request()
             os._exit(0)
         
@@ -130,9 +130,8 @@
     def create_event(self):
         def BridgeEvent(function):
             if callable(function):
                 if not str(function) in self.functions:
                     self.functions.add_function(function)
                 return f"bridge('{str(function)}')"
             raise BridgeEventError("Event attribute is not a function.")
-        return BridgeEvent
-    
+        return BridgeEvent
```

### Comparing `ralium-0.3.7/ralium/engine.pyi` & `ralium-1.0.0/ralium/engine.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.7/ralium/errors.py` & `ralium-1.0.0/ralium/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 import warnings
 
 global __RALIUM_WARNING_MESSAGES__
 __RALIUM_WARNING_MESSAGES__ = True
 
+class SetupError(Exception): pass
 class WindowLoadError(Exception): pass
 class BridgeEventError(Exception): pass
 class FilePathLimitError(Exception): pass
 class RegistryNotFoundError(Exception): pass
 class WindowNotRunningError(Exception): pass
 
 class WebFunctionApiError(Exception): pass
-class WebFolderNotFoundError(Exception): pass
-class WebRoutesNotFoundError(Exception): pass
-class WebFolderDirectoryError(Exception): pass
-class WebRoutesDirectoryError(Exception): pass
 
 class WebHookNotFoundError(Exception): pass
 class WebHookHomepageError(Exception): pass
 
-class FrozenMemberExistsError(Exception): pass
+class WebFolderNotFoundError(Exception): pass
+class WebRoutesNotFoundError(Exception): pass
+
+class WebFolderDirectoryError(Exception): pass
+class WebRoutesDirectoryError(Exception): pass
 
 class FileNotFoundWarning(Warning): pass
+class FilePathLimitWarning(Warning): pass
 
 def DisableWarnings():
     """
     Disables Ralium warnings from being displayed.
     """
 
     global __RALIUM_WARNING_MESSAGES__
     __RALIUM_WARNING_MESSAGES__ = False
 
 def warn(message, warning, major = False):
+    return
+    if not __RALIUM_WARNING_MESSAGES__:
+        return
+
     if major:
         return warnings.warn(f"[Ralium]: {message}", warning)
+
     print(f"[Ralium] {warning.__name__}: {message}")
```

### Comparing `ralium-0.3.7/ralium/listener.py` & `ralium-1.0.0/ralium/listener.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.7/ralium/listener.pyi` & `ralium-1.0.0/ralium/listener.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.7/ralium/navigation.py` & `ralium-1.0.0/ralium/navigation.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.7/ralium/setup.py` & `ralium-1.0.0/ralium/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from ralium.errors import DisableWarnings
-import PyInstaller.__main__
+from PyInstaller.__main__ import logger, run as CompileExe
+from ralium.errors import DisableWarnings, SetupError
+from ralium.bundle import PyBundler
+from ralium._util import __version__
 import sys
 import os
 
 HTML_FILE_EXTENSIONS = [".htm", ".html"]
 FILE_EXTENSIONS = [*HTML_FILE_EXTENSIONS, ".css", ".py"]
 
 def _exe_str_error(name, var):
@@ -45,37 +47,73 @@
     
     return webfiles
 
 def setup(
     pyfile,
     name = None,
     icon = None,
-    onefile = True,
+    bundle = False,
+    webfolder = None,
     warnings = False,
+    onefile = True,
     noconsole = True,
-    webfolder = None,
+    bundle_dist = None,
     pyi_args = None
 ):
     """
-    Compiles a Ralium project using PyInstaller.
+    Compiles a Ralium project to an executable using PyInstaller.
 
     :param pyfile: Python file to compile.
     :param name: Display name for the executable.
     :param icon: Display icon for the executable.
-    :param onefile: Bundles the executable as a standalone file.
+    :param bundle: Bundles all of the html, css, python and image files into one executable. (Requires a `webfolder`)
+    :param webfolder: Directory of the project.
     :param warnings: Calls the `DisableWarnings` to prevent warnings.
+    :param onefile: Creates the executable as a standalone file.
     :param noconsole: Prevents a console from being displayed.
-    :param webfolder: Directory of the project.
+    :param bundle_dist: The directory name Ralium will use for bundling projects. (Default: `dist`)
     :param pyi_args: Extra parameters for PyInstaller to use.
 
     :raises TypeError: If the name or icon is not a `str` or `None`.
+    :raises SetupError: If bundle is `True` while the webfolder is `None`.
     :raises RuntimeError: If this function is called within an already compiled executable file.
     :raises FileNotFoundError: If a certain file path doesn't exist.
     """
 
+    logger.info("Ralium: %s", __version__)
+
+    if bundle:
+        if webfolder is None:
+            raise SetupError("Cannot bundle project without a webfolder.")
+
+        if bundle_dist is None:
+            bundle_dist = "dist"
+        
+        bundle_dist = os.path.abspath(bundle_dist)
+
+        if not os.path.exists(bundle_dist):
+            os.mkdir(bundle_dist)
+            logger.info("created %s", bundle_dist)
+
+        name, ext = os.path.splitext(os.path.basename(pyfile))
+        filename = os.path.join(bundle_dist, f"{name}.bundle{ext}")
+
+        logger.info("Bundling '%s' with project '%s'", pyfile, os.path.abspath(webfolder))
+
+        code = PyBundler(pyfile, webfolder).view()
+
+        if not warnings:
+            code.insert(0, b"import ralium.errors; ralium.errors.DisableWarnings()\n")
+
+        with open(filename, "wb") as f:
+            f.writelines(code)
+
+        logger.info("wrote %s", filename)
+        logger.info("Finished Bundling")
+
     if getattr(sys, "frozen", False):
         raise RuntimeError("Ralium setup cannot be ran from an executable file.")
     
     if not os.path.exists(pyfile):
         raise FileNotFoundError(f"Failed to find python file '{pyfile}'")
 
     args = [pyfile, *(pyi_args or [])]
@@ -100,12 +138,12 @@
     
     if not warnings:
         DisableWarnings()
     
     if noconsole:
         args.append(f"--noconsole")
     
-    if webfolder:
+    if webfolder and not bundle:
         for src, dst in collect_webfolder(webfolder).items():
             args.append(_add_data_arg(src, dst))
 
-    PyInstaller.__main__.run(args)
+    CompileExe(args)
```

### Comparing `ralium-0.3.7/ralium/setup.pyi` & `ralium-1.0.0/ralium/setup.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -12,12 +12,15 @@
 
 def collect_webfolder(webfolder: DirPathStr) -> dict[FilePathStr]: ...
 
 def setup(
     pyfile: FilePathStr,
     name: str | None = None,
     icon: FilePathStr | None = None,
+    bundle: bool = False,
+    webfolder: DirPathStr | None = None,
+    warnings: bool = False,
     onefile: bool = True,
     noconsole: bool = True,
-    webfolder: DirPathStr | None = None,
+    bundle_dist: DirPathStr | None = None,
     pyi_args: list[str] | None = None
 ) -> None: ...
```

### Comparing `ralium-0.3.7/ralium/webpage.py` & `ralium-1.0.0/ralium/webpage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from ralium.errors import *
 from ralium._util import *
 import inspect
-import os
 
 HTML_TEMPLATE = """<!DOCTYPE html>
 <html>
 <head lang="en">
 <meta charset="UTF-8">
 </head>
 <body>
@@ -29,28 +28,43 @@
         self._read()
         return self.__data
     
     def _read(self):
         if self.__read:
             return
 
-        if not os.path.exists(self.__data):
+        if not _check_exists(self.__data):
             return warn(f"Failed to load file with path: '{self.__data}'", FileNotFoundWarning, True)
         
-        with open(_get_path(self.__data), "r", encoding=self.__encoding) as f:
-            self.__data = f.read()
-            self.__read = True
+        self.__data = _read_file(_get_path(self.__data), self.__encoding)
+        self.__read = True
 
 class CSSReader:
     def __init__(self, *files, encoding):
-        self.__readers = [FileReader(file, encoding) for file in files if len(file) <= _get_path_limit()]
+        self.__readers = []
+
+        for file in files:
+            if _check_exists(file):
+                if len(file) <= _get_path_limit():
+                    warn(f"File '{file}' exceeds path limit.", FilePathLimitWarning, major=True)
+                
+                self.__readers.append(FileReader(file, encoding))
+                continue
+
+            self.__readers.append(file)
 
     @property
     def content(self):
-        return "\n".join([reader.content for reader in self.__readers])
+        items = []
+        for reader in self.__readers:
+            if isinstance(reader, FileReader):
+                items.append(reader.content)
+                continue
+            items.append(reader)
+        return "\n".join(items)
 
 class WebHookNamespace(dict):
     def __init__(self, name, *functions, **named_functions):
         self.name = name
 
         self.add_functions(*functions)
         self.add_named_functions(**named_functions)
@@ -114,23 +128,25 @@
         self._get_html()
         self._get_css()
     
     def __repr__(self):
         return f"WebHook(url='{self.url}')"
     
     def _get_html(self):
-        if not _is_markup_filelike(self.html): return
+        if not _check_exists(self.html): return
         self.html = FileReader(self.html, self.encoding).content
     
     def _get_css(self):
         if isinstance(self.css, (list, tuple, set,)):
-            self.css = CSSReader(*self.css, encoding=self.encoding).content
+            files = [item for item in self.css if _check_exists(item)]
+            values = [item for item in self.css if not _check_exists(item)]
+            self.css = "\n".join([CSSReader(*files, encoding=self.encoding).content, *values])
             return
         
-        if isinstance(self.css, str) and _is_markup_filelike(self.css):
+        if isinstance(self.css, (str, bytes,)) and _check_exists(self.css):
             self.css = CSSReader(self.css, encoding=self.encoding).content
     
     def _wrap_functions(self):
         if self.window is None:
             return
 
         self.functions = [WebHookFunction(function, self.window) for function in self.functions]
@@ -160,8 +176,26 @@
     
     def get(self, url):
         webhook = super().get(url, None)
 
         if webhook is None:
             raise WebHookNotFoundError(f"Failed to find WebHook for the url '{url}'")
 
-        return webhook
+        return webhook
+
+def create_namespace(name, *functions, **named_functions):
+    """
+    Creates a `Namespace` to use within JavaScript.
+
+    :param name: The alias the namespace is accessed by.
+    :param functions: A list of functions to add.
+    :param named_functions: A dictionary of functions to add.
+
+    :returns: A `WebHookNamespace` object.
+
+    The names of the regularly listed functions will be the value
+    of the `__name__` property of the function objects.
+
+    The names of the named function dictionary will be the keyword part.
+    """
+
+    return WebHookNamespace(name, *functions, **named_functions)
```

### Comparing `ralium-0.3.7/ralium/webpage.pyi` & `ralium-1.0.0/ralium/webpage.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ralium.window import Window
+from ralium._util import FunctionType
 from typing import Iterator
 import os
 
 HTML_TEMPLATE: str
 
 class FileReader:
     def __init__(self, file: str | os.PathLike, encoding: str) -> None: ...
@@ -11,31 +12,48 @@
     def _read(self) -> None: ...
 
 class CSSReader:
     def __init__(self, *files: list[str | os.PathLike], encoding: str) -> None: ...
     @property
     def content(self) -> str: None
 
+class WebHookNamespace(dict):
+    def __init__(self, 
+        name: str, 
+        *functions: tuple[FunctionType], 
+        **named_functions: dict[str, FunctionType]
+    ) -> None: ...
+
+    def add_functions(self, *functions: tuple[FunctionType]) -> None: ...
+    def add_named_functions(self, **functions: dict[str, FunctionType]) -> None: ...
+
 class WebHookFunction:
-    def __new__(cls, function: function, window: Window) -> function: ...
+    def __new__(cls, function: FunctionType, window: Window) -> function: ...
 
 class WebHook:
     def __init__(self, 
         url: str, 
         html: str | os.PathLike, 
         css: str | list[str] | None = None, 
-        functions: list[function] | None = None, 
+        functions: list[FunctionType] | None = None, 
+        namespaces: list[WebHookNamespace] | None = None,
         homepage: bool = False, 
         encoding: str = "UTF-8"
     ) -> None: ...
     def __repr__(self) -> str: ...
     
     def _get_html(self) -> None: ...
     def _get_css(self) -> None: ...
     def _wrap_functions(self) -> None: ...
     def set_window(self, window: Window) -> None: ...
 
 class WebHookDict(dict):
     def __init__(self, webhooks: list[WebHook]) -> None: ...
     def __repr__(self) -> str: ...
     def __iter__(self) -> Iterator[tuple]: ...
-    def get(self, url: str) -> WebHook: ...
+    def get(self, url: str) -> WebHook: ...
+
+def create_namespace(
+    name: str, 
+    *functions: tuple[FunctionType], 
+    **named_functions: dict[str, FunctionType]
+) -> WebHookNamespace: ...
```

### Comparing `ralium-0.3.7/ralium/window.py` & `ralium-1.0.0/ralium/window.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.7/ralium/window.pyi` & `ralium-1.0.0/ralium/window.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.7/ralium.egg-info/PKG-INFO` & `ralium-1.0.0/ralium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 0.3.7
+Version: 1.0.0
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-0.3.7/ralium.egg-info/SOURCES.txt` & `ralium-1.0.0/ralium.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 ralium/__init__.py
 ralium/_util.py
 ralium/_util.pyi
 ralium/api.py
 ralium/api.pyi
 ralium/builtins.py
 ralium/builtins.pyi
+ralium/bundle.py
+ralium/bundle.pyi
 ralium/config.py
 ralium/config.pyi
 ralium/element.py
 ralium/element.pyi
 ralium/engine.py
 ralium/engine.pyi
 ralium/errors.py
```

