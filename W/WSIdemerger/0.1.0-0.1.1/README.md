# Comparing `tmp/wsidemerger-0.1.0.tar.gz` & `tmp/wsidemerger-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsidemerger-0.1.0.tar", last modified: Tue May 21 11:14:38 2024, max compression
+gzip compressed data, was "wsidemerger-0.1.1.tar", last modified: Tue May 21 11:22:34 2024, max compression
```

## Comparing `wsidemerger-0.1.0.tar` & `wsidemerger-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 11:14:38.683174 wsidemerger-0.1.0/
--rw-rw-rw-   0        0        0     1086 2024-05-21 10:23:57.000000 wsidemerger-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3463 2024-05-21 11:14:38.681180 wsidemerger-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2731 2024-05-21 11:12:57.000000 wsidemerger-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 11:14:38.637585 wsidemerger-0.1.0/WSIdemerger/
--rw-rw-rw-   0        0        0     1137 2024-05-21 11:11:18.000000 wsidemerger-0.1.0/WSIdemerger/Colour_standardisation.py
--rw-rw-rw-   0        0        0     2892 2024-05-21 11:11:24.000000 wsidemerger-0.1.0/WSIdemerger/Patches_generation.py
--rw-rw-rw-   0        0        0      936 2024-05-21 11:10:13.000000 wsidemerger-0.1.0/WSIdemerger/__init__.py
--rw-rw-rw-   0        0        0     1690 2024-05-21 11:12:01.000000 wsidemerger-0.1.0/WSIdemerger/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 11:14:38.679186 wsidemerger-0.1.0/WSIdemerger.egg-info/
--rw-rw-rw-   0        0        0     3463 2024-05-21 11:14:38.000000 wsidemerger-0.1.0/WSIdemerger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-05-21 11:14:38.000000 wsidemerger-0.1.0/WSIdemerger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 11:14:38.000000 wsidemerger-0.1.0/WSIdemerger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-21 11:14:38.000000 wsidemerger-0.1.0/WSIdemerger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-21 11:14:38.000000 wsidemerger-0.1.0/WSIdemerger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 11:14:38.683174 wsidemerger-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      936 2024-05-21 11:13:24.000000 wsidemerger-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:22:34.395035 wsidemerger-0.1.1/
+-rw-rw-rw-   0        0        0     1086 2024-05-21 10:23:57.000000 wsidemerger-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       19 2024-05-21 11:21:04.000000 wsidemerger-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3463 2024-05-21 11:22:34.394034 wsidemerger-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2731 2024-05-21 11:12:57.000000 wsidemerger-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 11:22:34.344179 wsidemerger-0.1.1/WSIdemerger/
+-rw-rw-rw-   0        0        0     1137 2024-05-21 11:11:18.000000 wsidemerger-0.1.1/WSIdemerger/Colour_standardisation.py
+-rw-rw-rw-   0        0        0     2892 2024-05-21 11:11:24.000000 wsidemerger-0.1.1/WSIdemerger/Patches_generation.py
+-rw-rw-rw-   0        0        0      936 2024-05-21 11:10:13.000000 wsidemerger-0.1.1/WSIdemerger/__init__.py
+-rw-rw-rw-   0        0        0     1690 2024-05-21 11:12:01.000000 wsidemerger-0.1.1/WSIdemerger/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:22:34.392395 wsidemerger-0.1.1/WSIdemerger.egg-info/
+-rw-rw-rw-   0        0        0     3463 2024-05-21 11:22:34.000000 wsidemerger-0.1.1/WSIdemerger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-21 11:22:34.000000 wsidemerger-0.1.1/WSIdemerger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 11:22:34.000000 wsidemerger-0.1.1/WSIdemerger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-21 11:22:34.000000 wsidemerger-0.1.1/WSIdemerger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 11:22:34.000000 wsidemerger-0.1.1/WSIdemerger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 11:22:34.395035 wsidemerger-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      955 2024-05-21 11:20:40.000000 wsidemerger-0.1.1/setup.py
```

### Comparing `wsidemerger-0.1.0/LICENSE` & `wsidemerger-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wsidemerger-0.1.0/PKG-INFO` & `wsidemerger-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WSIdemerger
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for extracting image patches from SVS files and performing color normalization
 Home-page: https://github.com/yourusername/WSI_Preprocessing
 Author: Thirteen
 Author-email: 506607814@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wsidemerger-0.1.0/README.md` & `wsidemerger-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wsidemerger-0.1.0/WSIdemerger/Colour_standardisation.py` & `wsidemerger-0.1.1/WSIdemerger/Colour_standardisation.py`

 * *Files identical despite different names*

### Comparing `wsidemerger-0.1.0/WSIdemerger/Patches_generation.py` & `wsidemerger-0.1.1/WSIdemerger/Patches_generation.py`

 * *Files identical despite different names*

### Comparing `wsidemerger-0.1.0/WSIdemerger/__init__.py` & `wsidemerger-0.1.1/WSIdemerger/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidemerger-0.1.0/WSIdemerger/utils.py` & `wsidemerger-0.1.1/WSIdemerger/utils.py`

 * *Files identical despite different names*

### Comparing `wsidemerger-0.1.0/WSIdemerger.egg-info/PKG-INFO` & `wsidemerger-0.1.1/WSIdemerger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WSIdemerger
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for extracting image patches from SVS files and performing color normalization
 Home-page: https://github.com/yourusername/WSI_Preprocessing
 Author: Thirteen
 Author-email: 506607814@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wsidemerger-0.1.0/setup.py` & `wsidemerger-0.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='WSIdemerger',
-    version='0.1.0',
+    version='0.1.1',  # 更新版本号
     packages=find_packages(),
     install_requires=[
         'pandas',
         'openslide-python',
         'Pillow',
         'numpy',
         'scikit-image',
```

