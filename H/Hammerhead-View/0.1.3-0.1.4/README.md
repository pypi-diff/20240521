# Comparing `tmp/Hammerhead-View-0.1.3.tar.gz` & `tmp/Hammerhead-View-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hammerhead-View-0.1.3.tar", last modified: Fri Jan  5 07:16:19 2024, max compression
+gzip compressed data, was "Hammerhead-View-0.1.4.tar", last modified: Tue May 21 05:52:21 2024, max compression
```

## Comparing `Hammerhead-View-0.1.3.tar` & `Hammerhead-View-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-01-05 07:16:19.036192 Hammerhead-View-0.1.3/
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-01-05 07:16:19.036192 Hammerhead-View-0.1.3/Hammerhead/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4824 2024-01-05 07:15:53.000000 Hammerhead-View-0.1.3/Hammerhead/hammerhead
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-01-05 07:16:19.036192 Hammerhead-View-0.1.3/Hammerhead_View.egg-info/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3619 2024-01-05 07:16:18.000000 Hammerhead-View-0.1.3/Hammerhead_View.egg-info/PKG-INFO
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      246 2024-01-05 07:16:19.000000 Hammerhead-View-0.1.3/Hammerhead_View.egg-info/SOURCES.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2024-01-05 07:16:18.000000 Hammerhead-View-0.1.3/Hammerhead_View.egg-info/dependency_links.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       17 2024-01-05 07:16:18.000000 Hammerhead-View-0.1.3/Hammerhead_View.egg-info/requires.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2024-01-05 07:16:18.000000 Hammerhead-View-0.1.3/Hammerhead_View.egg-info/top_level.txt
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)    35149 2024-01-05 06:36:43.000000 Hammerhead-View-0.1.3/LICENSE.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3619 2024-01-05 07:16:19.036192 Hammerhead-View-0.1.3/PKG-INFO
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     3142 2024-01-05 07:06:00.000000 Hammerhead-View-0.1.3/README.md
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2024-01-05 07:16:19.036192 Hammerhead-View-0.1.3/setup.cfg
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      760 2024-01-05 06:35:54.000000 Hammerhead-View-0.1.3/setup.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-05-21 05:52:21.489079 Hammerhead-View-0.1.4/
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-05-21 05:52:21.489079 Hammerhead-View-0.1.4/Hammerhead_View/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4928 2024-05-21 05:51:23.000000 Hammerhead-View-0.1.4/Hammerhead_View/hammer_polish
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     6195 2024-05-21 05:51:23.000000 Hammerhead-View-0.1.4/Hammerhead_View/hammerhead
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-05-21 05:52:21.489079 Hammerhead-View-0.1.4/Hammerhead_View.egg-info/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5730 2024-05-21 05:52:21.000000 Hammerhead-View-0.1.4/Hammerhead_View.egg-info/PKG-INFO
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      277 2024-05-21 05:52:21.000000 Hammerhead-View-0.1.4/Hammerhead_View.egg-info/SOURCES.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2024-05-21 05:52:21.000000 Hammerhead-View-0.1.4/Hammerhead_View.egg-info/dependency_links.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       31 2024-05-21 05:52:21.000000 Hammerhead-View-0.1.4/Hammerhead_View.egg-info/requires.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2024-05-21 05:52:21.000000 Hammerhead-View-0.1.4/Hammerhead_View.egg-info/top_level.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)    18092 2024-05-21 05:51:23.000000 Hammerhead-View-0.1.4/LICENSE
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5730 2024-05-21 05:52:21.489079 Hammerhead-View-0.1.4/PKG-INFO
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5257 2024-05-21 05:51:23.000000 Hammerhead-View-0.1.4/README.md
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2024-05-21 05:52:21.489079 Hammerhead-View-0.1.4/setup.cfg
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      827 2024-05-21 05:51:23.000000 Hammerhead-View-0.1.4/setup.py
```

### Comparing `Hammerhead-View-0.1.3/setup.py` & `Hammerhead-View-0.1.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="Hammerhead-View",
-  version="0.1.3",
+  version="0.1.4",
   author="Xudong Liu",
   author_email="xudongliu98@gmail.com",
   description="A tool designed to de novo find potential modification sites.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/lrslab/Hammerhead",
   packages=setuptools.find_packages(),
   classifiers=[
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   ],
   python_requires = '>=3.7, <=3.11',
   install_requires=[
-  'termcolor >= 2.2.0'
+  'termcolor >= 2.2.0',
+  'pandas >= 2.0.3'
   ],
-  scripts = ["Hammerhead/hammerhead"]
+  scripts = ["Hammerhead_View/hammerhead",
+      "Hammerhead_View/hammer_polish"]
 )
```

