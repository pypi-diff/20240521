# Comparing `tmp/azol-0.2.3b1.tar.gz` & `tmp/azol-0.2.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azol-0.2.3b1.tar", last modified: Wed Apr 24 13:15:28 2024, max compression
+gzip compressed data, was "azol-0.2.4b1.tar", last modified: Tue May 21 19:55:00 2024, max compression
```

## Comparing `azol-0.2.3b1.tar` & `azol-0.2.4b1.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.497771 azol-0.2.3b1/
--rw-r--r--   0 runner    (1001) docker     (127)    35801 2024-04-24 13:15:11.000000 azol-0.2.3b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-24 13:15:28.497771 azol-0.2.3b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-24 13:15:11.000000 azol-0.2.3b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.489771 azol-0.2.3b1/azol/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.489771 azol-0.2.3b1/azol/caches/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/caches/azol_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/caches/in_memory_token_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/caches/local_token_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.489771 azol-0.2.3b1/azol/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44625 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/clients/arm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    33149 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/clients/graph_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/clients/key_vault_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/clients/oauth_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    41909 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.493771 azol-0.2.3b1/azol/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/credentials/access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/credentials/application_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/credentials/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/credentials/entraid_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/credentials/service_principal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/credentials/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.493771 azol-0.2.3b1/azol/models/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/models/generic_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/models/sp_login_init_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.493771 azol-0.2.3b1/azol/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/providers/file_secret_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/providers/key_vault_secret_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.493771 azol-0.2.3b1/azol/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   270913 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/resources/graph_delegated_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)   182559 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/resources/graph_permissions_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    32330 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/resources/rbac_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.493771 azol-0.2.3b1/azol/services/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24848 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/services/token_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    44361 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/services/token_service_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.497771 azol-0.2.3b1/azol/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/utils/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.497771 azol-0.2.3b1/azol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-24 13:15:28.000000 azol-0.2.3b1/azol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-24 13:15:28.000000 azol-0.2.3b1/azol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:15:28.000000 azol-0.2.3b1/azol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 13:15:28.000000 azol-0.2.3b1/azol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 13:15:28.000000 azol-0.2.3b1/azol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 13:15:11.000000 azol-0.2.3b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:15:28.497771 azol-0.2.3b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-24 13:15:11.000000 azol-0.2.3b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:55:00.567666 azol-0.2.4b1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35801 2024-05-21 19:54:50.000000 azol-0.2.4b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-21 19:55:00.567666 azol-0.2.4b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-21 19:54:50.000000 azol-0.2.4b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:55:00.563666 azol-0.2.4b1/azol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:55:00.563666 azol-0.2.4b1/azol/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/caches/azol_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/caches/in_memory_token_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/caches/local_token_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:55:00.563666 azol-0.2.4b1/azol/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44625 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/clients/arm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38194 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/clients/graph_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/clients/key_vault_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/clients/oauth_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   208122 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:55:00.563666 azol-0.2.4b1/azol/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/credentials/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/credentials/application_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/credentials/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/credentials/entraid_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/credentials/service_principal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/credentials/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:55:00.567666 azol-0.2.4b1/azol/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/models/ests_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/models/generic_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/models/sp_login_init_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:55:00.567666 azol-0.2.4b1/azol/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/providers/file_secret_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/providers/key_vault_secret_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:55:00.567666 azol-0.2.4b1/azol/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   270913 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/resources/graph_delegated_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   182559 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/resources/graph_permissions_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32330 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/resources/rbac_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:55:00.567666 azol-0.2.4b1/azol/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25016 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/services/token_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44361 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/services/token_service_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:55:00.567666 azol-0.2.4b1/azol/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/utils/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-21 19:54:50.000000 azol-0.2.4b1/azol/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:55:00.567666 azol-0.2.4b1/azol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-21 19:55:00.000000 azol-0.2.4b1/azol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-21 19:55:00.000000 azol-0.2.4b1/azol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:55:00.000000 azol-0.2.4b1/azol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-21 19:55:00.000000 azol-0.2.4b1/azol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 19:55:00.000000 azol-0.2.4b1/azol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-21 19:54:50.000000 azol-0.2.4b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 19:55:00.567666 azol-0.2.4b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-21 19:54:50.000000 azol-0.2.4b1/setup.py
```

### Comparing `azol-0.2.3b1/LICENSE` & `azol-0.2.4b1/LICENSE`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/PKG-INFO` & `azol-0.2.4b1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azol
-Version: 0.2.3b1
+Version: 0.2.4b1
 Summary: A python-based pentesting library for Azure and Entra ID
 Home-page: https://github.com/cdburkard/azol
 Author: Cody Burkard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: dataclasses==0.6
```

### Comparing `azol-0.2.3b1/README.md` & `azol-0.2.4b1/README.md`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/__init__.py` & `azol-0.2.4b1/azol/__init__.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/caches/azol_cache.py` & `azol-0.2.4b1/azol/caches/azol_cache.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/caches/local_token_cache.py` & `azol-0.2.4b1/azol/caches/local_token_cache.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/clients/arm_client.py` & `azol-0.2.4b1/azol/clients/arm_client.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/clients/graph_client.py` & `azol-0.2.4b1/azol/clients/graph_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A module containing a client for interacting with the Graph API"""
 import logging
 from azol.clients.oauth_http_client import OAuthHTTPClient
-from azol.constants import GRAPHBETAURL, OAuthResourceIDs
+from azol.constants import GRAPHBETAURL, OAuthResourceIDs, roleNameMap, appPermissionNameMap
 
 class GraphRequestFailedException(Exception):
     """
         Exception that is raised when requests to MS Graph
         unexpectedly fail
     """
 
@@ -58,14 +58,134 @@
         """
         response = self._send_request( "/roleManagement/directory/roleDefinitions?"
                                        "$select=displayName,id,isBuiltIn" )
         if response:
             return self._get_all_graph_objects(response)
         raise GraphRequestFailedException()
 
+    def get_access_catalogs_roles( self, catalogId ):
+        """
+            Get all the roles assigned to a specific access catalog
+
+            Args:
+                catalogId - the ID of the catalog
+
+            Returns:
+                A list of dictionaries containing role assignments for the catalog
+
+            Raises:
+                GraphRequestFailedException: An error occurred accessing the Graph API
+
+        """
+        response=self._send_request( f"/roleManagement/entitlementManagement/roleAssignments?$filter=appScopeId eq '/AccessPackageCatalog/{catalogId}'" )
+
+        if response:
+            roles=response.json()["value"]
+            for role in roles:
+                role["azolAnnotations"] = {
+                    "roleName" : roleNameMap[role["roleDefinitionId"]]
+                }
+            return roles
+        raise GraphRequestFailedException()
+
+
+    def create_package_policy( self, policy ):
+        """Create policy for Entitlement Management Pacakge
+
+        Returns:
+            A dictionary containing the entitlement management package policy.
+
+        Args:
+            catalog - dictionary containing entitlement management package policy
+
+        Raises:
+            GraphRequestFailedException: An error occurred accessing the Graph API
+
+        """
+        response=self._send_request( "/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies",
+                                     method="POST", json=policy, success_code=201 )
+
+        if response:
+            return response.json()
+        raise GraphRequestFailedException()
+
+    def create_entitlement_management_package( self, package ):
+        """Create Entitlement Management Pacakge
+
+        Returns:
+            A dictionary containing the entitlement management package.
+
+        Args:
+            catalog - dictionary containing entitlement management package metadata
+
+        Raises:
+            GraphRequestFailedException: An error occurred accessing the Graph API
+
+        """
+        response=self._send_request( "/identityGovernance/entitlementManagement/accessPackages",
+                                     method="POST", json=package, success_code=201 )
+
+        if response:
+            return response.json()
+        raise GraphRequestFailedException()
+
+    def create_entitlement_management_catalog( self, catalog ):
+        """Create Entitlement Management Catalog
+
+        Returns:
+            A list of dictionaries containing all entitlement management catalog.
+
+        Args:
+            catalog - dictionary containing entitlement management catalog metadata
+
+        Raises:
+            GraphRequestFailedException: An error occurred accessing the Graph API
+
+        """
+        response=self._send_request( "/identityGovernance/entitlementManagement/accessPackageCatalogs",
+                                     method="POST", json=catalog, success_code=201 )
+
+        if response:
+            return self._get_all_graph_objects(response)
+        raise GraphRequestFailedException()
+
+    def get_access_packages( self ):
+        """Get Entitlement Management Access Packages.
+
+        Returns:
+            A list of dictionaries containing all entitlement management access packages metadata.
+
+        Raises:
+            GraphRequestFailedException: An error occurred accessing the Graph API
+
+        """
+
+        response=self._send_request( "/identityGovernance/entitlementManagement/accessPackages?$expand=accessPackageCatalog($select=displayName,id,description)" )
+
+        if response:
+            return self._get_all_graph_objects(response)
+        raise GraphRequestFailedException()
+
+    def get_entitlement_management_catalogs( self ):
+        """Get Entitlement Management Catalogs.
+
+        Returns:
+            A list of dictionaries containing entitlement management catalog metadata.
+
+        Raises:
+            GraphRequestFailedException: An error occurred accessing the Graph API
+
+        """
+
+        response=self._send_request( "/identityGovernance/entitlementManagement/accessPackageCatalogs" )
+
+        if response:
+            return self._get_all_graph_objects(response)
+        raise GraphRequestFailedException()
+
     def get_current_pim_eligibility( self ):
         """Get pim eligibility of the current principal.
 
         Returns:
             A list of dictionaries containing the pim eligibility of the current principal.
 
         Raises:
@@ -229,17 +349,17 @@
         Returns:
             A list of dictionaries containing role assignment metadata
 
         Raises:
             GraphRequestFailedException: An error occurred accessing the Graph API
         """
         if object is None:
-            response = self._send_request( "/roleManagement/directory/roleAssignments" )
+            response = self._send_request( "/roleManagement/directory/roleAssignments?$expand=roleDefinition($select=id,displayName)&select=roleDefinition,roleDefinitionId,principalId,resourceScope,principalOrganizationId" )
         else:
-            response = self._send_request( f"/roleManagement/directory/roleAssignments?$count=true&$filter=principalId eq '{object}'" )
+            response = self._send_request( f"/roleManagement/directory/roleAssignments?$expand=roleDefinition($select=id,displayName)&select=roleDefinition,roleDefinitionId,principalId,resourceScope,principalOrganizationId&$count=true&$filter=principalId eq '{object}'" )
         if response:
             return self._get_all_graph_objects(response)
         raise GraphRequestFailedException()
 
     def delete_directory_role_assignments( self, assignment_id ):
         """Remove an Entra ID role from a principal in the directory.
 
@@ -433,15 +553,22 @@
         Raises:
             GraphRequestFailedException: An error occurred accessing the Graph API
         """
         response = self._send_request( "/servicePrincipals?$expand=appRoleAssignments("
                                        "$select=resourceId,resourceDisplayName,principalType,"
                                        "appRoleId)&$select=appRoleAssignments,id,displayName" )
         if response:
-            return self._get_all_graph_objects(response)
+            sps = self._get_all_graph_objects(response)
+            for sp in sps:
+                for ass in sp["appRoleAssignments"]:
+                    from pprint import pprint
+                    ass["azolannotations"] = {
+                        "permissionName": appPermissionNameMap[ass["appRoleId"]]
+                    }
+            return sps
         raise GraphRequestFailedException()
 
     #def get_all_sp_delegated_permissions( self ): # TODO: currently errors
     #    """Get all the API permissions assigned to all service principals.
     #
     #    Returns:
     #       A list of dictionaries with API permissions assigned to all service principal
@@ -497,15 +624,20 @@
            its API permissions 
 
         Raises:
             GraphRequestFailedException: An error occurred accessing the Graph API
         """
         response = self._send_request( f"/servicePrincipals/{sp_object_id}/appRoleAssignments" )
         if response:
-            return self._get_all_graph_objects(response)
+            api_permissions=self._get_all_graph_objects(response)
+            for permission in api_permissions:
+                permission["azolAnnotations"] = {
+                        "permissionName": appPermissionNameMap[permission["appRoleId"]]
+                }
+            return api_permissions
         raise GraphRequestFailedException()
 
     def get_delegated_permissions( self, sp_object_id ):
         """Get all the delegated permissions assigned to a service principal.
 
         Get all the API permissions assigned to a service principal.
```

### Comparing `azol-0.2.3b1/azol/clients/key_vault_client.py` & `azol-0.2.4b1/azol/clients/key_vault_client.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/clients/oauth_http_client.py` & `azol-0.2.4b1/azol/clients/oauth_http_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 class OAuthHTTPClient:
     """
         Base class for OAuth HTTP client objects.
     """
 
     def __init__( self, cred, oauth_resource, base_url,
                   tenant=None, azol_id=None, oauth_flow=None, secrets_provider=None,
-                  use_persistent_cache=True, auto_refresh=True):
+                  use_persistent_cache=True, auto_refresh=True, scopes=[]):
         if tenant is None:
             if cred.credentialType != "user":
                 raise Exception("tenant must be specified if credential is not of type 'user'")
             if not cred.default_oauth_flow=="refresh_token":
                 username=cred.get_username()
                 tenant=username.split("@")[1]
-        self.scopes=[]
+        self.scopes=scopes
         self.default_scope=True
         self.profile_scope=True
         self.openid_scope=True
         self.offline_access_scope=True
         self._baseurl = base_url
 
         self._tenant = tenant
```

### Comparing `azol-0.2.3b1/azol/credentials/access_token.py` & `azol-0.2.4b1/azol/credentials/access_token.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/credentials/application_object.py` & `azol-0.2.4b1/azol/credentials/application_object.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/credentials/credential.py` & `azol-0.2.4b1/azol/credentials/credential.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/credentials/service_principal.py` & `azol-0.2.4b1/azol/credentials/service_principal.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/credentials/user.py` & `azol-0.2.4b1/azol/credentials/user.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 """A module containing the User credential class"""
 import logging
 
 from azol.constants import FOCIClients, known_client_redirect_uris
 from azol.credentials.entraid_credential import EntraIdCredential
+from azol.models.ests_cookie import ESTS
 
 class User( EntraIdCredential ):
     """
         A credential object that may be used when a refresh token is stolen, 
         or a username/password combo is stolen
     """
 
     supportedOAuthFlows = [ "refresh_token", "device_code", "authorization_code" ]
     credentialType="user"
     default_oauth_flow="device_code"
 
-    def __init__( self, username=None, refresh_token=None,
-                  client_id=FOCIClients.MicrosoftAzurePowershell,
-                  redirect_uri=None, 
+    def __init__( self, username=None, refresh_token=None, ests=None,
+                 ests_persistent=None, redirect_uri=None,
+                 client_id=FOCIClients.MicrosoftAzurePowershell,  
                   *args, **kwargs ):
         """
             User objects always have a username, pasword and refresh token. 
             However, sometimes some or all of these are unknown
             during a test. Accept any combo except for password only, 
             and if none are provided, ask the user.
+
+            If an ests cookies is provided, it will be overridden if an ests
+            cookies is also found for the user in the cache. to avoid this, 
+            consider useing use_persistent_cache=False
         """
 
         super().__init__( *args, **kwargs)
         if refresh_token:
             self.default_oauth_flow="refresh_token"
         if username:
             self._username=username.lower()
         else:
             self._username=username
         self._refresh_token=refresh_token
+        self._ests=ests
+        self._ests_persistent=None
 
         self._client_id=client_id
         self._redirect_uri=redirect_uri
 
     def username_is_known( self ):
         """
             Returns True if the username is set on the user object
@@ -44,19 +51,36 @@
             Returns: bool depending on whether the username is set or not
         """
         return False if self._username is None else True
 
     def get_client_id(self):
         return self._client_id
 
+    def has_ests(self):
+        if self._ests is None and self._ests_persistent is None:
+            return False
+        return True
+
     def has_refresh_token(self):
         if self._refresh_token is None:
             return False
         return True
 
+    def get_ests(self):
+        """
+            Get the user's ests and ests_persistent cookies
+    
+            Returns: ESTS object containing ests cookies for the user
+        """
+        cookies=ESTS(
+            ests=self._ests,
+            ests_persistent=self._ests_persistent
+        )
+        return cookies
+
     def get_refresh_token(self):
         """
             Get the current refresh token of the user object
     
             Returns: string containing the raw refresh token, or None
         """
         return self._refresh_token
```

### Comparing `azol-0.2.3b1/azol/models/generic_resource.py` & `azol-0.2.4b1/azol/models/generic_resource.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/providers/file_secret_provider.py` & `azol-0.2.4b1/azol/providers/file_secret_provider.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/providers/key_vault_secret_provider.py` & `azol-0.2.4b1/azol/providers/key_vault_secret_provider.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/resources/graph_delegated_permissions.py` & `azol-0.2.4b1/azol/resources/graph_delegated_permissions.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/resources/graph_permissions_map.py` & `azol-0.2.4b1/azol/resources/graph_permissions_map.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/resources/rbac_roles.py` & `azol-0.2.4b1/azol/resources/rbac_roles.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/services/token_service.py` & `azol-0.2.4b1/azol/services/token_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,21 @@
         self.scopes=scopes
         self.default_scope=default_scope
         self.profile_scope=profile_scope
         self.openid_scope=openid_scope
         self.offline_access_scope=offline_access_scope
         self.ests_cookie=None
         self.ests_persistent_cookie=None
+        if self.credential_object.has_ests():
+            cookies=self.credential_object.get_ests()
+            self.ests_cookie=cookies.ests
+            self.ests_persistent_cookie=cookies.ests_persistent
+        else:
+            self.ests_cookie=None
+            self.ests_persistent_cookie=None
         if self.credential_object.has_refresh_token():
             self._refresh_token=self.credential_object.get_refresh_token()
         else:
             self._refresh_token=None
 
         if self.credential_object.credentialType == "user":
             self.flow_type="delegated"
@@ -371,20 +378,16 @@
         body = {
             "client_id" : client_id,
             "refresh_token": self._refresh_token,
             "scope": extended_scope_string,
             "grant_type": "refresh_token"
         }
 
-        headers={
-            "origin": "http://localhost"
-        }
-
         response = requests.post( "https://login.microsoftonline.com/"
-                                 f"{self._tenant}/oauth2/v2.0/token", data=body, headers=headers, timeout=10 )
+                                 f"{self._tenant}/oauth2/v2.0/token", data=body,  timeout=10 )
         if "error" in response.json().keys():
             error_msg = response.content
             msg_dict = json.loads(error_msg)
             eid_error_code=msg_dict["error_description"].split(":")[0]
             if eid_error_code=="AADSTS50076":
                 # We need to use MFA to switch tenants.
                 # This requires an ESTSAUTH or ESTSPERSISTENTAUTH cookie
@@ -393,15 +396,14 @@
                     new_token_data=ests_login_flow(self._tenant, self.credential_object.get_client_id(),
                                                    self.ests_cookie, self.ests_persistent_cookie, 
                                                    self.credential_object.get_username(),
                                                    extended_scope_string, self.credential_object._redirect_uri)
                     self._refresh_token=new_token_data["refresh_token"]
                     return new_token_data
             else:
-                print(response.request.body)
                 logging.error( "Error: error while refreshing token. "
                             "Raw Error Message from Identity Platform: %s", error_msg )
                 
                 raise IdentityPlatformRequestFailedException()
             
         if "refresh_token" in response.json().keys():
             token = response.json()[ "access_token" ]
```

### Comparing `azol-0.2.3b1/azol/services/token_service_helpers.py` & `azol-0.2.4b1/azol/services/token_service_helpers.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/utils/auth_utils.py` & `azol-0.2.4b1/azol/utils/auth_utils.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol/utils/utils.py` & `azol-0.2.4b1/azol/utils/utils.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.3b1/azol.egg-info/PKG-INFO` & `azol-0.2.4b1/azol.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azol
-Version: 0.2.3b1
+Version: 0.2.4b1
 Summary: A python-based pentesting library for Azure and Entra ID
 Home-page: https://github.com/cdburkard/azol
 Author: Cody Burkard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: dataclasses==0.6
```

### Comparing `azol-0.2.3b1/azol.egg-info/SOURCES.txt` & `azol-0.2.4b1/azol.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 azol/credentials/access_token.py
 azol/credentials/application_object.py
 azol/credentials/credential.py
 azol/credentials/entraid_credential.py
 azol/credentials/service_principal.py
 azol/credentials/user.py
 azol/models/__init__.py
+azol/models/ests_cookie.py
 azol/models/generic_resource.py
 azol/models/sp_login_init_model.py
 azol/providers/__init__.py
 azol/providers/file_secret_provider.py
 azol/providers/key_vault_secret_provider.py
 azol/resources/__init__.py
 azol/resources/graph_delegated_permissions.py
```

### Comparing `azol-0.2.3b1/setup.py` & `azol-0.2.4b1/setup.py`

 * *Files identical despite different names*

