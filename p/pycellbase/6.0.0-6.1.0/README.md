# Comparing `tmp/pycellbase-6.0.0.tar.gz` & `tmp/pycellbase-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycellbase-6.0.0.tar", last modified: Mon Mar  4 16:13:48 2024, max compression
+gzip compressed data, was "pycellbase-6.1.0.tar", last modified: Tue May 21 09:22:14 2024, max compression
```

## Comparing `pycellbase-6.0.0.tar` & `pycellbase-6.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 juanfe    (1000) juanfe    (1000)        0 2024-03-04 16:13:48.793561 pycellbase-6.0.0/
--rw-rw-r--   0 juanfe    (1000) juanfe    (1000)    11303 2024-03-04 16:09:39.000000 pycellbase-6.0.0/LICENSE.txt
--rwxrwxr-x   0 juanfe    (1000) juanfe    (1000)       76 2024-03-04 16:09:39.000000 pycellbase-6.0.0/MANIFEST.in
--rw-r--r--   0 juanfe    (1000) juanfe    (1000)     9786 2024-03-04 16:13:48.793561 pycellbase-6.0.0/PKG-INFO
--rwxrwxr-x   0 juanfe    (1000) juanfe    (1000)     8495 2024-03-04 16:09:39.000000 pycellbase-6.0.0/README.rst
-drwxrwxr-x   0 juanfe    (1000) juanfe    (1000)        0 2024-03-04 16:13:48.793561 pycellbase-6.0.0/pycellbase/
--rwxrwxr-x   0 juanfe    (1000) juanfe    (1000)       22 2024-03-04 16:09:39.000000 pycellbase-6.0.0/pycellbase/__init__.py
--rwxrwxr-x   0 juanfe    (1000) juanfe    (1000)     6256 2024-03-04 16:09:39.000000 pycellbase-6.0.0/pycellbase/cbclient.py
--rwxrwxr-x   0 juanfe    (1000) juanfe    (1000)     4444 2024-03-04 16:09:39.000000 pycellbase-6.0.0/pycellbase/cbconfig.py
--rwxrwxr-x   0 juanfe    (1000) juanfe    (1000)    23967 2024-03-04 16:09:39.000000 pycellbase-6.0.0/pycellbase/cbrestclients.py
--rw-rw-r--   0 juanfe    (1000) juanfe    (1000)    10601 2024-03-04 16:09:39.000000 pycellbase-6.0.0/pycellbase/commons.py
-drwxrwxr-x   0 juanfe    (1000) juanfe    (1000)        0 2024-03-04 16:13:48.793561 pycellbase-6.0.0/pycellbase.egg-info/
--rw-r--r--   0 juanfe    (1000) juanfe    (1000)     9786 2024-03-04 16:13:48.000000 pycellbase-6.0.0/pycellbase.egg-info/PKG-INFO
--rw-rw-r--   0 juanfe    (1000) juanfe    (1000)      455 2024-03-04 16:13:48.000000 pycellbase-6.0.0/pycellbase.egg-info/SOURCES.txt
--rw-rw-r--   0 juanfe    (1000) juanfe    (1000)        1 2024-03-04 16:13:48.000000 pycellbase-6.0.0/pycellbase.egg-info/dependency_links.txt
--rw-rw-r--   0 juanfe    (1000) juanfe    (1000)       25 2024-03-04 16:13:48.000000 pycellbase-6.0.0/pycellbase.egg-info/requires.txt
--rw-rw-r--   0 juanfe    (1000) juanfe    (1000)       11 2024-03-04 16:13:48.000000 pycellbase-6.0.0/pycellbase.egg-info/top_level.txt
--rw-rw-r--   0 juanfe    (1000) juanfe    (1000)      106 2024-03-04 16:13:48.793561 pycellbase-6.0.0/setup.cfg
--rwxrwxr-x   0 juanfe    (1000) juanfe    (1000)     1881 2024-03-04 16:09:39.000000 pycellbase-6.0.0/setup.py
-drwxrwxr-x   0 juanfe    (1000) juanfe    (1000)        0 2024-03-04 16:13:48.793561 pycellbase-6.0.0/tests/
--rw-rw-r--   0 juanfe    (1000) juanfe    (1000)     1108 2024-03-04 16:09:39.000000 pycellbase-6.0.0/tests/test_cbcclient.py
--rw-rw-r--   0 juanfe    (1000) juanfe    (1000)     2223 2024-03-04 16:09:39.000000 pycellbase-6.0.0/tests/test_cbconfig.py
--rwxrwxr-x   0 juanfe    (1000) juanfe    (1000)     7814 2024-03-04 16:09:39.000000 pycellbase-6.0.0/tests/test_cbrestclients.py
--rw-rw-r--   0 juanfe    (1000) juanfe    (1000)     8124 2024-03-04 16:09:39.000000 pycellbase-6.0.0/tests/test_commons.py
-drwxrwxr-x   0 juanfe    (1000) juanfe    (1000)        0 2024-03-04 16:13:48.793561 pycellbase-6.0.0/tools/
--rw-rw-r--   0 juanfe    (1000) juanfe    (1000)    23900 2024-03-04 16:09:39.000000 pycellbase-6.0.0/tools/cbtools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:22:14.437135 pycellbase-6.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-05-21 09:22:11.000000 pycellbase-6.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-21 09:22:11.000000 pycellbase-6.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-05-21 09:22:14.437135 pycellbase-6.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-05-21 09:22:11.000000 pycellbase-6.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:22:14.433135 pycellbase-6.1.0/pycellbase/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 09:22:11.000000 pycellbase-6.1.0/pycellbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-21 09:22:11.000000 pycellbase-6.1.0/pycellbase/cbclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-21 09:22:11.000000 pycellbase-6.1.0/pycellbase/cbconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23967 2024-05-21 09:22:11.000000 pycellbase-6.1.0/pycellbase/cbrestclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10601 2024-05-21 09:22:11.000000 pycellbase-6.1.0/pycellbase/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:22:14.437135 pycellbase-6.1.0/pycellbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-05-21 09:22:14.000000 pycellbase-6.1.0/pycellbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-21 09:22:14.000000 pycellbase-6.1.0/pycellbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:22:14.000000 pycellbase-6.1.0/pycellbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 09:22:14.000000 pycellbase-6.1.0/pycellbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 09:22:14.000000 pycellbase-6.1.0/pycellbase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-21 09:22:14.437135 pycellbase-6.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-21 09:22:11.000000 pycellbase-6.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:22:14.437135 pycellbase-6.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-21 09:22:11.000000 pycellbase-6.1.0/tests/test_cbcclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-21 09:22:11.000000 pycellbase-6.1.0/tests/test_cbconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-05-21 09:22:11.000000 pycellbase-6.1.0/tests/test_cbrestclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8124 2024-05-21 09:22:11.000000 pycellbase-6.1.0/tests/test_commons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:22:14.437135 pycellbase-6.1.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    23900 2024-05-21 09:22:11.000000 pycellbase-6.1.0/tools/cbtools.py
```

### Comparing `pycellbase-6.0.0/LICENSE.txt` & `pycellbase-6.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycellbase-6.0.0/PKG-INFO` & `pycellbase-6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycellbase
-Version: 6.0.0
+Version: 6.1.0
 Summary: Python client for CellBase
 Home-page: https://github.com/opencb/cellbase/tree/develop/clients/python
 Author: Daniel Perez-Gil
 Author-email: dperezgil89@gmail.com
 License: Apache Software License
 Project-URL: Documentation, http://docs.opencb.org/display/cellbase/RESTful+Web+Services
 Project-URL: Tutorial, http://docs.opencb.org/display/cellbase/Python+client+library
```

### Comparing `pycellbase-6.0.0/README.rst` & `pycellbase-6.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pycellbase-6.0.0/pycellbase/cbclient.py` & `pycellbase-6.1.0/pycellbase/cbclient.py`

 * *Files identical despite different names*

### Comparing `pycellbase-6.0.0/pycellbase/cbconfig.py` & `pycellbase-6.1.0/pycellbase/cbconfig.py`

 * *Files identical despite different names*

### Comparing `pycellbase-6.0.0/pycellbase/cbrestclients.py` & `pycellbase-6.1.0/pycellbase/cbrestclients.py`

 * *Files identical despite different names*

### Comparing `pycellbase-6.0.0/pycellbase/commons.py` & `pycellbase-6.1.0/pycellbase/commons.py`

 * *Files identical despite different names*

### Comparing `pycellbase-6.0.0/pycellbase.egg-info/PKG-INFO` & `pycellbase-6.1.0/pycellbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycellbase
-Version: 6.0.0
+Version: 6.1.0
 Summary: Python client for CellBase
 Home-page: https://github.com/opencb/cellbase/tree/develop/clients/python
 Author: Daniel Perez-Gil
 Author-email: dperezgil89@gmail.com
 License: Apache Software License
 Project-URL: Documentation, http://docs.opencb.org/display/cellbase/RESTful+Web+Services
 Project-URL: Tutorial, http://docs.opencb.org/display/cellbase/Python+client+library
```

### Comparing `pycellbase-6.0.0/setup.py` & `pycellbase-6.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup_kwargs = {
     'name': 'pycellbase',
-    'version': '6.0.0',
+    'version': '6.1.0',
     'description': 'Python client for CellBase',
     'long_description': long_description,
     'long_description_content_type': 'text/x-rst',
     'url': 'https://github.com/opencb/cellbase/tree/develop/clients/python',
     'author': 'Daniel Perez-Gil',
     'author_email': 'dperezgil89@gmail.com',
     'license': 'Apache Software License',
```

### Comparing `pycellbase-6.0.0/tests/test_cbcclient.py` & `pycellbase-6.1.0/tests/test_cbcclient.py`

 * *Files identical despite different names*

### Comparing `pycellbase-6.0.0/tests/test_cbconfig.py` & `pycellbase-6.1.0/tests/test_cbconfig.py`

 * *Files identical despite different names*

### Comparing `pycellbase-6.0.0/tests/test_cbrestclients.py` & `pycellbase-6.1.0/tests/test_cbrestclients.py`

 * *Files identical despite different names*

### Comparing `pycellbase-6.0.0/tests/test_commons.py` & `pycellbase-6.1.0/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `pycellbase-6.0.0/tools/cbtools.py` & `pycellbase-6.1.0/tools/cbtools.py`

 * *Files identical despite different names*

