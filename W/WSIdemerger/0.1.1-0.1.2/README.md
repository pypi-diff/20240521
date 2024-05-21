# Comparing `tmp/wsidemerger-0.1.1.tar.gz` & `tmp/wsidemerger-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsidemerger-0.1.1.tar", last modified: Tue May 21 11:22:34 2024, max compression
+gzip compressed data, was "wsidemerger-0.1.2.tar", last modified: Tue May 21 11:53:32 2024, max compression
```

## Comparing `wsidemerger-0.1.1.tar` & `wsidemerger-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 11:22:34.395035 wsidemerger-0.1.1/
--rw-rw-rw-   0        0        0     1086 2024-05-21 10:23:57.000000 wsidemerger-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       19 2024-05-21 11:21:04.000000 wsidemerger-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3463 2024-05-21 11:22:34.394034 wsidemerger-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2731 2024-05-21 11:12:57.000000 wsidemerger-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 11:22:34.344179 wsidemerger-0.1.1/WSIdemerger/
--rw-rw-rw-   0        0        0     1137 2024-05-21 11:11:18.000000 wsidemerger-0.1.1/WSIdemerger/Colour_standardisation.py
--rw-rw-rw-   0        0        0     2892 2024-05-21 11:11:24.000000 wsidemerger-0.1.1/WSIdemerger/Patches_generation.py
--rw-rw-rw-   0        0        0      936 2024-05-21 11:10:13.000000 wsidemerger-0.1.1/WSIdemerger/__init__.py
--rw-rw-rw-   0        0        0     1690 2024-05-21 11:12:01.000000 wsidemerger-0.1.1/WSIdemerger/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 11:22:34.392395 wsidemerger-0.1.1/WSIdemerger.egg-info/
--rw-rw-rw-   0        0        0     3463 2024-05-21 11:22:34.000000 wsidemerger-0.1.1/WSIdemerger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-21 11:22:34.000000 wsidemerger-0.1.1/WSIdemerger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 11:22:34.000000 wsidemerger-0.1.1/WSIdemerger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-21 11:22:34.000000 wsidemerger-0.1.1/WSIdemerger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-21 11:22:34.000000 wsidemerger-0.1.1/WSIdemerger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 11:22:34.395035 wsidemerger-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      955 2024-05-21 11:20:40.000000 wsidemerger-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:53:32.214850 wsidemerger-0.1.2/
+-rw-rw-rw-   0        0        0     1086 2024-05-21 10:23:57.000000 wsidemerger-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       19 2024-05-21 11:21:04.000000 wsidemerger-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3463 2024-05-21 11:53:32.213853 wsidemerger-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2731 2024-05-21 11:40:02.000000 wsidemerger-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 11:53:32.202646 wsidemerger-0.1.2/WSIdemerger/
+-rw-rw-rw-   0        0        0     1137 2024-05-21 11:11:18.000000 wsidemerger-0.1.2/WSIdemerger/Colour_standardisation.py
+-rw-rw-rw-   0        0        0     2892 2024-05-21 11:11:24.000000 wsidemerger-0.1.2/WSIdemerger/Patches_generation.py
+-rw-rw-rw-   0        0        0      936 2024-05-21 11:10:13.000000 wsidemerger-0.1.2/WSIdemerger/__init__.py
+-rw-rw-rw-   0        0        0     1690 2024-05-21 11:12:01.000000 wsidemerger-0.1.2/WSIdemerger/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:53:32.212856 wsidemerger-0.1.2/WSIdemerger.egg-info/
+-rw-rw-rw-   0        0        0     3463 2024-05-21 11:53:31.000000 wsidemerger-0.1.2/WSIdemerger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-21 11:53:32.000000 wsidemerger-0.1.2/WSIdemerger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 11:53:31.000000 wsidemerger-0.1.2/WSIdemerger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-21 11:53:31.000000 wsidemerger-0.1.2/WSIdemerger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 11:53:31.000000 wsidemerger-0.1.2/WSIdemerger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 11:53:32.214850 wsidemerger-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1123 2024-05-21 11:49:28.000000 wsidemerger-0.1.2/setup.py
```

### Comparing `wsidemerger-0.1.1/LICENSE` & `wsidemerger-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wsidemerger-0.1.1/PKG-INFO` & `wsidemerger-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WSIdemerger
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for extracting image patches from SVS files and performing color normalization
 Home-page: https://github.com/yourusername/WSI_Preprocessing
 Author: Thirteen
 Author-email: 506607814@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wsidemerger-0.1.1/README.md` & `wsidemerger-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `wsidemerger-0.1.1/WSIdemerger/Colour_standardisation.py` & `wsidemerger-0.1.2/WSIdemerger/Colour_standardisation.py`

 * *Files identical despite different names*

### Comparing `wsidemerger-0.1.1/WSIdemerger/Patches_generation.py` & `wsidemerger-0.1.2/WSIdemerger/Patches_generation.py`

 * *Files identical despite different names*

### Comparing `wsidemerger-0.1.1/WSIdemerger/__init__.py` & `wsidemerger-0.1.2/WSIdemerger/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidemerger-0.1.1/WSIdemerger/utils.py` & `wsidemerger-0.1.2/WSIdemerger/utils.py`

 * *Files identical despite different names*

### Comparing `wsidemerger-0.1.1/WSIdemerger.egg-info/PKG-INFO` & `wsidemerger-0.1.2/WSIdemerger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WSIdemerger
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for extracting image patches from SVS files and performing color normalization
 Home-page: https://github.com/yourusername/WSI_Preprocessing
 Author: Thirteen
 Author-email: 506607814@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wsidemerger-0.1.1/setup.py` & `wsidemerger-0.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from setuptools import setup, find_packages
+import os
+
+def read(file_name):
+    try:
+        return open(os.path.join(os.path.dirname(__file__), file_name)).read()
+    except FileNotFoundError:
+        return ""
 
 setup(
     name='WSIdemerger',
-    version='0.1.1',  # 更新版本号
+    version='0.1.2',  # 更新版本号
     packages=find_packages(),
     install_requires=[
         'pandas',
         'openslide-python',
         'Pillow',
         'numpy',
         'scikit-image',
         'tqdm',
         'opencv-python',
         'staintools'
     ],
     author='Thirteen',
     author_email='506607814@qq.com',
     description='A package for extracting image patches from SVS files and performing color normalization',
-    long_description=open('README.md').read(),
+    long_description=read('README.md'),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/WSI_Preprocessing',  # 替换为你的GitHub仓库地址
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

