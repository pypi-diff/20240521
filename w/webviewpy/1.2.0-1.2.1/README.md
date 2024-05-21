# Comparing `tmp/webviewpy-1.2.0.tar.gz` & `tmp/webviewpy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webviewpy-1.2.0.tar", last modified: Wed May  1 03:30:44 2024, max compression
+gzip compressed data, was "webviewpy-1.2.1.tar", last modified: Tue May 21 16:01:55 2024, max compression
```

## Comparing `webviewpy-1.2.0.tar` & `webviewpy-1.2.1.tar`

### file list

```diff
@@ -1,60 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 03:30:44.772983 webviewpy-1.2.0/
--rw-rw-rw-   0        0        0       68 2024-05-01 03:30:18.000000 webviewpy-1.2.0/.gitattributes
-drwxrwxrwx   0        0        0        0 2024-05-01 03:30:44.745418 webviewpy-1.2.0/.github/
-drwxrwxrwx   0        0        0        0 2024-05-01 03:30:44.751730 webviewpy-1.2.0/.github/workflows/
--rw-rw-rw-   0        0        0     1418 2024-05-01 03:30:18.000000 webviewpy-1.2.0/.github/workflows/main.yml
--rw-rw-rw-   0        0        0      150 2024-05-01 03:30:18.000000 webviewpy-1.2.0/.gitignore
--rw-rw-rw-   0        0        0       87 2024-05-01 03:30:18.000000 webviewpy-1.2.0/.gitmodules
--rw-rw-rw-   0        0        0     1098 2024-05-01 03:30:18.000000 webviewpy-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     2886 2024-05-01 03:30:44.772418 webviewpy-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      841 2024-05-01 03:30:18.000000 webviewpy-1.2.0/README.md
--rw-rw-rw-   0        0        0     3129 2024-05-01 03:30:18.000000 webviewpy-1.2.0/cibuildlib.py
-drwxrwxrwx   0        0        0        0 2024-05-01 03:30:44.751730 webviewpy-1.2.0/example/
-drwxrwxrwx   0        0        0        0 2024-05-01 03:30:44.751730 webviewpy-1.2.0/example/fluent/
--rw-rw-rw-   0        0        0      333 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/.gitignore
--rw-rw-rw-   0        0        0     3429 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/README.md
--rw-rw-rw-   0        0        0     1946 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/main.py
--rw-rw-rw-   0        0        0      893 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/package.json
-drwxrwxrwx   0        0        0        0 2024-05-01 03:30:44.757853 webviewpy-1.2.0/example/fluent/public/
--rw-rw-rw-   0        0        0     3870 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/public/favicon.ico
--rw-rw-rw-   0        0        0     1764 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/public/index.html
--rw-rw-rw-   0        0        0     5347 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/public/logo192.png
--rw-rw-rw-   0        0        0     9664 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/public/logo512.png
--rw-rw-rw-   0        0        0      517 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/public/manifest.json
--rw-rw-rw-   0        0        0       70 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/public/robots.txt
-drwxrwxrwx   0        0        0        0 2024-05-01 03:30:44.763256 webviewpy-1.2.0/example/fluent/src/
--rw-rw-rw-   0        0        0      602 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/src/App.css
--rw-rw-rw-   0        0        0     1986 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/src/App.js
--rw-rw-rw-   0        0        0      254 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/src/App.test.js
--rw-rw-rw-   0        0        0      379 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/src/index.css
--rw-rw-rw-   0        0        0      552 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/src/index.js
--rw-rw-rw-   0        0        0     2632 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/src/logo.svg
--rw-rw-rw-   0        0        0      375 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/src/reportWebVitals.js
--rw-rw-rw-   0        0        0      246 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/fluent/src/setupTests.js
--rw-rw-rw-   0        0        0     2046 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/test.py
--rw-rw-rw-   0        0        0     2553 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/testpyqt.py
--rw-rw-rw-   0        0        0      907 2024-05-01 03:30:18.000000 webviewpy-1.2.0/example/testtkinter.py
--rw-rw-rw-   0        0        0     1139 2024-05-01 03:30:18.000000 webviewpy-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-01 03:30:44.772983 webviewpy-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-01 03:30:44.764974 webviewpy-1.2.0/webviewpy/
--rw-rw-rw-   0        0        0    10663 2024-05-01 03:30:18.000000 webviewpy-1.2.0/webviewpy/__init__.py
--rw-rw-rw-   0        0        0     9089 2024-05-01 03:30:18.000000 webviewpy-1.2.0/webviewpy/__init__.pyi
--rw-rw-rw-   0        0        0      456 2024-05-01 03:30:44.000000 webviewpy-1.2.0/webviewpy/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 03:30:44.767823 webviewpy-1.2.0/webviewpy/platform/
--rw-rw-rw-   0        0        0        0 2024-05-01 03:30:18.000000 webviewpy-1.2.0/webviewpy/platform/.keepdir
-drwxrwxrwx   0        0        0        0 2024-05-01 03:30:44.747082 webviewpy-1.2.0/webviewpy/platform/darwin/
-drwxrwxrwx   0        0        0        0 2024-05-01 03:30:44.768391 webviewpy-1.2.0/webviewpy/platform/darwin/x64/
--rw-rw-rw-   0        0        0   438216 2024-05-01 03:30:37.000000 webviewpy-1.2.0/webviewpy/platform/darwin/x64/libwebview.dylib
-drwxrwxrwx   0        0        0        0 2024-05-01 03:30:44.747082 webviewpy-1.2.0/webviewpy/platform/linux/
-drwxrwxrwx   0        0        0        0 2024-05-01 03:30:44.769525 webviewpy-1.2.0/webviewpy/platform/linux/x64/
--rw-rw-rw-   0        0        0   226984 2024-05-01 03:30:37.000000 webviewpy-1.2.0/webviewpy/platform/linux/x64/libwebview.so
-drwxrwxrwx   0        0        0        0 2024-05-01 03:30:44.747082 webviewpy-1.2.0/webviewpy/platform/win32/
-drwxrwxrwx   0        0        0        0 2024-05-01 03:30:44.770092 webviewpy-1.2.0/webviewpy/platform/win32/x64/
--rw-rw-rw-   0        0        0   301568 2024-05-01 03:30:37.000000 webviewpy-1.2.0/webviewpy/platform/win32/x64/webview.dll
-drwxrwxrwx   0        0        0        0 2024-05-01 03:30:44.771225 webviewpy-1.2.0/webviewpy/platform/win32/x86/
--rw-rw-rw-   0        0        0   240128 2024-05-01 03:30:37.000000 webviewpy-1.2.0/webviewpy/platform/win32/x86/webview.dll
-drwxrwxrwx   0        0        0        0 2024-05-01 03:30:44.771845 webviewpy-1.2.0/webviewpy.egg-info/
--rw-rw-rw-   0        0        0     2886 2024-05-01 03:30:44.000000 webviewpy-1.2.0/webviewpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1118 2024-05-01 03:30:44.000000 webviewpy-1.2.0/webviewpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 03:30:44.000000 webviewpy-1.2.0/webviewpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-01 03:30:44.000000 webviewpy-1.2.0/webviewpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.425063 webviewpy-1.2.1/
+-rw-rw-rw-   0        0        0       68 2024-05-21 16:01:36.000000 webviewpy-1.2.1/.gitattributes
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.393820 webviewpy-1.2.1/.github/
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.393820 webviewpy-1.2.1/.github/workflows/
+-rw-rw-rw-   0        0        0     1418 2024-05-21 16:01:36.000000 webviewpy-1.2.1/.github/workflows/main.yml
+-rw-rw-rw-   0        0        0      150 2024-05-21 16:01:36.000000 webviewpy-1.2.1/.gitignore
+-rw-rw-rw-   0        0        0       87 2024-05-21 16:01:36.000000 webviewpy-1.2.1/.gitmodules
+-rw-rw-rw-   0        0        0     1098 2024-05-21 16:01:36.000000 webviewpy-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2886 2024-05-21 16:01:55.425063 webviewpy-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      841 2024-05-21 16:01:36.000000 webviewpy-1.2.1/README.md
+-rw-rw-rw-   0        0        0     3129 2024-05-21 16:01:36.000000 webviewpy-1.2.1/cibuildlib.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.409439 webviewpy-1.2.1/example/
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.409439 webviewpy-1.2.1/example/fluent/
+-rw-rw-rw-   0        0        0      333 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/.gitignore
+-rw-rw-rw-   0        0        0     3429 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/README.md
+-rw-rw-rw-   0        0        0     1946 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/main.py
+-rw-rw-rw-   0        0        0      893 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/package.json
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.409439 webviewpy-1.2.1/example/fluent/public/
+-rw-rw-rw-   0        0        0     3870 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/public/favicon.ico
+-rw-rw-rw-   0        0        0     1764 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/public/index.html
+-rw-rw-rw-   0        0        0     5347 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/public/logo192.png
+-rw-rw-rw-   0        0        0     9664 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/public/logo512.png
+-rw-rw-rw-   0        0        0      517 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/public/manifest.json
+-rw-rw-rw-   0        0        0       70 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/public/robots.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.409439 webviewpy-1.2.1/example/fluent/src/
+-rw-rw-rw-   0        0        0      602 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/src/App.css
+-rw-rw-rw-   0        0        0     1986 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/src/App.js
+-rw-rw-rw-   0        0        0      254 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/src/App.test.js
+-rw-rw-rw-   0        0        0      379 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/src/index.css
+-rw-rw-rw-   0        0        0      552 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/src/index.js
+-rw-rw-rw-   0        0        0     2632 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/src/logo.svg
+-rw-rw-rw-   0        0        0      375 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/src/reportWebVitals.js
+-rw-rw-rw-   0        0        0      246 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/fluent/src/setupTests.js
+-rw-rw-rw-   0        0        0     2046 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/test.py
+-rw-rw-rw-   0        0        0     2553 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/testpyqt.py
+-rw-rw-rw-   0        0        0      907 2024-05-21 16:01:36.000000 webviewpy-1.2.1/example/testtkinter.py
+-rw-rw-rw-   0        0        0     1290 2024-05-21 16:01:36.000000 webviewpy-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 16:01:55.425063 webviewpy-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.409439 webviewpy-1.2.1/webviewpy/
+-rw-rw-rw-   0        0        0    10848 2024-05-21 16:01:36.000000 webviewpy-1.2.1/webviewpy/__init__.py
+-rw-rw-rw-   0        0        0     9089 2024-05-21 16:01:36.000000 webviewpy-1.2.1/webviewpy/__init__.pyi
+-rw-rw-rw-   0        0        0      456 2024-05-21 16:01:55.000000 webviewpy-1.2.1/webviewpy/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.409439 webviewpy-1.2.1/webviewpy/platform/
+-rw-rw-rw-   0        0        0        0 2024-05-21 16:01:36.000000 webviewpy-1.2.1/webviewpy/platform/.keepdir
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.393820 webviewpy-1.2.1/webviewpy/platform/darwin/
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.409439 webviewpy-1.2.1/webviewpy/platform/darwin/x64/
+-rw-rw-rw-   0        0        0   438216 2024-05-21 16:01:49.000000 webviewpy-1.2.1/webviewpy/platform/darwin/x64/libwebview.dylib
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.393820 webviewpy-1.2.1/webviewpy/platform/linux/
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.425063 webviewpy-1.2.1/webviewpy/platform/linux/x64/
+-rw-rw-rw-   0        0        0   226984 2024-05-21 16:01:49.000000 webviewpy-1.2.1/webviewpy/platform/linux/x64/libwebview.so
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.393820 webviewpy-1.2.1/webviewpy/platform/win32/
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.425063 webviewpy-1.2.1/webviewpy/platform/win32/x64/
+-rw-rw-rw-   0        0        0   301568 2024-05-21 16:01:49.000000 webviewpy-1.2.1/webviewpy/platform/win32/x64/webview.dll
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.425063 webviewpy-1.2.1/webviewpy/platform/win32/x86/
+-rw-rw-rw-   0        0        0   240128 2024-05-21 16:01:49.000000 webviewpy-1.2.1/webviewpy/platform/win32/x86/webview.dll
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.425063 webviewpy-1.2.1/webviewpy/tools/
+-rw-rw-rw-   0        0        0        0 2024-05-21 16:01:36.000000 webviewpy-1.2.1/webviewpy/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.425063 webviewpy-1.2.1/webviewpy/tools/__pyinstaller/
+-rw-rw-rw-   0        0        0       77 2024-05-21 16:01:36.000000 webviewpy-1.2.1/webviewpy/tools/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0       67 2024-05-21 16:01:36.000000 webviewpy-1.2.1/webviewpy/tools/__pyinstaller/hook-webviewpy.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:01:55.425063 webviewpy-1.2.1/webviewpy.egg-info/
+-rw-rw-rw-   0        0        0     2886 2024-05-21 16:01:55.000000 webviewpy-1.2.1/webviewpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1272 2024-05-21 16:01:55.000000 webviewpy-1.2.1/webviewpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 16:01:55.000000 webviewpy-1.2.1/webviewpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-21 16:01:55.000000 webviewpy-1.2.1/webviewpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2024-05-21 16:01:55.000000 webviewpy-1.2.1/webviewpy.egg-info/top_level.txt
```

### Comparing `webviewpy-1.2.0/.github/workflows/main.yml` & `webviewpy-1.2.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/LICENSE` & `webviewpy-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/PKG-INFO` & `webviewpy-1.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webviewpy
-Version: 1.2.0
+Version: 1.2.1
 Summary: ctypes binding of webview
 Author: HIllya51
 License: Copyright (c) 2013, Aldo Cortesi. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `webviewpy-1.2.0/README.md` & `webviewpy-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/cibuildlib.py` & `webviewpy-1.2.1/cibuildlib.py`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/example/fluent/README.md` & `webviewpy-1.2.1/example/fluent/README.md`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/example/fluent/main.py` & `webviewpy-1.2.1/example/fluent/main.py`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/example/fluent/package.json` & `webviewpy-1.2.1/example/fluent/package.json`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/example/fluent/public/favicon.ico` & `webviewpy-1.2.1/example/fluent/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/example/fluent/public/index.html` & `webviewpy-1.2.1/example/fluent/public/index.html`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/example/fluent/public/logo192.png` & `webviewpy-1.2.1/example/fluent/public/logo192.png`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/example/fluent/public/logo512.png` & `webviewpy-1.2.1/example/fluent/public/logo512.png`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/example/fluent/public/manifest.json` & `webviewpy-1.2.1/example/fluent/public/manifest.json`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/example/fluent/src/App.css` & `webviewpy-1.2.1/example/fluent/src/App.css`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/example/fluent/src/App.js` & `webviewpy-1.2.1/example/fluent/src/App.js`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/example/fluent/src/index.js` & `webviewpy-1.2.1/example/fluent/src/index.js`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/example/fluent/src/logo.svg` & `webviewpy-1.2.1/example/fluent/src/logo.svg`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/example/test.py` & `webviewpy-1.2.1/example/test.py`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/example/testpyqt.py` & `webviewpy-1.2.1/example/testpyqt.py`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/example/testtkinter.py` & `webviewpy-1.2.1/example/testtkinter.py`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/pyproject.toml` & `webviewpy-1.2.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools_scm[toml]"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webviewpy"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="HIllya51"},
 ]
 license = { file = "LICENSE" }
 description = "ctypes binding of webview"
 readme = "README.md"
 
@@ -27,14 +27,17 @@
 
 [project.urls]
 Homepage = "https://github.com/HIllya51/webviewpy"
 Repository = "https://github.com/HIllya51/webviewpy"
 
 [tool.setuptools]
 include-package-data = false
-packages = ["webviewpy", "webviewpy.platform"]
+packages = ["webviewpy", "webviewpy.platform", "webviewpy.tools", "webviewpy.tools.__pyinstaller"]
 
 [tool.setuptools.package-data]
 "webviewpy.platform" = ["**/*.dll","**/*.so","**/*.dylib"]
 
 [tool.setuptools_scm]
 write_to = "webviewpy/__version__.py"
+
+[project.entry-points.pyinstaller40]
+hook-dirs = "webviewpy.tools.__pyinstaller:get_hook_dirs"
```

### Comparing `webviewpy-1.2.0/webviewpy/__init__.py` & `webviewpy-1.2.1/webviewpy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,29 +98,32 @@
         self.build_metadata = lpwv.contents.build_metadata.decode("utf8")
 
 
 class webview_exception(Exception):
     pass
 
 
-isbit64 = platform.architecture()[0] == "64bit"
-DLL3264path = os.path.abspath(
-    os.path.join(
-        os.path.dirname(__file__), "platform", sys.platform, ("x86", "x64")[isbit64]
+def get_library_path():
+    is_64bit = platform.architecture()[0] == "64bit"
+    library_base_path = os.path.abspath(
+        os.path.join(
+            os.path.dirname(__file__), "platform", sys.platform, ("x86", "x64")[is_64bit]
+        )
     )
-)
-if sys.platform == "win32":
-    targetdllname = "webview.dll"
-elif sys.platform == "linux":
-    targetdllname = "libwebview.so"
-elif sys.platform == "darwin":
-    targetdllname = "libwebview.dylib"
-else:
-    targetdllname = "webview"
-webviewdll = os.path.join(DLL3264path, targetdllname)
+    if sys.platform == "win32":
+        target_library_name = "webview.dll"
+    elif sys.platform == "linux":
+        target_library_name = "libwebview.so"
+    elif sys.platform == "darwin":
+        target_library_name = "libwebview.dylib"
+    else:
+        target_library_name = "webview"
+    return os.path.join(library_base_path, target_library_name)
+
+webviewdll = get_library_path()
 
 
 webview_dispatch_fn_t = CFUNCTYPE(None, webview_t, c_void_p)
 webview_bind_fn_t = CFUNCTYPE(None, c_char_p, c_char_p, c_void_p)
 
 
 def declare_library_path(librarypath=None, exception=True):
@@ -309,14 +312,15 @@
     def version():
         return Webview_Version(webview_version())
 
 
 __all__ = [
     getattr(_, "__name__")
     for _ in [
+        get_library_path,
         declare_library_path,
         webview_hint_t,
         webview_error_t,
         webview_native_handle_kind_t,
         webview_exception,
         Webview,
     ]
```

### Comparing `webviewpy-1.2.0/webviewpy/__init__.pyi` & `webviewpy-1.2.1/webviewpy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/webviewpy/platform/darwin/x64/libwebview.dylib` & `webviewpy-1.2.1/webviewpy/platform/darwin/x64/libwebview.dylib`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/webviewpy/platform/linux/x64/libwebview.so` & `webviewpy-1.2.1/webviewpy/platform/linux/x64/libwebview.so`

 * *Files identical despite different names*

### Comparing `webviewpy-1.2.0/webviewpy/platform/win32/x64/webview.dll` & `webviewpy-1.2.1/webviewpy/platform/win32/x64/webview.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018001985c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May  1 03:29:31 2024
+Time/Date		Tue May 21 16:00:33 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000032800
 SizeOfInitializedData	0000000000018000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001985c
@@ -83830,15 +83830,17 @@
    18003e5db:	(bad)
    18003e5dc:	(bad)
    18003e5dd:	(bad)
    18003e5de:	(bad)
    18003e5df:	ret
    18003e5e0:	add    %al,(%rax)
    18003e5e2:	add    %al,(%rax)
-   18003e5e4:	sbb    0x6631(%rdi),%esi
+   18003e5e4:	and    %eax,%ebp
+   18003e5e6:	rex.WR
+   18003e5e7:	data16 add %al,(%rax)
    18003e5ea:	add    %al,(%rax)
    18003e5ec:	or     $0x4c000000,%eax
    18003e5f1:	add    (%rax),%eax
    18003e5f3:	add    %bl,%ah
    18003e5f5:	incl   (%rbx)
    18003e5f7:	add    %bl,%ah
    18003e5f9:	jmp    0x18003e5fe
```

### Comparing `webviewpy-1.2.0/webviewpy/platform/win32/x86/webview.dll` & `webviewpy-1.2.1/webviewpy/platform/win32/x86/webview.dll`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 96d1 adb1 d6a9 aeb0 96d1 abb1 53a9 aeb0  ............S...
 000000a0: 96d1 aab1 c9a9 aeb0 8fdc aab1 d2a9 aeb0  ................
 000000b0: 8fdc adb1 c8a9 aeb0 96d1 afb1 d2a9 aeb0  ................
 000000c0: dda9 afb0 a3a9 aeb0 8fdc abb1 faa9 aeb0  ................
 000000d0: 17dc abb1 dca9 aeb0 17dc aeb1 dca9 aeb0  ................
 000000e0: 17dc acb1 dca9 aeb0 5269 6368 dda9 aeb0  ........Rich....
 000000f0: 0000 0000 0000 0000 5045 0000 4c01 0400  ........PE..L...
-00000100: 21b7 3166 0000 0000 0000 0000 e000 0221  !.1f...........!
+00000100: 34c5 4c66 0000 0000 0000 0000 e000 0221  4.Lf...........!
 00000110: 0b01 0e1d 00b4 0200 00fe 0000 0000 0000  ................
 00000120: 7e5b 0100 0010 0000 00d0 0200 0000 0010  ~[..............
 00000130: 0010 0000 0002 0000 0600 0000 0000 0000  ................
 00000140: 0600 0000 0000 0000 00e0 0300 0004 0000  ................
 00000150: 0000 0000 0200 4001 0000 1000 0010 0000  ......@.........
 00000160: 0000 1000 0010 0000 0000 0000 1000 0000  ................
 00000170: 907d 0300 f401 0000 847f 0300 a000 0000  .}..............
@@ -13004,15 +13004,15 @@
 00032cb0: 7300 0000 5f68 7970 6f74 0000 666d 6f64  s..._hypot..fmod
 00032cc0: 0000 0000 6672 6578 7000 0000 5f79 3000  ....frexp..._y0.
 00032cd0: 5f79 3100 5f79 6e00 5f6c 6f67 6200 0000  _y1._yn._logb...
 00032ce0: 5f6e 6578 7461 6674 6572 0000 0000 0000  _nextafter......
 00032cf0: 0000 0000 0000 f07f ffff ffff ffff ef7f  ................
 00032d00: 0000 0000 0000 0080 0000 0000 0000 0000  ................
 00032d10: 0000 804f 0000 005f ffff ffff 0000 0000  ...O..._........
-00032d20: 21b7 3166 0000 0000 0d00 0000 2003 0000  !.1f........ ...
+00032d20: 34c5 4c66 0000 0000 0d00 0000 2003 0000  4.Lf........ ...
 00032d30: d859 0300 d841 0300 bc00 0000 0000 0000  .Y...A..........
 00032d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00032d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00032d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00032d70: 0000 0000 0c90 0310 7451 0310 6d00 0000  ........tQ..m...
 00032d80: dcd1 0210 0000 0000 0000 0000 0000 0000  ................
 00032d90: 0001 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `webviewpy-1.2.0/webviewpy.egg-info/PKG-INFO` & `webviewpy-1.2.1/webviewpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webviewpy
-Version: 1.2.0
+Version: 1.2.1
 Summary: ctypes binding of webview
 Author: HIllya51
 License: Copyright (c) 2013, Aldo Cortesi. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `webviewpy-1.2.0/webviewpy.egg-info/SOURCES.txt` & `webviewpy-1.2.1/webviewpy.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -29,13 +29,17 @@
 example/fluent/src/setupTests.js
 webviewpy/__init__.py
 webviewpy/__init__.pyi
 webviewpy/__version__.py
 webviewpy.egg-info/PKG-INFO
 webviewpy.egg-info/SOURCES.txt
 webviewpy.egg-info/dependency_links.txt
+webviewpy.egg-info/entry_points.txt
 webviewpy.egg-info/top_level.txt
 webviewpy/platform/.keepdir
 webviewpy/platform/darwin/x64/libwebview.dylib
 webviewpy/platform/linux/x64/libwebview.so
 webviewpy/platform/win32/x64/webview.dll
-webviewpy/platform/win32/x86/webview.dll
+webviewpy/platform/win32/x86/webview.dll
+webviewpy/tools/__init__.py
+webviewpy/tools/__pyinstaller/__init__.py
+webviewpy/tools/__pyinstaller/hook-webviewpy.py
```

