# Comparing `tmp/permission_manager_drf-0.2.0.tar.gz` & `tmp/permission_manager_drf-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permission_manager_drf-0.2.0.tar", max compression
+gzip compressed data, was "permission_manager_drf-0.2.1.tar", max compression
```

## Comparing `permission_manager_drf-0.2.0.tar` & `permission_manager_drf-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1075 2024-05-15 23:05:23.553639 permission_manager_drf-0.2.0/LICENSE
--rw-r--r--   0        0        0     2229 2024-05-15 23:05:23.553639 permission_manager_drf-0.2.0/README.md
--rw-r--r--   0        0        0      264 2024-05-15 23:05:23.553639 permission_manager_drf-0.2.0/permission_manager_drf/__init__.py
--rw-r--r--   0        0        0     1793 2024-05-15 23:05:23.553639 permission_manager_drf-0.2.0/permission_manager_drf/fields.py
--rw-r--r--   0        0        0     1149 2024-05-15 23:05:23.553639 permission_manager_drf-0.2.0/permission_manager_drf/managers.py
--rw-r--r--   0        0        0      811 2024-05-15 23:05:23.553639 permission_manager_drf-0.2.0/permission_manager_drf/pagination.py
--rw-r--r--   0        0        0     1629 2024-05-15 23:05:23.553639 permission_manager_drf-0.2.0/permission_manager_drf/permissions.py
--rw-r--r--   0        0        0      369 2024-05-15 23:05:23.553639 permission_manager_drf-0.2.0/permission_manager_drf/settings.py
--rw-r--r--   0        0        0     1629 2024-05-15 23:05:23.553639 permission_manager_drf-0.2.0/permission_manager_drf/utils.py
--rw-r--r--   0        0        0     2413 2024-05-15 23:05:23.553639 permission_manager_drf-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3112 1970-01-01 00:00:00.000000 permission_manager_drf-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2499 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/README.md
+-rw-r--r--   0        0        0      264 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/permission_manager_drf/__init__.py
+-rw-r--r--   0        0        0     3833 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/permission_manager_drf/fields.py
+-rw-r--r--   0        0        0     2607 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/permission_manager_drf/managers.py
+-rw-r--r--   0        0        0     1610 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/permission_manager_drf/pagination.py
+-rw-r--r--   0        0        0     3058 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/permission_manager_drf/permissions.py
+-rw-r--r--   0        0        0      503 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/permission_manager_drf/settings.py
+-rw-r--r--   0        0        0     2150 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/permission_manager_drf/utils.py
+-rw-r--r--   0        0        0     2471 2024-05-21 08:33:53.960086 permission_manager_drf-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3382 1970-01-01 00:00:00.000000 permission_manager_drf-0.2.1/PKG-INFO
```

### Comparing `permission_manager_drf-0.2.0/LICENSE` & `permission_manager_drf-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `permission_manager_drf-0.2.0/README.md` & `permission_manager_drf-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Permission Manager for django rest framework
 
+![example workflow](https://github.com/kindlycat/permission-manager-drf/actions/workflows/tests.yml/badge.svg)
+[![codecov](https://codecov.io/gh/kindlycat/permission-manager-drf/graph/badge.svg?token=5XAFJZS6A8)](https://codecov.io/gh/kindlycat/permission-manager-drf)
+
 Use [permission_manager](https://github.com/kindlycat/permission-manager) for 
 django rest framework.
 
 Full documentation on [read the docs](https://permission-manager-drf.readthedocs.io/).
 
 ## Install
```

### Comparing `permission_manager_drf-0.2.0/permission_manager_drf/permissions.py` & `permission_manager_drf-0.2.1/permission_manager_drf/permissions.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,46 +5,90 @@
 from rest_framework.request import Request
 from rest_framework.viewsets import GenericViewSet
 
 from permission_manager_drf.utils import get_permission_manager
 
 
 class ManagerPermission(BasePermission):
-    """DRF Permission class for a permission manager."""
+    """DRF Permission class for a permission manager.
+
+    This class integrates with a permission manager to handle permissions
+    for DRF views and objects.
+
+    Attributes:
+        default_detail_actions (ClassVar[tuple]): Default actions considered
+            as detail actions.
+    """
 
     default_detail_actions: ClassVar[tuple] = ('retrieve', 'destroy', 'update')
 
     def is_detail(self, view: GenericViewSet, action_name: str) -> bool:
-        """Check if action is detail."""
+        """Check if the action is a detail action.
+
+        Args:
+            view (GenericViewSet): The view being accessed.
+            action_name (str): The name of the action.
+
+        Returns:
+            bool: True if the action is a detail action, False otherwise.
+        """
         if action_name in self.default_detail_actions:
             return True
 
         action = getattr(view, action_name)
         return getattr(action, 'detail', False)
 
     def _has_perm(self, view: GenericViewSet, obj: Model = None) -> bool:
+        """Check if the permission is granted for the action.
+
+        Args:
+            view (GenericViewSet): The view being accessed.
+            obj (Model, optional): The object being accessed.
+
+        Returns:
+            bool: True if the permission is granted, False otherwise.
+        """
         action_name = view.action
 
-        # Let drf decide what to do if view hasn't action
+        # Let DRF decide what to do if view hasn't action
         if not action_name:
             return True
 
         # Resolve partial_update action like update action
         if action_name == 'partial_update':
             action_name = 'update'
 
         if not obj and self.is_detail(view=view, action_name=action_name):
             return True
 
         manager = get_permission_manager(view=view, instance=obj)
         return manager.has_permission(action_name)
 
     def has_permission(self, request: Request, view: GenericViewSet) -> bool:
+        """Check if the request has permission to access the view.
+
+        Args:
+            request (Request): The request being made.
+            view (GenericViewSet): The view being accessed.
+
+        Returns:
+            bool: True if the request has permission, False otherwise.
+        """
         return self._has_perm(view=view)
 
     def has_object_permission(
         self,
         request: Request,
         view: GenericViewSet,
         obj: Model,
     ) -> bool:
+        """Check if the request has permission to access the object.
+
+        Args:
+            request (Request): The request being made.
+            view (GenericViewSet): The view being accessed.
+            obj (Model): The object being accessed.
+
+        Returns:
+            bool: True if the request has permission, False otherwise.
+        """
         return self._has_perm(view=view, obj=obj)
```

### Comparing `permission_manager_drf-0.2.0/pyproject.toml` & `permission_manager_drf-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "permission-manager-drf"
-version = "0.2.0"
+version = "0.2.1"
 description = "A simple way to manage object permissions in drf."
 authors = ["Grigory Mishchenko <grishkokot@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "permission_manager_drf"}]
 repository = "https://github.com/kindlycat/permission-manager-drf"
 keywords = ["permissions", "drf", "rest framework"]
@@ -15,16 +15,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-djangorestframework = "^3.15.1"
-permission-manager = "^0.4.1"
+djangorestframework = "^3.14.0"
+permission-manager = "^0.4.2"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.24"
 ipdb = "^0.13.13"
 pytest = "^8.1.2"
 ruff = "^0.4.2"
 pytest-django = "^4.8.0"
@@ -104,8 +104,11 @@
 line-ending = "auto"
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
-addopts = "-ra -s"
+addopts = "-ra -v"
+
+[tool.coverage.run]
+source = ["permission_manager_drf"]
```

### Comparing `permission_manager_drf-0.2.0/PKG-INFO` & `permission_manager_drf-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: permission-manager-drf
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple way to manage object permissions in drf.
 Home-page: https://github.com/kindlycat/permission-manager-drf
 License: MIT
 Keywords: permissions,drf,rest framework
 Author: Grigory Mishchenko
 Author-email: grishkokot@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: djangorestframework (>=3.15.1,<4.0.0)
-Requires-Dist: permission-manager (>=0.4.1,<0.5.0)
+Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
+Requires-Dist: permission-manager (>=0.4.2,<0.5.0)
 Project-URL: Repository, https://github.com/kindlycat/permission-manager-drf
 Description-Content-Type: text/markdown
 
 # Permission Manager for django rest framework
 
+![example workflow](https://github.com/kindlycat/permission-manager-drf/actions/workflows/tests.yml/badge.svg)
+[![codecov](https://codecov.io/gh/kindlycat/permission-manager-drf/graph/badge.svg?token=5XAFJZS6A8)](https://codecov.io/gh/kindlycat/permission-manager-drf)
+
 Use [permission_manager](https://github.com/kindlycat/permission-manager) for 
 django rest framework.
 
 Full documentation on [read the docs](https://permission-manager-drf.readthedocs.io/).
 
 ## Install
```

