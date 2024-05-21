# Comparing `tmp/dungeonmaker-0.6.7.tar.gz` & `tmp/dungeonmaker-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dungeonmaker-0.6.7.tar", last modified: Mon May 20 18:53:45 2024, max compression
+gzip compressed data, was "dungeonmaker-0.6.8.tar", last modified: Tue May 21 06:58:44 2024, max compression
```

## Comparing `dungeonmaker-0.6.7.tar` & `dungeonmaker-0.6.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:53:45.806608 dungeonmaker-0.6.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-20 18:53:45.806608 dungeonmaker-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:53:45.802608 dungeonmaker-0.6.7/dungeonmaker/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:53:45.802608 dungeonmaker-0.6.7/dungeonmaker/dm_backend/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17455 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:53:45.802608 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:53:45.802608 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/database/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/database/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/database/dba.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:53:45.802608 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/dba.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/dmtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/dungeon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/room.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:53:45.802608 dungeonmaker-0.6.7/dungeonmaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-20 18:53:45.000000 dungeonmaker-0.6.7/dungeonmaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-20 18:53:45.000000 dungeonmaker-0.6.7/dungeonmaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:53:45.000000 dungeonmaker-0.6.7/dungeonmaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 18:53:45.000000 dungeonmaker-0.6.7/dungeonmaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 18:53:45.000000 dungeonmaker-0.6.7/dungeonmaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:53:45.806608 dungeonmaker-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:58:44.190410 dungeonmaker-0.6.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 06:58:44.190410 dungeonmaker-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:58:44.186410 dungeonmaker-0.6.8/dungeonmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:58:44.186410 dungeonmaker-0.6.8/dungeonmaker/dm_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17455 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:58:44.186410 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:58:44.186410 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/database/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/database/dba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:58:44.190410 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/dba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/dmtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/dungeon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/room.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:58:44.190410 dungeonmaker-0.6.8/dungeonmaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 06:58:44.000000 dungeonmaker-0.6.8/dungeonmaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-21 06:58:44.000000 dungeonmaker-0.6.8/dungeonmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 06:58:44.000000 dungeonmaker-0.6.8/dungeonmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-21 06:58:44.000000 dungeonmaker-0.6.8/dungeonmaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 06:58:44.000000 dungeonmaker-0.6.8/dungeonmaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 06:58:44.190410 dungeonmaker-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/setup.py
```

### Comparing `dungeonmaker-0.6.7/LICENSE` & `dungeonmaker-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.7/PKG-INFO` & `dungeonmaker-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dungeonmaker
-Version: 0.6.7
+Version: 0.6.8
 Summary: Dungeon maker backend and other things
 Home-page: https://github.com/thecommcraft/dungeon-maker-reinvented
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dungeonmaker-0.6.7/dungeonmaker/dm_backend/backend.py` & `dungeonmaker-0.6.8/dungeonmaker/dm_backend/backend.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/database/basetypes.py` & `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/database/basetypes.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/database/connection.py` & `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/database/connection.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/database/dba.py` & `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/database/dba.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Submodule for Database Abstractions.
 """
 from typing import Literal
 from dataclasses import dataclass, field
 from .basetypes import BaseMongoDBAtlasSession
-from ..dm.dba import dba.BaseDatabaseAbstraction
+from ..dm.dba import BaseDatabaseAbstraction
 from ..dm.dmtypes import UserId, DungeonId, RoomId
 
 @dataclass(slots=True)
-class MongoDBDatabaseAbstraction(dba.BaseDatabaseAbstraction):
+class MongoDBDatabaseAbstraction(BaseDatabaseAbstraction):
     """
     Class for MongoDB database abstractions.
     """
     connection : BaseMongoDBAtlasSession = field(kw_only=True)
     
     def select_user(self, user_id : UserId = None, *, fields : dict = None) -> dict:
         """
```

### Comparing `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/dba.py` & `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/dba.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/dmtypes.py` & `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/dmtypes.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/dungeon.py` & `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/dungeon.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/room.py` & `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/room.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/session.py` & `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/session.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/user.py` & `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/user.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.7/dungeonmaker.egg-info/PKG-INFO` & `dungeonmaker-0.6.8/dungeonmaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dungeonmaker
-Version: 0.6.7
+Version: 0.6.8
 Summary: Dungeon maker backend and other things
 Home-page: https://github.com/thecommcraft/dungeon-maker-reinvented
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dungeonmaker-0.6.7/dungeonmaker.egg-info/SOURCES.txt` & `dungeonmaker-0.6.8/dungeonmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.7/setup.py` & `dungeonmaker-0.6.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='dungeonmaker',
-    version='0.6.7',
+    version='0.6.8',
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='Dungeon maker backend and other things',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/thecommcraft/dungeon-maker-reinvented',
     packages=find_packages(),
```

