# Comparing `tmp/data_snack_dynamic_entity-0.1.2.tar.gz` & `tmp/data_snack_dynamic_entity-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_snack_dynamic_entity-0.1.2.tar", last modified: Fri Apr  7 08:27:42 2023, max compression
+gzip compressed data, was "data_snack_dynamic_entity-0.2.0.tar", last modified: Tue May 21 08:59:43 2024, max compression
```

## Comparing `data_snack_dynamic_entity-0.1.2.tar` & `data_snack_dynamic_entity-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:27:42.567129 data_snack_dynamic_entity-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-07 08:27:25.000000 data_snack_dynamic_entity-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-07 08:27:25.000000 data_snack_dynamic_entity-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-07 08:27:42.567129 data_snack_dynamic_entity-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-07 08:27:25.000000 data_snack_dynamic_entity-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-07 08:27:25.000000 data_snack_dynamic_entity-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 08:27:25.000000 data_snack_dynamic_entity-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-07 08:27:42.567129 data_snack_dynamic_entity-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-07 08:27:25.000000 data_snack_dynamic_entity-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:27:42.563129 data_snack_dynamic_entity-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:27:42.567129 data_snack_dynamic_entity-0.1.2/src/data_snack_dynamic_entity/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-07 08:27:25.000000 data_snack_dynamic_entity-0.1.2/src/data_snack_dynamic_entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-07 08:27:25.000000 data_snack_dynamic_entity-0.1.2/src/data_snack_dynamic_entity/entityTemplates.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-07 08:27:25.000000 data_snack_dynamic_entity-0.1.2/src/data_snack_dynamic_entity/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-07 08:27:25.000000 data_snack_dynamic_entity-0.1.2/src/data_snack_dynamic_entity/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-07 08:27:25.000000 data_snack_dynamic_entity-0.1.2/src/data_snack_dynamic_entity/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:27:42.567129 data_snack_dynamic_entity-0.1.2/src/data_snack_dynamic_entity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-07 08:27:42.000000 data_snack_dynamic_entity-0.1.2/src/data_snack_dynamic_entity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-07 08:27:42.000000 data_snack_dynamic_entity-0.1.2/src/data_snack_dynamic_entity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 08:27:42.000000 data_snack_dynamic_entity-0.1.2/src/data_snack_dynamic_entity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-07 08:27:42.000000 data_snack_dynamic_entity-0.1.2/src/data_snack_dynamic_entity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-07 08:27:42.000000 data_snack_dynamic_entity-0.1.2/src/data_snack_dynamic_entity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:59:43.179689 data_snack_dynamic_entity-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-21 08:59:43.179689 data_snack_dynamic_entity-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-21 08:59:43.179689 data_snack_dynamic_entity-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:59:43.175689 data_snack_dynamic_entity-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:59:43.175689 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity/entityTemplates.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-21 08:59:38.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:59:43.179689 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-21 08:59:43.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-21 08:59:43.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:59:43.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 08:59:43.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 08:59:43.000000 data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity.egg-info/top_level.txt
```

### Comparing `data_snack_dynamic_entity-0.1.2/LICENSE` & `data_snack_dynamic_entity-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `data_snack_dynamic_entity-0.1.2/PKG-INFO` & `data_snack_dynamic_entity-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: data_snack_dynamic_entity
-Version: 0.1.2
+Version: 0.2.0
 Home-page: https://github.com/webinterpret-ds/data-snack-dynamic-entity
 Author: webinterpret-datascience
 Author-email: data-science@webinterpret.com
 Project-URL: Bug Tracker, https://github.com/webinterpret-ds/data-snack-dynamic-entity/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: data-snack>=1.0.3
+Requires-Dist: jsonschema>=4.17.3
 
 # Data Snack - Dynamic entity 
 
 # About
 Used to dynamically load `data-snack` `Entity` objects from json schema.
 Especially useful for complex dataset with many fields.
```

### Comparing `data_snack_dynamic_entity-0.1.2/README.md` & `data_snack_dynamic_entity-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `data_snack_dynamic_entity-0.1.2/setup.cfg` & `data_snack_dynamic_entity-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = data-snack-dynamic-entity
-version = 0.1.2
+version = 0.2.0
 author = webinterpret-datascience
 author_email = data-science@webinterpret.com
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/webinterpret-ds/data-snack-dynamic-entity
 project_urls =
```

### Comparing `data_snack_dynamic_entity-0.1.2/setup.py` & `data_snack_dynamic_entity-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `data_snack_dynamic_entity-0.1.2/src/data_snack_dynamic_entity/entityTemplates.schema.json` & `data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity/entityTemplates.schema.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333334%*

 * *Differences: {"'patternProperties'": "{'^[A-Z][a-zA-Z0-9]*$': {'properties': {'version': OrderedDict([('type', "*

 * *                        "'integer')])}, 'required': {insert: [(1, 'version')]}}}"}*

```diff
@@ -69,17 +69,21 @@
                                     },
                                     "type": "object"
                                 }
                             ]
                         }
                     },
                     "type": "object"
+                },
+                "version": {
+                    "type": "integer"
                 }
             },
             "required": [
-                "properties"
+                "properties",
+                "version"
             ],
             "type": "object"
         }
     },
     "type": "object"
 }
```

### Comparing `data_snack_dynamic_entity-0.1.2/src/data_snack_dynamic_entity/factory.py` & `data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity/factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 fields_with_defaults.append(
                     (field_name, field_type, field(default=field_schema["default"]))
                 )
             else:
                 fields.append((field_name, field_type))
 
         entity_template = self._create_entity_template(
-            entity_name=entity_name, keys=keys, excluded_fields=excluded_fields
+            entity_name=entity_name, keys=keys, excluded_fields=excluded_fields, version=entity_schema["version"]
         )
         return make_dataclass(
             entity_name,
             fields + fields_with_defaults,
             bases=(entity_template,),
             namespace={"__module__": __name__},
         )
@@ -74,24 +74,24 @@
         except AttributeError as e:
             if t := self.types_mapping.get(name):
                 return t
             raise ValueError(name) from e
 
     @staticmethod
     def _create_entity_template(
-        entity_name: str, keys: List[str], excluded_fields: List[str]
+        entity_name: str, keys: List[str], excluded_fields: List[str], version: int
     ) -> Type:
         return type(
             f"{entity_name}Template",
             (Entity,),
             {
                 "Meta": type(
                     "Meta",
                     (object,),
-                    {"keys": keys, "excluded_fields": excluded_fields},
+                    {"keys": keys, "excluded_fields": excluded_fields, "version": version},
                 )
             },
         )
 
 
 def load_entities(
     templates: EntityTemplates, types_mapping: Dict[str, Any] = None
```

### Comparing `data_snack_dynamic_entity-0.1.2/src/data_snack_dynamic_entity/validate.py` & `data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity/validate.py`

 * *Files identical despite different names*

### Comparing `data_snack_dynamic_entity-0.1.2/src/data_snack_dynamic_entity.egg-info/PKG-INFO` & `data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
-Name: data-snack-dynamic-entity
-Version: 0.1.2
+Name: data_snack_dynamic_entity
+Version: 0.2.0
 Home-page: https://github.com/webinterpret-ds/data-snack-dynamic-entity
 Author: webinterpret-datascience
 Author-email: data-science@webinterpret.com
 Project-URL: Bug Tracker, https://github.com/webinterpret-ds/data-snack-dynamic-entity/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: data-snack>=1.0.3
+Requires-Dist: jsonschema>=4.17.3
 
 # Data Snack - Dynamic entity 
 
 # About
 Used to dynamically load `data-snack` `Entity` objects from json schema.
 Especially useful for complex dataset with many fields.
```

### Comparing `data_snack_dynamic_entity-0.1.2/src/data_snack_dynamic_entity.egg-info/SOURCES.txt` & `data_snack_dynamic_entity-0.2.0/src/data_snack_dynamic_entity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

