# Comparing `tmp/apiiif-0.2.0.tar.gz` & `tmp/apiiif-0.2.1.tar.gz`

## Comparing `apiiif-0.2.0.tar` & `apiiif-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.2.0/src/apiiif/__about__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.2.0/src/apiiif/__init__.py
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 apiiif-0.2.0/src/apiiif/factory.py
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 apiiif-0.2.0/src/apiiif/resource_properties.py
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 apiiif-0.2.0/src/apiiif/resource_types.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.2.0/.gitignore
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 apiiif-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.2.0/README.md
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 apiiif-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 apiiif-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.2.1/.vscode/settings.json
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.2.1/src/apiiif/__about__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.2.1/src/apiiif/__init__.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 apiiif-0.2.1/src/apiiif/factory.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 apiiif-0.2.1/src/apiiif/resource_properties.py
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 apiiif-0.2.1/src/apiiif/resource_types.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 apiiif-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.2.1/README.md
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 apiiif-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 apiiif-0.2.1/PKG-INFO
```

### Comparing `apiiif-0.2.0/src/apiiif/factory.py` & `apiiif-0.2.1/src/apiiif/factory.py`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.0/src/apiiif/resource_properties.py` & `apiiif-0.2.1/src/apiiif/resource_properties.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from multiprocessing import context
 from pydantic import BaseModel, AnyUrl, root_validator, validator, Field
-from pytest import fail
 
 
 class BaseID(BaseModel):
 
     @validator("id", pre=True)
     def slugify(s):
         if isinstance(s, str):
```

### Comparing `apiiif-0.2.0/src/apiiif/resource_types.py` & `apiiif-0.2.1/src/apiiif/resource_types.py`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.0/.gitignore` & `apiiif-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.0/LICENSE.txt` & `apiiif-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.0/README.md` & `apiiif-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.0/pyproject.toml` & `apiiif-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.0/PKG-INFO` & `apiiif-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiiif
-Version: 0.2.0
+Version: 0.2.1
 Project-URL: Documentation, https://github.com/d-flood/apiiif#readme
 Project-URL: Issues, https://github.com/d-flood/apiiif/issues
 Project-URL: Source, https://github.com/d-flood/apiiif
 Author-email: David Flood <d-flood@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

