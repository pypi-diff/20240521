# Comparing `tmp/apiiif-0.2.3.tar.gz` & `tmp/apiiif-0.2.4.tar.gz`

## Comparing `apiiif-0.2.3.tar` & `apiiif-0.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.2.3/.vscode/settings.json
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.2.3/src/apiiif/__about__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.2.3/src/apiiif/__init__.py
--rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 apiiif-0.2.3/src/apiiif/factory.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 apiiif-0.2.3/src/apiiif/resource_properties.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 apiiif-0.2.3/src/apiiif/resource_types.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.2.3/.gitignore
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 apiiif-0.2.3/LICENSE.txt
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.2.3/README.md
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 apiiif-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 apiiif-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.2.4/.vscode/settings.json
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.2.4/src/apiiif/__about__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.2.4/src/apiiif/__init__.py
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 apiiif-0.2.4/src/apiiif/factory.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 apiiif-0.2.4/src/apiiif/resource_properties.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 apiiif-0.2.4/src/apiiif/resource_types.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 apiiif-0.2.4/LICENSE.txt
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.2.4/README.md
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 apiiif-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 apiiif-0.2.4/PKG-INFO
```

### Comparing `apiiif-0.2.3/src/apiiif/factory.py` & `apiiif-0.2.4/src/apiiif/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,21 +135,21 @@
             width=width,
             height=height,
             service=[self.imageService(iiif_root_url, additional_services)],
         )
 
     def external_auth_service(
         self,
-        id: str,
+        _id: str,
         label: str,
         failure_header: str,
         failure_description: str,
     ):
         return ExternalAuthService(
-            id=id,
+            _id=_id,
             label=self.langugae_string(label),
             failureHeader=self.langugae_string(failure_header),
             failureDescription=self.langugae_string(failure_description),
         )
 
     def annotation_page(
         self,
```

### Comparing `apiiif-0.2.3/src/apiiif/resource_properties.py` & `apiiif-0.2.4/src/apiiif/resource_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 class Choice(BaseModel):
     type: str = "Choice"
     items: list = []
 
 
 class ExternalAuthService(BaseModel):
-    id: AnyUrl = Field(alias="@id")
+    _id: AnyUrl = Field(alias="@id")
     context: str = Field(
         default="http://iiif.io/api/auth/1/context.json", alias="@context"
     )
     profile: str = "http://iiif.io/api/auth/1/external"
     label: LanguageString
     failureHeader: LanguageString
     failureDescription: LanguageString
```

### Comparing `apiiif-0.2.3/src/apiiif/resource_types.py` & `apiiif-0.2.4/src/apiiif/resource_types.py`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.3/.gitignore` & `apiiif-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.3/LICENSE.txt` & `apiiif-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.3/README.md` & `apiiif-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.3/pyproject.toml` & `apiiif-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.3/PKG-INFO` & `apiiif-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiiif
-Version: 0.2.3
+Version: 0.2.4
 Project-URL: Documentation, https://github.com/d-flood/apiiif#readme
 Project-URL: Issues, https://github.com/d-flood/apiiif/issues
 Project-URL: Source, https://github.com/d-flood/apiiif
 Author-email: David Flood <d-flood@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

