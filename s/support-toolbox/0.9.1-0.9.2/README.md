# Comparing `tmp/support-toolbox-0.9.1.tar.gz` & `tmp/support-toolbox-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "support-toolbox-0.9.1.tar", last modified: Tue May 14 02:45:18 2024, max compression
+gzip compressed data, was "support-toolbox-0.9.2.tar", last modified: Tue May 21 13:55:28 2024, max compression
```

## Comparing `support-toolbox-0.9.1.tar` & `support-toolbox-0.9.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:18.458542 support-toolbox-0.9.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-05-14 02:45:18.458542 support-toolbox-0.9.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2495 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-14 02:45:18.462542 support-toolbox-0.9.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:18.450542 support-toolbox-0.9.1/support_toolbox/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:18.458542 support-toolbox-0.9.1/support_toolbox/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4294 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/entitlements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      615 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2549 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/org.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1338 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/project.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3675 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/service_account.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2206 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/site.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1853 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/user.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:18.458542 support-toolbox-0.9.1/support_toolbox/app_handler/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/app_handler/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1195 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/app_handler/app.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/app_handler/app_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      761 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/app_handler/auto_updater.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/app_handler/token_manager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3845 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/clear_user_layer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4590 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/delete_users.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2208 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/deploy_browse_card.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1355 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/deploy_ctk_service_account.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5379 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/deploy_integrations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18802 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/deploy_pi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      294 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2728 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/onboard_ctk_orgs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2158 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/revert_soft_delete.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1319 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/update_saml.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:18.458542 support-toolbox-0.9.1/support_toolbox/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1969 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/utils/api_url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/utils/csv_to_iris.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6258 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/utils/metrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1337 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/utils/resource_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/utils/saml_parser.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:18.458542 support-toolbox-0.9.1/support_toolbox.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-05-14 02:45:18.000000 support-toolbox-0.9.1/support_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1331 2024-05-14 02:45:18.000000 support-toolbox-0.9.1/support_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-14 02:45:18.000000 support-toolbox-0.9.1/support_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2024-05-14 02:45:18.000000 support-toolbox-0.9.1/support_toolbox.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2024-05-14 02:45:18.000000 support-toolbox-0.9.1/support_toolbox.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-05-14 02:45:18.000000 support-toolbox-0.9.1/support_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-21 13:55:28.615996 support-toolbox-0.9.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-05-21 13:55:28.615996 support-toolbox-0.9.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2495 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-21 13:55:28.615996 support-toolbox-0.9.2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-21 13:55:28.611996 support-toolbox-0.9.2/support_toolbox/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-21 13:55:28.611996 support-toolbox-0.9.2/support_toolbox/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/api/dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4294 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/api/entitlements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      615 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/api/file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2549 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/api/org.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1338 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/api/project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3675 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/api/service_account.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2206 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/api/site.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1853 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/api/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-21 13:55:28.611996 support-toolbox-0.9.2/support_toolbox/app_handler/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/app_handler/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1195 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/app_handler/app.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/app_handler/app_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      761 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/app_handler/auto_updater.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/app_handler/token_manager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3845 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/clear_user_layer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4590 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/delete_users.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2208 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/deploy_browse_card.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1355 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/deploy_ctk_service_account.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5379 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/deploy_integrations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18802 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/deploy_pi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      294 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2728 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/onboard_ctk_orgs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2100 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/revert_soft_delete.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1319 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/update_saml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-21 13:55:28.615996 support-toolbox-0.9.2/support_toolbox/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1969 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/utils/api_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/utils/csv_to_iris.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6258 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/utils/metrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1337 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/utils/resource_type.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2024-05-21 13:55:21.000000 support-toolbox-0.9.2/support_toolbox/utils/saml_parser.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-21 13:55:28.615996 support-toolbox-0.9.2/support_toolbox.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-05-21 13:55:28.000000 support-toolbox-0.9.2/support_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1331 2024-05-21 13:55:28.000000 support-toolbox-0.9.2/support_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-21 13:55:28.000000 support-toolbox-0.9.2/support_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2024-05-21 13:55:28.000000 support-toolbox-0.9.2/support_toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2024-05-21 13:55:28.000000 support-toolbox-0.9.2/support_toolbox.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-05-21 13:55:28.000000 support-toolbox-0.9.2/support_toolbox.egg-info/top_level.txt
```

### Comparing `support-toolbox-0.9.1/PKG-INFO` & `support-toolbox-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: support-toolbox
-Version: 0.9.1
+Version: 0.9.2
 Summary: A suite of CLI tools for the data.world support team
 Home-page: https://github.com/datadotworld/support-toolbox/tree/main
 Author: Jack Compton
 Author-email: jack.compton@data.world
 Requires-Dist: certifi==2023.7.22
 Requires-Dist: charset-normalizer==3.2.0
 Requires-Dist: defusedxml==0.7.1
```

### Comparing `support-toolbox-0.9.1/README.md` & `support-toolbox-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/setup.py` & `support-toolbox-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/api/dataset.py` & `support-toolbox-0.9.2/support_toolbox/api/dataset.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/api/entitlements.py` & `support-toolbox-0.9.2/support_toolbox/api/entitlements.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/api/file.py` & `support-toolbox-0.9.2/support_toolbox/api/file.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/api/org.py` & `support-toolbox-0.9.2/support_toolbox/api/org.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/api/project.py` & `support-toolbox-0.9.2/support_toolbox/api/project.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/api/service_account.py` & `support-toolbox-0.9.2/support_toolbox/api/service_account.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/api/site.py` & `support-toolbox-0.9.2/support_toolbox/api/site.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/api/user.py` & `support-toolbox-0.9.2/support_toolbox/api/user.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/app_handler/app.py` & `support-toolbox-0.9.2/support_toolbox/app_handler/app.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/app_handler/auto_updater.py` & `support-toolbox-0.9.2/support_toolbox/app_handler/auto_updater.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/app_handler/token_manager.py` & `support-toolbox-0.9.2/support_toolbox/app_handler/token_manager.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/clear_user_layer.py` & `support-toolbox-0.9.2/support_toolbox/clear_user_layer.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/delete_users.py` & `support-toolbox-0.9.2/support_toolbox/delete_users.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/deploy_browse_card.py` & `support-toolbox-0.9.2/support_toolbox/deploy_browse_card.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/deploy_ctk_service_account.py` & `support-toolbox-0.9.2/support_toolbox/deploy_ctk_service_account.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/deploy_integrations.py` & `support-toolbox-0.9.2/support_toolbox/deploy_integrations.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/deploy_pi.py` & `support-toolbox-0.9.2/support_toolbox/deploy_pi.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/onboard_ctk_orgs.py` & `support-toolbox-0.9.2/support_toolbox/onboard_ctk_orgs.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/revert_soft_delete.py` & `support-toolbox-0.9.2/support_toolbox/revert_soft_delete.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,19 +8,15 @@
 # Revert soft delete for a resource
 def revert_soft_delete(admin_token, org, iri, resource_type, customer_url):
     url = f"{customer_url}/editActivities/{org}/ddw-catalogs"
 
     header = {
         'Accept': 'application/json',
         'Content-Type': 'application/json',
-        'Authorization': f'Bearer {admin_token}'
-    }
-
-    cookies = {
-        'adminToken': admin_token
+        'Cookie': f'token={admin_token};adminToken={admin_token}'
     }
 
     resource_data = {
         "changeMessage": "Revert deleted resources",
         "activities": [{
             "type": "RevertSoftDelete",
             "entityType": resource_type,
@@ -29,26 +25,26 @@
             "type": "RevertSoftDelete",
             "entityType": resource_type,
             "target": iri
         }]
     }
 
     body = json.dumps(resource_data)
-    response = requests.post(url, body, cookies=cookies, headers=header)
+    response = requests.post(url, body, headers=header)
 
     # Verify the revert
     if response.status_code == 200:
         print(f"Successfully reverted soft delete for: {iri}")
     else:
         print(response.text)
 
 
 def run():
     api_url = select_api_url("private")
-    admin_token = input("Enter your active admin token for the selected customer: ")
+    admin_token = input("Enter your active adminToken for the selected customer: ")
     org = input("Enter the org ID where the resource is located: ")
 
     # Allow the user to input multiple IRIs as a comma-separated list or specify a CSV file path
     iris_input = input("Enter the resource IRIs (comma-separated) or specify a CSV file path: ")
 
     if iris_input.endswith('.csv'):
         # User provided a CSV file path, read and process it
```

### Comparing `support-toolbox-0.9.1/support_toolbox/update_saml.py` & `support-toolbox-0.9.2/support_toolbox/update_saml.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/utils/api_url.py` & `support-toolbox-0.9.2/support_toolbox/utils/api_url.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/utils/metrics.py` & `support-toolbox-0.9.2/support_toolbox/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/utils/resource_type.py` & `support-toolbox-0.9.2/support_toolbox/utils/resource_type.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox/utils/saml_parser.py` & `support-toolbox-0.9.2/support_toolbox/utils/saml_parser.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.1/support_toolbox.egg-info/PKG-INFO` & `support-toolbox-0.9.2/support_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: support-toolbox
-Version: 0.9.1
+Version: 0.9.2
 Summary: A suite of CLI tools for the data.world support team
 Home-page: https://github.com/datadotworld/support-toolbox/tree/main
 Author: Jack Compton
 Author-email: jack.compton@data.world
 Requires-Dist: certifi==2023.7.22
 Requires-Dist: charset-normalizer==3.2.0
 Requires-Dist: defusedxml==0.7.1
```

### Comparing `support-toolbox-0.9.1/support_toolbox.egg-info/SOURCES.txt` & `support-toolbox-0.9.2/support_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

