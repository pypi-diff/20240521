# Comparing `tmp/organization_profile_local-0.0.4.tar.gz` & `tmp/organization_profile_local-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "organization_profile_local-0.0.4.tar", last modified: Wed May  8 12:25:45 2024, max compression
+gzip compressed data, was "organization_profile_local-0.0.5.tar", last modified: Tue May 21 21:03:10 2024, max compression
```

## Comparing `organization_profile_local-0.0.4.tar` & `organization_profile_local-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:25:45.400213 organization_profile_local-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-08 12:25:45.400213 organization_profile_local-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 12:25:23.000000 organization_profile_local-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:25:45.392213 organization_profile_local-0.0.4/organization_profile_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:25:45.396213 organization_profile_local-0.0.4/organization_profile_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:25:23.000000 organization_profile_local-0.0.4/organization_profile_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-08 12:25:23.000000 organization_profile_local-0.0.4/organization_profile_local/src/organization_profile_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-08 12:25:23.000000 organization_profile_local-0.0.4/organization_profile_local/src/organization_profile_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:25:45.396213 organization_profile_local-0.0.4/organization_profile_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-08 12:25:45.000000 organization_profile_local-0.0.4/organization_profile_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-08 12:25:45.000000 organization_profile_local-0.0.4/organization_profile_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:25:45.000000 organization_profile_local-0.0.4/organization_profile_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-08 12:25:45.000000 organization_profile_local-0.0.4/organization_profile_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 12:25:45.000000 organization_profile_local-0.0.4/organization_profile_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-08 12:25:23.000000 organization_profile_local-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:25:45.400213 organization_profile_local-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-08 12:25:23.000000 organization_profile_local-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:03:10.823605 organization_profile_local-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-21 21:03:10.823605 organization_profile_local-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 21:02:36.000000 organization_profile_local-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:03:10.823605 organization_profile_local-0.0.5/organization_profile_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:03:10.823605 organization_profile_local-0.0.5/organization_profile_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 21:02:36.000000 organization_profile_local-0.0.5/organization_profile_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-21 21:02:36.000000 organization_profile_local-0.0.5/organization_profile_local/src/organization_profile_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-05-21 21:02:36.000000 organization_profile_local-0.0.5/organization_profile_local/src/organization_profile_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:03:10.823605 organization_profile_local-0.0.5/organization_profile_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-21 21:03:10.000000 organization_profile_local-0.0.5/organization_profile_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-21 21:03:10.000000 organization_profile_local-0.0.5/organization_profile_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 21:03:10.000000 organization_profile_local-0.0.5/organization_profile_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-21 21:03:10.000000 organization_profile_local-0.0.5/organization_profile_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 21:03:10.000000 organization_profile_local-0.0.5/organization_profile_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-21 21:02:36.000000 organization_profile_local-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 21:03:10.823605 organization_profile_local-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-21 21:02:36.000000 organization_profile_local-0.0.5/setup.py
```

### Comparing `organization_profile_local-0.0.4/PKG-INFO` & `organization_profile_local-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: organization-profile-local
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyPI Package for Circles organization-profile-local Python
 Home-page: https://github.com/circles-zone/organization-profile-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `organization_profile_local-0.0.4/organization_profile_local/src/organization_profile_constants.py` & `organization_profile_local-0.0.5/organization_profile_local/src/organization_profile_constants.py`

 * *Files identical despite different names*

### Comparing `organization_profile_local-0.0.4/organization_profile_local/src/organization_profile_local.py` & `organization_profile_local-0.0.5/organization_profile_local/src/organization_profile_local.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dotenv import load_dotenv
+from datetime import datetime
 from logger_local.Logger import Logger
 from .organization_profile_constants import ORGANIZATION_PROFILE_PYTHON_PACKAGE_CODE_LOGGER_OBJECT
 from database_mysql_local.generic_mapping import GenericMapping
 load_dotenv()
 
 logger = Logger(object=ORGANIZATION_PROFILE_PYTHON_PACKAGE_CODE_LOGGER_OBJECT)
 
@@ -10,15 +11,15 @@
 DEFAULT_TABLE_NAME = "organization_profile_table"
 DEFAULT_VIEW_NAME = "organization_profile_view"
 DEFAULT_ID_COLUMN_NAME = "organization_profile_id"
 DEFAULT_ENTITY_NAME1 = "organization"
 DEFAULT_ENTITY_NAME2 = "profile"
 
 
-class OrganizationProfileLocal(GenericMapping):
+class OrganizationProfilesLocal(GenericMapping):
     def __init__(self, is_test_data: bool = False):
         GenericMapping.__init__(self, default_schema_name=DEFAULT_SCHEMA_NAME,
                                 default_table_name=DEFAULT_TABLE_NAME,
                                 default_view_table_name=DEFAULT_VIEW_NAME,
                                 default_id_column_name=DEFAULT_ID_COLUMN_NAME,
                                 default_entity_name1=DEFAULT_ENTITY_NAME1,
                                 default_entity_name2=DEFAULT_ENTITY_NAME2,
@@ -72,14 +73,27 @@
             where="profile_id = %s",
             params=(profile_id,)
         )
         organization_ids_list = [organization_id for (organization_id,) in organization_ids_tuple_list]
         logger.end(object={"organization_ids_list": organization_ids_list})
         return organization_ids_list
 
+    # get organization ids linked to a profile id with updated_timestamp greater than remote_last_modified_timestamp
+    def get_linked_organization_ids_with_updated_timestamp(self, profile_id: int,
+                                                           remote_last_modified_timestamp: datetime) -> list[int]:
+        logger.start(object={"profile_id": profile_id, "remote_last_modified_timestamp": remote_last_modified_timestamp})
+        organization_ids_tuple_list = self.select_multi_tuple_by_where(
+            select_clause_value="organization_id",
+            where="profile_id = %s AND updated_timestamp > %s",
+            params=(profile_id, remote_last_modified_timestamp)
+        )
+        organization_ids_list = [organization_id for (organization_id,) in organization_ids_tuple_list]
+        logger.end(object={"organization_ids_list": organization_ids_list})
+        return organization_ids_list
+
     def get_organization_profile_id(self, organization_id: int, profile_id: int) -> int | None:
         logger.start(object={"organization_id": organization_id, "profile_id": profile_id})
         organization_profile_id_dict = self.select_one_dict_by_where(
             select_clause_value="organization_profile_id",
             where="organization_id = %s AND profile_id = %s",
             params=(organization_id, profile_id)
         )
```

### Comparing `organization_profile_local-0.0.4/organization_profile_local.egg-info/PKG-INFO` & `organization_profile_local-0.0.5/organization_profile_local.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: organization-profile-local
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyPI Package for Circles organization-profile-local Python
 Home-page: https://github.com/circles-zone/organization-profile-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `organization_profile_local-0.0.4/setup.py` & `organization_profile_local-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "organization-profile-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.4',  # update only the minor version each time # https://pypi.org/project/organization-profile-local/
+    version='0.0.5',  # update only the minor version each time # https://pypi.org/project/organization-profile-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles organization-profile-local Python",
     long_description="PyPI Package for Circles organization-profile-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/organization-profile-local-python-package",
     packages=[package_dir],
```

