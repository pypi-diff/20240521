# Comparing `tmp/milestomuppets-0.0.3.tar.gz` & `tmp/milestomuppets-0.0.4.tar.gz`

## Comparing `milestomuppets-0.0.3.tar` & `milestomuppets-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/src/milesToMuppets/__init__.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/src/milesToMuppets/data.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/src/milesToMuppets/functions.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/src/milesToMuppets/muppet.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/src/milesToMuppets/txt/links.txt
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/src/milesToMuppets/txt/notes.txt
--rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/tests/legacy.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/tests/tmp
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/LICENSE
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/README.md
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 milestomuppets-0.0.4/src/milesToMuppets/__init__.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 milestomuppets-0.0.4/src/milesToMuppets/data.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 milestomuppets-0.0.4/src/milesToMuppets/functions.py
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 milestomuppets-0.0.4/src/milesToMuppets/muppet.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 milestomuppets-0.0.4/src/milesToMuppets/txt/links.txt
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 milestomuppets-0.0.4/src/milesToMuppets/txt/notes.txt
+-rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 milestomuppets-0.0.4/tests/legacy.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 milestomuppets-0.0.4/tests/tmp
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 milestomuppets-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 milestomuppets-0.0.4/README.md
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 milestomuppets-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 milestomuppets-0.0.4/PKG-INFO
```

### Comparing `milestomuppets-0.0.3/src/milesToMuppets/functions.py` & `milestomuppets-0.0.4/src/milesToMuppets/functions.py`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.3/src/milesToMuppets/muppet.py` & `milestomuppets-0.0.4/src/milesToMuppets/muppet.py`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.3/tests/legacy.py` & `milestomuppets-0.0.4/tests/legacy.py`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.3/LICENSE` & `milestomuppets-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.3/README.md` & `milestomuppets-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,25 @@
+Metadata-Version: 2.3
+Name: MilesToMuppets
+Version: 0.0.4
+Summary: A conversion package to convert Miles to how many songs you can listen to from the Muppets Album
+Author-email: Sketched Doughnut <author@example.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+
 # Miles to Muppets
 A calculator that converts mile distance to how many Muppets songs you can listen to.
 
 # Setup
 
-- first, import **miletomuppets** <br>
+- first, import muppet from milesToMuppets <br>
 `from milesToMuppets import muppet` <br>
 
 - in the code, set up your class object, passing in your Spotify client id and client secret (which can be obtained from Spotify for Developers for free) <br>
 `foo = muppet.MilesToMuppets(client_id = client_id, client_secret = client_secret)` <br>
 
     - When initializing the class, if you want it to print data, initialize the class as so. <br>
 `foo = MilesToMuppets(client_id = client_id, client_secret = client_secret, output_mode = 'print')`
```

### Comparing `milestomuppets-0.0.3/pyproject.toml` & `milestomuppets-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "src/milesToMuppets",
     "src/data",
     "src/functions"
 ]
 
 [project]
 name = "MilesToMuppets"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Sketched Doughnut", email="author@example.com" },
 ]
 description = "A conversion package to convert Miles to how many songs you can listen to from the Muppets Album"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `milestomuppets-0.0.3/PKG-INFO` & `milestomuppets-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,13 @@
-Metadata-Version: 2.3
-Name: MilesToMuppets
-Version: 0.0.3
-Summary: A conversion package to convert Miles to how many songs you can listen to from the Muppets Album
-Author-email: Sketched Doughnut <author@example.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-
 # Miles to Muppets
 A calculator that converts mile distance to how many Muppets songs you can listen to.
 
 # Setup
 
-- first, import **miletomuppets** <br>
+- first, import muppet from milesToMuppets <br>
 `from milesToMuppets import muppet` <br>
 
 - in the code, set up your class object, passing in your Spotify client id and client secret (which can be obtained from Spotify for Developers for free) <br>
 `foo = muppet.MilesToMuppets(client_id = client_id, client_secret = client_secret)` <br>
 
     - When initializing the class, if you want it to print data, initialize the class as so. <br>
 `foo = MilesToMuppets(client_id = client_id, client_secret = client_secret, output_mode = 'print')`
```

