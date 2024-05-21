# Comparing `tmp/ralium-1.1.0.tar.gz` & `tmp/ralium-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralium-1.1.0.tar", last modified: Tue May 21 04:31:12 2024, max compression
+gzip compressed data, was "ralium-1.2.0.tar", last modified: Tue May 21 05:44:15 2024, max compression
```

## Comparing `ralium-1.1.0.tar` & `ralium-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 04:31:12.642890 ralium-1.1.0/
--rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-1.1.0/LICENSE
--rw-rw-rw-   0        0        0    41897 2024-05-21 04:31:12.641622 ralium-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-1.1.0/README.md
--rw-rw-rw-   0        0        0      970 2024-05-21 04:30:23.000000 ralium-1.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-21 04:31:12.616269 ralium-1.1.0/ralium/
--rw-rw-rw-   0        0        0      383 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/__init__.py
--rw-rw-rw-   0        0        0     2965 2024-05-21 04:28:49.000000 ralium-1.1.0/ralium/_util.py
--rw-rw-rw-   0        0        0     1170 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/_util.pyi
--rw-rw-rw-   0        0        0     7555 2024-05-21 04:21:31.000000 ralium-1.1.0/ralium/api.py
--rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/api.pyi
--rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/builtins.py
--rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/builtins.pyi
--rw-rw-rw-   0        0        0     8321 2024-05-21 04:14:13.000000 ralium-1.1.0/ralium/bundle.py
--rw-rw-rw-   0        0        0     1581 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/bundle.pyi
--rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/config.py
--rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/config.pyi
--rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/element.py
--rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/element.pyi
--rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/engine.py
--rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/engine.pyi
--rw-rw-rw-   0        0        0     1191 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/errors.py
--rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/listener.py
--rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/listener.pyi
--rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/navigation.py
--rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/navigation.pyi
--rw-rw-rw-   0        0        0     6017 2024-05-21 04:03:11.000000 ralium-1.1.0/ralium/setup.py
--rw-rw-rw-   0        0        0      699 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/setup.pyi
--rw-rw-rw-   0        0        0     6936 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/webpage.py
--rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-1.1.0/ralium/webpage.pyi
--rw-rw-rw-   0        0        0     6031 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/window.py
--rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-1.1.0/ralium/window.pyi
-drwxrwxrwx   0        0        0        0 2024-05-21 04:31:12.639589 ralium-1.1.0/ralium.egg-info/
--rw-rw-rw-   0        0        0    41897 2024-05-21 04:31:12.000000 ralium-1.1.0/ralium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      647 2024-05-21 04:31:12.000000 ralium-1.1.0/ralium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 04:31:12.000000 ralium-1.1.0/ralium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 04:31:12.000000 ralium-1.1.0/ralium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 04:31:12.000000 ralium-1.1.0/ralium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 04:31:12.642890 ralium-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 05:44:15.858890 ralium-1.2.0/
+-rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0    41897 2024-05-21 05:44:15.856887 ralium-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-1.2.0/README.md
+-rw-rw-rw-   0        0        0      970 2024-05-21 05:43:45.000000 ralium-1.2.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-21 05:44:15.828859 ralium-1.2.0/ralium/
+-rw-rw-rw-   0        0        0      357 2024-05-21 05:00:06.000000 ralium-1.2.0/ralium/__init__.py
+-rw-rw-rw-   0        0        0     2965 2024-05-21 05:43:41.000000 ralium-1.2.0/ralium/_util.py
+-rw-rw-rw-   0        0        0     1170 2024-05-21 00:26:03.000000 ralium-1.2.0/ralium/_util.pyi
+-rw-rw-rw-   0        0        0     7555 2024-05-21 04:21:31.000000 ralium-1.2.0/ralium/api.py
+-rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-1.2.0/ralium/api.pyi
+-rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-1.2.0/ralium/builtins.py
+-rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-1.2.0/ralium/builtins.pyi
+-rw-rw-rw-   0        0        0     8321 2024-05-21 04:14:13.000000 ralium-1.2.0/ralium/bundle.py
+-rw-rw-rw-   0        0        0     1581 2024-05-21 00:26:03.000000 ralium-1.2.0/ralium/bundle.pyi
+-rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-1.2.0/ralium/config.py
+-rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-1.2.0/ralium/config.pyi
+-rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-1.2.0/ralium/element.py
+-rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-1.2.0/ralium/element.pyi
+-rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-1.2.0/ralium/engine.py
+-rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-1.2.0/ralium/engine.pyi
+-rw-rw-rw-   0        0        0     1191 2024-05-21 00:26:03.000000 ralium-1.2.0/ralium/errors.py
+-rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-1.2.0/ralium/listener.py
+-rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-1.2.0/ralium/listener.pyi
+-rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-1.2.0/ralium/navigation.py
+-rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-1.2.0/ralium/navigation.pyi
+-rw-rw-rw-   0        0        0     7851 2024-05-21 05:23:35.000000 ralium-1.2.0/ralium/setuptools.py
+-rw-rw-rw-   0        0        0      965 2024-05-21 05:19:13.000000 ralium-1.2.0/ralium/setuptools.pyi
+-rw-rw-rw-   0        0        0     6936 2024-05-21 00:26:03.000000 ralium-1.2.0/ralium/webpage.py
+-rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-1.2.0/ralium/webpage.pyi
+-rw-rw-rw-   0        0        0     6031 2024-05-21 00:25:27.000000 ralium-1.2.0/ralium/window.py
+-rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-1.2.0/ralium/window.pyi
+drwxrwxrwx   0        0        0        0 2024-05-21 05:44:15.854699 ralium-1.2.0/ralium.egg-info/
+-rw-rw-rw-   0        0        0    41897 2024-05-21 05:44:15.000000 ralium-1.2.0/ralium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      657 2024-05-21 05:44:15.000000 ralium-1.2.0/ralium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 05:44:15.000000 ralium-1.2.0/ralium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 05:44:15.000000 ralium-1.2.0/ralium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 05:44:15.000000 ralium-1.2.0/ralium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 05:44:15.858890 ralium-1.2.0/setup.cfg
```

### Comparing `ralium-1.1.0/LICENSE` & `ralium-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/PKG-INFO` & `ralium-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 1.1.0
+Version: 1.2.0
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-1.1.0/pyproject.toml` & `ralium-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools >= 69.5.0", "wheel >= 0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ralium"
-version = "1.1.0"
+version = "1.2.0"
 description = "An easy to use wrapper for pywebview."
 readme = "README.md"
 authors = [{ name = "Isaiah Coroama", email = "coroamaisaiah@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

### Comparing `ralium-1.1.0/ralium/_util.py` & `ralium-1.2.0/ralium/_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 __all__ = [
     "__version__",
     "BasicHTTPServer", "_get_http_server_handler", "_get_bundle", "_norm_url", "_check_exists", 
     "_check_is_dir", "_get_path_limit", "_read_file", "_get_path", "_is_markup_filelike"
 ]
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 
 SYS_BUNDLE_ATTRIBUTE = "bundled"
 
 class BasicHTTPServer(http.server.SimpleHTTPRequestHandler):
     pass
 
 def _get_bundle():
```

### Comparing `ralium-1.1.0/ralium/_util.pyi` & `ralium-1.2.0/ralium/_util.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/api.py` & `ralium-1.2.0/ralium/api.py`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/api.pyi` & `ralium-1.2.0/ralium/api.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/builtins.py` & `ralium-1.2.0/ralium/builtins.py`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/builtins.pyi` & `ralium-1.2.0/ralium/builtins.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/bundle.py` & `ralium-1.2.0/ralium/bundle.py`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/bundle.pyi` & `ralium-1.2.0/ralium/bundle.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/config.py` & `ralium-1.2.0/ralium/config.py`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/element.py` & `ralium-1.2.0/ralium/element.py`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/element.pyi` & `ralium-1.2.0/ralium/element.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/engine.py` & `ralium-1.2.0/ralium/engine.py`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/engine.pyi` & `ralium-1.2.0/ralium/engine.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/errors.py` & `ralium-1.2.0/ralium/errors.py`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/listener.py` & `ralium-1.2.0/ralium/listener.py`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/listener.pyi` & `ralium-1.2.0/ralium/listener.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/navigation.py` & `ralium-1.2.0/ralium/navigation.py`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/setup.pyi` & `ralium-1.2.0/ralium/setuptools.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,29 @@
 FILE_EXTENSIONS: list[str]
 
 def _exe_str_error(name: str, var: Any) -> Exception: ...
 def _add_data_arg(src: FilePathStr, dst: FilePathStr) -> str: ...
 
 def collect_webfolder(webfolder: DirPathStr) -> dict[FilePathStr]: ...
 
+def bundle(
+    pyfile: FilePathStr,
+    webfolder: DirPathStr,
+    name: str | None = None,
+    warnings: bool = False,
+    distpath: DirPathStr | None = None
+) -> FilePathStr: ...
+
 def setup(
     pyfile: FilePathStr,
     name: str | None = None,
     icon: FilePathStr | None = None,
     bundle: bool = False,
     webfolder: DirPathStr | None = None,
     warnings: bool = False,
     onefile: bool = True,
     noconsole: bool = True,
     bundle_dist: DirPathStr | None = None,
-    pyi_args: list[str] | None = None
+    pyi_args: list[str] | None = None,
+    use_subprocess: bool = False,
+    optimize_level: int | None = None
 ) -> None: ...
```

### Comparing `ralium-1.1.0/ralium/webpage.py` & `ralium-1.2.0/ralium/webpage.py`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/webpage.pyi` & `ralium-1.2.0/ralium/webpage.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/window.py` & `ralium-1.2.0/ralium/window.py`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium/window.pyi` & `ralium-1.2.0/ralium/window.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.1.0/ralium.egg-info/PKG-INFO` & `ralium-1.2.0/ralium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 1.1.0
+Version: 1.2.0
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-1.1.0/ralium.egg-info/SOURCES.txt` & `ralium-1.2.0/ralium.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 ralium/engine.py
 ralium/engine.pyi
 ralium/errors.py
 ralium/listener.py
 ralium/listener.pyi
 ralium/navigation.py
 ralium/navigation.pyi
-ralium/setup.py
-ralium/setup.pyi
+ralium/setuptools.py
+ralium/setuptools.pyi
 ralium/webpage.py
 ralium/webpage.pyi
 ralium/window.py
 ralium/window.pyi
 ralium.egg-info/PKG-INFO
 ralium.egg-info/SOURCES.txt
 ralium.egg-info/dependency_links.txt
```

