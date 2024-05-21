# Comparing `tmp/pyodre-0.0.5.tar.gz` & `tmp/pyodre-0.0.6.tar.gz`

## Comparing `pyodre-0.0.5.tar` & `pyodre-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pyodre-0.0.5/.idea/.gitignore
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pyodre-0.0.5/.idea/.name
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodre-0.0.5/.idea/misc.xml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pyodre-0.0.5/.idea/modules.xml
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyodre-0.0.5/.idea/pyodre.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyodre-0.0.5/.idea/vcs.xml
--rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 pyodre-0.0.5/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyodre-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodre-0.0.5/src/__init__.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pyodre-0.0.5/src/interpreters.py
--rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 pyodre-0.0.5/src/pyodre.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 pyodre-0.0.5/src/python_functions.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 pyodre-0.0.5/src/python_interpreter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodre-0.0.5/test/__init__.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyodre-0.0.5/LICENSE
--rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 pyodre-0.0.5/README.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyodre-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    22890 2020-02-02 00:00:00.000000 pyodre-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pyodre-0.0.6/.idea/.gitignore
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pyodre-0.0.6/.idea/.name
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodre-0.0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pyodre-0.0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyodre-0.0.6/.idea/pyodre.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyodre-0.0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 pyodre-0.0.6/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyodre-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodre-0.0.6/src/__init__.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pyodre-0.0.6/src/interpreters.py
+-rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 pyodre-0.0.6/src/odre.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 pyodre-0.0.6/src/python_functions.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 pyodre-0.0.6/src/python_interpreter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodre-0.0.6/test/__init__.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyodre-0.0.6/LICENSE
+-rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 pyodre-0.0.6/README.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pyodre-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    22890 2020-02-02 00:00:00.000000 pyodre-0.0.6/PKG-INFO
```

### Comparing `pyodre-0.0.5/.idea/workspace.xml` & `pyodre-0.0.6/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.5/src/pyodre.py` & `pyodre-0.0.6/src/odre.py`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.5/src/python_functions.py` & `pyodre-0.0.6/src/python_functions.py`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.5/src/python_interpreter.py` & `pyodre-0.0.6/src/python_interpreter.py`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.5/LICENSE` & `pyodre-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.5/README.md` & `pyodre-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.5/pyproject.toml` & `pyodre-0.0.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
 requires=["hatchling"]
 build-backend="hatchling.build"
 
+[tool.hatch.build.targets.wheel]
+include = ["src/pyodre"]
+
 [project]
 name="pyodre"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name = "Andrea Cimmino", email="andreajesus.cimmino@upm.es"}
 ]
 dependencies = [
     "rdflib>=7.0.0",
     "jinja2>=3.1.2"
 ]
@@ -24,9 +27,7 @@
 
 [project.urls]
 "Homepage" = "https://github.com/ODRE-Framework/odre-python"
 "Bug Tracker" = "https://github.com/ODRE-Framework/odre-python/issues"
 
 
 
-[tool.hatch.build.targets.wheel]
-include = ["src/pyodre"]
```

### Comparing `pyodre-0.0.5/PKG-INFO` & `pyodre-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyodre
-Version: 0.0.5
+Version: 0.0.6
 Summary: Open Digital Rights Enforcement Framework python implementation
 Project-URL: Homepage, https://github.com/ODRE-Framework/odre-python
 Project-URL: Bug Tracker, https://github.com/ODRE-Framework/odre-python/issues
 Author-email: Andrea Cimmino <andreajesus.cimmino@upm.es>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

