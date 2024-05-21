# Comparing `tmp/ralium-1.0.1.tar.gz` & `tmp/ralium-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralium-1.0.1.tar", last modified: Tue May 21 00:41:39 2024, max compression
+gzip compressed data, was "ralium-1.1.0.tar", last modified: Tue May 21 04:31:12 2024, max compression
```

## Comparing `ralium-1.0.1.tar` & `ralium-1.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 00:41:39.277462 ralium-1.0.1/
--rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    41876 2024-05-21 00:41:39.276018 ralium-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-1.0.1/README.md
--rw-rw-rw-   0        0        0      958 2024-05-21 00:40:52.000000 ralium-1.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-21 00:41:39.256858 ralium-1.0.1/ralium/
--rw-rw-rw-   0        0        0      383 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/__init__.py
--rw-rw-rw-   0        0        0     2947 2024-05-21 00:40:35.000000 ralium-1.0.1/ralium/_util.py
--rw-rw-rw-   0        0        0     1170 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/_util.pyi
--rw-rw-rw-   0        0        0     7547 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/api.py
--rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/api.pyi
--rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/builtins.py
--rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/builtins.pyi
--rw-rw-rw-   0        0        0     8293 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/bundle.py
--rw-rw-rw-   0        0        0     1581 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/bundle.pyi
--rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/config.py
--rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/config.pyi
--rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/element.py
--rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/element.pyi
--rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/engine.py
--rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/engine.pyi
--rw-rw-rw-   0        0        0     1191 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/errors.py
--rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/listener.py
--rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/listener.pyi
--rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/navigation.py
--rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/navigation.pyi
--rw-rw-rw-   0        0        0     5463 2024-05-21 00:39:16.000000 ralium-1.0.1/ralium/setup.py
--rw-rw-rw-   0        0        0      699 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/setup.pyi
--rw-rw-rw-   0        0        0     6936 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/webpage.py
--rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/webpage.pyi
--rw-rw-rw-   0        0        0     6031 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/window.py
--rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/window.pyi
-drwxrwxrwx   0        0        0        0 2024-05-21 00:41:39.274919 ralium-1.0.1/ralium.egg-info/
--rw-rw-rw-   0        0        0    41876 2024-05-21 00:41:39.000000 ralium-1.0.1/ralium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      647 2024-05-21 00:41:39.000000 ralium-1.0.1/ralium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 00:41:39.000000 ralium-1.0.1/ralium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-21 00:41:39.000000 ralium-1.0.1/ralium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 00:41:39.000000 ralium-1.0.1/ralium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 00:41:39.278785 ralium-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 04:31:12.642890 ralium-1.1.0/
+-rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0    41897 2024-05-21 04:31:12.641622 ralium-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-1.1.0/README.md
+-rw-rw-rw-   0        0        0      970 2024-05-21 04:30:23.000000 ralium-1.1.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-21 04:31:12.616269 ralium-1.1.0/ralium/
+-rw-rw-rw-   0        0        0      383 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/__init__.py
+-rw-rw-rw-   0        0        0     2965 2024-05-21 04:28:49.000000 ralium-1.1.0/ralium/_util.py
+-rw-rw-rw-   0        0        0     1170 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/_util.pyi
+-rw-rw-rw-   0        0        0     7555 2024-05-21 04:21:31.000000 ralium-1.1.0/ralium/api.py
+-rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/api.pyi
+-rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/builtins.py
+-rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/builtins.pyi
+-rw-rw-rw-   0        0        0     8321 2024-05-21 04:14:13.000000 ralium-1.1.0/ralium/bundle.py
+-rw-rw-rw-   0        0        0     1581 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/bundle.pyi
+-rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/config.py
+-rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/config.pyi
+-rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/element.py
+-rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/element.pyi
+-rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/engine.py
+-rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/engine.pyi
+-rw-rw-rw-   0        0        0     1191 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/errors.py
+-rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/listener.py
+-rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/listener.pyi
+-rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/navigation.py
+-rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/navigation.pyi
+-rw-rw-rw-   0        0        0     6017 2024-05-21 04:03:11.000000 ralium-1.1.0/ralium/setup.py
+-rw-rw-rw-   0        0        0      699 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/setup.pyi
+-rw-rw-rw-   0        0        0     6936 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/webpage.py
+-rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/webpage.pyi
+-rw-rw-rw-   0        0        0     6031 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/window.py
+-rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/window.pyi
+drwxrwxrwx   0        0        0        0 2024-05-21 04:31:12.639589 ralium-1.1.0/ralium.egg-info/
+-rw-rw-rw-   0        0        0    41897 2024-05-21 04:31:12.000000 ralium-1.1.0/ralium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      647 2024-05-21 04:31:12.000000 ralium-1.1.0/ralium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 04:31:12.000000 ralium-1.1.0/ralium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 04:31:12.000000 ralium-1.1.0/ralium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 04:31:12.000000 ralium-1.1.0/ralium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 04:31:12.642890 ralium-1.1.0/setup.cfg
```

### Comparing `ralium-1.0.1/LICENSE` & `ralium-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/PKG-INFO` & `ralium-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 1.0.1
+Version: 1.1.0
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,10 +685,11 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4
 Requires-Dist: pyinstaller
 Requires-Dist: pywebview
+Requires-Dist: lxml
 
 # Ralium
 A pywebview wrapper inspired by Neutron.
```

### Comparing `ralium-1.0.1/pyproject.toml` & `ralium-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires      = ["setuptools >= 69.5.0", "wheel >= 0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ralium"
-version = "1.0.1"
+version = "1.1.0"
 description = "An easy to use wrapper for pywebview."
 readme = "README.md"
 authors = [{ name = "Isaiah Coroama", email = "coroamaisaiah@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Programming Language :: Python :: 3.12',
 ]
 keywords = ["gui", "webkit", "ralium", "windows", "html", "web", "isaiah", "coroama"]
 dependencies = [
     "beautifulsoup4",
     "pyinstaller",
     "pywebview",
+    "lxml"
 ]
 
 requires-python = ">3.9"
 
 [project.urls]
 Homepage = "https://github.com/IsaiahCoroama/Ralium"
```

### Comparing `ralium-1.0.1/ralium/_util.py` & `ralium-1.1.0/ralium/_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 __all__ = [
     "__version__",
     "BasicHTTPServer", "_get_http_server_handler", "_get_bundle", "_norm_url", "_check_exists", 
     "_check_is_dir", "_get_path_limit", "_read_file", "_get_path", "_is_markup_filelike"
 ]
 
-__version__ = "1.0.1"
+__version__ = "1.1.0"
 
 SYS_BUNDLE_ATTRIBUTE = "bundled"
 
 class BasicHTTPServer(http.server.SimpleHTTPRequestHandler):
     pass
 
 def _get_bundle():
@@ -28,15 +28,15 @@
         return ralium.bundle.BundledHTTPServer
     return BasicHTTPServer
 
 def _check_exists(path):
     bundle = _get_bundle()
 
     if bundle is not None:
-        if path in ["\\", "\\routes"]: return True
+        if path in ["\\template", "\\template\\routes"]: return True
         return bundle.get(path, False)
     
     return os.path.exists(path)
 
 def _check_is_dir(path):
     bundle = _get_bundle()
```

### Comparing `ralium-1.0.1/ralium/_util.pyi` & `ralium-1.1.0/ralium/_util.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/api.py` & `ralium-1.1.0/ralium/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from ralium.config import WindowConfig
 from ralium.window import Window
 from ralium.errors import *
 from ralium._util import (
     _get_path, 
     _norm_url, 
     _read_file,
+    _get_bundle,
     _check_exists,
     _check_is_dir
 )
 
 from types import FunctionType, MethodType
 
 import inspect
@@ -45,15 +46,15 @@
 def _get_registry_contents(pyfile):
     _globals = {}
     exec(_read_file(pyfile), _globals)
 
     return _globals.get(RALIUM_API_REGISTRY_IDENTIFIER, [])
 
 def _bundle_collect_webhooks():
-    filesystem = getattr(sys, "bundled")
+    filesystem = _get_bundle()
 
     styles = [str(style) for style in filesystem.styles]
     webhooks = []
 
     for bundle in filesystem.bundles:
         _styles = [str(style) for style in bundle.styles]
         _styles.extend(styles)
```

### Comparing `ralium-1.0.1/ralium/api.pyi` & `ralium-1.1.0/ralium/api.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/builtins.py` & `ralium-1.1.0/ralium/builtins.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/builtins.pyi` & `ralium-1.1.0/ralium/builtins.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/bundle.py` & `ralium-1.1.0/ralium/bundle.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     def __init__(self, *, url, page, server, styles):
         self.url = url
         self.page = page
         self.server = server
         self.styles = styles
     
     def __repr__(self):
-        return f"ralium.bundle.Bundle(url='{self.url}', page={repr(self.page)}, server={repr(self.server)}, styles={[repr(f) for f in self.styles]})"
+        return f"ralium.bundle.Bundle(url='{self.url}', page={repr(self.page)}, server={repr(self.server)}, styles=[{''.join([repr(v) for v in self.styles])}])"
 
 class FileSystem(dict):
     def __init__(self, *, images, styles, bundles):
         self.images = images
         self.styles = styles
         self.bundles = bundles
 
@@ -208,15 +208,15 @@
             f"    styles = {styles},\n".encode(),
             f"    bundles = {bundles}\n".encode(),
             b"))\n\n",
             self.get_content(self.pyfile)
         ]
     
     def relpath(self, filename):
-        return os.path.normpath(os.path.abspath(filename).removeprefix(self.webfolder))
+        return os.path.normpath(os.path.abspath(filename).removeprefix(os.path.dirname(self.webfolder)))
 
     def collect(self, dir, callback):
         data = []
 
         for root, _, files in os.walk(dir):
             for file in files:
                 filepath = os.path.abspath(os.path.join(root, file))
```

### Comparing `ralium-1.0.1/ralium/bundle.pyi` & `ralium-1.1.0/ralium/bundle.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/config.py` & `ralium-1.1.0/ralium/config.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/element.py` & `ralium-1.1.0/ralium/element.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/element.pyi` & `ralium-1.1.0/ralium/element.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/engine.py` & `ralium-1.1.0/ralium/engine.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/engine.pyi` & `ralium-1.1.0/ralium/engine.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/errors.py` & `ralium-1.1.0/ralium/errors.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/listener.py` & `ralium-1.1.0/ralium/listener.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/listener.pyi` & `ralium-1.1.0/ralium/listener.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/navigation.py` & `ralium-1.1.0/ralium/navigation.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/setup.py` & `ralium-1.1.0/ralium/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from PyInstaller.__main__ import logger, run as CompileExe
+from PyInstaller.__main__ import logger, run as pack
+from PyInstaller import compat
+
 from ralium.errors import DisableWarnings, SetupError
 from ralium.bundle import PyBundler
 from ralium._util import __version__
+
 import sys
 import os
 
 HTML_FILE_EXTENSIONS = [".htm", ".html"]
 FILE_EXTENSIONS = [*HTML_FILE_EXTENSIONS, ".css", ".py"]
 
 def _exe_str_error(name, var):
@@ -90,23 +93,31 @@
         
         bundle_dist = os.path.abspath(bundle_dist)
 
         if not os.path.exists(bundle_dist):
             os.mkdir(bundle_dist)
             logger.info("created %s", bundle_dist)
 
-        name, ext = os.path.splitext(os.path.basename(pyfile))
-        filename = os.path.join(bundle_dist, f"{name}.bundle{ext}")
+        base, ext = os.path.splitext(os.path.basename(pyfile))
+        filename = os.path.join(bundle_dist, f"{name or base}.bundle{ext}")
 
         logger.info("Bundling '%s' with project '%s'", pyfile, os.path.abspath(webfolder))
 
         code = PyBundler(pyfile, webfolder).view()
 
         if not warnings:
             code.insert(0, b"import ralium.errors; ralium.errors.DisableWarnings()\n")
+        
+        # PyInstaller 6.6.0 and greater require these modules on Windows.
+        # If you compile the program without these lines added to the file.
+        # An ImportError will occur in which the pywin32-ctypes module needs to be installed.
+        # Adding these lines as imports before everything else fixes this problem.
+        if compat.is_win:
+            code.insert(0, b"from win32ctypes.pywin32 import pywintypes\n")
+            code.insert(1, b"from win32ctypes.pywin32 import win32api\n\n")
 
         with open(filename, "wb") as f:
             f.writelines(code)
 
         logger.info("wrote %s", filename)
         logger.info("Finished Bundling")
 
@@ -144,8 +155,8 @@
     if noconsole:
         args.append(f"--noconsole")
     
     if webfolder and not bundle:
         for src, dst in collect_webfolder(webfolder).items():
             args.append(_add_data_arg(src, dst))
 
-    CompileExe(args)
+    pack(args)
```

### Comparing `ralium-1.0.1/ralium/setup.pyi` & `ralium-1.1.0/ralium/setup.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/webpage.py` & `ralium-1.1.0/ralium/webpage.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/webpage.pyi` & `ralium-1.1.0/ralium/webpage.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/window.py` & `ralium-1.1.0/ralium/window.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium/window.pyi` & `ralium-1.1.0/ralium/window.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.1/ralium.egg-info/PKG-INFO` & `ralium-1.1.0/ralium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 1.0.1
+Version: 1.1.0
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,10 +685,11 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4
 Requires-Dist: pyinstaller
 Requires-Dist: pywebview
+Requires-Dist: lxml
 
 # Ralium
 A pywebview wrapper inspired by Neutron.
```

### Comparing `ralium-1.0.1/ralium.egg-info/SOURCES.txt` & `ralium-1.1.0/ralium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

