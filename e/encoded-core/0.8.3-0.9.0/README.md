# Comparing `tmp/encoded_core-0.8.3.tar.gz` & `tmp/encoded_core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encoded_core-0.8.3.tar", max compression
+gzip compressed data, was "encoded_core-0.9.0.tar", max compression
```

## Comparing `encoded_core-0.8.3.tar` & `encoded_core-0.9.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
--rw-r--r--   0        0        0     1083 2024-03-26 16:15:26.289695 encoded_core-0.8.3/LICENSE
--rw-r--r--   0        0        0      174 2024-03-26 16:15:26.293695 encoded_core-0.8.3/README.rst
--rw-r--r--   0        0        0     3778 2024-03-26 16:15:26.293695 encoded_core-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     2324 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/__init__.py
--rw-r--r--   0        0        0    31432 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/file_views.py
--rw-r--r--   0        0        0     4847 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/local_roles.py
--rw-r--r--   0        0        0    12807 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/page_views.py
--rw-r--r--   0        0        0      280 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/project_defs.py
--rw-r--r--   0        0        0     2490 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/qc_views.py
--rw-r--r--   0        0        0     1659 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/document.json
--rw-r--r--   0        0        0    14606 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/file.json
--rw-r--r--   0        0        0     4982 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/file_format.json
--rw-r--r--   0        0        0     4751 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/file_processed.json
--rw-r--r--   0        0        0     2161 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/file_reference.json
--rw-r--r--   0        0        0     1205 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/file_submitted.json
--rw-r--r--   0        0        0     1812 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/higlass_view_config.json
--rw-r--r--   0        0        0     1296 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/image.json
--rw-r--r--   0        0        0    13842 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/meta_workflow.json
--rw-r--r--   0        0        0    13367 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/meta_workflow_run.json
--rw-r--r--   0        0        0    16691 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/mixins.json
--rw-r--r--   0        0        0     5014 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/page.json
--rw-r--r--   0        0        0     1460 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/quality_metric.json
--rw-r--r--   0        0        0     3196 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/quality_metric_generic.json
--rw-r--r--   0        0        0     5660 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/software.json
--rw-r--r--   0        0        0     5340 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/static_section.json
--rw-r--r--   0        0        0    20417 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/tracking_item.json
--rw-r--r--   0        0        0     3396 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/user_content.json
--rw-r--r--   0        0        0    27190 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/workflow.json
--rw-r--r--   0        0        0    10478 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/workflow_run.json
--rw-r--r--   0        0        0     1914 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/schemas/workflow_run_awsem.json
--rw-r--r--   0        0        0        0 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/tests/__init__.py
--rw-r--r--   0        0        0    14054 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/tests/conftest.py
--rw-r--r--   0        0        0     1873 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/tests/conftest_settings.py
--rw-r--r--   0        0        0     7726 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/tests/datafixtures.py
--rw-r--r--   0        0        0    11010 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/tests/test_types_file.py
--rw-r--r--   0        0        0      262 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/tests/test_types_file_format.py
--rw-r--r--   0        0        0      239 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/tests/test_types_meta_workflow.py
--rw-r--r--   0        0        0      212 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/tests/test_types_software.py
--rw-r--r--   0        0        0      502 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/tests/test_types_workflow.py
--rw-r--r--   0        0        0       70 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/types/__init__.py
--rw-r--r--   0        0        0     1284 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/types/document.py
--rw-r--r--   0        0        0    20341 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/types/file.py
--rw-r--r--   0        0        0      789 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/types/file_format.py
--rw-r--r--   0        0        0     2297 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/types/file_processed.py
--rw-r--r--   0        0        0      462 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/types/file_reference.py
--rw-r--r--   0        0        0     1970 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/types/file_submitted.py
--rw-r--r--   0        0        0      584 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/types/higlass_view_config.py
--rw-r--r--   0        0        0     1040 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/types/image.py
--rw-r--r--   0        0        0     3217 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/types/meta_workflow.py
--rw-r--r--   0        0        0      858 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/types/page.py
--rw-r--r--   0        0        0     1314 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/types/quality_metric.py
--rw-r--r--   0        0        0      479 2024-03-26 16:15:26.293695 encoded_core-0.8.3/src/encoded_core/types/quality_metric_generic.py
--rw-r--r--   0        0        0     2750 2024-03-26 16:15:26.297695 encoded_core-0.8.3/src/encoded_core/types/software.py
--rw-r--r--   0        0        0     3847 2024-03-26 16:15:26.297695 encoded_core-0.8.3/src/encoded_core/types/tracking_item.py
--rw-r--r--   0        0        0     5468 2024-03-26 16:15:26.297695 encoded_core-0.8.3/src/encoded_core/types/user_content.py
--rw-r--r--   0        0        0    12886 2024-03-26 16:15:26.297695 encoded_core-0.8.3/src/encoded_core/types/workflow.py
--rw-r--r--   0        0        0     1522 2024-03-26 16:15:26.297695 encoded_core-0.8.3/src/encoded_core/upgrade.py
--rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 encoded_core-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-05-21 19:06:45.943839 encoded_core-0.9.0/LICENSE
+-rw-r--r--   0        0        0      174 2024-05-21 19:06:45.943839 encoded_core-0.9.0/README.rst
+-rw-r--r--   0        0        0     3778 2024-05-21 19:06:45.943839 encoded_core-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2683 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/__init__.py
+-rw-r--r--   0        0        0    32944 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/file_views.py
+-rw-r--r--   0        0        0     4847 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/local_roles.py
+-rw-r--r--   0        0        0    12807 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/page_views.py
+-rw-r--r--   0        0        0      280 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/project_defs.py
+-rw-r--r--   0        0        0     2490 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/qc_views.py
+-rw-r--r--   0        0        0     1659 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/document.json
+-rw-r--r--   0        0        0    14606 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/file.json
+-rw-r--r--   0        0        0     4982 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/file_format.json
+-rw-r--r--   0        0        0     4751 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/file_processed.json
+-rw-r--r--   0        0        0     2161 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/file_reference.json
+-rw-r--r--   0        0        0     1205 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/file_submitted.json
+-rw-r--r--   0        0        0     1812 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/higlass_view_config.json
+-rw-r--r--   0        0        0     1296 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/image.json
+-rw-r--r--   0        0        0    13842 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/meta_workflow.json
+-rw-r--r--   0        0        0    13367 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/meta_workflow_run.json
+-rw-r--r--   0        0        0    16691 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/mixins.json
+-rw-r--r--   0        0        0     5014 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/page.json
+-rw-r--r--   0        0        0     1460 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/quality_metric.json
+-rw-r--r--   0        0        0     3196 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/quality_metric_generic.json
+-rw-r--r--   0        0        0     5660 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/software.json
+-rw-r--r--   0        0        0     5340 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/static_section.json
+-rw-r--r--   0        0        0    20417 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/tracking_item.json
+-rw-r--r--   0        0        0     3396 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/user_content.json
+-rw-r--r--   0        0        0    27190 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/workflow.json
+-rw-r--r--   0        0        0    10478 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/workflow_run.json
+-rw-r--r--   0        0        0     1914 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/schemas/workflow_run_awsem.json
+-rw-r--r--   0        0        0        0 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/tests/__init__.py
+-rw-r--r--   0        0        0    14054 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/tests/conftest.py
+-rw-r--r--   0        0        0     1873 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/tests/conftest_settings.py
+-rw-r--r--   0        0        0     7736 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/tests/datafixtures.py
+-rw-r--r--   0        0        0     2171 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/tests/test_download_cli.py
+-rw-r--r--   0        0        0    11010 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/tests/test_types_file.py
+-rw-r--r--   0        0        0      262 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/tests/test_types_file_format.py
+-rw-r--r--   0        0        0      239 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/tests/test_types_meta_workflow.py
+-rw-r--r--   0        0        0      212 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/tests/test_types_software.py
+-rw-r--r--   0        0        0      502 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/tests/test_types_workflow.py
+-rw-r--r--   0        0        0       70 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/types/__init__.py
+-rw-r--r--   0        0        0     1284 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/types/document.py
+-rw-r--r--   0        0        0    20541 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/types/file.py
+-rw-r--r--   0        0        0      789 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/types/file_format.py
+-rw-r--r--   0        0        0     2297 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/types/file_processed.py
+-rw-r--r--   0        0        0      462 2024-05-21 19:06:45.943839 encoded_core-0.9.0/src/encoded_core/types/file_reference.py
+-rw-r--r--   0        0        0     1970 2024-05-21 19:06:45.947839 encoded_core-0.9.0/src/encoded_core/types/file_submitted.py
+-rw-r--r--   0        0        0      584 2024-05-21 19:06:45.947839 encoded_core-0.9.0/src/encoded_core/types/higlass_view_config.py
+-rw-r--r--   0        0        0     1040 2024-05-21 19:06:45.947839 encoded_core-0.9.0/src/encoded_core/types/image.py
+-rw-r--r--   0        0        0     3217 2024-05-21 19:06:45.947839 encoded_core-0.9.0/src/encoded_core/types/meta_workflow.py
+-rw-r--r--   0        0        0      858 2024-05-21 19:06:45.947839 encoded_core-0.9.0/src/encoded_core/types/page.py
+-rw-r--r--   0        0        0     1314 2024-05-21 19:06:45.947839 encoded_core-0.9.0/src/encoded_core/types/quality_metric.py
+-rw-r--r--   0        0        0      479 2024-05-21 19:06:45.947839 encoded_core-0.9.0/src/encoded_core/types/quality_metric_generic.py
+-rw-r--r--   0        0        0     2750 2024-05-21 19:06:45.947839 encoded_core-0.9.0/src/encoded_core/types/software.py
+-rw-r--r--   0        0        0     3847 2024-05-21 19:06:45.947839 encoded_core-0.9.0/src/encoded_core/types/tracking_item.py
+-rw-r--r--   0        0        0     5468 2024-05-21 19:06:45.947839 encoded_core-0.9.0/src/encoded_core/types/user_content.py
+-rw-r--r--   0        0        0    12886 2024-05-21 19:06:45.947839 encoded_core-0.9.0/src/encoded_core/types/workflow.py
+-rw-r--r--   0        0        0     1522 2024-05-21 19:06:45.947839 encoded_core-0.9.0/src/encoded_core/upgrade.py
+-rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 encoded_core-0.9.0/PKG-INFO
```

### Comparing `encoded_core-0.8.3/LICENSE` & `encoded_core-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/pyproject.toml` & `encoded_core-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encoded-core"
-version = "0.8.3"
+version = "0.9.0"
 description = "Core data models for Park Lab ENCODE based projects"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/smaht-dac/encoded-core"
 repository = "https://github.com/smaht-dac/encoded-core"
 documentation = "https://github.com/smaht-dac/encoded-core"
```

### Comparing `encoded_core-0.8.3/src/encoded_core/__init__.py` & `encoded_core-0.9.0/src/encoded_core/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
+import netaddr
 from pyramid.config import Configurator
 from pyramid.settings import asbool
 
-from snovault.app import session, configure_dbsession
+from snovault.app import session, configure_dbsession, json_from_path
 from snovault.elasticsearch import APP_FACTORY
 from snovault.elasticsearch.interfaces import INVALIDATION_SCOPE_ENABLED
 from .local_roles import LocalRolesAuthorizationPolicy
 
 
 APP_VERSION_REGISTRY_KEY = 'encoded-core.app_version'
 
@@ -15,14 +16,20 @@
     if not config.registry.settings.get(APP_VERSION_REGISTRY_KEY):
         # we update version as part of deployment process `deploy_beanstalk.py`
         # but if we didn't check env then git
         version = os.environ.get("ENCODED_VERSION", "test")
         config.registry.settings[APP_VERSION_REGISTRY_KEY] = version
 
 
+def setup_aws_ip_ranges(config, settings):
+    aws_ip_ranges = json_from_path(settings.get('aws_ip_ranges_path'), {'prefixes': []})
+    config.registry['aws_ipset'] = netaddr.IPSet(
+        record['ip_prefix'] for record in aws_ip_ranges['prefixes'] if record['service'] == 'AMAZON')
+
+
 def main(global_config, **local_config):
     """ Returns a pyramid wsgi application that can be used as encoded-core - should only
         be used in testing
     """
     settings = global_config
     settings.update(local_config)
 
@@ -56,10 +63,11 @@
 
     if asbool(settings.get('testing', False)):
         config.include('snovault.tests.testing_views')
         config.include('snovault.root')
 
     config.include('.upgrade')
     config.scan()
+    setup_aws_ip_ranges(config, settings)
 
     app = config.make_wsgi_app()
     return app
```

### Comparing `encoded_core-0.8.3/src/encoded_core/file_views.py` & `encoded_core-0.9.0/src/encoded_core/file_views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import json
 import os
 import pytz
 import requests
 import structlog
 from typing import Any, Dict, List
-
+from dcicutils.misc_utils import ignored
 from pyramid.httpexceptions import (
     HTTPForbidden,
     HTTPTemporaryRedirect,
     HTTPNotFound,
 )
 from pyramid.response import Response
 from pyramid.settings import asbool
@@ -48,14 +48,52 @@
 log = structlog.getLogger(__name__)
 
 
 def includeme(config):
     config.scan(__name__)
 
 
+def extract_bucket_and_key(url: str) -> (str, str):
+    """ Takes an HTTPS URL to S3 and extracts the bucket and key """
+    parsed_url = urlparse(url)
+    bucket = parsed_url.netloc.split('.')[0]
+    key = parsed_url.path.strip('/')
+    if '?' in key:  # remove query params
+        key = key.split('?', 1)[0]
+    return bucket, key
+
+
+def generate_creds(e: HTTPTemporaryRedirect) -> dict:
+    """ Processes HTTPTemporary redirect response from the app, grabbing the bucket/key
+        and calling external_creds with upload=False
+    """
+    url = e.location
+    bucket, key = extract_bucket_and_key(url)
+    return external_creds(bucket, key, name=f'DownloadCredentials', upload=False)
+
+
+@view_config(name='download_cli', context=File, permission='view', request_method=['GET'])
+@debug_log
+def download_cli(context, request):
+    """ Runs the external_creds function with upload=False assuming user passes auth check """
+    ignored(context)
+    path = request.path
+    # Direct to @@download to track via GA and run perm check
+    try:  # this call will raise HTTPTemporary redirect if successful
+        uri = path.replace('@@download_cli', '@@download')
+        request.embed(uri, as_user=True)
+    except HTTPTemporaryRedirect as e:
+        return generate_creds(e)
+    except Exception as e:
+        msg = f'Error encountered with /embed {e}'
+        log.error(msg)
+        return Response(msg, status=400)
+    return Response('Could not retrieve creds', status=400)
+
+
 @view_config(name='upload', context=File, request_method='GET',
              permission='edit')
 @debug_log
 def get_upload(context, request):
     external = context.propsheets.get('external', {})
     upload_credentials = external.get('upload_credentials')
     # Show s3 location info for files originally submitted to EDW.
@@ -261,15 +299,15 @@
     # try:
     #     TrackingItem.create_and_commit(request, tracking_item, clean_headers=True)
     # except Exception as e:
     #     log.error('Cannot create TrackingItem on download of %s' % context.uuid, error=str(e))
 
     # Analytics Stuff
     ga_config = request.registry.settings.get('ga_config')
-    
+
     if ga_config:
         submitter_title = get_submitter_title(request, context, properties)
         exp_or_assay_type = get_experiment_or_assay_type(request, context, properties)
         file_type = get_file_type(request, context, properties)
         file_at_id = context.jsonld_id(request)
         update_google_analytics(context, request, ga_config, filename, file_size_downloaded, file_at_id, submitter_title,
                                 user_uuid, user_groups, exp_or_assay_type, file_type)
@@ -301,44 +339,46 @@
     # both aws and non-aws users.
     if use_download_proxy:
         location = request.registry.settings.get('download_proxy', '') + str(location)
 
     # 307 redirect specifies to keep original method
     raise HTTPTemporaryRedirect(location=location)
 
+
 def get_submitter_title(request, context, properties):
     submitter = None
     if properties.get('lab') is not None:
         submitter = get_item_or_none(request, properties.get('lab'), 'labs')
     elif properties.get('sequencing_center') is not None:
         submitter = get_item_or_none(request, properties.get('sequencing_center'), 'submission-centers')
     # elif properties.get('submission_centers') is not None and len(properties.get('submission_centers')) > 0:
     #     submitter = get_item_or_none(request, properties.get('submission_centers')[0], 'submission-centers')
 
     return submitter and submitter.get('display_title')
 
 
 def get_experiment_or_assay_type(request, context, properties):
     # SMaHT
-    if properties.get('file_sets') is not None: 
+    if properties.get('file_sets') is not None:
         if len(properties.get('file_sets')) > 0:
             file_set = get_item_or_none(request, properties.get('file_sets')[0], 'file-sets', frame='embedded')
             if file_set is not None and file_set.get('assay'):
                 return file_set['assay'].get('display_title')
     # 4DN
     elif properties.get('track_and_facet_info') is None:
         file_item = get_item_or_none(request, context.uuid)
         if file_item is not None and file_item.get('track_and_facet_info') and file_item['track_and_facet_info'].get('experiment_type'):
             return file_item['track_and_facet_info']['experiment_type']
     # fallback
     return None
 
+
 def get_file_type(request, context, properties):
     # SMaHT
-    if properties.get('data_category') is not None: 
+    if properties.get('data_category') is not None:
         if len(properties.get('data_category')) > 0:
             return properties.get('data_category')[0]
     # 4DN/fallback
     return properties.get('file_type') or 'other'
 
 
 def update_google_analytics(context, request, ga_config, filename, file_size_downloaded,
```

### Comparing `encoded_core-0.8.3/src/encoded_core/local_roles.py` & `encoded_core-0.9.0/src/encoded_core/local_roles.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/page_views.py` & `encoded_core-0.9.0/src/encoded_core/page_views.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/qc_views.py` & `encoded_core-0.9.0/src/encoded_core/qc_views.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/document.json` & `encoded_core-0.9.0/src/encoded_core/schemas/document.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/file.json` & `encoded_core-0.9.0/src/encoded_core/schemas/file.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/file_format.json` & `encoded_core-0.9.0/src/encoded_core/schemas/file_format.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/file_processed.json` & `encoded_core-0.9.0/src/encoded_core/schemas/file_processed.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/file_reference.json` & `encoded_core-0.9.0/src/encoded_core/schemas/file_reference.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/file_submitted.json` & `encoded_core-0.9.0/src/encoded_core/schemas/file_submitted.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/higlass_view_config.json` & `encoded_core-0.9.0/src/encoded_core/schemas/higlass_view_config.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/image.json` & `encoded_core-0.9.0/src/encoded_core/schemas/image.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/meta_workflow.json` & `encoded_core-0.9.0/src/encoded_core/schemas/meta_workflow.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/meta_workflow_run.json` & `encoded_core-0.9.0/src/encoded_core/schemas/meta_workflow_run.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/mixins.json` & `encoded_core-0.9.0/src/encoded_core/schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/page.json` & `encoded_core-0.9.0/src/encoded_core/schemas/page.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/quality_metric.json` & `encoded_core-0.9.0/src/encoded_core/schemas/quality_metric.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/quality_metric_generic.json` & `encoded_core-0.9.0/src/encoded_core/schemas/quality_metric_generic.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/software.json` & `encoded_core-0.9.0/src/encoded_core/schemas/software.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/static_section.json` & `encoded_core-0.9.0/src/encoded_core/schemas/static_section.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/tracking_item.json` & `encoded_core-0.9.0/src/encoded_core/schemas/tracking_item.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/user_content.json` & `encoded_core-0.9.0/src/encoded_core/schemas/user_content.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/workflow.json` & `encoded_core-0.9.0/src/encoded_core/schemas/workflow.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/workflow_run.json` & `encoded_core-0.9.0/src/encoded_core/schemas/workflow_run.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/schemas/workflow_run_awsem.json` & `encoded_core-0.9.0/src/encoded_core/schemas/workflow_run_awsem.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/tests/conftest.py` & `encoded_core-0.9.0/src/encoded_core/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/tests/conftest_settings.py` & `encoded_core-0.9.0/src/encoded_core/tests/conftest_settings.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/tests/datafixtures.py` & `encoded_core-0.9.0/src/encoded_core/tests/datafixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 def file_formats(testapp):
     formats = {}
     ef_format_info = {
         'bai': {'standard_file_extension': 'bam.bai',
                 "valid_item_types": ["FileProcessed"]},
         'beddb': {"standard_file_extension": "beddb",
                   "valid_item_types": ["FileProcessed", "FileReference"]},
+        'vcf_gz': {"standard_file_extension": "vcf.gz",
+                   "valid_item_types": ["FileProcessed", "FileSubmitted"]}
     }
     format_info = {
         'fastq': {'standard_file_extension': 'fastq.gz',
                   'other_allowed_extensions': ['fq.gz'],
                   "valid_item_types": ["FileSubmitted"]},
         'bam': {'standard_file_extension': 'bam',
-                'extrafile_formats': ['bai'],
+                'extrafile_formats': ['bai', 'vcf_gz'],
                 "valid_item_types": ["FileProcessed"]},
         'zip': {'standard_file_extension': 'zip',
                 "valid_item_types": ["FileProcessed"]},
         'chromsizes': {'standard_file_extension': 'chrom.sizes',
                        "valid_item_types": ["FileReference"]},
         'other': {'standard_file_extension': '',
                   "valid_item_types": ["FileProcessed", "FileReference"]},
@@ -29,16 +31,14 @@
         'bg': {'standard_file_extension': 'bedGraph.gz',
                "valid_item_types": ["FileProcessed"]},
         'bigbed': {'standard_file_extension': 'bb',
                    "valid_item_types": ["FileProcessed", "FileReference"]},
         'bed': {"standard_file_extension": "bed.gz",
                 "extrafile_formats": ['beddb'],
                 "valid_item_types": ["FileProcessed", "FileReference"]},
-        'vcf_gz': {"standard_file_extension": "vcf.gz",
-                   "valid_item_types": ["FileProcessed", "FileSubmitted"]}
     }
 
     for eff, info in ef_format_info.items():
         info['file_format'] = eff
         info['uuid'] = str(uuid4())
         formats[eff] = testapp.post_json('/file_format', info, status=[201]).json['@graph'][0]
     for ff, info in format_info.items():
```

### Comparing `encoded_core-0.8.3/src/encoded_core/tests/test_types_file.py` & `encoded_core-0.9.0/src/encoded_core/tests/test_types_file.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/types/document.py` & `encoded_core-0.9.0/src/encoded_core/types/document.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/types/file.py` & `encoded_core-0.9.0/src/encoded_core/types/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,40 +68,42 @@
 
 def show_upload_credentials(request=None, context=None, status=None):
     if request is None or status not in File.SHOW_UPLOAD_CREDENTIALS_STATUSES:
         return False
     return request.has_permission('edit', context)
 
 
-def external_creds(bucket, key, name=None, profile_name=None):
+def external_creds(bucket, key, name=None, profile_name=None, upload=True):
     """
     if name is None, we want the link to s3 but no need to generate
     an access token.  This is useful for linking metadata to files that
     already exist on s3.
     """
 
     logging.getLogger('boto3').setLevel(logging.CRITICAL)
     credentials = {}
+    upload_or_download = 'upload' if upload else 'download'  # upload is the default
     s3_encrypt_key_id = None  # might be reassigned later from identity.get('ENCODED_S3_ENCRYPT_KEY_ID')
     if name is not None:
         policy = {
             "Version": "2012-10-17",
             "Statement": [
                 {
                     "Action": [
-                        "s3:PutObject",
                         "s3:GetObject"
                     ],
                     "Resource": [
                         f"arn:aws:s3:::{bucket}/{key}"
                     ],
                     "Effect": "Allow"
                 }
             ]
         }
+        if upload:  # by default allow this
+            policy['Statement'][0]['Action'].append('s3:PutObject')
         # In the new environment, extract S3 Keys from global application configuration
         if 'IDENTITY' in os.environ:
             identity = assume_identity()
             with override_environ(**identity):
                 conn = boto3.client('sts',
                                     aws_access_key_id=os.environ.get('S3_AWS_ACCESS_KEY_ID'),
                                     aws_secret_access_key=os.environ.get('S3_AWS_SECRET_ACCESS_KEY'))
@@ -126,26 +128,26 @@
         token = conn.get_federation_token(Name=name, Policy=json.dumps(policy))
         # 'access_key' 'secret_key' 'expiration' 'session_token'
         credentials = token.get('Credentials')
         # Convert Expiration datetime object to string via cast
         # Uncaught serialization error picked up by Docker - Will 2/25/2021
         credentials['Expiration'] = str(credentials['Expiration'])
         credentials.update({
-            'upload_url': f's3://{bucket}/{key}',
+            f'{upload_or_download}_url': f's3://{bucket}/{key}',
             'federated_user_arn': token.get('FederatedUser').get('Arn'),
             'federated_user_id': token.get('FederatedUser').get('FederatedUserId'),
             's3_encrypt_key_id': s3_encrypt_key_id,
             'request_id': token.get('ResponseMetadata').get('RequestId'),
             'key': key
         })
     return {
         'service': 's3',
         'bucket': bucket,
         'key': key,
-        'upload_credentials': credentials,
+        f'{upload_or_download}_credentials': credentials,
     }
 
 
 def property_closure(request, propname, root_uuid):
     # Must avoid cycles
     conn = request.registry[CONNECTION]
     seen = set()
```

### Comparing `encoded_core-0.8.3/src/encoded_core/types/file_format.py` & `encoded_core-0.9.0/src/encoded_core/types/file_format.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/types/file_processed.py` & `encoded_core-0.9.0/src/encoded_core/types/file_processed.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/types/file_submitted.py` & `encoded_core-0.9.0/src/encoded_core/types/file_submitted.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/types/higlass_view_config.py` & `encoded_core-0.9.0/src/encoded_core/types/higlass_view_config.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/types/image.py` & `encoded_core-0.9.0/src/encoded_core/types/image.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/types/meta_workflow.py` & `encoded_core-0.9.0/src/encoded_core/types/meta_workflow.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/types/page.py` & `encoded_core-0.9.0/src/encoded_core/types/page.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/types/quality_metric.py` & `encoded_core-0.9.0/src/encoded_core/types/quality_metric.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/types/software.py` & `encoded_core-0.9.0/src/encoded_core/types/software.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/types/tracking_item.py` & `encoded_core-0.9.0/src/encoded_core/types/tracking_item.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/types/user_content.py` & `encoded_core-0.9.0/src/encoded_core/types/user_content.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/types/workflow.py` & `encoded_core-0.9.0/src/encoded_core/types/workflow.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/src/encoded_core/upgrade.py` & `encoded_core-0.9.0/src/encoded_core/upgrade.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.8.3/PKG-INFO` & `encoded_core-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encoded-core
-Version: 0.8.3
+Version: 0.9.0
 Summary: Core data models for Park Lab ENCODE based projects
 Home-page: https://github.com/smaht-dac/encoded-core
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 3 - Alpha
```

