# Comparing `tmp/vy_lambda_tools-0.4.1.tar.gz` & `tmp/vy_lambda_tools-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vy_lambda_tools-0.4.1.tar", max compression
+gzip compressed data, was "vy_lambda_tools-0.4.2.tar", max compression
```

## Comparing `vy_lambda_tools-0.4.1.tar` & `vy_lambda_tools-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       88 2024-05-13 11:47:04.000000 vy_lambda_tools-0.4.1/README.adoc
--rw-r--r--   0        0        0      605 2024-05-13 11:47:04.000000 vy_lambda_tools-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 11:47:04.000000 vy_lambda_tools-0.4.1/vy_lambda_tools/__init__.py
--rw-r--r--   0        0        0      904 2024-05-13 11:47:04.000000 vy_lambda_tools-0.4.1/vy_lambda_tools/configuration.py
--rw-r--r--   0        0        0      217 2024-05-13 11:47:04.000000 vy_lambda_tools-0.4.1/vy_lambda_tools/feature_flag/__init__.py
--rw-r--r--   0        0        0     1988 2024-05-13 11:47:04.000000 vy_lambda_tools-0.4.1/vy_lambda_tools/feature_flag/base.py
--rw-r--r--   0        0        0     3519 2024-05-13 11:47:04.000000 vy_lambda_tools-0.4.1/vy_lambda_tools/feature_flag/providers.py
--rw-r--r--   0        0        0      312 2024-05-13 11:47:04.000000 vy_lambda_tools-0.4.1/vy_lambda_tools/handlers/__init__.py
--rw-r--r--   0        0        0     3990 2024-05-13 11:47:04.000000 vy_lambda_tools-0.4.1/vy_lambda_tools/handlers/api_gateway.py
--rw-r--r--   0        0        0     1205 2024-05-13 11:47:04.000000 vy_lambda_tools-0.4.1/vy_lambda_tools/handlers/dynamodb.py
--rw-r--r--   0        0        0      857 2024-05-13 11:47:04.000000 vy_lambda_tools-0.4.1/vy_lambda_tools/handlers/handler.py
--rw-r--r--   0        0        0     2850 2024-05-13 11:47:04.000000 vy_lambda_tools-0.4.1/vy_lambda_tools/handlers/sqs.py
--rw-r--r--   0        0        0     2360 2024-05-13 11:47:04.000000 vy_lambda_tools-0.4.1/vy_lambda_tools/instrumentation.py
--rw-r--r--   0        0        0        0 2024-05-13 11:47:04.000000 vy_lambda_tools-0.4.1/vy_lambda_tools/py.typed
--rw-r--r--   0        0        0     7217 2024-05-13 11:47:04.000000 vy_lambda_tools-0.4.1/vy_lambda_tools/routing.py
--rw-r--r--   0        0        0     4712 2024-05-13 11:47:04.000000 vy_lambda_tools-0.4.1/vy_lambda_tools/test_helpers.py
--rw-r--r--   0        0        0      446 2024-05-13 11:47:04.000000 vy_lambda_tools-0.4.1/vy_lambda_tools/types.py
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 vy_lambda_tools-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       88 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/README.adoc
+-rw-r--r--   0        0        0      605 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/__init__.py
+-rw-r--r--   0        0        0      904 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/configuration.py
+-rw-r--r--   0        0        0      217 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/feature_flag/__init__.py
+-rw-r--r--   0        0        0     1988 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/feature_flag/base.py
+-rw-r--r--   0        0        0     3519 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/feature_flag/providers.py
+-rw-r--r--   0        0        0      312 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/__init__.py
+-rw-r--r--   0        0        0     4020 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/api_gateway.py
+-rw-r--r--   0        0        0     1205 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/dynamodb.py
+-rw-r--r--   0        0        0      857 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/handler.py
+-rw-r--r--   0        0        0     2850 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/sqs.py
+-rw-r--r--   0        0        0     2360 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/instrumentation.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/py.typed
+-rw-r--r--   0        0        0     7217 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/routing.py
+-rw-r--r--   0        0        0     4957 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/test_helpers.py
+-rw-r--r--   0        0        0      446 2024-05-21 12:33:43.000000 vy_lambda_tools-0.4.2/vy_lambda_tools/types.py
+-rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 vy_lambda_tools-0.4.2/PKG-INFO
```

### Comparing `vy_lambda_tools-0.4.1/pyproject.toml` & `vy_lambda_tools-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "vy-lambda-tools"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["Nicolas Harlem Eide <nicolas@harlemeide.net>"]
 readme = "README.adoc"
 packages = [{include = "vy_lambda_tools"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.12"
 aws-lambda-powertools = "^2.32.0"
 boto3-stubs = {extras = ["dynamodb", "ssm"], version = "^1.28.53"}
 python-json-logger = "^2.0.7"
 boto3 = "^1.28.53"
 moto = "^4.2.13"
```

### Comparing `vy_lambda_tools-0.4.1/vy_lambda_tools/configuration.py` & `vy_lambda_tools-0.4.2/vy_lambda_tools/configuration.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.1/vy_lambda_tools/feature_flag/base.py` & `vy_lambda_tools-0.4.2/vy_lambda_tools/feature_flag/base.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.1/vy_lambda_tools/feature_flag/providers.py` & `vy_lambda_tools-0.4.2/vy_lambda_tools/feature_flag/providers.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.1/vy_lambda_tools/handlers/api_gateway.py` & `vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/api_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         if not api_gw_event.body:
             body = {}
         elif (
             api_gw_event.headers.get("Content-Type")
             == "application/x-www-form-urlencoded"
         ):
             body = parse_qs(api_gw_event.body)
-        elif _is_json(api_gw_event.decoded_body):
+        elif api_gw_event.decoded_body and _is_json(api_gw_event.decoded_body):
             body = api_gw_event.json_body
         else:
             raise ValueError("Unsupported content type")
 
         try:
             jwt = api_gw_event.request_context.authorizer
         except KeyError:
```

### Comparing `vy_lambda_tools-0.4.1/vy_lambda_tools/handlers/dynamodb.py` & `vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/dynamodb.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.1/vy_lambda_tools/handlers/handler.py` & `vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.1/vy_lambda_tools/handlers/sqs.py` & `vy_lambda_tools-0.4.2/vy_lambda_tools/handlers/sqs.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.1/vy_lambda_tools/instrumentation.py` & `vy_lambda_tools-0.4.2/vy_lambda_tools/instrumentation.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.1/vy_lambda_tools/routing.py` & `vy_lambda_tools-0.4.2/vy_lambda_tools/routing.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.1/vy_lambda_tools/test_helpers.py` & `vy_lambda_tools-0.4.2/vy_lambda_tools/test_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     method: Optional[str] = None,
     body: Optional[Union[dict[str, Any], str]] = None,
     path_parameters: Optional[dict[str, str]] = None,
     query_parameters: Optional[dict[str, str]] = None,
     caller_account_id: Optional[str] = None,
     jwt_claims: Optional[dict[str, Any]] = None,
     jwt_scopes: Optional[list[str]] = None,
+    jwt_context: Optional[dict[str, Any]] = None,
     headers: Optional[dict[str, str]] = None,
 ) -> dict[str, Any]:
     headers = headers or {}
 
     if body is None:
         body = ""
     elif "application/x-www-form-urlencoded" not in headers.get("Content-Type", ""):
@@ -76,15 +77,20 @@
         "resource": resource,
         "httpMethod": method,
         "body": body,
         "pathParameters": path_parameters,
         "queryStringParameters": query_parameters,
         "requestContext": {
             "identity": {"accountId": caller_account_id},
-            "authorizer": {"claims": jwt_claims, "scopes": jwt_scopes},
+            "authorizer": {
+                "claims": jwt_claims,
+                "scopes": jwt_scopes,
+                # authorization context details injected by a Lambda Authorizer
+                **(jwt_context if jwt_context is not None else {}),
+            },
         },
         "headers": headers,
     }
 
     return event
```

### Comparing `vy_lambda_tools-0.4.1/PKG-INFO` & `vy_lambda_tools-0.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: vy-lambda-tools
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Author: Nicolas Harlem Eide
 Author-email: nicolas@harlemeide.net
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aws-lambda-powertools (>=2.32.0,<3.0.0)
 Requires-Dist: boto3 (>=1.28.53,<2.0.0)
 Requires-Dist: boto3-stubs[dynamodb,ssm] (>=1.28.53,<2.0.0)
 Requires-Dist: moto (>=4.2.13,<5.0.0)
 Requires-Dist: python-json-logger (>=2.0.7,<3.0.0)
 Description-Content-Type: text/plain
```

