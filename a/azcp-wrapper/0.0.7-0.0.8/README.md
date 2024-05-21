# Comparing `tmp/azcp_wrapper-0.0.7.tar.gz` & `tmp/azcp_wrapper-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azcp_wrapper-0.0.7.tar", last modified: Sat May 18 16:03:23 2024, max compression
+gzip compressed data, was "azcp_wrapper-0.0.8.tar", last modified: Tue May 21 16:30:29 2024, max compression
```

## Comparing `azcp_wrapper-0.0.7.tar` & `azcp_wrapper-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:03:23.414786 azcp_wrapper-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-18 16:03:23.414786 azcp_wrapper-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:03:23.410786 azcp_wrapper-0.0.7/azcp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9767 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/azcp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/azcp_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    14580 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/azcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:03:23.410786 azcp_wrapper-0.0.7/azcp_wrapper/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/utils/execute_command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:03:23.410786 azcp_wrapper-0.0.7/azcp_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-18 16:03:23.000000 azcp_wrapper-0.0.7/azcp_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-18 16:03:23.000000 azcp_wrapper-0.0.7/azcp_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 16:03:23.000000 azcp_wrapper-0.0.7/azcp_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-18 16:03:23.000000 azcp_wrapper-0.0.7/azcp_wrapper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-18 16:03:23.000000 azcp_wrapper-0.0.7/azcp_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-18 16:03:23.000000 azcp_wrapper-0.0.7/azcp_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 16:03:23.414786 azcp_wrapper-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:30:29.459838 azcp_wrapper-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-21 16:30:25.000000 azcp_wrapper-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-21 16:30:29.459838 azcp_wrapper-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-21 16:30:25.000000 azcp_wrapper-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:30:29.455837 azcp_wrapper-0.0.8/azcp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 16:30:25.000000 azcp_wrapper-0.0.8/azcp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9767 2024-05-21 16:30:25.000000 azcp_wrapper-0.0.8/azcp_wrapper/azcp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-21 16:30:25.000000 azcp_wrapper-0.0.8/azcp_wrapper/azcp_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14580 2024-05-21 16:30:25.000000 azcp_wrapper-0.0.8/azcp_wrapper/azcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-05-21 16:30:25.000000 azcp_wrapper-0.0.8/azcp_wrapper/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-21 16:30:25.000000 azcp_wrapper-0.0.8/azcp_wrapper/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:30:29.459838 azcp_wrapper-0.0.8/azcp_wrapper/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 16:30:25.000000 azcp_wrapper-0.0.8/azcp_wrapper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-21 16:30:25.000000 azcp_wrapper-0.0.8/azcp_wrapper/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-21 16:30:25.000000 azcp_wrapper-0.0.8/azcp_wrapper/utils/execute_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:30:29.459838 azcp_wrapper-0.0.8/azcp_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-21 16:30:29.000000 azcp_wrapper-0.0.8/azcp_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-21 16:30:29.000000 azcp_wrapper-0.0.8/azcp_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 16:30:29.000000 azcp_wrapper-0.0.8/azcp_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 16:30:29.000000 azcp_wrapper-0.0.8/azcp_wrapper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-21 16:30:29.000000 azcp_wrapper-0.0.8/azcp_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 16:30:29.000000 azcp_wrapper-0.0.8/azcp_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 16:30:29.459838 azcp_wrapper-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-21 16:30:25.000000 azcp_wrapper-0.0.8/setup.py
```

### Comparing `azcp_wrapper-0.0.7/LICENSE` & `azcp_wrapper-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `azcp_wrapper-0.0.7/PKG-INFO` & `azcp_wrapper-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azcp_wrapper
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple AzCopy wrapper to transfer data
 Home-page: https://github.com/eabdala/azcp_wrapper
 Author: Erik Alejandro Abdala
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `azcp_wrapper-0.0.7/azcp_wrapper/azcp_client.py` & `azcp_wrapper-0.0.8/azcp_wrapper/azcp_client.py`

 * *Files identical despite different names*

### Comparing `azcp_wrapper-0.0.7/azcp_wrapper/azcp_summary.py` & `azcp_wrapper-0.0.8/azcp_wrapper/azcp_summary.py`

 * *Files identical despite different names*

### Comparing `azcp_wrapper-0.0.7/azcp_wrapper/azcp_utils.py` & `azcp_wrapper-0.0.8/azcp_wrapper/azcp_utils.py`

 * *Files identical despite different names*

### Comparing `azcp_wrapper-0.0.7/azcp_wrapper/logging_config.py` & `azcp_wrapper-0.0.8/azcp_wrapper/logging_config.py`

 * *Files identical despite different names*

### Comparing `azcp_wrapper-0.0.7/azcp_wrapper/setup.py` & `azcp_wrapper-0.0.8/azcp_wrapper/setup.py`

 * *Files identical despite different names*

### Comparing `azcp_wrapper-0.0.7/azcp_wrapper/utils/execute_command.py` & `azcp_wrapper-0.0.8/azcp_wrapper/utils/execute_command.py`

 * *Files identical despite different names*

### Comparing `azcp_wrapper-0.0.7/azcp_wrapper.egg-info/PKG-INFO` & `azcp_wrapper-0.0.8/azcp_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azcp_wrapper
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple AzCopy wrapper to transfer data
 Home-page: https://github.com/eabdala/azcp_wrapper
 Author: Erik Alejandro Abdala
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `azcp_wrapper-0.0.7/setup.py` & `azcp_wrapper-0.0.8/setup.py`

 * *Files identical despite different names*

