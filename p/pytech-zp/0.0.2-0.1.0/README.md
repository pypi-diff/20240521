# Comparing `tmp/pytech_zp-0.0.2.tar.gz` & `tmp/pytech_zp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytech_zp-0.0.2.tar", last modified: Tue May 14 03:17:46 2024, max compression
+gzip compressed data, was "pytech_zp-0.1.0.tar", last modified: Tue May 21 12:39:11 2024, max compression
```

## Comparing `pytech_zp-0.0.2.tar` & `pytech_zp-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 03:17:46.157453 pytech_zp-0.0.2/
--rw-rw-rw-   0        0        0     1091 2024-05-13 10:56:51.000000 pytech_zp-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       33 2024-05-13 11:16:04.000000 pytech_zp-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1811 2024-05-14 03:17:46.156044 pytech_zp-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      332 2024-05-13 10:55:50.000000 pytech_zp-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 03:17:46.144044 pytech_zp-0.0.2/pytech/
--rw-rw-rw-   0        0        0       36 2024-05-14 02:16:03.000000 pytech_zp-0.0.2/pytech/__init__.py
--rw-rw-rw-   0        0        0   208384 2024-05-14 01:44:08.000000 pytech_zp-0.0.2/pytech/pytech.cp39-win_amd64.pyd
-drwxrwxrwx   0        0        0        0 2024-05-14 03:17:46.149043 pytech_zp-0.0.2/pytech_zp.egg-info/
--rw-rw-rw-   0        0        0     1811 2024-05-14 03:17:46.000000 pytech_zp-0.0.2/pytech_zp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2024-05-14 03:17:46.000000 pytech_zp-0.0.2/pytech_zp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 03:17:46.000000 pytech_zp-0.0.2/pytech_zp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-14 03:17:46.000000 pytech_zp-0.0.2/pytech_zp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 03:17:46.157453 pytech_zp-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      510 2024-05-14 03:17:08.000000 pytech_zp-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:39:11.247542 pytech_zp-0.1.0/
+-rw-rw-rw-   0        0        0     1091 2024-05-13 10:56:51.000000 pytech_zp-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0       33 2024-05-13 11:16:04.000000 pytech_zp-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1914 2024-05-21 12:39:11.245541 pytech_zp-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2024-05-13 10:55:50.000000 pytech_zp-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 12:39:11.231541 pytech_zp-0.1.0/getpricedata/
+-rw-rw-rw-   0        0        0       41 2024-05-21 11:43:07.000000 pytech_zp-0.1.0/getpricedata/__init__.py
+-rw-rw-rw-   0        0        0     1398 2024-05-17 08:27:09.000000 pytech_zp-0.1.0/getpricedata/getETFprice.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:39:11.234540 pytech_zp-0.1.0/pytech/
+-rw-rw-rw-   0        0        0       36 2024-05-14 02:16:03.000000 pytech_zp-0.1.0/pytech/__init__.py
+-rw-rw-rw-   0        0        0   413696 2024-05-21 11:32:00.000000 pytech_zp-0.1.0/pytech/pytech.cp39-win_amd64.pyd
+drwxrwxrwx   0        0        0        0 2024-05-21 12:39:11.243540 pytech_zp-0.1.0/pytech_zp.egg-info/
+-rw-rw-rw-   0        0        0     1914 2024-05-21 12:39:11.000000 pytech_zp-0.1.0/pytech_zp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-05-21 12:39:11.000000 pytech_zp-0.1.0/pytech_zp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 12:39:11.000000 pytech_zp-0.1.0/pytech_zp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-21 12:39:11.000000 pytech_zp-0.1.0/pytech_zp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-21 12:39:11.000000 pytech_zp-0.1.0/pytech_zp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 12:39:11.247542 pytech_zp-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      664 2024-05-21 12:38:15.000000 pytech_zp-0.1.0/setup.py
```

### Comparing `pytech_zp-0.0.2/LICENSE` & `pytech_zp-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytech_zp-0.0.2/PKG-INFO` & `pytech_zp-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: pytech-zp
-Version: 0.0.2
+Version: 0.1.0
 Summary: Python function package of technical indicators and patterns implemented by C++
 Author: Peng Zhao
+Author-email: zhaokehan86@163.com
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
@@ -20,14 +21,17 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: pyodbc
 
 # pytech
   
 Python package providing technical indicators and patterns implemented in C++.  
   
 ## Installation
```

### Comparing `pytech_zp-0.0.2/pytech_zp.egg-info/PKG-INFO` & `pytech_zp-0.1.0/pytech_zp.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: pytech-zp
-Version: 0.0.2
+Version: 0.1.0
 Summary: Python function package of technical indicators and patterns implemented by C++
 Author: Peng Zhao
+Author-email: zhaokehan86@163.com
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
@@ -20,14 +21,17 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: pyodbc
 
 # pytech
   
 Python package providing technical indicators and patterns implemented in C++.  
   
 ## Installation
```

