# Comparing `tmp/pyDetektia-2.1.0.tar.gz` & `tmp/pyDetektia-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDetektia-2.1.0.tar", last modified: Wed May 15 11:59:04 2024, max compression
+gzip compressed data, was "pyDetektia-2.1.1.tar", last modified: Tue May 21 15:24:02 2024, max compression
```

## Comparing `pyDetektia-2.1.0.tar` & `pyDetektia-2.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2024-05-15 11:59:04.173305 pyDetektia-2.1.0/
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        0 2023-06-19 12:15:27.000000 pyDetektia-2.1.0/LICENSE.txt
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      326 2024-05-15 11:59:04.173305 pyDetektia-2.1.0/PKG-INFO
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       13 2023-09-05 11:56:56.000000 pyDetektia-2.1.0/README.md
-drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2024-05-15 11:59:04.173305 pyDetektia-2.1.0/pyDetektia/
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        0 2022-07-11 08:00:56.000000 pyDetektia-2.1.0/pyDetektia/__init__.py
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)    45698 2024-05-15 11:54:58.000000 pyDetektia-2.1.0/pyDetektia/manager.py
-drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2024-05-15 11:59:04.173305 pyDetektia-2.1.0/pyDetektia.egg-info/
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      326 2024-05-15 11:59:04.000000 pyDetektia-2.1.0/pyDetektia.egg-info/PKG-INFO
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      244 2024-05-15 11:59:04.000000 pyDetektia-2.1.0/pyDetektia.egg-info/SOURCES.txt
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        1 2024-05-15 11:59:04.000000 pyDetektia-2.1.0/pyDetektia.egg-info/dependency_links.txt
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        9 2024-05-15 11:59:04.000000 pyDetektia-2.1.0/pyDetektia.egg-info/requires.txt
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       11 2024-05-15 11:59:04.000000 pyDetektia-2.1.0/pyDetektia.egg-info/top_level.txt
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       38 2024-05-15 11:59:04.173305 pyDetektia-2.1.0/setup.cfg
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      464 2024-05-15 11:58:37.000000 pyDetektia-2.1.0/setup.py
+drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2024-05-21 15:24:02.827543 pyDetektia-2.1.1/
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        0 2023-06-19 12:15:27.000000 pyDetektia-2.1.1/LICENSE.txt
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      326 2024-05-21 15:24:02.827543 pyDetektia-2.1.1/PKG-INFO
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       13 2023-09-05 11:56:56.000000 pyDetektia-2.1.1/README.md
+drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2024-05-21 15:24:02.827543 pyDetektia-2.1.1/pyDetektia/
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        0 2022-07-11 08:00:56.000000 pyDetektia-2.1.1/pyDetektia/__init__.py
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)    45690 2024-05-21 15:19:41.000000 pyDetektia-2.1.1/pyDetektia/manager.py
+drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2024-05-21 15:24:02.827543 pyDetektia-2.1.1/pyDetektia.egg-info/
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      326 2024-05-21 15:24:02.000000 pyDetektia-2.1.1/pyDetektia.egg-info/PKG-INFO
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      244 2024-05-21 15:24:02.000000 pyDetektia-2.1.1/pyDetektia.egg-info/SOURCES.txt
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        1 2024-05-21 15:24:02.000000 pyDetektia-2.1.1/pyDetektia.egg-info/dependency_links.txt
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        9 2024-05-21 15:24:02.000000 pyDetektia-2.1.1/pyDetektia.egg-info/requires.txt
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       11 2024-05-21 15:24:02.000000 pyDetektia-2.1.1/pyDetektia.egg-info/top_level.txt
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       38 2024-05-21 15:24:02.827543 pyDetektia-2.1.1/setup.cfg
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      464 2024-05-21 15:23:59.000000 pyDetektia-2.1.1/setup.py
```

### Comparing `pyDetektia-2.1.0/pyDetektia/manager.py` & `pyDetektia-2.1.1/pyDetektia/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -798,15 +798,15 @@
         '''
         Returns a list of scenarios names.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"{self._ip}/organization/{organization}/polygons"
+        url = f"{self._ip}/organization/{organization}/_polygons"
 
         ret = self.session.get(url, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = self.session.get(url, headers=self._headers)
 
         jsonret = ret.json()
@@ -820,15 +820,15 @@
         '''
         Returns a list of the loaded polygons metadata in this organization and scenario.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"{self._ip}/organization/{organization}/polygons"
+        url = f"{self._ip}/organization/{organization}/_polygons"
 
         ret = self.session.get(url, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = self.session.get(url, headers=self._headers)
 
         jsonret = ret.json()
@@ -1061,15 +1061,15 @@
 
     ###----------------------
     ##--------------------
     #--- usable methods
 
     #-----------------------#
     #--- manage datasets ---#
-    def add_dataset(self, dataset_json, title=None, scenario=None, organization=None):
+    def add_dataset(self, dataset_json, title, scenario, organization=None):
         '''
         This method adds new dataset data and metadata tables from the dataset_json object.
         '''
 
         if organization is None:
             organization = self._organization
```

