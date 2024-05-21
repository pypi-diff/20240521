# Comparing `tmp/docmesh_core-0.0.6.tar.gz` & `tmp/docmesh_core-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_core-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_core-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_core-0.0.6.tar` & `docmesh_core-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       10 2024-05-13 04:13:58.033801 docmesh_core-0.0.6/README.md
--rw-r--r--   0        0        0       22 2024-05-20 07:43:11.239920 docmesh_core-0.0.6/docmesh_core/__init__.py
--rw-r--r--   0        0        0     1388 2024-05-20 07:41:31.413472 docmesh_core-0.0.6/docmesh_core/db/__init__.py
--rw-r--r--   0        0        0     1325 2024-05-13 04:13:58.033801 docmesh_core-0.0.6/docmesh_core/db/auth.py
--rw-r--r--   0        0        0    11864 2024-05-20 05:24:06.535535 docmesh_core-0.0.6/docmesh_core/db/neo.py
--rw-r--r--   0        0        0      417 2024-05-15 10:24:49.939048 docmesh_core-0.0.6/docmesh_core/utils/__init__.py
--rw-r--r--   0        0        0      269 2024-05-13 04:13:58.037801 docmesh_core-0.0.6/docmesh_core/utils/graph_utils.py
--rw-r--r--   0        0        0     3857 2024-05-13 11:40:13.918990 docmesh_core-0.0.6/docmesh_core/utils/semantic_scholar.py
--rw-r--r--   0        0        0      750 2024-05-13 04:13:58.037801 docmesh_core-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 docmesh_core-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-05-13 04:13:58.033801 docmesh_core-0.0.7/README.md
+-rw-r--r--   0        0        0       22 2024-05-20 09:07:34.938414 docmesh_core-0.0.7/docmesh_core/__init__.py
+-rw-r--r--   0        0        0     1388 2024-05-20 07:41:31.413472 docmesh_core-0.0.7/docmesh_core/db/__init__.py
+-rw-r--r--   0        0        0     1325 2024-05-13 04:13:58.033801 docmesh_core-0.0.7/docmesh_core/db/auth.py
+-rw-r--r--   0        0        0    11863 2024-05-20 08:48:01.707729 docmesh_core-0.0.7/docmesh_core/db/neo.py
+-rw-r--r--   0        0        0      417 2024-05-15 10:24:49.939048 docmesh_core-0.0.7/docmesh_core/utils/__init__.py
+-rw-r--r--   0        0        0      269 2024-05-13 04:13:58.037801 docmesh_core-0.0.7/docmesh_core/utils/graph_utils.py
+-rw-r--r--   0        0        0     3857 2024-05-13 11:40:13.918990 docmesh_core-0.0.7/docmesh_core/utils/semantic_scholar.py
+-rw-r--r--   0        0        0      750 2024-05-13 04:13:58.037801 docmesh_core-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 docmesh_core-0.0.7/PKG-INFO
```

### Comparing `docmesh_core-0.0.6/docmesh_core/db/__init__.py` & `docmesh_core-0.0.7/docmesh_core/db/__init__.py`

 * *Files identical despite different names*

### Comparing `docmesh_core-0.0.6/docmesh_core/db/auth.py` & `docmesh_core-0.0.7/docmesh_core/db/auth.py`

 * *Files identical despite different names*

### Comparing `docmesh_core-0.0.6/docmesh_core/db/neo.py` & `docmesh_core-0.0.7/docmesh_core/db/neo.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,14 @@
 
 class Venue(StructuredNode):
     name = StringProperty(unique_index=True)
 
     collections = RelationshipTo("Collection", "publish")
 
 
-
 def _nodelist_to_dataframe(nodes: list[StructuredNode]) -> DataFrame:
     df = pd.DataFrame.from_dict([node.serialize for node in nodes])
     return df
 
 
 def get_entity(entity_name: str) -> Entity:
     entity = Entity.nodes.get(name=entity_name)
```

### Comparing `docmesh_core-0.0.6/docmesh_core/utils/semantic_scholar.py` & `docmesh_core-0.0.7/docmesh_core/utils/semantic_scholar.py`

 * *Files identical despite different names*

### Comparing `docmesh_core-0.0.6/pyproject.toml` & `docmesh_core-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docmesh_core-0.0.6/PKG-INFO` & `docmesh_core-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmesh_core
-Version: 0.0.6
+Version: 0.0.7
 Summary: Core components for docmesh.
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

