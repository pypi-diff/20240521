# Comparing `tmp/ralium-1.0.0.tar.gz` & `tmp/ralium-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralium-1.0.0.tar", last modified: Tue May 21 00:37:45 2024, max compression
+gzip compressed data, was "ralium-1.0.1.tar", last modified: Tue May 21 00:41:39 2024, max compression
```

## Comparing `ralium-1.0.0.tar` & `ralium-1.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 00:37:45.942921 ralium-1.0.0/
--rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    41876 2024-05-21 00:37:45.940917 ralium-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-1.0.0/README.md
--rw-rw-rw-   0        0        0     1018 2024-05-21 00:37:01.000000 ralium-1.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-21 00:37:45.916088 ralium-1.0.0/ralium/
--rw-rw-rw-   0        0        0      383 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/__init__.py
--rw-rw-rw-   0        0        0     2947 2024-05-21 00:30:56.000000 ralium-1.0.0/ralium/_util.py
--rw-rw-rw-   0        0        0     1170 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/_util.pyi
--rw-rw-rw-   0        0        0     7547 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/api.py
--rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/api.pyi
--rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/builtins.py
--rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/builtins.pyi
--rw-rw-rw-   0        0        0     8293 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/bundle.py
--rw-rw-rw-   0        0        0     1581 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/bundle.pyi
--rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/config.py
--rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/config.pyi
--rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/element.py
--rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/element.pyi
--rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/engine.py
--rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/engine.pyi
--rw-rw-rw-   0        0        0     1191 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/errors.py
--rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/listener.py
--rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/listener.pyi
--rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/navigation.py
--rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/navigation.pyi
--rw-rw-rw-   0        0        0     5434 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/setup.py
--rw-rw-rw-   0        0        0      699 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/setup.pyi
--rw-rw-rw-   0        0        0     6936 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/webpage.py
--rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-1.0.0/ralium/webpage.pyi
--rw-rw-rw-   0        0        0     6031 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/window.py
--rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-1.0.0/ralium/window.pyi
-drwxrwxrwx   0        0        0        0 2024-05-21 00:37:45.938830 ralium-1.0.0/ralium.egg-info/
--rw-rw-rw-   0        0        0    41876 2024-05-21 00:37:45.000000 ralium-1.0.0/ralium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      647 2024-05-21 00:37:45.000000 ralium-1.0.0/ralium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 00:37:45.000000 ralium-1.0.0/ralium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-21 00:37:45.000000 ralium-1.0.0/ralium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 00:37:45.000000 ralium-1.0.0/ralium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 00:37:45.942921 ralium-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 00:41:39.277462 ralium-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    41876 2024-05-21 00:41:39.276018 ralium-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-1.0.1/README.md
+-rw-rw-rw-   0        0        0      958 2024-05-21 00:40:52.000000 ralium-1.0.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-21 00:41:39.256858 ralium-1.0.1/ralium/
+-rw-rw-rw-   0        0        0      383 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/__init__.py
+-rw-rw-rw-   0        0        0     2947 2024-05-21 00:40:35.000000 ralium-1.0.1/ralium/_util.py
+-rw-rw-rw-   0        0        0     1170 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/_util.pyi
+-rw-rw-rw-   0        0        0     7547 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/api.py
+-rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/api.pyi
+-rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/builtins.py
+-rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/builtins.pyi
+-rw-rw-rw-   0        0        0     8293 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/bundle.py
+-rw-rw-rw-   0        0        0     1581 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/bundle.pyi
+-rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/config.py
+-rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/config.pyi
+-rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/element.py
+-rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/element.pyi
+-rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/engine.py
+-rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/engine.pyi
+-rw-rw-rw-   0        0        0     1191 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/errors.py
+-rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/listener.py
+-rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/listener.pyi
+-rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/navigation.py
+-rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/navigation.pyi
+-rw-rw-rw-   0        0        0     5463 2024-05-21 00:39:16.000000 ralium-1.0.1/ralium/setup.py
+-rw-rw-rw-   0        0        0      699 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/setup.pyi
+-rw-rw-rw-   0        0        0     6936 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/webpage.py
+-rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-1.0.1/ralium/webpage.pyi
+-rw-rw-rw-   0        0        0     6031 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/window.py
+-rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-1.0.1/ralium/window.pyi
+drwxrwxrwx   0        0        0        0 2024-05-21 00:41:39.274919 ralium-1.0.1/ralium.egg-info/
+-rw-rw-rw-   0        0        0    41876 2024-05-21 00:41:39.000000 ralium-1.0.1/ralium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      647 2024-05-21 00:41:39.000000 ralium-1.0.1/ralium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 00:41:39.000000 ralium-1.0.1/ralium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-21 00:41:39.000000 ralium-1.0.1/ralium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 00:41:39.000000 ralium-1.0.1/ralium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 00:41:39.278785 ralium-1.0.1/setup.cfg
```

### Comparing `ralium-1.0.0/LICENSE` & `ralium-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/PKG-INFO` & `ralium-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 1.0.0
+Version: 1.0.1
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-1.0.0/pyproject.toml` & `ralium-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools >= 69.5.0", "wheel >= 0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ralium"
-version = "1.0.0"
+version = "1.0.1"
 description = "An easy to use wrapper for pywebview."
 readme = "README.md"
 authors = [{ name = "Isaiah Coroama", email = "coroamaisaiah@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
@@ -33,11 +33,8 @@
     "old/*",
     "tests/*",
     "examples/*"
 ]
 
 [tool.setuptools]
 include-package-data = true
-packages = ["ralium"]
-
-[tool.setuptools.package-data]
-"pkgname" = ["py.typed"]
+packages = ["ralium"]
```

### Comparing `ralium-1.0.0/ralium/_util.py` & `ralium-1.0.1/ralium/_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 __all__ = [
     "__version__",
     "BasicHTTPServer", "_get_http_server_handler", "_get_bundle", "_norm_url", "_check_exists", 
     "_check_is_dir", "_get_path_limit", "_read_file", "_get_path", "_is_markup_filelike"
 ]
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 SYS_BUNDLE_ATTRIBUTE = "bundled"
 
 class BasicHTTPServer(http.server.SimpleHTTPRequestHandler):
     pass
 
 def _get_bundle():
```

### Comparing `ralium-1.0.0/ralium/_util.pyi` & `ralium-1.0.1/ralium/_util.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/api.py` & `ralium-1.0.1/ralium/api.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/api.pyi` & `ralium-1.0.1/ralium/api.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/builtins.py` & `ralium-1.0.1/ralium/builtins.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/builtins.pyi` & `ralium-1.0.1/ralium/builtins.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/bundle.py` & `ralium-1.0.1/ralium/bundle.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/bundle.pyi` & `ralium-1.0.1/ralium/bundle.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/config.py` & `ralium-1.0.1/ralium/config.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/element.py` & `ralium-1.0.1/ralium/element.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/element.pyi` & `ralium-1.0.1/ralium/element.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/engine.py` & `ralium-1.0.1/ralium/engine.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/engine.pyi` & `ralium-1.0.1/ralium/engine.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/errors.py` & `ralium-1.0.1/ralium/errors.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/listener.py` & `ralium-1.0.1/ralium/listener.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/listener.pyi` & `ralium-1.0.1/ralium/listener.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/navigation.py` & `ralium-1.0.1/ralium/navigation.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/setup.py` & `ralium-1.0.1/ralium/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,16 @@
 
         with open(filename, "wb") as f:
             f.writelines(code)
 
         logger.info("wrote %s", filename)
         logger.info("Finished Bundling")
 
+        pyfile = filename
+
     if getattr(sys, "frozen", False):
         raise RuntimeError("Ralium setup cannot be ran from an executable file.")
     
     if not os.path.exists(pyfile):
         raise FileNotFoundError(f"Failed to find python file '{pyfile}'")
 
     args = [pyfile, *(pyi_args or [])]
```

### Comparing `ralium-1.0.0/ralium/setup.pyi` & `ralium-1.0.1/ralium/setup.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/webpage.py` & `ralium-1.0.1/ralium/webpage.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/webpage.pyi` & `ralium-1.0.1/ralium/webpage.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/window.py` & `ralium-1.0.1/ralium/window.py`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium/window.pyi` & `ralium-1.0.1/ralium/window.pyi`

 * *Files identical despite different names*

### Comparing `ralium-1.0.0/ralium.egg-info/PKG-INFO` & `ralium-1.0.1/ralium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 1.0.0
+Version: 1.0.1
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-1.0.0/ralium.egg-info/SOURCES.txt` & `ralium-1.0.1/ralium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

