# Comparing `tmp/shipyard_tableau-0.2.2.tar.gz` & `tmp/shipyard_tableau-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_tableau-0.2.2.tar", max compression
+gzip compressed data, was "shipyard_tableau-0.2.3.tar", max compression
```

## Comparing `shipyard_tableau-0.2.2.tar` & `shipyard_tableau-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-05-12 18:48:21.844008 shipyard_tableau-0.2.2/README.md
--rw-r--r--   0        0        0      502 2024-04-26 19:44:56.645691 shipyard_tableau-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-12 18:48:21.844300 shipyard_tableau-0.2.2/shipyard_tableau/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 03:34:57.766724 shipyard_tableau-0.2.2/shipyard_tableau/cli/__init__.py
--rw-r--r--   0        0        0      478 2024-04-26 19:46:17.511014 shipyard_tableau-0.2.2/shipyard_tableau/cli/authtest.py
--rw-r--r--   0        0        0     4860 2024-04-23 15:02:35.316668 shipyard_tableau-0.2.2/shipyard_tableau/cli/download_view.py
--rw-r--r--   0        0        0     1741 2024-03-26 15:34:44.459652 shipyard_tableau-0.2.2/shipyard_tableau/cli/job_status.py
--rw-r--r--   0        0        0     5419 2024-04-01 15:54:40.974367 shipyard_tableau-0.2.2/shipyard_tableau/cli/refresh_resource.py
--rw-r--r--   0        0        0     3435 2024-04-26 19:44:15.239193 shipyard_tableau-0.2.2/shipyard_tableau/tableau.py
--rw-r--r--   0        0        0     9037 2024-03-26 15:35:00.430548 shipyard_tableau-0.2.2/shipyard_tableau/tableau_utils.py
--rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 shipyard_tableau-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-03 22:01:51.349993 shipyard_tableau-0.2.3/README.md
+-rw-r--r--   0        0        0      656 2024-05-21 16:14:58.721562 shipyard_tableau-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-03-06 15:05:20.226023 shipyard_tableau-0.2.3/shipyard_tableau/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-04 01:57:27.597457 shipyard_tableau-0.2.3/shipyard_tableau/cli/__init__.py
+-rw-r--r--   0        0        0      478 2024-04-29 16:36:13.926582 shipyard_tableau-0.2.3/shipyard_tableau/cli/authtest.py
+-rw-r--r--   0        0        0     4860 2024-04-23 14:34:21.445130 shipyard_tableau-0.2.3/shipyard_tableau/cli/download_view.py
+-rw-r--r--   0        0        0     1741 2024-04-18 03:07:13.761918 shipyard_tableau-0.2.3/shipyard_tableau/cli/job_status.py
+-rw-r--r--   0        0        0     5419 2024-04-18 03:07:13.762363 shipyard_tableau-0.2.3/shipyard_tableau/cli/refresh_resource.py
+-rw-r--r--   0        0        0     3484 2024-05-21 15:58:19.565376 shipyard_tableau-0.2.3/shipyard_tableau/tableau.py
+-rw-r--r--   0        0        0     9037 2024-04-18 03:07:13.763110 shipyard_tableau-0.2.3/shipyard_tableau/tableau_utils.py
+-rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 shipyard_tableau-0.2.3/PKG-INFO
```

### Comparing `shipyard_tableau-0.2.2/shipyard_tableau/cli/download_view.py` & `shipyard_tableau-0.2.3/shipyard_tableau/cli/download_view.py`

 * *Files identical despite different names*

### Comparing `shipyard_tableau-0.2.2/shipyard_tableau/cli/job_status.py` & `shipyard_tableau-0.2.3/shipyard_tableau/cli/job_status.py`

 * *Files identical despite different names*

### Comparing `shipyard_tableau-0.2.2/shipyard_tableau/cli/refresh_resource.py` & `shipyard_tableau-0.2.3/shipyard_tableau/cli/refresh_resource.py`

 * *Files identical despite different names*

### Comparing `shipyard_tableau-0.2.2/shipyard_tableau/tableau.py` & `shipyard_tableau-0.2.3/shipyard_tableau/tableau.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 class TableauClient(DataVisualization):
     def __init__(
         self, username: str, password: str, server_url: str, site: str = ""
     ) -> None:
         self.username = username
         self.password = password
         self.server_url = server_url
-        self.site = site
+        self.site = "" if str(site).lower() == "default" else site
 
     def connect(self, sign_in_method="", **kwargs):
         if not sign_in_method:
             logger.debug("No sign in method provided.")
             try:
                 self.connect_username_password()
                 logger.authtest("Successfully connected with username_password")
                 return 0
             except Exception as username_password_error:
-                logger.debug(f"Failed to connect with UN & PW. Message from Tableau Server {username_password_error} \n"
-                             f"Attempting with token...")
+                logger.debug(
+                    f"Failed to connect with UN & PW. Message from Tableau Server {username_password_error} \n"
+                    f"Attempting with token..."
+                )
                 try:
                     self.connect_access_token()
                     logger.authtest("Successfully connected with Access Token")
                     return 0
                 except Exception as token_error:
                     logger.debug(f"Failed to connect with token: {token_error}")
                     logger.authtest(
@@ -53,17 +55,15 @@
             logger.authtest(f"Could not connect to Tableau: {error}")
             return 1
         logger.authtest("Successfully connected to Tableau")
         return 0
 
     def connect_username_password(self):
         logger.debug("Attempting to Tableau with username and password")
-        tableau_auth = tsc.TableauAuth(
-            self.username, self.password, site_id=self.site
-        )
+        tableau_auth = tsc.TableauAuth(self.username, self.password, site_id=self.site)
         server = tsc.Server(self.server_url, use_server_version=True)
         server.auth.sign_in(tableau_auth)
         logger.debug("Successfully connected to Tableau with username and password")
         return server
 
     def connect_access_token(self):
         logger.debug("Attempting to connect to Tableau with token...")
```

### Comparing `shipyard_tableau-0.2.2/shipyard_tableau/tableau_utils.py` & `shipyard_tableau-0.2.3/shipyard_tableau/tableau_utils.py`

 * *Files identical despite different names*

### Comparing `shipyard_tableau-0.2.2/PKG-INFO` & `shipyard_tableau-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-tableau
-Version: 0.2.2
+Version: 0.2.3
 Summary: A local client for connecting and working with Tableau
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

