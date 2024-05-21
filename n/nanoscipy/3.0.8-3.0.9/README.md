# Comparing `tmp/nanoscipy-3.0.8.tar.gz` & `tmp/nanoscipy-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoscipy-3.0.8.tar", last modified: Sun Nov 20 11:50:06 2022, max compression
+gzip compressed data, was "nanoscipy-3.0.9.tar", last modified: Mon Nov 21 14:57:14 2022, max compression
```

## Comparing `nanoscipy-3.0.8.tar` & `nanoscipy-3.0.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:50:06.486514 nanoscipy-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    16931 2022-11-20 11:50:06.486514 nanoscipy-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16978 2022-11-20 11:49:53.000000 nanoscipy-3.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:50:06.486514 nanoscipy-3.0.8/nanoscipy/
--rw-r--r--   0 runner    (1001) docker     (121)    30552 2022-11-20 11:49:53.000000 nanoscipy-3.0.8/nanoscipy/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    28154 2022-11-20 11:49:53.000000 nanoscipy-3.0.8/nanoscipy/mathpar.py
--rw-r--r--   0 runner    (1001) docker     (121)    55447 2022-11-20 11:49:53.000000 nanoscipy-3.0.8/nanoscipy/modules.py
--rw-r--r--   0 runner    (1001) docker     (121)    42325 2022-11-20 11:49:53.000000 nanoscipy-3.0.8/nanoscipy/unitpar.py
--rw-r--r--   0 runner    (1001) docker     (121)    20936 2022-11-20 11:49:53.000000 nanoscipy-3.0.8/nanoscipy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:50:06.486514 nanoscipy-3.0.8/nanoscipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16931 2022-11-20 11:50:06.000000 nanoscipy-3.0.8/nanoscipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-20 11:50:06.000000 nanoscipy-3.0.8/nanoscipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-20 11:50:06.000000 nanoscipy-3.0.8/nanoscipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-20 11:50:06.000000 nanoscipy-3.0.8/nanoscipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-20 11:50:06.000000 nanoscipy-3.0.8/nanoscipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-20 11:50:06.486514 nanoscipy-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-11-20 11:49:53.000000 nanoscipy-3.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 14:57:14.643729 nanoscipy-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-21 14:57:02.000000 nanoscipy-3.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)    17049 2022-11-21 14:57:14.643729 nanoscipy-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    17072 2022-11-21 14:57:02.000000 nanoscipy-3.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 14:57:14.639729 nanoscipy-3.0.9/nanoscipy/
+-rw-r--r--   0 runner    (1001) docker     (121)    30552 2022-11-21 14:57:02.000000 nanoscipy-3.0.9/nanoscipy/functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28154 2022-11-21 14:57:02.000000 nanoscipy-3.0.9/nanoscipy/mathpar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    55447 2022-11-21 14:57:02.000000 nanoscipy-3.0.9/nanoscipy/modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42345 2022-11-21 14:57:02.000000 nanoscipy-3.0.9/nanoscipy/unitpar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20936 2022-11-21 14:57:02.000000 nanoscipy-3.0.9/nanoscipy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 14:57:14.643729 nanoscipy-3.0.9/nanoscipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    17049 2022-11-21 14:57:14.000000 nanoscipy-3.0.9/nanoscipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2022-11-21 14:57:14.000000 nanoscipy-3.0.9/nanoscipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 14:57:14.000000 nanoscipy-3.0.9/nanoscipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-21 14:57:14.000000 nanoscipy-3.0.9/nanoscipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-21 14:57:14.000000 nanoscipy-3.0.9/nanoscipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-21 14:57:14.643729 nanoscipy-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      695 2022-11-21 14:57:02.000000 nanoscipy-3.0.9/setup.py
```

### Comparing `nanoscipy-3.0.8/PKG-INFO` & `nanoscipy-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: nanoscipy
-Version: 3.0.8
+Version: 3.0.9
 Summary: A package containing compiled functions, to make data-handling and -analysis easier.
 Home-page: https://github.com/nicholas12392/nanoscipy
 Author: Nicholas Hansen
 Author-email: nicholas.2000@live.dk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/nicholas12392/nanoscipy/issues
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 # nanoscipy
 
-nanoscipy has been made, to ease the more heavy data-handling, -processing, and - analysis. 
+nanoscipy has been made, to ease the data-handling, -processing, and - analysis. Additionally, it also provides a 
+simple way to perform numerical calculations with units.
 This package is being readily updated at the moment, so be sure to keep up, as new and useful additions and fixes are 
 very likely to be included.
 
 ## Installation and updating
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install nanoscipy like below. 
 Rerun this command to check for and install  updates .
 ```bash
@@ -178,22 +180,22 @@
 Planck constant `_h` or the speed of light in a vacuum `_c`. Note that all constants are denoted with an underscore.
 A full list of the supported units can be seen by calling the attribute `.supported_physical_constants`. 
 Depending on whether `units` is set to `True` or `False`, these natural constants will either have associated units or will 
 simply be the natural constant value with SI units:
 
 ```python
 test = nsm.NumAn(units=False)
-test.supported_physical_constants
+print(test.supported_physical_constants)
 ```
 ```
 >>> ('_hbar=1.0545718176461565e-34', ..., '_mp=1.67262192369e-27')
 ```
 ```python
 test = nsm.NumAn(units=True)
-test.supported_physical_constants
+print(test.supported_physical_constants)
 ```
 ```
 >>> ('_hbar=(1.0545718176461565e-34 J Hz^-1)', ..., '_mp=(1.67262192369e-27 kg)')
 ```
 ### 3) Calculations
 Calculations are performed via the `.calc()` attribute function. This effectively utilizes `unitpar.unit_parser()`, 
 which utilizes `mathpar.parser()` to compute the numerical part of the expression. An example of basic usage is seen
```

### Comparing `nanoscipy-3.0.8/README.md` & `nanoscipy-3.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # nanoscipy
 
-nanoscipy has been made, to ease the more heavy data-handling, -processing, and - analysis. 
+nanoscipy has been made, to ease the data-handling, -processing, and - analysis. Additionally, it also provides a 
+simple way to perform numerical calculations with units.
 This package is being readily updated at the moment, so be sure to keep up, as new and useful additions and fixes are 
 very likely to be included.
 
 ## Installation and updating
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install nanoscipy like below. 
 Rerun this command to check for and install  updates .
 ```bash
@@ -167,22 +168,22 @@
 Planck constant `_h` or the speed of light in a vacuum `_c`. Note that all constants are denoted with an underscore.
 A full list of the supported units can be seen by calling the attribute `.supported_physical_constants`. 
 Depending on whether `units` is set to `True` or `False`, these natural constants will either have associated units or will 
 simply be the natural constant value with SI units:
 
 ```python
 test = nsm.NumAn(units=False)
-test.supported_physical_constants
+print(test.supported_physical_constants)
 ```
 ```
 >>> ('_hbar=1.0545718176461565e-34', ..., '_mp=1.67262192369e-27')
 ```
 ```python
 test = nsm.NumAn(units=True)
-test.supported_physical_constants
+print(test.supported_physical_constants)
 ```
 ```
 >>> ('_hbar=(1.0545718176461565e-34 J Hz^-1)', ..., '_mp=(1.67262192369e-27 kg)')
 ```
 ### 3) Calculations
 Calculations are performed via the `.calc()` attribute function. This effectively utilizes `unitpar.unit_parser()`, 
 which utilizes `mathpar.parser()` to compute the numerical part of the expression. An example of basic usage is seen
```

### Comparing `nanoscipy-3.0.8/nanoscipy/functions.py` & `nanoscipy-3.0.9/nanoscipy/functions.py`

 * *Files identical despite different names*

### Comparing `nanoscipy-3.0.8/nanoscipy/mathpar.py` & `nanoscipy-3.0.9/nanoscipy/mathpar.py`

 * *Files identical despite different names*

### Comparing `nanoscipy-3.0.8/nanoscipy/modules.py` & `nanoscipy-3.0.9/nanoscipy/modules.py`

 * *Files identical despite different names*

### Comparing `nanoscipy-3.0.8/nanoscipy/unitpar.py` & `nanoscipy-3.0.9/nanoscipy/unitpar.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             unit_powers += [power_string]
             temp_split_list[i0:end_pos] = [power_string]
         i0 += 1  # update iterative
 
     # clean-up symbols from scientific notation and remove excess math symbols at the end
     unit_expression = split_list.copy()
     i0 = 0
-    while i0 < len(unit_expression):
+    while unit_expression and i0 < len(unit_expression):
         i0_val = unit_expression[i0]  # define current value
         ip1 = i0 + 1  # define right value index
         try:  # try to define real right value, otherwise set to None
             ip1_val = unit_expression[ip1]
         except IndexError:
             ip1_val = None
```

### Comparing `nanoscipy-3.0.8/nanoscipy/util.py` & `nanoscipy-3.0.9/nanoscipy/util.py`

 * *Files identical despite different names*

### Comparing `nanoscipy-3.0.8/nanoscipy.egg-info/PKG-INFO` & `nanoscipy-3.0.9/nanoscipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: nanoscipy
-Version: 3.0.8
+Version: 3.0.9
 Summary: A package containing compiled functions, to make data-handling and -analysis easier.
 Home-page: https://github.com/nicholas12392/nanoscipy
 Author: Nicholas Hansen
 Author-email: nicholas.2000@live.dk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/nicholas12392/nanoscipy/issues
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 # nanoscipy
 
-nanoscipy has been made, to ease the more heavy data-handling, -processing, and - analysis. 
+nanoscipy has been made, to ease the data-handling, -processing, and - analysis. Additionally, it also provides a 
+simple way to perform numerical calculations with units.
 This package is being readily updated at the moment, so be sure to keep up, as new and useful additions and fixes are 
 very likely to be included.
 
 ## Installation and updating
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install nanoscipy like below. 
 Rerun this command to check for and install  updates .
 ```bash
@@ -178,22 +180,22 @@
 Planck constant `_h` or the speed of light in a vacuum `_c`. Note that all constants are denoted with an underscore.
 A full list of the supported units can be seen by calling the attribute `.supported_physical_constants`. 
 Depending on whether `units` is set to `True` or `False`, these natural constants will either have associated units or will 
 simply be the natural constant value with SI units:
 
 ```python
 test = nsm.NumAn(units=False)
-test.supported_physical_constants
+print(test.supported_physical_constants)
 ```
 ```
 >>> ('_hbar=1.0545718176461565e-34', ..., '_mp=1.67262192369e-27')
 ```
 ```python
 test = nsm.NumAn(units=True)
-test.supported_physical_constants
+print(test.supported_physical_constants)
 ```
 ```
 >>> ('_hbar=(1.0545718176461565e-34 J Hz^-1)', ..., '_mp=(1.67262192369e-27 kg)')
 ```
 ### 3) Calculations
 Calculations are performed via the `.calc()` attribute function. This effectively utilizes `unitpar.unit_parser()`, 
 which utilizes `mathpar.parser()` to compute the numerical part of the expression. An example of basic usage is seen
```

### Comparing `nanoscipy-3.0.8/setup.py` & `nanoscipy-3.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='nanoscipy',
-    version='3.0.8',
+    version='3.0.9',
     author='Nicholas Hansen',
     author_email='nicholas.2000@live.dk',
     description='A package containing compiled functions, to make data-handling and -analysis easier.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/nicholas12392/nanoscipy',
     project_urls = {
```

