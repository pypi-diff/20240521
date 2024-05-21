# Comparing `tmp/cirro-1.1.2.tar.gz` & `tmp/cirro-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirro-1.1.2.tar", max compression
+gzip compressed data, was "cirro-1.1.3.tar", max compression
```

## Comparing `cirro-1.1.2.tar` & `cirro-1.1.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1066 2024-05-17 00:35:45.145764 cirro-1.1.2/LICENSE.txt
--rw-r--r--   0        0        0     6113 2024-05-17 00:35:45.145764 cirro-1.1.2/README.md
--rw-r--r--   0        0        0      476 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/__init__.py
--rw-r--r--   0        0        0     1486 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/auth/__init__.py
--rw-r--r--   0        0        0      308 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/auth/base.py
--rw-r--r--   0        0        0     6983 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/auth/device_code.py
--rw-r--r--   0        0        0      432 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/auth/oauth_models.py
--rw-r--r--   0        0        0     4470 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cirro_client.py
--rw-r--r--   0        0        0      190 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/__init__.py
--rw-r--r--   0        0        0     2538 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/cli.py
--rw-r--r--   0        0        0     6694 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/controller.py
--rw-r--r--   0        0        0        0 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/interactive/__init__.py
--rw-r--r--   0        0        0     1277 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/interactive/auth_args.py
--rw-r--r--   0        0        0      773 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/interactive/common_args.py
--rw-r--r--   0        0        0     5229 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/interactive/download_args.py
--rw-r--r--   0        0        0      576 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/interactive/list_dataset_args.py
--rw-r--r--   0        0        0     5672 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/interactive/upload_args.py
--rw-r--r--   0        0        0     2801 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/interactive/utils.py
--rw-r--r--   0        0        0      443 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/models.py
--rw-r--r--   0        0        0       68 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/clients/__init__.py
--rw-r--r--   0        0        0     4456 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/clients/s3.py
--rw-r--r--   0        0        0     4335 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/config.py
--rw-r--r--   0        0        0     4033 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/file_utils.py
--rw-r--r--   0        0        0      164 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/helpers/__init__.py
--rw-r--r--   0        0        0     1708 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/helpers/constants.py
--rw-r--r--   0        0        0     5202 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/helpers/form.py
--rw-r--r--   0        0        0     5922 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/helpers/preprocess_dataset.py
--rw-r--r--   0        0        0        0 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/models/__init__.py
--rw-r--r--   0        0        0     3567 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/models/file.py
--rw-r--r--   0        0        0     2607 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/models/form_specification.py
--rw-r--r--   0        0        0      502 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/models/s3_path.py
--rw-r--r--   0        0        0      110 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/models/tenant.py
--rw-r--r--   0        0        0        0 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/__init__.py
--rw-r--r--   0        0        0     2993 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/asset.py
--rw-r--r--   0        0        0     7080 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/dataset.py
--rw-r--r--   0        0        0      245 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/exceptions.py
--rw-r--r--   0        0        0     5496 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/file.py
--rw-r--r--   0        0        0     1536 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/helpers.py
--rw-r--r--   0        0        0     4607 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/portal.py
--rw-r--r--   0        0        0     2230 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/process.py
--rw-r--r--   0        0        0     7733 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/project.py
--rw-r--r--   0        0        0     1823 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/reference.py
--rw-r--r--   0        0        0     1188 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/reference_type.py
--rw-r--r--   0        0        0      593 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/__init__.py
--rw-r--r--   0        0        0      981 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/base.py
--rw-r--r--   0        0        0     1417 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/billing.py
--rw-r--r--   0        0        0     7475 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/dataset.py
--rw-r--r--   0        0        0     4680 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/execution.py
--rw-r--r--   0        0        0     6282 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/file.py
--rw-r--r--   0        0        0     2412 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/metadata.py
--rw-r--r--   0        0        0      831 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/metrics.py
--rw-r--r--   0        0        0     3754 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/process.py
--rw-r--r--   0        0        0     5572 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/projects.py
--rw-r--r--   0        0        0      789 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/references.py
--rw-r--r--   0        0        0      819 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/user.py
--rw-r--r--   0        0        0     1514 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/utils.py
--rw-r--r--   0        0        0      925 2024-05-17 00:35:45.145764 cirro-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     7255 1970-01-01 00:00:00.000000 cirro-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-21 14:35:11.553537 cirro-1.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     6113 2024-05-21 14:35:11.553537 cirro-1.1.3/README.md
+-rw-r--r--   0        0        0      476 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/__init__.py
+-rw-r--r--   0        0        0     1486 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/auth/__init__.py
+-rw-r--r--   0        0        0      308 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/auth/base.py
+-rw-r--r--   0        0        0     6983 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/auth/device_code.py
+-rw-r--r--   0        0        0      432 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/auth/oauth_models.py
+-rw-r--r--   0        0        0     4470 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/cirro_client.py
+-rw-r--r--   0        0        0      190 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/cli/__init__.py
+-rw-r--r--   0        0        0     2538 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/cli/cli.py
+-rw-r--r--   0        0        0     6694 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/cli/controller.py
+-rw-r--r--   0        0        0        0 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/cli/interactive/__init__.py
+-rw-r--r--   0        0        0     1288 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/cli/interactive/auth_args.py
+-rw-r--r--   0        0        0      773 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/cli/interactive/common_args.py
+-rw-r--r--   0        0        0     5229 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/cli/interactive/download_args.py
+-rw-r--r--   0        0        0      576 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/cli/interactive/list_dataset_args.py
+-rw-r--r--   0        0        0     5672 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/cli/interactive/upload_args.py
+-rw-r--r--   0        0        0     2801 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/cli/interactive/utils.py
+-rw-r--r--   0        0        0      443 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/cli/models.py
+-rw-r--r--   0        0        0       68 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/clients/__init__.py
+-rw-r--r--   0        0        0     4456 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/clients/s3.py
+-rw-r--r--   0        0        0     4335 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/config.py
+-rw-r--r--   0        0        0     4033 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/file_utils.py
+-rw-r--r--   0        0        0      164 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/helpers/__init__.py
+-rw-r--r--   0        0        0     1708 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/helpers/constants.py
+-rw-r--r--   0        0        0     5202 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/helpers/form.py
+-rw-r--r--   0        0        0     5922 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/helpers/preprocess_dataset.py
+-rw-r--r--   0        0        0        0 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/models/__init__.py
+-rw-r--r--   0        0        0     3567 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/models/file.py
+-rw-r--r--   0        0        0     2607 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/models/form_specification.py
+-rw-r--r--   0        0        0      502 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/models/s3_path.py
+-rw-r--r--   0        0        0      110 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/models/tenant.py
+-rw-r--r--   0        0        0        0 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/sdk/__init__.py
+-rw-r--r--   0        0        0     2993 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/sdk/asset.py
+-rw-r--r--   0        0        0     7080 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/sdk/dataset.py
+-rw-r--r--   0        0        0      245 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/sdk/exceptions.py
+-rw-r--r--   0        0        0     5496 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/sdk/file.py
+-rw-r--r--   0        0        0     1536 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/sdk/helpers.py
+-rw-r--r--   0        0        0     4607 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/sdk/portal.py
+-rw-r--r--   0        0        0     2230 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/sdk/process.py
+-rw-r--r--   0        0        0     7733 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/sdk/project.py
+-rw-r--r--   0        0        0     1823 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/sdk/reference.py
+-rw-r--r--   0        0        0     1188 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/sdk/reference_type.py
+-rw-r--r--   0        0        0      593 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/services/__init__.py
+-rw-r--r--   0        0        0      981 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/services/base.py
+-rw-r--r--   0        0        0     1417 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/services/billing.py
+-rw-r--r--   0        0        0     7475 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/services/dataset.py
+-rw-r--r--   0        0        0     4680 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/services/execution.py
+-rw-r--r--   0        0        0     6282 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/services/file.py
+-rw-r--r--   0        0        0     2412 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/services/metadata.py
+-rw-r--r--   0        0        0      831 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/services/metrics.py
+-rw-r--r--   0        0        0     3754 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/services/process.py
+-rw-r--r--   0        0        0     5572 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/services/projects.py
+-rw-r--r--   0        0        0      789 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/services/references.py
+-rw-r--r--   0        0        0      819 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/services/user.py
+-rw-r--r--   0        0        0     1514 2024-05-21 14:35:11.553537 cirro-1.1.3/cirro/utils.py
+-rw-r--r--   0        0        0      925 2024-05-21 14:35:11.557537 cirro-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7255 1970-01-01 00:00:00.000000 cirro-1.1.3/PKG-INFO
```

### Comparing `cirro-1.1.2/LICENSE.txt` & `cirro-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/README.md` & `cirro-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/auth/__init__.py` & `cirro-1.1.3/cirro/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/auth/device_code.py` & `cirro-1.1.3/cirro/auth/device_code.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/cirro_client.py` & `cirro-1.1.3/cirro/cirro_client.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/cli/cli.py` & `cirro-1.1.3/cirro/cli/cli.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/cli/controller.py` & `cirro-1.1.3/cirro/cli/controller.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/cli/interactive/auth_args.py` & `cirro-1.1.3/cirro/cli/interactive/auth_args.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     base_url = ask(
         'autocomplete',
         'Enter the URL of the Cirro instance you\'d like to connect to (press TAB for options)',
         choices=[tenant['domain'] for tenant in tenant_options],
         meta_information={tenant['domain']: tenant['displayName'] for tenant in tenant_options}
     )
     # remove http(s):// if it's there
-    base_url = re.compile(r'https?://').sub('', base_url).strip()
+    base_url = re.compile(r'https?://').sub('', base_url).strip('/').strip()
 
     auth_method_config = {
         'enable_cache': ask_yes_no('Would you like to save your login? (do not use this on shared devices)')
     }
 
     enable_additional_checksum = ask(
         'select',
```

### Comparing `cirro-1.1.2/cirro/cli/interactive/common_args.py` & `cirro-1.1.3/cirro/cli/interactive/common_args.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/cli/interactive/download_args.py` & `cirro-1.1.3/cirro/cli/interactive/download_args.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/cli/interactive/list_dataset_args.py` & `cirro-1.1.3/cirro/cli/interactive/list_dataset_args.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/cli/interactive/upload_args.py` & `cirro-1.1.3/cirro/cli/interactive/upload_args.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/cli/interactive/utils.py` & `cirro-1.1.3/cirro/cli/interactive/utils.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/clients/s3.py` & `cirro-1.1.3/cirro/clients/s3.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/config.py` & `cirro-1.1.3/cirro/config.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/file_utils.py` & `cirro-1.1.3/cirro/file_utils.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/helpers/constants.py` & `cirro-1.1.3/cirro/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/helpers/form.py` & `cirro-1.1.3/cirro/helpers/form.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/helpers/preprocess_dataset.py` & `cirro-1.1.3/cirro/helpers/preprocess_dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/models/file.py` & `cirro-1.1.3/cirro/models/file.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/models/form_specification.py` & `cirro-1.1.3/cirro/models/form_specification.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/sdk/asset.py` & `cirro-1.1.3/cirro/sdk/asset.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/sdk/dataset.py` & `cirro-1.1.3/cirro/sdk/dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/sdk/file.py` & `cirro-1.1.3/cirro/sdk/file.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/sdk/helpers.py` & `cirro-1.1.3/cirro/sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/sdk/portal.py` & `cirro-1.1.3/cirro/sdk/portal.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/sdk/process.py` & `cirro-1.1.3/cirro/sdk/process.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/sdk/project.py` & `cirro-1.1.3/cirro/sdk/project.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/sdk/reference.py` & `cirro-1.1.3/cirro/sdk/reference.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/sdk/reference_type.py` & `cirro-1.1.3/cirro/sdk/reference_type.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/services/__init__.py` & `cirro-1.1.3/cirro/services/__init__.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/services/base.py` & `cirro-1.1.3/cirro/services/base.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/services/billing.py` & `cirro-1.1.3/cirro/services/billing.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/services/dataset.py` & `cirro-1.1.3/cirro/services/dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/services/execution.py` & `cirro-1.1.3/cirro/services/execution.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/services/file.py` & `cirro-1.1.3/cirro/services/file.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/services/metadata.py` & `cirro-1.1.3/cirro/services/metadata.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/services/metrics.py` & `cirro-1.1.3/cirro/services/metrics.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/services/process.py` & `cirro-1.1.3/cirro/services/process.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/services/projects.py` & `cirro-1.1.3/cirro/services/projects.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/services/references.py` & `cirro-1.1.3/cirro/services/references.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/services/user.py` & `cirro-1.1.3/cirro/services/user.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/cirro/utils.py` & `cirro-1.1.3/cirro/utils.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.2/pyproject.toml` & `cirro-1.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cirro"
-version = "1.1.2"
+version = "1.1.3"
 description = "CLI tool and SDK for interacting with the Cirro platform"
 authors = ["Cirro Bio <support@cirro.bio>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/CirroBio/Cirro-client"
 packages = [{include = "cirro"}]
```

### Comparing `cirro-1.1.2/PKG-INFO` & `cirro-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirro
-Version: 1.1.2
+Version: 1.1.3
 Summary: CLI tool and SDK for interacting with the Cirro platform
 Home-page: https://github.com/CirroBio/Cirro-client
 License: MIT
 Author: Cirro Bio
 Author-email: support@cirro.bio
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

