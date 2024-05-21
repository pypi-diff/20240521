# Comparing `tmp/data_snack-1.0.2.tar.gz` & `tmp/data_snack-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_snack-1.0.2.tar", last modified: Thu Mar 28 13:37:39 2024, max compression
+gzip compressed data, was "data_snack-1.0.3.tar", last modified: Tue May 21 08:57:49 2024, max compression
```

## Comparing `data_snack-1.0.2.tar` & `data_snack-1.0.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:37:39.250074 data_snack-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-28 13:37:34.000000 data_snack-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-28 13:37:34.000000 data_snack-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-03-28 13:37:39.250074 data_snack-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-03-28 13:37:34.000000 data_snack-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-28 13:37:34.000000 data_snack-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-28 13:37:34.000000 data_snack-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-28 13:37:39.250074 data_snack-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-28 13:37:34.000000 data_snack-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:37:39.242074 data_snack-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:37:39.246075 data_snack-1.0.2/src/data_snack/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:37:39.246075 data_snack-1.0.2/src/data_snack/connections/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/connections/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/connections/memcached.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/connections/mongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/connections/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:37:39.246075 data_snack-1.0.2/src/data_snack/entities/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/entities/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/entities/entity_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/entities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/entities/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/entities/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:37:39.250074 data_snack-1.0.2/src/data_snack/key_factories/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/key_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/key_factories/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/key_factories/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/key_factories/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/key_factories/non_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:37:39.250074 data_snack-1.0.2/src/data_snack/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/serializers/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/snack.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:37:39.250074 data_snack-1.0.2/src/data_snack/wrap/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/wrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/wrap/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/wrap/data_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/wrap/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-28 13:37:34.000000 data_snack-1.0.2/src/data_snack/wrap/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:37:39.250074 data_snack-1.0.2/src/data_snack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-03-28 13:37:39.000000 data_snack-1.0.2/src/data_snack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-28 13:37:39.000000 data_snack-1.0.2/src/data_snack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 13:37:39.000000 data_snack-1.0.2/src/data_snack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-28 13:37:39.000000 data_snack-1.0.2/src/data_snack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-28 13:37:39.000000 data_snack-1.0.2/src/data_snack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:37:39.250074 data_snack-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-28 13:37:34.000000 data_snack-1.0.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.743463 data_snack-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-21 08:57:42.000000 data_snack-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-21 08:57:42.000000 data_snack-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-21 08:57:49.743463 data_snack-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-21 08:57:42.000000 data_snack-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 08:57:42.000000 data_snack-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 08:57:42.000000 data_snack-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 08:57:49.743463 data_snack-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-21 08:57:42.000000 data_snack-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.735463 data_snack-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.735463 data_snack-1.0.3/src/data_snack/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.739463 data_snack-1.0.3/src/data_snack/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/connections/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/connections/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/connections/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/connections/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.739463 data_snack-1.0.3/src/data_snack/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/entities/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/entities/entity_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/entities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/entities/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/entities/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.739463 data_snack-1.0.3/src/data_snack/key_factories/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/key_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/key_factories/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/key_factories/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/key_factories/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/key_factories/non_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.739463 data_snack-1.0.3/src/data_snack/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/serializers/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/snack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.743463 data_snack-1.0.3/src/data_snack/wrap/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/wrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/wrap/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/wrap/data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/wrap/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/wrap/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.743463 data_snack-1.0.3/src/data_snack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-21 08:57:49.000000 data_snack-1.0.3/src/data_snack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-21 08:57:49.000000 data_snack-1.0.3/src/data_snack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:57:49.000000 data_snack-1.0.3/src/data_snack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-21 08:57:49.000000 data_snack-1.0.3/src/data_snack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 08:57:49.000000 data_snack-1.0.3/src/data_snack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.743463 data_snack-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-21 08:57:42.000000 data_snack-1.0.3/tests/test_utils.py
```

### Comparing `data_snack-1.0.2/LICENSE` & `data_snack-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/PKG-INFO` & `data_snack-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_snack
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://github.com/webinterpret-ds/data-snack
 Author: webinterpret-datascience
 Author-email: data-science@webinterpret.com
 Project-URL: Bug Tracker, https://github.com/webinterpret-ds/data-snack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `data_snack-1.0.2/README.md` & `data_snack-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/setup.cfg` & `data_snack-1.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = data-snack
-version = 1.0.2
+version = 1.0.3
 author = webinterpret-datascience
 author_email = data-science@webinterpret.com
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/webinterpret-ds/data-snack
 project_urls =
```

### Comparing `data_snack-1.0.2/setup.py` & `data_snack-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/src/data_snack/connections/base.py` & `data_snack-1.0.3/src/data_snack/connections/base.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/src/data_snack/connections/memcached.py` & `data_snack-1.0.3/src/data_snack/connections/memcached.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/src/data_snack/connections/mongo.py` & `data_snack-1.0.3/src/data_snack/connections/mongo.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/src/data_snack/connections/redis.py` & `data_snack-1.0.3/src/data_snack/connections/redis.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/src/data_snack/entities/entity.py` & `data_snack-1.0.3/src/data_snack/entities/entity.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/src/data_snack/entities/entity_meta.py` & `data_snack-1.0.3/src/data_snack/entities/entity_meta.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/src/data_snack/entities/schema.py` & `data_snack-1.0.3/src/data_snack/entities/schema.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/src/data_snack/key_factories/base.py` & `data_snack-1.0.3/src/data_snack/key_factories/base.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/src/data_snack/serializers/base.py` & `data_snack-1.0.3/src/data_snack/serializers/base.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/src/data_snack/serializers/dataclass.py` & `data_snack-1.0.3/src/data_snack/serializers/dataclass.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/src/data_snack/serializers/json.py` & `data_snack-1.0.3/src/data_snack/serializers/json.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/src/data_snack/snack.py` & `data_snack-1.0.3/src/data_snack/snack.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/src/data_snack/wrap/base.py` & `data_snack-1.0.3/src/data_snack/wrap/base.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/src/data_snack/wrap/data_frame.py` & `data_snack-1.0.3/src/data_snack/wrap/data_frame.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/src/data_snack/wrap/entity.py` & `data_snack-1.0.3/src/data_snack/wrap/entity.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/src/data_snack.egg-info/PKG-INFO` & `data_snack-1.0.3/src/data_snack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_snack
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://github.com/webinterpret-ds/data-snack
 Author: webinterpret-datascience
 Author-email: data-science@webinterpret.com
 Project-URL: Bug Tracker, https://github.com/webinterpret-ds/data-snack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `data_snack-1.0.2/src/data_snack.egg-info/SOURCES.txt` & `data_snack-1.0.3/src/data_snack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.2/tests/test_utils.py` & `data_snack-1.0.3/tests/test_utils.py`

 * *Files identical despite different names*

