# Comparing `tmp/pycrtbp-0.1.5.tar.gz` & `tmp/pycrtbp-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrtbp-0.1.5.tar", last modified: Mon May 20 14:07:23 2024, max compression
+gzip compressed data, was "pycrtbp-0.1.6.tar", last modified: Tue May 21 17:57:42 2024, max compression
```

## Comparing `pycrtbp-0.1.5.tar` & `pycrtbp-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-05-20 14:07:23.146101 pycrtbp-0.1.5/
--rwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)     1073 2024-05-20 06:10:07.000000 pycrtbp-0.1.5/LICENSE
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)     3936 2024-05-20 14:07:23.146101 pycrtbp-0.1.5/PKG-INFO
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)     3433 2024-05-20 13:55:40.000000 pycrtbp-0.1.5/README.md
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)       38 2024-05-20 14:07:23.146101 pycrtbp-0.1.5/setup.cfg
--rwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)     2185 2024-05-20 14:07:19.000000 pycrtbp-0.1.5/setup.py
-drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-05-20 14:07:23.146101 pycrtbp-0.1.5/src/
-drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-05-20 14:07:23.146101 pycrtbp-0.1.5/src/pycrtbp/
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)      839 2024-05-20 06:01:47.000000 pycrtbp-0.1.5/src/pycrtbp/__init__.py
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)      773 2024-05-20 05:40:22.000000 pycrtbp-0.1.5/src/pycrtbp/particles.py
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)    16499 2024-05-20 08:35:38.000000 pycrtbp-0.1.5/src/pycrtbp/system.py
--rwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)       16 2024-05-20 14:07:19.000000 pycrtbp-0.1.5/src/pycrtbp/version.py
-drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-05-20 14:07:23.146101 pycrtbp-0.1.5/src/pycrtbp.egg-info/
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)     3936 2024-05-20 14:07:23.000000 pycrtbp-0.1.5/src/pycrtbp.egg-info/PKG-INFO
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)      332 2024-05-20 14:07:23.000000 pycrtbp-0.1.5/src/pycrtbp.egg-info/SOURCES.txt
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)        1 2024-05-20 14:07:23.000000 pycrtbp-0.1.5/src/pycrtbp.egg-info/dependency_links.txt
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)       48 2024-05-20 14:07:23.000000 pycrtbp-0.1.5/src/pycrtbp.egg-info/entry_points.txt
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)       13 2024-05-20 14:07:23.000000 pycrtbp-0.1.5/src/pycrtbp.egg-info/requires.txt
--rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)        8 2024-05-20 14:07:23.000000 pycrtbp-0.1.5/src/pycrtbp.egg-info/top_level.txt
+drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-05-21 17:57:42.372262 pycrtbp-0.1.6/
+-rwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)     1073 2024-05-20 06:10:07.000000 pycrtbp-0.1.6/LICENSE
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)     4362 2024-05-21 17:57:42.342262 pycrtbp-0.1.6/PKG-INFO
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)     3859 2024-05-21 17:55:52.000000 pycrtbp-0.1.6/README.md
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)       38 2024-05-21 17:57:42.372262 pycrtbp-0.1.6/setup.cfg
+-rwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)     2185 2024-05-21 17:57:16.000000 pycrtbp-0.1.6/setup.py
+drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-05-21 17:57:42.272262 pycrtbp-0.1.6/src/
+drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-05-21 17:57:42.332262 pycrtbp-0.1.6/src/pycrtbp/
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)      876 2024-05-21 17:47:24.000000 pycrtbp-0.1.6/src/pycrtbp/__init__.py
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)      773 2024-05-20 05:40:22.000000 pycrtbp-0.1.6/src/pycrtbp/particles.py
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)       19 2024-05-21 17:47:07.000000 pycrtbp-0.1.6/src/pycrtbp/periodicorbits.py
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)    16499 2024-05-20 08:35:38.000000 pycrtbp-0.1.6/src/pycrtbp/system.py
+-rwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)       16 2024-05-21 17:57:16.000000 pycrtbp-0.1.6/src/pycrtbp/version.py
+drwxr-xr-x   0 jzuluaga  (1000) jzuluaga  (1000)        0 2024-05-21 17:57:42.342262 pycrtbp-0.1.6/src/pycrtbp.egg-info/
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)     4362 2024-05-21 17:57:42.000000 pycrtbp-0.1.6/src/pycrtbp.egg-info/PKG-INFO
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)      362 2024-05-21 17:57:42.000000 pycrtbp-0.1.6/src/pycrtbp.egg-info/SOURCES.txt
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)        1 2024-05-21 17:57:42.000000 pycrtbp-0.1.6/src/pycrtbp.egg-info/dependency_links.txt
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)       48 2024-05-21 17:57:42.000000 pycrtbp-0.1.6/src/pycrtbp.egg-info/entry_points.txt
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)       13 2024-05-21 17:57:42.000000 pycrtbp-0.1.6/src/pycrtbp.egg-info/requires.txt
+-rw-r--r--   0 jzuluaga  (1000) jzuluaga  (1000)        8 2024-05-21 17:57:42.000000 pycrtbp-0.1.6/src/pycrtbp.egg-info/top_level.txt
```

### Comparing `pycrtbp-0.1.5/LICENSE` & `pycrtbp-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrtbp-0.1.5/PKG-INFO` & `pycrtbp-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrtbp
-Version: 0.1.5
+Version: 0.1.6
 Summary: CRTBP Integrator and Tools
 Home-page: https://pypi.org/project/pycrtbp
 Author: Diego A. Acosta & Jorge I. Zuluaga
 Author-email: diego.acostab@udea.edu.co
 License: MIT
 Keywords: astrodynamics
 Classifier: Programming Language :: Python :: 3
@@ -138,14 +138,26 @@
     yaxis=dict(title='Y',range=[-rang,rang]),
     zaxis=dict(title='Z',range=[-rang,rang]),
 ))
 
 fig.show()
 ```
 
+## Periodic orbit database
+
+The package can interact with the periodic orbit database by Acosta, Zuluaga and Restrepo. To do it you must install independently mysql:
+
+```
+pip3 install mysql-connector-python
+```
+
+and install the database following the instructions we will publish. 
+
+The present version of the package does not have yet this functionality but we include it in this README to let you know of a coming feature.
+
 ## What's new
 
 For a detailed list of the newest features introduced in the latest
 releases pleas check [What's
 new](https://github.com/seap-udea/crtbpCorrectorIntegrator/blob/main/WHATSNEW.md).
 
 ------------
```

### Comparing `pycrtbp-0.1.5/README.md` & `pycrtbp-0.1.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -121,14 +121,26 @@
     yaxis=dict(title='Y',range=[-rang,rang]),
     zaxis=dict(title='Z',range=[-rang,rang]),
 ))
 
 fig.show()
 ```
 
+## Periodic orbit database
+
+The package can interact with the periodic orbit database by Acosta, Zuluaga and Restrepo. To do it you must install independently mysql:
+
+```
+pip3 install mysql-connector-python
+```
+
+and install the database following the instructions we will publish. 
+
+The present version of the package does not have yet this functionality but we include it in this README to let you know of a coming feature.
+
 ## What's new
 
 For a detailed list of the newest features introduced in the latest
 releases pleas check [What's
 new](https://github.com/seap-udea/crtbpCorrectorIntegrator/blob/main/WHATSNEW.md).
 
 ------------
```

### Comparing `pycrtbp-0.1.5/setup.py` & `pycrtbp-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         ],
-    version='0.1.5',
+    version='0.1.6',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `pycrtbp-0.1.5/src/pycrtbp/__init__.py` & `pycrtbp-0.1.6/src/pycrtbp/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,12 +15,13 @@
     ROOTDIR=os.path.abspath('')
 
 #############################################################
 # PACKAGES MODULES
 #############################################################
 from pycrtbp.particles import *
 from pycrtbp.system import *
+from pycrtbp.periodicorbits import *
 
 #############################################################
 # EXECUTE
 #############################################################
 print(f"Running pycrtbp {version} from {ROOTDIR}")
```

### Comparing `pycrtbp-0.1.5/src/pycrtbp/particles.py` & `pycrtbp-0.1.6/src/pycrtbp/particles.py`

 * *Files identical despite different names*

### Comparing `pycrtbp-0.1.5/src/pycrtbp/system.py` & `pycrtbp-0.1.6/src/pycrtbp/system.py`

 * *Files identical despite different names*

### Comparing `pycrtbp-0.1.5/src/pycrtbp.egg-info/PKG-INFO` & `pycrtbp-0.1.6/src/pycrtbp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrtbp
-Version: 0.1.5
+Version: 0.1.6
 Summary: CRTBP Integrator and Tools
 Home-page: https://pypi.org/project/pycrtbp
 Author: Diego A. Acosta & Jorge I. Zuluaga
 Author-email: diego.acostab@udea.edu.co
 License: MIT
 Keywords: astrodynamics
 Classifier: Programming Language :: Python :: 3
@@ -138,14 +138,26 @@
     yaxis=dict(title='Y',range=[-rang,rang]),
     zaxis=dict(title='Z',range=[-rang,rang]),
 ))
 
 fig.show()
 ```
 
+## Periodic orbit database
+
+The package can interact with the periodic orbit database by Acosta, Zuluaga and Restrepo. To do it you must install independently mysql:
+
+```
+pip3 install mysql-connector-python
+```
+
+and install the database following the instructions we will publish. 
+
+The present version of the package does not have yet this functionality but we include it in this README to let you know of a coming feature.
+
 ## What's new
 
 For a detailed list of the newest features introduced in the latest
 releases pleas check [What's
 new](https://github.com/seap-udea/crtbpCorrectorIntegrator/blob/main/WHATSNEW.md).
 
 ------------
```

