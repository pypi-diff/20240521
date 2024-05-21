# Comparing `tmp/miska-0.0.2.tar.gz` & `tmp/miska-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miska-0.0.2.tar", last modified: Fri May 17 18:14:48 2024, max compression
+gzip compressed data, was "miska-0.0.3.tar", last modified: Tue May 21 08:59:23 2024, max compression
```

## Comparing `miska-0.0.2.tar` & `miska-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-17 18:14:48.355019 miska-0.0.2/
--rw-r--r--   0 cell      (1000) cell      (1000)     1289 2024-03-09 16:24:22.000000 miska-0.0.2/LICENSE
--rw-r--r--   0 cell      (1000) cell      (1000)     2853 2024-05-17 18:14:48.354019 miska-0.0.2/PKG-INFO
--rw-r--r--   0 cell      (1000) cell      (1000)      578 2024-03-09 16:24:22.000000 miska-0.0.2/README.rst
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-17 18:14:48.346019 miska-0.0.2/miska/
--rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.2/miska/__init__.py
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-17 18:14:48.351019 miska-0.0.2/miska/http/
--rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.2/miska/http/__init__.py
--rw-r--r--   0 cell      (1000) cell      (1000)     1395 2024-03-09 16:24:22.000000 miska-0.0.2/miska/http/rs.py
--rw-r--r--   0 cell      (1000) cell      (1000)      222 2024-03-09 16:24:22.000000 miska-0.0.2/miska/mixins.py
--rw-r--r--   0 cell      (1000) cell      (1000)     1531 2024-05-17 13:52:44.000000 miska-0.0.2/miska/registries.py
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-17 18:14:48.351019 miska-0.0.2/miska/types/
--rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.2/miska/types/__init__.py
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-17 18:14:48.352019 miska-0.0.2/miska/types/network/
--rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.2/miska/types/network/__init__.py
--rw-r--r--   0 cell      (1000) cell      (1000)     3206 2024-03-09 16:24:22.000000 miska-0.0.2/miska/types/network/bgp.py
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-17 18:14:48.353019 miska-0.0.2/miska.egg-info/
--rw-r--r--   0 cell      (1000) cell      (1000)     2853 2024-05-17 18:14:48.000000 miska-0.0.2/miska.egg-info/PKG-INFO
--rw-r--r--   0 cell      (1000) cell      (1000)      379 2024-05-17 18:14:48.000000 miska-0.0.2/miska.egg-info/SOURCES.txt
--rw-r--r--   0 cell      (1000) cell      (1000)        1 2024-05-17 18:14:48.000000 miska-0.0.2/miska.egg-info/dependency_links.txt
--rw-r--r--   0 cell      (1000) cell      (1000)       36 2024-05-17 18:14:48.000000 miska-0.0.2/miska.egg-info/requires.txt
--rw-r--r--   0 cell      (1000) cell      (1000)        6 2024-05-17 18:14:48.000000 miska-0.0.2/miska.egg-info/top_level.txt
--rw-r--r--   0 cell      (1000) cell      (1000)      843 2024-05-17 18:11:31.000000 miska-0.0.2/pyproject.toml
--rw-r--r--   0 cell      (1000) cell      (1000)       38 2024-05-17 18:14:48.355019 miska-0.0.2/setup.cfg
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-17 18:14:48.353019 miska-0.0.2/tests/
--rw-r--r--   0 cell      (1000) cell      (1000)      275 2024-05-17 18:10:11.000000 miska-0.0.2/tests/test_registries.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-21 08:59:23.175150 miska-0.0.3/
+-rw-r--r--   0 cell      (1000) cell      (1000)     1289 2024-03-09 16:24:22.000000 miska-0.0.3/LICENSE
+-rw-r--r--   0 cell      (1000) cell      (1000)     2853 2024-05-21 08:59:23.174150 miska-0.0.3/PKG-INFO
+-rw-r--r--   0 cell      (1000) cell      (1000)      578 2024-03-09 16:24:22.000000 miska-0.0.3/README.rst
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-21 08:59:23.169150 miska-0.0.3/miska/
+-rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.3/miska/__init__.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-21 08:59:23.171150 miska-0.0.3/miska/http/
+-rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.3/miska/http/__init__.py
+-rw-r--r--   0 cell      (1000) cell      (1000)     1395 2024-03-09 16:24:22.000000 miska-0.0.3/miska/http/rs.py
+-rw-r--r--   0 cell      (1000) cell      (1000)      222 2024-03-09 16:24:22.000000 miska-0.0.3/miska/mixins.py
+-rw-r--r--   0 cell      (1000) cell      (1000)     1828 2024-05-21 08:55:25.000000 miska-0.0.3/miska/registries.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-21 08:59:23.172150 miska-0.0.3/miska/types/
+-rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.3/miska/types/__init__.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-21 08:59:23.173150 miska-0.0.3/miska/types/network/
+-rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.3/miska/types/network/__init__.py
+-rw-r--r--   0 cell      (1000) cell      (1000)     3206 2024-03-09 16:24:22.000000 miska-0.0.3/miska/types/network/bgp.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-21 08:59:23.173150 miska-0.0.3/miska.egg-info/
+-rw-r--r--   0 cell      (1000) cell      (1000)     2853 2024-05-21 08:59:23.000000 miska-0.0.3/miska.egg-info/PKG-INFO
+-rw-r--r--   0 cell      (1000) cell      (1000)      379 2024-05-21 08:59:23.000000 miska-0.0.3/miska.egg-info/SOURCES.txt
+-rw-r--r--   0 cell      (1000) cell      (1000)        1 2024-05-21 08:59:23.000000 miska-0.0.3/miska.egg-info/dependency_links.txt
+-rw-r--r--   0 cell      (1000) cell      (1000)       36 2024-05-21 08:59:23.000000 miska-0.0.3/miska.egg-info/requires.txt
+-rw-r--r--   0 cell      (1000) cell      (1000)        6 2024-05-21 08:59:23.000000 miska-0.0.3/miska.egg-info/top_level.txt
+-rw-r--r--   0 cell      (1000) cell      (1000)      843 2024-05-21 08:57:50.000000 miska-0.0.3/pyproject.toml
+-rw-r--r--   0 cell      (1000) cell      (1000)       38 2024-05-21 08:59:23.175150 miska-0.0.3/setup.cfg
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-21 08:59:23.173150 miska-0.0.3/tests/
+-rw-r--r--   0 cell      (1000) cell      (1000)      275 2024-05-21 08:54:48.000000 miska-0.0.3/tests/test_registries.py
```

### Comparing `miska-0.0.2/LICENSE` & `miska-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `miska-0.0.2/PKG-INFO` & `miska-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miska
-Version: 0.0.2
+Version: 0.0.3
 Summary: An exceptional library
 Author-email: Dima Burmistrov <pyctrl.dev@gmail.com>
 License: Copyright (c) 2023-2024 Dmitry Burmistrov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `miska-0.0.2/README.rst` & `miska-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `miska-0.0.2/miska/http/rs.py` & `miska-0.0.3/miska/http/rs.py`

 * *Files identical despite different names*

### Comparing `miska-0.0.2/miska/registries.py` & `miska-0.0.3/miska/registries.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import types
 import typing as t
 
 
 class BaseRegistryError(Exception):
     pass
 
 
@@ -13,49 +14,55 @@
     pass
 
 
 class ChildNotFound(BaseRegistryError):
     pass
 
 
-class RegistriesMixin:
+class ClassRegistriesMixin:
 
     __registries: dict[str, dict[t.Any, type]] = {}
 
     __registry_type__: str  # default: class name
-    __registry_locator__: str
+    __registry_locator__: str | t.Callable[[t.Type], str]
 
     @classmethod
     def __get_type(cls):
         return getattr(cls, "__registry_type__", cls.__name__)
 
     @classmethod
     def __get_loc(cls):
         loc = getattr(cls, "__registry_locator__", None)
         if loc is None:
             raise ChildMissingLocator(cls)
         return loc
 
     @classmethod
     def __get_loc_val(cls):
-        value = getattr(cls, cls.__get_loc(), None)
+        loc = cls.__get_loc()
+        value = getattr(cls, loc, None) if isinstance(loc, str) else loc(cls)
         if value is None:
             raise ChildMissingLocatorValue(cls)
         return value
 
     def __init_subclass__(cls, **kwargs: t.Any):
         super().__init_subclass__(**kwargs)
-        mixin = RegistriesMixin
+        mixin = ClassRegistriesMixin
 
         if mixin in cls.__bases__:
             cls.__registry_type__ = cls.__get_type()  # enrich
             cls.__get_loc()  # validation
         else:
             store = mixin.__registries.setdefault(cls.__get_type(), {})
             store[cls.__get_loc_val()] = cls
 
     @classmethod
     def get_child_for(cls, locator_value: t.Any) -> type:
         store = cls.__registries[cls.__registry_type__]
         if locator_value not in store:
             raise ChildNotFound(locator_value)
         return store[locator_value]
+
+    @classmethod
+    def get_children(cls) -> types.MappingProxyType[str, type]:
+        store = cls.__registries[cls.__registry_type__]
+        return types.MappingProxyType(store.copy())
```

### Comparing `miska-0.0.2/miska/types/network/bgp.py` & `miska-0.0.3/miska/types/network/bgp.py`

 * *Files identical despite different names*

### Comparing `miska-0.0.2/miska.egg-info/PKG-INFO` & `miska-0.0.3/miska.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miska
-Version: 0.0.2
+Version: 0.0.3
 Summary: An exceptional library
 Author-email: Dima Burmistrov <pyctrl.dev@gmail.com>
 License: Copyright (c) 2023-2024 Dmitry Burmistrov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `miska-0.0.2/pyproject.toml` & `miska-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "miska"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Dima Burmistrov", email="pyctrl.dev@gmail.com" },
 ]
 description = "An exceptional library"
 readme = "README.rst"
 license = {file = "LICENSE"}
```

