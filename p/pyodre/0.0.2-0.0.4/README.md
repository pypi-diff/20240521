# Comparing `tmp/pyodre-0.0.2.tar.gz` & `tmp/pyodre-0.0.4.tar.gz`

## Comparing `pyodre-0.0.2.tar` & `pyodre-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pyodre-0.0.2/interpreters.py
--rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 pyodre-0.0.2/pyodre.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 pyodre-0.0.2/python_functions.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 pyodre-0.0.2/python_interpreter.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pyodre-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pyodre-0.0.2/.idea/.name
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodre-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pyodre-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyodre-0.0.2/.idea/pyodre.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyodre-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 pyodre-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyodre-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyodre-0.0.2/LICENSE
--rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 pyodre-0.0.2/README.md
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pyodre-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    22832 2020-02-02 00:00:00.000000 pyodre-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pyodre-0.0.4/interpreters.py
+-rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 pyodre-0.0.4/pyodre.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 pyodre-0.0.4/python_functions.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 pyodre-0.0.4/python_interpreter.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pyodre-0.0.4/.idea/.gitignore
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pyodre-0.0.4/.idea/.name
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodre-0.0.4/.idea/misc.xml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pyodre-0.0.4/.idea/modules.xml
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyodre-0.0.4/.idea/pyodre.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyodre-0.0.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 pyodre-0.0.4/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyodre-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyodre-0.0.4/LICENSE
+-rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 pyodre-0.0.4/README.md
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 pyodre-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    22890 2020-02-02 00:00:00.000000 pyodre-0.0.4/PKG-INFO
```

### Comparing `pyodre-0.0.2/pyodre.py` & `pyodre-0.0.4/pyodre.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from rdflib import Graph, plugin
 from python_interpreter import PythonInterpreter
 from interpreters import Interpreter
 from jinja2 import Template
 
+
 class ODRE:
     def __init__(self, debug=False):
         self.__debug = debug
         self.__interpreter = PythonInterpreter()
 
     def set_interpreter(self, interpreter):
         if isinstance(interpreter, Interpreter):
@@ -28,26 +29,24 @@
               <http://www.w3.org/ns/odrl/2/permission> 
               <http://www.w3.org/ns/odrl/2/obligation> 
               <http://www.w3.org/ns/odrl/2/prohibition> 
             } .
         }"""
         return [str(row.rule_id.n3()) for row in graph.query(rules_query)]
 
-
     def _constraints(self, rule_id, graph):
         rules_query = """
             SELECT DISTINCT ?operator ?left_operand ?right_operand WHERE {
                   """ + rule_id + """ <http://www.w3.org/ns/odrl/2/operator>  ?operator;
                     <http://www.w3.org/ns/odrl/2/leftOperand> ?left_operand ;
                     <http://www.w3.org/ns/odrl/2/rightOperand> ?right_operand .
     
             }"""
         return [(str(row.operator), row.left_operand, row.right_operand) for row in graph.query(rules_query)]
 
-
     def _action(self, rule_id, graph):
         rules_query = """
         SELECT DISTINCT ?action WHERE {
             """ + rule_id + """ <http://www.w3.org/ns/odrl/2/action>  ?action . 
         }"""
         return [str(row.action) for row in graph.query(rules_query)][0]
 
@@ -100,12 +99,14 @@
            "operator": "eq",
            "rightOperand":  { "@value": "{{token}}", "@type": "xsd:string" }
        }]
    }]
 }
 """
 
+
 def get_token():
     return "AAA"
 
-usage_decision = ODRE().set_debug(True).enforce(policy, interpolations={'token' : 'AAA', 'retrieve_token' : get_token})
-print(usage_decision)
+
+usage_decision = ODRE().set_debug(True).enforce(policy, interpolations={'token': 'AAA', 'retrieve_token': get_token})
+print(usage_decision)
```

### Comparing `pyodre-0.0.2/python_functions.py` & `pyodre-0.0.4/python_functions.py`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.2/python_interpreter.py` & `pyodre-0.0.4/python_interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from interpreters import Interpreter
 import python_functions
-from python_functions import *
 from rdflib.term import Literal
 
 
 class PythonInterpreter(Interpreter):
 
     def __init__(self):
         self.__prefixes_mappings = {"odrl_": "http://www.w3.org/ns/odrl/2/",
```

### Comparing `pyodre-0.0.2/.idea/workspace.xml` & `pyodre-0.0.4/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.2/LICENSE` & `pyodre-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.2/README.md` & `pyodre-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.2/pyproject.toml` & `pyodre-0.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [build-system]
 requires=["hatchling"]
 build-backend="hatchling.build"
 
 [project]
 name="pyodre"
-version = "0.0.2"
+version = "0.0.4"
 authors = [
     { name = "Andrea Cimmino", email="andreajesus.cimmino@upm.es"}
 ]
+dependencies = [
+    "rdflib>=7.0.0",
+    "jinja2>=3.1.2"
+]
 description="Open Digital Rights Enforcement Framework python implementation"
 readme = "README.md"
 license = {file= "LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `pyodre-0.0.2/PKG-INFO` & `pyodre-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyodre
-Version: 0.0.2
+Version: 0.0.4
 Summary: Open Digital Rights Enforcement Framework python implementation
 Project-URL: Homepage, https://github.com/ODRE-Framework/odre-python
 Project-URL: Bug Tracker, https://github.com/ODRE-Framework/odre-python/issues
 Author-email: Andrea Cimmino <andreajesus.cimmino@upm.es>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -207,14 +207,16 @@
            See the License for the specific language governing permissions and
            limitations under the License.
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
+Requires-Dist: jinja2>=3.1.2
+Requires-Dist: rdflib>=7.0.0
 Description-Content-Type: text/markdown
 
 # ODRE Framework
 
 ## Quickstart
 To enforce an ODRL policy using the Python Interpreter
 ```python
```

