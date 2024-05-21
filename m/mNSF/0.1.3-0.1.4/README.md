# Comparing `tmp/mNSF-0.1.3.tar.gz` & `tmp/mNSF-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mNSF-0.1.3.tar", last modified: Sun May 12 17:33:42 2024, max compression
+gzip compressed data, was "mNSF-0.1.4.tar", last modified: Tue May 21 15:53:11 2024, max compression
```

## Comparing `mNSF-0.1.3.tar` & `mNSF-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-s---   0 ywang    (41982) hansen_lab1  (4128)        0 2024-05-12 17:33:42.517919 mNSF-0.1.3/
--rw-r--r--   0 ywang    (41982) hansen_lab1  (4128)      949 2024-05-12 17:33:42.474918 mNSF-0.1.3/PKG-INFO
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)     1204 2024-04-30 13:10:22.000000 mNSF-0.1.3/README.txt
-drwxr-s---   0 ywang    (41982) hansen_lab1  (4128)        0 2024-05-12 17:33:41.570895 mNSF-0.1.3/mNSF/
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)       58 2024-04-30 13:10:24.000000 mNSF-0.1.3/mNSF/__init__.py
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)    21513 2024-04-30 13:10:24.000000 mNSF-0.1.3/mNSF/pf_multiSample.py
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)     6762 2024-04-30 13:10:25.000000 mNSF-0.1.3/mNSF/process_multiSample.py
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)    19708 2024-04-30 13:10:25.000000 mNSF-0.1.3/mNSF/training_multiSample.py
-drwxr-s---   0 ywang    (41982) hansen_lab1  (4128)        0 2024-05-12 17:33:42.307914 mNSF-0.1.3/mNSF.egg-info/
--rw-r--r--   0 ywang    (41982) hansen_lab1  (4128)      949 2024-05-12 17:33:40.000000 mNSF-0.1.3/mNSF.egg-info/PKG-INFO
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)      279 2024-05-12 17:33:40.000000 mNSF-0.1.3/mNSF.egg-info/SOURCES.txt
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)        1 2024-05-12 17:33:40.000000 mNSF-0.1.3/mNSF.egg-info/dependency_links.txt
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)      116 2024-05-12 17:33:40.000000 mNSF-0.1.3/mNSF.egg-info/requires.txt
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)        5 2024-05-12 17:33:40.000000 mNSF-0.1.3/mNSF.egg-info/top_level.txt
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)       38 2024-05-12 17:33:42.529919 mNSF-0.1.3/setup.cfg
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)     1227 2024-05-12 17:32:43.000000 mNSF-0.1.3/setup.py
-drwxr-s---   0 ywang    (41982) hansen_lab1  (4128)        0 2024-05-12 17:33:42.382916 mNSF-0.1.3/tests/
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)     2830 2024-04-30 13:10:26.000000 mNSF-0.1.3/tests/test_small_run.py
+drwxr-s---   0 ywang    (41982) hansen_lab1  (4128)        0 2024-05-21 15:53:11.502507 mNSF-0.1.4/
+-rw-r--r--   0 ywang    (41982) hansen_lab1  (4128)      935 2024-05-21 15:53:11.452506 mNSF-0.1.4/PKG-INFO
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)     1204 2024-05-21 15:32:40.000000 mNSF-0.1.4/README.txt
+drwxr-s---   0 ywang    (41982) hansen_lab1  (4128)        0 2024-05-21 15:53:10.391478 mNSF-0.1.4/mNSF/
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)       58 2024-05-21 15:32:44.000000 mNSF-0.1.4/mNSF/__init__.py
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)    21513 2024-05-21 15:32:44.000000 mNSF-0.1.4/mNSF/pf_multiSample.py
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)     6762 2024-05-21 15:32:44.000000 mNSF-0.1.4/mNSF/process_multiSample.py
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)    19708 2024-05-21 15:32:44.000000 mNSF-0.1.4/mNSF/training_multiSample.py
+drwxr-s---   0 ywang    (41982) hansen_lab1  (4128)        0 2024-05-21 15:53:10.853490 mNSF-0.1.4/mNSF.egg-info/
+-rw-r--r--   0 ywang    (41982) hansen_lab1  (4128)      935 2024-05-21 15:53:09.000000 mNSF-0.1.4/mNSF.egg-info/PKG-INFO
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)      279 2024-05-21 15:53:09.000000 mNSF-0.1.4/mNSF.egg-info/SOURCES.txt
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)        1 2024-05-21 15:53:09.000000 mNSF-0.1.4/mNSF.egg-info/dependency_links.txt
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)      110 2024-05-21 15:53:09.000000 mNSF-0.1.4/mNSF.egg-info/requires.txt
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)        5 2024-05-21 15:53:09.000000 mNSF-0.1.4/mNSF.egg-info/top_level.txt
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)       38 2024-05-21 15:53:11.513507 mNSF-0.1.4/setup.cfg
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)     1213 2024-05-21 15:53:05.000000 mNSF-0.1.4/setup.py
+drwxr-s---   0 ywang    (41982) hansen_lab1  (4128)        0 2024-05-21 15:53:10.979493 mNSF-0.1.4/tests/
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)     2830 2024-05-21 15:32:46.000000 mNSF-0.1.4/tests/test_small_run.py
```

### Comparing `mNSF-0.1.3/PKG-INFO` & `mNSF-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mNSF
-Version: 0.1.3
+Version: 0.1.4
 Summary: multi-sample non-negative spatial factorization
 Home-page: https://github.com/hansenlab/mNSF/
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Yi Wang, Kyla Woyshner, Chaichontat Sriworarat, Loyal Goff, Genevieve Stein-O'Brien, Kasper D. Hansen
 Author-email: yiwangthu4@gmail.com
 License: MIT
 Keywords: spatial,factorization,multi-sample
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: python==3.10
+Classifier: Programming Language :: Python
+Requires-Dist: python
 Requires-Dist: anndata
 Requires-Dist: click
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pip
 Requires-Dist: scanpy
```

### Comparing `mNSF-0.1.3/README.txt` & `mNSF-0.1.4/README.txt`

 * *Files identical despite different names*

### Comparing `mNSF-0.1.3/mNSF/pf_multiSample.py` & `mNSF-0.1.4/mNSF/pf_multiSample.py`

 * *Files identical despite different names*

### Comparing `mNSF-0.1.3/mNSF/process_multiSample.py` & `mNSF-0.1.4/mNSF/process_multiSample.py`

 * *Files identical despite different names*

### Comparing `mNSF-0.1.3/mNSF/training_multiSample.py` & `mNSF-0.1.4/mNSF/training_multiSample.py`

 * *Files identical despite different names*

### Comparing `mNSF-0.1.3/mNSF.egg-info/PKG-INFO` & `mNSF-0.1.4/mNSF.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mNSF
-Version: 0.1.3
+Version: 0.1.4
 Summary: multi-sample non-negative spatial factorization
 Home-page: https://github.com/hansenlab/mNSF/
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Yi Wang, Kyla Woyshner, Chaichontat Sriworarat, Loyal Goff, Genevieve Stein-O'Brien, Kasper D. Hansen
 Author-email: yiwangthu4@gmail.com
 License: MIT
 Keywords: spatial,factorization,multi-sample
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: python==3.10
+Classifier: Programming Language :: Python
+Requires-Dist: python
 Requires-Dist: anndata
 Requires-Dist: click
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pip
 Requires-Dist: scanpy
```

### Comparing `mNSF-0.1.3/setup.py` & `mNSF-0.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from distutils.core import setup
 setup(
   name = 'mNSF',       
   packages = ['mNSF'],   
-  version = '0.1.3',     
+  version = '0.1.4',     
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'multi-sample non-negative spatial factorization',   #
   author = "Yi Wang, Kyla Woyshner, Chaichontat Sriworarat, Loyal Goff, Genevieve Stein-O'Brien, Kasper D. Hansen",                   
   author_email = 'yiwangthu4@gmail.com',      
   url = 'https://github.com/hansenlab/mNSF/',   
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    
   keywords = ['spatial', 'factorization', 'multi-sample'],   
   install_requires=[
-          'python==3.10','anndata', 'click', 'matplotlib', 'numpy', 'pandas', 'pip', 
+          'python','anndata', 'click', 'matplotlib', 'numpy', 'pandas', 'pip', 
           'scanpy', 'squidpy', 'tensorflow==2.13', 'tensorflow-probability==0.21'],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
 
     'Intended Audience :: Developers',     
     'Topic :: Software Development :: Build Tools',
 
     'License :: OSI Approved :: MIT License',   
-    'Programming Language :: Python :: 3.10',      
+    'Programming Language :: Python',      
 
   ],
 )
```

### Comparing `mNSF-0.1.3/tests/test_small_run.py` & `mNSF-0.1.4/tests/test_small_run.py`

 * *Files identical despite different names*

