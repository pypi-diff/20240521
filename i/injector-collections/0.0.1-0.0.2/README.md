# Comparing `tmp/injector_collections-0.0.1.tar.gz` & `tmp/injector_collections-0.0.2.tar.gz`

## Comparing `injector_collections-0.0.1.tar` & `injector_collections-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 injector_collections-0.0.1/src/injector_collections/Collection.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 injector_collections-0.0.1/src/injector_collections/CollectionItem.py
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 injector_collections-0.0.1/src/injector_collections/Generator.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 injector_collections-0.0.1/src/injector_collections/__init__.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 injector_collections-0.0.1/src/injector_collections/collections.jinja
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 injector_collections-0.0.1/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 injector_collections-0.0.1/LICENSE
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 injector_collections-0.0.1/README.md
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 injector_collections-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5466 2020-02-02 00:00:00.000000 injector_collections-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 injector_collections-0.0.2/src/injector_collections/Collection.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 injector_collections-0.0.2/src/injector_collections/CollectionItem.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 injector_collections-0.0.2/src/injector_collections/Generator.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 injector_collections-0.0.2/src/injector_collections/__init__.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 injector_collections-0.0.2/src/injector_collections/collections.jinja
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 injector_collections-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 injector_collections-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 injector_collections-0.0.2/README.md
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 injector_collections-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5466 2020-02-02 00:00:00.000000 injector_collections-0.0.2/PKG-INFO
```

### Comparing `injector_collections-0.0.1/src/injector_collections/CollectionItem.py` & `injector_collections-0.0.2/src/injector_collections/CollectionItem.py`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.1/src/injector_collections/Generator.py` & `injector_collections-0.0.2/src/injector_collections/Generator.py`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.1/src/injector_collections/collections.jinja` & `injector_collections-0.0.2/src/injector_collections/collections.jinja`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.1/LICENSE` & `injector_collections-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.1/README.md` & `injector_collections-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.1/pyproject.toml` & `injector_collections-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "injector_collections"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Benjamin Schnitzler", email="regenbogenbauer@web.de" },
 ]
 description = "Collections for the Injector Package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `injector_collections-0.0.1/PKG-INFO` & `injector_collections-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: injector_collections
-Version: 0.0.1
+Version: 0.0.2
 Summary: Collections for the Injector Package
 Project-URL: Homepage, https://github.com/bschnitz/injector_collections
 Project-URL: Issues, https://github.com/bschnitz/injector_collections/issues
 Author-email: Benjamin Schnitzler <regenbogenbauer@web.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

