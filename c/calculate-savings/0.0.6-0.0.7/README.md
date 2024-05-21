# Comparing `tmp/calculate_savings-0.0.6.tar.gz` & `tmp/calculate_savings-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculate_savings-0.0.6.tar", last modified: Tue May 21 10:01:33 2024, max compression
+gzip compressed data, was "calculate_savings-0.0.7.tar", last modified: Tue May 21 11:27:16 2024, max compression
```

## Comparing `calculate_savings-0.0.6.tar` & `calculate_savings-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 10:01:33.620582 calculate_savings-0.0.6/
--rw-r--r--   0 takenakayuuki   (501) staff       (20)      561 2024-05-21 10:01:33.620418 calculate_savings-0.0.6/PKG-INFO
--rw-r--r--   0 takenakayuuki   (501) staff       (20)        0 2024-05-20 10:47:16.000000 calculate_savings-0.0.6/README.md
--rw-r--r--   0 takenakayuuki   (501) staff       (20)       38 2024-05-21 10:01:33.620613 calculate_savings-0.0.6/setup.cfg
--rw-r--r--   0 takenakayuuki   (501) staff       (20)     1094 2024-05-21 10:01:09.000000 calculate_savings-0.0.6/setup.py
-drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 10:01:33.619547 calculate_savings-0.0.6/src/
-drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 10:01:33.620256 calculate_savings-0.0.6/src/calculate_savings.egg-info/
--rw-r--r--   0 takenakayuuki   (501) staff       (20)      561 2024-05-21 10:01:33.000000 calculate_savings-0.0.6/src/calculate_savings.egg-info/PKG-INFO
--rw-r--r--   0 takenakayuuki   (501) staff       (20)      271 2024-05-21 10:01:33.000000 calculate_savings-0.0.6/src/calculate_savings.egg-info/SOURCES.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)        1 2024-05-21 10:01:33.000000 calculate_savings-0.0.6/src/calculate_savings.egg-info/dependency_links.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)       61 2024-05-21 10:01:33.000000 calculate_savings-0.0.6/src/calculate_savings.egg-info/entry_points.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)       18 2024-05-21 10:01:33.000000 calculate_savings-0.0.6/src/calculate_savings.egg-info/top_level.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)     3156 2024-05-21 09:38:01.000000 calculate_savings-0.0.6/src/calculate_savings.py
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 11:27:16.747826 calculate_savings-0.0.7/
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       20 2024-05-21 11:26:12.000000 calculate_savings-0.0.7/MANIFEST.in
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)      561 2024-05-21 11:27:16.747627 calculate_savings-0.0.7/PKG-INFO
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)        0 2024-05-20 10:47:16.000000 calculate_savings-0.0.7/README.md
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 11:27:16.734068 calculate_savings-0.0.7/data/
+-rw-r--r--   0 takenakayuuki   (501) staff       (20) 19188118 2024-05-21 05:28:42.000000 calculate_savings-0.0.7/data/hon-maikin-k-jissu.csv
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       38 2024-05-21 11:27:16.747866 calculate_savings-0.0.7/setup.cfg
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)     1038 2024-05-21 11:26:50.000000 calculate_savings-0.0.7/setup.py
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 11:27:16.746668 calculate_savings-0.0.7/src/
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 11:27:16.747422 calculate_savings-0.0.7/src/calculate_savings.egg-info/
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)      561 2024-05-21 11:27:16.000000 calculate_savings-0.0.7/src/calculate_savings.egg-info/PKG-INFO
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)      311 2024-05-21 11:27:16.000000 calculate_savings-0.0.7/src/calculate_savings.egg-info/SOURCES.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)        1 2024-05-21 11:27:16.000000 calculate_savings-0.0.7/src/calculate_savings.egg-info/dependency_links.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       61 2024-05-21 11:27:16.000000 calculate_savings-0.0.7/src/calculate_savings.egg-info/entry_points.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       18 2024-05-21 11:27:16.000000 calculate_savings-0.0.7/src/calculate_savings.egg-info/top_level.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)     3156 2024-05-21 09:38:01.000000 calculate_savings-0.0.7/src/calculate_savings.py
```

### Comparing `calculate_savings-0.0.6/PKG-INFO` & `calculate_savings-0.0.7/src/calculate_savings.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: calculate_savings
-Version: 0.0.6
+Name: calculate-savings
+Version: 0.0.7
 Summary: How much can you save in 10 years by predicting your salary?
 Home-page: https://github.com/takenakayuuki0901/calculate_savings.git
 Author: YukiTakenaka
 Author-email: s2222024@stu.musashino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/takenakayuuki0901/calculate_savings.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calculate_savings-0.0.6/setup.py` & `calculate_savings-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="calculate_savings",
-    version="0.0.6",
+    version="0.0.7",
     author="YukiTakenaka",
     author_email="s2222024@stu.musashino-u.ac.jp",
     description="How much can you save in 10 years by predicting your salary?",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/takenakayuuki0901/calculate_savings.git",
     project_urls={
@@ -19,11 +19,10 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     py_modules=["calculate_savings"],
     packages=setuptools.find_packages(where="sre"),
     include_package_data=True,
-    package_data={"calculate_savings": ["data/*.csv"]},
     python_requires=">=3.8",
     entry_points={"console_scripts": ["calculate_savings = calculate_savings:main"]},
 )
```

### Comparing `calculate_savings-0.0.6/src/calculate_savings.egg-info/PKG-INFO` & `calculate_savings-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: calculate-savings
-Version: 0.0.6
+Name: calculate_savings
+Version: 0.0.7
 Summary: How much can you save in 10 years by predicting your salary?
 Home-page: https://github.com/takenakayuuki0901/calculate_savings.git
 Author: YukiTakenaka
 Author-email: s2222024@stu.musashino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/takenakayuuki0901/calculate_savings.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calculate_savings-0.0.6/src/calculate_savings.py` & `calculate_savings-0.0.7/src/calculate_savings.py`

 * *Files identical despite different names*

