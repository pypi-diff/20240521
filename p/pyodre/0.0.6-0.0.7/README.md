# Comparing `tmp/pyodre-0.0.6.tar.gz` & `tmp/pyodre-0.0.7.tar.gz`

## Comparing `pyodre-0.0.6.tar` & `pyodre-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pyodre-0.0.6/.idea/.gitignore
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pyodre-0.0.6/.idea/.name
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodre-0.0.6/.idea/misc.xml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pyodre-0.0.6/.idea/modules.xml
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyodre-0.0.6/.idea/pyodre.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyodre-0.0.6/.idea/vcs.xml
--rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 pyodre-0.0.6/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyodre-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodre-0.0.6/src/__init__.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pyodre-0.0.6/src/interpreters.py
--rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 pyodre-0.0.6/src/odre.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 pyodre-0.0.6/src/python_functions.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 pyodre-0.0.6/src/python_interpreter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodre-0.0.6/test/__init__.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyodre-0.0.6/LICENSE
--rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 pyodre-0.0.6/README.md
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pyodre-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    22890 2020-02-02 00:00:00.000000 pyodre-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pyodre-0.0.7/.idea/.gitignore
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pyodre-0.0.7/.idea/.name
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodre-0.0.7/.idea/misc.xml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pyodre-0.0.7/.idea/modules.xml
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyodre-0.0.7/.idea/pyodre.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyodre-0.0.7/.idea/vcs.xml
+-rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 pyodre-0.0.7/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyodre-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodre-0.0.7/src/__init__.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pyodre-0.0.7/src/interpreters.py
+-rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 pyodre-0.0.7/src/odre.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 pyodre-0.0.7/src/python_functions.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 pyodre-0.0.7/src/python_interpreter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodre-0.0.7/test/__init__.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyodre-0.0.7/LICENSE
+-rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 pyodre-0.0.7/README.md
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 pyodre-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    22890 2020-02-02 00:00:00.000000 pyodre-0.0.7/PKG-INFO
```

### Comparing `pyodre-0.0.6/.idea/workspace.xml` & `pyodre-0.0.7/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.6/src/odre.py` & `pyodre-0.0.7/src/odre.py`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.6/src/python_functions.py` & `pyodre-0.0.7/src/python_functions.py`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.6/src/python_interpreter.py` & `pyodre-0.0.7/src/python_interpreter.py`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.6/LICENSE` & `pyodre-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.6/README.md` & `pyodre-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.6/pyproject.toml` & `pyodre-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [build-system]
 requires=["hatchling"]
 build-backend="hatchling.build"
 
 [tool.hatch.build.targets.wheel]
-include = ["src/pyodre"]
+packages = ["src"]
+
+
 
 [project]
 name="pyodre"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "Andrea Cimmino", email="andreajesus.cimmino@upm.es"}
 ]
 dependencies = [
     "rdflib>=7.0.0",
     "jinja2>=3.1.2"
 ]
```

### Comparing `pyodre-0.0.6/PKG-INFO` & `pyodre-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyodre
-Version: 0.0.6
+Version: 0.0.7
 Summary: Open Digital Rights Enforcement Framework python implementation
 Project-URL: Homepage, https://github.com/ODRE-Framework/odre-python
 Project-URL: Bug Tracker, https://github.com/ODRE-Framework/odre-python/issues
 Author-email: Andrea Cimmino <andreajesus.cimmino@upm.es>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

