# Comparing `tmp/milestomuppets-0.0.6.tar.gz` & `tmp/milestomuppets-0.0.7.tar.gz`

## Comparing `milestomuppets-0.0.6.tar` & `milestomuppets-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/src/milesToMuppets/__init__.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/src/milesToMuppets/data.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/src/milesToMuppets/functions.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/src/milesToMuppets/muppet.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/src/milesToMuppets/txt/links.txt
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/src/milesToMuppets/txt/notes.txt
--rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/tests/legacy.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/tests/tmp
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/LICENSE
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/README.md
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 milestomuppets-0.0.7/src/milesToMuppets/__init__.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 milestomuppets-0.0.7/src/milesToMuppets/data.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 milestomuppets-0.0.7/src/milesToMuppets/functions.py
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 milestomuppets-0.0.7/src/milesToMuppets/muppet.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 milestomuppets-0.0.7/src/milesToMuppets/txt/links.txt
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 milestomuppets-0.0.7/src/milesToMuppets/txt/notes.txt
+-rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 milestomuppets-0.0.7/tests/legacy.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 milestomuppets-0.0.7/tests/tmp
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 milestomuppets-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 milestomuppets-0.0.7/README.md
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 milestomuppets-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 milestomuppets-0.0.7/PKG-INFO
```

### Comparing `milestomuppets-0.0.6/src/milesToMuppets/functions.py` & `milestomuppets-0.0.7/src/milesToMuppets/functions.py`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.6/src/milesToMuppets/muppet.py` & `milestomuppets-0.0.7/src/milesToMuppets/muppet.py`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.6/tests/legacy.py` & `milestomuppets-0.0.7/tests/legacy.py`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.6/LICENSE` & `milestomuppets-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.6/README.md` & `milestomuppets-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.6/PKG-INFO` & `milestomuppets-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.3
 Name: MilesToMuppets
-Version: 0.0.6
+Version: 0.0.7
 Summary: A conversion package to convert Miles to how many songs you can listen to from the Muppets Album
 Project-URL: Homepage, https://github.com/SketchedDoughnut/miles-to-muppets
 Project-URL: Issues, https://github.com/SketchedDoughnut/miles-to-muppets/issues
 Author-email: Sketched Doughnut <sketcheddoughnut@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # Miles to Muppets
 A calculator that converts mile distance to how many Muppets songs you can listen to.
 
 # Setup
```

