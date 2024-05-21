# Comparing `tmp/calculate_savings-0.0.2.tar.gz` & `tmp/calculate_savings-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculate_savings-0.0.2.tar", last modified: Tue May 21 09:16:04 2024, max compression
+gzip compressed data, was "calculate_savings-0.0.3.tar", last modified: Tue May 21 09:39:18 2024, max compression
```

## Comparing `calculate_savings-0.0.2.tar` & `calculate_savings-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 09:16:04.302427 calculate_savings-0.0.2/
--rw-r--r--   0 takenakayuuki   (501) staff       (20)      564 2024-05-21 09:16:04.302250 calculate_savings-0.0.2/PKG-INFO
--rw-r--r--   0 takenakayuuki   (501) staff       (20)        0 2024-05-20 10:47:16.000000 calculate_savings-0.0.2/README.md
--rw-r--r--   0 takenakayuuki   (501) staff       (20)       38 2024-05-21 09:16:04.302462 calculate_savings-0.0.2/setup.cfg
--rw-r--r--   0 takenakayuuki   (501) staff       (20)     1030 2024-05-21 09:12:12.000000 calculate_savings-0.0.2/setup.py
-drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 09:16:04.301109 calculate_savings-0.0.2/src/
-drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 09:16:04.302065 calculate_savings-0.0.2/src/calculate_savings.egg-info/
--rw-r--r--   0 takenakayuuki   (501) staff       (20)      564 2024-05-21 09:16:04.000000 calculate_savings-0.0.2/src/calculate_savings.egg-info/PKG-INFO
--rw-r--r--   0 takenakayuuki   (501) staff       (20)      271 2024-05-21 09:16:04.000000 calculate_savings-0.0.2/src/calculate_savings.egg-info/SOURCES.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)        1 2024-05-21 09:16:04.000000 calculate_savings-0.0.2/src/calculate_savings.egg-info/dependency_links.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)       67 2024-05-21 09:16:04.000000 calculate_savings-0.0.2/src/calculate_savings.egg-info/entry_points.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)       18 2024-05-21 09:16:04.000000 calculate_savings-0.0.2/src/calculate_savings.egg-info/top_level.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)     3043 2024-05-21 08:20:23.000000 calculate_savings-0.0.2/src/calculate_savings.py
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 09:39:18.891732 calculate_savings-0.0.3/
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)      564 2024-05-21 09:39:18.891563 calculate_savings-0.0.3/PKG-INFO
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)        0 2024-05-20 10:47:16.000000 calculate_savings-0.0.3/README.md
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       38 2024-05-21 09:39:18.891764 calculate_savings-0.0.3/setup.cfg
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)     1117 2024-05-21 09:38:59.000000 calculate_savings-0.0.3/setup.py
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 09:39:18.890667 calculate_savings-0.0.3/src/
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-21 09:39:18.891399 calculate_savings-0.0.3/src/calculate_savings.egg-info/
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)      564 2024-05-21 09:39:18.000000 calculate_savings-0.0.3/src/calculate_savings.egg-info/PKG-INFO
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)      271 2024-05-21 09:39:18.000000 calculate_savings-0.0.3/src/calculate_savings.egg-info/SOURCES.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)        1 2024-05-21 09:39:18.000000 calculate_savings-0.0.3/src/calculate_savings.egg-info/dependency_links.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       67 2024-05-21 09:39:18.000000 calculate_savings-0.0.3/src/calculate_savings.egg-info/entry_points.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       18 2024-05-21 09:39:18.000000 calculate_savings-0.0.3/src/calculate_savings.egg-info/top_level.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)     3156 2024-05-21 09:38:01.000000 calculate_savings-0.0.3/src/calculate_savings.py
```

### Comparing `calculate_savings-0.0.2/PKG-INFO` & `calculate_savings-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calculate_savings
-Version: 0.0.2
+Version: 0.0.3
 Summary: How much can you save in 10 years by predicting your salary?
 Home-page: https://github.com/takenakayuuki0901/calculate_savings.git
 Author: YukiTakenaka
 Author-email: s2222024@stu.musashino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/takenakayuuki0901/calculate_savings.git
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calculate_savings-0.0.2/setup.py` & `calculate_savings-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="calculate_savings",
-    version="0.0.2",
+    version="0.0.3",
     author="YukiTakenaka",
     author_email="s2222024@stu.musashino-u.ac.jp",
     description="How much can you save in 10 years by predicting your salary?",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/takenakayuuki0901/calculate_savings.git",
     project_urls={
@@ -18,12 +18,14 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     py_modules=["calculate_savings"],
     packages=setuptools.find_packages(where="sre"),
+    include_package_data=True,
+    package_data={"calculate_savings": ["data/*.csv"]},
     python_requires=">=3.7",
     entry_points={
         "console _scripts": ["calculate_savings = calculate_savings.main:main"]
     },
 )
```

### Comparing `calculate_savings-0.0.2/src/calculate_savings.egg-info/PKG-INFO` & `calculate_savings-0.0.3/src/calculate_savings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calculate-savings
-Version: 0.0.2
+Version: 0.0.3
 Summary: How much can you save in 10 years by predicting your salary?
 Home-page: https://github.com/takenakayuuki0901/calculate_savings.git
 Author: YukiTakenaka
 Author-email: s2222024@stu.musashino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/takenakayuuki0901/calculate_savings.git
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calculate_savings-0.0.2/src/calculate_savings.py` & `calculate_savings-0.0.3/src/calculate_savings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from datetime import datetime
 from sklearn.linear_model import LinearRegression
+from pkg_resources import resource_filename
 
 
 def calculate(living_expenses, discretionary_spending):
-    df = pd.read_csv("hon-maikin-k-jissu.csv", encoding="Shift JIS")
+    csv_path = resource_filename("calculate_savings.data", "hon-maikin-k-jissu.csv")
+    df = pd.read_csv(csv_path, encoding="Shift JIS")
 
     filtered_df = df[df["産業分類"] == "TL  "]
     filtered_df = filtered_df[filtered_df["就業形態"] != 2]
     new_df = filtered_df[["年", "現金給与総額"]]
 
     # 規模別に対してその年の平均をとる
     df = new_df.groupby("年", as_index=False)["現金給与総額"].mean()
```

