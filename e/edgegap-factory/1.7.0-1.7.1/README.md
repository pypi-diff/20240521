# Comparing `tmp/edgegap_factory-1.7.0.tar.gz` & `tmp/edgegap_factory-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_factory-1.7.0.tar", max compression
+gzip compressed data, was "edgegap_factory-1.7.1.tar", max compression
```

## Comparing `edgegap_factory-1.7.0.tar` & `edgegap_factory-1.7.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0        0 2024-05-06 18:04:44.781040 edgegap_factory-1.7.0/README.md
--rw-r--r--   0        0        0       17 2024-05-06 18:04:44.781156 edgegap_factory-1.7.0/edgegap_factory/BUILD
--rw-r--r--   0        0        0      144 2024-05-06 18:04:44.781340 edgegap_factory-1.7.0/edgegap_factory/__init__.py
--rw-r--r--   0        0        0      173 2024-05-06 18:04:44.781534 edgegap_factory-1.7.0/edgegap_factory/_base_factory.py
--rw-r--r--   0        0        0     1490 2024-05-06 18:04:44.781738 edgegap_factory-1.7.0/edgegap_factory/_generator.py
--rw-r--r--   0        0        0     3614 2024-05-06 20:32:49.188993 edgegap_factory-1.7.0/edgegap_factory/_sql_model_factory.py
--rw-r--r--   0        0        0      366 2024-05-07 13:27:32.204185 edgegap_factory-1.7.0/pyproject.toml
--rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 edgegap_factory-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-09 20:06:47.236991 edgegap_factory-1.7.1/README.md
+-rw-r--r--   0        0        0      144 2024-05-09 20:06:47.237292 edgegap_factory-1.7.1/edgegap_factory/__init__.py
+-rw-r--r--   0        0        0      173 2024-05-09 20:06:47.237464 edgegap_factory-1.7.1/edgegap_factory/_base_factory.py
+-rw-r--r--   0        0        0     1490 2024-05-09 20:06:47.237648 edgegap_factory-1.7.1/edgegap_factory/_generator.py
+-rw-r--r--   0        0        0     3613 2024-05-21 18:49:40.479758 edgegap_factory-1.7.1/edgegap_factory/_sql_model_factory.py
+-rw-r--r--   0        0        0      511 2024-05-21 18:50:20.985768 edgegap_factory-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 edgegap_factory-1.7.1/PKG-INFO
```

### Comparing `edgegap_factory-1.7.0/edgegap_factory/_generator.py` & `edgegap_factory-1.7.1/edgegap_factory/_generator.py`

 * *Files identical despite different names*

### Comparing `edgegap_factory-1.7.0/edgegap_factory/_sql_model_factory.py` & `edgegap_factory-1.7.1/edgegap_factory/_sql_model_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,39 +19,37 @@
         float: generator.FloatGenerator(),
         datetime.datetime: generator.DatetimeGenerator(),
         bool: generator.BooleanGenerator(),
         None: generator.NoneGenerator(),
         dict: generator.DictGenerator(),
     }
 
-    def __init__(self, session: Session, *, auto_commit: bool):
+    def __init__(self, session: Session | None, *, auto_commit: bool):
         self.__session = session
         self.__auto_commit = auto_commit
 
     def create(self, model: T):
         return self.__create(model, self.__auto_commit)
 
     def __create(self, model: T, commit: bool) -> T:
         inspected_model = inspect(model.__class__)
         relations = inspected_model.relationships.items()
         columns = list(inspected_model.columns)
         model = self.__create_relation(model, relations)
         model = self.__create_columns(model, columns)
 
-        self.__session.add(model)
+        if self.__session is not None:
+            self.__session.add(model)
 
-        if commit:
+        if self.__session is not None and commit:
             self.__session.commit()
 
         return model
 
-    def __create_relation(self, model: T, relations) -> T:  # TODO: typing
-        """
-        TODO Max: comment
-        """
+    def __create_relation(self, model: T, relations) -> T:
         for relation_name, relation_property in filter(lambda v: not v[1].uselist, relations):
             local_column = [c for c in relation_property.local_columns][0]
 
             should_create = all(
                 [
                     not local_column.nullable,
                     getattr(model, local_column.name) is None,
@@ -61,15 +59,15 @@
             if should_create:
                 base_model = getattr(model, relation_name) or relation_property.mapper.class_()
                 constructed_model = self.__create(base_model, commit=False)
                 setattr(model, relation_name, constructed_model)
 
         return model
 
-    def __create_columns(self, model: T, columns) -> T:  # TODO: typing
+    def __create_columns(self, model: T, columns) -> T:
         for column in columns:
             if not column.nullable and getattr(model, column.name) is None:
                 # This column type hack is needed because of the way TypeDecorator are designed in SqlAlchemy.
                 # E.G. AutoString form SqlModel is a SqlAlchemy String however it does not inherit from it. It inherits
                 # from TypeDecorator. This is why we need to check if the column type is a TypeDecorator and if it is
                 # get property called impl which is the actual SqlAlchemy type. This is needed to get the python type
                 # of the column.
```

### Comparing `edgegap_factory-1.7.0/PKG-INFO` & `edgegap_factory-1.7.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-factory
-Version: 1.7.0
+Version: 1.7.1
 Summary: Edgegap library for creating SqlModel
 Author: Maxime Boisvert
 Author-email: maxime.boisvert@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

