# Comparing `tmp/glpic-99.0.202405182305.tar.gz` & `tmp/glpic-99.0.202405210607.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202405182305.tar", last modified: Sat May 18 23:05:09 2024, max compression
+gzip compressed data, was "glpic-99.0.202405210607.tar", last modified: Tue May 21 06:08:00 2024, max compression
```

## Comparing `glpic-99.0.202405182305.tar` & `glpic-99.0.202405210607.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:05:09.587549 glpic-99.0.202405182305/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-18 23:05:09.587549 glpic-99.0.202405182305/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-18 23:04:57.000000 glpic-99.0.202405182305/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:05:09.587549 glpic-99.0.202405182305/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-05-18 23:04:57.000000 glpic-99.0.202405182305/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-05-18 23:04:57.000000 glpic-99.0.202405182305/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:05:09.587549 glpic-99.0.202405182305/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-18 23:05:09.000000 glpic-99.0.202405182305/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-18 23:05:09.000000 glpic-99.0.202405182305/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 23:05:09.000000 glpic-99.0.202405182305/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-18 23:05:09.000000 glpic-99.0.202405182305/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 23:05:09.000000 glpic-99.0.202405182305/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-18 23:05:09.000000 glpic-99.0.202405182305/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-18 23:05:09.000000 glpic-99.0.202405182305/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 23:05:09.587549 glpic-99.0.202405182305/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-18 23:05:08.000000 glpic-99.0.202405182305/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:08:00.190183 glpic-99.0.202405210607/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-21 06:08:00.190183 glpic-99.0.202405210607/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-21 06:07:07.000000 glpic-99.0.202405210607/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:08:00.190183 glpic-99.0.202405210607/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-05-21 06:07:07.000000 glpic-99.0.202405210607/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-05-21 06:07:07.000000 glpic-99.0.202405210607/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:08:00.190183 glpic-99.0.202405210607/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-21 06:08:00.000000 glpic-99.0.202405210607/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-21 06:08:00.000000 glpic-99.0.202405210607/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 06:08:00.000000 glpic-99.0.202405210607/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-21 06:08:00.000000 glpic-99.0.202405210607/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 06:08:00.000000 glpic-99.0.202405210607/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-21 06:08:00.000000 glpic-99.0.202405210607/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 06:08:00.000000 glpic-99.0.202405210607/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 06:08:00.190183 glpic-99.0.202405210607/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-21 06:07:59.000000 glpic-99.0.202405210607/setup.py
```

### Comparing `glpic-99.0.202405182305/README.md` & `glpic-99.0.202405210607/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405182305/glpic/__init__.py` & `glpic-99.0.202405210607/glpic/__init__.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405182305/glpic/cli.py` & `glpic-99.0.202405210607/glpic/cli.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405182305/setup.py` & `glpic-99.0.202405210607/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202405182305',
+    version='99.0.202405210607',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```
