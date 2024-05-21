# Comparing `tmp/dwd_global_radiation-1.0.0rc4.tar.gz` & `tmp/dwd_global_radiation-1.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwd_global_radiation-1.0.0rc4.tar", last modified: Fri May 17 11:21:39 2024, max compression
+gzip compressed data, was "dwd_global_radiation-1.0.0rc5.tar", last modified: Tue May 21 11:01:52 2024, max compression
```

## Comparing `dwd_global_radiation-1.0.0rc4.tar` & `dwd_global_radiation-1.0.0rc5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-17 11:21:39.906342 dwd_global_radiation-1.0.0rc4/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1065 2024-05-05 09:59:58.000000 dwd_global_radiation-1.0.0rc4/LICENSE
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-17 11:21:39.906342 dwd_global_radiation-1.0.0rc4/PKG-INFO
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    21423 2024-05-15 22:21:14.000000 dwd_global_radiation-1.0.0rc4/README.md
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-17 11:21:39.902342 dwd_global_radiation-1.0.0rc4/dwd_global_radiation/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       45 2024-05-07 07:51:24.000000 dwd_global_radiation-1.0.0rc4/dwd_global_radiation/__init__.py
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    23928 2024-05-17 10:30:25.000000 dwd_global_radiation-1.0.0rc4/dwd_global_radiation/global_radiation.py
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    18137 2024-05-15 21:06:36.000000 dwd_global_radiation-1.0.0rc4/dwd_global_radiation/utils.py
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-17 11:21:39.906342 dwd_global_radiation-1.0.0rc4/dwd_global_radiation.egg-info/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-17 11:21:39.000000 dwd_global_radiation-1.0.0rc4/dwd_global_radiation.egg-info/PKG-INFO
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)      349 2024-05-17 11:21:39.000000 dwd_global_radiation-1.0.0rc4/dwd_global_radiation.egg-info/SOURCES.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)        1 2024-05-17 11:21:39.000000 dwd_global_radiation-1.0.0rc4/dwd_global_radiation.egg-info/dependency_links.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)      128 2024-05-17 11:21:39.000000 dwd_global_radiation-1.0.0rc4/dwd_global_radiation.egg-info/requires.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       21 2024-05-17 11:21:39.000000 dwd_global_radiation-1.0.0rc4/dwd_global_radiation.egg-info/top_level.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       38 2024-05-17 11:21:39.906342 dwd_global_radiation-1.0.0rc4/setup.cfg
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1656 2024-05-17 10:43:19.000000 dwd_global_radiation-1.0.0rc4/setup.py
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-21 11:01:52.151512 dwd_global_radiation-1.0.0rc5/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1065 2024-05-05 09:59:58.000000 dwd_global_radiation-1.0.0rc5/LICENSE
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-21 11:01:52.151512 dwd_global_radiation-1.0.0rc5/PKG-INFO
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    21423 2024-05-21 10:47:19.000000 dwd_global_radiation-1.0.0rc5/README.md
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-21 11:01:52.147512 dwd_global_radiation-1.0.0rc5/dwd_global_radiation/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       45 2024-05-07 07:51:24.000000 dwd_global_radiation-1.0.0rc5/dwd_global_radiation/__init__.py
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    23928 2024-05-17 10:30:25.000000 dwd_global_radiation-1.0.0rc5/dwd_global_radiation/global_radiation.py
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    18137 2024-05-15 21:06:36.000000 dwd_global_radiation-1.0.0rc5/dwd_global_radiation/utils.py
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-21 11:01:52.147512 dwd_global_radiation-1.0.0rc5/dwd_global_radiation.egg-info/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-21 11:01:52.000000 dwd_global_radiation-1.0.0rc5/dwd_global_radiation.egg-info/PKG-INFO
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)      349 2024-05-21 11:01:52.000000 dwd_global_radiation-1.0.0rc5/dwd_global_radiation.egg-info/SOURCES.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)        1 2024-05-21 11:01:52.000000 dwd_global_radiation-1.0.0rc5/dwd_global_radiation.egg-info/dependency_links.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)      128 2024-05-21 11:01:52.000000 dwd_global_radiation-1.0.0rc5/dwd_global_radiation.egg-info/requires.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       21 2024-05-21 11:01:52.000000 dwd_global_radiation-1.0.0rc5/dwd_global_radiation.egg-info/top_level.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       38 2024-05-21 11:01:52.151512 dwd_global_radiation-1.0.0rc5/setup.cfg
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1656 2024-05-21 10:47:19.000000 dwd_global_radiation-1.0.0rc5/setup.py
```

### Comparing `dwd_global_radiation-1.0.0rc4/LICENSE` & `dwd_global_radiation-1.0.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.0.0rc4/PKG-INFO` & `dwd_global_radiation-1.0.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwd_global_radiation
-Version: 1.0.0rc4
+Version: 1.0.0rc5
 Summary: Access and analyze DWD global radiation data and forecasts
 Home-page: https://github.com/aschmere/dwd_global_radiation
 Author: Arno Schmerer
 License: MIT
 Keywords: weather meteorology radiation solar forecasting DWD data environmental data climate studies solar energy forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,17 +13,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: netCDF4>=1.6.5
-Requires-Dist: numpy>=1.26.4
+Requires-Dist: numpy>=1.26.0
 Requires-Dist: pytz>=2024.1
-Requires-Dist: Requests>=2.31.0
+Requires-Dist: requests>=2.31.0
 Requires-Dist: tabulate>=0.9.0
 Requires-Dist: tzlocal>=5.2
 Requires-Dist: xarray>=2024.3.0
 
 DISCLAIMER: This project is a private open source project and is not affiliated with the German public meteorology service institute "Deutscher Wetterdienst" (DWD). However, it uses its publicly available data interfaces. 
 
 # Summary
@@ -38,22 +38,22 @@
 Complying with typical best practices for using Python it is highly recommended to create and use a python virtual environement [[4]](#R4) as installation target.
 ```
 python3 -m pip install dwd_global_radiation
 ```
 The listed installation command will usually install all required dependant Python packages.
 As of the current version of this package the following Python packages are required:
 ```
-beautifulsoup4==4.12.3
-netCDF4==1.6.5
-numpy==1.26.4
-pytz==2024.1
-Requests==2.31.0
-tabulate==0.9.0
-tzlocal==5.2
-xarray==2024.3.0
+beautifulsoup4>=4.12.3
+netCDF4>=1.6.5
+numpy>=1.26.0
+pytz>=2024.1
+requests>=2.31.0
+tabulate>=0.9.0
+tzlocal>=5.2
+xarray>=2024.3.0
 ```
 <ins>Note:</ins>The above listed versions of dependant Python packages reflect the versions, on which this package was developed and tested. Typically you would expect, that later versions of these packages will be compatible as well. Earlier versions might also be compatible. The Python version, with which this package
 was developed and tested, is 3.12.3.
 
 The workstation, on which you use Python along with this package, needs internet access, specifically via https protocol to the Open Data server of the DWD [[5]](#R5) in order to retrieve global radiation forecasts and observations.
 # Fast Track
```

### Comparing `dwd_global_radiation-1.0.0rc4/README.md` & `dwd_global_radiation-1.0.0rc5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 Complying with typical best practices for using Python it is highly recommended to create and use a python virtual environement [[4]](#R4) as installation target.
 ```
 python3 -m pip install dwd_global_radiation
 ```
 The listed installation command will usually install all required dependant Python packages.
 As of the current version of this package the following Python packages are required:
 ```
-beautifulsoup4==4.12.3
-netCDF4==1.6.5
-numpy==1.26.4
-pytz==2024.1
-Requests==2.31.0
-tabulate==0.9.0
-tzlocal==5.2
-xarray==2024.3.0
+beautifulsoup4>=4.12.3
+netCDF4>=1.6.5
+numpy>=1.26.0
+pytz>=2024.1
+requests>=2.31.0
+tabulate>=0.9.0
+tzlocal>=5.2
+xarray>=2024.3.0
 ```
 <ins>Note:</ins>The above listed versions of dependant Python packages reflect the versions, on which this package was developed and tested. Typically you would expect, that later versions of these packages will be compatible as well. Earlier versions might also be compatible. The Python version, with which this package
 was developed and tested, is 3.12.3.
 
 The workstation, on which you use Python along with this package, needs internet access, specifically via https protocol to the Open Data server of the DWD [[5]](#R5) in order to retrieve global radiation forecasts and observations.
 # Fast Track
```

### Comparing `dwd_global_radiation-1.0.0rc4/dwd_global_radiation/global_radiation.py` & `dwd_global_radiation-1.0.0rc5/dwd_global_radiation/global_radiation.py`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.0.0rc4/dwd_global_radiation/utils.py` & `dwd_global_radiation-1.0.0rc5/dwd_global_radiation/utils.py`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.0.0rc4/dwd_global_radiation.egg-info/PKG-INFO` & `dwd_global_radiation-1.0.0rc5/dwd_global_radiation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwd_global_radiation
-Version: 1.0.0rc4
+Version: 1.0.0rc5
 Summary: Access and analyze DWD global radiation data and forecasts
 Home-page: https://github.com/aschmere/dwd_global_radiation
 Author: Arno Schmerer
 License: MIT
 Keywords: weather meteorology radiation solar forecasting DWD data environmental data climate studies solar energy forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,17 +13,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: netCDF4>=1.6.5
-Requires-Dist: numpy>=1.26.4
+Requires-Dist: numpy>=1.26.0
 Requires-Dist: pytz>=2024.1
-Requires-Dist: Requests>=2.31.0
+Requires-Dist: requests>=2.31.0
 Requires-Dist: tabulate>=0.9.0
 Requires-Dist: tzlocal>=5.2
 Requires-Dist: xarray>=2024.3.0
 
 DISCLAIMER: This project is a private open source project and is not affiliated with the German public meteorology service institute "Deutscher Wetterdienst" (DWD). However, it uses its publicly available data interfaces. 
 
 # Summary
@@ -38,22 +38,22 @@
 Complying with typical best practices for using Python it is highly recommended to create and use a python virtual environement [[4]](#R4) as installation target.
 ```
 python3 -m pip install dwd_global_radiation
 ```
 The listed installation command will usually install all required dependant Python packages.
 As of the current version of this package the following Python packages are required:
 ```
-beautifulsoup4==4.12.3
-netCDF4==1.6.5
-numpy==1.26.4
-pytz==2024.1
-Requests==2.31.0
-tabulate==0.9.0
-tzlocal==5.2
-xarray==2024.3.0
+beautifulsoup4>=4.12.3
+netCDF4>=1.6.5
+numpy>=1.26.0
+pytz>=2024.1
+requests>=2.31.0
+tabulate>=0.9.0
+tzlocal>=5.2
+xarray>=2024.3.0
 ```
 <ins>Note:</ins>The above listed versions of dependant Python packages reflect the versions, on which this package was developed and tested. Typically you would expect, that later versions of these packages will be compatible as well. Earlier versions might also be compatible. The Python version, with which this package
 was developed and tested, is 3.12.3.
 
 The workstation, on which you use Python along with this package, needs internet access, specifically via https protocol to the Open Data server of the DWD [[5]](#R5) in order to retrieve global radiation forecasts and observations.
 # Fast Track
```

### Comparing `dwd_global_radiation-1.0.0rc4/setup.py` & `dwd_global_radiation-1.0.0rc5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='dwd_global_radiation',
-    version='1.0.0rc4',
+    version='1.0.0rc5',
     packages=find_packages(),
     description='Access and analyze DWD global radiation data and forecasts',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/aschmere/dwd_global_radiation',
     author='Arno Schmerer',
     license='MIT',
     install_requires=[
         'beautifulsoup4>=4.12.3',
         'netCDF4>=1.6.5',
-        'numpy>=1.26.4',
+        'numpy>=1.26.0',
         'pytz>=2024.1',
-        'Requests>=2.31.0',
+        'requests>=2.31.0',
         'tabulate>=0.9.0',
         'tzlocal>=5.2',
         'xarray>=2024.3.0'
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
```

