# Comparing `tmp/dj_component_view-8.0.tar.gz` & `tmp/dj_component_view-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_component_view-8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dj_component_view-9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dj_component_view-8.0.tar` & `dj_component_view-9.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3078 2024-04-29 05:31:20.582104 dj_component_view-8.0/.gitignore
--rw-r--r--   0        0        0     1086 2024-04-29 05:24:52.851465 dj_component_view-8.0/LICENSE
--rw-r--r--   0        0        0     1838 2024-05-04 02:42:09.140597 dj_component_view-8.0/README.md
--rw-r--r--   0        0        0     1981 2024-05-04 03:28:12.608004 dj_component_view-8.0/dj_component_view.py
--rw-r--r--   0        0        0      500 2024-05-04 03:28:21.168363 dj_component_view-8.0/pyproject.toml
--rw-r--r--   0        0        0     2210 1970-01-01 00:00:00.000000 dj_component_view-8.0/PKG-INFO
+-rw-r--r--   0        0        0     3078 2024-05-21 00:37:01.063042 dj_component_view-9.0/.gitignore
+-rw-r--r--   0        0        0     1086 2024-05-21 00:37:01.063196 dj_component_view-9.0/LICENSE
+-rw-r--r--   0        0        0     2329 2024-05-21 00:58:31.099710 dj_component_view-9.0/README.md
+-rw-r--r--   0        0        0     2561 2024-05-21 00:42:01.208310 dj_component_view-9.0/dj_component_view.py
+-rw-r--r--   0        0        0      500 2024-05-21 00:41:31.624963 dj_component_view-9.0/pyproject.toml
+-rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 dj_component_view-9.0/PKG-INFO
```

### Comparing `dj_component_view-8.0/.gitignore` & `dj_component_view-9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dj_component_view-8.0/LICENSE` & `dj_component_view-9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_component_view-8.0/dj_component_view.py` & `dj_component_view-9.0/dj_component_view.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from importlib import import_module
 from typing import Union
+from functools import wraps
 
 from django.conf import settings
 from django.http import HttpResponse, HttpResponseNotAllowed
 from django.views import View
 
 
 class ComponentView(View):
@@ -26,15 +27,15 @@
             raise ValueError("ComponentView subclasses must define a component.")
         return HttpResponse(str(catalog.render(self.component, **context)))
 
     def dispatch(self, request, *args, **kwargs):
         if request.method.lower() not in (method.lower() for method in self.methods):
             return HttpResponseNotAllowed(self.methods)
         return super().dispatch(request, *args, **kwargs)
-    
+
     def _base_get_post(self, request, *args, **kwargs):
         rendered = self.render(request)
 
         if isinstance(rendered, HttpResponse):
             return rendered
         elif rendered is None:
             rendered = {}
@@ -47,7 +48,27 @@
         return self._base_get_post(request, *args, **kwargs)
 
     def post(self, request, *args, **kwargs):
         return self._base_get_post(request, *args, **kwargs)
 
     def render(self, request) -> Union[dict, HttpResponse, None]:
         return {}
+
+
+def component(component_name, methods=["GET"]):
+    def decorator(func):
+        @wraps(func)
+        def wrapper(request, *args, **kwargs):
+            _methods = methods
+            class WrappedComponentView(ComponentView):
+                component = component_name
+                methods = _methods
+
+                def render(self, request):
+                    return func(request, *args, **kwargs)
+
+            view = WrappedComponentView.as_view()
+            return view(request, *args, **kwargs)
+
+        return wrapper
+
+    return decorator
```

