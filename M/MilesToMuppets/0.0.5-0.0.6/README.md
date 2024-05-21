# Comparing `tmp/milestomuppets-0.0.5.tar.gz` & `tmp/milestomuppets-0.0.6.tar.gz`

## Comparing `milestomuppets-0.0.5.tar` & `milestomuppets-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 milestomuppets-0.0.5/src/milesToMuppets/__init__.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 milestomuppets-0.0.5/src/milesToMuppets/data.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 milestomuppets-0.0.5/src/milesToMuppets/functions.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 milestomuppets-0.0.5/src/milesToMuppets/muppet.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 milestomuppets-0.0.5/src/milesToMuppets/txt/links.txt
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 milestomuppets-0.0.5/src/milesToMuppets/txt/notes.txt
--rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 milestomuppets-0.0.5/tests/legacy.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 milestomuppets-0.0.5/tests/tmp
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 milestomuppets-0.0.5/LICENSE
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 milestomuppets-0.0.5/README.md
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 milestomuppets-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 milestomuppets-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/src/milesToMuppets/__init__.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/src/milesToMuppets/data.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/src/milesToMuppets/functions.py
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/src/milesToMuppets/muppet.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/src/milesToMuppets/txt/links.txt
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/src/milesToMuppets/txt/notes.txt
+-rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/tests/legacy.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/tests/tmp
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/README.md
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 milestomuppets-0.0.6/PKG-INFO
```

### Comparing `milestomuppets-0.0.5/src/milesToMuppets/functions.py` & `milestomuppets-0.0.6/src/milesToMuppets/functions.py`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.5/src/milesToMuppets/muppet.py` & `milestomuppets-0.0.6/src/milesToMuppets/muppet.py`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.5/tests/legacy.py` & `milestomuppets-0.0.6/tests/legacy.py`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.5/LICENSE` & `milestomuppets-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.5/README.md` & `milestomuppets-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.5/pyproject.toml` & `milestomuppets-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -10,21 +10,21 @@
     "src/milesToMuppets",
     "src/data",
     "src/functions"
 ]
 
 [project]
 name = "MilesToMuppets"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Sketched Doughnut", email="sketcheddoughnut@gmail.com" },
 ]
 description = "A conversion package to convert Miles to how many songs you can listen to from the Muppets Album"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `milestomuppets-0.0.5/PKG-INFO` & `milestomuppets-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: MilesToMuppets
-Version: 0.0.5
+Version: 0.0.6
 Summary: A conversion package to convert Miles to how many songs you can listen to from the Muppets Album
 Project-URL: Homepage, https://github.com/SketchedDoughnut/miles-to-muppets
 Project-URL: Issues, https://github.com/SketchedDoughnut/miles-to-muppets/issues
 Author-email: Sketched Doughnut <sketcheddoughnut@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Miles to Muppets
 A calculator that converts mile distance to how many Muppets songs you can listen to.
 
 # Setup
```

