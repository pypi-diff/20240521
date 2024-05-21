# Comparing `tmp/apiiif-0.2.2.tar.gz` & `tmp/apiiif-0.2.3.tar.gz`

## Comparing `apiiif-0.2.2.tar` & `apiiif-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.2.2/.vscode/settings.json
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.2.2/src/apiiif/__about__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.2.2/src/apiiif/__init__.py
--rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 apiiif-0.2.2/src/apiiif/factory.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 apiiif-0.2.2/src/apiiif/resource_properties.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 apiiif-0.2.2/src/apiiif/resource_types.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.2.2/.gitignore
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 apiiif-0.2.2/LICENSE.txt
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.2.2/README.md
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 apiiif-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 apiiif-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.2.3/.vscode/settings.json
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.2.3/src/apiiif/__about__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.2.3/src/apiiif/__init__.py
+-rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 apiiif-0.2.3/src/apiiif/factory.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 apiiif-0.2.3/src/apiiif/resource_properties.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 apiiif-0.2.3/src/apiiif/resource_types.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 apiiif-0.2.3/LICENSE.txt
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.2.3/README.md
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 apiiif-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 apiiif-0.2.3/PKG-INFO
```

### Comparing `apiiif-0.2.2/src/apiiif/factory.py` & `apiiif-0.2.3/src/apiiif/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,19 +135,21 @@
             width=width,
             height=height,
             service=[self.imageService(iiif_root_url, additional_services)],
         )
 
     def external_auth_service(
         self,
+        id: str,
         label: str,
         failure_header: str,
         failure_description: str,
     ):
         return ExternalAuthService(
+            id=id,
             label=self.langugae_string(label),
             failureHeader=self.langugae_string(failure_header),
             failureDescription=self.langugae_string(failure_description),
         )
 
     def annotation_page(
         self,
```

### Comparing `apiiif-0.2.2/src/apiiif/resource_properties.py` & `apiiif-0.2.3/src/apiiif/resource_properties.py`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.2/src/apiiif/resource_types.py` & `apiiif-0.2.3/src/apiiif/resource_types.py`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.2/.gitignore` & `apiiif-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.2/LICENSE.txt` & `apiiif-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.2/README.md` & `apiiif-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.2/pyproject.toml` & `apiiif-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.2/PKG-INFO` & `apiiif-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiiif
-Version: 0.2.2
+Version: 0.2.3
 Project-URL: Documentation, https://github.com/d-flood/apiiif#readme
 Project-URL: Issues, https://github.com/d-flood/apiiif/issues
 Project-URL: Source, https://github.com/d-flood/apiiif
 Author-email: David Flood <d-flood@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

