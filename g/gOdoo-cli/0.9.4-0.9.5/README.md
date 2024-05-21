# Comparing `tmp/godoo_cli-0.9.4.tar.gz` & `tmp/godoo_cli-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godoo_cli-0.9.4.tar", max compression
+gzip compressed data, was "godoo_cli-0.9.5.tar", max compression
```

## Comparing `godoo_cli-0.9.4.tar` & `godoo_cli-0.9.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     7633 2023-12-13 18:48:37.493760 godoo_cli-0.9.4/LICENSE
--rw-r--r--   0        0        0     7300 2023-12-13 18:48:37.493760 godoo_cli-0.9.4/README.md
--rw-r--r--   0        0        0     5078 2023-12-13 18:48:54.837793 godoo_cli-0.9.4/pyproject.toml
--rw-r--r--   0        0        0       61 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/__init__.py
--rw-r--r--   0        0        0       88 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/__main__.py
--rw-r--r--   0        0        0     2214 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/cli.py
--rw-r--r--   0        0        0     5061 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/cli_common.py
--rw-r--r--   0        0        0      373 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/__init__.py
--rw-r--r--   0        0        0       32 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/backup/__init__.py
--rw-r--r--   0        0        0      443 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/backup/cli.py
--rw-r--r--   0        0        0     2395 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/backup/dump.py
--rw-r--r--   0        0        0     3102 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/backup/load.py
--rw-r--r--   0        0        0     5280 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/backup/pull.py
--rw-r--r--   0        0        0     1360 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/backup/util.py
--rw-r--r--   0        0        0     6262 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/bootstrap.py
--rw-r--r--   0        0        0     1173 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/config.py
--rw-r--r--   0        0        0       28 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/db/__init__.py
--rw-r--r--   0        0        0      540 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/db/cli.py
--rw-r--r--   0        0        0     3079 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/db/connection.py
--rw-r--r--   0        0        0     1400 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/db/passwords.py
--rw-r--r--   0        0        0     4062 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/db/query.py
--rw-r--r--   0        0        0    10790 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/launch.py
--rw-r--r--   0        0        0      177 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/rpc/__init__.py
--rw-r--r--   0        0        0      897 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/rpc/cli.py
--rw-r--r--   0        0        0     1484 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/rpc/config_parameters.py
--rw-r--r--   0        0        0     2278 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/rpc/importer.py
--rw-r--r--   0        0        0     4828 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/rpc/modules.py
--rw-r--r--   0        0        0     3912 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/rpc/translations.py
--rw-r--r--   0        0        0     2619 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/shell.py
--rw-r--r--   0        0        0    11815 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/source_get.py
--rw-r--r--   0        0        0      123 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/test/__init__.py
--rw-r--r--   0        0        0      345 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/test/cli.py
--rw-r--r--   0        0        0     3437 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/test/test_load_data.py
--rw-r--r--   0        0        0     5418 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/commands/test/test_run.py
--rw-r--r--   0        0        0      161 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/git/__init__.py
--rw-r--r--   0        0        0     1300 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/git/git_odoo.py
--rw-r--r--   0        0        0     3296 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/git/git_odoo_addons.py
--rw-r--r--   0        0        0     6460 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/git/git_repo.py
--rw-r--r--   0        0        0     4585 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/git/git_url.py
--rw-r--r--   0        0        0     1575 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/git/zip_download.py
--rw-r--r--   0        0        0       49 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/helpers/__init__.py
--rw-r--r--   0        0        0     2201 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/helpers/bootstrap.py
--rw-r--r--   0        0        0      386 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/helpers/cli.py
--rw-r--r--   0        0        0     9532 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/helpers/odoo_files.py
--rw-r--r--   0        0        0     3277 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/helpers/odoo_manifest.py
--rw-r--r--   0        0        0     4691 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/helpers/system.py
--rw-r--r--   0        0        0       22 2023-12-13 18:48:37.497760 godoo_cli-0.9.4/src/godoo_cli/version.py
--rw-r--r--   0        0        0     9359 1970-01-01 00:00:00.000000 godoo_cli-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     7633 2023-12-13 21:41:46.405141 godoo_cli-0.9.5/LICENSE
+-rw-r--r--   0        0        0     7300 2023-12-13 21:41:46.405141 godoo_cli-0.9.5/README.md
+-rw-r--r--   0        0        0     5078 2023-12-13 21:42:02.489086 godoo_cli-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/__init__.py
+-rw-r--r--   0        0        0       88 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/__main__.py
+-rw-r--r--   0        0        0     2214 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/cli.py
+-rw-r--r--   0        0        0     5061 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/cli_common.py
+-rw-r--r--   0        0        0      373 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/__init__.py
+-rw-r--r--   0        0        0       32 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/backup/__init__.py
+-rw-r--r--   0        0        0      443 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/backup/cli.py
+-rw-r--r--   0        0        0     2395 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/backup/dump.py
+-rw-r--r--   0        0        0     3102 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/backup/load.py
+-rw-r--r--   0        0        0     5280 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/backup/pull.py
+-rw-r--r--   0        0        0     1360 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/backup/util.py
+-rw-r--r--   0        0        0     6259 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/bootstrap.py
+-rw-r--r--   0        0        0     1173 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/config.py
+-rw-r--r--   0        0        0       28 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/db/__init__.py
+-rw-r--r--   0        0        0      540 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/db/cli.py
+-rw-r--r--   0        0        0     3079 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/db/connection.py
+-rw-r--r--   0        0        0     1400 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/db/passwords.py
+-rw-r--r--   0        0        0     4062 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/db/query.py
+-rw-r--r--   0        0        0    10790 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/launch.py
+-rw-r--r--   0        0        0      177 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/rpc/__init__.py
+-rw-r--r--   0        0        0      897 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/rpc/cli.py
+-rw-r--r--   0        0        0     1484 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/rpc/config_parameters.py
+-rw-r--r--   0        0        0     2278 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/rpc/importer.py
+-rw-r--r--   0        0        0     4828 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/rpc/modules.py
+-rw-r--r--   0        0        0     3912 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/rpc/translations.py
+-rw-r--r--   0        0        0     2619 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/shell.py
+-rw-r--r--   0        0        0    11815 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/source_get.py
+-rw-r--r--   0        0        0      123 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/test/__init__.py
+-rw-r--r--   0        0        0      345 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/test/cli.py
+-rw-r--r--   0        0        0     3437 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/test/test_load_data.py
+-rw-r--r--   0        0        0     5418 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/commands/test/test_run.py
+-rw-r--r--   0        0        0      161 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/git/__init__.py
+-rw-r--r--   0        0        0     1300 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/git/git_odoo.py
+-rw-r--r--   0        0        0     3296 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/git/git_odoo_addons.py
+-rw-r--r--   0        0        0     6460 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/git/git_repo.py
+-rw-r--r--   0        0        0     4585 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/git/git_url.py
+-rw-r--r--   0        0        0     1575 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/git/zip_download.py
+-rw-r--r--   0        0        0       49 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/helpers/__init__.py
+-rw-r--r--   0        0        0     2201 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/helpers/bootstrap.py
+-rw-r--r--   0        0        0      386 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/helpers/cli.py
+-rw-r--r--   0        0        0     9532 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/helpers/odoo_files.py
+-rw-r--r--   0        0        0     3277 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/helpers/odoo_manifest.py
+-rw-r--r--   0        0        0     4691 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/helpers/system.py
+-rw-r--r--   0        0        0       22 2023-12-13 21:41:46.409141 godoo_cli-0.9.5/src/godoo_cli/version.py
+-rw-r--r--   0        0        0     9359 1970-01-01 00:00:00.000000 godoo_cli-0.9.5/PKG-INFO
```

### Comparing `godoo_cli-0.9.4/LICENSE` & `godoo_cli-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/README.md` & `godoo_cli-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/pyproject.toml` & `godoo_cli-0.9.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gOdoo-cli"
-version = "0.9.4"
+version = "0.9.5"
 description = "Wrapper around Odoo-Bin with some convinience RPC functions."
 authors = ["Joshua Kreuder <Joshua_Kreuder@outlook.com>"]
 license = "LGPL-3"
 readme = "README.md"
 packages = [{include = "godoo_cli",  from = "src"}]
 repository = "https://github.com/OpenJKSoftware/gOdoo"
 keywords = ["odoo", "godoo","devcontainer"]
```

### Comparing `godoo_cli-0.9.4/src/godoo_cli/cli.py` & `godoo_cli-0.9.5/src/godoo_cli/cli.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/cli_common.py` & `godoo_cli-0.9.5/src/godoo_cli/cli_common.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/backup/dump.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/backup/dump.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/backup/load.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/backup/load.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/backup/pull.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/backup/pull.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/backup/util.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/backup/util.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/bootstrap.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/bootstrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,21 +79,23 @@
         f"--db-filter=^{db_filter}$",
     ]
 
     LOGGER.info("Getting Addon Paths")
 
     init_modules = []
     extra_cmd_args_str = " ".join(extra_cmd_args or [])
-    if not re.match(r"(-i|--init|-u|--upgrade) ", extra_cmd_args_str):
+    if not re.search(r"(-i|--init) ", extra_cmd_args_str):
         if install_workspace_modules:
-            workspace_addons = get_odoo_module_paths(workspace_addon_path)
-            if install_workspace_modules and workspace_addons:
+            if workspace_addons := get_odoo_module_paths(workspace_addon_path):
                 init_modules += [f.name for f in workspace_addons]
-        elif not re.match(r"(-u|--update) ", extra_cmd_args_str):
-            # If Upgrade command is present, we assume base and web are already installed
+        elif re.search(r"(-u|--update) ", extra_cmd_args_str):
+            # if -u is present, do not install any modules
+            pass
+        else:
+            # if no -i or -u is present, install base and web modules
             init_modules = ["base", "web"]
     init_cmd = "--init " + ",".join(init_modules) if init_modules else ""
 
     addon_paths = [str(p.absolute()) for p in addon_paths]
     addon_paths = ", ".join(list(filter(None, addon_paths)))
 
     base_cmds = [
```

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/config.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/db/cli.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/db/cli.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/db/connection.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/db/connection.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/db/passwords.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/db/passwords.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/db/query.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/db/query.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/launch.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/launch.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/rpc/cli.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/rpc/cli.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/rpc/config_parameters.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/rpc/config_parameters.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/rpc/importer.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/rpc/importer.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/rpc/modules.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/rpc/modules.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/rpc/translations.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/rpc/translations.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/shell.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/shell.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/source_get.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/source_get.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/test/test_load_data.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/test/test_load_data.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/commands/test/test_run.py` & `godoo_cli-0.9.5/src/godoo_cli/commands/test/test_run.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/git/git_odoo.py` & `godoo_cli-0.9.5/src/godoo_cli/git/git_odoo.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/git/git_odoo_addons.py` & `godoo_cli-0.9.5/src/godoo_cli/git/git_odoo_addons.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/git/git_repo.py` & `godoo_cli-0.9.5/src/godoo_cli/git/git_repo.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/git/git_url.py` & `godoo_cli-0.9.5/src/godoo_cli/git/git_url.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/git/zip_download.py` & `godoo_cli-0.9.5/src/godoo_cli/git/zip_download.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/helpers/bootstrap.py` & `godoo_cli-0.9.5/src/godoo_cli/helpers/bootstrap.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/helpers/odoo_files.py` & `godoo_cli-0.9.5/src/godoo_cli/helpers/odoo_files.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/helpers/odoo_manifest.py` & `godoo_cli-0.9.5/src/godoo_cli/helpers/odoo_manifest.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/src/godoo_cli/helpers/system.py` & `godoo_cli-0.9.5/src/godoo_cli/helpers/system.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.9.4/PKG-INFO` & `godoo_cli-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gOdoo-cli
-Version: 0.9.4
+Version: 0.9.5
 Summary: Wrapper around Odoo-Bin with some convinience RPC functions.
 Home-page: https://github.com/OpenJKSoftware/gOdoo
 License: LGPL-3
 Keywords: odoo,godoo,devcontainer
 Author: Joshua Kreuder
 Author-email: Joshua_Kreuder@outlook.com
 Requires-Python: >=3.8.1,<3.12
```

