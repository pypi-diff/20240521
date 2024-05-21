# Comparing `tmp/chemical_safety-0.0.2.tar.gz` & `tmp/chemical_safety-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemical_safety-0.0.2.tar", last modified: Tue May 21 16:02:34 2024, max compression
+gzip compressed data, was "chemical_safety-0.0.3.tar", last modified: Tue May 21 16:17:41 2024, max compression
```

## Comparing `chemical_safety-0.0.2.tar` & `chemical_safety-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 16:02:34.000000 chemical_safety-0.0.2/
--rw-rw-rw-   0        0        0     1095 2024-02-03 21:17:28.000000 chemical_safety-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      217 2024-05-21 16:02:34.000000 chemical_safety-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      419 2024-05-21 16:01:33.000000 chemical_safety-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 16:02:34.000000 chemical_safety-0.0.2/chemical_safety/
--rw-rw-rw-   0        0        0       66 2024-05-18 17:22:12.000000 chemical_safety-0.0.2/chemical_safety/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:02:34.000000 chemical_safety-0.0.2/chemical_safety/chemical/
--rw-rw-rw-   0        0        0       30 2024-05-18 16:55:19.000000 chemical_safety-0.0.2/chemical_safety/chemical/__init__.py
--rw-rw-rw-   0        0        0    38858 2024-05-21 15:58:58.000000 chemical_safety-0.0.2/chemical_safety/chemical/chemical.py
--rw-rw-rw-   0        0        0    11694 2024-05-03 04:13:48.000000 chemical_safety-0.0.2/chemical_safety/chemical/molecule.py
--rw-rw-rw-   0        0        0     5474 2024-03-11 02:03:14.000000 chemical_safety-0.0.2/chemical_safety/chemical/periodictable.py
--rw-rw-rw-   0        0        0    14908 2024-05-03 04:14:07.000000 chemical_safety-0.0.2/chemical_safety/chemical/sigfig.py
--rw-rw-rw-   0        0        0     8223 2024-02-12 03:32:32.000000 chemical_safety-0.0.2/chemical_safety/chemical/units.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:02:34.000000 chemical_safety-0.0.2/chemical_safety/dashboard/
--rw-rw-rw-   0        0        0       26 2024-05-18 17:22:03.000000 chemical_safety-0.0.2/chemical_safety/dashboard/__init__.py
--rw-rw-rw-   0        0        0    11776 2024-05-20 22:51:02.000000 chemical_safety-0.0.2/chemical_safety/dashboard/app.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:02:34.000000 chemical_safety-0.0.2/chemical_safety.egg-info/
--rw-rw-rw-   0        0        0      217 2024-05-21 16:02:33.000000 chemical_safety-0.0.2/chemical_safety.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      583 2024-05-21 16:02:34.000000 chemical_safety-0.0.2/chemical_safety.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 16:02:33.000000 chemical_safety-0.0.2/chemical_safety.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-05-21 16:02:33.000000 chemical_safety-0.0.2/chemical_safety.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2024-05-21 16:02:33.000000 chemical_safety-0.0.2/chemical_safety.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-21 16:02:33.000000 chemical_safety-0.0.2/chemical_safety.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 16:02:34.000000 chemical_safety-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      693 2024-05-21 15:58:51.000000 chemical_safety-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:17:41.000000 chemical_safety-0.0.3/
+-rw-rw-rw-   0        0        0     1095 2024-02-03 21:17:28.000000 chemical_safety-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      679 2024-05-21 16:17:41.000000 chemical_safety-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2024-05-21 16:01:33.000000 chemical_safety-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 16:17:41.000000 chemical_safety-0.0.3/chemical_safety/
+-rw-rw-rw-   0        0        0       66 2024-05-18 17:22:12.000000 chemical_safety-0.0.3/chemical_safety/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:17:41.000000 chemical_safety-0.0.3/chemical_safety/chemical/
+-rw-rw-rw-   0        0        0       30 2024-05-18 16:55:19.000000 chemical_safety-0.0.3/chemical_safety/chemical/__init__.py
+-rw-rw-rw-   0        0        0    38858 2024-05-21 15:58:58.000000 chemical_safety-0.0.3/chemical_safety/chemical/chemical.py
+-rw-rw-rw-   0        0        0    11694 2024-05-03 04:13:48.000000 chemical_safety-0.0.3/chemical_safety/chemical/molecule.py
+-rw-rw-rw-   0        0        0     5474 2024-03-11 02:03:14.000000 chemical_safety-0.0.3/chemical_safety/chemical/periodictable.py
+-rw-rw-rw-   0        0        0    14908 2024-05-03 04:14:07.000000 chemical_safety-0.0.3/chemical_safety/chemical/sigfig.py
+-rw-rw-rw-   0        0        0     8223 2024-02-12 03:32:32.000000 chemical_safety-0.0.3/chemical_safety/chemical/units.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:17:41.000000 chemical_safety-0.0.3/chemical_safety/dashboard/
+-rw-rw-rw-   0        0        0       26 2024-05-18 17:22:03.000000 chemical_safety-0.0.3/chemical_safety/dashboard/__init__.py
+-rw-rw-rw-   0        0        0    11776 2024-05-20 22:51:02.000000 chemical_safety-0.0.3/chemical_safety/dashboard/app.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:17:41.000000 chemical_safety-0.0.3/chemical_safety.egg-info/
+-rw-rw-rw-   0        0        0      679 2024-05-21 16:17:40.000000 chemical_safety-0.0.3/chemical_safety.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2024-05-21 16:17:41.000000 chemical_safety-0.0.3/chemical_safety.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 16:17:40.000000 chemical_safety-0.0.3/chemical_safety.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-21 16:17:40.000000 chemical_safety-0.0.3/chemical_safety.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       67 2024-05-21 16:17:40.000000 chemical_safety-0.0.3/chemical_safety.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-21 16:17:40.000000 chemical_safety-0.0.3/chemical_safety.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 16:17:41.000000 chemical_safety-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      825 2024-05-21 16:17:19.000000 chemical_safety-0.0.3/setup.py
```

### Comparing `chemical_safety-0.0.2/LICENSE` & `chemical_safety-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.2/chemical_safety/chemical/chemical.py` & `chemical_safety-0.0.3/chemical_safety/chemical/chemical.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.2/chemical_safety/chemical/molecule.py` & `chemical_safety-0.0.3/chemical_safety/chemical/molecule.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.2/chemical_safety/chemical/periodictable.py` & `chemical_safety-0.0.3/chemical_safety/chemical/periodictable.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.2/chemical_safety/chemical/sigfig.py` & `chemical_safety-0.0.3/chemical_safety/chemical/sigfig.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.2/chemical_safety/chemical/units.py` & `chemical_safety-0.0.3/chemical_safety/chemical/units.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.2/chemical_safety/dashboard/app.py` & `chemical_safety-0.0.3/chemical_safety/dashboard/app.py`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.2/chemical_safety.egg-info/SOURCES.txt` & `chemical_safety-0.0.3/chemical_safety.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chemical_safety-0.0.2/setup.py` & `chemical_safety-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chemical_safety",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(include=['chemical_safety', 'chemical_safety.*']),
     description="A package for retreiving chemical safety information",
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     author="Demetrios Pagonis",
     author_email="demetriospagonis@weber.edu",
+    include_package_data=True,
     install_requires=[
         'pandas',
         'numpy',
         'jinja2',
         'requests',
         'Levenshtein',
         'natsort',
```

