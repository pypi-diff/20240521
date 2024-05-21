# Comparing `tmp/alembic_utils-0.8.1.tar.gz` & `tmp/alembic_utils-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alembic_utils-0.8.1.tar", last modified: Wed Feb 15 21:23:00 2023, max compression
+gzip compressed data, was "alembic_utils-0.8.2.tar", last modified: Wed Oct 18 22:09:59 2023, max compression
```

## Comparing `alembic_utils-0.8.1.tar` & `alembic_utils-0.8.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-02-15 21:23:00.145540 alembic_utils-0.8.1/
--rw-r--r--   0 oliverrice   (501) staff       (20)     1068 2021-12-27 15:58:01.000000 alembic_utils-0.8.1/LICENSE
--rw-r--r--   0 oliverrice   (501) staff       (20)      787 2023-02-15 21:23:00.145625 alembic_utils-0.8.1/PKG-INFO
--rw-r--r--   0 oliverrice   (501) staff       (20)     4857 2023-02-15 21:22:51.000000 alembic_utils-0.8.1/README.md
--rw-r--r--   0 oliverrice   (501) staff       (20)      155 2021-12-27 15:58:01.000000 alembic_utils-0.8.1/pyproject.toml
--rw-r--r--   0 oliverrice   (501) staff       (20)      103 2023-02-15 21:23:00.145859 alembic_utils-0.8.1/setup.cfg
--rw-r--r--   0 oliverrice   (501) staff       (20)     1681 2023-02-15 21:22:51.000000 alembic_utils-0.8.1/setup.py
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-02-15 21:23:00.139111 alembic_utils-0.8.1/src/
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-02-15 21:23:00.143351 alembic_utils-0.8.1/src/alembic_utils/
--rw-r--r--   0 oliverrice   (501) staff       (20)       22 2023-02-15 21:22:51.000000 alembic_utils-0.8.1/src/alembic_utils/__init__.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     4589 2023-02-15 20:45:58.000000 alembic_utils-0.8.1/src/alembic_utils/depends.py
--rw-r--r--   0 oliverrice   (501) staff       (20)      464 2022-04-07 18:44:28.000000 alembic_utils-0.8.1/src/alembic_utils/exceptions.py
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-02-15 21:23:00.145287 alembic_utils-0.8.1/src/alembic_utils/experimental/
--rw-r--r--   0 oliverrice   (501) staff       (20)      164 2021-12-27 15:58:01.000000 alembic_utils-0.8.1/src/alembic_utils/experimental/__init__.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     2727 2021-12-27 16:08:22.000000 alembic_utils-0.8.1/src/alembic_utils/experimental/_collect_instances.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     1896 2022-04-07 18:44:28.000000 alembic_utils-0.8.1/src/alembic_utils/on_entity_mixin.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     2999 2022-01-13 21:58:53.000000 alembic_utils-0.8.1/src/alembic_utils/pg_extension.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     6492 2022-07-05 19:08:22.000000 alembic_utils-0.8.1/src/alembic_utils/pg_function.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     7970 2022-04-07 18:44:28.000000 alembic_utils-0.8.1/src/alembic_utils/pg_grant_table.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     5503 2022-07-05 19:23:29.000000 alembic_utils-0.8.1/src/alembic_utils/pg_materialized_view.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     4201 2022-04-07 18:44:28.000000 alembic_utils-0.8.1/src/alembic_utils/pg_policy.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     6302 2022-04-07 18:44:28.000000 alembic_utils-0.8.1/src/alembic_utils/pg_trigger.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     3727 2022-01-13 21:58:53.000000 alembic_utils-0.8.1/src/alembic_utils/pg_view.py
--rw-r--r--   0 oliverrice   (501) staff       (20)    16598 2023-02-07 13:51:14.000000 alembic_utils-0.8.1/src/alembic_utils/replaceable_entity.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     4616 2021-12-27 15:58:01.000000 alembic_utils-0.8.1/src/alembic_utils/reversible_op.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     2214 2023-02-15 21:22:51.000000 alembic_utils-0.8.1/src/alembic_utils/simulate.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     2310 2022-04-07 18:44:28.000000 alembic_utils-0.8.1/src/alembic_utils/statement.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     1696 2023-02-15 21:22:51.000000 alembic_utils-0.8.1/src/alembic_utils/testbase.py
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-02-15 21:23:00.144926 alembic_utils-0.8.1/src/alembic_utils.egg-info/
--rw-r--r--   0 oliverrice   (501) staff       (20)      787 2023-02-15 21:23:00.000000 alembic_utils-0.8.1/src/alembic_utils.egg-info/PKG-INFO
--rw-r--r--   0 oliverrice   (501) staff       (20)      882 2023-02-15 21:23:00.000000 alembic_utils-0.8.1/src/alembic_utils.egg-info/SOURCES.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)        1 2023-02-15 21:23:00.000000 alembic_utils-0.8.1/src/alembic_utils.egg-info/dependency_links.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)      236 2023-02-15 21:23:00.000000 alembic_utils-0.8.1/src/alembic_utils.egg-info/requires.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)       14 2023-02-15 21:23:00.000000 alembic_utils-0.8.1/src/alembic_utils.egg-info/top_level.txt
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-10-18 22:09:59.939766 alembic_utils-0.8.2/
+-rw-r--r--   0 oliverrice   (501) staff       (20)     1068 2021-12-27 15:58:01.000000 alembic_utils-0.8.2/LICENSE
+-rw-r--r--   0 oliverrice   (501) staff       (20)      737 2023-10-18 22:09:59.939838 alembic_utils-0.8.2/PKG-INFO
+-rw-r--r--   0 oliverrice   (501) staff       (20)     4857 2023-02-15 21:22:51.000000 alembic_utils-0.8.2/README.md
+-rw-r--r--   0 oliverrice   (501) staff       (20)      155 2021-12-27 15:58:01.000000 alembic_utils-0.8.2/pyproject.toml
+-rw-r--r--   0 oliverrice   (501) staff       (20)      103 2023-10-18 22:09:59.940055 alembic_utils-0.8.2/setup.cfg
+-rw-r--r--   0 oliverrice   (501) staff       (20)     1630 2023-10-18 22:02:44.000000 alembic_utils-0.8.2/setup.py
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-10-18 22:09:59.931084 alembic_utils-0.8.2/src/
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-10-18 22:09:59.937078 alembic_utils-0.8.2/src/alembic_utils/
+-rw-r--r--   0 oliverrice   (501) staff       (20)       22 2023-10-18 22:09:53.000000 alembic_utils-0.8.2/src/alembic_utils/__init__.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     4589 2023-02-15 20:45:58.000000 alembic_utils-0.8.2/src/alembic_utils/depends.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)      464 2022-04-07 18:44:28.000000 alembic_utils-0.8.2/src/alembic_utils/exceptions.py
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-10-18 22:09:59.939520 alembic_utils-0.8.2/src/alembic_utils/experimental/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      164 2021-12-27 15:58:01.000000 alembic_utils-0.8.2/src/alembic_utils/experimental/__init__.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     2727 2021-12-27 16:08:22.000000 alembic_utils-0.8.2/src/alembic_utils/experimental/_collect_instances.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     1896 2022-04-07 18:44:28.000000 alembic_utils-0.8.2/src/alembic_utils/on_entity_mixin.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     2999 2022-01-13 21:58:53.000000 alembic_utils-0.8.2/src/alembic_utils/pg_extension.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     6492 2023-06-22 16:19:31.000000 alembic_utils-0.8.2/src/alembic_utils/pg_function.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     7970 2022-04-07 18:44:28.000000 alembic_utils-0.8.2/src/alembic_utils/pg_grant_table.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     5503 2022-07-05 19:23:29.000000 alembic_utils-0.8.2/src/alembic_utils/pg_materialized_view.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     4201 2022-04-07 18:44:28.000000 alembic_utils-0.8.2/src/alembic_utils/pg_policy.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     6302 2022-04-07 18:44:28.000000 alembic_utils-0.8.2/src/alembic_utils/pg_trigger.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     3727 2022-01-13 21:58:53.000000 alembic_utils-0.8.2/src/alembic_utils/pg_view.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)    16598 2023-10-18 22:01:34.000000 alembic_utils-0.8.2/src/alembic_utils/replaceable_entity.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     5335 2023-10-18 22:02:44.000000 alembic_utils-0.8.2/src/alembic_utils/reversible_op.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     2214 2023-02-15 21:22:51.000000 alembic_utils-0.8.2/src/alembic_utils/simulate.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     2310 2022-04-07 18:44:28.000000 alembic_utils-0.8.2/src/alembic_utils/statement.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     1729 2023-10-18 22:02:44.000000 alembic_utils-0.8.2/src/alembic_utils/testbase.py
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-10-18 22:09:59.939159 alembic_utils-0.8.2/src/alembic_utils.egg-info/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      737 2023-10-18 22:09:59.000000 alembic_utils-0.8.2/src/alembic_utils.egg-info/PKG-INFO
+-rw-r--r--   0 oliverrice   (501) staff       (20)      882 2023-10-18 22:09:59.000000 alembic_utils-0.8.2/src/alembic_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)        1 2023-10-18 22:09:59.000000 alembic_utils-0.8.2/src/alembic_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)      234 2023-10-18 22:09:59.000000 alembic_utils-0.8.2/src/alembic_utils.egg-info/requires.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)       14 2023-10-18 22:09:59.000000 alembic_utils-0.8.2/src/alembic_utils.egg-info/top_level.txt
```

### Comparing `alembic_utils-0.8.1/LICENSE` & `alembic_utils-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alembic_utils-0.8.1/PKG-INFO` & `alembic_utils-0.8.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: alembic_utils
-Version: 0.8.1
+Version: 0.8.2
 Summary: A sqlalchemy/alembic extension for migrating procedures and views 
 Author: Oliver Rice
 Author-email: oliver@oliverrice.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: SQL
 Requires-Python: >=3.7
 Provides-Extra: dev
```

### Comparing `alembic_utils-0.8.1/README.md` & `alembic_utils-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `alembic_utils-0.8.1/setup.py` & `alembic_utils-0.8.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     author_email="oliver@oliverrice.com",
     license="MIT",
     description="A sqlalchemy/alembic extension for migrating procedures and views ",
     python_requires=">=3.7",
     packages=find_packages("src"),
     package_dir={"": "src"},
     install_requires=[
-        "alembic>=1.5.7",
+        "alembic>=1.9",
         "flupy",
         "parse>=1.8.4",
         "sqlalchemy>=1.4",
         "typing_extensions",
     ],
     extras_require={
         "dev": DEV_REQUIRES,
@@ -47,15 +47,14 @@
     },
     include_package_data=True,
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: SQL",
     ],
 )
```

### Comparing `alembic_utils-0.8.1/src/alembic_utils/depends.py` & `alembic_utils-0.8.2/src/alembic_utils/depends.py`

 * *Files identical despite different names*

### Comparing `alembic_utils-0.8.1/src/alembic_utils/experimental/_collect_instances.py` & `alembic_utils-0.8.2/src/alembic_utils/experimental/_collect_instances.py`

 * *Files identical despite different names*

### Comparing `alembic_utils-0.8.1/src/alembic_utils/on_entity_mixin.py` & `alembic_utils-0.8.2/src/alembic_utils/on_entity_mixin.py`

 * *Files identical despite different names*

### Comparing `alembic_utils-0.8.1/src/alembic_utils/pg_extension.py` & `alembic_utils-0.8.2/src/alembic_utils/pg_extension.py`

 * *Files identical despite different names*

### Comparing `alembic_utils-0.8.1/src/alembic_utils/pg_function.py` & `alembic_utils-0.8.2/src/alembic_utils/pg_function.py`

 * *Files identical despite different names*

### Comparing `alembic_utils-0.8.1/src/alembic_utils/pg_grant_table.py` & `alembic_utils-0.8.2/src/alembic_utils/pg_grant_table.py`

 * *Files identical despite different names*

### Comparing `alembic_utils-0.8.1/src/alembic_utils/pg_materialized_view.py` & `alembic_utils-0.8.2/src/alembic_utils/pg_materialized_view.py`

 * *Files identical despite different names*

### Comparing `alembic_utils-0.8.1/src/alembic_utils/pg_policy.py` & `alembic_utils-0.8.2/src/alembic_utils/pg_policy.py`

 * *Files identical despite different names*

### Comparing `alembic_utils-0.8.1/src/alembic_utils/pg_trigger.py` & `alembic_utils-0.8.2/src/alembic_utils/pg_trigger.py`

 * *Files identical despite different names*

### Comparing `alembic_utils-0.8.1/src/alembic_utils/pg_view.py` & `alembic_utils-0.8.2/src/alembic_utils/pg_view.py`

 * *Files identical despite different names*

### Comparing `alembic_utils-0.8.1/src/alembic_utils/replaceable_entity.py` & `alembic_utils-0.8.2/src/alembic_utils/replaceable_entity.py`

 * *Files identical despite different names*

### Comparing `alembic_utils-0.8.1/src/alembic_utils/reversible_op.py` & `alembic_utils-0.8.2/src/alembic_utils/reversible_op.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Type
+from typing import TYPE_CHECKING, Any, Tuple, Type
 
 from alembic.autogenerate import renderers
 from alembic.operations import MigrateOperation, Operations
 from typing_extensions import Protocol
 
 from alembic_utils.exceptions import UnreachableException
 
@@ -48,34 +48,53 @@
 
 
 @Operations.register_operation("create_entity", "invoke_for_target")
 class CreateOp(ReversibleOp):
     def reverse(self):
         return DropOp(self.target)
 
+    def to_diff_tuple(self) -> Tuple[Any, ...]:
+        return "create_entity", self.target.identity, str(self.target.to_sql_statement_create())
+
 
 @Operations.register_operation("drop_entity", "invoke_for_target_optional_cascade")
 class DropOp(ReversibleOp):
     def __init__(self, target: "ReplaceableEntity", cascade: bool = False) -> None:
         self.cascade = cascade
         super().__init__(target)
 
     def reverse(self):
         return CreateOp(self.target)
 
+    def to_diff_tuple(self) -> Tuple[Any, ...]:
+        return "drop_entity", self.target.identity
+
 
 @Operations.register_operation("replace_entity", "invoke_for_target")
 class ReplaceOp(ReversibleOp):
     def reverse(self):
         return RevertOp(self.target)
 
+    def to_diff_tuple(self) -> Tuple[Any, ...]:
+        return (
+            "replace_or_revert_entity",
+            self.target.identity,
+            str([str(x) for x in self.target.to_sql_statement_create_or_replace()]),
+        )
+
 
 class RevertOp(ReversibleOp):
     # Revert is never in an upgrade, so no need to implement reverse
-    pass
+
+    def to_diff_tuple(self) -> Tuple[Any, ...]:
+        return (
+            "replace_or_revert_entity",
+            self.target.identity,
+            str([str(x) for x in self.target.to_sql_statement_create_or_replace()]),
+        )
 
 
 ###################
 # Implementations #
 ###################
```

### Comparing `alembic_utils-0.8.1/src/alembic_utils/simulate.py` & `alembic_utils-0.8.2/src/alembic_utils/simulate.py`

 * *Files identical despite different names*

### Comparing `alembic_utils-0.8.1/src/alembic_utils/statement.py` & `alembic_utils-0.8.2/src/alembic_utils/statement.py`

 * *Files identical despite different names*

### Comparing `alembic_utils-0.8.1/src/alembic_utils/testbase.py` & `alembic_utils-0.8.2/src/alembic_utils/testbase.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 
 ALEMBIC_COMMAND_MAP: Dict[str, Callable[..., NoReturn]] = {
     "upgrade": alem_command.upgrade,
     "downgrade": alem_command.downgrade,
     "revision": alem_command.revision,
     "current": alem_command.current,
+    "check": alem_command.check,
 }
 
 
 def build_alembic_config(engine: Engine) -> Config:
     """Populate alembic configuration from metadata and config file."""
     path_to_alembic_ini = REPO_ROOT / "alembic.ini"
```

### Comparing `alembic_utils-0.8.1/src/alembic_utils.egg-info/PKG-INFO` & `alembic_utils-0.8.2/src/alembic_utils.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: alembic-utils
-Version: 0.8.1
+Version: 0.8.2
 Summary: A sqlalchemy/alembic extension for migrating procedures and views 
 Author: Oliver Rice
 Author-email: oliver@oliverrice.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: SQL
 Requires-Python: >=3.7
 Provides-Extra: dev
```

### Comparing `alembic_utils-0.8.1/src/alembic_utils.egg-info/SOURCES.txt` & `alembic_utils-0.8.2/src/alembic_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

