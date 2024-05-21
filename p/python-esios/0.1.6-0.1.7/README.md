# Comparing `tmp/python_esios-0.1.6.tar.gz` & `tmp/python_esios-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_esios-0.1.6.tar", last modified: Fri May 17 06:57:16 2024, max compression
+gzip compressed data, was "python_esios-0.1.7.tar", last modified: Tue May 21 15:51:22 2024, max compression
```

## Comparing `python_esios-0.1.6.tar` & `python_esios-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:57:16.327729 python_esios-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-17 06:57:08.000000 python_esios-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-17 06:57:16.327729 python_esios-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-17 06:57:08.000000 python_esios-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:57:16.323729 python_esios-0.1.6/esios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:57:08.000000 python_esios-0.1.6/esios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-17 06:57:08.000000 python_esios-0.1.6/esios/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:57:16.323729 python_esios-0.1.6/esios/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-17 06:57:08.000000 python_esios-0.1.6/esios/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:57:16.323729 python_esios-0.1.6/esios/endpoints/archives/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-17 06:57:08.000000 python_esios-0.1.6/esios/endpoints/archives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:57:16.323729 python_esios-0.1.6/esios/endpoints/archives/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-17 06:57:08.000000 python_esios-0.1.6/esios/endpoints/archives/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-17 06:57:08.000000 python_esios-0.1.6/esios/endpoints/archives/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:57:16.323729 python_esios-0.1.6/esios/endpoints/indicators/
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-17 06:57:08.000000 python_esios-0.1.6/esios/endpoints/indicators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:57:16.327729 python_esios-0.1.6/python_esios.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-17 06:57:16.000000 python_esios-0.1.6/python_esios.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-17 06:57:16.000000 python_esios-0.1.6/python_esios.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:57:16.000000 python_esios-0.1.6/python_esios.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-17 06:57:16.000000 python_esios-0.1.6/python_esios.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 06:57:16.000000 python_esios-0.1.6/python_esios.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 06:57:16.327729 python_esios-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-17 06:57:08.000000 python_esios-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:51:22.057422 python_esios-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-21 15:51:14.000000 python_esios-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-21 15:51:22.057422 python_esios-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-21 15:51:14.000000 python_esios-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:51:22.053422 python_esios-0.1.7/esios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:51:14.000000 python_esios-0.1.7/esios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-21 15:51:14.000000 python_esios-0.1.7/esios/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:51:22.053422 python_esios-0.1.7/esios/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-21 15:51:14.000000 python_esios-0.1.7/esios/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:51:22.053422 python_esios-0.1.7/esios/endpoints/archives/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-21 15:51:14.000000 python_esios-0.1.7/esios/endpoints/archives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:51:22.057422 python_esios-0.1.7/esios/endpoints/archives/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-21 15:51:14.000000 python_esios-0.1.7/esios/endpoints/archives/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-21 15:51:14.000000 python_esios-0.1.7/esios/endpoints/archives/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:51:22.057422 python_esios-0.1.7/esios/endpoints/indicators/
+-rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-05-21 15:51:14.000000 python_esios-0.1.7/esios/endpoints/indicators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:51:22.057422 python_esios-0.1.7/python_esios.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-21 15:51:22.000000 python_esios-0.1.7/python_esios.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-21 15:51:22.000000 python_esios-0.1.7/python_esios.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:51:22.000000 python_esios-0.1.7/python_esios.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 15:51:22.000000 python_esios-0.1.7/python_esios.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 15:51:22.000000 python_esios-0.1.7/python_esios.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:51:22.057422 python_esios-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-21 15:51:14.000000 python_esios-0.1.7/setup.py
```

### Comparing `python_esios-0.1.6/LICENSE` & `python_esios-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_esios-0.1.6/PKG-INFO` & `python_esios-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-esios
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python wrapper for the ESIOS API
 Home-page: https://github.com/datons/python-esios
 Author: Jesús López
 Author-email: jesus.lopez@datons.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_esios-0.1.6/esios/api_client.py` & `python_esios-0.1.7/esios/api_client.py`

 * *Files identical despite different names*

### Comparing `python_esios-0.1.6/esios/endpoints/archives/__init__.py` & `python_esios-0.1.7/esios/endpoints/archives/__init__.py`

 * *Files identical despite different names*

### Comparing `python_esios-0.1.6/esios/endpoints/archives/utils.py` & `python_esios-0.1.7/esios/endpoints/archives/utils.py`

 * *Files identical despite different names*

### Comparing `python_esios-0.1.6/esios/endpoints/indicators/__init__.py` & `python_esios-0.1.7/esios/endpoints/indicators/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         
         params = {}
         if start_date:
             params['start_date'] = start_date
         if end_date:
             params['end_date'] = end_date + 'T23:59:59'
         if geo_ids:
-            params['geo_ids'] = ','.join(map(str, geo_ids))
+            params['geo_ids[]'] = ','.join(map(str, geo_ids))
         if locale:
             params['locale'] = locale
         if time_agg:
             params['time_agg'] = time_agg
         if geo_agg:
             params['geo_agg'] = geo_agg
         if time_trunc:
```

### Comparing `python_esios-0.1.6/python_esios.egg-info/PKG-INFO` & `python_esios-0.1.7/python_esios.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-esios
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python wrapper for the ESIOS API
 Home-page: https://github.com/datons/python-esios
 Author: Jesús López
 Author-email: jesus.lopez@datons.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_esios-0.1.6/setup.py` & `python_esios-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='utf-8')
 
 setup(
     name='python-esios',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(),
     install_requires=[
         'requests',
         'pandas',
     ],
     author="Jesús López",
     author_email="jesus.lopez@datons.ai",
```

