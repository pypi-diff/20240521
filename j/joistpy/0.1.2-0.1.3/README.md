# Comparing `tmp/joistpy-0.1.2.tar.gz` & `tmp/joistpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joistpy-0.1.2.tar", last modified: Tue May 21 17:18:36 2024, max compression
+gzip compressed data, was "joistpy-0.1.3.tar", last modified: Tue May 21 17:25:35 2024, max compression
```

## Comparing `joistpy-0.1.2.tar` & `joistpy-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 17:18:36.903575 joistpy-0.1.2/
--rw-rw-rw-   0        0        0    35149 2024-05-21 15:08:39.000000 joistpy-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      475 2024-05-21 17:18:36.899709 joistpy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1403 2024-05-21 16:23:40.000000 joistpy-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 17:18:36.871843 joistpy-0.1.2/joistpy/
--rw-rw-rw-   0        0        0       24 2024-05-21 04:34:52.000000 joistpy-0.1.2/joistpy/__init__.py
--rw-rw-rw-   0        0        0     4971 2024-05-21 16:09:45.000000 joistpy-0.1.2/joistpy/joistpy.py
-drwxrwxrwx   0        0        0        0 2024-05-21 17:18:36.898699 joistpy-0.1.2/joistpy.egg-info/
--rw-rw-rw-   0        0        0      475 2024-05-21 17:18:36.000000 joistpy-0.1.2/joistpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2024-05-21 17:18:36.000000 joistpy-0.1.2/joistpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 17:18:36.000000 joistpy-0.1.2/joistpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-21 17:18:36.000000 joistpy-0.1.2/joistpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 17:18:36.904348 joistpy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      739 2024-05-21 17:18:30.000000 joistpy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 17:25:35.315808 joistpy-0.1.3/
+-rw-rw-rw-   0        0        0    35149 2024-05-21 15:08:39.000000 joistpy-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      475 2024-05-21 17:25:35.314704 joistpy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1403 2024-05-21 16:23:40.000000 joistpy-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 17:25:35.210819 joistpy-0.1.3/joistpy/
+-rw-rw-rw-   0        0        0       24 2024-05-21 04:34:52.000000 joistpy-0.1.3/joistpy/__init__.py
+-rw-rw-rw-   0        0        0     4971 2024-05-21 16:09:45.000000 joistpy-0.1.3/joistpy/joistpy.py
+drwxrwxrwx   0        0        0        0 2024-05-21 17:25:35.310394 joistpy-0.1.3/joistpy/property files/
+-rw-rw-rw-   0        0        0    24559 2024-05-21 14:09:30.000000 joistpy-0.1.3/joistpy/property files/K_L_360.csv
+-rw-rw-rw-   0        0        0    24416 2024-05-21 14:09:48.000000 joistpy-0.1.3/joistpy/property files/K_Total.csv
+-rw-rw-rw-   0        0        0      602 2024-05-21 14:10:04.000000 joistpy-0.1.3/joistpy/property files/K_weight.csv
+drwxrwxrwx   0        0        0        0 2024-05-21 17:25:35.312891 joistpy-0.1.3/joistpy.egg-info/
+-rw-rw-rw-   0        0        0      475 2024-05-21 17:25:35.000000 joistpy-0.1.3/joistpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2024-05-21 17:25:35.000000 joistpy-0.1.3/joistpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 17:25:35.000000 joistpy-0.1.3/joistpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-21 17:25:35.000000 joistpy-0.1.3/joistpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 17:25:35.315808 joistpy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      802 2024-05-21 17:25:14.000000 joistpy-0.1.3/setup.py
```

### Comparing `joistpy-0.1.2/LICENSE` & `joistpy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `joistpy-0.1.2/README.md` & `joistpy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `joistpy-0.1.2/joistpy/joistpy.py` & `joistpy-0.1.3/joistpy/joistpy.py`

 * *Files identical despite different names*

### Comparing `joistpy-0.1.2/setup.py` & `joistpy-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from setuptools import setup, find_packages
 
 name = 'joistpy'
-version = '0.1.2'
+version = '0.1.3'
 author = 'Matthew Upshaw'
 author_email = 'matthew.upshaw02@gmail.com'
 description = 'Library that acts as a database for SJI steel open web bar joist shapes for easy use in structural calculations.'
 packages = find_packages()
+package_data = {
+    'joistpy': ['property files/*.csv'],
+}
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
     'Operating System :: OS Independent',
 ]
 python_requires = '>=3.8'
 
-setup(name=name, version=version, author=author, author_email=author_email, description=description, packages=packages, classifiers=classifiers, python_requires=python_requires, include_package_data=True)
+setup(name=name, version=version, author=author, author_email=author_email, description=description, packages=packages, package_data=package_data, classifiers=classifiers, python_requires=python_requires)
```

