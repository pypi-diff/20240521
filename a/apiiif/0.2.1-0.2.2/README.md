# Comparing `tmp/apiiif-0.2.1.tar.gz` & `tmp/apiiif-0.2.2.tar.gz`

## Comparing `apiiif-0.2.1.tar` & `apiiif-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.2.1/.vscode/settings.json
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.2.1/src/apiiif/__about__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.2.1/src/apiiif/__init__.py
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 apiiif-0.2.1/src/apiiif/factory.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 apiiif-0.2.1/src/apiiif/resource_properties.py
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 apiiif-0.2.1/src/apiiif/resource_types.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.2.1/.gitignore
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 apiiif-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.2.1/README.md
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 apiiif-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 apiiif-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.2.2/src/apiiif/__about__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.2.2/src/apiiif/__init__.py
+-rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 apiiif-0.2.2/src/apiiif/factory.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 apiiif-0.2.2/src/apiiif/resource_properties.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 apiiif-0.2.2/src/apiiif/resource_types.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 apiiif-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.2.2/README.md
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 apiiif-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 apiiif-0.2.2/PKG-INFO
```

### Comparing `apiiif-0.2.1/src/apiiif/factory.py` & `apiiif-0.2.2/src/apiiif/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,16 +57,18 @@
             homepage=[homepage],
             logo=[self.logo(url, 100, 100)],
         )
 
     def choice(self, items: list):
         return Choice(items=items)
 
-    def imageService(self, url: str):
-        return ImageService(id=url)
+    def imageService(
+        self, url: str, additional_services: list[ExternalAuthService] = []
+    ):
+        return ImageService(id=url, service=additional_services)
 
     def collection(
         self, url: str, label: str, attribution_label: str, attribution_value: str
     ):
         return Collection(
             id=url,
             label=self.langugae_string(label),
@@ -122,23 +124,21 @@
 
     def IIIF_image(
         self,
         thumbnail_url: str,
         iiif_root_url: str,
         width: int,
         height: int,
-        additional_services: list[ImageService | ExternalAuthService] = [],
+        additional_services: list[ExternalAuthService] = [],
     ):
-        services = [self.imageService(iiif_root_url)]
-        services.extend(additional_services)
         return IIIFImage(
             id=thumbnail_url,
             width=width,
             height=height,
-            service=services,
+            service=[self.imageService(iiif_root_url, additional_services)],
         )
 
     def external_auth_service(
         self,
         label: str,
         failure_header: str,
         failure_description: str,
```

### Comparing `apiiif-0.2.1/src/apiiif/resource_properties.py` & `apiiif-0.2.2/src/apiiif/resource_properties.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,20 +72,22 @@
 
 
 class Choice(BaseModel):
     type: str = "Choice"
     items: list = []
 
 
-class ImageService(BaseID):
-    type: str = "ImageService3"
-    profile: str = "level0"
-
-
 class ExternalAuthService(BaseModel):
+    id: AnyUrl = Field(alias="@id")
     context: str = Field(
         default="http://iiif.io/api/auth/1/context.json", alias="@context"
     )
     profile: str = "http://iiif.io/api/auth/1/external"
     label: LanguageString
     failureHeader: LanguageString
     failureDescription: LanguageString
+
+
+class ImageService(BaseID):
+    type: str = "ImageService3"
+    profile: str = "level0"
+    service: list[ExternalAuthService] = []
```

### Comparing `apiiif-0.2.1/src/apiiif/resource_types.py` & `apiiif-0.2.2/src/apiiif/resource_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     BaseID,
 )
 
 
 class IIIFImage(Image):
     format: str = "image/jpeg"
     # as other services are defined, add them as options.
-    service: list[ImageService | ExternalAuthService] = []
+    service: list[ImageService] = []
 
 
 class Annotation(BaseID):
     context: str = Field(
         default="http://iiif.io/api/presentation/3/context.json", alias="@context"
     )
     type: str = "Annotation"
@@ -81,14 +81,15 @@
     behavior: list[str] = ["paged"]
     rights: AnyUrl | str | None
     requiredStatement: LabelValue | None
     provider: list[Provider] | None
     homepage: Homepage | None
     partOf: PartOf | None
     items: list = []
+    services: list[ExternalAuthService] = []
 
     def add_canvas(self, canvas: Canvas):
         self.items.append(canvas)
 
 
 class Collection(BaseID):
     context: str = Field(
```

### Comparing `apiiif-0.2.1/.gitignore` & `apiiif-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.1/LICENSE.txt` & `apiiif-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.1/README.md` & `apiiif-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.1/pyproject.toml` & `apiiif-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.1/PKG-INFO` & `apiiif-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiiif
-Version: 0.2.1
+Version: 0.2.2
 Project-URL: Documentation, https://github.com/d-flood/apiiif#readme
 Project-URL: Issues, https://github.com/d-flood/apiiif/issues
 Project-URL: Source, https://github.com/d-flood/apiiif
 Author-email: David Flood <d-flood@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

