# Comparing `tmp/inferless_cli-1.1.6.tar.gz` & `tmp/inferless_cli-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inferless_cli-1.1.6.tar", max compression
+gzip compressed data, was "inferless_cli-1.1.7.tar", max compression
```

## Comparing `inferless_cli-1.1.6.tar` & `inferless_cli-1.1.7.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0    10052 2024-04-29 12:49:54.154706 inferless_cli-1.1.6/README.md
--rw-r--r--   0        0        0       37 2024-05-15 17:36:04.247694 inferless_cli-1.1.6/inferless_cli/__init__.py
--rw-r--r--   0        0        0       50 2024-03-13 03:52:17.953547 inferless_cli-1.1.6/inferless_cli/__main__.py
--rw-r--r--   0        0        0     7282 2024-04-29 12:49:54.155402 inferless_cli-1.1.6/inferless_cli/main.py
--rw-r--r--   0        0        0        0 2024-03-13 03:51:47.516671 inferless_cli-1.1.6/inferless_cli/prompts/__init__.py
--rw-r--r--   0        0        0    23068 2024-04-29 12:49:54.155748 inferless_cli-1.1.6/inferless_cli/prompts/deploy.py
--rw-r--r--   0        0        0     1802 2024-04-29 12:49:54.156043 inferless_cli-1.1.6/inferless_cli/prompts/export.py
--rw-r--r--   0        0        0    11391 2024-04-29 12:49:54.156678 inferless_cli-1.1.6/inferless_cli/prompts/init.py
--rw-r--r--   0        0        0     3779 2024-04-30 07:21:43.512104 inferless_cli-1.1.6/inferless_cli/prompts/log.py
--rw-r--r--   0        0        0      854 2024-03-13 03:51:54.338936 inferless_cli-1.1.6/inferless_cli/prompts/login.py
--rw-r--r--   0        0        0    15846 2024-04-29 12:49:54.157620 inferless_cli-1.1.6/inferless_cli/prompts/model.py
--rw-r--r--   0        0        0    18882 2024-04-29 12:49:54.157892 inferless_cli-1.1.6/inferless_cli/prompts/run.py
--rw-r--r--   0        0        0     5984 2024-04-29 12:49:54.158229 inferless_cli-1.1.6/inferless_cli/prompts/runtime.py
--rw-r--r--   0        0        0     2026 2024-04-29 12:49:54.158392 inferless_cli-1.1.6/inferless_cli/prompts/secret.py
--rw-r--r--   0        0        0     4231 2024-04-29 12:49:54.158770 inferless_cli-1.1.6/inferless_cli/prompts/token.py
--rw-r--r--   0        0        0    22378 2024-04-29 18:01:24.312203 inferless_cli-1.1.6/inferless_cli/prompts/volume.py
--rw-r--r--   0        0        0     1699 2024-04-29 12:49:54.159427 inferless_cli-1.1.6/inferless_cli/prompts/workspace.py
--rw-r--r--   0        0        0        0 2024-03-13 03:52:07.884835 inferless_cli-1.1.6/inferless_cli/utils/__init__.py
--rw-r--r--   0        0        0     2870 2024-04-29 12:49:54.159619 inferless_cli-1.1.6/inferless_cli/utils/api.py
--rw-r--r--   0        0        0    14752 2024-04-29 12:49:54.160026 inferless_cli-1.1.6/inferless_cli/utils/constants.py
--rw-r--r--   0        0        0     1277 2024-05-15 17:23:04.668037 inferless_cli-1.1.6/inferless_cli/utils/convertors.py
--rw-r--r--   0        0        0     7179 2024-04-29 12:49:54.160563 inferless_cli-1.1.6/inferless_cli/utils/credentials.py
--rw-r--r--   0        0        0    29299 2024-05-15 17:35:52.807108 inferless_cli-1.1.6/inferless_cli/utils/helpers.py
--rw-r--r--   0        0        0    26839 2024-04-29 12:49:54.161332 inferless_cli-1.1.6/inferless_cli/utils/services.py
--rw-r--r--   0        0        0     7065 2024-03-13 03:52:15.076191 inferless_cli-1.1.6/inferless_cli/utils/validators.py
--rw-r--r--   0        0        0      671 2024-05-15 17:34:36.026866 inferless_cli-1.1.6/pyproject.toml
--rw-r--r--   0        0        0    11065 1970-01-01 00:00:00.000000 inferless_cli-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0    10052 2024-04-29 12:49:54.154706 inferless_cli-1.1.7/README.md
+-rw-r--r--   0        0        0       37 2024-05-21 06:49:34.982661 inferless_cli-1.1.7/inferless_cli/__init__.py
+-rw-r--r--   0        0        0       50 2024-03-13 03:52:17.953547 inferless_cli-1.1.7/inferless_cli/__main__.py
+-rw-r--r--   0        0        0     7282 2024-04-29 12:49:54.155402 inferless_cli-1.1.7/inferless_cli/main.py
+-rw-r--r--   0        0        0        0 2024-03-13 03:51:47.516671 inferless_cli-1.1.7/inferless_cli/prompts/__init__.py
+-rw-r--r--   0        0        0    23562 2024-05-21 06:49:34.982992 inferless_cli-1.1.7/inferless_cli/prompts/deploy.py
+-rw-r--r--   0        0        0     1802 2024-04-29 12:49:54.156043 inferless_cli-1.1.7/inferless_cli/prompts/export.py
+-rw-r--r--   0        0        0    11391 2024-04-29 12:49:54.156678 inferless_cli-1.1.7/inferless_cli/prompts/init.py
+-rw-r--r--   0        0        0     3779 2024-04-30 07:21:43.512104 inferless_cli-1.1.7/inferless_cli/prompts/log.py
+-rw-r--r--   0        0        0      854 2024-03-13 03:51:54.338936 inferless_cli-1.1.7/inferless_cli/prompts/login.py
+-rw-r--r--   0        0        0    15846 2024-04-29 12:49:54.157620 inferless_cli-1.1.7/inferless_cli/prompts/model.py
+-rw-r--r--   0        0        0    18882 2024-04-29 12:49:54.157892 inferless_cli-1.1.7/inferless_cli/prompts/run.py
+-rw-r--r--   0        0        0     5984 2024-04-29 12:49:54.158229 inferless_cli-1.1.7/inferless_cli/prompts/runtime.py
+-rw-r--r--   0        0        0     2026 2024-04-29 12:49:54.158392 inferless_cli-1.1.7/inferless_cli/prompts/secret.py
+-rw-r--r--   0        0        0     4231 2024-04-29 12:49:54.158770 inferless_cli-1.1.7/inferless_cli/prompts/token.py
+-rw-r--r--   0        0        0    22378 2024-04-29 18:01:24.312203 inferless_cli-1.1.7/inferless_cli/prompts/volume.py
+-rw-r--r--   0        0        0     1699 2024-04-29 12:49:54.159427 inferless_cli-1.1.7/inferless_cli/prompts/workspace.py
+-rw-r--r--   0        0        0        0 2024-03-13 03:52:07.884835 inferless_cli-1.1.7/inferless_cli/utils/__init__.py
+-rw-r--r--   0        0        0     3492 2024-05-21 06:49:34.983395 inferless_cli-1.1.7/inferless_cli/utils/api.py
+-rw-r--r--   0        0        0    14752 2024-04-29 12:49:54.160026 inferless_cli-1.1.7/inferless_cli/utils/constants.py
+-rw-r--r--   0        0        0     1277 2024-05-15 17:23:04.668037 inferless_cli-1.1.7/inferless_cli/utils/convertors.py
+-rw-r--r--   0        0        0     7179 2024-04-29 12:49:54.160563 inferless_cli-1.1.7/inferless_cli/utils/credentials.py
+-rw-r--r--   0        0        0       48 2024-05-21 06:49:34.983775 inferless_cli-1.1.7/inferless_cli/utils/exceptions.py
+-rw-r--r--   0        0        0    29299 2024-05-15 17:35:52.807108 inferless_cli-1.1.7/inferless_cli/utils/helpers.py
+-rw-r--r--   0        0        0    27185 2024-05-21 06:49:34.984106 inferless_cli-1.1.7/inferless_cli/utils/services.py
+-rw-r--r--   0        0        0     7065 2024-03-13 03:52:15.076191 inferless_cli-1.1.7/inferless_cli/utils/validators.py
+-rw-r--r--   0        0        0      671 2024-05-21 06:49:34.984814 inferless_cli-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0    11065 1970-01-01 00:00:00.000000 inferless_cli-1.1.7/PKG-INFO
```

### Comparing `inferless_cli-1.1.6/README.md` & `inferless_cli-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/inferless_cli/main.py` & `inferless_cli-1.1.7/inferless_cli/main.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/inferless_cli/prompts/deploy.py` & `inferless_cli-1.1.7/inferless_cli/prompts/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import time
 import os
 import tempfile
 import typer
 
+from inferless_cli.utils.exceptions import ModelImportException
 from inferless_cli.utils.helpers import (
     create_yaml,
     create_zip_file,
     decrypt_tokens,
     get_current_mode,
     get_default_machine_values,
     is_inferless_yaml_present,
@@ -231,14 +232,23 @@
             # except Exception as e:
             #     rich.print(e)
             #     raise typer.Exit(1)
 
             progress.update(task_id, description="Validating the model...")
             try:
                 _ = start_import_model({"id": model_id})
+
+            except ModelImportException:
+                del config["model_import_id"]
+                create_yaml(config, config_file_name)
+                rich.print(
+                    f"[red]Could'nt find Model Import ID[/red] we have removed the model_import_id from the {config_file_name} file. for the new deployment and run command [blue]`inferless deploy`[/blue]"
+                )
+                raise typer.Exit(1)
+
             except Exception as e:
                 rich.print(e)
                 raise typer.Exit(1)
 
             status, res = poll_model_status(model_id)
             if status == "FAILURE":
                 error_msg = res["model_import"]["import_error"]["message"]
```

### Comparing `inferless_cli-1.1.6/inferless_cli/prompts/export.py` & `inferless_cli-1.1.7/inferless_cli/prompts/export.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/inferless_cli/prompts/init.py` & `inferless_cli-1.1.7/inferless_cli/prompts/init.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/inferless_cli/prompts/log.py` & `inferless_cli-1.1.7/inferless_cli/prompts/log.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/inferless_cli/prompts/login.py` & `inferless_cli-1.1.7/inferless_cli/prompts/login.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/inferless_cli/prompts/model.py` & `inferless_cli-1.1.7/inferless_cli/prompts/model.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/inferless_cli/prompts/run.py` & `inferless_cli-1.1.7/inferless_cli/prompts/run.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/inferless_cli/prompts/runtime.py` & `inferless_cli-1.1.7/inferless_cli/prompts/runtime.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/inferless_cli/prompts/secret.py` & `inferless_cli-1.1.7/inferless_cli/prompts/secret.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/inferless_cli/prompts/token.py` & `inferless_cli-1.1.7/inferless_cli/prompts/token.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/inferless_cli/prompts/volume.py` & `inferless_cli-1.1.7/inferless_cli/prompts/volume.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/inferless_cli/prompts/workspace.py` & `inferless_cli-1.1.7/inferless_cli/prompts/workspace.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/inferless_cli/utils/api.py` & `inferless_cli-1.1.7/inferless_cli/utils/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,14 +73,30 @@
         elif method == "DELETE":
             response = requests.delete(url, headers=headers)
 
         response.raise_for_status()
 
         return response
 
+    except requests.HTTPError as http_err:
+        capture_exception(http_err)
+        flush()
+        # Handle HTTPError specifically
+        error_message = ""
+        if hasattr(response, "json") and callable(response.json):
+            error = response.json()
+            if "reason" in error:
+                error_message = error["reason"]
+            elif "details" in error:
+                error_message = error["details"]
+        else:
+            error_message = "Something went wrong"
+        rich.print(f"Error: [red]{error_message}[/red]")
+        raise requests.HTTPError(error_message, response=response)
+
     except Exception as e:
         capture_exception(e)
         flush()
         error_message = ""
         if hasattr(response, "json") and callable(response.json):
             error = response.json()
             if "reason" in error:
```

### Comparing `inferless_cli-1.1.6/inferless_cli/utils/constants.py` & `inferless_cli-1.1.7/inferless_cli/utils/constants.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/inferless_cli/utils/convertors.py` & `inferless_cli-1.1.7/inferless_cli/utils/convertors.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/inferless_cli/utils/credentials.py` & `inferless_cli-1.1.7/inferless_cli/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/inferless_cli/utils/helpers.py` & `inferless_cli-1.1.7/inferless_cli/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/inferless_cli/utils/services.py` & `inferless_cli-1.1.7/inferless_cli/utils/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from requests.exceptions import HTTPError
 import rich
 import typer
 from inferless_cli.utils.api import make_request
 from inferless_cli.utils.constants import (
     CREATE_VOLUME_URL,
     DELETE_S3_VOLUME_TEMP_DIR,
     DELETE_S3_VOLUME_URL,
@@ -38,14 +39,15 @@
     GET_SIGNED_URL_FOR_MODEL_UPLOAD_URL,
     COMPLETE_MODEL_UPLOAD_URL,
     GET_MODEL_DETAILS_URL,
     GET_MODEL_FULL_DETAILS_URL,
     VALIDATE_GITHUB_URL_PERMISIONS_URL,
 )
 from inferless_cli import __version__
+from inferless_cli.utils.exceptions import ModelImportException
 from inferless_cli.utils.helpers import (
     decrypt_cli_key,
     decrypt_tokens,
     log_exception,
     save_tokens,
     validate_jwt,
 )
@@ -558,14 +560,19 @@
 
 
 def start_import_model(data):
     try:
         response = make_request(START_IMPORT_URL, method="POST", auth=True, data=data)
 
         return response.json()["details"]
+    except HTTPError as http_err:
+        if http_err.response.status_code == 404:
+            raise ModelImportException("Model Import Id not found")
+        log_exception(http_err)
+        raise Exception("Failed to start import model.")
     except Exception as e:
         log_exception(e)
         raise Exception("Failed to start import model.")
 
 
 def get_model_import_details(id):
     try:
```

### Comparing `inferless_cli-1.1.6/inferless_cli/utils/validators.py` & `inferless_cli-1.1.7/inferless_cli/utils/validators.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.6/pyproject.toml` & `inferless_cli-1.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inferless-cli"
-version = "1.1.6"
+version = "1.1.7"
 description = "Inferless - Deploy Machine Learning Models in Minutes."
 authors = ["Naveen <naveen@inferless.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 inferless = "inferless_cli.main:app"
```

### Comparing `inferless_cli-1.1.6/PKG-INFO` & `inferless_cli-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inferless-cli
-Version: 1.1.6
+Version: 1.1.7
 Summary: Inferless - Deploy Machine Learning Models in Minutes.
 Author: Naveen
 Author-email: naveen@inferless.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

