# Comparing `tmp/cleaner_panda-0.1.0.tar.gz` & `tmp/cleaner_panda-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleaner_panda-0.1.0.tar", last modified: Tue May 21 14:48:04 2024, max compression
+gzip compressed data, was "cleaner_panda-0.1.1.tar", last modified: Tue May 21 16:17:05 2024, max compression
```

## Comparing `cleaner_panda-0.1.0.tar` & `cleaner_panda-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 14:48:04.284973 cleaner_panda-0.1.0/
--rw-rw-rw-   0        0        0    35803 2024-05-20 15:24:41.000000 cleaner_panda-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      584 2024-05-21 14:48:04.285968 cleaner_panda-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2310 2024-05-21 13:52:39.000000 cleaner_panda-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 14:48:04.142591 cleaner_panda-0.1.0/cleaner_panda/
--rw-rw-rw-   0        0        0      581 2024-05-21 10:40:47.000000 cleaner_panda-0.1.0/cleaner_panda/__init__.py
--rw-rw-rw-   0        0        0     1263 2024-05-21 12:25:42.000000 cleaner_panda-0.1.0/cleaner_panda/categorical_encoder.py
--rw-rw-rw-   0        0        0      652 2024-05-21 10:46:50.000000 cleaner_panda-0.1.0/cleaner_panda/data_type_converter.py
--rw-rw-rw-   0        0        0     3440 2024-05-21 13:52:39.000000 cleaner_panda-0.1.0/cleaner_panda/date_time_handler.py
--rw-rw-rw-   0        0        0     3623 2024-05-21 14:33:42.000000 cleaner_panda-0.1.0/cleaner_panda/missing_value_handler.py
--rw-rw-rw-   0        0        0     2671 2024-05-20 15:42:21.000000 cleaner_panda-0.1.0/cleaner_panda/outlier_handler.py
--rw-rw-rw-   0        0        0     1681 2024-05-21 10:47:33.000000 cleaner_panda-0.1.0/cleaner_panda/scaler.py
--rw-rw-rw-   0        0        0     3224 2024-05-21 10:47:33.000000 cleaner_panda-0.1.0/cleaner_panda/text_cleaner.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:48:04.184782 cleaner_panda-0.1.0/cleaner_panda.egg-info/
--rw-rw-rw-   0        0        0      584 2024-05-21 14:48:04.000000 cleaner_panda-0.1.0/cleaner_panda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2024-05-21 14:48:04.000000 cleaner_panda-0.1.0/cleaner_panda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:48:04.000000 cleaner_panda-0.1.0/cleaner_panda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-05-21 14:48:04.000000 cleaner_panda-0.1.0/cleaner_panda.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-21 14:48:04.000000 cleaner_panda-0.1.0/cleaner_panda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-21 14:48:04.288982 cleaner_panda-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      840 2024-05-21 14:45:38.000000 cleaner_panda-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:48:04.282439 cleaner_panda-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2024-05-20 15:24:41.000000 cleaner_panda-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1894 2024-05-21 14:31:59.000000 cleaner_panda-0.1.0/tests/test_categorical_encoder.py
--rw-rw-rw-   0        0        0     1343 2024-05-21 14:29:20.000000 cleaner_panda-0.1.0/tests/test_data_type_converter.py
--rw-rw-rw-   0        0        0     3973 2024-05-21 14:31:58.000000 cleaner_panda-0.1.0/tests/test_date_time_handler.py
--rw-rw-rw-   0        0        0     3853 2024-05-21 14:34:15.000000 cleaner_panda-0.1.0/tests/test_missing_value_handler.py
--rw-rw-rw-   0        0        0     2743 2024-05-21 14:33:33.000000 cleaner_panda-0.1.0/tests/test_outlier_handler.py
--rw-rw-rw-   0        0        0     3701 2024-05-21 14:33:31.000000 cleaner_panda-0.1.0/tests/test_scaler.py
--rw-rw-rw-   0        0        0     4451 2024-05-21 14:33:30.000000 cleaner_panda-0.1.0/tests/test_text_cleaner.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:17:05.122497 cleaner_panda-0.1.1/
+-rw-rw-rw-   0        0        0    35803 2024-05-20 15:24:41.000000 cleaner_panda-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      584 2024-05-21 16:17:05.123476 cleaner_panda-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2310 2024-05-21 13:52:39.000000 cleaner_panda-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 16:17:05.067636 cleaner_panda-0.1.1/cleaner_panda/
+-rw-rw-rw-   0        0        0      581 2024-05-21 10:40:47.000000 cleaner_panda-0.1.1/cleaner_panda/__init__.py
+-rw-rw-rw-   0        0        0     1263 2024-05-21 12:25:42.000000 cleaner_panda-0.1.1/cleaner_panda/categorical_encoder.py
+-rw-rw-rw-   0        0        0      652 2024-05-21 10:46:50.000000 cleaner_panda-0.1.1/cleaner_panda/data_type_converter.py
+-rw-rw-rw-   0        0        0     3440 2024-05-21 13:52:39.000000 cleaner_panda-0.1.1/cleaner_panda/date_time_handler.py
+-rw-rw-rw-   0        0        0     3623 2024-05-21 14:33:42.000000 cleaner_panda-0.1.1/cleaner_panda/missing_value_handler.py
+-rw-rw-rw-   0        0        0     2671 2024-05-20 15:42:21.000000 cleaner_panda-0.1.1/cleaner_panda/outlier_handler.py
+-rw-rw-rw-   0        0        0     1681 2024-05-21 10:47:33.000000 cleaner_panda-0.1.1/cleaner_panda/scaler.py
+-rw-rw-rw-   0        0        0     3224 2024-05-21 10:47:33.000000 cleaner_panda-0.1.1/cleaner_panda/text_cleaner.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:17:05.099717 cleaner_panda-0.1.1/cleaner_panda.egg-info/
+-rw-rw-rw-   0        0        0      584 2024-05-21 16:17:04.000000 cleaner_panda-0.1.1/cleaner_panda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2024-05-21 16:17:04.000000 cleaner_panda-0.1.1/cleaner_panda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 16:17:04.000000 cleaner_panda-0.1.1/cleaner_panda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2024-05-21 16:17:04.000000 cleaner_panda-0.1.1/cleaner_panda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-21 16:17:04.000000 cleaner_panda-0.1.1/cleaner_panda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-21 16:17:05.127667 cleaner_panda-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      886 2024-05-21 16:13:04.000000 cleaner_panda-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:17:05.117478 cleaner_panda-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-20 15:24:41.000000 cleaner_panda-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     1894 2024-05-21 14:31:59.000000 cleaner_panda-0.1.1/tests/test_categorical_encoder.py
+-rw-rw-rw-   0        0        0     1343 2024-05-21 14:29:20.000000 cleaner_panda-0.1.1/tests/test_data_type_converter.py
+-rw-rw-rw-   0        0        0     3973 2024-05-21 14:31:58.000000 cleaner_panda-0.1.1/tests/test_date_time_handler.py
+-rw-rw-rw-   0        0        0     3853 2024-05-21 14:34:15.000000 cleaner_panda-0.1.1/tests/test_missing_value_handler.py
+-rw-rw-rw-   0        0        0     2743 2024-05-21 14:33:33.000000 cleaner_panda-0.1.1/tests/test_outlier_handler.py
+-rw-rw-rw-   0        0        0     3701 2024-05-21 14:33:31.000000 cleaner_panda-0.1.1/tests/test_scaler.py
+-rw-rw-rw-   0        0        0     4451 2024-05-21 14:33:30.000000 cleaner_panda-0.1.1/tests/test_text_cleaner.py
```

### Comparing `cleaner_panda-0.1.0/LICENSE` & `cleaner_panda-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.0/PKG-INFO` & `cleaner_panda-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cleaner_panda
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for handling various data preprocessing tasks
 Home-page: https://github.com/EmirhanSyl/cleaner-panda
 Author: asimtarik & emirs
 Author-email: support@cleanpanda.com
 License: UNKNOWN
-Download-URL: https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.0.tar.gz
+Download-URL: https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.1.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `cleaner_panda-0.1.0/README.md` & `cleaner_panda-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.0/cleaner_panda/__init__.py` & `cleaner_panda-0.1.1/cleaner_panda/__init__.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.0/cleaner_panda/categorical_encoder.py` & `cleaner_panda-0.1.1/cleaner_panda/categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.0/cleaner_panda/data_type_converter.py` & `cleaner_panda-0.1.1/cleaner_panda/data_type_converter.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.0/cleaner_panda/date_time_handler.py` & `cleaner_panda-0.1.1/cleaner_panda/date_time_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.0/cleaner_panda/missing_value_handler.py` & `cleaner_panda-0.1.1/cleaner_panda/missing_value_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.0/cleaner_panda/outlier_handler.py` & `cleaner_panda-0.1.1/cleaner_panda/outlier_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.0/cleaner_panda/scaler.py` & `cleaner_panda-0.1.1/cleaner_panda/scaler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.0/cleaner_panda/text_cleaner.py` & `cleaner_panda-0.1.1/cleaner_panda/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.0/cleaner_panda.egg-info/PKG-INFO` & `cleaner_panda-0.1.1/cleaner_panda.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cleaner-panda
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for handling various data preprocessing tasks
 Home-page: https://github.com/EmirhanSyl/cleaner-panda
 Author: asimtarik & emirs
 Author-email: support@cleanpanda.com
 License: UNKNOWN
-Download-URL: https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.0.tar.gz
+Download-URL: https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.1.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `cleaner_panda-0.1.0/cleaner_panda.egg-info/SOURCES.txt` & `cleaner_panda-0.1.1/cleaner_panda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.0/setup.py` & `cleaner_panda-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cleaner_panda',
-    version='0.1.0',
+    version='0.1.1',
     description='A package for handling various data preprocessing tasks',
     author='asimtarik & emirs',
     author_email='support@cleanpanda.com',
     url='https://github.com/EmirhanSyl/cleaner-panda',
-    download_url='https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.0.tar.gz',
+    download_url='https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.1.tar.gz',
     packages=find_packages(),
     install_requires=[
+        'unittest',
         'pandas',
         'numpy',
         'scikit-learn',
-        'nltk'
-        'category_encoders'
-        'scipy'
-        'bs4'
-        'contractions'
+        'nltk',
+        'category_encoders',
+        'scipy',
+        'bs4',
+        'contractions',
+        'datetime'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.8',
```

### Comparing `cleaner_panda-0.1.0/tests/test_categorical_encoder.py` & `cleaner_panda-0.1.1/tests/test_categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.0/tests/test_data_type_converter.py` & `cleaner_panda-0.1.1/tests/test_data_type_converter.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.0/tests/test_date_time_handler.py` & `cleaner_panda-0.1.1/tests/test_date_time_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.0/tests/test_missing_value_handler.py` & `cleaner_panda-0.1.1/tests/test_missing_value_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.0/tests/test_outlier_handler.py` & `cleaner_panda-0.1.1/tests/test_outlier_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.0/tests/test_scaler.py` & `cleaner_panda-0.1.1/tests/test_scaler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.0/tests/test_text_cleaner.py` & `cleaner_panda-0.1.1/tests/test_text_cleaner.py`

 * *Files identical despite different names*

