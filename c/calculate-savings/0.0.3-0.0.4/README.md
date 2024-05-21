# Comparing `tmp/calculate_savings-0.0.3.tar.gz` & `tmp/calculate_savings-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculate_savings-0.0.3.tar", last modified: Tue May 21 09:39:18 2024, max compression
+gzip compressed data, was "calculate_savings-0.0.4.tar", last modified: Tue May 21 09:50:50 2024, max compression
```

## Comparing `calculate_savings-0.0.3.tar` & `calculate_savings-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 09:39:18.891732 calculate_savings-0.0.3/
--rw-r--r--   0 takenakayuuki   (501) staff       (20)      564 2024-05-21 09:39:18.891563 calculate_savings-0.0.3/PKG-INFO
--rw-r--r--   0 takenakayuuki   (501) staff       (20)        0 2024-05-20 10:47:16.000000 calculate_savings-0.0.3/README.md
--rw-r--r--   0 takenakayuuki   (501) staff       (20)       38 2024-05-21 09:39:18.891764 calculate_savings-0.0.3/setup.cfg
--rw-r--r--   0 takenakayuuki   (501) staff       (20)     1117 2024-05-21 09:38:59.000000 calculate_savings-0.0.3/setup.py
-drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 09:39:18.890667 calculate_savings-0.0.3/src/
-drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 09:39:18.891399 calculate_savings-0.0.3/src/calculate_savings.egg-info/
--rw-r--r--   0 takenakayuuki   (501) staff       (20)      564 2024-05-21 09:39:18.000000 calculate_savings-0.0.3/src/calculate_savings.egg-info/PKG-INFO
--rw-r--r--   0 takenakayuuki   (501) staff       (20)      271 2024-05-21 09:39:18.000000 calculate_savings-0.0.3/src/calculate_savings.egg-info/SOURCES.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)        1 2024-05-21 09:39:18.000000 calculate_savings-0.0.3/src/calculate_savings.egg-info/dependency_links.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)       67 2024-05-21 09:39:18.000000 calculate_savings-0.0.3/src/calculate_savings.egg-info/entry_points.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)       18 2024-05-21 09:39:18.000000 calculate_savings-0.0.3/src/calculate_savings.egg-info/top_level.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)     3156 2024-05-21 09:38:01.000000 calculate_savings-0.0.3/src/calculate_savings.py
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 09:50:50.012900 calculate_savings-0.0.4/
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)      561 2024-05-21 09:50:50.012736 calculate_savings-0.0.4/PKG-INFO
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)        0 2024-05-20 10:47:16.000000 calculate_savings-0.0.4/README.md
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       38 2024-05-21 09:50:50.012932 calculate_savings-0.0.4/setup.cfg
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)     1095 2024-05-21 09:48:07.000000 calculate_savings-0.0.4/setup.py
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 09:50:50.011871 calculate_savings-0.0.4/src/
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 09:50:50.012565 calculate_savings-0.0.4/src/calculate_savings.egg-info/
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)      561 2024-05-21 09:50:49.000000 calculate_savings-0.0.4/src/calculate_savings.egg-info/PKG-INFO
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)      271 2024-05-21 09:50:49.000000 calculate_savings-0.0.4/src/calculate_savings.egg-info/SOURCES.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)        1 2024-05-21 09:50:49.000000 calculate_savings-0.0.4/src/calculate_savings.egg-info/dependency_links.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       62 2024-05-21 09:50:49.000000 calculate_savings-0.0.4/src/calculate_savings.egg-info/entry_points.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       18 2024-05-21 09:50:49.000000 calculate_savings-0.0.4/src/calculate_savings.egg-info/top_level.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)     3156 2024-05-21 09:38:01.000000 calculate_savings-0.0.4/src/calculate_savings.py
```

### Comparing `calculate_savings-0.0.3/PKG-INFO` & `calculate_savings-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: calculate_savings
-Version: 0.0.3
+Version: 0.0.4
 Summary: How much can you save in 10 years by predicting your salary?
 Home-page: https://github.com/takenakayuuki0901/calculate_savings.git
 Author: YukiTakenaka
 Author-email: s2222024@stu.musashino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/takenakayuuki0901/calculate_savings.git
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `calculate_savings-0.0.3/setup.py` & `calculate_savings-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="calculate_savings",
-    version="0.0.3",
+    version="0.0.4",
     author="YukiTakenaka",
     author_email="s2222024@stu.musashino-u.ac.jp",
     description="How much can you save in 10 years by predicting your salary?",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/takenakayuuki0901/calculate_savings.git",
     project_urls={
         "Bug Tracker": "https://github.com/takenakayuuki0901/calculate_savings.git",
     },
     classifiers=[
-        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     py_modules=["calculate_savings"],
     packages=setuptools.find_packages(where="sre"),
     include_package_data=True,
     package_data={"calculate_savings": ["data/*.csv"]},
-    python_requires=">=3.7",
-    entry_points={
-        "console _scripts": ["calculate_savings = calculate_savings.main:main"]
-    },
+    python_requires=">=3.8",
+    entry_points={"console _scripts": ["calculate_savings = calculate_savings:main"]},
 )
```

### Comparing `calculate_savings-0.0.3/src/calculate_savings.egg-info/PKG-INFO` & `calculate_savings-0.0.4/src/calculate_savings.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: calculate-savings
-Version: 0.0.3
+Version: 0.0.4
 Summary: How much can you save in 10 years by predicting your salary?
 Home-page: https://github.com/takenakayuuki0901/calculate_savings.git
 Author: YukiTakenaka
 Author-email: s2222024@stu.musashino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/takenakayuuki0901/calculate_savings.git
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `calculate_savings-0.0.3/src/calculate_savings.py` & `calculate_savings-0.0.4/src/calculate_savings.py`

 * *Files identical despite different names*

