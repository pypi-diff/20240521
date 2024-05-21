# Comparing `tmp/joistpy-0.1.1.tar.gz` & `tmp/joistpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joistpy-0.1.1.tar", last modified: Tue May 21 17:07:57 2024, max compression
+gzip compressed data, was "joistpy-0.1.2.tar", last modified: Tue May 21 17:18:36 2024, max compression
```

## Comparing `joistpy-0.1.1.tar` & `joistpy-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 17:07:57.648254 joistpy-0.1.1/
--rw-rw-rw-   0        0        0    35149 2024-05-21 15:08:39.000000 joistpy-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      475 2024-05-21 17:07:57.644132 joistpy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1403 2024-05-21 16:23:40.000000 joistpy-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 17:07:57.601875 joistpy-0.1.1/joistpy/
--rw-rw-rw-   0        0        0       24 2024-05-21 04:34:52.000000 joistpy-0.1.1/joistpy/__init__.py
--rw-rw-rw-   0        0        0     4971 2024-05-21 16:09:45.000000 joistpy-0.1.1/joistpy/joistpy.py
-drwxrwxrwx   0        0        0        0 2024-05-21 17:07:57.644132 joistpy-0.1.1/joistpy.egg-info/
--rw-rw-rw-   0        0        0      475 2024-05-21 17:07:56.000000 joistpy-0.1.1/joistpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2024-05-21 17:07:57.000000 joistpy-0.1.1/joistpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 17:07:57.000000 joistpy-0.1.1/joistpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-21 17:07:57.000000 joistpy-0.1.1/joistpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 17:07:57.649871 joistpy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      712 2024-05-21 17:07:49.000000 joistpy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 17:18:36.903575 joistpy-0.1.2/
+-rw-rw-rw-   0        0        0    35149 2024-05-21 15:08:39.000000 joistpy-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      475 2024-05-21 17:18:36.899709 joistpy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1403 2024-05-21 16:23:40.000000 joistpy-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 17:18:36.871843 joistpy-0.1.2/joistpy/
+-rw-rw-rw-   0        0        0       24 2024-05-21 04:34:52.000000 joistpy-0.1.2/joistpy/__init__.py
+-rw-rw-rw-   0        0        0     4971 2024-05-21 16:09:45.000000 joistpy-0.1.2/joistpy/joistpy.py
+drwxrwxrwx   0        0        0        0 2024-05-21 17:18:36.898699 joistpy-0.1.2/joistpy.egg-info/
+-rw-rw-rw-   0        0        0      475 2024-05-21 17:18:36.000000 joistpy-0.1.2/joistpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2024-05-21 17:18:36.000000 joistpy-0.1.2/joistpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 17:18:36.000000 joistpy-0.1.2/joistpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-21 17:18:36.000000 joistpy-0.1.2/joistpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 17:18:36.904348 joistpy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      739 2024-05-21 17:18:30.000000 joistpy-0.1.2/setup.py
```

### Comparing `joistpy-0.1.1/LICENSE` & `joistpy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `joistpy-0.1.1/README.md` & `joistpy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `joistpy-0.1.1/joistpy/joistpy.py` & `joistpy-0.1.2/joistpy/joistpy.py`

 * *Files identical despite different names*

### Comparing `joistpy-0.1.1/setup.py` & `joistpy-0.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 name = 'joistpy'
-version = '0.1.1'
+version = '0.1.2'
 author = 'Matthew Upshaw'
 author_email = 'matthew.upshaw02@gmail.com'
 description = 'Library that acts as a database for SJI steel open web bar joist shapes for easy use in structural calculations.'
 packages = find_packages()
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
     'Operating System :: OS Independent',
 ]
 python_requires = '>=3.8'
 
-setup(name=name, version=version, author=author, author_email=author_email, description=description, packages=packages, classifiers=classifiers, python_requires=python_requires)
+setup(name=name, version=version, author=author, author_email=author_email, description=description, packages=packages, classifiers=classifiers, python_requires=python_requires, include_package_data=True)
```

