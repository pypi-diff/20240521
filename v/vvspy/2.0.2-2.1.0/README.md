# Comparing `tmp/vvspy-2.0.2.tar.gz` & `tmp/vvspy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vvspy-2.0.2.tar", last modified: Mon May 20 11:49:14 2024, max compression
+gzip compressed data, was "vvspy-2.1.0.tar", last modified: Tue May 21 19:04:20 2024, max compression
```

## Comparing `vvspy-2.0.2.tar` & `vvspy-2.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:49:14.799428 vvspy-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-20 11:49:05.000000 vvspy-2.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-20 11:49:05.000000 vvspy-2.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-20 11:49:05.000000 vvspy-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-20 11:49:05.000000 vvspy-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-05-20 11:49:14.799428 vvspy-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 11:49:05.000000 vvspy-2.0.2/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-20 11:49:05.000000 vvspy-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-20 11:49:05.000000 vvspy-2.0.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 11:49:05.000000 vvspy-2.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 11:49:14.799428 vvspy-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-20 11:49:05.000000 vvspy-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:49:14.795428 vvspy-2.0.2/vvspy/
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-20 11:49:05.000000 vvspy-2.0.2/vvspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-20 11:49:05.000000 vvspy-2.0.2/vvspy/arrivals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-20 11:49:05.000000 vvspy-2.0.2/vvspy/departures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:49:14.795428 vvspy-2.0.2/vvspy/enums/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 11:49:05.000000 vvspy-2.0.2/vvspy/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1576406 2024-05-20 11:49:05.000000 vvspy-2.0.2/vvspy/enums/stations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:49:14.799428 vvspy-2.0.2/vvspy/models/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-20 11:49:05.000000 vvspy-2.0.2/vvspy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-20 11:49:05.000000 vvspy-2.0.2/vvspy/models/arrival.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-20 11:49:05.000000 vvspy-2.0.2/vvspy/models/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-20 11:49:05.000000 vvspy-2.0.2/vvspy/models/departure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-20 11:49:05.000000 vvspy-2.0.2/vvspy/models/destination.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-20 11:49:05.000000 vvspy-2.0.2/vvspy/models/line_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-20 11:49:05.000000 vvspy-2.0.2/vvspy/models/origin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-20 11:49:05.000000 vvspy-2.0.2/vvspy/models/serving_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-20 11:49:05.000000 vvspy-2.0.2/vvspy/models/transportation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-20 11:49:05.000000 vvspy-2.0.2/vvspy/models/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-20 11:49:05.000000 vvspy-2.0.2/vvspy/trip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:49:14.799428 vvspy-2.0.2/vvspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-05-20 11:49:14.000000 vvspy-2.0.2/vvspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-20 11:49:14.000000 vvspy-2.0.2/vvspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:49:14.000000 vvspy-2.0.2/vvspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 11:49:14.000000 vvspy-2.0.2/vvspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 11:49:14.000000 vvspy-2.0.2/vvspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:20.760009 vvspy-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-21 19:04:10.000000 vvspy-2.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-21 19:04:10.000000 vvspy-2.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-21 19:04:10.000000 vvspy-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-21 19:04:10.000000 vvspy-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-05-21 19:04:20.760009 vvspy-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 19:04:10.000000 vvspy-2.1.0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-21 19:04:10.000000 vvspy-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-21 19:04:10.000000 vvspy-2.1.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 19:04:10.000000 vvspy-2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 19:04:20.760009 vvspy-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-21 19:04:10.000000 vvspy-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:20.752009 vvspy-2.1.0/vvspy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-21 19:04:10.000000 vvspy-2.1.0/vvspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-21 19:04:10.000000 vvspy-2.1.0/vvspy/arrivals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-21 19:04:10.000000 vvspy-2.1.0/vvspy/departures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:20.756009 vvspy-2.1.0/vvspy/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-21 19:04:10.000000 vvspy-2.1.0/vvspy/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1576406 2024-05-21 19:04:10.000000 vvspy-2.1.0/vvspy/enums/stations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:20.760009 vvspy-2.1.0/vvspy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-21 19:04:10.000000 vvspy-2.1.0/vvspy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-21 19:04:10.000000 vvspy-2.1.0/vvspy/models/arrival.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-21 19:04:10.000000 vvspy-2.1.0/vvspy/models/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-21 19:04:10.000000 vvspy-2.1.0/vvspy/models/departure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-21 19:04:10.000000 vvspy-2.1.0/vvspy/models/destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-21 19:04:10.000000 vvspy-2.1.0/vvspy/models/line_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-21 19:04:10.000000 vvspy-2.1.0/vvspy/models/origin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-21 19:04:10.000000 vvspy-2.1.0/vvspy/models/serving_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-21 19:04:10.000000 vvspy-2.1.0/vvspy/models/transportation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-21 19:04:10.000000 vvspy-2.1.0/vvspy/models/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-21 19:04:10.000000 vvspy-2.1.0/vvspy/trip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:20.760009 vvspy-2.1.0/vvspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-05-21 19:04:20.000000 vvspy-2.1.0/vvspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-21 19:04:20.000000 vvspy-2.1.0/vvspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:04:20.000000 vvspy-2.1.0/vvspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 19:04:20.000000 vvspy-2.1.0/vvspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 19:04:20.000000 vvspy-2.1.0/vvspy.egg-info/top_level.txt
```

### Comparing `vvspy-2.0.2/CODE_OF_CONDUCT.md` & `vvspy-2.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.2/CONTRIBUTING.md` & `vvspy-2.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.2/LICENSE` & `vvspy-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.2/PKG-INFO` & `vvspy-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: vvspy
-Version: 2.0.2
+Version: 2.1.0
 Summary: API Wrapper for VVS (Verkehrsverbund Stuttgart)
 Home-page: https://github.com/zaanposni/vvspy
 Author: zaanposni
 Author-email: vvspy@zaanposni.com
 License: MIT
 Keywords: vvs,api,stuttgart,wrapper,json,rest,efa,python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: typing
 
 # 🚂 VVS API Wrapper
 
@@ -32,16 +30,14 @@
 [![PythonVersions][python_versions_img]][python_versions_img]
 [![License][repo_license_img]][repo_license_url]
 
 **Fully object-oriented library** to integrate the **VVS API** into your project.
 
 ## Installation
 
-Python 3.6 or higher required
-
 ```bash
 pip install vvspy
 ```
 
 ## Examples
 
 - Detect delay in upcoming departures:
@@ -97,15 +93,15 @@
 
 ### Get your station id
 
 See: [#64][station_id_issue_url]
 
 ### Logging
 
-vvspy uses the python logging module. If you want to change the log level of vvsp, use the following:
+vvspy uses the python logging module. If you want to change the log level of vvspy, use the following:
 
 ```python
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("vvspy")
 logger.setLevel(logging.DEBUG)
```

### Comparing `vvspy-2.0.2/readme.md` & `vvspy-2.1.0/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 [![PythonVersions][python_versions_img]][python_versions_img]
 [![License][repo_license_img]][repo_license_url]
 
 **Fully object-oriented library** to integrate the **VVS API** into your project.
 
 ## Installation
 
-Python 3.6 or higher required
-
 ```bash
 pip install vvspy
 ```
 
 ## Examples
 
 - Detect delay in upcoming departures:
@@ -69,15 +67,15 @@
 
 ### Get your station id
 
 See: [#64][station_id_issue_url]
 
 ### Logging
 
-vvspy uses the python logging module. If you want to change the log level of vvsp, use the following:
+vvspy uses the python logging module. If you want to change the log level of vvspy, use the following:
 
 ```python
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("vvspy")
 logger.setLevel(logging.DEBUG)
```

### Comparing `vvspy-2.0.2/setup.py` & `vvspy-2.1.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="vvspy",
-    version="2.0.2",
+    version="2.1.0",
     license="MIT",
     description="API Wrapper for VVS (Verkehrsverbund Stuttgart)",
     author="zaanposni",
     author_email="vvspy@zaanposni.com",
     url="https://github.com/zaanposni/vvspy",
     keywords=["vvs", "api", "stuttgart", "wrapper", "json", "rest", "efa", "python"],
     packages=find_packages(exclude=["*tests"]),
     package_data={"vvspy": ["vvspy/*"]},
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     install_requires=[
         "requests",
         "typing",
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Operating System :: OS Independent",
     ],
```

### Comparing `vvspy-2.0.2/vvspy/__init__.py` & `vvspy-2.1.0/vvspy/__init__.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.2/vvspy/arrivals.py` & `vvspy-2.1.0/vvspy/arrivals.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.2/vvspy/departures.py` & `vvspy-2.1.0/vvspy/departures.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.2/vvspy/enums/stations.py` & `vvspy-2.1.0/vvspy/enums/stations.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.2/vvspy/models/arrival.py` & `vvspy-2.1.0/vvspy/models/arrival.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.2/vvspy/models/connection.py` & `vvspy-2.1.0/vvspy/models/connection.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.2/vvspy/models/departure.py` & `vvspy-2.1.0/vvspy/models/departure.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.2/vvspy/models/destination.py` & `vvspy-2.1.0/vvspy/models/destination.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.2/vvspy/models/line_operator.py` & `vvspy-2.1.0/vvspy/models/line_operator.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.2/vvspy/models/origin.py` & `vvspy-2.1.0/vvspy/models/origin.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.2/vvspy/models/serving_line.py` & `vvspy-2.1.0/vvspy/models/serving_line.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.2/vvspy/models/transportation.py` & `vvspy-2.1.0/vvspy/models/transportation.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.2/vvspy/models/trip.py` & `vvspy-2.1.0/vvspy/models/trip.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.2/vvspy/trip.py` & `vvspy-2.1.0/vvspy/trip.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.2/vvspy.egg-info/PKG-INFO` & `vvspy-2.1.0/vvspy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: vvspy
-Version: 2.0.2
+Version: 2.1.0
 Summary: API Wrapper for VVS (Verkehrsverbund Stuttgart)
 Home-page: https://github.com/zaanposni/vvspy
 Author: zaanposni
 Author-email: vvspy@zaanposni.com
 License: MIT
 Keywords: vvs,api,stuttgart,wrapper,json,rest,efa,python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: typing
 
 # 🚂 VVS API Wrapper
 
@@ -32,16 +30,14 @@
 [![PythonVersions][python_versions_img]][python_versions_img]
 [![License][repo_license_img]][repo_license_url]
 
 **Fully object-oriented library** to integrate the **VVS API** into your project.
 
 ## Installation
 
-Python 3.6 or higher required
-
 ```bash
 pip install vvspy
 ```
 
 ## Examples
 
 - Detect delay in upcoming departures:
@@ -97,15 +93,15 @@
 
 ### Get your station id
 
 See: [#64][station_id_issue_url]
 
 ### Logging
 
-vvspy uses the python logging module. If you want to change the log level of vvsp, use the following:
+vvspy uses the python logging module. If you want to change the log level of vvspy, use the following:
 
 ```python
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("vvspy")
 logger.setLevel(logging.DEBUG)
```

### Comparing `vvspy-2.0.2/vvspy.egg-info/SOURCES.txt` & `vvspy-2.1.0/vvspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

