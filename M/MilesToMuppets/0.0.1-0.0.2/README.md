# Comparing `tmp/milestomuppets-0.0.1.tar.gz` & `tmp/milestomuppets-0.0.2.tar.gz`

## Comparing `milestomuppets-0.0.1.tar` & `milestomuppets-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 milestomuppets-0.0.1/src/milesToMuppets/__init__.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 milestomuppets-0.0.1/src/milesToMuppets/data.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 milestomuppets-0.0.1/src/milesToMuppets/functions.py
--rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 milestomuppets-0.0.1/src/milesToMuppets/muppet.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 milestomuppets-0.0.1/src/milesToMuppets/txt/links.txt
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 milestomuppets-0.0.1/src/milesToMuppets/txt/notes.txt
--rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 milestomuppets-0.0.1/tests/legacy.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 milestomuppets-0.0.1/tests/tmp
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 milestomuppets-0.0.1/LICENSE
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 milestomuppets-0.0.1/README.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 milestomuppets-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 milestomuppets-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/src/milesToMuppets/__init__.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/src/milesToMuppets/data.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/src/milesToMuppets/functions.py
+-rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/src/milesToMuppets/muppet.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/src/milesToMuppets/txt/links.txt
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/src/milesToMuppets/txt/notes.txt
+-rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/tests/legacy.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/tests/tmp
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/README.md
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/PKG-INFO
```

### Comparing `milestomuppets-0.0.1/src/milesToMuppets/functions.py` & `milestomuppets-0.0.2/src/milesToMuppets/functions.py`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.1/src/milesToMuppets/muppet.py` & `milestomuppets-0.0.2/src/milesToMuppets/muppet.py`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.1/tests/legacy.py` & `milestomuppets-0.0.2/tests/legacy.py`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.1/LICENSE` & `milestomuppets-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.1/README.md` & `milestomuppets-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Miles to Muppets
 A calculator that converts mile distance to how many Muppets songs you can listen to.
 
 # Setup
 
 - first, import **miletomuppets** <br>
-`import milestomuppets` <br>
+`from milesToMuppets import muppet` <br>
 
 - in the code, set up your class object, passing in your Spotify client id and client secret (which can be obtained from Spotify for Developers for free) <br>
-`foo = milestomuppets.MilesToMuppets(client_id = client_id, client_secret = client_secret)` <br>
+`foo = muppet.MilesToMuppets(client_id = client_id, client_secret = client_secret)` <br>
 
     - When initializing the class, if you want it to print data, initialize the class as so. <br>
 `foo = MilesToMuppets(client_id = client_id, client_secret = client_secret, output_mode = 'print')`
 
 - next, set the distance you are going, in miles. This number can be anything, but 60 is used as an example here. <br>
   `foo.set_mile_distance(60)`
```

### Comparing `milestomuppets-0.0.1/pyproject.toml` & `milestomuppets-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,28 @@
     "hatchling",
     "requests"
 ]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = [
-    "src/milesToMuppets"
+    "src/milesToMuppets",
+    "src/data",
+    "src/functions"
 ]
 
 [project]
 name = "MilesToMuppets"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Sketched Doughnut", email="author@example.com" },
 ]
 description = "A conversion package to convert Miles to how many songs you can listen to from the Muppets Album"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 # [project.urls]
```

### Comparing `milestomuppets-0.0.1/PKG-INFO` & `milestomuppets-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.3
 Name: MilesToMuppets
-Version: 0.0.1
+Version: 0.0.2
 Summary: A conversion package to convert Miles to how many songs you can listen to from the Muppets Album
 Author-email: Sketched Doughnut <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Miles to Muppets
 A calculator that converts mile distance to how many Muppets songs you can listen to.
 
 # Setup
 
 - first, import **miletomuppets** <br>
-`import milestomuppets` <br>
+`from milesToMuppets import muppet` <br>
 
 - in the code, set up your class object, passing in your Spotify client id and client secret (which can be obtained from Spotify for Developers for free) <br>
-`foo = milestomuppets.MilesToMuppets(client_id = client_id, client_secret = client_secret)` <br>
+`foo = muppet.MilesToMuppets(client_id = client_id, client_secret = client_secret)` <br>
 
     - When initializing the class, if you want it to print data, initialize the class as so. <br>
 `foo = MilesToMuppets(client_id = client_id, client_secret = client_secret, output_mode = 'print')`
 
 - next, set the distance you are going, in miles. This number can be anything, but 60 is used as an example here. <br>
   `foo.set_mile_distance(60)`
```

