# Comparing `tmp/elmer_circuitbuilder-1.0.2.tar.gz` & `tmp/elmer_circuitbuilder-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elmer_circuitbuilder-1.0.2.tar", last modified: Tue May 21 17:38:50 2024, max compression
+gzip compressed data, was "elmer_circuitbuilder-1.0.3.tar", last modified: Tue May 21 18:44:42 2024, max compression
```

## Comparing `elmer_circuitbuilder-1.0.2.tar` & `elmer_circuitbuilder-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2024-05-21 17:38:50.659635 elmer_circuitbuilder-1.0.2/
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)      196 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/AUTHORS.rst
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)     3798 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       89 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/HISTORY.rst
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)     7651 2023-08-16 13:20:49.000000 elmer_circuitbuilder-1.0.2/LICENSE
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)      265 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/MANIFEST.in
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)     2609 2024-05-21 17:38:50.659288 elmer_circuitbuilder-1.0.2/PKG-INFO
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)    16177 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/README.md
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)     1405 2023-08-16 13:20:44.000000 elmer_circuitbuilder-1.0.2/README.rst
-drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2024-05-21 17:38:50.644867 elmer_circuitbuilder-1.0.2/docs/
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)      621 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/docs/Makefile
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       28 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/docs/authors.rst
--rwxr-xr-x   0 jonathanvelasco   (501) staff       (20)     4959 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/docs/conf.py
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       33 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/docs/contributing.rst
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       28 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/docs/history.rst
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)      317 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/docs/index.rst
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)     1218 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/docs/installation.rst
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)      782 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/docs/make.bat
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       27 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/docs/readme.rst
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       95 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/docs/usage.rst
-drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2024-05-21 17:38:50.645882 elmer_circuitbuilder-1.0.2/elmer_circuitbuilder/
-drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2024-05-21 17:38:50.657147 elmer_circuitbuilder-1.0.2/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)     2609 2024-05-21 17:38:50.000000 elmer_circuitbuilder-1.0.2/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/PKG-INFO
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)      751 2024-05-21 17:38:50.000000 elmer_circuitbuilder-1.0.2/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)        1 2024-05-21 17:38:50.000000 elmer_circuitbuilder-1.0.2/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)        1 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/not-zip-safe
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       19 2024-05-21 17:38:50.000000 elmer_circuitbuilder-1.0.2/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/requires.txt
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       21 2024-05-21 17:38:50.000000 elmer_circuitbuilder-1.0.2/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/top_level.txt
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)    75263 2024-05-21 16:59:54.000000 elmer_circuitbuilder-1.0.2/elmer_circuitbuilder/elmer_circuitbuilder.py
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)      437 2024-05-21 17:38:50.660979 elmer_circuitbuilder-1.0.2/setup.cfg
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)     1783 2024-05-21 17:38:39.000000 elmer_circuitbuilder-1.0.2/setup.py
-drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2024-05-21 17:38:50.656189 elmer_circuitbuilder-1.0.2/tests/
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       50 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/tests/__init__.py
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)      766 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.2/tests/test_elmer_circuitbuilder.py
+drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2024-05-21 18:44:42.509197 elmer_circuitbuilder-1.0.3/
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)      196 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/AUTHORS.rst
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)     3798 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       89 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/HISTORY.rst
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)     7651 2023-08-16 13:20:49.000000 elmer_circuitbuilder-1.0.3/LICENSE
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)      265 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/MANIFEST.in
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)     2609 2024-05-21 18:44:42.508570 elmer_circuitbuilder-1.0.3/PKG-INFO
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)    16177 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/README.md
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)     1405 2023-08-16 13:20:44.000000 elmer_circuitbuilder-1.0.3/README.rst
+drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2024-05-21 18:44:42.493210 elmer_circuitbuilder-1.0.3/docs/
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)      621 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/docs/Makefile
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       28 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/docs/authors.rst
+-rwxr-xr-x   0 jonathanvelasco   (501) staff       (20)     4959 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/docs/conf.py
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       33 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/docs/contributing.rst
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       28 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/docs/history.rst
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)      317 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/docs/index.rst
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)     1218 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/docs/installation.rst
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)      782 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/docs/make.bat
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       27 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/docs/readme.rst
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       95 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/docs/usage.rst
+drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2024-05-21 18:44:42.495682 elmer_circuitbuilder-1.0.3/elmer_circuitbuilder/
+drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2024-05-21 18:44:42.506736 elmer_circuitbuilder-1.0.3/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)     2609 2024-05-21 18:44:42.000000 elmer_circuitbuilder-1.0.3/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)      751 2024-05-21 18:44:42.000000 elmer_circuitbuilder-1.0.3/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)        1 2024-05-21 18:44:42.000000 elmer_circuitbuilder-1.0.3/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)        1 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/not-zip-safe
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       19 2024-05-21 18:44:42.000000 elmer_circuitbuilder-1.0.3/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/requires.txt
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       21 2024-05-21 18:44:42.000000 elmer_circuitbuilder-1.0.3/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/top_level.txt
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)    75253 2024-05-21 18:37:01.000000 elmer_circuitbuilder-1.0.3/elmer_circuitbuilder/elmer_circuitbuilder.py
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)      437 2024-05-21 18:44:42.511926 elmer_circuitbuilder-1.0.3/setup.cfg
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)     1783 2024-05-21 18:41:57.000000 elmer_circuitbuilder-1.0.3/setup.py
+drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2024-05-21 18:44:42.505430 elmer_circuitbuilder-1.0.3/tests/
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       50 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/tests/__init__.py
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)      766 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.3/tests/test_elmer_circuitbuilder.py
```

### Comparing `elmer_circuitbuilder-1.0.2/CONTRIBUTING.rst` & `elmer_circuitbuilder-1.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.2/LICENSE` & `elmer_circuitbuilder-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.2/PKG-INFO` & `elmer_circuitbuilder-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elmer_circuitbuilder
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python module for creating the circuit simulation definitions for Elmer FEM. The circuit definitions enable easy setup of coils (e.g. massive, stranded, and foil) in 2D and 3D for magnetodynamics applications.
 Home-page: https://github.com/ElmerCSC/elmer_circuitbuilder.git
 Author: Jonathan Velasco
 Author-email: velasco_jonathan@hotmail.com
 Maintainer: CSC - IT Center for Science :  ElmerFEM Developers
 License: GNU Lesser General Public License v3
 Keywords: elmer_circuitbuilder
```

### Comparing `elmer_circuitbuilder-1.0.2/README.md` & `elmer_circuitbuilder-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.2/README.rst` & `elmer_circuitbuilder-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.2/docs/Makefile` & `elmer_circuitbuilder-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.2/docs/conf.py` & `elmer_circuitbuilder-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.2/docs/installation.rst` & `elmer_circuitbuilder-1.0.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.2/docs/make.bat` & `elmer_circuitbuilder-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.2/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/PKG-INFO` & `elmer_circuitbuilder-1.0.3/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elmer_circuitbuilder
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python module for creating the circuit simulation definitions for Elmer FEM. The circuit definitions enable easy setup of coils (e.g. massive, stranded, and foil) in 2D and 3D for magnetodynamics applications.
 Home-page: https://github.com/ElmerCSC/elmer_circuitbuilder.git
 Author: Jonathan Velasco
 Author-email: velasco_jonathan@hotmail.com
 Maintainer: CSC - IT Center for Science :  ElmerFEM Developers
 License: GNU Lesser General Public License v3
 Keywords: elmer_circuitbuilder
```

### Comparing `elmer_circuitbuilder-1.0.2/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/SOURCES.txt` & `elmer_circuitbuilder-1.0.3/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.2/elmer_circuitbuilder/elmer_circuitbuilder.py` & `elmer_circuitbuilder-1.0.3/elmer_circuitbuilder/elmer_circuitbuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1968,16 +1968,16 @@
     print("! General Parameters ", file=elmer_file)
     for component in components:
         if not isinstance(component, ElmerComponent):
             if(isinstance(component.value, complex)):
                 print("! " + component.name + " = re_" + component.name + "+ j im_" + component.name + ", phase_"
                       + component.name + " = " + str(np.degrees(cmath.phase(component.value)))
                       + "(Deg)", file=elmer_file)
-                print("$ re_" + component.name + " = " + str(abs(np.real(component.value))), file=elmer_file)
-                print("$ im_" + component.name + " = " + str(abs(np.imag(component.value))), file=elmer_file)
+                print("$ re_" + component.name + " = " + str(np.real(component.value)), file=elmer_file)
+                print("$ im_" + component.name + " = " + str(np.imag(component.value)), file=elmer_file)
                 print("$ phase_" + component.name + " = " + str(cmath.phase(component.value)), file=elmer_file)
             else:
                 print("$ " + component.name + " = " + str(component.value), file=elmer_file)
     print("", file=elmer_file)
 
     for component in components:
         if isinstance(component, ElmerComponent):
```

### Comparing `elmer_circuitbuilder-1.0.2/setup.py` & `elmer_circuitbuilder-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,14 @@
     include_package_data=True,
     keywords='elmer_circuitbuilder',
     name='elmer_circuitbuilder',
     #packages=find_packages(include=['elmer_circuitbuilder', 'elmer_circuitbuilder.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ElmerCSC/elmer_circuitbuilder.git',
-    version='v1.0.2',
+    version='v1.0.3',
     zip_safe=False,
     extras_require={"dev":["pytest>=3.7"], },
     py_modules=["elmer_circuitbuilder"],
     package_dir={'': 'elmer_circuitbuilder'},
 
 )
```

### Comparing `elmer_circuitbuilder-1.0.2/tests/test_elmer_circuitbuilder.py` & `elmer_circuitbuilder-1.0.3/tests/test_elmer_circuitbuilder.py`

 * *Files identical despite different names*

