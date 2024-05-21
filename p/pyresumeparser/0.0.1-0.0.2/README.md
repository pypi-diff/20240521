# Comparing `tmp/pyresumeparser-0.0.1.tar.gz` & `tmp/pyresumeparser-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyresumeparser-0.0.1.tar", last modified: Tue May 21 07:58:42 2024, max compression
+gzip compressed data, was "pyresumeparser-0.0.2.tar", last modified: Tue May 21 08:22:36 2024, max compression
```

## Comparing `pyresumeparser-0.0.1.tar` & `pyresumeparser-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-21 07:58:42.178245 pyresumeparser-0.0.1/
--rw-r--r--   0 pluto      (501) staff       (20)     2721 2024-05-21 07:58:42.176968 pyresumeparser-0.0.1/PKG-INFO
--rw-r--r--   0 pluto      (501) staff       (20)     2170 2024-05-21 07:40:05.000000 pyresumeparser-0.0.1/README.md
-drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-21 07:58:42.175690 pyresumeparser-0.0.1/pyresumeparser.egg-info/
--rw-r--r--   0 pluto      (501) staff       (20)     2721 2024-05-21 07:58:42.000000 pyresumeparser-0.0.1/pyresumeparser.egg-info/PKG-INFO
--rw-r--r--   0 pluto      (501) staff       (20)      402 2024-05-21 07:58:42.000000 pyresumeparser-0.0.1/pyresumeparser.egg-info/SOURCES.txt
--rw-r--r--   0 pluto      (501) staff       (20)        1 2024-05-21 07:58:42.000000 pyresumeparser-0.0.1/pyresumeparser.egg-info/dependency_links.txt
--rw-r--r--   0 pluto      (501) staff       (20)       57 2024-05-21 07:58:42.000000 pyresumeparser-0.0.1/pyresumeparser.egg-info/entry_points.txt
--rw-r--r--   0 pluto      (501) staff       (20)       62 2024-05-21 07:58:42.000000 pyresumeparser-0.0.1/pyresumeparser.egg-info/requires.txt
--rw-r--r--   0 pluto      (501) staff       (20)       14 2024-05-21 07:58:42.000000 pyresumeparser-0.0.1/pyresumeparser.egg-info/top_level.txt
-drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-21 07:58:42.171585 pyresumeparser-0.0.1/resume_parser/
--rw-r--r--   0 pluto      (501) staff       (20)       44 2024-05-21 07:40:09.000000 pyresumeparser-0.0.1/resume_parser/__init__.py
--rw-r--r--   0 pluto      (501) staff       (20)     2866 2024-05-21 07:40:00.000000 pyresumeparser-0.0.1/resume_parser/main.py
-drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-21 07:58:42.174270 pyresumeparser-0.0.1/resume_parser/model-best/
--rw-r--r--   0 pluto      (501) staff       (20)     2885 2024-05-15 13:00:41.000000 pyresumeparser-0.0.1/resume_parser/model-best/config.cfg
--rw-r--r--   0 pluto      (501) staff       (20)     2499 2024-05-15 13:00:41.000000 pyresumeparser-0.0.1/resume_parser/model-best/meta.json
--rw-r--r--   0 pluto      (501) staff       (20)    77066 2024-05-15 13:00:40.000000 pyresumeparser-0.0.1/resume_parser/model-best/tokenizer
--rw-r--r--   0 pluto      (501) staff       (20)       38 2024-05-21 07:58:42.178461 pyresumeparser-0.0.1/setup.cfg
--rw-r--r--   0 pluto      (501) staff       (20)     1044 2024-05-21 07:54:15.000000 pyresumeparser-0.0.1/setup.py
+drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-21 08:22:36.454246 pyresumeparser-0.0.2/
+-rw-r--r--   0 pluto      (501) staff       (20)       35 2024-05-21 08:12:01.000000 pyresumeparser-0.0.2/MANIFEST.in
+-rw-r--r--   0 pluto      (501) staff       (20)     2721 2024-05-21 08:22:36.452976 pyresumeparser-0.0.2/PKG-INFO
+-rw-r--r--   0 pluto      (501) staff       (20)     2170 2024-05-21 08:22:18.000000 pyresumeparser-0.0.2/README.md
+drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-21 08:22:36.451402 pyresumeparser-0.0.2/pyresumeparser.egg-info/
+-rw-r--r--   0 pluto      (501) staff       (20)     2721 2024-05-21 08:22:36.000000 pyresumeparser-0.0.2/pyresumeparser.egg-info/PKG-INFO
+-rw-r--r--   0 pluto      (501) staff       (20)      414 2024-05-21 08:22:36.000000 pyresumeparser-0.0.2/pyresumeparser.egg-info/SOURCES.txt
+-rw-r--r--   0 pluto      (501) staff       (20)        1 2024-05-21 08:22:36.000000 pyresumeparser-0.0.2/pyresumeparser.egg-info/dependency_links.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       59 2024-05-21 08:22:36.000000 pyresumeparser-0.0.2/pyresumeparser.egg-info/entry_points.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       62 2024-05-21 08:22:36.000000 pyresumeparser-0.0.2/pyresumeparser.egg-info/requires.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       14 2024-05-21 08:22:36.000000 pyresumeparser-0.0.2/pyresumeparser.egg-info/top_level.txt
+drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-21 08:22:36.446506 pyresumeparser-0.0.2/resume_parser/
+-rw-r--r--   0 pluto      (501) staff       (20)       44 2024-05-21 07:40:09.000000 pyresumeparser-0.0.2/resume_parser/__init__.py
+-rw-r--r--   0 pluto      (501) staff       (20)     2866 2024-05-21 07:40:00.000000 pyresumeparser-0.0.2/resume_parser/main.py
+drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-21 08:22:36.449624 pyresumeparser-0.0.2/resume_parser/model-best/
+-rw-r--r--   0 pluto      (501) staff       (20)     2885 2024-05-15 13:00:41.000000 pyresumeparser-0.0.2/resume_parser/model-best/config.cfg
+-rw-r--r--   0 pluto      (501) staff       (20)     2499 2024-05-15 13:00:41.000000 pyresumeparser-0.0.2/resume_parser/model-best/meta.json
+-rw-r--r--   0 pluto      (501) staff       (20)    77066 2024-05-15 13:00:40.000000 pyresumeparser-0.0.2/resume_parser/model-best/tokenizer
+-rw-r--r--   0 pluto      (501) staff       (20)       38 2024-05-21 08:22:36.454465 pyresumeparser-0.0.2/setup.cfg
+-rw-r--r--   0 pluto      (501) staff       (20)     1046 2024-05-21 08:13:08.000000 pyresumeparser-0.0.2/setup.py
```

### Comparing `pyresumeparser-0.0.1/PKG-INFO` & `pyresumeparser-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyresumeparser
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for parsing resume and extracting entities.
 Home-page: https://github.com/pkhan123/resume_parser
 Author: Palash Khan
 Author-email: palashkhan777@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyresumeparser-0.0.1/README.md` & `pyresumeparser-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyresumeparser-0.0.1/pyresumeparser.egg-info/PKG-INFO` & `pyresumeparser-0.0.2/pyresumeparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyresumeparser
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for parsing resume and extracting entities.
 Home-page: https://github.com/pkhan123/resume_parser
 Author: Palash Khan
 Author-email: palashkhan777@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyresumeparser-0.0.1/resume_parser/main.py` & `pyresumeparser-0.0.2/resume_parser/main.py`

 * *Files identical despite different names*

### Comparing `pyresumeparser-0.0.1/resume_parser/model-best/config.cfg` & `pyresumeparser-0.0.2/resume_parser/model-best/config.cfg`

 * *Files identical despite different names*

### Comparing `pyresumeparser-0.0.1/resume_parser/model-best/meta.json` & `pyresumeparser-0.0.2/resume_parser/model-best/meta.json`

 * *Files identical despite different names*

### Comparing `pyresumeparser-0.0.1/resume_parser/model-best/tokenizer` & `pyresumeparser-0.0.2/resume_parser/model-best/tokenizer`

 * *Files identical despite different names*

### Comparing `pyresumeparser-0.0.1/setup.py` & `pyresumeparser-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='pyresumeparser',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'pdfminer.six==20231228',
         'spacy==3.7.4',
         'spacy-transformers==1.3.5'
     ],
     package_data={
         'resume_parser': ['model-best/*']
     },
     entry_points={
         'console_scripts': [
-            'resumeparser=resume_parser.main:main',
+            'pyresumeparser=resume_parser.main:main',
         ],
     },
     author='Palash Khan',
     author_email='palashkhan777@gmail.com',
     description='A package for parsing resume and extracting entities.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

