# Comparing `tmp/elmer_circuitbuilder-1.0.0.tar.gz` & `tmp/elmer_circuitbuilder-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elmer_circuitbuilder-1.0.0.tar", last modified: Wed Aug 16 13:39:26 2023, max compression
+gzip compressed data, was "elmer_circuitbuilder-1.0.1.tar", last modified: Tue May 21 17:10:34 2024, max compression
```

## Comparing `elmer_circuitbuilder-1.0.0.tar` & `elmer_circuitbuilder-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2023-08-16 13:39:26.832892 elmer_circuitbuilder-1.0.0/
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)      196 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/AUTHORS.rst
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)     3798 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/CONTRIBUTING.rst
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       89 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/HISTORY.rst
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)     7651 2023-08-16 13:20:49.000000 elmer_circuitbuilder-1.0.0/LICENSE
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)      265 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/MANIFEST.in
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)     2566 2023-08-16 13:39:26.833145 elmer_circuitbuilder-1.0.0/PKG-INFO
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)    16177 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/README.md
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)     1405 2023-08-16 13:20:44.000000 elmer_circuitbuilder-1.0.0/README.rst
-drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2023-08-16 13:39:26.825676 elmer_circuitbuilder-1.0.0/docs/
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)      621 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/docs/Makefile
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       28 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/docs/authors.rst
--rwxr-xr-x   0 jonathanvelasco   (501) staff       (20)     4959 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/docs/conf.py
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       33 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/docs/contributing.rst
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       28 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/docs/history.rst
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)      317 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/docs/index.rst
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)     1218 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/docs/installation.rst
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)      782 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/docs/make.bat
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       27 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/docs/readme.rst
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       95 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/docs/usage.rst
-drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2023-08-16 13:39:26.826289 elmer_circuitbuilder-1.0.0/elmer_circuitbuilder/
-drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2023-08-16 13:39:26.830869 elmer_circuitbuilder-1.0.0/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)     2566 2023-08-16 13:39:26.000000 elmer_circuitbuilder-1.0.0/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/PKG-INFO
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)      751 2023-08-16 13:39:26.000000 elmer_circuitbuilder-1.0.0/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)        1 2023-08-16 13:39:26.000000 elmer_circuitbuilder-1.0.0/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)        1 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/not-zip-safe
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       19 2023-08-16 13:39:26.000000 elmer_circuitbuilder-1.0.0/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/requires.txt
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       21 2023-08-16 13:39:26.000000 elmer_circuitbuilder-1.0.0/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/top_level.txt
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)    75570 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/elmer_circuitbuilder/elmer_circuitbuilder.py
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)      437 2023-08-16 13:39:26.835777 elmer_circuitbuilder-1.0.0/setup.cfg
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)     1783 2023-08-16 13:36:45.000000 elmer_circuitbuilder-1.0.0/setup.py
-drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2023-08-16 13:39:26.832340 elmer_circuitbuilder-1.0.0/tests/
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)       50 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/tests/__init__.py
--rw-r--r--   0 jonathanvelasco   (501) staff       (20)      766 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.0/tests/test_elmer_circuitbuilder.py
+drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2024-05-21 17:10:34.838193 elmer_circuitbuilder-1.0.1/
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)      196 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/AUTHORS.rst
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)     3798 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       89 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/HISTORY.rst
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)     7651 2023-08-16 13:20:49.000000 elmer_circuitbuilder-1.0.1/LICENSE
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)      265 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/MANIFEST.in
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)     2609 2024-05-21 17:10:34.837818 elmer_circuitbuilder-1.0.1/PKG-INFO
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)    16177 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/README.md
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)     1405 2023-08-16 13:20:44.000000 elmer_circuitbuilder-1.0.1/README.rst
+drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2024-05-21 17:10:34.828530 elmer_circuitbuilder-1.0.1/docs/
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)      621 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/docs/Makefile
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       28 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/docs/authors.rst
+-rwxr-xr-x   0 jonathanvelasco   (501) staff       (20)     4959 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/docs/conf.py
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       33 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/docs/contributing.rst
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       28 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/docs/history.rst
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)      317 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/docs/index.rst
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)     1218 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/docs/installation.rst
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)      782 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/docs/make.bat
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       27 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/docs/readme.rst
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       95 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/docs/usage.rst
+drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2024-05-21 17:10:34.829140 elmer_circuitbuilder-1.0.1/elmer_circuitbuilder/
+drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2024-05-21 17:10:34.836001 elmer_circuitbuilder-1.0.1/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)     2609 2024-05-21 17:10:34.000000 elmer_circuitbuilder-1.0.1/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)      751 2024-05-21 17:10:34.000000 elmer_circuitbuilder-1.0.1/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)        1 2024-05-21 17:10:34.000000 elmer_circuitbuilder-1.0.1/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)        1 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/not-zip-safe
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       19 2024-05-21 17:10:34.000000 elmer_circuitbuilder-1.0.1/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/requires.txt
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       21 2024-05-21 17:10:34.000000 elmer_circuitbuilder-1.0.1/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/top_level.txt
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)    75263 2024-05-21 16:59:54.000000 elmer_circuitbuilder-1.0.1/elmer_circuitbuilder/elmer_circuitbuilder.py
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)      437 2024-05-21 17:10:34.839307 elmer_circuitbuilder-1.0.1/setup.cfg
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)     1783 2024-05-21 17:09:04.000000 elmer_circuitbuilder-1.0.1/setup.py
+drwxr-xr-x   0 jonathanvelasco   (501) staff       (20)        0 2024-05-21 17:10:34.835183 elmer_circuitbuilder-1.0.1/tests/
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)       50 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/tests/__init__.py
+-rw-r--r--   0 jonathanvelasco   (501) staff       (20)      766 2023-08-16 13:11:05.000000 elmer_circuitbuilder-1.0.1/tests/test_elmer_circuitbuilder.py
```

### Comparing `elmer_circuitbuilder-1.0.0/CONTRIBUTING.rst` & `elmer_circuitbuilder-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.0/LICENSE` & `elmer_circuitbuilder-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.0/PKG-INFO` & `elmer_circuitbuilder-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elmer_circuitbuilder
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python module for creating the circuit simulation definitions for Elmer FEM. The circuit definitions enable easy setup of coils (e.g. massive, stranded, and foil) in 2D and 3D for magnetodynamics applications.
 Home-page: https://github.com/ElmerCSC/elmer_circuitbuilder.git
 Author: Jonathan Velasco
 Author-email: velasco_jonathan@hotmail.com
 Maintainer: CSC - IT Center for Science :  ElmerFEM Developers
 License: GNU Lesser General Public License v3
 Keywords: elmer_circuitbuilder
@@ -13,17 +13,18 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
-Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.rst
+Provides-Extra: dev
+Requires-Dist: pytest>=3.7; extra == "dev"
 
 ====================
 elmer_circuitbuilder
 ====================
 
 
 .. image:: https://img.shields.io/pypi/v/elmer_circuitbuilder.svg
```

### Comparing `elmer_circuitbuilder-1.0.0/README.md` & `elmer_circuitbuilder-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.0/README.rst` & `elmer_circuitbuilder-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.0/docs/Makefile` & `elmer_circuitbuilder-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.0/docs/conf.py` & `elmer_circuitbuilder-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.0/docs/installation.rst` & `elmer_circuitbuilder-1.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.0/docs/make.bat` & `elmer_circuitbuilder-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.0/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/PKG-INFO` & `elmer_circuitbuilder-1.0.1/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: elmer-circuitbuilder
-Version: 1.0.0
+Name: elmer_circuitbuilder
+Version: 1.0.1
 Summary: Python module for creating the circuit simulation definitions for Elmer FEM. The circuit definitions enable easy setup of coils (e.g. massive, stranded, and foil) in 2D and 3D for magnetodynamics applications.
 Home-page: https://github.com/ElmerCSC/elmer_circuitbuilder.git
 Author: Jonathan Velasco
 Author-email: velasco_jonathan@hotmail.com
 Maintainer: CSC - IT Center for Science :  ElmerFEM Developers
 License: GNU Lesser General Public License v3
 Keywords: elmer_circuitbuilder
@@ -13,17 +13,18 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
-Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.rst
+Provides-Extra: dev
+Requires-Dist: pytest>=3.7; extra == "dev"
 
 ====================
 elmer_circuitbuilder
 ====================
 
 
 .. image:: https://img.shields.io/pypi/v/elmer_circuitbuilder.svg
```

### Comparing `elmer_circuitbuilder-1.0.0/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/SOURCES.txt` & `elmer_circuitbuilder-1.0.1/elmer_circuitbuilder/elmer_circuitbuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elmer_circuitbuilder-1.0.0/elmer_circuitbuilder/elmer_circuitbuilder.py` & `elmer_circuitbuilder-1.0.1/elmer_circuitbuilder/elmer_circuitbuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -535,17 +535,17 @@
 
     # dummy vector for indexing in A matrix
     plus_terminal = [i for i in range(0, numedges)]
     minus_terminal = [i for i in range(0, numedges)]
 
     # initialize string matrices
     Amat_plus_str = np.chararray((numnodes, numedges))
-    Amat_plus_str = np.chararray(Amat_plus_str.shape, itemsize=3)
+    Amat_plus_str = np.chararray(Amat_plus_str.shape, itemsize=500)
     Amat_minus_str = np.chararray((numnodes, numedges))
-    Amat_minus_str = np.chararray(Amat_minus_str.shape, itemsize=3)
+    Amat_minus_str = np.chararray(Amat_minus_str.shape, itemsize=500)
 
     # initialize zero char in all matrices
     for i in range(0, numnodes):
         for j in range(0, numedges):
             Amat_plus_str[i][j] = ''
             Amat_minus_str[i][j] = ''
 
@@ -642,19 +642,19 @@
     ----------
     Rmat_str : numpy.chararray
         Returns string/char resistance matrix
 
     """
     # initialize R matrix. R = R_r + R_i + R_cap
     Rmat_r_str = np.chararray((nedges, nedges))
-    Rmat_r_str = np.chararray(Rmat_r_str.shape, itemsize=5)
+    Rmat_r_str = np.chararray(Rmat_r_str.shape, itemsize=500)
     Rmat_i_str = np.chararray((nedges, nedges))
-    Rmat_i_str = np.chararray(Rmat_i_str.shape, itemsize=5)
+    Rmat_i_str = np.chararray(Rmat_i_str.shape, itemsize=500)
     Rmat_cap_str = np.chararray((nedges, nedges))
-    Rmat_cap_str = np.chararray(Rmat_cap_str.shape, itemsize=5)
+    Rmat_cap_str = np.chararray(Rmat_cap_str.shape, itemsize=500)
 
     # initialize zero char in all matrices
 
     for i in range(0, nedges):
         for j in range(0, nedges):
             Rmat_r_str[i][j] = ''
             Rmat_i_str[i][j] = ''
@@ -751,19 +751,19 @@
     Gmat_str : numpy.chararray
         Returns string/char conductance matrix
 
     """
     # initialize G matrix. G = G_r + G_v + G_ind
     # (resistor, voltage generators, inductors)
     Gmat_r_str = np.chararray((nedges, nedges))
-    Gmat_r_str = np.chararray(Gmat_r_str.shape, itemsize=5)
+    Gmat_r_str = np.chararray(Gmat_r_str.shape, itemsize=500)
     Gmat_v_str = np.chararray((nedges, nedges))
-    Gmat_v_str = np.chararray(Gmat_v_str.shape, itemsize=5)
+    Gmat_v_str = np.chararray(Gmat_v_str.shape, itemsize=500)
     Gmat_ind_str = np.chararray((nedges, nedges))
-    Gmat_ind_str = np.chararray(Gmat_ind_str.shape, itemsize=5)
+    Gmat_ind_str = np.chararray(Gmat_ind_str.shape, itemsize=500)
 
     # initialize zero char in all matrices
     for i in range(0, nedges):
         for j in range(0, nedges):
             Gmat_r_str[i][j] = ''
             Gmat_v_str[i][j] = ''
             Gmat_ind_str[i][j] = ''
@@ -831,15 +831,15 @@
     Returns
     ----------
     Lmat_str : numpy.chararray
         Returns string/char inductance matrix
     """
     # initialize L matrix.
     Lmat_str = np.chararray((nedges, nedges))
-    Lmat_str = np.chararray(Lmat_str.shape, itemsize=5)
+    Lmat_str = np.chararray(Lmat_str.shape, itemsize=500)
 
     # initialize zero char in all matrices
     for i in range(0, nedges):
         for j in range(0, nedges):
             Lmat_str[i][j] = ''
 
     for i in indInd:
@@ -895,15 +895,15 @@
     Returns
     ----------
     Cmat_str : numpy.chararray
         Returns string/char capacitance matrix
     """
     # initialize L matrix.
     Cmat_str = np.chararray((nedges, nedges))
-    Cmat_str = np.chararray(Cmat_str.shape, itemsize=5)
+    Cmat_str = np.chararray(Cmat_str.shape, itemsize=500)
 
     # initialize zero char in all matrices
     for i in range(0, nedges):
         for j in range(0, nedges):
             Cmat_str[i][j] = ''
 
     for i in indcap:
@@ -1005,18 +1005,18 @@
     rhs : numpy.chararray
         Returns string/char source vector
     """
 
     # initialize RHS vector. RHS = RHS_i + RHS_v
     # (current source, voltage source)
     rhs_v_str = np.chararray((nedges, 1))
-    rhs_v_str = np.chararray(rhs_v_str.shape, itemsize=5)
+    rhs_v_str = np.chararray(rhs_v_str.shape, itemsize=500)
 
     rhs_i_str = np.chararray((nedges, 1))
-    rhs_i_str = np.chararray(rhs_i_str.shape, itemsize=5)
+    rhs_i_str = np.chararray(rhs_i_str.shape, itemsize=500)
 
     # initialize zero char in all matrices
     for i in range(0, nedges):
         rhs_v_str[i] = ''
         rhs_i_str[i] = ''
 
     #complex_switch = True  # used to create separate real and imag rhs
@@ -1922,18 +1922,16 @@
         name = component.name
         value = component.value
 
         val_sign = ""
         if "-" in str_val:
             val_sign = "-"
         if isinstance(value, complex):
-            body_force_list.append("  " + name + "_Source re = Real $ " + val_sign + "re_" + str_val.strip("-")
-                                   + "*cos(phase_" + name+")")
-            body_force_list.append("  " + name + "_Source im = Real $ " + val_sign + "im_" + str_val.strip("-")
-                                   + "*sin(phase_" + name+")")
+            body_force_list.append("  " + name + "_Source re = Real $ " + val_sign + "re_" + str_val.strip("-"))
+            body_force_list.append("  " + name + "_Source im = Real $ " + val_sign + "im_" + str_val.strip("-"))
         else:
             body_force_list.append("  " + name + "_Source = Variable \"time\" \n  \t Real MATC \""
                                    + str_val.strip("-") + "\"")
 
     elmer_file.close()
 
     return body_force_list
@@ -1997,17 +1995,14 @@
                       + "\t ! Number of Turns", file=elmer_file)
                 print("$ L_" + component.name + " = " + str(component.getCoilThickness())
                       + "\t ! Coil Thickness", file=elmer_file)
 
             print("$ Ns_" + component.name + " = " + str(component.sector)
                   + "\t ! Sector/Symmetry Coefficient (e.g. 4 is 1/4 of the domain)", file=elmer_file)
 
-            if(component.dimension == "3D"):
-                print("$ Ae_" + component.name + " = 0.0025 " + "\t ! Electrode Area (dummy for now change as required)"
-                      , file=elmer_file)
     print("", file=elmer_file)
 
     elmer_file.close
 
 
 def write_elmer_circuit_file(c, elmerA, elmerB, elmersource, unknown_names, num_nodes, num_edges, ofile):
     """
```

### Comparing `elmer_circuitbuilder-1.0.0/setup.py` & `elmer_circuitbuilder-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,14 @@
     include_package_data=True,
     keywords='elmer_circuitbuilder',
     name='elmer_circuitbuilder',
     #packages=find_packages(include=['elmer_circuitbuilder', 'elmer_circuitbuilder.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ElmerCSC/elmer_circuitbuilder.git',
-    version='v1.0.0',
+    version='v1.0.1',
     zip_safe=False,
     extras_require={"dev":["pytest>=3.7"], },
     py_modules=["elmer_circuitbuilder"],
     package_dir={'': 'elmer_circuitbuilder'},
 
 )
```

### Comparing `elmer_circuitbuilder-1.0.0/tests/test_elmer_circuitbuilder.py` & `elmer_circuitbuilder-1.0.1/tests/test_elmer_circuitbuilder.py`

 * *Files identical despite different names*

