# Comparing `tmp/pyodre-0.0.1.tar.gz` & `tmp/pyodre-0.0.2.tar.gz`

## Comparing `pyodre-0.0.1.tar` & `pyodre-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pyodre-0.0.1/interpreters.py
--rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 pyodre-0.0.1/pyodre.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 pyodre-0.0.1/python_functions.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 pyodre-0.0.1/python_interpreter.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pyodre-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pyodre-0.0.1/.idea/.name
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodre-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pyodre-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyodre-0.0.1/.idea/pyodre.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyodre-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 pyodre-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyodre-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyodre-0.0.1/LICENSE
--rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 pyodre-0.0.1/README.md
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pyodre-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    22832 2020-02-02 00:00:00.000000 pyodre-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pyodre-0.0.2/interpreters.py
+-rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 pyodre-0.0.2/pyodre.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 pyodre-0.0.2/python_functions.py
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 pyodre-0.0.2/python_interpreter.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pyodre-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pyodre-0.0.2/.idea/.name
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodre-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pyodre-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyodre-0.0.2/.idea/pyodre.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyodre-0.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 pyodre-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyodre-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyodre-0.0.2/LICENSE
+-rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 pyodre-0.0.2/README.md
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pyodre-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    22832 2020-02-02 00:00:00.000000 pyodre-0.0.2/PKG-INFO
```

### Comparing `pyodre-0.0.1/pyodre.py` & `pyodre-0.0.2/pyodre.py`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.1/python_functions.py` & `pyodre-0.0.2/python_functions.py`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.1/python_interpreter.py` & `pyodre-0.0.2/python_interpreter.py`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.1/.idea/workspace.xml` & `pyodre-0.0.2/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.1/LICENSE` & `pyodre-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.1/README.md` & `pyodre-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.1/pyproject.toml` & `pyodre-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["hatchling"]
 build-backend="hatchling.build"
 
 [project]
 name="pyodre"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "Andrea Cimmino", email="andreajesus.cimmino@upm.es"}
 ]
 description="Open Digital Rights Enforcement Framework python implementation"
 readme = "README.md"
 license = {file= "LICENSE"}
 requires-python = ">=3.9"
```

### Comparing `pyodre-0.0.1/PKG-INFO` & `pyodre-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyodre
-Version: 0.0.1
+Version: 0.0.2
 Summary: Open Digital Rights Enforcement Framework python implementation
 Project-URL: Homepage, https://github.com/ODRE-Framework/odre-python
 Project-URL: Bug Tracker, https://github.com/ODRE-Framework/odre-python/issues
 Author-email: Andrea Cimmino <andreajesus.cimmino@upm.es>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

