# Comparing `tmp/iam_actions-1.2.20240519.tar.gz` & `tmp/iam_actions-1.2.20240520.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240519.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240520.tar", max compression
```

## Comparing `iam_actions-1.2.20240519.tar` & `iam_actions-1.2.20240520.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-05-19 02:24:17.101822 iam_actions-1.2.20240519/LICENSE
--rw-r--r--   0        0        0     2302 2024-05-19 02:24:17.101822 iam_actions-1.2.20240519/README.md
--rw-r--r--   0        0        0      228 2024-05-19 02:24:17.105822 iam_actions-1.2.20240519/iam_actions/__init__.py
--rw-r--r--   0        0        0  4837373 2024-05-19 02:26:07.797197 iam_actions-1.2.20240519/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-05-19 02:24:17.105822 iam_actions-1.2.20240519/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-05-19 02:24:17.105822 iam_actions-1.2.20240519/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-05-19 02:24:17.105822 iam_actions-1.2.20240519/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-05-19 02:24:17.105822 iam_actions-1.2.20240519/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-05-19 02:24:17.105822 iam_actions-1.2.20240519/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-05-19 02:24:17.105822 iam_actions-1.2.20240519/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-05-19 02:24:17.105822 iam_actions-1.2.20240519/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-05-19 02:24:17.105822 iam_actions-1.2.20240519/iam_actions/generate/services.py
--rw-r--r--   0        0        0   629260 2024-05-19 02:26:07.797197 iam_actions-1.2.20240519/iam_actions/policies.json
--rw-r--r--   0        0        0   209717 2024-05-19 02:26:07.797197 iam_actions-1.2.20240519/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   610645 2024-05-19 02:26:07.797197 iam_actions-1.2.20240519/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-05-19 02:26:08.445193 iam_actions-1.2.20240519/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240519/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240519/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-20 02:24:23.455344 iam_actions-1.2.20240520/LICENSE
+-rw-r--r--   0        0        0     2302 2024-05-20 02:24:23.455344 iam_actions-1.2.20240520/README.md
+-rw-r--r--   0        0        0      228 2024-05-20 02:24:23.455344 iam_actions-1.2.20240520/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4837373 2024-05-20 02:26:06.951898 iam_actions-1.2.20240520/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-05-20 02:24:23.455344 iam_actions-1.2.20240520/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-05-20 02:24:23.455344 iam_actions-1.2.20240520/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-05-20 02:24:23.455344 iam_actions-1.2.20240520/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-05-20 02:24:23.455344 iam_actions-1.2.20240520/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-05-20 02:24:23.459344 iam_actions-1.2.20240520/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-05-20 02:24:23.459344 iam_actions-1.2.20240520/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-05-20 02:24:23.459344 iam_actions-1.2.20240520/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-05-20 02:24:23.459344 iam_actions-1.2.20240520/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   629260 2024-05-20 02:26:06.951898 iam_actions-1.2.20240520/iam_actions/policies.json
+-rw-r--r--   0        0        0   209717 2024-05-20 02:26:06.951898 iam_actions-1.2.20240520/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   610645 2024-05-20 02:26:06.951898 iam_actions-1.2.20240520/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-05-20 02:26:07.659901 iam_actions-1.2.20240520/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240520/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240520/PKG-INFO
```

### Comparing `iam_actions-1.2.20240519/LICENSE` & `iam_actions-1.2.20240520/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240519/README.md` & `iam_actions-1.2.20240520/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240519/iam_actions/actions.json` & `iam_actions-1.2.20240520/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -4450,209 +4450,209 @@
             "access_level": "Undocumented",
             "action": "ListIngestions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIngestion": {
+        "CreateAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "DeleteIngestion",
+            "action": "CreateAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
             "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAppBundle": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetAppBundle",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListAppAuthorizations": {
             "access_level": "Undocumented",
             "action": "ListAppAuthorizations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetUserAccessTasks": {
+        "GetIngestion": {
             "access_level": "Undocumented",
-            "action": "BatchGetUserAccessTasks",
+            "action": "GetIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIngestionDestination": {
+        "DeleteIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "UpdateIngestionDestination",
+            "action": "DeleteIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ConnectAppAuthorization": {
+        "UpdateIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "ConnectAppAuthorization",
+            "action": "UpdateIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIngestionDestination": {
+        "StartIngestion": {
             "access_level": "Undocumented",
-            "action": "CreateIngestionDestination",
+            "action": "StartIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopIngestion": {
+        "CreateIngestion": {
             "access_level": "Undocumented",
-            "action": "StopIngestion",
+            "action": "CreateIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAppAuthorization": {
+        "ListAppBundles": {
             "access_level": "Undocumented",
-            "action": "GetAppAuthorization",
+            "action": "ListAppBundles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppBundle": {
+        "GetAppBundle": {
             "access_level": "Undocumented",
-            "action": "DeleteAppBundle",
+            "action": "GetAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartIngestion": {
+        "StartUserAccessTasks": {
             "access_level": "Undocumented",
-            "action": "StartIngestion",
+            "action": "StartUserAccessTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIngestion": {
+        "BatchGetUserAccessTasks": {
             "access_level": "Undocumented",
-            "action": "CreateIngestion",
+            "action": "BatchGetUserAccessTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestion": {
+        "DeleteIngestion": {
             "access_level": "Undocumented",
-            "action": "GetIngestion",
+            "action": "DeleteIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartUserAccessTasks": {
+        "ConnectAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "StartUserAccessTasks",
+            "action": "ConnectAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestionDestination": {
+        "DeleteAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "GetIngestionDestination",
+            "action": "DeleteAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppBundle": {
+        "DeleteAppBundle": {
             "access_level": "Undocumented",
-            "action": "CreateAppBundle",
+            "action": "DeleteAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppAuthorization": {
+        "GetIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "CreateAppAuthorization",
+            "action": "GetIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppAuthorization": {
+        "StopIngestion": {
             "access_level": "Undocumented",
-            "action": "UpdateAppAuthorization",
+            "action": "StopIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIngestionDestination": {
+        "GetAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "DeleteIngestionDestination",
+            "action": "GetAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppBundles": {
+        "CreateAppBundle": {
             "access_level": "Undocumented",
-            "action": "ListAppBundles",
+            "action": "CreateAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListIngestionDestinations": {
             "access_level": "Undocumented",
             "action": "ListIngestionDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppAuthorization": {
+        "UpdateAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "DeleteAppAuthorization",
+            "action": "UpdateAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "appflow": {
@@ -5170,25 +5170,25 @@
             "condition_keys": [],
             "description": "Grants permission to update an existing Application Cost Profiler Report configuration",
             "orphan": false,
             "resources": []
         }
     },
     "application-transformation": {
-        "GetPortingCompatibilityAssessment": {
+        "StartContainerization": {
             "access_level": "Undocumented",
-            "action": "GetPortingCompatibilityAssessment",
+            "action": "StartContainerization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPortingRecommendationAssessment": {
+        "PutMetricData": {
             "access_level": "Undocumented",
-            "action": "StartPortingRecommendationAssessment",
+            "action": "PutMetricData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetRuntimeAssessment": {
             "access_level": "Undocumented",
@@ -5202,89 +5202,89 @@
             "access_level": "Undocumented",
             "action": "StartGroupingAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPortingCompatibilityAssessment": {
+        "GetContainerization": {
             "access_level": "Undocumented",
-            "action": "StartPortingCompatibilityAssessment",
+            "action": "GetContainerization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPortingRecommendationAssessment": {
+        "GetDeployment": {
             "access_level": "Undocumented",
-            "action": "GetPortingRecommendationAssessment",
+            "action": "GetDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeployment": {
+        "GetGroupingAssessment": {
             "access_level": "Undocumented",
-            "action": "GetDeployment",
+            "action": "GetGroupingAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartContainerization": {
+        "StartPortingCompatibilityAssessment": {
             "access_level": "Undocumented",
-            "action": "StartContainerization",
+            "action": "StartPortingCompatibilityAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "PutLogData": {
             "access_level": "Undocumented",
             "action": "PutLogData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContainerization": {
+        "GetPortingCompatibilityAssessment": {
             "access_level": "Undocumented",
-            "action": "GetContainerization",
+            "action": "GetPortingCompatibilityAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartRuntimeAssessment": {
+        "StartPortingRecommendationAssessment": {
             "access_level": "Undocumented",
-            "action": "StartRuntimeAssessment",
+            "action": "StartPortingRecommendationAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartDeployment": {
+        "StartRuntimeAssessment": {
             "access_level": "Undocumented",
-            "action": "StartDeployment",
+            "action": "StartRuntimeAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutMetricData": {
+        "GetPortingRecommendationAssessment": {
             "access_level": "Undocumented",
-            "action": "PutMetricData",
+            "action": "GetPortingRecommendationAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupingAssessment": {
+        "StartDeployment": {
             "access_level": "Undocumented",
-            "action": "GetGroupingAssessment",
+            "action": "StartDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "applicationinsights": {
@@ -11773,25 +11773,25 @@
             "condition_keys": [],
             "description": "Grants permission to view a seller dashboard",
             "orphan": false,
             "resources": [
                 "SellerDashboard"
             ]
         },
-        "ListPrivateListings": {
+        "PutDeploymentParameter": {
             "access_level": "Undocumented",
-            "action": "ListPrivateListings",
+            "action": "PutDeploymentParameter",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutDeploymentParameter": {
+        "ListPrivateListings": {
             "access_level": "Undocumented",
-            "action": "PutDeploymentParameter",
+            "action": "ListPrivateListings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "aws-marketplace-management": {
@@ -11997,225 +11997,225 @@
             "condition_keys": [],
             "description": "Validates Server Migration Connector Id that was registered with AWS Connector Service.",
             "orphan": false,
             "resources": []
         }
     },
     "b2bi": {
-        "GetTransformerJob": {
+        "GetTransformer": {
             "access_level": "Undocumented",
-            "action": "GetTransformerJob",
+            "action": "GetTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProfile": {
+        "DeletePartnership": {
             "access_level": "Undocumented",
-            "action": "UpdateProfile",
+            "action": "DeletePartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePartnership": {
+        "CreateTransformer": {
             "access_level": "Undocumented",
-            "action": "DeletePartnership",
+            "action": "CreateTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCapabilities": {
+        "ListProfiles": {
             "access_level": "Undocumented",
-            "action": "ListCapabilities",
+            "action": "ListProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListTransformers": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListTransformers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "StartTransformerJob": {
             "access_level": "Undocumented",
             "action": "StartTransformerJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTransformer": {
+        "ListPartnerships": {
             "access_level": "Undocumented",
-            "action": "CreateTransformer",
+            "action": "ListPartnerships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPartnership": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetPartnership",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePartnership": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreatePartnership",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTransformer": {
+        "DeleteCapability": {
             "access_level": "Undocumented",
-            "action": "DeleteTransformer",
+            "action": "DeleteCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTransformer": {
+        "GetCapability": {
             "access_level": "Undocumented",
-            "action": "UpdateTransformer",
+            "action": "GetCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProfile": {
+        "TestMapping": {
             "access_level": "Undocumented",
-            "action": "DeleteProfile",
+            "action": "TestMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTransformer": {
+        "GetTransformerJob": {
             "access_level": "Undocumented",
-            "action": "GetTransformer",
+            "action": "GetTransformerJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestMapping": {
+        "CreatePartnership": {
             "access_level": "Undocumented",
-            "action": "TestMapping",
+            "action": "CreatePartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UpdatePartnership": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UpdatePartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCapability": {
+        "UpdateCapability": {
             "access_level": "Undocumented",
-            "action": "DeleteCapability",
+            "action": "UpdateCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCapability": {
+        "ListCapabilities": {
             "access_level": "Undocumented",
-            "action": "GetCapability",
+            "action": "ListCapabilities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCapability": {
+        "UpdateProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateCapability",
+            "action": "UpdateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTransformers": {
+        "TestParsing": {
             "access_level": "Undocumented",
-            "action": "ListTransformers",
+            "action": "TestParsing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCapability": {
+        "CreateProfile": {
             "access_level": "Undocumented",
-            "action": "CreateCapability",
+            "action": "CreateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProfile": {
+        "DeleteProfile": {
             "access_level": "Undocumented",
-            "action": "CreateProfile",
+            "action": "DeleteProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePartnership": {
+        "CreateCapability": {
             "access_level": "Undocumented",
-            "action": "UpdatePartnership",
+            "action": "CreateCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProfiles": {
+        "DeleteTransformer": {
             "access_level": "Undocumented",
-            "action": "ListProfiles",
+            "action": "DeleteTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdateTransformer": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProfile": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetProfile",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPartnerships": {
+        "GetProfile": {
             "access_level": "Undocumented",
-            "action": "ListPartnerships",
+            "action": "GetProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestParsing": {
+        "GetPartnership": {
             "access_level": "Undocumented",
-            "action": "TestParsing",
+            "action": "GetPartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "backup": {
@@ -13857,909 +13857,909 @@
             "access_level": "Undocumented",
             "action": "ListTables",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExport": {
+        "GetExecution": {
             "access_level": "Undocumented",
-            "action": "GetExport",
+            "action": "GetExecution",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExports": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListExports",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExecutions": {
+        "GetTable": {
             "access_level": "Undocumented",
-            "action": "ListExecutions",
+            "action": "GetTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteExport": {
+        "CreateExport": {
             "access_level": "Undocumented",
-            "action": "DeleteExport",
+            "action": "CreateExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateExport": {
+        "UpdateExport": {
             "access_level": "Undocumented",
-            "action": "CreateExport",
+            "action": "UpdateExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTable": {
+        "GetExport": {
             "access_level": "Undocumented",
-            "action": "GetTable",
+            "action": "GetExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListExecutions": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListExecutions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExecution": {
+        "ListExports": {
             "access_level": "Undocumented",
-            "action": "GetExecution",
+            "action": "ListExports",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateExport": {
+        "DeleteExport": {
             "access_level": "Undocumented",
-            "action": "UpdateExport",
+            "action": "DeleteExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "bedrock": {
-        "GetKnowledgeBase": {
+        "GetAgentVersion": {
             "access_level": "Undocumented",
-            "action": "GetKnowledgeBase",
+            "action": "GetAgentVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListFoundationModelAgreementOffers": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListFoundationModelAgreementOffers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Retrieve": {
+        "GetFoundationModelAvailability": {
             "access_level": "Undocumented",
-            "action": "Retrieve",
+            "action": "GetFoundationModelAvailability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgentKnowledgeBase": {
+        "CreateEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "UpdateAgentKnowledgeBase",
+            "action": "CreateEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEvaluationJobs": {
+        "DeleteProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "ListEvaluationJobs",
+            "action": "DeleteProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFoundationModelAgreement": {
+        "StopModelCustomizationJob": {
             "access_level": "Undocumented",
-            "action": "CreateFoundationModelAgreement",
+            "action": "StopModelCustomizationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InvokeModelWithResponseStream": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "InvokeModelWithResponseStream",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "DeleteAgentAlias": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "DeleteAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUseCaseForModelAccess": {
+        "GetDataSource": {
             "access_level": "Undocumented",
-            "action": "GetUseCaseForModelAccess",
+            "action": "GetDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCustomModel": {
+        "CreateFoundationModelAgreement": {
             "access_level": "Undocumented",
-            "action": "GetCustomModel",
+            "action": "CreateFoundationModelAgreement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PrepareAgent": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "PrepareAgent",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DisassociateAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DisassociateAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgentVersion": {
+        "InvokeModel": {
             "access_level": "Undocumented",
-            "action": "GetAgentVersion",
+            "action": "InvokeModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InvokeModel": {
+        "PrepareAgent": {
             "access_level": "Undocumented",
-            "action": "InvokeModel",
+            "action": "PrepareAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUseCaseForModelAccess": {
+        "GetProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "PutUseCaseForModelAccess",
+            "action": "GetProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIngestionJobs": {
+        "UpdateAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "ListIngestionJobs",
+            "action": "UpdateAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentActionGroups": {
+        "ListModelEvaluationJobs": {
             "access_level": "Undocumented",
-            "action": "ListAgentActionGroups",
+            "action": "ListModelEvaluationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteModelInvocationLoggingConfiguration": {
+        "UpdateProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "DeleteModelInvocationLoggingConfiguration",
+            "action": "UpdateProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSource": {
+        "GetFoundationModel": {
             "access_level": "Undocumented",
-            "action": "GetDataSource",
+            "action": "GetFoundationModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestionJob": {
+        "GetEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "GetIngestionJob",
+            "action": "GetEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateModelEvaluationJob": {
+        "CreateProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "CreateModelEvaluationJob",
+            "action": "CreateProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgentAlias": {
+        "DeleteModelInvocationLoggingConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteAgentAlias",
+            "action": "DeleteModelInvocationLoggingConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelCustomizationJob": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "GetModelCustomizationJob",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCustomModel": {
+        "Retrieve": {
             "access_level": "Undocumented",
-            "action": "DeleteCustomModel",
+            "action": "Retrieve",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopModelInvocationJob": {
+        "GetAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "StopModelInvocationJob",
+            "action": "GetAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelInvocationJob": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetModelInvocationJob",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGuardrail": {
+        "ListAgentAliases": {
             "access_level": "Undocumented",
-            "action": "GetGuardrail",
+            "action": "ListAgentAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProvisionedModelThroughput": {
+        "ListProvisionedModelThroughputs": {
             "access_level": "Undocumented",
-            "action": "CreateProvisionedModelThroughput",
+            "action": "ListProvisionedModelThroughputs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKnowledgeBases": {
+        "CreateGuardrailVersion": {
             "access_level": "Undocumented",
-            "action": "ListKnowledgeBases",
+            "action": "CreateGuardrailVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopModelCustomizationJob": {
+        "GetModelCustomizationJob": {
             "access_level": "Undocumented",
-            "action": "StopModelCustomizationJob",
+            "action": "GetModelCustomizationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGuardrail": {
+        "GetModelInvocationJob": {
             "access_level": "Undocumented",
-            "action": "CreateGuardrail",
+            "action": "GetModelInvocationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateAgentKnowledgeBase": {
+        "PutModelInvocationLoggingConfiguration": {
             "access_level": "Undocumented",
-            "action": "AssociateAgentKnowledgeBase",
+            "action": "PutModelInvocationLoggingConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RetrieveAndGenerate": {
+        "StopModelInvocationJob": {
             "access_level": "Undocumented",
-            "action": "RetrieveAndGenerate",
+            "action": "StopModelInvocationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAgentActionGroup": {
+        "UpdateAgentAlias": {
             "access_level": "Undocumented",
-            "action": "CreateAgentActionGroup",
+            "action": "UpdateAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProvisionedModelThroughput": {
+        "DeleteGuardrail": {
             "access_level": "Undocumented",
-            "action": "UpdateProvisionedModelThroughput",
+            "action": "DeleteGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgents": {
+        "ListCustomModels": {
             "access_level": "Undocumented",
-            "action": "ListAgents",
+            "action": "ListCustomModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFoundationModelAgreement": {
+        "ListFoundationModels": {
             "access_level": "Undocumented",
-            "action": "DeleteFoundationModelAgreement",
+            "action": "ListFoundationModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentAliases": {
+        "ListIngestionJobs": {
             "access_level": "Undocumented",
-            "action": "ListAgentAliases",
+            "action": "ListIngestionJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCustomModels": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "ListCustomModels",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelInvocationLoggingConfiguration": {
+        "UpdateKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "GetModelInvocationLoggingConfiguration",
+            "action": "UpdateKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateKnowledgeBase": {
+        "ListAgentActionGroups": {
             "access_level": "Undocumented",
-            "action": "UpdateKnowledgeBase",
+            "action": "ListAgentActionGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "GetModelInvocationLoggingConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "GetModelInvocationLoggingConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ApplyGuardrail": {
+        "CreateGuardrail": {
             "access_level": "Undocumented",
-            "action": "ApplyGuardrail",
+            "action": "CreateGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateModelCustomizationJob": {
+        "ListAgentVersions": {
             "access_level": "Undocumented",
-            "action": "CreateModelCustomizationJob",
+            "action": "ListAgentVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgentActionGroup": {
+        "StartIngestionJob": {
             "access_level": "Undocumented",
-            "action": "GetAgentActionGroup",
+            "action": "StartIngestionJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateAgentKnowledgeBase": {
+        "ListAgentKnowledgeBases": {
             "access_level": "Undocumented",
-            "action": "DisassociateAgentKnowledgeBase",
+            "action": "ListAgentKnowledgeBases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAgent": {
+        "GetAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "CreateAgent",
+            "action": "GetAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFoundationModelAvailability": {
+        "PutFoundationModelEntitlement": {
             "access_level": "Undocumented",
-            "action": "GetFoundationModelAvailability",
+            "action": "PutFoundationModelEntitlement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgent": {
+        "GetUseCaseForModelAccess": {
             "access_level": "Undocumented",
-            "action": "UpdateAgent",
+            "action": "GetUseCaseForModelAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgentVersion": {
+        "ListModelInvocationJobs": {
             "access_level": "Undocumented",
-            "action": "DeleteAgentVersion",
+            "action": "ListModelInvocationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEvaluationJob": {
+        "RetrieveAndGenerate": {
             "access_level": "Undocumented",
-            "action": "GetEvaluationJob",
+            "action": "RetrieveAndGenerate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListModelEvaluationJobs": {
+        "CreateAgent": {
             "access_level": "Undocumented",
-            "action": "ListModelEvaluationJobs",
+            "action": "CreateAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFoundationModelEntitlement": {
+        "DeleteAgent": {
             "access_level": "Undocumented",
-            "action": "PutFoundationModelEntitlement",
+            "action": "DeleteAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKnowledgeBase": {
+        "InvokeAgent": {
             "access_level": "Undocumented",
-            "action": "DeleteKnowledgeBase",
+            "action": "InvokeAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetectGeneratedContent": {
+        "StopEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "DetectGeneratedContent",
+            "action": "StopEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEvaluationJob": {
+        "DeleteCustomModel": {
             "access_level": "Undocumented",
-            "action": "CreateEvaluationJob",
+            "action": "DeleteCustomModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "DeleteFoundationModelAgreement": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "DeleteFoundationModelAgreement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetModelEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetModelEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFoundationModel": {
+        "InvokeModelWithResponseStream": {
             "access_level": "Undocumented",
-            "action": "GetFoundationModel",
+            "action": "InvokeModelWithResponseStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProvisionedModelThroughput": {
+        "CreateAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteProvisionedModelThroughput",
+            "action": "CreateAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKnowledgeBase": {
+        "DeleteAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "CreateKnowledgeBase",
+            "action": "DeleteAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateModelInvocationJob": {
+        "AssociateAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "CreateModelInvocationJob",
+            "action": "AssociateAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListModelInvocationJobs": {
+        "CreateModelCustomizationJob": {
             "access_level": "Undocumented",
-            "action": "ListModelInvocationJobs",
+            "action": "CreateModelCustomizationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgent": {
+        "PutUseCaseForModelAccess": {
             "access_level": "Undocumented",
-            "action": "GetAgent",
+            "action": "PutUseCaseForModelAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentKnowledgeBases": {
+        "UpdateAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "ListAgentKnowledgeBases",
+            "action": "UpdateAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProvisionedModelThroughputs": {
+        "GetCustomModel": {
             "access_level": "Undocumented",
-            "action": "ListProvisionedModelThroughputs",
+            "action": "GetCustomModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InvokeAgent": {
+        "AssociateThirdPartyKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "InvokeAgent",
+            "action": "AssociateThirdPartyKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelEvaluationJob": {
+        "ListAgents": {
             "access_level": "Undocumented",
-            "action": "GetModelEvaluationJob",
+            "action": "ListAgents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartIngestionJob": {
+        "DeleteAgentVersion": {
             "access_level": "Undocumented",
-            "action": "StartIngestionJob",
+            "action": "DeleteAgentVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAgentAlias": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "CreateAgentAlias",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgentActionGroup": {
+        "ListGuardrails": {
             "access_level": "Undocumented",
-            "action": "UpdateAgentActionGroup",
+            "action": "ListGuardrails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgentAlias": {
+        "CreateKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "UpdateAgentAlias",
+            "action": "CreateKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "CreateAgentAlias": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "CreateAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProvisionedModelThroughput": {
+        "DeleteKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "GetProvisionedModelThroughput",
+            "action": "DeleteKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentVersions": {
+        "GetGuardrail": {
             "access_level": "Undocumented",
-            "action": "ListAgentVersions",
+            "action": "GetGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgentActionGroup": {
+        "CreateModelInvocationJob": {
             "access_level": "Undocumented",
-            "action": "DeleteAgentActionGroup",
+            "action": "CreateModelInvocationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGuardrail": {
+        "DetectGeneratedContent": {
             "access_level": "Undocumented",
-            "action": "DeleteGuardrail",
+            "action": "DetectGeneratedContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGuardrailVersion": {
+        "ListEvaluationJobs": {
             "access_level": "Undocumented",
-            "action": "CreateGuardrailVersion",
+            "action": "ListEvaluationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFoundationModels": {
+        "ListModelCustomizationJobs": {
             "access_level": "Undocumented",
-            "action": "ListFoundationModels",
+            "action": "ListModelCustomizationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgentKnowledgeBase": {
+        "UpdateGuardrail": {
             "access_level": "Undocumented",
-            "action": "GetAgentKnowledgeBase",
+            "action": "UpdateGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateThirdPartyKnowledgeBase": {
+        "ApplyGuardrail": {
             "access_level": "Undocumented",
-            "action": "AssociateThirdPartyKnowledgeBase",
+            "action": "ApplyGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGuardrails": {
+        "UpdateAgent": {
             "access_level": "Undocumented",
-            "action": "ListGuardrails",
+            "action": "UpdateAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopEvaluationJob": {
+        "CreateModelEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "StopEvaluationJob",
+            "action": "CreateModelEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListModelCustomizationJobs": {
+        "ListKnowledgeBases": {
             "access_level": "Undocumented",
-            "action": "ListModelCustomizationJobs",
+            "action": "ListKnowledgeBases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFoundationModelAgreementOffers": {
+        "GetIngestionJob": {
             "access_level": "Undocumented",
-            "action": "ListFoundationModelAgreementOffers",
+            "action": "GetIngestionJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetAgentAlias": {
             "access_level": "Undocumented",
             "action": "GetAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgent": {
+        "GetAgent": {
             "access_level": "Undocumented",
-            "action": "DeleteAgent",
+            "action": "GetAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutModelInvocationLoggingConfiguration": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "PutModelInvocationLoggingConfiguration",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGuardrail": {
+        "GetKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "UpdateGuardrail",
+            "action": "GetKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "billing": {
-        "GetBillingData": {
+        "GetSellerOfRecord": {
             "access_level": "Undocumented",
-            "action": "GetBillingData",
+            "action": "GetSellerOfRecord",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIAMAccessPreference": {
+        "GetBillingData": {
             "access_level": "Undocumented",
-            "action": "GetIAMAccessPreference",
+            "action": "GetBillingData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RedeemCredits": {
+        "GetBillingPreferences": {
             "access_level": "Undocumented",
-            "action": "RedeemCredits",
+            "action": "GetBillingPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIAMAccessPreference": {
+        "ListBillingViews": {
             "access_level": "Undocumented",
-            "action": "UpdateIAMAccessPreference",
+            "action": "ListBillingViews",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillingPreferences": {
+        "GetBillingNotifications": {
             "access_level": "Undocumented",
-            "action": "GetBillingPreferences",
+            "action": "GetBillingNotifications",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListBillingViews": {
+        "GetBillingDetails": {
             "access_level": "Undocumented",
-            "action": "ListBillingViews",
+            "action": "GetBillingDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContractInformation": {
+        "UpdateIAMAccessPreference": {
             "access_level": "Undocumented",
-            "action": "GetContractInformation",
+            "action": "UpdateIAMAccessPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillingDetails": {
+        "GetContractInformation": {
             "access_level": "Undocumented",
-            "action": "GetBillingDetails",
+            "action": "GetContractInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutContractInformation": {
+        "RedeemCredits": {
             "access_level": "Undocumented",
-            "action": "PutContractInformation",
+            "action": "RedeemCredits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillingNotifications": {
+        "PutContractInformation": {
             "access_level": "Undocumented",
-            "action": "GetBillingNotifications",
+            "action": "PutContractInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateBillingPreferences": {
             "access_level": "Undocumented",
             "action": "UpdateBillingPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSellerOfRecord": {
+        "GetIAMAccessPreference": {
             "access_level": "Undocumented",
-            "action": "GetSellerOfRecord",
+            "action": "GetIAMAccessPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetCredits": {
             "access_level": "Undocumented",
@@ -19939,715 +19939,715 @@
             "condition_keys": [],
             "description": "Grants permission to validate an address to be used for 911 calls made with Amazon Chime Voice Connectors",
             "orphan": false,
             "resources": []
         }
     },
     "cleanrooms": {
-        "DeleteCollaboration": {
+        "BatchGetSchema": {
             "access_level": "Undocumented",
-            "action": "DeleteCollaboration",
+            "action": "BatchGetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrivacyBudgetTemplates": {
+        "GetMembership": {
             "access_level": "Undocumented",
-            "action": "ListPrivacyBudgetTemplates",
+            "action": "GetMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnalysisTemplates": {
+        "UpdateConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "ListAnalysisTemplates",
+            "action": "UpdateConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetCollaborationAnalysisTemplate": {
+        "CreateCollaboration": {
             "access_level": "Undocumented",
-            "action": "BatchGetCollaborationAnalysisTemplate",
+            "action": "CreateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProtectedQuery": {
+        "GetConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "StartProtectedQuery",
+            "action": "GetConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
             "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePrivacyBudgetTemplate": {
+        "GetConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "CreatePrivacyBudgetTemplate",
+            "action": "GetConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMember": {
+        "ListSchemas": {
             "access_level": "Undocumented",
-            "action": "DeleteMember",
+            "action": "ListSchemas",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMembership": {
+        "CreatePrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdateMembership",
+            "action": "CreatePrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredAudienceModelAssociation": {
+        "ListCollaborationPrivacyBudgets": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredAudienceModelAssociation",
+            "action": "ListCollaborationPrivacyBudgets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredAudienceModelAssociation": {
+        "BatchGetSchemaAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredAudienceModelAssociation",
+            "action": "BatchGetSchemaAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCollaboration": {
+        "DeleteConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "CreateCollaboration",
+            "action": "DeleteConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCollaboration": {
+        "GetCollaboration": {
             "access_level": "Undocumented",
-            "action": "UpdateCollaboration",
+            "action": "GetCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTable": {
+        "ListPrivacyBudgetTemplates": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTable",
+            "action": "ListPrivacyBudgetTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMembership": {
+        "UpdatePrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteMembership",
+            "action": "UpdatePrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PreviewPrivacyImpact": {
+        "GetConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "PreviewPrivacyImpact",
+            "action": "GetConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredAudienceModelAssociation": {
+        "GetCollaborationAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredAudienceModelAssociation",
+            "action": "GetCollaborationAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMemberships": {
+        "ListConfiguredTableAssociations": {
             "access_level": "Undocumented",
-            "action": "ListMemberships",
+            "action": "ListConfiguredTableAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAnalysisTemplate": {
+        "CreateAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteAnalysisTemplate",
+            "action": "CreateAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationConfiguredAudienceModelAssociations": {
+        "ListConfiguredTables": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationConfiguredAudienceModelAssociations",
+            "action": "ListConfiguredTables",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAssociation": {
+        "StartProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAssociation",
+            "action": "StartProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UpdateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UpdateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetSchema": {
+        "BatchGetCollaborationAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "BatchGetSchema",
+            "action": "BatchGetCollaborationAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetSchemaAnalysisRule": {
+        "DeleteConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "BatchGetSchemaAnalysisRule",
+            "action": "DeleteConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePrivacyBudgetTemplate": {
+        "ListMemberships": {
             "access_level": "Undocumented",
-            "action": "DeletePrivacyBudgetTemplate",
+            "action": "ListMemberships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredAudienceModelAssociations": {
+        "PreviewPrivacyImpact": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredAudienceModelAssociations",
+            "action": "PreviewPrivacyImpact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaborationConfiguredAudienceModelAssociation": {
+        "CreateMembership": {
             "access_level": "Undocumented",
-            "action": "GetCollaborationConfiguredAudienceModelAssociation",
+            "action": "CreateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationPrivacyBudgetTemplates": {
+        "DeleteMembership": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationPrivacyBudgetTemplates",
+            "action": "DeleteMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAnalysisRule": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAnalysisRule",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAnalysisTemplate": {
+        "UpdateMembership": {
             "access_level": "Undocumented",
-            "action": "UpdateAnalysisTemplate",
+            "action": "UpdateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSchemas": {
+        "ListCollaborationPrivacyBudgetTemplates": {
             "access_level": "Undocumented",
-            "action": "ListSchemas",
+            "action": "ListCollaborationPrivacyBudgetTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProtectedQuery": {
+        "DeleteMember": {
             "access_level": "Undocumented",
-            "action": "UpdateProtectedQuery",
+            "action": "DeleteMember",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTable": {
+        "DeleteConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTable",
+            "action": "DeleteConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMembership": {
+        "ListCollaborations": {
             "access_level": "Undocumented",
-            "action": "GetMembership",
+            "action": "ListCollaborations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePrivacyBudgetTemplate": {
+        "GetSchemaAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "UpdatePrivacyBudgetTemplate",
+            "action": "GetSchemaAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAssociation": {
+        "ListAnalysisTemplates": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAssociation",
+            "action": "ListAnalysisTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaboration": {
+        "CreateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "GetCollaboration",
+            "action": "CreateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationPrivacyBudgets": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationPrivacyBudgets",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProtectedQueries": {
+        "UpdateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "ListProtectedQueries",
+            "action": "UpdateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTableAssociations": {
+        "GetConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTableAssociations",
+            "action": "GetConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchemaAnalysisRule": {
+        "CreateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "GetSchemaAnalysisRule",
+            "action": "CreateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "DeleteAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "DeleteAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborations": {
+        "ListMembers": {
             "access_level": "Undocumented",
-            "action": "ListCollaborations",
+            "action": "ListMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAnalysisRule": {
+        "ListProtectedQueries": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAnalysisRule",
+            "action": "ListProtectedQueries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMembers": {
+        "DeleteCollaboration": {
             "access_level": "Undocumented",
-            "action": "ListMembers",
+            "action": "DeleteCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaborationAnalysisTemplate": {
+        "ListPrivacyBudgets": {
             "access_level": "Undocumented",
-            "action": "GetCollaborationAnalysisTemplate",
+            "action": "ListPrivacyBudgets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredAudienceModelAssociation": {
+        "UpdateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredAudienceModelAssociation",
+            "action": "UpdateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTable": {
+        "CreateConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTable",
+            "action": "CreateConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAssociation": {
+        "GetCollaborationConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAssociation",
+            "action": "GetCollaborationConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaborationPrivacyBudgetTemplate": {
+        "UpdateProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "GetCollaborationPrivacyBudgetTemplate",
+            "action": "UpdateProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnalysisTemplate": {
+        "ListConfiguredAudienceModelAssociations": {
             "access_level": "Undocumented",
-            "action": "GetAnalysisTemplate",
+            "action": "ListConfiguredAudienceModelAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTables": {
+        "CreateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTables",
+            "action": "CreateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMembership": {
+        "ListCollaborationConfiguredAudienceModelAssociations": {
             "access_level": "Undocumented",
-            "action": "CreateMembership",
+            "action": "ListCollaborationConfiguredAudienceModelAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTable": {
+        "DeleteConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTable",
+            "action": "DeleteConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPrivacyBudgetTemplate": {
+        "GetProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "GetPrivacyBudgetTemplate",
+            "action": "GetProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrivacyBudgets": {
+        "GetAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "ListPrivacyBudgets",
+            "action": "GetAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAnalysisRule": {
+        "DeletePrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAnalysisRule",
+            "action": "DeletePrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAssociation": {
+        "UpdateAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAssociation",
+            "action": "UpdateAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAnalysisTemplate": {
+        "ListCollaborationAnalysisTemplates": {
             "access_level": "Undocumented",
-            "action": "CreateAnalysisTemplate",
+            "action": "ListCollaborationAnalysisTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationAnalysisTemplates": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationAnalysisTemplates",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAnalysisRule": {
+        "GetPrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAnalysisRule",
+            "action": "GetPrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdateCollaboration": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProtectedQuery": {
+        "GetCollaborationPrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "GetProtectedQuery",
+            "action": "GetCollaborationPrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cleanrooms-ml": {
-        "UpdateConfiguredAudienceModel": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredAudienceModel",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTrainingDataset": {
+        "StartAudienceGenerationJob": {
             "access_level": "Undocumented",
-            "action": "CreateTrainingDataset",
+            "action": "StartAudienceGenerationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTrainingDataset": {
+        "ListAudienceExportJobs": {
             "access_level": "Undocumented",
-            "action": "DeleteTrainingDataset",
+            "action": "ListAudienceExportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTrainingDataset": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetTrainingDataset",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAudienceModels": {
+        "CreateAudienceModel": {
             "access_level": "Undocumented",
-            "action": "ListAudienceModels",
+            "action": "CreateAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAudienceModel": {
+        "DeleteTrainingDataset": {
             "access_level": "Undocumented",
-            "action": "CreateAudienceModel",
+            "action": "DeleteTrainingDataset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredAudienceModelPolicy": {
+        "GetAudienceModel": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredAudienceModelPolicy",
+            "action": "GetAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredAudienceModels": {
+        "GetConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredAudienceModels",
+            "action": "GetConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListAudienceGenerationJobs": {
             "access_level": "Undocumented",
             "action": "ListAudienceGenerationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UnTagResource": {
+        "GetAudienceGenerationJob": {
             "access_level": "Undocumented",
-            "action": "UnTagResource",
+            "action": "GetAudienceGenerationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAudienceGenerationJob": {
+        "ListConfiguredAudienceModels": {
             "access_level": "Undocumented",
-            "action": "GetAudienceGenerationJob",
+            "action": "ListConfiguredAudienceModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTrainingDatasets": {
+        "StartAudienceExportJob": {
             "access_level": "Undocumented",
-            "action": "ListTrainingDatasets",
+            "action": "StartAudienceExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutConfiguredAudienceModelPolicy": {
+        "ListAudienceModels": {
             "access_level": "Undocumented",
-            "action": "PutConfiguredAudienceModelPolicy",
+            "action": "ListAudienceModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAudienceModel": {
+        "CreateConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "GetAudienceModel",
+            "action": "CreateConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetConfiguredAudienceModelPolicy": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetConfiguredAudienceModelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAudienceGenerationJob": {
+        "GetTrainingDataset": {
             "access_level": "Undocumented",
-            "action": "DeleteAudienceGenerationJob",
+            "action": "GetTrainingDataset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAudienceModel": {
+        "CreateTrainingDataset": {
             "access_level": "Undocumented",
-            "action": "DeleteAudienceModel",
+            "action": "CreateTrainingDataset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredAudienceModel": {
+        "DeleteAudienceGenerationJob": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredAudienceModel",
+            "action": "DeleteAudienceGenerationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAudienceExportJob": {
+        "PutConfiguredAudienceModelPolicy": {
             "access_level": "Undocumented",
-            "action": "StartAudienceExportJob",
+            "action": "PutConfiguredAudienceModelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredAudienceModel": {
+        "DeleteAudienceModel": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredAudienceModel",
+            "action": "DeleteAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAudienceExportJobs": {
+        "UnTagResource": {
             "access_level": "Undocumented",
-            "action": "ListAudienceExportJobs",
+            "action": "UnTagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredAudienceModel": {
+        "UpdateConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredAudienceModel",
+            "action": "UpdateConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAudienceGenerationJob": {
+        "DeleteConfiguredAudienceModelPolicy": {
             "access_level": "Undocumented",
-            "action": "StartAudienceGenerationJob",
+            "action": "DeleteConfiguredAudienceModelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredAudienceModelPolicy": {
+        "ListTrainingDatasets": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredAudienceModelPolicy",
+            "action": "ListTrainingDatasets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cloud9": {
@@ -23650,41 +23650,41 @@
             "access_level": "Undocumented",
             "action": "ListKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKey": {
+        "DescribeKeyValueStore": {
             "access_level": "Undocumented",
-            "action": "GetKey",
+            "action": "DescribeKeyValueStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeKeyValueStore": {
+        "DeleteKey": {
             "access_level": "Undocumented",
-            "action": "DescribeKeyValueStore",
+            "action": "DeleteKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateKeys": {
             "access_level": "Undocumented",
             "action": "UpdateKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKey": {
+        "GetKey": {
             "access_level": "Undocumented",
-            "action": "DeleteKey",
+            "action": "GetKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cloudhsm": {
@@ -27836,305 +27836,305 @@
             "orphan": false,
             "resources": [
                 "repository"
             ]
         }
     },
     "codeconnections": {
-        "ListInstallationTargets": {
+        "GetSyncBlockerSummary": {
             "access_level": "Undocumented",
-            "action": "ListInstallationTargets",
+            "action": "GetSyncBlockerSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartOAuthHandshake": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "StartOAuthHandshake",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRepositoryLink": {
+        "DeleteRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "GetRepositoryLink",
+            "action": "DeleteRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSyncConfiguration": {
+        "PassConnection": {
             "access_level": "Undocumented",
-            "action": "GetSyncConfiguration",
+            "action": "PassConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateSyncBlocker": {
             "access_level": "Undocumented",
             "action": "UpdateSyncBlocker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UseConnection": {
+        "DeleteHost": {
             "access_level": "Undocumented",
-            "action": "UseConnection",
+            "action": "DeleteHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceSyncStatus": {
+        "DeleteSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetResourceSyncStatus",
+            "action": "DeleteSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateHost": {
+        "ListRepositoryLinks": {
             "access_level": "Undocumented",
-            "action": "UpdateHost",
+            "action": "ListRepositoryLinks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSyncConfiguration": {
+        "CreateConnection": {
             "access_level": "Undocumented",
-            "action": "DeleteSyncConfiguration",
+            "action": "CreateConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSyncConfiguration": {
+        "GetRepositorySyncStatus": {
             "access_level": "Undocumented",
-            "action": "UpdateSyncConfiguration",
+            "action": "GetRepositorySyncStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRepositoryLink": {
+        "ListInstallationTargets": {
             "access_level": "Undocumented",
-            "action": "CreateRepositoryLink",
+            "action": "ListInstallationTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConnection": {
+        "ListConnections": {
             "access_level": "Undocumented",
-            "action": "CreateConnection",
+            "action": "ListConnections",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConnection": {
+        "GetResourceSyncStatus": {
             "access_level": "Undocumented",
-            "action": "GetConnection",
+            "action": "GetResourceSyncStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateHost": {
+        "ListRepositorySyncDefinitions": {
             "access_level": "Undocumented",
-            "action": "CreateHost",
+            "action": "ListRepositorySyncDefinitions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSyncConfigurations": {
+        "UpdateRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "ListSyncConfigurations",
+            "action": "UpdateRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetHost": {
+        "UseConnection": {
             "access_level": "Undocumented",
-            "action": "GetHost",
+            "action": "UseConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAppRegistrationHandshake": {
+        "GetInstallationUrl": {
             "access_level": "Undocumented",
-            "action": "StartAppRegistrationHandshake",
+            "action": "GetInstallationUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassConnection": {
+        "UpdateHost": {
             "access_level": "Undocumented",
-            "action": "PassConnection",
+            "action": "UpdateHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSyncBlockerSummary": {
+        "GetIndividualAccessToken": {
             "access_level": "Undocumented",
-            "action": "GetSyncBlockerSummary",
+            "action": "GetIndividualAccessToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInstallationUrl": {
+        "PassRepository": {
             "access_level": "Undocumented",
-            "action": "GetInstallationUrl",
+            "action": "PassRepository",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRepositorySyncDefinitions": {
+        "GetRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "ListRepositorySyncDefinitions",
+            "action": "GetRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteHost": {
+        "GetSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteHost",
+            "action": "GetSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterAppCode": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "RegisterAppCode",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIndividualAccessToken": {
+        "GetConnection": {
             "access_level": "Undocumented",
-            "action": "GetIndividualAccessToken",
+            "action": "GetConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConnectionInstallation": {
+        "GetHost": {
             "access_level": "Undocumented",
-            "action": "UpdateConnectionInstallation",
+            "action": "GetHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConnections": {
+        "StartOAuthHandshake": {
             "access_level": "Undocumented",
-            "action": "ListConnections",
+            "action": "StartOAuthHandshake",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRepositoryLink": {
+        "UpdateConnectionInstallation": {
             "access_level": "Undocumented",
-            "action": "DeleteRepositoryLink",
+            "action": "UpdateConnectionInstallation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRepositoryLink": {
+        "ListHosts": {
             "access_level": "Undocumented",
-            "action": "UpdateRepositoryLink",
+            "action": "ListHosts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListHosts": {
+        "StartAppRegistrationHandshake": {
             "access_level": "Undocumented",
-            "action": "ListHosts",
+            "action": "StartAppRegistrationHandshake",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRepository": {
+        "ListSyncConfigurations": {
             "access_level": "Undocumented",
-            "action": "PassRepository",
+            "action": "ListSyncConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRepositorySyncStatus": {
+        "CreateSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetRepositorySyncStatus",
+            "action": "CreateSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConnection": {
+        "RegisterAppCode": {
             "access_level": "Undocumented",
-            "action": "DeleteConnection",
+            "action": "RegisterAppCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRepositoryLinks": {
+        "DeleteConnection": {
             "access_level": "Undocumented",
-            "action": "ListRepositoryLinks",
+            "action": "DeleteConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UpdateSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UpdateSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSyncConfiguration": {
+        "CreateHost": {
             "access_level": "Undocumented",
-            "action": "CreateSyncConfiguration",
+            "action": "CreateHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "codedeploy": {
@@ -29074,121 +29074,121 @@
             "access_level": "Undocumented",
             "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListScans": {
+        "ListFindingsMetrics": {
             "access_level": "Undocumented",
-            "action": "ListScans",
+            "action": "ListFindingsMetrics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteScansByCategory": {
+        "GetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteScansByCategory",
+            "action": "GetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateScan": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountConfiguration": {
+        "GetFindings": {
             "access_level": "Undocumented",
-            "action": "GetAccountConfiguration",
+            "action": "GetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindings": {
+        "DeleteScansByCategory": {
             "access_level": "Undocumented",
-            "action": "ListFindings",
+            "action": "DeleteScansByCategory",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountConfiguration": {
+        "GetMetricsSummary": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountConfiguration",
+            "action": "GetMetricsSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateScan": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateScan",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetScan": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetScan",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindingsMetrics": {
+        "GetScan": {
             "access_level": "Undocumented",
-            "action": "ListFindingsMetrics",
+            "action": "GetScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "BatchGetFindings": {
             "access_level": "Undocumented",
             "action": "BatchGetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdateAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUploadUrl": {
+        "ListScans": {
             "access_level": "Undocumented",
-            "action": "CreateUploadUrl",
+            "action": "ListScans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFindings": {
+        "ListFindings": {
             "access_level": "Undocumented",
-            "action": "GetFindings",
+            "action": "ListFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetricsSummary": {
+        "CreateUploadUrl": {
             "access_level": "Undocumented",
-            "action": "GetMetricsSummary",
+            "action": "CreateUploadUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "codepipeline": {
@@ -37783,25 +37783,25 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "consolidatedbilling": {
-        "GetAccountBillingRole": {
+        "ListLinkedAccounts": {
             "access_level": "Undocumented",
-            "action": "GetAccountBillingRole",
+            "action": "ListLinkedAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListLinkedAccounts": {
+        "GetAccountBillingRole": {
             "access_level": "Undocumented",
-            "action": "ListLinkedAccounts",
+            "action": "GetAccountBillingRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "controlcatalog": {
@@ -38377,65 +38377,65 @@
             "orphan": false,
             "resources": [
                 "LandingZone"
             ]
         }
     },
     "cost-optimization-hub": {
-        "ListRecommendations": {
+        "UpdatePreferences": {
             "access_level": "Undocumented",
-            "action": "ListRecommendations",
+            "action": "UpdatePreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnrollmentStatus": {
+        "ListRecommendations": {
             "access_level": "Undocumented",
-            "action": "UpdateEnrollmentStatus",
+            "action": "ListRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecommendation": {
+        "GetPreferences": {
             "access_level": "Undocumented",
-            "action": "GetRecommendation",
+            "action": "GetPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePreferences": {
+        "ListEnrollmentStatuses": {
             "access_level": "Undocumented",
-            "action": "UpdatePreferences",
+            "action": "ListEnrollmentStatuses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRecommendationSummaries": {
+        "UpdateEnrollmentStatus": {
             "access_level": "Undocumented",
-            "action": "ListRecommendationSummaries",
+            "action": "UpdateEnrollmentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnrollmentStatuses": {
+        "GetRecommendation": {
             "access_level": "Undocumented",
-            "action": "ListEnrollmentStatuses",
+            "action": "GetRecommendation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPreferences": {
+        "ListRecommendationSummaries": {
             "access_level": "Undocumented",
-            "action": "GetPreferences",
+            "action": "ListRecommendationSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cur": {
@@ -40272,1065 +40272,1065 @@
             "orphan": false,
             "resources": [
                 "taskexecution"
             ]
         }
     },
     "datazone": {
-        "RejectPredictions": {
+        "CreateDomain": {
             "access_level": "Undocumented",
-            "action": "RejectPredictions",
+            "action": "CreateDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSubscriptionTarget": {
+        "RevokeSubscription": {
             "access_level": "Undocumented",
-            "action": "UpdateSubscriptionTarget",
+            "action": "RevokeSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RevokeSubscription": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "RevokeSubscription",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTimeSeriesDataPoints": {
+        "ListAccountEnvironments": {
             "access_level": "Undocumented",
-            "action": "DeleteTimeSeriesDataPoints",
+            "action": "ListAccountEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateListingChangeSet": {
+        "GetEnvironmentCredentials": {
             "access_level": "Undocumented",
-            "action": "CreateListingChangeSet",
+            "action": "GetEnvironmentCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteListing": {
+        "DeleteTimeSeriesDataPoints": {
             "access_level": "Undocumented",
-            "action": "DeleteListing",
+            "action": "DeleteTimeSeriesDataPoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscriptionRequest": {
+        "GetAsset": {
             "access_level": "Undocumented",
-            "action": "CreateSubscriptionRequest",
+            "action": "GetAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentBlueprint": {
+        "GetDataSource": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentBlueprint",
+            "action": "GetDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PostTimeSeriesDataPoints": {
+        "GetSubscriptionGrant": {
             "access_level": "Undocumented",
-            "action": "PostTimeSeriesDataPoints",
+            "action": "GetSubscriptionGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAsset": {
+        "ListSubscriptions": {
             "access_level": "Undocumented",
-            "action": "DeleteAsset",
+            "action": "ListSubscriptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentProfile": {
+        "StartMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentProfile",
+            "action": "StartMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTimeSeriesDataPoint": {
+        "GetEnvironmentBlueprintConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetTimeSeriesDataPoint",
+            "action": "GetEnvironmentBlueprintConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGlossary": {
+        "UpdateEnvironmentConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateGlossary",
+            "action": "UpdateEnvironmentConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupProfile": {
+        "GetEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "GetGroupProfile",
+            "action": "GetEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSource": {
+        "CreateGroupProfile": {
             "access_level": "Undocumented",
-            "action": "GetDataSource",
+            "action": "CreateGroupProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountEnvironments": {
+        "DeleteSubscriptionGrant": {
             "access_level": "Undocumented",
-            "action": "ListAccountEnvironments",
+            "action": "DeleteSubscriptionGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetListing": {
+        "CreateAssetRevision": {
             "access_level": "Undocumented",
-            "action": "GetListing",
+            "action": "CreateAssetRevision",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchTypes": {
+        "RejectPredictions": {
             "access_level": "Undocumented",
-            "action": "SearchTypes",
+            "action": "RejectPredictions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGlossaryTerm": {
+        "DeleteEnvironmentBlueprintConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteGlossaryTerm",
+            "action": "DeleteEnvironmentBlueprintConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSubscriptionRequest": {
+        "CreateAsset": {
             "access_level": "Undocumented",
-            "action": "UpdateSubscriptionRequest",
+            "action": "CreateAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentActionLink": {
+        "GetTimeSeriesDataPoint": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentActionLink",
+            "action": "GetTimeSeriesDataPoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDomain": {
+        "DeleteGlossary": {
             "access_level": "Undocumented",
-            "action": "GetDomain",
+            "action": "DeleteGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGlossary": {
+        "CancelSubscription": {
             "access_level": "Undocumented",
-            "action": "GetGlossary",
+            "action": "CancelSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironments": {
+        "ProvisionDomain": {
             "access_level": "Undocumented",
-            "action": "ListEnvironments",
+            "action": "ProvisionDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGlossaryTerm": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateGlossaryTerm",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscriptionGrant": {
+        "CreateProjectMembership": {
             "access_level": "Undocumented",
-            "action": "CreateSubscriptionGrant",
+            "action": "CreateProjectMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFormType": {
+        "AcceptPredictions": {
             "access_level": "Undocumented",
-            "action": "DeleteFormType",
+            "action": "AcceptPredictions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssetRevision": {
+        "ListEnvironmentProfiles": {
             "access_level": "Undocumented",
-            "action": "CreateAssetRevision",
+            "action": "ListEnvironmentProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSubscriptionRequest": {
+        "ListGroupsForUser": {
             "access_level": "Undocumented",
-            "action": "DeleteSubscriptionRequest",
+            "action": "ListGroupsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscriptionTarget": {
+        "UpdateDataSourceRunActivities": {
             "access_level": "Undocumented",
-            "action": "CreateSubscriptionTarget",
+            "action": "UpdateDataSourceRunActivities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProjectMembership": {
+        "CreateListingChangeSet": {
             "access_level": "Undocumented",
-            "action": "DeleteProjectMembership",
+            "action": "CreateListingChangeSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscription": {
+        "GetListing": {
             "access_level": "Undocumented",
-            "action": "GetSubscription",
+            "action": "GetListing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDomains": {
+        "DeleteDomain": {
             "access_level": "Undocumented",
-            "action": "ListDomains",
+            "action": "DeleteDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateFormType": {
             "access_level": "Undocumented",
             "action": "CreateFormType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionRequestDetails": {
+        "PutDomainSharingPolicy": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionRequestDetails",
+            "action": "PutDomainSharingPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionGrant": {
+        "SsoLogout": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionGrant",
+            "action": "SsoLogout",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironment": {
+        "SearchUserProfiles": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironment",
+            "action": "SearchUserProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Search": {
+        "CreateSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "Search",
+            "action": "CreateSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemovePolicyGrant": {
+        "GetGroupProfile": {
             "access_level": "Undocumented",
-            "action": "RemovePolicyGrant",
+            "action": "GetGroupProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProjectMembership": {
+        "GetEnvironmentActionLink": {
             "access_level": "Undocumented",
-            "action": "CreateProjectMembership",
+            "action": "GetEnvironmentActionLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDomain": {
+        "GetDomain": {
             "access_level": "Undocumented",
-            "action": "UpdateDomain",
+            "action": "GetDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionTarget": {
+        "GetSubscriptionEligibility": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionTarget",
+            "action": "GetSubscriptionEligibility",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "DeleteDomainSharingPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "DeleteDomainSharingPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIamPortalLoginUrl": {
+        "GetAssetType": {
             "access_level": "Undocumented",
-            "action": "GetIamPortalLoginUrl",
+            "action": "GetAssetType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironmentBlueprintConfiguration": {
+        "Search": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironmentBlueprintConfiguration",
+            "action": "Search",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSourceRunActivities": {
+        "SearchListings": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSourceRunActivities",
+            "action": "SearchListings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSubscription": {
+        "CreateEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "CancelSubscription",
+            "action": "CreateEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWarehouseMetadata": {
+        "CreateEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "ListWarehouseMetadata",
+            "action": "CreateEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironmentProfile": {
+        "ValidatePassRole": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironmentProfile",
+            "action": "ValidatePassRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchGroupProfiles": {
+        "DeleteSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "SearchGroupProfiles",
+            "action": "DeleteSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserProfile": {
+        "ListAssetRevisions": {
             "access_level": "Undocumented",
-            "action": "GetUserProfile",
+            "action": "ListAssetRevisions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "UpdateGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "UpdateGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGlossary": {
+        "ListProjectMemberships": {
             "access_level": "Undocumented",
-            "action": "CreateGlossary",
+            "action": "ListProjectMemberships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptionTargets": {
+        "ListWarehouseMetadata": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptionTargets",
+            "action": "ListWarehouseMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssetRevisions": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "ListAssetRevisions",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptionRequests": {
+        "SearchTypes": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptionRequests",
+            "action": "SearchTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentBlueprintConfigurationSummaries": {
+        "GetProject": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentBlueprintConfigurationSummaries",
+            "action": "GetProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSubscriptionTarget": {
+        "ListSubscriptionGrants": {
             "access_level": "Undocumented",
-            "action": "DeleteSubscriptionTarget",
+            "action": "ListSubscriptionGrants",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDomainSharingPolicy": {
+        "ListEnvironments": {
             "access_level": "Undocumented",
-            "action": "DeleteDomainSharingPolicy",
+            "action": "ListEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProject": {
+        "DeleteEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "CreateProject",
+            "action": "DeleteEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGlossaryTerm": {
+        "PostTimeSeriesDataPoints": {
             "access_level": "Undocumented",
-            "action": "GetGlossaryTerm",
+            "action": "PostTimeSeriesDataPoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMetadataGenerationRuns": {
+        "AcceptSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "ListMetadataGenerationRuns",
+            "action": "AcceptSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUserProfile": {
+        "SearchGroupProfiles": {
             "access_level": "Undocumented",
-            "action": "UpdateUserProfile",
+            "action": "SearchGroupProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAsset": {
+        "UpdateUserProfile": {
             "access_level": "Undocumented",
-            "action": "GetAsset",
+            "action": "UpdateUserProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSourceRun": {
+        "CreateSubscriptionGrant": {
             "access_level": "Undocumented",
-            "action": "GetDataSourceRun",
+            "action": "CreateSubscriptionGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMetadataGenerationRun": {
+        "DeleteFormType": {
             "access_level": "Undocumented",
-            "action": "StartMetadataGenerationRun",
+            "action": "DeleteFormType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProject": {
+        "CreateSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "UpdateProject",
+            "action": "CreateSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFormType": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetFormType",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListDataSourceRunActivities": {
             "access_level": "Undocumented",
             "action": "ListDataSourceRunActivities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListNotifications": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListNotifications",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironment": {
+        "StopMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "GetEnvironment",
+            "action": "StopMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptionGrants": {
+        "GetIamPortalLoginUrl": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptionGrants",
+            "action": "GetIamPortalLoginUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentBlueprintConfiguration": {
+        "CreateGlossary": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentBlueprintConfiguration",
+            "action": "CreateGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironmentProfile": {
+        "DeleteProjectMembership": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironmentProfile",
+            "action": "DeleteProjectMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDomain": {
+        "CreateUserProfile": {
             "access_level": "Undocumented",
-            "action": "CreateDomain",
+            "action": "CreateUserProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "GetSubscription": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "GetSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentBlueprints": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentBlueprints",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddPolicyGrant": {
+        "ListEnvironmentBlueprints": {
             "access_level": "Undocumented",
-            "action": "AddPolicyGrant",
+            "action": "ListEnvironmentBlueprints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutDomainSharingPolicy": {
+        "UpdateEnvironmentDeploymentStatus": {
             "access_level": "Undocumented",
-            "action": "PutDomainSharingPolicy",
+            "action": "UpdateEnvironmentDeploymentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGlossaryTerm": {
+        "DeleteProject": {
             "access_level": "Undocumented",
-            "action": "CreateGlossaryTerm",
+            "action": "DeleteProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionEligibility": {
+        "ListMetadataGenerationRuns": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionEligibility",
+            "action": "ListMetadataGenerationRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironmentBlueprint": {
+        "CreateEnvironment": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironmentBlueprint",
+            "action": "CreateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSubscriptionGrant": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "DeleteSubscriptionGrant",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentBlueprint": {
+        "ListSubscriptionTargets": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentBlueprint",
+            "action": "ListSubscriptionTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssetType": {
+        "GetDomainSharingPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteAssetType",
+            "action": "GetDomainSharingPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetadataGenerationRun": {
+        "RefreshToken": {
             "access_level": "Undocumented",
-            "action": "GetMetadataGenerationRun",
+            "action": "RefreshToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDomainSharingPolicy": {
+        "ListEnvironmentBlueprintConfigurations": {
             "access_level": "Undocumented",
-            "action": "GetDomainSharingPolicy",
+            "action": "ListEnvironmentBlueprintConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SsoLogout": {
+        "GetEnvironment": {
             "access_level": "Undocumented",
-            "action": "SsoLogout",
+            "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotifications": {
+        "GetSubscriptionRequestDetails": {
             "access_level": "Undocumented",
-            "action": "ListNotifications",
+            "action": "GetSubscriptionRequestDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyGrants": {
+        "CreateGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "ListPolicyGrants",
+            "action": "CreateGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProject": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "DeleteProject",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupsForUser": {
+        "DeleteAsset": {
             "access_level": "Undocumented",
-            "action": "ListGroupsForUser",
+            "action": "DeleteAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentDeploymentStatus": {
+        "ListTimeSeriesDataPoints": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentDeploymentStatus",
+            "action": "ListTimeSeriesDataPoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentCredentials": {
+        "DeleteSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentCredentials",
+            "action": "DeleteSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjects": {
+        "GetUserProfile": {
             "access_level": "Undocumented",
-            "action": "ListProjects",
+            "action": "GetUserProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchListings": {
+        "GetEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "SearchListings",
+            "action": "GetEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ProvisionDomain": {
+        "UpdateEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "ProvisionDomain",
+            "action": "UpdateEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironment": {
+        "GetGlossary": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironment",
+            "action": "GetGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMetadataGenerationRun": {
+        "UpdateSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "CancelMetadataGenerationRun",
+            "action": "UpdateSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchUserProfiles": {
+        "SsoLogin": {
             "access_level": "Undocumented",
-            "action": "SearchUserProfiles",
+            "action": "SsoLogin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopMetadataGenerationRun": {
+        "GetFormType": {
             "access_level": "Undocumented",
-            "action": "StopMetadataGenerationRun",
+            "action": "GetFormType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "UpdateSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "UpdateSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDomain": {
+        "UpdateDomain": {
             "access_level": "Undocumented",
-            "action": "DeleteDomain",
+            "action": "UpdateDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGroupProfile": {
+        "AddPolicyGrant": {
             "access_level": "Undocumented",
-            "action": "UpdateGroupProfile",
+            "action": "AddPolicyGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RefreshToken": {
+        "GetSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "RefreshToken",
+            "action": "GetSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectSubscriptionRequest": {
+        "ListPolicyGrants": {
             "access_level": "Undocumented",
-            "action": "RejectSubscriptionRequest",
+            "action": "ListPolicyGrants",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptPredictions": {
+        "ListEnvironmentBlueprintConfigurationSummaries": {
             "access_level": "Undocumented",
-            "action": "AcceptPredictions",
+            "action": "ListEnvironmentBlueprintConfigurationSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptions": {
+        "RejectSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptions",
+            "action": "RejectSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTimeSeriesDataPoints": {
+        "UpdateEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListTimeSeriesDataPoints",
+            "action": "UpdateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUserProfile": {
+        "UpdateGroupProfile": {
             "access_level": "Undocumented",
-            "action": "CreateUserProfile",
+            "action": "UpdateGroupProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironment": {
+        "DeleteEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironment",
+            "action": "DeleteEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartDataSourceRun": {
+        "DeleteListing": {
             "access_level": "Undocumented",
-            "action": "StartDataSourceRun",
+            "action": "DeleteListing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentProfile": {
+        "ListSubscriptionRequests": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentProfile",
+            "action": "ListSubscriptionRequests",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutEnvironmentBlueprintConfiguration": {
+        "ListDataSourceRuns": {
             "access_level": "Undocumented",
-            "action": "PutEnvironmentBlueprintConfiguration",
+            "action": "ListDataSourceRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssetType": {
+        "GetMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "CreateAssetType",
+            "action": "GetMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGlossary": {
+        "UpdateGlossary": {
             "access_level": "Undocumented",
-            "action": "DeleteGlossary",
+            "action": "UpdateGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironmentBlueprint": {
+        "UpdateProject": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironmentBlueprint",
+            "action": "UpdateProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidatePassRole": {
+        "UpdateSubscriptionGrantStatus": {
             "access_level": "Undocumented",
-            "action": "ValidatePassRole",
+            "action": "UpdateSubscriptionGrantStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptSubscriptionRequest": {
+        "GetDataSourceRun": {
             "access_level": "Undocumented",
-            "action": "AcceptSubscriptionRequest",
+            "action": "GetDataSourceRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSubscriptionGrantStatus": {
+        "PutEnvironmentBlueprintConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateSubscriptionGrantStatus",
+            "action": "PutEnvironmentBlueprintConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGroupProfile": {
+        "StartDataSourceRun": {
             "access_level": "Undocumented",
-            "action": "CreateGroupProfile",
+            "action": "StartDataSourceRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjectMemberships": {
+        "ListProjects": {
             "access_level": "Undocumented",
-            "action": "ListProjectMemberships",
+            "action": "ListProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssetType": {
+        "ListDomains": {
             "access_level": "Undocumented",
-            "action": "GetAssetType",
+            "action": "ListDomains",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SsoLogin": {
+        "CreateProject": {
             "access_level": "Undocumented",
-            "action": "SsoLogin",
+            "action": "CreateProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentConfiguration": {
+        "CreateAssetType": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentConfiguration",
+            "action": "CreateAssetType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentBlueprintConfigurations": {
+        "GetGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentBlueprintConfigurations",
+            "action": "GetGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourceRuns": {
+        "DeleteEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListDataSourceRuns",
+            "action": "DeleteEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProject": {
+        "UpdateEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "GetProject",
+            "action": "UpdateEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentProfiles": {
+        "CancelMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentProfiles",
+            "action": "CancelMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAsset": {
+        "RemovePolicyGrant": {
             "access_level": "Undocumented",
-            "action": "CreateAsset",
+            "action": "RemovePolicyGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteAssetType": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteAssetType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "dax": {
@@ -41724,833 +41724,833 @@
             "condition_keys": [],
             "description": "Grants permission to update query tab",
             "orphan": false,
             "resources": []
         }
     },
     "deadline": {
-        "SearchTasks": {
+        "CreateLicenseEndpoint": {
             "access_level": "Undocumented",
-            "action": "SearchTasks",
+            "action": "CreateLicenseEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "StartSessionsStatisticsAggregation": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "StartSessionsStatisticsAggregation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFleet": {
+        "GetTask": {
             "access_level": "Undocumented",
-            "action": "UpdateFleet",
+            "action": "GetTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorker": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetWorker",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStorageProfile": {
+        "AssociateMemberToFleet": {
             "access_level": "Undocumented",
-            "action": "GetStorageProfile",
+            "action": "AssociateMemberToFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToFleet": {
+        "DeleteFleet": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToFleet",
+            "action": "DeleteFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAvailableMeteredProducts": {
+        "GetSessionsStatisticsAggregation": {
             "access_level": "Undocumented",
-            "action": "ListAvailableMeteredProducts",
+            "action": "GetSessionsStatisticsAggregation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWorker": {
+        "GetFarm": {
             "access_level": "Undocumented",
-            "action": "CreateWorker",
+            "action": "GetFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CopyJobTemplate": {
+        "ListSessionsForWorker": {
             "access_level": "Undocumented",
-            "action": "CopyJobTemplate",
+            "action": "ListSessionsForWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMonitor": {
+        "CreateQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "CreateMonitor",
+            "action": "CreateQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToQueue": {
+        "DeleteWorker": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToQueue",
+            "action": "DeleteWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFleet": {
+        "GetSessionAction": {
             "access_level": "Undocumented",
-            "action": "CreateFleet",
+            "action": "GetSessionAction",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSessionsStatisticsAggregation": {
+        "CreateQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "GetSessionsStatisticsAggregation",
+            "action": "CreateQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueueEnvironment": {
+        "UpdateStorageProfile": {
             "access_level": "Undocumented",
-            "action": "GetQueueEnvironment",
+            "action": "UpdateStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetStorageProfile": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSession": {
+        "AssumeQueueRoleForUser": {
             "access_level": "Undocumented",
-            "action": "GetSession",
+            "action": "AssumeQueueRoleForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueue": {
+        "ListFleets": {
             "access_level": "Undocumented",
-            "action": "GetQueue",
+            "action": "ListFleets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutMeteredProduct": {
+        "GetStorageProfileForQueue": {
             "access_level": "Undocumented",
-            "action": "PutMeteredProduct",
+            "action": "GetStorageProfileForQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWorker": {
+        "SearchJobs": {
             "access_level": "Undocumented",
-            "action": "DeleteWorker",
+            "action": "SearchJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchWorkers": {
+        "SearchTasks": {
             "access_level": "Undocumented",
-            "action": "SearchWorkers",
+            "action": "SearchTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStep": {
+        "GetMonitor": {
             "access_level": "Undocumented",
-            "action": "GetStep",
+            "action": "GetMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeQueueRoleForRead": {
+        "AssociateMemberToQueue": {
             "access_level": "Undocumented",
-            "action": "AssumeQueueRoleForRead",
+            "action": "AssociateMemberToQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFleets": {
+        "AssociateMemberToFarm": {
             "access_level": "Undocumented",
-            "action": "ListFleets",
+            "action": "AssociateMemberToFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMeteredProduct": {
+        "ListFarms": {
             "access_level": "Undocumented",
-            "action": "DeleteMeteredProduct",
+            "action": "ListFarms",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteBudget": {
+        "ListStorageProfiles": {
             "access_level": "Undocumented",
-            "action": "DeleteBudget",
+            "action": "ListStorageProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateBudget": {
+        "GetApplicationVersion": {
             "access_level": "Undocumented",
-            "action": "UpdateBudget",
+            "action": "GetApplicationVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchJobs": {
+        "UpdateFleet": {
             "access_level": "Undocumented",
-            "action": "SearchJobs",
+            "action": "UpdateFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateStorageProfile": {
+        "CreateFleet": {
             "access_level": "Undocumented",
-            "action": "CreateStorageProfile",
+            "action": "CreateFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateJob": {
+        "GetSession": {
             "access_level": "Undocumented",
-            "action": "UpdateJob",
+            "action": "GetSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetJobEntity": {
+        "AssumeQueueRoleForRead": {
             "access_level": "Undocumented",
-            "action": "BatchGetJobEntity",
+            "action": "AssumeQueueRoleForRead",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFarm": {
+        "DeleteLicenseEndpoint": {
             "access_level": "Undocumented",
-            "action": "CreateFarm",
+            "action": "DeleteLicenseEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSteps": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListSteps",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueueFleetAssociation": {
+        "ListStepConsumers": {
             "access_level": "Undocumented",
-            "action": "GetQueueFleetAssociation",
+            "action": "ListStepConsumers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBudget": {
+        "GetFleet": {
             "access_level": "Undocumented",
-            "action": "GetBudget",
+            "action": "GetFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMonitor": {
+        "ListJobMembers": {
             "access_level": "Undocumented",
-            "action": "DeleteMonitor",
+            "action": "ListJobMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSessionsForWorker": {
+        "AssociateMemberToJob": {
             "access_level": "Undocumented",
-            "action": "ListSessionsForWorker",
+            "action": "AssociateMemberToJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQueueFleetAssociation": {
+        "ListSessions": {
             "access_level": "Undocumented",
-            "action": "UpdateQueueFleetAssociation",
+            "action": "ListSessions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQueueFleetAssociation": {
+        "ListAvailableMeteredProducts": {
             "access_level": "Undocumented",
-            "action": "CreateQueueFleetAssociation",
+            "action": "ListAvailableMeteredProducts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStorageProfiles": {
+        "GetWorker": {
             "access_level": "Undocumented",
-            "action": "ListStorageProfiles",
+            "action": "GetWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueueMembers": {
+        "ListStepDependencies": {
             "access_level": "Undocumented",
-            "action": "ListQueueMembers",
+            "action": "ListStepDependencies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSessions": {
+        "AssumeFleetRoleForRead": {
             "access_level": "Undocumented",
-            "action": "ListSessions",
+            "action": "AssumeFleetRoleForRead",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromJob": {
+        "ListStorageProfilesForQueue": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromJob",
+            "action": "ListStorageProfilesForQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromFarm": {
+        "AssumeFleetRoleForWorker": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromFarm",
+            "action": "AssumeFleetRoleForWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStorageProfilesForQueue": {
+        "ListQueueMembers": {
             "access_level": "Undocumented",
-            "action": "ListStorageProfilesForQueue",
+            "action": "ListQueueMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetApplicationVersion": {
+        "CreateQueue": {
             "access_level": "Undocumented",
-            "action": "GetApplicationVersion",
+            "action": "CreateQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFarm": {
+        "GetStep": {
             "access_level": "Undocumented",
-            "action": "GetFarm",
+            "action": "GetStep",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQueueEnvironment": {
+        "DeleteQueue": {
             "access_level": "Undocumented",
-            "action": "CreateQueueEnvironment",
+            "action": "DeleteQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLicenseEndpoint": {
+        "ListLicenseEndpoints": {
             "access_level": "Undocumented",
-            "action": "DeleteLicenseEndpoint",
+            "action": "ListLicenseEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWorker": {
+        "GetBudget": {
             "access_level": "Undocumented",
-            "action": "UpdateWorker",
+            "action": "GetBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStorageProfile": {
+        "DisassociateMemberFromJob": {
             "access_level": "Undocumented",
-            "action": "UpdateStorageProfile",
+            "action": "DisassociateMemberFromJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromQueue": {
+        "GetQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromQueue",
+            "action": "GetQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQueue": {
+        "GetJob": {
             "access_level": "Undocumented",
-            "action": "UpdateQueue",
+            "action": "GetJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLicenseEndpoint": {
+        "ListMeteredProducts": {
             "access_level": "Undocumented",
-            "action": "GetLicenseEndpoint",
+            "action": "ListMeteredProducts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSessionAction": {
+        "ListSessionActions": {
             "access_level": "Undocumented",
-            "action": "GetSessionAction",
+            "action": "ListSessionActions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueueFleetAssociations": {
+        "BatchGetJobEntity": {
             "access_level": "Undocumented",
-            "action": "ListQueueFleetAssociations",
+            "action": "BatchGetJobEntity",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateJob": {
+        "ListFarmMembers": {
             "access_level": "Undocumented",
-            "action": "CreateJob",
+            "action": "ListFarmMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFarm": {
+        "UpdateBudget": {
             "access_level": "Undocumented",
-            "action": "DeleteFarm",
+            "action": "UpdateBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueueEnvironment": {
+        "ListBudgets": {
             "access_level": "Undocumented",
-            "action": "DeleteQueueEnvironment",
+            "action": "ListBudgets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMeteredProducts": {
+        "ListSteps": {
             "access_level": "Undocumented",
-            "action": "ListMeteredProducts",
+            "action": "ListSteps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStepDependencies": {
+        "CreateWorker": {
             "access_level": "Undocumented",
-            "action": "ListStepDependencies",
+            "action": "CreateWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTask": {
+        "CreateMonitor": {
             "access_level": "Undocumented",
-            "action": "GetTask",
+            "action": "CreateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQueueEnvironment": {
+        "CopyJobTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdateQueueEnvironment",
+            "action": "CopyJobTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListJobMembers": {
+        "UpdateWorker": {
             "access_level": "Undocumented",
-            "action": "ListJobMembers",
+            "action": "UpdateWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFarmMembers": {
+        "DeleteFarm": {
             "access_level": "Undocumented",
-            "action": "ListFarmMembers",
+            "action": "DeleteFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetJob": {
+        "ListTasks": {
             "access_level": "Undocumented",
-            "action": "GetJob",
+            "action": "ListTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchSteps": {
+        "UpdateQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "SearchSteps",
+            "action": "UpdateQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFarms": {
+        "ListMonitors": {
             "access_level": "Undocumented",
-            "action": "ListFarms",
+            "action": "ListMonitors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueueFleetAssociation": {
+        "UpdateWorkerSchedule": {
             "access_level": "Undocumented",
-            "action": "DeleteQueueFleetAssociation",
+            "action": "UpdateWorkerSchedule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStorageProfileForQueue": {
+        "DisassociateMemberFromFarm": {
             "access_level": "Undocumented",
-            "action": "GetStorageProfileForQueue",
+            "action": "DisassociateMemberFromFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeFleetRoleForRead": {
+        "ListFleetMembers": {
             "access_level": "Undocumented",
-            "action": "AssumeFleetRoleForRead",
+            "action": "ListFleetMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartSessionsStatisticsAggregation": {
+        "CreateJob": {
             "access_level": "Undocumented",
-            "action": "StartSessionsStatisticsAggregation",
+            "action": "CreateJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkers": {
+        "UpdateQueue": {
             "access_level": "Undocumented",
-            "action": "ListWorkers",
+            "action": "UpdateQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMonitor": {
+        "DeleteMonitor": {
             "access_level": "Undocumented",
-            "action": "UpdateMonitor",
+            "action": "DeleteMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListLicenseEndpoints": {
+        "ListJobs": {
             "access_level": "Undocumented",
-            "action": "ListLicenseEndpoints",
+            "action": "ListJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLicenseEndpoint": {
+        "SearchSteps": {
             "access_level": "Undocumented",
-            "action": "CreateLicenseEndpoint",
+            "action": "SearchSteps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFarm": {
+        "DisassociateMemberFromQueue": {
             "access_level": "Undocumented",
-            "action": "UpdateFarm",
+            "action": "DisassociateMemberFromQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTasks": {
+        "DeleteQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "ListTasks",
+            "action": "DeleteQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToJob": {
+        "UpdateStep": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToJob",
+            "action": "UpdateStep",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListBudgets": {
+        "CreateStorageProfile": {
             "access_level": "Undocumented",
-            "action": "ListBudgets",
+            "action": "CreateStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteStorageProfile": {
             "access_level": "Undocumented",
             "action": "DeleteStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateBudget": {
+        "UpdateSession": {
             "access_level": "Undocumented",
-            "action": "CreateBudget",
+            "action": "UpdateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSessionActions": {
+        "GetQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListSessionActions",
+            "action": "GetQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueues": {
+        "DisassociateMemberFromFleet": {
             "access_level": "Undocumented",
-            "action": "ListQueues",
+            "action": "DisassociateMemberFromFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFleet": {
+        "GetLicenseEndpoint": {
             "access_level": "Undocumented",
-            "action": "DeleteFleet",
+            "action": "GetLicenseEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToFarm": {
+        "ListQueueFleetAssociations": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToFarm",
+            "action": "ListQueueFleetAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeQueueRoleForWorker": {
+        "PutMeteredProduct": {
             "access_level": "Undocumented",
-            "action": "AssumeQueueRoleForWorker",
+            "action": "PutMeteredProduct",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSession": {
+        "UpdateFarm": {
             "access_level": "Undocumented",
-            "action": "UpdateSession",
+            "action": "UpdateFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueue": {
+        "CreateBudget": {
             "access_level": "Undocumented",
-            "action": "DeleteQueue",
+            "action": "CreateBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWorkerSchedule": {
+        "DeleteQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "UpdateWorkerSchedule",
+            "action": "DeleteQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStep": {
+        "GetQueue": {
             "access_level": "Undocumented",
-            "action": "UpdateStep",
+            "action": "GetQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeQueueRoleForUser": {
+        "UpdateQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "AssumeQueueRoleForUser",
+            "action": "UpdateQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMonitor": {
+        "UpdateTask": {
             "access_level": "Undocumented",
-            "action": "GetMonitor",
+            "action": "UpdateTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFleetMembers": {
+        "UpdateJob": {
             "access_level": "Undocumented",
-            "action": "ListFleetMembers",
+            "action": "UpdateJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQueue": {
+        "AssumeQueueRoleForWorker": {
             "access_level": "Undocumented",
-            "action": "CreateQueue",
+            "action": "AssumeQueueRoleForWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeFleetRoleForWorker": {
+        "UpdateMonitor": {
             "access_level": "Undocumented",
-            "action": "AssumeFleetRoleForWorker",
+            "action": "UpdateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFleet": {
+        "SearchWorkers": {
             "access_level": "Undocumented",
-            "action": "GetFleet",
+            "action": "SearchWorkers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueueEnvironments": {
+        "CreateFarm": {
             "access_level": "Undocumented",
-            "action": "ListQueueEnvironments",
+            "action": "CreateFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTask": {
+        "ListQueues": {
             "access_level": "Undocumented",
-            "action": "UpdateTask",
+            "action": "ListQueues",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListJobs": {
+        "DeleteMeteredProduct": {
             "access_level": "Undocumented",
-            "action": "ListJobs",
+            "action": "DeleteMeteredProduct",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMonitors": {
+        "ListWorkers": {
             "access_level": "Undocumented",
-            "action": "ListMonitors",
+            "action": "ListWorkers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromFleet": {
+        "ListQueueEnvironments": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromFleet",
+            "action": "ListQueueEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStepConsumers": {
+        "DeleteBudget": {
             "access_level": "Undocumented",
-            "action": "ListStepConsumers",
+            "action": "DeleteBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "deepcomposer": {
@@ -65131,305 +65131,305 @@
             ],
             "description": "Grants permission to replace the current set of policies for the specified load balancer port with the specified set of policies",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
-        "DeleteRule": {
+        "ModifyTrustStore": {
             "access_level": "Undocumented",
-            "action": "DeleteRule",
+            "action": "ModifyTrustStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetGroupAttributes": {
+        "SetWebAcl": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetGroupAttributes",
+            "action": "SetWebAcl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTrustStoreCaCertificatesBundle": {
+        "DeleteListener": {
             "access_level": "Undocumented",
-            "action": "GetTrustStoreCaCertificatesBundle",
+            "action": "DeleteListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateListener": {
+        "ModifyRule": {
             "access_level": "Undocumented",
-            "action": "CreateListener",
+            "action": "ModifyRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetGroups": {
+        "DescribeTargetHealth": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetGroups",
+            "action": "DescribeTargetHealth",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveListenerCertificates": {
+        "DeregisterTargets": {
             "access_level": "Undocumented",
-            "action": "RemoveListenerCertificates",
+            "action": "DeregisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetWebAcl": {
+        "SetSubnets": {
             "access_level": "Undocumented",
-            "action": "SetWebAcl",
+            "action": "SetSubnets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTargetGroup": {
+        "DescribeTargetGroups": {
             "access_level": "Undocumented",
-            "action": "ModifyTargetGroup",
+            "action": "DescribeTargetGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteListener": {
+        "RemoveTrustStoreRevocations": {
             "access_level": "Undocumented",
-            "action": "DeleteListener",
+            "action": "RemoveTrustStoreRevocations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyListener": {
+        "CreateTrustStore": {
             "access_level": "Undocumented",
-            "action": "ModifyListener",
+            "action": "CreateTrustStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTrustStores": {
+        "CreateTargetGroup": {
             "access_level": "Undocumented",
-            "action": "DescribeTrustStores",
+            "action": "CreateTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSSLPolicies": {
+        "CreateListener": {
             "access_level": "Undocumented",
-            "action": "DescribeSSLPolicies",
+            "action": "CreateListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTrustStoreRevocations": {
+        "ModifyTargetGroupAttributes": {
             "access_level": "Undocumented",
-            "action": "DescribeTrustStoreRevocations",
+            "action": "ModifyTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetIpAddressType": {
+        "AddTrustStoreRevocations": {
             "access_level": "Undocumented",
-            "action": "SetIpAddressType",
+            "action": "AddTrustStoreRevocations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSubnets": {
+        "ModifyTargetGroup": {
             "access_level": "Undocumented",
-            "action": "SetSubnets",
+            "action": "ModifyTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterTargets": {
+        "GetTrustStoreCaCertificatesBundle": {
             "access_level": "Undocumented",
-            "action": "DeregisterTargets",
+            "action": "GetTrustStoreCaCertificatesBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTrustStore": {
+        "GetTrustStoreRevocationContent": {
             "access_level": "Undocumented",
-            "action": "CreateTrustStore",
+            "action": "GetTrustStoreRevocationContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetRulePriorities": {
+        "AddListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "SetRulePriorities",
+            "action": "AddListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityGroups": {
+        "DescribeTrustStores": {
             "access_level": "Undocumented",
-            "action": "SetSecurityGroups",
+            "action": "DescribeTrustStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetHealth": {
+        "DescribeListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetHealth",
+            "action": "DescribeListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTrustStoreAssociations": {
+        "CreateRule": {
             "access_level": "Undocumented",
-            "action": "DescribeTrustStoreAssociations",
+            "action": "CreateRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRule": {
+        "DescribeSSLPolicies": {
             "access_level": "Undocumented",
-            "action": "CreateRule",
+            "action": "DescribeSSLPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListeners": {
+        "SetIpAddressType": {
             "access_level": "Undocumented",
-            "action": "DescribeListeners",
+            "action": "SetIpAddressType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyRule": {
+        "DescribeTargetGroupAttributes": {
             "access_level": "Undocumented",
-            "action": "ModifyRule",
+            "action": "DescribeTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListenerCertificates": {
+        "DescribeTrustStoreAssociations": {
             "access_level": "Undocumented",
-            "action": "DescribeListenerCertificates",
+            "action": "DescribeTrustStoreAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "RegisterTargets": {
             "access_level": "Undocumented",
             "action": "RegisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeRules": {
+        "DescribeAccountLimits": {
             "access_level": "Undocumented",
-            "action": "DescribeRules",
+            "action": "DescribeAccountLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveTrustStoreRevocations": {
+        "DeleteRule": {
             "access_level": "Undocumented",
-            "action": "RemoveTrustStoreRevocations",
+            "action": "DeleteRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTargetGroup": {
+        "DescribeListeners": {
             "access_level": "Undocumented",
-            "action": "CreateTargetGroup",
+            "action": "DescribeListeners",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAccountLimits": {
+        "SetSecurityGroups": {
             "access_level": "Undocumented",
-            "action": "DescribeAccountLimits",
+            "action": "SetSecurityGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTargetGroupAttributes": {
+        "DeleteTrustStore": {
             "access_level": "Undocumented",
-            "action": "ModifyTargetGroupAttributes",
+            "action": "DeleteTrustStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddTrustStoreRevocations": {
+        "SetRulePriorities": {
             "access_level": "Undocumented",
-            "action": "AddTrustStoreRevocations",
+            "action": "SetRulePriorities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteTargetGroup": {
             "access_level": "Undocumented",
             "action": "DeleteTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTrustStore": {
+        "DescribeTrustStoreRevocations": {
             "access_level": "Undocumented",
-            "action": "DeleteTrustStore",
+            "action": "DescribeTrustStoreRevocations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddListenerCertificates": {
+        "RemoveListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "AddListenerCertificates",
+            "action": "RemoveListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTrustStoreRevocationContent": {
+        "DescribeRules": {
             "access_level": "Undocumented",
-            "action": "GetTrustStoreRevocationContent",
+            "action": "DescribeRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTrustStore": {
+        "ModifyListener": {
             "access_level": "Undocumented",
-            "action": "ModifyTrustStore",
+            "action": "ModifyListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "elasticmapreduce": {
@@ -67130,305 +67130,305 @@
             "orphan": false,
             "resources": [
                 "application"
             ]
         }
     },
     "entityresolution": {
-        "GetMatchingWorkflow": {
+        "GetIdNamespace": {
             "access_level": "Undocumented",
-            "action": "GetMatchingWorkflow",
+            "action": "GetIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdMappingWorkflows": {
+        "GetMatchId": {
             "access_level": "Undocumented",
-            "action": "ListIdMappingWorkflows",
+            "action": "GetMatchId",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddPolicyStatement": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "AddPolicyStatement",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSchemaMapping": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateSchemaMapping",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartIdMappingJob": {
+        "UpdateMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "StartIdMappingJob",
+            "action": "UpdateMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSchemaMapping": {
+        "UpdateIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "DeleteSchemaMapping",
+            "action": "UpdateIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyStatement": {
+        "UseIdNamespace": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyStatement",
+            "action": "UseIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMatchId": {
+        "GetSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "GetMatchId",
+            "action": "GetSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutPolicy": {
+        "CreateSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "PutPolicy",
+            "action": "CreateSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMatchingWorkflows": {
+        "ListIdNamespaces": {
             "access_level": "Undocumented",
-            "action": "ListMatchingWorkflows",
+            "action": "ListIdNamespaces",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdMappingWorkflow": {
+        "GetProviderService": {
             "access_level": "Undocumented",
-            "action": "GetIdMappingWorkflow",
+            "action": "GetProviderService",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSchemaMapping": {
+        "GetMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "UpdateSchemaMapping",
+            "action": "GetMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdMappingWorkflow": {
+        "ListIdMappingWorkflows": {
             "access_level": "Undocumented",
-            "action": "DeleteIdMappingWorkflow",
+            "action": "ListIdMappingWorkflows",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMatchingWorkflow": {
+        "AddPolicyStatement": {
             "access_level": "Undocumented",
-            "action": "UpdateMatchingWorkflow",
+            "action": "AddPolicyStatement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdMappingWorkflow": {
+        "DeleteIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "CreateIdMappingWorkflow",
+            "action": "DeleteIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UseIdNamespace": {
+        "GetMatchingJob": {
             "access_level": "Undocumented",
-            "action": "UseIdNamespace",
+            "action": "GetMatchingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMatchingJob": {
+        "PutPolicy": {
             "access_level": "Undocumented",
-            "action": "GetMatchingJob",
+            "action": "PutPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSchemaMappings": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListSchemaMappings",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProviderServices": {
+        "DeleteSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "ListProviderServices",
+            "action": "DeleteSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMatchingWorkflow": {
+        "StartIdMappingJob": {
             "access_level": "Undocumented",
-            "action": "DeleteMatchingWorkflow",
+            "action": "StartIdMappingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdNamespace": {
+        "StartMatchingJob": {
             "access_level": "Undocumented",
-            "action": "GetIdNamespace",
+            "action": "StartMatchingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "GetIdMappingJob": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "GetIdMappingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdNamespace": {
+        "ListMatchingJobs": {
             "access_level": "Undocumented",
-            "action": "UpdateIdNamespace",
+            "action": "ListMatchingJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdMappingJobs": {
+        "CreateIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListIdMappingJobs",
+            "action": "CreateIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdNamespaces": {
+        "GetIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListIdNamespaces",
+            "action": "GetIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMatchingJob": {
+        "CreateIdNamespace": {
             "access_level": "Undocumented",
-            "action": "StartMatchingJob",
+            "action": "CreateIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMatchingJobs": {
+        "ListMatchingWorkflows": {
             "access_level": "Undocumented",
-            "action": "ListMatchingJobs",
+            "action": "ListMatchingWorkflows",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdMappingJob": {
+        "ListProviderServices": {
             "access_level": "Undocumented",
-            "action": "GetIdMappingJob",
+            "action": "ListProviderServices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateMatchingWorkflow": {
             "access_level": "Undocumented",
             "action": "CreateMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdMappingWorkflow": {
+        "UpdateIdNamespace": {
             "access_level": "Undocumented",
-            "action": "UpdateIdMappingWorkflow",
+            "action": "UpdateIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchemaMapping": {
+        "DeleteIdNamespace": {
             "access_level": "Undocumented",
-            "action": "GetSchemaMapping",
+            "action": "DeleteIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdNamespace": {
+        "UpdateSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "CreateIdNamespace",
+            "action": "UpdateSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListSchemaMappings": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListSchemaMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListIdMappingJobs": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListIdMappingJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProviderService": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetProviderService",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdNamespace": {
+        "DeletePolicyStatement": {
             "access_level": "Undocumented",
-            "action": "DeleteIdNamespace",
+            "action": "DeletePolicyStatement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "es": {
@@ -70159,225 +70159,225 @@
             "orphan": false,
             "resources": [
                 "deliverystream"
             ]
         }
     },
     "fis": {
-        "ListExperimentResolvedTargets": {
+        "GetExperiment": {
             "access_level": "Undocumented",
-            "action": "ListExperimentResolvedTargets",
+            "action": "GetExperiment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTargetResourceTypes": {
+        "StartExperiment": {
             "access_level": "Undocumented",
-            "action": "ListTargetResourceTypes",
+            "action": "StartExperiment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExperimentTemplate": {
+        "ListActions": {
             "access_level": "Undocumented",
-            "action": "GetExperimentTemplate",
+            "action": "ListActions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateExperimentTemplate": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteExperimentTemplate": {
+        "GetExperimentTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteExperimentTemplate",
+            "action": "GetExperimentTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTargetAccountConfiguration": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateTargetAccountConfiguration",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAction": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetAction",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartExperiment": {
+        "DeleteTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartExperiment",
+            "action": "DeleteTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTargetAccountConfigurations": {
+        "ListExperimentTargetAccountConfigurations": {
             "access_level": "Undocumented",
-            "action": "ListTargetAccountConfigurations",
+            "action": "ListExperimentTargetAccountConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperiments": {
+        "ListTargetAccountConfigurations": {
             "access_level": "Undocumented",
-            "action": "ListExperiments",
+            "action": "ListTargetAccountConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateExperimentTemplate": {
+        "GetAction": {
             "access_level": "Undocumented",
-            "action": "CreateExperimentTemplate",
+            "action": "GetAction",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopExperiment": {
+        "ListExperimentResolvedTargets": {
             "access_level": "Undocumented",
-            "action": "StopExperiment",
+            "action": "ListExperimentResolvedTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExperimentTargetAccountConfiguration": {
+        "CreateTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetExperimentTargetAccountConfiguration",
+            "action": "CreateTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListActions": {
+        "GetTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListActions",
+            "action": "GetTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTargetAccountConfiguration": {
+        "InjectApiUnavailableError": {
             "access_level": "Undocumented",
-            "action": "CreateTargetAccountConfiguration",
+            "action": "InjectApiUnavailableError",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperimentTargetAccountConfigurations": {
+        "StopExperiment": {
             "access_level": "Undocumented",
-            "action": "ListExperimentTargetAccountConfigurations",
+            "action": "StopExperiment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InjectApiUnavailableError": {
+        "ListTargetResourceTypes": {
             "access_level": "Undocumented",
-            "action": "InjectApiUnavailableError",
+            "action": "ListTargetResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "InjectApiThrottleError": {
             "access_level": "Undocumented",
             "action": "InjectApiThrottleError",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperimentTemplates": {
+        "GetExperimentTemplate": {
             "access_level": "Undocumented",
-            "action": "ListExperimentTemplates",
+            "action": "GetExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateExperimentTemplate": {
+        "DeleteExperimentTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdateExperimentTemplate",
+            "action": "DeleteExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InjectApiInternalError": {
+        "ListExperiments": {
             "access_level": "Undocumented",
-            "action": "InjectApiInternalError",
+            "action": "ListExperiments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExperiment": {
+        "UpdateTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetExperiment",
+            "action": "UpdateTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTargetAccountConfiguration": {
+        "GetTargetResourceType": {
             "access_level": "Undocumented",
-            "action": "GetTargetAccountConfiguration",
+            "action": "GetTargetResourceType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTargetAccountConfiguration": {
+        "ListExperimentTemplates": {
             "access_level": "Undocumented",
-            "action": "DeleteTargetAccountConfiguration",
+            "action": "ListExperimentTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Undocumented",
             "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "InjectApiInternalError": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "InjectApiInternalError",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTargetResourceType": {
+        "UpdateExperimentTemplate": {
             "access_level": "Undocumented",
-            "action": "GetTargetResourceType",
+            "action": "UpdateExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "fms": {
@@ -80893,177 +80893,177 @@
             "condition_keys": [],
             "description": "Grants permission to enable the Organizational View feature",
             "orphan": false,
             "resources": []
         }
     },
     "healthlake": {
-        "CreateFHIRDatastore": {
+        "DeleteResource": {
             "access_level": "Undocumented",
-            "action": "CreateFHIRDatastore",
+            "action": "DeleteResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFHIRExportJobs": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListFHIRExportJobs",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFHIRImportJobs": {
+        "SearchEverything": {
             "access_level": "Undocumented",
-            "action": "ListFHIRImportJobs",
+            "action": "SearchEverything",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResource": {
+        "SearchWithPost": {
             "access_level": "Undocumented",
-            "action": "UpdateResource",
+            "action": "SearchWithPost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFHIRExportJob": {
+        "GetCapabilities": {
             "access_level": "Undocumented",
-            "action": "StartFHIRExportJob",
+            "action": "GetCapabilities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeFHIRImportJob": {
+        "ListFHIRDatastores": {
             "access_level": "Undocumented",
-            "action": "DescribeFHIRImportJob",
+            "action": "ListFHIRDatastores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResource": {
+        "DescribeFHIRDatastore": {
             "access_level": "Undocumented",
-            "action": "CreateResource",
+            "action": "DescribeFHIRDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchEverything": {
+        "DeleteFHIRDatastore": {
             "access_level": "Undocumented",
-            "action": "SearchEverything",
+            "action": "DeleteFHIRDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReadResource": {
+        "DescribeFHIRExportJob": {
             "access_level": "Undocumented",
-            "action": "ReadResource",
+            "action": "DescribeFHIRExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeFHIRExportJob": {
+        "StartFHIRExportJob": {
             "access_level": "Undocumented",
-            "action": "DescribeFHIRExportJob",
+            "action": "StartFHIRExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFHIRDatastore": {
+        "DescribeFHIRImportJob": {
             "access_level": "Undocumented",
-            "action": "DeleteFHIRDatastore",
+            "action": "DescribeFHIRImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFHIRDatastores": {
+        "UpdateResource": {
             "access_level": "Undocumented",
-            "action": "ListFHIRDatastores",
+            "action": "UpdateResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResource": {
+        "SearchWithGet": {
             "access_level": "Undocumented",
-            "action": "DeleteResource",
+            "action": "SearchWithGet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeFHIRDatastore": {
+        "ReadResource": {
             "access_level": "Undocumented",
-            "action": "DescribeFHIRDatastore",
+            "action": "ReadResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchWithPost": {
+        "CreateFHIRDatastore": {
             "access_level": "Undocumented",
-            "action": "SearchWithPost",
+            "action": "CreateFHIRDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCapabilities": {
+        "ListFHIRExportJobs": {
             "access_level": "Undocumented",
-            "action": "GetCapabilities",
+            "action": "ListFHIRExportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFHIRImportJob": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "StartFHIRImportJob",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListFHIRImportJobs": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListFHIRImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchWithGet": {
+        "StartFHIRImportJob": {
             "access_level": "Undocumented",
-            "action": "SearchWithGet",
+            "action": "StartFHIRImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "honeycode": {
@@ -81329,1377 +81329,1377 @@
             "condition_keys": [],
             "description": "Grants permission to update an Amazon Honeycode team for your AWS Account",
             "orphan": false,
             "resources": []
         }
     },
     "iam": {
-        "ListRolePolicies": {
+        "ListSTSRegionalEndpointsStatus": {
             "access_level": "Undocumented",
-            "action": "ListRolePolicies",
+            "action": "ListSTSRegionalEndpointsStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ChangePassword": {
+        "ListServiceSpecificCredentials": {
             "access_level": "Undocumented",
-            "action": "ChangePassword",
+            "action": "ListServiceSpecificCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadServerCertificate": {
+        "DeleteSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "UploadServerCertificate",
+            "action": "DeleteSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagMFADevice": {
+        "UploadSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "TagMFADevice",
+            "action": "UploadSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceLinkedRole": {
+        "GetGroup": {
             "access_level": "Undocumented",
-            "action": "CreateServiceLinkedRole",
+            "action": "GetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGroup": {
+        "CreateVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "UpdateGroup",
+            "action": "CreateVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulateCustomPolicy": {
+        "PassRole": {
             "access_level": "Undocumented",
-            "action": "SimulateCustomPolicy",
+            "action": "PassRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCloudFrontPublicKey": {
+        "GetLoginProfile": {
             "access_level": "Undocumented",
-            "action": "GetCloudFrontPublicKey",
+            "action": "GetLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountName": {
+        "ListOpenIDConnectProviderTags": {
             "access_level": "Undocumented",
-            "action": "GetAccountName",
+            "action": "ListOpenIDConnectProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServerCertificate": {
+        "DeleteGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateServerCertificate",
+            "action": "DeleteGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "ListInstanceProfilesForRole": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "ListInstanceProfilesForRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutGroupPolicy": {
+        "ListUserTags": {
             "access_level": "Undocumented",
-            "action": "PutGroupPolicy",
+            "action": "ListUserTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UntagServerCertificate": {
             "access_level": "Undocumented",
             "action": "UntagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMFADevice": {
+        "ResetServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "GetMFADevice",
+            "action": "ResetServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVirtualMFADevices": {
+        "SetSecurityTokenServicePreferences": {
             "access_level": "Undocumented",
-            "action": "ListVirtualMFADevices",
+            "action": "SetSecurityTokenServicePreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccessKey": {
+        "PutGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateAccessKey",
+            "action": "PutGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTags": {
+        "DeleteUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTags",
+            "action": "DeleteUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicies": {
+        "GetUserPolicy": {
             "access_level": "Undocumented",
-            "action": "ListPolicies",
+            "action": "GetUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachUserPolicy": {
+        "UpdateAccessKey": {
             "access_level": "Undocumented",
-            "action": "DetachUserPolicy",
+            "action": "UpdateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetails": {
+        "DeleteRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetails",
+            "action": "DeleteRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoleTags": {
+        "GetAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "ListRoleTags",
+            "action": "GetAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePermissionsBoundary": {
+        "ListPolicyVersions": {
             "access_level": "Undocumented",
-            "action": "PutRolePermissionsBoundary",
+            "action": "ListPolicyVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRolePolicy": {
+        "UntagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "GetRolePolicy",
+            "action": "UntagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSAMLProvider": {
+        "UploadServerCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateSAMLProvider",
+            "action": "UploadServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "DeleteSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "DeleteSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSigningCertificate": {
+        "DeleteServerCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateSigningCertificate",
+            "action": "DeleteServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "PutUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "PutUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSHPublicKey": {
+        "CreatePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "DeleteSSHPublicKey",
+            "action": "CreatePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyVersion": {
+        "ListRolePolicies": {
             "access_level": "Undocumented",
-            "action": "GetPolicyVersion",
+            "action": "ListRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstanceProfile": {
+        "GetMFADevice": {
             "access_level": "Undocumented",
-            "action": "CreateInstanceProfile",
+            "action": "GetMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagRole": {
+        "ListSigningCertificates": {
             "access_level": "Undocumented",
-            "action": "TagRole",
+            "action": "ListSigningCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountEmailAddress": {
+        "CreateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountEmailAddress",
+            "action": "CreateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviderTags": {
+        "ListGroupsForUser": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviderTags",
+            "action": "ListGroupsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRole": {
+        "ListSAMLProviderTags": {
             "access_level": "Undocumented",
-            "action": "CreateRole",
+            "action": "ListSAMLProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSAMLProvider": {
+        "CreateInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteSAMLProvider",
+            "action": "CreateInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachRolePolicy": {
+        "UpdateRoleDescription": {
             "access_level": "Undocumented",
-            "action": "DetachRolePolicy",
+            "action": "UpdateRoleDescription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupPolicy": {
+        "UpdateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "GetGroupPolicy",
+            "action": "UpdateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRole": {
+        "UntagMFADevice": {
             "access_level": "Undocumented",
-            "action": "PassRole",
+            "action": "UntagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetailsWithEntities": {
+        "CreateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetailsWithEntities",
+            "action": "CreateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviderTags": {
+        "ListUserPolicies": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviderTags",
+            "action": "ListUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetServiceSpecificCredential": {
+        "GetCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "ResetServiceSpecificCredential",
+            "action": "GetCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceSpecificCredential": {
+        "ListPolicies": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceSpecificCredential",
+            "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagSAMLProvider": {
+        "ListVirtualMFADevices": {
             "access_level": "Undocumented",
-            "action": "UntagSAMLProvider",
+            "action": "ListVirtualMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccountAlias": {
+        "ListPolicyTags": {
             "access_level": "Undocumented",
-            "action": "CreateAccountAlias",
+            "action": "ListPolicyTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfilesForRole": {
+        "UpdateAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfilesForRole",
+            "action": "UpdateAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPoliciesGrantingServiceAccess": {
+        "UpdateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "ListPoliciesGrantingServiceAccess",
+            "action": "UpdateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateVirtualMFADevice": {
+        "ListRoles": {
             "access_level": "Undocumented",
-            "action": "CreateVirtualMFADevice",
+            "action": "ListRoles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveRoleFromInstanceProfile": {
+        "GenerateServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "RemoveRoleFromInstanceProfile",
+            "action": "GenerateServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccessKeys": {
+        "UpdateAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "ListAccessKeys",
+            "action": "UpdateAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagOpenIDConnectProvider": {
+        "ListMFADevices": {
             "access_level": "Undocumented",
-            "action": "TagOpenIDConnectProvider",
+            "action": "ListMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulatePrincipalPolicy": {
+        "DeleteInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "SimulatePrincipalPolicy",
+            "action": "DeleteInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPermissionsBoundary": {
+        "GetPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPermissionsBoundary",
+            "action": "GetPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountPasswordPolicy": {
+        "GenerateOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountPasswordPolicy",
+            "action": "GenerateOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRole": {
+        "UntagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteRole",
+            "action": "UntagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachGroupPolicy": {
+        "TagUser": {
             "access_level": "Undocumented",
-            "action": "AttachGroupPolicy",
+            "action": "TagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForCustomPolicy": {
+        "ListGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForCustomPolicy",
+            "action": "ListGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEntitiesForPolicy": {
+        "CreateOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListEntitiesForPolicy",
+            "action": "CreateOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUser": {
+        "GetAccessKeyLastUsed": {
             "access_level": "Undocumented",
-            "action": "UpdateUser",
+            "action": "GetAccessKeyLastUsed",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfileTags": {
+        "GetContextKeysForPrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfileTags",
+            "action": "GetContextKeysForPrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupPolicies": {
+        "DeleteAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "ListGroupPolicies",
+            "action": "DeleteAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagPolicy": {
+        "DetachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "TagPolicy",
+            "action": "DetachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstanceProfile": {
+        "GetOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "DeleteInstanceProfile",
+            "action": "GetOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroups": {
+        "ResyncMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListGroups",
+            "action": "ResyncMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLoginProfile": {
+        "GetServiceLastAccessedDetailsWithEntities": {
             "access_level": "Undocumented",
-            "action": "UpdateLoginProfile",
+            "action": "GetServiceLastAccessedDetailsWithEntities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRole": {
+        "DetachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GetRole",
+            "action": "DetachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyVersion": {
+        "UntagUser": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyVersion",
+            "action": "UntagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountEmailAddress": {
+        "DeleteSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "GetAccountEmailAddress",
+            "action": "DeleteSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagOpenIDConnectProvider": {
+        "DeleteVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "UntagOpenIDConnectProvider",
+            "action": "DeleteVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountAlias": {
+        "GetAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountAlias",
+            "action": "GetAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADevices": {
+        "DeleteAccountAlias": {
             "access_level": "Undocumented",
-            "action": "ListMFADevices",
+            "action": "DeleteAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificateTags": {
+        "CreateAccessKey": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificateTags",
+            "action": "CreateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSigningCertificate": {
+        "ListOpenIDConnectProviders": {
             "access_level": "Undocumented",
-            "action": "DeleteSigningCertificate",
+            "action": "ListOpenIDConnectProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLoginProfile": {
+        "ListEntitiesForPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateLoginProfile",
+            "action": "ListEntitiesForPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserTags": {
+        "UpdateRole": {
             "access_level": "Undocumented",
-            "action": "ListUserTags",
+            "action": "UpdateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCredentialReport": {
+        "GetUser": {
             "access_level": "Undocumented",
-            "action": "GenerateCredentialReport",
+            "action": "GetUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServerCertificate": {
+        "ListServerCertificateTags": {
             "access_level": "Undocumented",
-            "action": "DeleteServerCertificate",
+            "action": "ListServerCertificateTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagMFADevice": {
+        "DeactivateMFADevice": {
             "access_level": "Undocumented",
-            "action": "UntagMFADevice",
+            "action": "DeactivateMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountName": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountName",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePolicy": {
+        "ListMFADeviceTags": {
             "access_level": "Undocumented",
-            "action": "PutRolePolicy",
+            "action": "ListMFADeviceTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedUserPolicies": {
+        "GetServiceLinkedRoleDeletionStatus": {
             "access_level": "Undocumented",
-            "action": "ListAttachedUserPolicies",
+            "action": "GetServiceLinkedRoleDeletionStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfiles": {
+        "GetRolePolicy": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfiles",
+            "action": "GetRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountSummary": {
+        "ListSSHPublicKeys": {
             "access_level": "Undocumented",
-            "action": "GetAccountSummary",
+            "action": "ListSSHPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteUserPolicy": {
             "access_level": "Undocumented",
             "action": "DeleteUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroup": {
+        "UpdateAccountName": {
             "access_level": "Undocumented",
-            "action": "GetGroup",
+            "action": "UpdateAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagUser": {
+        "CreateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "TagUser",
+            "action": "CreateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateOrganizationsAccessReport": {
+        "TagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "GenerateOrganizationsAccessReport",
+            "action": "TagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagInstanceProfile": {
+        "CreateGroup": {
             "access_level": "Undocumented",
-            "action": "TagInstanceProfile",
+            "action": "CreateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPolicy": {
+        "ListAccountAliases": {
             "access_level": "Undocumented",
-            "action": "PutUserPolicy",
+            "action": "ListAccountAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveClientIDFromOpenIDConnectProvider": {
+        "PutRolePolicy": {
             "access_level": "Undocumented",
-            "action": "RemoveClientIDFromOpenIDConnectProvider",
+            "action": "PutRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUser": {
+        "ListInstanceProfiles": {
             "access_level": "Undocumented",
-            "action": "GetUser",
+            "action": "ListInstanceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedRolePolicies": {
+        "ChangePassword": {
             "access_level": "Undocumented",
-            "action": "ListAttachedRolePolicies",
+            "action": "ChangePassword",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableMFADevice": {
+        "UpdateAssumeRolePolicy": {
             "access_level": "Undocumented",
-            "action": "EnableMFADevice",
+            "action": "UpdateAssumeRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddClientIDToOpenIDConnectProvider": {
+        "DeleteGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "AddClientIDToOpenIDConnectProvider",
+            "action": "DeleteGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountAliases": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "ListAccountAliases",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddRoleToInstanceProfile": {
+        "ListUsers": {
             "access_level": "Undocumented",
-            "action": "AddRoleToInstanceProfile",
+            "action": "ListUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoles": {
+        "GetContextKeysForCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "ListRoles",
+            "action": "GetContextKeysForCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLoginProfile": {
+        "UntagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteLoginProfile",
+            "action": "UntagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachGroupPolicy": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "DetachGroupPolicy",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyVersions": {
+        "DeleteRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "ListPolicyVersions",
+            "action": "DeleteRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUsers": {
+        "GetCredentialReport": {
             "access_level": "Undocumented",
-            "action": "ListUsers",
+            "action": "GetCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagServerCertificate": {
+        "ListRoleTags": {
             "access_level": "Undocumented",
-            "action": "TagServerCertificate",
+            "action": "ListRoleTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLinkedRoleDeletionStatus": {
+        "GetOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "GetServiceLinkedRoleDeletionStatus",
+            "action": "GetOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserPolicy": {
+        "GenerateCredentialReport": {
             "access_level": "Undocumented",
-            "action": "GetUserPolicy",
+            "action": "GenerateCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCloudFrontPublicKeys": {
+        "GetServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ListCloudFrontPublicKeys",
+            "action": "GetServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagSAMLProvider": {
+        "SetSTSRegionalEndpointStatus": {
             "access_level": "Undocumented",
-            "action": "TagSAMLProvider",
+            "action": "SetSTSRegionalEndpointStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLoginProfile": {
+        "UpdateUser": {
             "access_level": "Undocumented",
-            "action": "GetLoginProfile",
+            "action": "UpdateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForPrincipalPolicy": {
+        "AddUserToGroup": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForPrincipalPolicy",
+            "action": "AddUserToGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificates": {
+        "RemoveClientIDFromOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificates",
+            "action": "RemoveClientIDFromOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccessKey": {
+        "SimulateCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteAccessKey",
+            "action": "SimulateCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResyncMFADevice": {
+        "SimulatePrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "ResyncMFADevice",
+            "action": "SimulatePrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOpenIDConnectProvider": {
+        "DeleteServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "CreateOpenIDConnectProvider",
+            "action": "DeleteServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceSpecificCredential": {
+        "CreateAccountAlias": {
             "access_level": "Undocumented",
-            "action": "CreateServiceSpecificCredential",
+            "action": "CreateAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountAuthorizationDetails": {
+        "AttachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "GetAccountAuthorizationDetails",
+            "action": "AttachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupsForUser": {
+        "GetRole": {
             "access_level": "Undocumented",
-            "action": "ListGroupsForUser",
+            "action": "GetRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSSHPublicKey": {
+        "UntagPolicy": {
             "access_level": "Undocumented",
-            "action": "GetSSHPublicKey",
+            "action": "UntagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServerCertificate": {
+        "GetGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "GetServerCertificate",
+            "action": "GetGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccessKeyLastUsed": {
+        "DeletePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "GetAccessKeyLastUsed",
+            "action": "DeletePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviders": {
+        "GetSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviders",
+            "action": "GetSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateServiceLastAccessedDetails": {
+        "EnableMFADevice": {
             "access_level": "Undocumented",
-            "action": "GenerateServiceLastAccessedDetails",
+            "action": "EnableMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRole": {
+        "ListGroups": {
             "access_level": "Undocumented",
-            "action": "UpdateRole",
+            "action": "ListGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCloudFrontPublicKey": {
+        "AddRoleToInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateCloudFrontPublicKey",
+            "action": "AddRoleToInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagPolicy": {
+        "AttachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "UntagPolicy",
+            "action": "AttachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserPolicies": {
+        "UntagRole": {
             "access_level": "Undocumented",
-            "action": "ListUserPolicies",
+            "action": "UntagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOpenIDConnectProvider": {
+        "GetAccountAuthorizationDetails": {
             "access_level": "Undocumented",
-            "action": "GetOpenIDConnectProvider",
+            "action": "GetAccountAuthorizationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSSHPublicKeys": {
+        "TagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "ListSSHPublicKeys",
+            "action": "TagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCloudFrontPublicKey": {
+        "TagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteCloudFrontPublicKey",
+            "action": "TagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSSHPublicKey": {
+        "TagMFADevice": {
             "access_level": "Undocumented",
-            "action": "UpdateSSHPublicKey",
+            "action": "TagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyVersion": {
+        "TagPolicy": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyVersion",
+            "action": "TagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInstanceProfile": {
+        "UploadSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "GetInstanceProfile",
+            "action": "UploadSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountPasswordPolicy": {
+        "ListAccessKeys": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountPasswordPolicy",
+            "action": "ListAccessKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroupPolicy": {
+        "PutUserPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteGroupPolicy",
+            "action": "PutUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "SetDefaultPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "SetDefaultPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachRolePolicy": {
+        "UpdateServerCertificate": {
             "access_level": "Undocumented",
-            "action": "AttachRolePolicy",
+            "action": "UpdateServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePolicy": {
+        "TagRole": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePolicy",
+            "action": "TagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRoleDescription": {
+        "CreateRole": {
             "access_level": "Undocumented",
-            "action": "UpdateRoleDescription",
+            "action": "CreateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServiceSpecificCredential": {
+        "ListAttachedGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "UpdateServiceSpecificCredential",
+            "action": "ListAttachedGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeactivateMFADevice": {
+        "GetServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "DeactivateMFADevice",
+            "action": "GetServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagUser": {
+        "CreateServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "UntagUser",
+            "action": "CreateServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadCloudFrontPublicKey": {
+        "ListCloudFrontPublicKeys": {
             "access_level": "Undocumented",
-            "action": "UploadCloudFrontPublicKey",
+            "action": "ListCloudFrontPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedGroupPolicies": {
+        "UploadCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListAttachedGroupPolicies",
+            "action": "UploadCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPolicyVersion": {
+        "GetAccountSummary": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPolicyVersion",
+            "action": "GetAccountSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSigningCertificate": {
+        "PutRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "UploadSigningCertificate",
+            "action": "PutRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveUserFromGroup": {
+        "DeleteOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "RemoveUserFromGroup",
+            "action": "DeleteOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteVirtualMFADevice": {
+        "AttachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteVirtualMFADevice",
+            "action": "AttachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCredentialReport": {
+        "CreateUser": {
             "access_level": "Undocumented",
-            "action": "GetCredentialReport",
+            "action": "CreateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceSpecificCredentials": {
+        "ListAttachedRolePolicies": {
             "access_level": "Undocumented",
-            "action": "ListServiceSpecificCredentials",
+            "action": "ListAttachedRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccessKey": {
+        "DetachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateAccessKey",
+            "action": "DetachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSigningCertificates": {
+        "TagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListSigningCertificates",
+            "action": "TagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSAMLProvider": {
+        "DeleteRole": {
             "access_level": "Undocumented",
-            "action": "CreateSAMLProvider",
+            "action": "DeleteRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddUserToGroup": {
+        "ListSAMLProviders": {
             "access_level": "Undocumented",
-            "action": "AddUserToGroup",
+            "action": "ListSAMLProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSTSRegionalEndpointsStatus": {
+        "UpdateSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "ListSTSRegionalEndpointsStatus",
+            "action": "UpdateSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityTokenServicePreferences": {
+        "UpdateSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "SetSecurityTokenServicePreferences",
+            "action": "UpdateSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGroup": {
+        "GetAccountName": {
             "access_level": "Undocumented",
-            "action": "CreateGroup",
+            "action": "GetAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOpenIDConnectProvider": {
+        "ListInstanceProfileTags": {
             "access_level": "Undocumented",
-            "action": "DeleteOpenIDConnectProvider",
+            "action": "ListInstanceProfileTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSAMLProvider": {
+        "ListPoliciesGrantingServiceAccess": {
             "access_level": "Undocumented",
-            "action": "GetSAMLProvider",
+            "action": "ListPoliciesGrantingServiceAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePermissionsBoundary": {
+        "UpdateGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePermissionsBoundary",
+            "action": "UpdateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountPasswordPolicy": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "GetAccountPasswordPolicy",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachUserPolicy": {
+        "DeleteCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "AttachUserPolicy",
+            "action": "DeleteCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviders": {
+        "GetInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviders",
+            "action": "GetInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagRole": {
+        "DeleteServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "UntagRole",
+            "action": "DeleteServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPermissionsBoundary": {
+        "DeleteLoginProfile": {
             "access_level": "Undocumented",
-            "action": "PutUserPermissionsBoundary",
+            "action": "DeleteLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOpenIDConnectProviderThumbprint": {
+        "ListServerCertificates": {
             "access_level": "Undocumented",
-            "action": "UpdateOpenIDConnectProviderThumbprint",
+            "action": "ListServerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADeviceTags": {
+        "DeleteAccessKey": {
             "access_level": "Undocumented",
-            "action": "ListMFADeviceTags",
+            "action": "DeleteAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOrganizationsAccessReport": {
+        "GetSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "GetOrganizationsAccessReport",
+            "action": "GetSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUser": {
+        "RemoveRoleFromInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "CreateUser",
+            "action": "RemoveRoleFromInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagInstanceProfile": {
+        "UpdateOpenIDConnectProviderThumbprint": {
             "access_level": "Undocumented",
-            "action": "UntagInstanceProfile",
+            "action": "UpdateOpenIDConnectProviderThumbprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSSHPublicKey": {
+        "AddClientIDToOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "UploadSSHPublicKey",
+            "action": "AddClientIDToOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroup": {
+        "UpdateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "DeleteGroup",
+            "action": "UpdateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSTSRegionalEndpointStatus": {
+        "ListAttachedUserPolicies": {
             "access_level": "Undocumented",
-            "action": "SetSTSRegionalEndpointStatus",
+            "action": "ListAttachedUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAssumeRolePolicy": {
+        "UpdateCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "UpdateAssumeRolePolicy",
+            "action": "UpdateCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceLinkedRole": {
+        "RemoveUserFromGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceLinkedRole",
+            "action": "RemoveUserFromGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "identity-sync": {
@@ -84940,41 +84940,41 @@
             "orphan": false,
             "resources": [
                 "Monitor"
             ]
         }
     },
     "invoicing": {
-        "ListInvoiceSummaries": {
+        "PutInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "ListInvoiceSummaries",
+            "action": "PutInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInvoiceEmailDeliveryPreferences": {
+        "GetInvoicePDF": {
             "access_level": "Undocumented",
-            "action": "GetInvoiceEmailDeliveryPreferences",
+            "action": "GetInvoicePDF",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutInvoiceEmailDeliveryPreferences": {
+        "ListInvoiceSummaries": {
             "access_level": "Undocumented",
-            "action": "PutInvoiceEmailDeliveryPreferences",
+            "action": "ListInvoiceSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInvoicePDF": {
+        "GetInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "GetInvoicePDF",
+            "action": "GetInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iot": {
@@ -91139,913 +91139,913 @@
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         }
     },
     "iotwireless": {
-        "SendDataToMulticastGroup": {
+        "StartMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "SendDataToMulticastGroup",
+            "action": "StartMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromThing": {
+        "ListEventConfigurations": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromThing",
+            "action": "ListEventConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGateway": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGateway",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTaskDefinition": {
+        "ListQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTaskDefinition",
+            "action": "ListQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMulticastGroup": {
+        "GetFuotaTask": {
             "access_level": "Undocumented",
-            "action": "CreateMulticastGroup",
+            "action": "GetFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithThing": {
+        "DeleteWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithThing",
+            "action": "DeleteWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFuotaTasks": {
+        "AssociateWirelessDeviceWithThing": {
             "access_level": "Undocumented",
-            "action": "ListFuotaTasks",
+            "action": "AssociateWirelessDeviceWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceProfiles": {
+        "GetResourcePosition": {
             "access_level": "Undocumented",
-            "action": "ListDeviceProfiles",
+            "action": "GetResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDestination": {
+        "TestWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "DeleteDestination",
+            "action": "TestWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGatewayTaskDefinitions": {
+        "UpdateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGatewayTaskDefinitions",
+            "action": "UpdateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromMulticastGroup": {
+        "StartNetworkAnalyzerStream": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromMulticastGroup",
+            "action": "StartNetworkAnalyzerStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroup": {
+        "DisassociateAwsAccountFromPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroup",
+            "action": "DisassociateAwsAccountFromPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPartnerAccounts": {
+        "StartSingleWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "ListPartnerAccounts",
+            "action": "StartSingleWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTaskDefinition": {
+        "GetLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTaskDefinition",
+            "action": "GetLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartSingleWirelessDeviceImportTask": {
+        "GetWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "StartSingleWirelessDeviceImportTask",
+            "action": "GetWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDestination": {
+        "CancelMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "GetDestination",
+            "action": "CancelMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DisassociateWirelessDeviceFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DisassociateWirelessDeviceFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPositionConfigurations": {
+        "UpdatePosition": {
             "access_level": "Undocumented",
-            "action": "ListPositionConfigurations",
+            "action": "UpdatePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNetworkAnalyzerConfiguration": {
+        "GetMetrics": {
             "access_level": "Undocumented",
-            "action": "DeleteNetworkAnalyzerConfiguration",
+            "action": "GetMetrics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithCertificate": {
+        "AssociateMulticastGroupWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithCertificate",
+            "action": "AssociateMulticastGroupWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroupSession": {
+        "AssociateWirelessDeviceWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroupSession",
+            "action": "AssociateWirelessDeviceWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNetworkAnalyzerConfiguration": {
+        "DisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetNetworkAnalyzerConfiguration",
+            "action": "DisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMulticastGroupSession": {
+        "GetEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "CancelMulticastGroupSession",
+            "action": "GetEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromThing": {
+        "PutPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromThing",
+            "action": "PutPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGateway": {
+        "UpdateMetricConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGateway",
+            "action": "UpdateMetricConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDevices": {
+        "UpdateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDevices",
+            "action": "UpdateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMetricConfiguration": {
+        "UpdateResourcePosition": {
             "access_level": "Undocumented",
-            "action": "UpdateMetricConfiguration",
+            "action": "UpdateResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMulticastGroup": {
+        "ResetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "UpdateMulticastGroup",
+            "action": "ResetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartWirelessDeviceImportTask": {
+        "UpdateDestination": {
             "access_level": "Undocumented",
-            "action": "StartWirelessDeviceImportTask",
+            "action": "UpdateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceProfiles": {
+        "DeleteNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListServiceProfiles",
+            "action": "DeleteNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithMulticastGroup": {
+        "DeleteWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithMulticastGroup",
+            "action": "DeleteWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceEventConfiguration": {
+        "SendDataToWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetResourceEventConfiguration",
+            "action": "SendDataToWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDestination": {
+        "ListDestinations": {
             "access_level": "Undocumented",
-            "action": "UpdateDestination",
+            "action": "ListDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessDevice": {
+        "UpdatePartnerAccount": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessDevice",
+            "action": "UpdatePartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToWirelessDevice": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "SendDataToWirelessDevice",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFuotaTask": {
+        "GetDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteFuotaTask",
+            "action": "GetDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceImportTask": {
+        "CreateWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceImportTask",
+            "action": "CreateWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessGateway": {
+        "DisassociateWirelessDeviceFromThing": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessGateway",
+            "action": "DisassociateWirelessDeviceFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceProfile": {
+        "UpdateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceProfile",
+            "action": "UpdateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDevice": {
+        "CreateWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDevice",
+            "action": "CreateWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTaskDefinition": {
+        "AssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTaskDefinition",
+            "action": "AssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroups": {
+        "DisassociateWirelessGatewayFromCertificate": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroups",
+            "action": "DisassociateWirelessGatewayFromCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMulticastGroupSession": {
+        "DeregisterWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "StartMulticastGroupSession",
+            "action": "DeregisterWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceEndpoint": {
+        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetServiceEndpoint",
+            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDevice": {
+        "ListServiceProfiles": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDevice",
+            "action": "ListServiceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceEventConfiguration": {
+        "GetWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceEventConfiguration",
+            "action": "GetWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDevice": {
+        "UpdateLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDevice",
+            "action": "UpdateLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePosition": {
+        "UpdateEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "UpdatePosition",
+            "action": "UpdateEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFuotaTask": {
+        "UpdateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetFuotaTask",
+            "action": "UpdateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventConfigurations": {
+        "DeleteWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "ListEventConfigurations",
+            "action": "DeleteWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFuotaTask": {
+        "ListDeviceProfiles": {
             "access_level": "Undocumented",
-            "action": "CreateFuotaTask",
+            "action": "ListDeviceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGateways": {
+        "DisassociateWirelessGatewayFromThing": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGateways",
+            "action": "DisassociateWirelessGatewayFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLogLevelsByResourceTypes": {
+        "ListMulticastGroupsByFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetLogLevelsByResourceTypes",
+            "action": "ListMulticastGroupsByFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTask": {
+        "CreateDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTask",
+            "action": "CreateDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromCertificate": {
+        "DeleteDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromCertificate",
+            "action": "DeleteDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceProfile": {
+        "GetWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "CreateServiceProfile",
+            "action": "GetWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetAllResourceLogLevels": {
+        "AssociateWirelessGatewayWithThing": {
             "access_level": "Undocumented",
-            "action": "ResetAllResourceLogLevels",
+            "action": "AssociateWirelessGatewayWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetResourceLogLevel": {
+        "GetDestination": {
             "access_level": "Undocumented",
-            "action": "ResetResourceLogLevel",
+            "action": "GetDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayFirmwareInformation": {
+        "GetPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayFirmwareInformation",
+            "action": "GetPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePosition": {
+        "ListNetworkAnalyzerConfigurations": {
             "access_level": "Undocumented",
-            "action": "GetResourcePosition",
+            "action": "ListNetworkAnalyzerConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithThing": {
+        "StartFuotaTask": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithThing",
+            "action": "StartFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPosition": {
+        "AssociateWirelessGatewayWithCertificate": {
             "access_level": "Undocumented",
-            "action": "GetPosition",
+            "action": "AssociateWirelessGatewayWithCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetWirelessGatewayCertificate": {
             "access_level": "Undocumented",
             "action": "GetWirelessGatewayCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLogLevelsByResourceTypes": {
+        "ListFuotaTasks": {
             "access_level": "Undocumented",
-            "action": "UpdateLogLevelsByResourceTypes",
+            "action": "ListFuotaTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayStatistics": {
+        "ListDevicesForWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayStatistics",
+            "action": "ListDevicesForWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionEstimate": {
+        "GetPosition": {
             "access_level": "Undocumented",
-            "action": "GetPositionEstimate",
+            "action": "GetPosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDeviceImportTasks": {
+        "SendDataToMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDeviceImportTasks",
+            "action": "SendDataToMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMulticastGroupFromFuotaTask": {
+        "GetResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "DisassociateMulticastGroupFromFuotaTask",
+            "action": "GetResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMulticastGroupWithFuotaTask": {
+        "GetMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "AssociateMulticastGroupWithFuotaTask",
+            "action": "GetMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDestination": {
+        "CreateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "CreateDestination",
+            "action": "CreateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestWirelessDevice": {
+        "DeleteMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "TestWirelessDevice",
+            "action": "DeleteMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventConfigurationByResourceTypes": {
+        "ListWirelessDevices": {
             "access_level": "Undocumented",
-            "action": "UpdateEventConfigurationByResourceTypes",
+            "action": "ListWirelessDevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromFuotaTask": {
+        "GetWirelessGatewayFirmwareInformation": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromFuotaTask",
+            "action": "GetWirelessGatewayFirmwareInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNetworkAnalyzerConfiguration": {
+        "GetPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateNetworkAnalyzerConfiguration",
+            "action": "GetPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGateway": {
+        "CreateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGateway",
+            "action": "CreateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFuotaTask": {
+        "PutResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "StartFuotaTask",
+            "action": "PutResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPartnerAccount": {
+        "StartWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetPartnerAccount",
+            "action": "StartWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceLogLevel": {
+        "DeleteServiceProfile": {
             "access_level": "Undocumented",
-            "action": "GetResourceLogLevel",
+            "action": "DeleteServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePartnerAccount": {
+        "UpdateResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdatePartnerAccount",
+            "action": "UpdateResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNetworkAnalyzerConfigurations": {
+        "GetWirelessDeviceStatistics": {
             "access_level": "Undocumented",
-            "action": "ListNetworkAnalyzerConfigurations",
+            "action": "GetWirelessDeviceStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDestinations": {
+        "DeleteFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ListDestinations",
+            "action": "DeleteFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDevicesForWirelessDeviceImportTask": {
+        "DisassociateMulticastGroupFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ListDevicesForWirelessDeviceImportTask",
+            "action": "DisassociateMulticastGroupFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTask": {
+        "DeleteWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTask",
+            "action": "DeleteWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTask": {
+        "GetServiceEndpoint": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTask",
+            "action": "GetServiceEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMulticastGroup": {
+        "GetMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "DeleteMulticastGroup",
+            "action": "GetMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetrics": {
+        "GetWirelessGatewayStatistics": {
             "access_level": "Undocumented",
-            "action": "GetMetrics",
+            "action": "GetWirelessGatewayStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutPositionConfiguration": {
+        "GetNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "PutPositionConfiguration",
+            "action": "GetNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithFuotaTask": {
+        "ListPartnerAccounts": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithFuotaTask",
+            "action": "ListPartnerAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceProfile": {
+        "ListWirelessGatewayTaskDefinitions": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceProfile",
+            "action": "ListWirelessGatewayTaskDefinitions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetricConfiguration": {
+        "UpdateWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetMetricConfiguration",
+            "action": "UpdateWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceProfile": {
+        "AssociateAwsAccountWithPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceProfile",
+            "action": "AssociateAwsAccountWithPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueuedMessages": {
+        "ResetAllResourceLogLevels": {
             "access_level": "Undocumented",
-            "action": "DeleteQueuedMessages",
+            "action": "ResetAllResourceLogLevels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroupsByFuotaTask": {
+        "ListPositionConfigurations": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroupsByFuotaTask",
+            "action": "ListPositionConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDeviceImportTask": {
+        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDeviceImportTask",
+            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartNetworkAnalyzerStream": {
+        "DeleteQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "StartNetworkAnalyzerStream",
+            "action": "DeleteQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionConfiguration": {
+        "CreateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "GetPositionConfiguration",
+            "action": "CreateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceProfile": {
+        "GetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "GetDeviceProfile",
+            "action": "GetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
+        "GetMetricConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
+            "action": "GetMetricConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterWirelessDevice": {
+        "GetServiceProfile": {
             "access_level": "Undocumented",
-            "action": "DeregisterWirelessDevice",
+            "action": "GetServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceStatistics": {
+        "CreateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceStatistics",
+            "action": "CreateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
+        "DeleteDestination": {
             "access_level": "Undocumented",
-            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
+            "action": "DeleteDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateAwsAccountFromPartnerAccount": {
+        "ListMulticastGroups": {
             "access_level": "Undocumented",
-            "action": "DisassociateAwsAccountFromPartnerAccount",
+            "action": "ListMulticastGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutResourceLogLevel": {
+        "CreateDestination": {
             "access_level": "Undocumented",
-            "action": "PutResourceLogLevel",
+            "action": "CreateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDeviceImportTask": {
+        "GetPositionEstimate": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDeviceImportTask",
+            "action": "GetPositionEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceProfile": {
+        "ListWirelessGateways": {
             "access_level": "Undocumented",
-            "action": "GetServiceProfile",
+            "action": "ListWirelessGateways",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFuotaTask": {
+        "CreateServiceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateFuotaTask",
+            "action": "CreateServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNetworkAnalyzerConfiguration": {
+        "ListWirelessDeviceImportTasks": {
             "access_level": "Undocumented",
-            "action": "UpdateNetworkAnalyzerConfiguration",
+            "action": "ListWirelessDeviceImportTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueuedMessages": {
+        "GetWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "ListQueuedMessages",
+            "action": "GetWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourcePosition": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateResourcePosition",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventConfigurationByResourceTypes": {
+        "UpdateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetEventConfigurationByResourceTypes",
+            "action": "UpdateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateAwsAccountWithPartnerAccount": {
+        "DeleteWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "AssociateAwsAccountWithPartnerAccount",
+            "action": "DeleteWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iq": {
@@ -95212,22 +95212,14 @@
             "resources": [
                 "index",
                 "thesaurus"
             ]
         }
     },
     "kendra-ranking": {
-        "UpdateRescoreExecutionPlan": {
-            "access_level": "Undocumented",
-            "action": "UpdateRescoreExecutionPlan",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
         "DeleteRescoreExecutionPlan": {
             "access_level": "Undocumented",
             "action": "DeleteRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -95236,315 +95228,323 @@
             "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRescoreExecutionPlan": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateRescoreExecutionPlan",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeRescoreExecutionPlan": {
+        "Rescore": {
             "access_level": "Undocumented",
-            "action": "DescribeRescoreExecutionPlan",
+            "action": "Rescore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListRescoreExecutionPlans": {
             "access_level": "Undocumented",
             "action": "ListRescoreExecutionPlans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "DescribeRescoreExecutionPlan": {
+            "access_level": "Undocumented",
+            "action": "DescribeRescoreExecutionPlan",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "TagResource": {
             "access_level": "Undocumented",
             "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Rescore": {
+        "UpdateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "Rescore",
+            "action": "UpdateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesis": {
-        "DescribeLimits": {
+        "DescribeStream": {
             "access_level": "Undocumented",
-            "action": "DescribeLimits",
+            "action": "DescribeStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecords": {
+        "EnableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "PutRecords",
+            "action": "EnableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutResourcePolicy": {
+        "StartStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "PutResourcePolicy",
+            "action": "StartStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopStreamEncryption": {
+        "ListShards": {
             "access_level": "Undocumented",
-            "action": "StopStreamEncryption",
+            "action": "ListShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterStreamConsumer": {
+        "PutResourcePolicy": {
             "access_level": "Undocumented",
-            "action": "RegisterStreamConsumer",
+            "action": "PutResourcePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteStream": {
+        "GetResourcePolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteStream",
+            "action": "GetResourcePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamConsumer": {
+        "DisableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamConsumer",
+            "action": "DisableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForStream": {
+        "SplitShard": {
             "access_level": "Undocumented",
-            "action": "ListTagsForStream",
+            "action": "SplitShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MergeShards": {
+        "DescribeLimits": {
             "access_level": "Undocumented",
-            "action": "MergeShards",
+            "action": "DescribeLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IncreaseStreamRetentionPeriod": {
+        "AddTagsToStream": {
             "access_level": "Undocumented",
-            "action": "IncreaseStreamRetentionPeriod",
+            "action": "AddTagsToStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableEnhancedMonitoring": {
+        "UpdateStreamMode": {
             "access_level": "Undocumented",
-            "action": "EnableEnhancedMonitoring",
+            "action": "UpdateStreamMode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartStreamEncryption": {
+        "RemoveTagsFromStream": {
             "access_level": "Undocumented",
-            "action": "StartStreamEncryption",
+            "action": "RemoveTagsFromStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddTagsToStream": {
+        "MergeShards": {
             "access_level": "Undocumented",
-            "action": "AddTagsToStream",
+            "action": "MergeShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecord": {
+        "DeleteStream": {
             "access_level": "Undocumented",
-            "action": "PutRecord",
+            "action": "DeleteStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateShardCount": {
+        "PutRecord": {
             "access_level": "Undocumented",
-            "action": "UpdateShardCount",
+            "action": "PutRecord",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisableEnhancedMonitoring": {
+        "DescribeStreamSummary": {
             "access_level": "Undocumented",
-            "action": "DisableEnhancedMonitoring",
+            "action": "DescribeStreamSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveTagsFromStream": {
+        "GetShardIterator": {
             "access_level": "Undocumented",
-            "action": "RemoveTagsFromStream",
+            "action": "GetShardIterator",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStreamMode": {
+        "ListTagsForStream": {
             "access_level": "Undocumented",
-            "action": "UpdateStreamMode",
+            "action": "ListTagsForStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateStream": {
             "access_level": "Undocumented",
             "action": "CreateStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SubscribeToShard": {
+        "PutRecords": {
             "access_level": "Undocumented",
-            "action": "SubscribeToShard",
+            "action": "PutRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterStreamConsumer": {
+        "SubscribeToShard": {
             "access_level": "Undocumented",
-            "action": "DeregisterStreamConsumer",
+            "action": "SubscribeToShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecreaseStreamRetentionPeriod": {
+        "DeleteResourcePolicy": {
             "access_level": "Undocumented",
-            "action": "DecreaseStreamRetentionPeriod",
+            "action": "DeleteResourcePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecords": {
+        "UpdateShardCount": {
             "access_level": "Undocumented",
-            "action": "GetRecords",
+            "action": "UpdateShardCount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreams": {
+        "GetRecords": {
             "access_level": "Undocumented",
-            "action": "ListStreams",
+            "action": "GetRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamSummary": {
+        "DecreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamSummary",
+            "action": "DecreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreamConsumers": {
+        "IncreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "ListStreamConsumers",
+            "action": "IncreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SplitShard": {
+        "DescribeStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "SplitShard",
+            "action": "DescribeStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResourcePolicy": {
+        "ListStreams": {
             "access_level": "Undocumented",
-            "action": "DeleteResourcePolicy",
+            "action": "ListStreams",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStream": {
+        "RegisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "DescribeStream",
+            "action": "RegisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListShards": {
+        "StopStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "ListShards",
+            "action": "StopStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePolicy": {
+        "ListStreamConsumers": {
             "access_level": "Undocumented",
-            "action": "GetResourcePolicy",
+            "action": "ListStreamConsumers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetShardIterator": {
+        "DeregisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "GetShardIterator",
+            "action": "DeregisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesisanalytics": {
@@ -98214,273 +98214,273 @@
             "orphan": false,
             "resources": [
                 "function"
             ]
         }
     },
     "launchwizard": {
-        "CreateSettingsSet": {
-            "access_level": "Undocumented",
-            "action": "CreateSettingsSet",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
         "GetInfrastructureSuggestion": {
             "access_level": "Undocumented",
             "action": "GetInfrastructureSuggestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAdditionalNode": {
+        "UpdateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "CreateAdditionalNode",
+            "action": "UpdateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAllowedResources": {
+        "GetResourceCostEstimate": {
             "access_level": "Undocumented",
-            "action": "ListAllowedResources",
+            "action": "GetResourceCostEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeployments": {
+        "StartProvisioning": {
             "access_level": "Undocumented",
-            "action": "ListDeployments",
+            "action": "StartProvisioning",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAdditionalNode": {
+        "ListSettingsSets": {
             "access_level": "Undocumented",
-            "action": "DescribeAdditionalNode",
+            "action": "ListSettingsSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeProvisionedApp": {
             "access_level": "Undocumented",
             "action": "DescribeProvisionedApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSettingsSet": {
+        "GetIpAddress": {
             "access_level": "Undocumented",
-            "action": "DeleteSettingsSet",
+            "action": "GetIpAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSettingsSet": {
+        "ListResourceCostEstimates": {
             "access_level": "Undocumented",
-            "action": "UpdateSettingsSet",
+            "action": "ListResourceCostEstimates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeployment": {
+        "CreateAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "DeleteDeployment",
+            "action": "CreateAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetDeployment": {
             "access_level": "Undocumented",
             "action": "GetDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeploymentEvents": {
+        "ListWorkloadDeploymentPatterns": {
             "access_level": "Undocumented",
-            "action": "ListDeploymentEvents",
+            "action": "ListWorkloadDeploymentPatterns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceCostEstimates": {
+        "PutSettingsSet": {
             "access_level": "Undocumented",
-            "action": "ListResourceCostEstimates",
+            "action": "PutSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloadDeploymentOptions": {
+        "ListWorkloads": {
             "access_level": "Undocumented",
-            "action": "ListWorkloadDeploymentOptions",
+            "action": "ListWorkloads",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisioningEvents": {
+        "GetWorkloadAsset": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisioningEvents",
+            "action": "GetWorkloadAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProvisioning": {
+        "DeleteAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "StartProvisioning",
+            "action": "DeleteAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSettingsSet": {
+        "DescribeProvisioningEvents": {
             "access_level": "Undocumented",
-            "action": "GetSettingsSet",
+            "action": "DescribeProvisioningEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAdditionalNode": {
+        "GetWorkload": {
             "access_level": "Undocumented",
-            "action": "DeleteAdditionalNode",
+            "action": "GetWorkload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkloadAssets": {
+        "DescribeAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "GetWorkloadAssets",
+            "action": "DescribeAdditionalNode",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListProvisionedApps": {
+            "access_level": "Undocumented",
+            "action": "ListProvisionedApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeSettingsSet": {
             "access_level": "Undocumented",
             "action": "DescribeSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloads": {
+        "DeleteDeployment": {
             "access_level": "Undocumented",
-            "action": "ListWorkloads",
+            "action": "DeleteDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkload": {
+        "GetSettingsSet": {
             "access_level": "Undocumented",
-            "action": "GetWorkload",
+            "action": "GetSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSettingsSet": {
+        "CreateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "PutSettingsSet",
+            "action": "CreateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceRecommendation": {
+        "GetWorkloadAssets": {
             "access_level": "Undocumented",
-            "action": "GetResourceRecommendation",
+            "action": "GetWorkloadAssets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdditionalNodes": {
+        "ListDeploymentEvents": {
             "access_level": "Undocumented",
-            "action": "ListAdditionalNodes",
+            "action": "ListDeploymentEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceCostEstimate": {
+        "ListWorkloadDeploymentOptions": {
             "access_level": "Undocumented",
-            "action": "GetResourceCostEstimate",
+            "action": "ListWorkloadDeploymentOptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloadDeploymentPatterns": {
+        "GetResourceRecommendation": {
             "access_level": "Undocumented",
-            "action": "ListWorkloadDeploymentPatterns",
+            "action": "GetResourceRecommendation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeployment": {
+        "ListAllowedResources": {
             "access_level": "Undocumented",
-            "action": "CreateDeployment",
+            "action": "ListAllowedResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProvisionedApps": {
+        "DeleteApp": {
             "access_level": "Undocumented",
-            "action": "ListProvisionedApps",
+            "action": "DeleteApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkloadAsset": {
+        "CreateDeployment": {
             "access_level": "Undocumented",
-            "action": "GetWorkloadAsset",
+            "action": "CreateDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSettingsSets": {
+        "ListAdditionalNodes": {
             "access_level": "Undocumented",
-            "action": "ListSettingsSets",
+            "action": "ListAdditionalNodes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIpAddress": {
+        "ListDeployments": {
             "access_level": "Undocumented",
-            "action": "GetIpAddress",
+            "action": "ListDeployments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApp": {
+        "DeleteSettingsSet": {
             "access_level": "Undocumented",
-            "action": "DeleteApp",
+            "action": "DeleteSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "lex": {
@@ -105705,99 +105705,99 @@
             "orphan": false,
             "resources": [
                 "proposal"
             ]
         }
     },
     "managedblockchain-query": {
-        "ListAssetContracts": {
+        "ListTokenBalances": {
             "access_level": "Undocumented",
-            "action": "ListAssetContracts",
+            "action": "ListTokenBalances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssetContract": {
+        "GetTokenBalance": {
             "access_level": "Undocumented",
-            "action": "GetAssetContract",
+            "action": "GetTokenBalance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTokenBalance": {
+        "ListTransactions": {
             "access_level": "Undocumented",
-            "action": "GetTokenBalance",
+            "action": "ListTransactions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTransactions": {
+        "ListFilteredTransactionEvents": {
             "access_level": "Undocumented",
-            "action": "ListTransactions",
+            "action": "ListFilteredTransactionEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "BatchGetTokenBalance": {
             "access_level": "Undocumented",
             "action": "BatchGetTokenBalance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTransactionEvents": {
+        "GetTransaction": {
             "access_level": "Undocumented",
-            "action": "ListTransactionEvents",
+            "action": "GetTransaction",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFilteredTransactionEvents": {
+        "GetAssetContract": {
             "access_level": "Undocumented",
-            "action": "ListFilteredTransactionEvents",
+            "action": "GetAssetContract",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTokenBalances": {
+        "ListTransactionEvents": {
             "access_level": "Undocumented",
-            "action": "ListTokenBalances",
+            "action": "ListTransactionEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTransaction": {
+        "ListAssetContracts": {
             "access_level": "Undocumented",
-            "action": "GetTransaction",
+            "action": "ListAssetContracts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "mapcredits": {
-        "ListQuarterCredits": {
+        "ListQuarterSpend": {
             "access_level": "Undocumented",
-            "action": "ListQuarterCredits",
+            "action": "ListQuarterSpend",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQuarterSpend": {
+        "ListQuarterCredits": {
             "access_level": "Undocumented",
-            "action": "ListQuarterSpend",
+            "action": "ListQuarterCredits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListAssociatedPrograms": {
             "access_level": "Undocumented",
@@ -108249,225 +108249,225 @@
             "orphan": false,
             "resources": [
                 "packaging-groups"
             ]
         }
     },
     "mediapackagev2": {
-        "CreateOriginEndpoint": {
+        "GetChannel": {
             "access_level": "Undocumented",
-            "action": "CreateOriginEndpoint",
+            "action": "GetChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateChannelGroup": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateChannelGroup",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetObject": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannel": {
+        "PutOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "GetChannel",
+            "action": "PutOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOriginEndpoints": {
+        "DeleteOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListOriginEndpoints",
+            "action": "DeleteOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetObject": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetObject",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannelGroups": {
+        "GetOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListChannelGroups",
+            "action": "GetOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateChannel": {
+        "ListOriginEndpoints": {
             "access_level": "Undocumented",
-            "action": "CreateChannel",
+            "action": "ListOriginEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListChannels": {
             "access_level": "Undocumented",
             "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutObject": {
+        "DeleteChannel": {
             "access_level": "Undocumented",
-            "action": "PutObject",
+            "action": "DeleteChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannel": {
+        "DeleteChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteChannel",
+            "action": "DeleteChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetHeadObject": {
             "access_level": "Undocumented",
             "action": "GetHeadObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOriginEndpointPolicy": {
+        "PutObject": {
             "access_level": "Undocumented",
-            "action": "DeleteOriginEndpointPolicy",
+            "action": "PutObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpoint": {
+        "CreateOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpoint",
+            "action": "CreateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListChannelGroups": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListChannelGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutOriginEndpointPolicy": {
+        "UpdateChannelGroup": {
             "access_level": "Undocumented",
-            "action": "PutOriginEndpointPolicy",
+            "action": "UpdateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannelGroup": {
+        "DeleteOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelGroup",
+            "action": "DeleteOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelPolicy": {
+        "DeleteChannelGroup": {
             "access_level": "Undocumented",
-            "action": "GetChannelPolicy",
+            "action": "DeleteChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOriginEndpoint": {
+        "GetChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteOriginEndpoint",
+            "action": "GetChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChannelGroup": {
+        "GetChannelGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateChannelGroup",
+            "action": "GetChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateOriginEndpoint": {
             "access_level": "Undocumented",
             "action": "UpdateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpointPolicy": {
+        "CreateChannelGroup": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpointPolicy",
+            "action": "CreateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutChannelPolicy": {
+        "UpdateChannel": {
             "access_level": "Undocumented",
-            "action": "PutChannelPolicy",
+            "action": "UpdateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelGroup": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetChannelGroup",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannelPolicy": {
+        "CreateChannel": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelPolicy",
+            "action": "CreateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChannel": {
+        "PutChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateChannel",
+            "action": "PutChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "mediastore": {
@@ -109185,161 +109185,161 @@
             "orphan": false,
             "resources": [
                 "vodSource"
             ]
         }
     },
     "medical-imaging": {
-        "StartDICOMImportJob": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "StartDICOMImportJob",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CopyImageSet": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CopyImageSet",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDatastore": {
+        "GetDatastore": {
             "access_level": "Undocumented",
-            "action": "DeleteDatastore",
+            "action": "GetDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteImageSet": {
+        "ListImageSetVersions": {
             "access_level": "Undocumented",
-            "action": "DeleteImageSet",
+            "action": "ListImageSetVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListDatastores": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListDatastores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImageSetMetadata": {
+        "UpdateImageSetMetadata": {
             "access_level": "Undocumented",
-            "action": "GetImageSetMetadata",
+            "action": "UpdateImageSetMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateDatastore": {
             "access_level": "Undocumented",
             "action": "CreateDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImageSet": {
+        "ListDICOMImportJobs": {
             "access_level": "Undocumented",
-            "action": "GetImageSet",
+            "action": "ListDICOMImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImageFrame": {
+        "CopyImageSet": {
             "access_level": "Undocumented",
-            "action": "GetImageFrame",
+            "action": "CopyImageSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchImageSets": {
+        "GetDICOMInstance": {
             "access_level": "Undocumented",
-            "action": "SearchImageSets",
+            "action": "GetDICOMInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDatastores": {
+        "GetImageFrame": {
             "access_level": "Undocumented",
-            "action": "ListDatastores",
+            "action": "GetImageFrame",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDICOMInstance": {
+        "GetDICOMImportJob": {
             "access_level": "Undocumented",
-            "action": "GetDICOMInstance",
+            "action": "GetDICOMImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateImageSetMetadata": {
+        "DeleteImageSet": {
             "access_level": "Undocumented",
-            "action": "UpdateImageSetMetadata",
+            "action": "DeleteImageSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDICOMImportJob": {
+        "GetImageSet": {
             "access_level": "Undocumented",
-            "action": "GetDICOMImportJob",
+            "action": "GetImageSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "SearchImageSets": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "SearchImageSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "StartDICOMImportJob": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "StartDICOMImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDatastore": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetDatastore",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListImageSetVersions": {
+        "DeleteDatastore": {
             "access_level": "Undocumented",
-            "action": "ListImageSetVersions",
+            "action": "DeleteDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDICOMImportJobs": {
+        "GetImageSetMetadata": {
             "access_level": "Undocumented",
-            "action": "ListDICOMImportJobs",
+            "action": "GetImageSetMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "memorydb": {
@@ -113758,265 +113758,265 @@
             "orphan": false,
             "resources": [
                 "database"
             ]
         }
     },
     "neptune-graph": {
-        "CreateGraphUsingImportTask": {
+        "ListGraphs": {
             "access_level": "Undocumented",
-            "action": "CreateGraphUsingImportTask",
+            "action": "ListGraphs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGraphSnapshots": {
+        "DeletePrivateGraphEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListGraphSnapshots",
+            "action": "DeletePrivateGraphEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueries": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListQueries",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetGraph": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataViaQuery": {
+        "CreatePrivateGraphEndpoint": {
             "access_level": "Undocumented",
-            "action": "DeleteDataViaQuery",
+            "action": "CreatePrivateGraphEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePrivateGraphEndpoint": {
+        "GetGraphSnapshot": {
             "access_level": "Undocumented",
-            "action": "DeletePrivateGraphEndpoint",
+            "action": "GetGraphSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelImportTask": {
+        "CreateGraphSnapshot": {
             "access_level": "Undocumented",
-            "action": "CancelImportTask",
+            "action": "CreateGraphSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGraphSnapshot": {
+        "ReadDataViaQuery": {
             "access_level": "Undocumented",
-            "action": "CreateGraphSnapshot",
+            "action": "ReadDataViaQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartImportTask": {
+        "DeleteGraphSnapshot": {
             "access_level": "Undocumented",
-            "action": "StartImportTask",
+            "action": "DeleteGraphSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueryStatus": {
+        "GetGraphSummary": {
             "access_level": "Undocumented",
-            "action": "GetQueryStatus",
+            "action": "GetGraphSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGraph": {
+        "GetImportTask": {
             "access_level": "Undocumented",
-            "action": "DeleteGraph",
+            "action": "GetImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGraph": {
+        "GetQueryStatus": {
             "access_level": "Undocumented",
-            "action": "GetGraph",
+            "action": "GetQueryStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGraphSnapshot": {
+        "DeleteGraph": {
             "access_level": "Undocumented",
-            "action": "DeleteGraphSnapshot",
+            "action": "DeleteGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEngineStatus": {
+        "WriteDataViaQuery": {
             "access_level": "Undocumented",
-            "action": "GetEngineStatus",
+            "action": "WriteDataViaQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePrivateGraphEndpoint": {
+        "ListImportTasks": {
             "access_level": "Undocumented",
-            "action": "CreatePrivateGraphEndpoint",
+            "action": "ListImportTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetGraph": {
+        "CreateGraphUsingImportTask": {
             "access_level": "Undocumented",
-            "action": "ResetGraph",
+            "action": "CreateGraphUsingImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelQuery": {
+        "ResetGraph": {
             "access_level": "Undocumented",
-            "action": "CancelQuery",
+            "action": "ResetGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGraph": {
+        "CreateGraph": {
             "access_level": "Undocumented",
-            "action": "UpdateGraph",
+            "action": "CreateGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RestoreGraphFromSnapshot": {
+        "ListQueries": {
             "access_level": "Undocumented",
-            "action": "RestoreGraphFromSnapshot",
+            "action": "ListQueries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "WriteDataViaQuery": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "WriteDataViaQuery",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImportTask": {
+        "StartImportTask": {
             "access_level": "Undocumented",
-            "action": "GetImportTask",
+            "action": "StartImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrivateGraphEndpoints": {
+        "GetEngineStatus": {
             "access_level": "Undocumented",
-            "action": "ListPrivateGraphEndpoints",
+            "action": "GetEngineStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGraphSnapshot": {
+        "CancelImportTask": {
             "access_level": "Undocumented",
-            "action": "GetGraphSnapshot",
+            "action": "CancelImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListImportTasks": {
+        "ListPrivateGraphEndpoints": {
             "access_level": "Undocumented",
-            "action": "ListImportTasks",
+            "action": "ListPrivateGraphEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReadDataViaQuery": {
+        "CancelQuery": {
             "access_level": "Undocumented",
-            "action": "ReadDataViaQuery",
+            "action": "CancelQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGraph": {
+        "UpdateGraph": {
             "access_level": "Undocumented",
-            "action": "CreateGraph",
+            "action": "UpdateGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPrivateGraphEndpoint": {
+        "RestoreGraphFromSnapshot": {
             "access_level": "Undocumented",
-            "action": "GetPrivateGraphEndpoint",
+            "action": "RestoreGraphFromSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStatisticsStatus": {
+        "ListGraphSnapshots": {
             "access_level": "Undocumented",
-            "action": "GetStatisticsStatus",
+            "action": "ListGraphSnapshots",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGraphSummary": {
+        "DeleteDataViaQuery": {
             "access_level": "Undocumented",
-            "action": "GetGraphSummary",
+            "action": "DeleteDataViaQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetStatisticsStatus": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetStatisticsStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGraphs": {
+        "GetPrivateGraphEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListGraphs",
+            "action": "GetPrivateGraphEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "network-firewall": {
@@ -115391,155 +115391,155 @@
             "access_level": "Undocumented",
             "action": "CancelMessageResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConversation": {
+        "ListConversationMessages": {
             "access_level": "Undocumented",
-            "action": "CreateConversation",
+            "action": "ListConversationMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConversation": {
+        "ListConversations": {
             "access_level": "Undocumented",
-            "action": "DeleteConversation",
+            "action": "ListConversations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversations": {
+        "SendConversationMessage": {
             "access_level": "Undocumented",
-            "action": "ListConversations",
+            "action": "SendConversationMessage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "NotifyConversationIsActive": {
+        "CreateConversation": {
             "access_level": "Undocumented",
-            "action": "NotifyConversationIsActive",
+            "action": "CreateConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversationMessages": {
+        "DeleteConversation": {
             "access_level": "Undocumented",
-            "action": "ListConversationMessages",
+            "action": "DeleteConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendConversationMessage": {
+        "NotifyConversationIsActive": {
             "access_level": "Undocumented",
-            "action": "SendConversationMessage",
+            "action": "NotifyConversationIsActive",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "networkmonitor": {
-        "GetProbe": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetProbe",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UpdateProbe": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UpdateProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProbe": {
+        "CreateMonitor": {
             "access_level": "Undocumented",
-            "action": "DeleteProbe",
+            "action": "CreateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMonitor": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetMonitor",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProbe": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateProbe",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMonitor": {
+        "UpdateMonitor": {
             "access_level": "Undocumented",
-            "action": "DeleteMonitor",
+            "action": "UpdateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMonitor": {
+        "GetMonitor": {
             "access_level": "Undocumented",
-            "action": "CreateMonitor",
+            "action": "GetMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMonitors": {
+        "DeleteMonitor": {
             "access_level": "Undocumented",
-            "action": "ListMonitors",
+            "action": "DeleteMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProbe": {
+        "GetProbe": {
             "access_level": "Undocumented",
-            "action": "UpdateProbe",
+            "action": "GetProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateProbe": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMonitor": {
+        "DeleteProbe": {
             "access_level": "Undocumented",
-            "action": "UpdateMonitor",
+            "action": "DeleteProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListMonitors": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListMonitors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "nimble": {
@@ -116107,251 +116107,251 @@
             "orphan": false,
             "resources": [
                 "studio-component"
             ]
         }
     },
     "notifications": {
-        "ListTagsForResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNotificationConfiguration": {
+        "DeregisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "UpdateNotificationConfiguration",
+            "action": "DeregisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "UpdateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "UpdateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEventRule": {
+        "RegisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "DeleteEventRule",
+            "action": "RegisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventRule": {
+        "GetNotificationEvent": {
             "access_level": "Undocumented",
-            "action": "UpdateEventRule",
+            "action": "GetNotificationEvent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterNotificationHub": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "RegisterNotificationHub",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateChannel": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "AssociateChannel",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNotificationEvent": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "GetNotificationEvent",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNotificationConfiguration": {
+        "DisassociateChannel": {
             "access_level": "Undocumented",
-            "action": "DeleteNotificationConfiguration",
+            "action": "DisassociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationEvents": {
+        "ListEventRules": {
             "access_level": "Undocumented",
-            "action": "ListNotificationEvents",
+            "action": "ListEventRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationConfigurations": {
+        "ListNotificationEvents": {
             "access_level": "Undocumented",
-            "action": "ListNotificationConfigurations",
+            "action": "ListNotificationEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateChannel": {
+        "DeleteEventRule": {
             "access_level": "Undocumented",
-            "action": "DisassociateChannel",
+            "action": "DeleteEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdateEventRule": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNotificationConfiguration": {
+        "ListNotificationHubs": {
             "access_level": "Undocumented",
-            "action": "GetNotificationConfiguration",
+            "action": "ListNotificationHubs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNotificationConfiguration": {
+        "GetEventRule": {
             "access_level": "Undocumented",
-            "action": "CreateNotificationConfiguration",
+            "action": "GetEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationHubs": {
+        "CreateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListNotificationHubs",
+            "action": "CreateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEventRule": {
+        "DeleteNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateEventRule",
+            "action": "DeleteNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventRules": {
+        "ListNotificationConfigurations": {
             "access_level": "Undocumented",
-            "action": "ListEventRules",
+            "action": "ListNotificationConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterNotificationHub": {
+        "AssociateChannel": {
             "access_level": "Undocumented",
-            "action": "DeregisterNotificationHub",
+            "action": "AssociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventRule": {
+        "CreateEventRule": {
             "access_level": "Undocumented",
-            "action": "GetEventRule",
+            "action": "CreateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "notifications-contacts": {
-        "ListTagsForResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEmailContacts": {
+        "CreateEmailContact": {
             "access_level": "Undocumented",
-            "action": "ListEmailContacts",
+            "action": "CreateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEmailContact": {
+        "GetEmailContact": {
             "access_level": "Undocumented",
-            "action": "DeleteEmailContact",
+            "action": "GetEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ActivateEmailContact": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ActivateEmailContact",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "SendActivationCode": {
             "access_level": "Undocumented",
             "action": "SendActivationCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListEmailContacts": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListEmailContacts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEmailContact": {
+        "ActivateEmailContact": {
             "access_level": "Undocumented",
-            "action": "GetEmailContact",
+            "action": "ActivateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEmailContact": {
+        "DeleteEmailContact": {
             "access_level": "Undocumented",
-            "action": "CreateEmailContact",
+            "action": "DeleteEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "oam": {
@@ -116529,883 +116529,883 @@
             "orphan": false,
             "resources": [
                 "Link"
             ]
         }
     },
     "omics": {
-        "GetAnnotationImportJob": {
+        "DeleteReference": {
             "access_level": "Undocumented",
-            "action": "GetAnnotationImportJob",
+            "action": "DeleteReference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMultipartReadSetUploads": {
+        "ListReferenceImportJobs": {
             "access_level": "Undocumented",
-            "action": "ListMultipartReadSetUploads",
+            "action": "ListReferenceImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRun": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteRun",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "StartRun": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "StartRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRuns": {
+        "CancelAnnotationImportJob": {
             "access_level": "Undocumented",
-            "action": "ListRuns",
+            "action": "CancelAnnotationImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWorkflow": {
+        "CreateMultipartReadSetUpload": {
             "access_level": "Undocumented",
-            "action": "UpdateWorkflow",
+            "action": "CreateMultipartReadSetUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteShare": {
+        "GetShare": {
             "access_level": "Undocumented",
-            "action": "DeleteShare",
+            "action": "GetShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReferenceStores": {
+        "StartVariantImportJob": {
             "access_level": "Undocumented",
-            "action": "ListReferenceStores",
+            "action": "StartVariantImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "StartAnnotationImportJob": {
             "access_level": "Undocumented",
             "action": "StartAnnotationImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAnnotationStoreVersions": {
+        "GetAnnotationImportJob": {
             "access_level": "Undocumented",
-            "action": "DeleteAnnotationStoreVersions",
+            "action": "GetAnnotationImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReadSetActivationJob": {
+        "GetReadSet": {
             "access_level": "Undocumented",
-            "action": "StartReadSetActivationJob",
+            "action": "GetReadSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAnnotationStore": {
+        "ListAnnotationStores": {
             "access_level": "Undocumented",
-            "action": "UpdateAnnotationStore",
+            "action": "ListAnnotationStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRunGroup": {
+        "DeleteAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "UpdateRunGroup",
+            "action": "DeleteAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateShare": {
+        "AcceptShare": {
             "access_level": "Undocumented",
-            "action": "CreateShare",
+            "action": "AcceptShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAnnotationStore": {
+        "DeleteVariantStore": {
             "access_level": "Undocumented",
-            "action": "CreateAnnotationStore",
+            "action": "DeleteVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetVariantImportJob": {
+        "CreateSequenceStore": {
             "access_level": "Undocumented",
-            "action": "GetVariantImportJob",
+            "action": "CreateSequenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReferenceImportJobs": {
+        "GetAnnotationStoreVersion": {
             "access_level": "Undocumented",
-            "action": "ListReferenceImportJobs",
+            "action": "GetAnnotationStoreVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelVariantImportJob": {
+        "GetVariantImportJob": {
             "access_level": "Undocumented",
-            "action": "CancelVariantImportJob",
+            "action": "GetVariantImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteVariantStore": {
+        "StartReferenceImportJob": {
             "access_level": "Undocumented",
-            "action": "DeleteVariantStore",
+            "action": "StartReferenceImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnnotationStores": {
+        "DeleteShare": {
             "access_level": "Undocumented",
-            "action": "ListAnnotationStores",
+            "action": "DeleteShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetVariantStore": {
+        "ListReadSetExportJobs": {
             "access_level": "Undocumented",
-            "action": "GetVariantStore",
+            "action": "ListReadSetExportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnnotationStore": {
+        "CreateVariantStore": {
             "access_level": "Undocumented",
-            "action": "GetAnnotationStore",
+            "action": "CreateVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetImportJob": {
+        "ListReferenceStores": {
             "access_level": "Undocumented",
-            "action": "GetReadSetImportJob",
+            "action": "ListReferenceStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelAnnotationImportJob": {
+        "DeleteRunGroup": {
             "access_level": "Undocumented",
-            "action": "CancelAnnotationImportJob",
+            "action": "DeleteRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSequenceStore": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteSequenceStore",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRunGroup": {
+        "CreateWorkflow": {
             "access_level": "Undocumented",
-            "action": "GetRunGroup",
+            "action": "CreateWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelRun": {
+        "CancelVariantImportJob": {
             "access_level": "Undocumented",
-            "action": "CancelRun",
+            "action": "CancelVariantImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReference": {
+        "StartReadSetExportJob": {
             "access_level": "Undocumented",
-            "action": "GetReference",
+            "action": "StartReadSetExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetMetadata": {
+        "GetReferenceImportJob": {
             "access_level": "Undocumented",
-            "action": "GetReadSetMetadata",
+            "action": "GetReferenceImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMultipartReadSetUpload": {
+        "GetReferenceMetadata": {
             "access_level": "Undocumented",
-            "action": "CreateMultipartReadSetUpload",
+            "action": "GetReferenceMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CompleteMultipartReadSetUpload": {
+        "ListReadSets": {
             "access_level": "Undocumented",
-            "action": "CompleteMultipartReadSetUpload",
+            "action": "ListReadSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteReferenceStore": {
+        "GetSequenceStore": {
             "access_level": "Undocumented",
-            "action": "DeleteReferenceStore",
+            "action": "GetSequenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkflow": {
+        "DeleteReferenceStore": {
             "access_level": "Undocumented",
-            "action": "GetWorkflow",
+            "action": "DeleteReferenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkflows": {
+        "DeleteSequenceStore": {
             "access_level": "Undocumented",
-            "action": "ListWorkflows",
+            "action": "DeleteSequenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSets": {
+        "ListReadSetActivationJobs": {
             "access_level": "Undocumented",
-            "action": "ListReadSets",
+            "action": "ListReadSetActivationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchDeleteReadSet": {
+        "CreateShare": {
             "access_level": "Undocumented",
-            "action": "BatchDeleteReadSet",
+            "action": "CreateShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReferenceImportJob": {
+        "GetReadSetMetadata": {
             "access_level": "Undocumented",
-            "action": "GetReferenceImportJob",
+            "action": "GetReadSetMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetActivationJobs": {
+        "BatchDeleteReadSet": {
             "access_level": "Undocumented",
-            "action": "ListReadSetActivationJobs",
+            "action": "BatchDeleteReadSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWorkflow": {
+        "ListRunGroups": {
             "access_level": "Undocumented",
-            "action": "DeleteWorkflow",
+            "action": "ListRunGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAnnotationStoreVersion": {
+        "GetWorkflow": {
             "access_level": "Undocumented",
-            "action": "UpdateAnnotationStoreVersion",
+            "action": "GetWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRunTask": {
+        "GetReadSetImportJob": {
             "access_level": "Undocumented",
-            "action": "GetRunTask",
+            "action": "GetReadSetImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRun": {
+        "ListVariantStores": {
             "access_level": "Undocumented",
-            "action": "GetRun",
+            "action": "ListVariantStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetExportJobs": {
+        "UpdateAnnotationStoreVersion": {
             "access_level": "Undocumented",
-            "action": "ListReadSetExportJobs",
+            "action": "UpdateAnnotationStoreVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnnotationStoreVersions": {
+        "AbortMultipartReadSetUpload": {
             "access_level": "Undocumented",
-            "action": "ListAnnotationStoreVersions",
+            "action": "AbortMultipartReadSetUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartVariantImportJob": {
+        "GetReadSetExportJob": {
             "access_level": "Undocumented",
-            "action": "StartVariantImportJob",
+            "action": "GetReadSetExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSequenceStores": {
+        "UploadReadSetPart": {
             "access_level": "Undocumented",
-            "action": "ListSequenceStores",
+            "action": "UploadReadSetPart",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRunGroup": {
+        "GetAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "CreateRunGroup",
+            "action": "GetAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAnnotationStoreVersion": {
+        "ListReferences": {
             "access_level": "Undocumented",
-            "action": "CreateAnnotationStoreVersion",
+            "action": "ListReferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateVariantStore": {
+        "StartReadSetActivationJob": {
             "access_level": "Undocumented",
-            "action": "CreateVariantStore",
+            "action": "StartReadSetActivationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSequenceStore": {
+        "CreateAnnotationStoreVersion": {
             "access_level": "Undocumented",
-            "action": "GetSequenceStore",
+            "action": "CreateAnnotationStoreVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReferences": {
+        "GetReferenceStore": {
             "access_level": "Undocumented",
-            "action": "ListReferences",
+            "action": "GetReferenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteReference": {
+        "ListReadSetImportJobs": {
             "access_level": "Undocumented",
-            "action": "DeleteReference",
+            "action": "ListReadSetImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVariantImportJobs": {
+        "ListShares": {
             "access_level": "Undocumented",
-            "action": "ListVariantImportJobs",
+            "action": "ListShares",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReadSetExportJob": {
+        "DeleteRun": {
             "access_level": "Undocumented",
-            "action": "StartReadSetExportJob",
+            "action": "DeleteRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSet": {
+        "StartReadSetImportJob": {
             "access_level": "Undocumented",
-            "action": "GetReadSet",
+            "action": "StartReadSetImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSequenceStore": {
+        "CreateRunGroup": {
             "access_level": "Undocumented",
-            "action": "CreateSequenceStore",
+            "action": "CreateRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadReadSetPart": {
+        "GetReadSetActivationJob": {
             "access_level": "Undocumented",
-            "action": "UploadReadSetPart",
+            "action": "GetReadSetActivationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptShare": {
+        "ListWorkflows": {
             "access_level": "Undocumented",
-            "action": "AcceptShare",
+            "action": "ListWorkflows",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnnotationStoreVersion": {
+        "GetRunGroup": {
             "access_level": "Undocumented",
-            "action": "GetAnnotationStoreVersion",
+            "action": "GetRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListShares": {
+        "CancelRun": {
             "access_level": "Undocumented",
-            "action": "ListShares",
+            "action": "CancelRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateReferenceStore": {
+        "GetVariantStore": {
             "access_level": "Undocumented",
-            "action": "CreateReferenceStore",
+            "action": "GetVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReadSetImportJob": {
+        "CreateAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "StartReadSetImportJob",
+            "action": "CreateAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReferenceImportJob": {
+        "DeleteWorkflow": {
             "access_level": "Undocumented",
-            "action": "StartReferenceImportJob",
+            "action": "DeleteWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetActivationJob": {
+        "ListMultipartReadSetUploads": {
             "access_level": "Undocumented",
-            "action": "GetReadSetActivationJob",
+            "action": "ListMultipartReadSetUploads",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRunGroup": {
+        "CreateReferenceStore": {
             "access_level": "Undocumented",
-            "action": "DeleteRunGroup",
+            "action": "CreateReferenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAnnotationStore": {
+        "ListReadSetUploadParts": {
             "access_level": "Undocumented",
-            "action": "DeleteAnnotationStore",
+            "action": "ListReadSetUploadParts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnnotationImportJobs": {
+        "UpdateAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "ListAnnotationImportJobs",
+            "action": "UpdateAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AbortMultipartReadSetUpload": {
+        "UpdateVariantStore": {
             "access_level": "Undocumented",
-            "action": "AbortMultipartReadSetUpload",
+            "action": "UpdateVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetExportJob": {
+        "GetRunTask": {
             "access_level": "Undocumented",
-            "action": "GetReadSetExportJob",
+            "action": "GetRunTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartRun": {
+        "ListAnnotationStoreVersions": {
             "access_level": "Undocumented",
-            "action": "StartRun",
+            "action": "ListAnnotationStoreVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRunGroups": {
+        "ListRunTasks": {
             "access_level": "Undocumented",
-            "action": "ListRunGroups",
+            "action": "ListRunTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReferenceMetadata": {
+        "DeleteAnnotationStoreVersions": {
             "access_level": "Undocumented",
-            "action": "GetReferenceMetadata",
+            "action": "DeleteAnnotationStoreVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetShare": {
+        "ListRuns": {
             "access_level": "Undocumented",
-            "action": "GetShare",
+            "action": "ListRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRunTasks": {
+        "UpdateRunGroup": {
             "access_level": "Undocumented",
-            "action": "ListRunTasks",
+            "action": "UpdateRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetUploadParts": {
+        "GetRun": {
             "access_level": "Undocumented",
-            "action": "ListReadSetUploadParts",
+            "action": "GetRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWorkflow": {
+        "UpdateWorkflow": {
             "access_level": "Undocumented",
-            "action": "CreateWorkflow",
+            "action": "UpdateWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateVariantStore": {
+        "GetReference": {
             "access_level": "Undocumented",
-            "action": "UpdateVariantStore",
+            "action": "GetReference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetImportJobs": {
+        "CompleteMultipartReadSetUpload": {
             "access_level": "Undocumented",
-            "action": "ListReadSetImportJobs",
+            "action": "CompleteMultipartReadSetUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVariantStores": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListVariantStores",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReferenceStore": {
+        "ListSequenceStores": {
             "access_level": "Undocumented",
-            "action": "GetReferenceStore",
+            "action": "ListSequenceStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListVariantImportJobs": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListVariantImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListAnnotationImportJobs": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListAnnotationImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "one": {
-        "GetSiteAddress": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetSiteAddress",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceActivationQrCode": {
+        "ListDeviceInstances": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceActivationQrCode",
+            "action": "ListDeviceInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSite": {
+        "DeleteSite": {
             "access_level": "Undocumented",
-            "action": "UpdateSite",
+            "action": "DeleteSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceConfigurationTemplate": {
+        "GetDeviceInstance": {
             "access_level": "Undocumented",
-            "action": "GetDeviceConfigurationTemplate",
+            "action": "GetDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListUsers": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceConfigurationTemplates": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListDeviceConfigurationTemplates",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceConfigurationTemplate": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceConfigurationTemplate",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "DeleteDeviceInstance": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "DeleteDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDeviceConfigurationTemplate": {
+        "DeleteDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdateDeviceConfigurationTemplate",
+            "action": "DeleteDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceInstance": {
+        "GetDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceInstance",
+            "action": "GetDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateDeviceInstance": {
             "access_level": "Undocumented",
             "action": "UpdateDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSite": {
+        "CreateDeviceActivationQrCode": {
             "access_level": "Undocumented",
-            "action": "DeleteSite",
+            "action": "CreateDeviceActivationQrCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUsers": {
+        "ListSites": {
             "access_level": "Undocumented",
-            "action": "ListUsers",
+            "action": "ListSites",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSiteAddress": {
+        "GetDeviceInstanceConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateSiteAddress",
+            "action": "GetDeviceInstanceConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceInstance": {
+        "CreateDeviceInstance": {
             "access_level": "Undocumented",
-            "action": "GetDeviceInstance",
+            "action": "CreateDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSite": {
+        "UpdateSiteAddress": {
             "access_level": "Undocumented",
-            "action": "GetSite",
+            "action": "UpdateSiteAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSite": {
+        "CreateDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateSite",
+            "action": "CreateDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceInstanceConfiguration": {
+        "GetSiteAddress": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceInstanceConfiguration",
+            "action": "GetSiteAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSites": {
+        "CreateSite": {
             "access_level": "Undocumented",
-            "action": "ListSites",
+            "action": "CreateSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "RebootDevice": {
             "access_level": "Undocumented",
             "action": "RebootDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceConfigurationTemplate": {
+        "GetSite": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceConfigurationTemplate",
+            "action": "GetSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceInstance": {
+        "DeleteAssociatedDevice": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceInstance",
+            "action": "DeleteAssociatedDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceInstanceConfiguration": {
+        "UpdateDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "GetDeviceInstanceConfiguration",
+            "action": "UpdateDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateDeviceInstanceConfiguration": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateDeviceInstanceConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssociatedDevice": {
+        "ListDeviceConfigurationTemplates": {
             "access_level": "Undocumented",
-            "action": "DeleteAssociatedDevice",
+            "action": "ListDeviceConfigurationTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceInstances": {
+        "UpdateSite": {
             "access_level": "Undocumented",
-            "action": "ListDeviceInstances",
+            "action": "UpdateSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "opsworks": {
@@ -118878,129 +118878,129 @@
             "orphan": false,
             "resources": [
                 "policy"
             ]
         }
     },
     "osis": {
-        "Ingest": {
+        "GetPipelineBlueprint": {
             "access_level": "Undocumented",
-            "action": "Ingest",
+            "action": "GetPipelineBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreatePipeline": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePipeline": {
+        "GetPipelineChangeProgress": {
             "access_level": "Undocumented",
-            "action": "UpdatePipeline",
+            "action": "GetPipelineChangeProgress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPipelineBlueprints": {
+        "Ingest": {
             "access_level": "Undocumented",
-            "action": "ListPipelineBlueprints",
+            "action": "Ingest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListPipelineBlueprints": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListPipelineBlueprints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopPipeline": {
+        "DeletePipeline": {
             "access_level": "Undocumented",
-            "action": "StopPipeline",
+            "action": "DeletePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidatePipeline": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ValidatePipeline",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipeline": {
+        "UpdatePipeline": {
             "access_level": "Undocumented",
-            "action": "GetPipeline",
+            "action": "UpdatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePipeline": {
+        "StartPipeline": {
             "access_level": "Undocumented",
-            "action": "DeletePipeline",
+            "action": "StartPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineBlueprint": {
+        "StopPipeline": {
             "access_level": "Undocumented",
-            "action": "GetPipelineBlueprint",
+            "action": "StopPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPipeline": {
+        "ValidatePipeline": {
             "access_level": "Undocumented",
-            "action": "StartPipeline",
+            "action": "ValidatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePipeline": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreatePipeline",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListPipelines": {
             "access_level": "Undocumented",
             "action": "ListPipelines",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineChangeProgress": {
+        "GetPipeline": {
             "access_level": "Undocumented",
-            "action": "GetPipelineChangeProgress",
+            "action": "GetPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "outposts": {
@@ -119689,517 +119689,517 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "payment-cryptography": {
-        "VerifyPinData": {
+        "TranslatePinData": {
             "access_level": "Undocumented",
-            "action": "VerifyPinData",
+            "action": "TranslatePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCardValidationData": {
+        "GeneratePinData": {
             "access_level": "Undocumented",
-            "action": "GenerateCardValidationData",
+            "action": "GeneratePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyAuthRequestCryptogram": {
+        "GenerateCardValidationData": {
             "access_level": "Undocumented",
-            "action": "VerifyAuthRequestCryptogram",
+            "action": "GenerateCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ImportKey": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ImportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyCardValidationData": {
+        "ExportKey": {
             "access_level": "Undocumented",
-            "action": "VerifyCardValidationData",
+            "action": "ExportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RestoreKey": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "RestoreKey",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAlias": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetAlias",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPublicKeyCertificate": {
+        "EncryptData": {
             "access_level": "Undocumented",
-            "action": "GetPublicKeyCertificate",
+            "action": "EncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopKeyUsage": {
+        "GetParametersForExport": {
             "access_level": "Undocumented",
-            "action": "StopKeyUsage",
+            "action": "GetParametersForExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAlias": {
+        "StopKeyUsage": {
             "access_level": "Undocumented",
-            "action": "DeleteAlias",
+            "action": "StopKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateMac": {
+        "ListKeys": {
             "access_level": "Undocumented",
-            "action": "GenerateMac",
+            "action": "ListKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EncryptData": {
+        "RestoreKey": {
             "access_level": "Undocumented",
-            "action": "EncryptData",
+            "action": "RestoreKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecryptData": {
+        "VerifyAuthRequestCryptogram": {
             "access_level": "Undocumented",
-            "action": "DecryptData",
+            "action": "VerifyAuthRequestCryptogram",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKeys": {
+        "GetParametersForImport": {
             "access_level": "Undocumented",
-            "action": "ListKeys",
+            "action": "GetParametersForImport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReEncryptData": {
+        "GenerateMac": {
             "access_level": "Undocumented",
-            "action": "ReEncryptData",
+            "action": "GenerateMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateAlias": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForImport": {
+        "VerifyMac": {
             "access_level": "Undocumented",
-            "action": "GetParametersForImport",
+            "action": "VerifyMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKey": {
+        "DecryptData": {
             "access_level": "Undocumented",
-            "action": "DeleteKey",
+            "action": "DecryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyMac": {
+        "GetPublicKeyCertificate": {
             "access_level": "Undocumented",
-            "action": "VerifyMac",
+            "action": "GetPublicKeyCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForExport": {
+        "GetAlias": {
             "access_level": "Undocumented",
-            "action": "GetParametersForExport",
+            "action": "GetAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ImportKey": {
+        "ListAliases": {
             "access_level": "Undocumented",
-            "action": "ImportKey",
+            "action": "ListAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartKeyUsage": {
+        "DeleteAlias": {
             "access_level": "Undocumented",
-            "action": "StartKeyUsage",
+            "action": "DeleteAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKey": {
+        "DeleteKey": {
             "access_level": "Undocumented",
-            "action": "GetKey",
+            "action": "DeleteKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAliases": {
+        "GetKey": {
             "access_level": "Undocumented",
-            "action": "ListAliases",
+            "action": "GetKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAlias": {
+        "StartKeyUsage": {
             "access_level": "Undocumented",
-            "action": "UpdateAlias",
+            "action": "StartKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GeneratePinData": {
+        "CreateKey": {
             "access_level": "Undocumented",
-            "action": "GeneratePinData",
+            "action": "CreateKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TranslatePinData": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "TranslatePinData",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ExportKey": {
+        "ReEncryptData": {
             "access_level": "Undocumented",
-            "action": "ExportKey",
+            "action": "ReEncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAlias": {
+        "UpdateAlias": {
             "access_level": "Undocumented",
-            "action": "CreateAlias",
+            "action": "UpdateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "VerifyPinData": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "VerifyPinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKey": {
+        "VerifyCardValidationData": {
             "access_level": "Undocumented",
-            "action": "CreateKey",
+            "action": "VerifyCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "payments": {
-        "GetPaymentStatus": {
+        "GetPaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "GetPaymentStatus",
+            "action": "GetPaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePaymentPreferences": {
+        "MakePayment": {
             "access_level": "Undocumented",
-            "action": "UpdatePaymentPreferences",
+            "action": "MakePayment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePaymentInstrument": {
+        "DeletePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "CreatePaymentInstrument",
+            "action": "DeletePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePaymentInstrument": {
+        "CreatePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "DeletePaymentInstrument",
+            "action": "CreatePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPaymentInstrument": {
+        "GetPaymentStatus": {
             "access_level": "Undocumented",
-            "action": "GetPaymentInstrument",
+            "action": "GetPaymentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MakePayment": {
+        "ListPaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "MakePayment",
+            "action": "ListPaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPaymentPreferences": {
+        "UpdatePaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "ListPaymentPreferences",
+            "action": "UpdatePaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "pca-connector-ad": {
-        "UpdateTemplate": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateTemplate",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTemplateGroupAccessControlEntry": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteTemplateGroupAccessControlEntry",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteDirectoryRegistration": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteDirectoryRegistration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConnector": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateConnector",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDirectoryRegistration": {
+        "GetTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "DeleteDirectoryRegistration",
+            "action": "GetTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConnector": {
+        "ListTemplates": {
             "access_level": "Undocumented",
-            "action": "GetConnector",
+            "action": "ListTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateTemplate": {
             "access_level": "Undocumented",
             "action": "CreateTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConnectors": {
+        "ListServicePrincipalNames": {
             "access_level": "Undocumented",
-            "action": "ListConnectors",
+            "action": "ListServicePrincipalNames",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTemplate": {
+        "CreateTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "GetTemplate",
+            "action": "CreateTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateDirectoryRegistration": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateDirectoryRegistration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServicePrincipalNames": {
+        "GetConnector": {
             "access_level": "Undocumented",
-            "action": "ListServicePrincipalNames",
+            "action": "GetConnector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTemplateGroupAccessControlEntry": {
+        "ListConnectors": {
             "access_level": "Undocumented",
-            "action": "UpdateTemplateGroupAccessControlEntry",
+            "action": "ListConnectors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTemplateGroupAccessControlEntries": {
+        "DeleteConnector": {
             "access_level": "Undocumented",
-            "action": "ListTemplateGroupAccessControlEntries",
+            "action": "DeleteConnector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDirectoryRegistration": {
+        "ListDirectoryRegistrations": {
             "access_level": "Undocumented",
-            "action": "GetDirectoryRegistration",
+            "action": "ListDirectoryRegistrations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServicePrincipalName": {
+        "GetTemplate": {
             "access_level": "Undocumented",
-            "action": "GetServicePrincipalName",
+            "action": "GetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDirectoryRegistrations": {
+        "DeleteTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "ListDirectoryRegistrations",
+            "action": "DeleteTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConnector": {
+        "CreateServicePrincipalName": {
             "access_level": "Undocumented",
-            "action": "DeleteConnector",
+            "action": "CreateServicePrincipalName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTemplates": {
+        "GetServicePrincipalName": {
             "access_level": "Undocumented",
-            "action": "ListTemplates",
+            "action": "GetServicePrincipalName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdateTemplate": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteServicePrincipalName": {
             "access_level": "Undocumented",
             "action": "DeleteServicePrincipalName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDirectoryRegistration": {
+        "GetDirectoryRegistration": {
             "access_level": "Undocumented",
-            "action": "CreateDirectoryRegistration",
+            "action": "GetDirectoryRegistration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTemplateGroupAccessControlEntry": {
+        "CreateConnector": {
             "access_level": "Undocumented",
-            "action": "GetTemplateGroupAccessControlEntry",
+            "action": "CreateConnector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServicePrincipalName": {
+        "DeleteTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateServicePrincipalName",
+            "action": "DeleteTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTemplate": {
+        "ListTemplateGroupAccessControlEntries": {
             "access_level": "Undocumented",
-            "action": "DeleteTemplate",
+            "action": "ListTemplateGroupAccessControlEntries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTemplateGroupAccessControlEntry": {
+        "UpdateTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "CreateTemplateGroupAccessControlEntry",
+            "action": "UpdateTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "personalize": {
@@ -123557,797 +123557,797 @@
             "orphan": false,
             "resources": [
                 "purchase-order"
             ]
         }
     },
     "q": {
-        "CreateAssignment": {
+        "SendMessage": {
             "access_level": "Undocumented",
-            "action": "CreateAssignment",
+            "action": "SendMessage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConversation": {
+        "StartTroubleshootingResolutionExplanation": {
             "access_level": "Undocumented",
-            "action": "GetConversation",
+            "action": "StartTroubleshootingResolutionExplanation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssignment": {
+        "CreateAssignment": {
             "access_level": "Undocumented",
-            "action": "DeleteAssignment",
+            "action": "CreateAssignment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendMessage": {
+        "UpdateTroubleshootingCommandResult": {
             "access_level": "Undocumented",
-            "action": "SendMessage",
+            "action": "UpdateTroubleshootingCommandResult",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartTroubleshootingResolutionExplanation": {
+        "GetIdentityMetadata": {
             "access_level": "Undocumented",
-            "action": "StartTroubleshootingResolutionExplanation",
+            "action": "GetIdentityMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRequest": {
+        "ListConversations": {
             "access_level": "Undocumented",
-            "action": "PassRequest",
+            "action": "ListConversations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTroubleshootingCommandResult": {
+        "StartTroubleshootingAnalysis": {
             "access_level": "Undocumented",
-            "action": "UpdateTroubleshootingCommandResult",
+            "action": "StartTroubleshootingAnalysis",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTroubleshootingResults": {
+        "GetConversation": {
             "access_level": "Undocumented",
-            "action": "GetTroubleshootingResults",
+            "action": "GetConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartTroubleshootingAnalysis": {
+        "StartConversation": {
             "access_level": "Undocumented",
-            "action": "StartTroubleshootingAnalysis",
+            "action": "StartConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversations": {
+        "DeleteAssignment": {
             "access_level": "Undocumented",
-            "action": "ListConversations",
+            "action": "DeleteAssignment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdentityMetadata": {
+        "PassRequest": {
             "access_level": "Undocumented",
-            "action": "GetIdentityMetadata",
+            "action": "PassRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartConversation": {
+        "GetTroubleshootingResults": {
             "access_level": "Undocumented",
-            "action": "StartConversation",
+            "action": "GetTroubleshootingResults",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "qapps": {
-        "CreateSubscriptionToken": {
+        "ListQApps": {
             "access_level": "Undocumented",
-            "action": "CreateSubscriptionToken",
+            "action": "ListQApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartQAppSession": {
+        "CreateLibraryItemReview": {
             "access_level": "Undocumented",
-            "action": "StartQAppSession",
+            "action": "CreateLibraryItemReview",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopQAppSession": {
+        "CopyQApp": {
             "access_level": "Undocumented",
-            "action": "StopQAppSession",
+            "action": "CopyQApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLibraryItem": {
+        "ImportDocumentToQAppSession": {
             "access_level": "Undocumented",
-            "action": "GetLibraryItem",
+            "action": "ImportDocumentToQAppSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQApp": {
+        "GetLibraryItem": {
             "access_level": "Undocumented",
-            "action": "CreateQApp",
+            "action": "GetLibraryItem",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQApp": {
+        "AssociateQAppWithUser": {
             "access_level": "Undocumented",
-            "action": "UpdateQApp",
+            "action": "AssociateQAppWithUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CopyQApp": {
+        "DeleteLibraryItem": {
             "access_level": "Undocumented",
-            "action": "CopyQApp",
+            "action": "DeleteLibraryItem",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListLibraryItems": {
+        "StartQAppSession": {
             "access_level": "Undocumented",
-            "action": "ListLibraryItems",
+            "action": "StartQAppSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PredictProblemStatementFromConversation": {
+        "CreateLibraryItem": {
             "access_level": "Undocumented",
-            "action": "PredictProblemStatementFromConversation",
+            "action": "CreateLibraryItem",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQApp": {
+        "PredictProblemStatementFromConversation": {
             "access_level": "Undocumented",
-            "action": "DeleteQApp",
+            "action": "PredictProblemStatementFromConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQApps": {
+        "StopQAppSession": {
             "access_level": "Undocumented",
-            "action": "ListQApps",
+            "action": "StopQAppSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ImportDocumentToQApp": {
+        "UpdateQApp": {
             "access_level": "Undocumented",
-            "action": "ImportDocumentToQApp",
+            "action": "UpdateQApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQApp": {
+        "DisassociateQAppFromUser": {
             "access_level": "Undocumented",
-            "action": "GetQApp",
+            "action": "DisassociateQAppFromUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateLibraryItem": {
             "access_level": "Undocumented",
             "action": "UpdateLibraryItem",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateQAppFromUser": {
+        "ImportDocumentToQApp": {
             "access_level": "Undocumented",
-            "action": "DisassociateQAppFromUser",
+            "action": "ImportDocumentToQApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PredictQAppFromProblemStatement": {
+        "DeleteQApp": {
             "access_level": "Undocumented",
-            "action": "PredictQAppFromProblemStatement",
+            "action": "DeleteQApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ImportDocumentToQAppSession": {
+        "ListLibraryItems": {
             "access_level": "Undocumented",
-            "action": "ImportDocumentToQAppSession",
+            "action": "ListLibraryItems",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLibraryItem": {
+        "PredictQAppFromProblemStatement": {
             "access_level": "Undocumented",
-            "action": "CreateLibraryItem",
+            "action": "PredictQAppFromProblemStatement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLibraryItemReview": {
+        "CreateQApp": {
             "access_level": "Undocumented",
-            "action": "CreateLibraryItemReview",
+            "action": "CreateQApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLibraryItem": {
+        "CreateSubscriptionToken": {
             "access_level": "Undocumented",
-            "action": "DeleteLibraryItem",
+            "action": "CreateSubscriptionToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateQAppWithUser": {
+        "GetQApp": {
             "access_level": "Undocumented",
-            "action": "AssociateQAppWithUser",
+            "action": "GetQApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "qbusiness": {
-        "ListDataSourceSyncJobs": {
+        "CreateLicense": {
             "access_level": "Undocumented",
-            "action": "ListDataSourceSyncJobs",
+            "action": "CreateLicense",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
             "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUser": {
+        "GetGroup": {
             "access_level": "Undocumented",
-            "action": "GetUser",
+            "action": "GetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIndices": {
+        "GetDataSource": {
             "access_level": "Undocumented",
-            "action": "ListIndices",
+            "action": "GetDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscription": {
+        "ListSubscriptions": {
             "access_level": "Undocumented",
-            "action": "CreateSubscription",
+            "action": "ListSubscriptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartDataSourceSyncJob": {
+        "DeleteIndex": {
             "access_level": "Undocumented",
-            "action": "StartDataSourceSyncJob",
+            "action": "DeleteIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMessages": {
+        "ListApplications": {
             "access_level": "Undocumented",
-            "action": "ListMessages",
+            "action": "ListApplications",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListDataSources": {
             "access_level": "Undocumented",
             "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetApplication": {
+        "DeleteGroup": {
             "access_level": "Undocumented",
-            "action": "GetApplication",
+            "action": "DeleteGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConversation": {
+        "UpdateUser": {
             "access_level": "Undocumented",
-            "action": "DeleteConversation",
+            "action": "UpdateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchPutDocument": {
+        "Chat": {
             "access_level": "Undocumented",
-            "action": "BatchPutDocument",
+            "action": "Chat",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserLicenses": {
+        "ListMessages": {
             "access_level": "Undocumented",
-            "action": "ListUserLicenses",
+            "action": "ListMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ChatSync": {
+        "CreateApplication": {
             "access_level": "Undocumented",
-            "action": "ChatSync",
+            "action": "CreateApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWebExperiences": {
+        "PutFeedback": {
             "access_level": "Undocumented",
-            "action": "ListWebExperiences",
+            "action": "PutFeedback",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLicense": {
+        "DeleteApplication": {
             "access_level": "Undocumented",
-            "action": "CreateLicense",
+            "action": "DeleteApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateApplication": {
+        "CreateRetriever": {
             "access_level": "Undocumented",
-            "action": "CreateApplication",
+            "action": "CreateRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveUserLicenses": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "RemoveUserLicenses",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSource": {
+        "PutGroup": {
             "access_level": "Undocumented",
-            "action": "GetDataSource",
+            "action": "PutGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutGroup": {
+        "DeletePlugin": {
             "access_level": "Undocumented",
-            "action": "PutGroup",
+            "action": "DeletePlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRetriever": {
+        "CancelSubscription": {
             "access_level": "Undocumented",
-            "action": "UpdateRetriever",
+            "action": "CancelSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIndex": {
+        "CreatePlugin": {
             "access_level": "Undocumented",
-            "action": "UpdateIndex",
+            "action": "CreatePlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWebExperience": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetWebExperience",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopDataSourceSyncJob": {
+        "GetLicense": {
             "access_level": "Undocumented",
-            "action": "StopDataSourceSyncJob",
+            "action": "GetLicense",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Chat": {
+        "ListGroups": {
             "access_level": "Undocumented",
-            "action": "Chat",
+            "action": "ListGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "ListConversations": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "ListConversations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPlugins": {
+        "RemoveUserLicenses": {
             "access_level": "Undocumented",
-            "action": "ListPlugins",
+            "action": "RemoveUserLicenses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIndex": {
+        "UpdateChatControlsConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteIndex",
+            "action": "UpdateChatControlsConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePlugin": {
+        "ListDocuments": {
             "access_level": "Undocumented",
-            "action": "CreatePlugin",
+            "action": "ListDocuments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "ChatSync": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "ChatSync",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIndex": {
+        "DeleteConversation": {
             "access_level": "Undocumented",
-            "action": "GetIndex",
+            "action": "DeleteConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLicense": {
+        "GetChatControlsConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetLicense",
+            "action": "GetChatControlsConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRetrievers": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "ListRetrievers",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPlugin": {
+        "ListPlugins": {
             "access_level": "Undocumented",
-            "action": "GetPlugin",
+            "action": "ListPlugins",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFeedback": {
+        "GetWebExperience": {
             "access_level": "Undocumented",
-            "action": "PutFeedback",
+            "action": "GetWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWebExperience": {
+        "UpdateRetriever": {
             "access_level": "Undocumented",
-            "action": "UpdateWebExperience",
+            "action": "UpdateRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChatControlsConfiguration": {
+        "DeleteRetriever": {
             "access_level": "Undocumented",
-            "action": "GetChatControlsConfiguration",
+            "action": "DeleteRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddUserLicenses": {
+        "ListWebExperiences": {
             "access_level": "Undocumented",
-            "action": "AddUserLicenses",
+            "action": "ListWebExperiences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePlugin": {
+        "DeleteWebExperience": {
             "access_level": "Undocumented",
-            "action": "UpdatePlugin",
+            "action": "DeleteWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchDeleteDocument": {
+        "ListUserLicenses": {
             "access_level": "Undocumented",
-            "action": "BatchDeleteDocument",
+            "action": "ListUserLicenses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptions": {
+        "ListDataSourceSyncJobs": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptions",
+            "action": "ListDataSourceSyncJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "BatchDeleteDocument": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "BatchDeleteDocument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUser": {
+        "ListIndices": {
             "access_level": "Undocumented",
-            "action": "UpdateUser",
+            "action": "ListIndices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWebExperience": {
+        "UpdateApplication": {
             "access_level": "Undocumented",
-            "action": "DeleteWebExperience",
+            "action": "UpdateApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApplication": {
+        "UpdateIndex": {
             "access_level": "Undocumented",
-            "action": "DeleteApplication",
+            "action": "UpdateIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroups": {
+        "UpdatePlugin": {
             "access_level": "Undocumented",
-            "action": "ListGroups",
+            "action": "UpdatePlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSubscription": {
+        "GetPlugin": {
             "access_level": "Undocumented",
-            "action": "CancelSubscription",
+            "action": "GetPlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRetriever": {
+        "UpdateWebExperience": {
             "access_level": "Undocumented",
-            "action": "CreateRetriever",
+            "action": "UpdateWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDocuments": {
+        "CreateUser": {
             "access_level": "Undocumented",
-            "action": "ListDocuments",
+            "action": "CreateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "GetApplication": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "GetApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRetriever": {
+        "GetRetriever": {
             "access_level": "Undocumented",
-            "action": "DeleteRetriever",
+            "action": "GetRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWebExperience": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "CreateWebExperience",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSubscription": {
+        "GetUser": {
             "access_level": "Undocumented",
-            "action": "UpdateSubscription",
+            "action": "GetUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIndex": {
+        "ListRetrievers": {
             "access_level": "Undocumented",
-            "action": "CreateIndex",
+            "action": "ListRetrievers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListApplications": {
+        "StopDataSourceSyncJob": {
             "access_level": "Undocumented",
-            "action": "ListApplications",
+            "action": "StopDataSourceSyncJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePlugin": {
+        "CreateWebExperience": {
             "access_level": "Undocumented",
-            "action": "DeletePlugin",
+            "action": "CreateWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUser": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "CreateUser",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRetriever": {
+        "UpdateSubscription": {
             "access_level": "Undocumented",
-            "action": "GetRetriever",
+            "action": "UpdateSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChatControlsConfiguration": {
+        "DeleteChatControlsConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateChatControlsConfiguration",
+            "action": "DeleteChatControlsConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroup": {
+        "CreateIndex": {
             "access_level": "Undocumented",
-            "action": "GetGroup",
+            "action": "CreateIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChatControlsConfiguration": {
+        "GetIndex": {
             "access_level": "Undocumented",
-            "action": "DeleteChatControlsConfiguration",
+            "action": "GetIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "StartDataSourceSyncJob": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "StartDataSourceSyncJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroup": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteGroup",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversations": {
+        "CreateSubscription": {
             "access_level": "Undocumented",
-            "action": "ListConversations",
+            "action": "CreateSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "BatchPutDocument": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "BatchPutDocument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateApplication": {
+        "AddUserLicenses": {
             "access_level": "Undocumented",
-            "action": "UpdateApplication",
+            "action": "AddUserLicenses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "qldb": {
@@ -126828,273 +126828,273 @@
             "access_level": "Undocumented",
             "action": "CreatePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePolicies": {
+        "RejectResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "GetResourcePolicies",
+            "action": "RejectResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShares": {
+        "ListPendingInvitationResources": {
             "access_level": "Undocumented",
-            "action": "GetResourceShares",
+            "action": "ListPendingInvitationResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromoteResourceShareCreatedFromPolicy": {
+        "ListResources": {
             "access_level": "Undocumented",
-            "action": "PromoteResourceShareCreatedFromPolicy",
+            "action": "ListResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermission": {
+        "ListPermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "DeletePermission",
+            "action": "ListPermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissions": {
+        "DisassociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListPermissions",
+            "action": "DisassociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareInvitations": {
+        "DisassociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareInvitations",
+            "action": "DisassociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromotePermissionCreatedFromPolicy": {
+        "GetResourceShares": {
             "access_level": "Undocumented",
-            "action": "PromotePermissionCreatedFromPolicy",
+            "action": "GetResourceShares",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptResourceShareInvitation": {
+        "AssociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "AcceptResourceShareInvitation",
+            "action": "AssociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceShare": {
+        "ListPrincipals": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceShare",
+            "action": "ListPrincipals",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionAssociations": {
+        "ReplacePermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "ListPermissionAssociations",
+            "action": "ReplacePermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceSharePermission": {
+        "ListResourceTypes": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceSharePermission",
+            "action": "ListResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReplacePermissionAssociations": {
+        "SetDefaultPermissionVersion": {
             "access_level": "Undocumented",
-            "action": "ReplacePermissionAssociations",
+            "action": "SetDefaultPermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareAssociations": {
+        "DeletePermission": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareAssociations",
+            "action": "DeletePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPendingInvitationResources": {
+        "PromoteResourceShareCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "ListPendingInvitationResources",
+            "action": "PromoteResourceShareCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPermissionVersion": {
+        "DeletePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPermissionVersion",
+            "action": "DeletePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPermission": {
+        "AssociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "GetPermission",
+            "action": "AssociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermissionVersion": {
+        "CreatePermission": {
             "access_level": "Undocumented",
-            "action": "DeletePermissionVersion",
+            "action": "CreatePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListResourceSharePermissions": {
             "access_level": "Undocumented",
             "action": "ListResourceSharePermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResourceShare": {
+        "ListReplacePermissionAssociationsWork": {
             "access_level": "Undocumented",
-            "action": "DeleteResourceShare",
+            "action": "ListReplacePermissionAssociationsWork",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResourceShare": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateResourceShare",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResources": {
+        "UpdateResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListResources",
+            "action": "UpdateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceShare": {
+        "EnableSharingWithAwsOrganization": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceShare",
+            "action": "EnableSharingWithAwsOrganization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceTypes": {
+        "GetPermission": {
             "access_level": "Undocumented",
-            "action": "ListResourceTypes",
+            "action": "GetPermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableSharingWithAwsOrganization": {
+        "PromotePermissionCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "EnableSharingWithAwsOrganization",
+            "action": "PromotePermissionCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermission": {
+        "ListPermissionVersions": {
             "access_level": "Undocumented",
-            "action": "CreatePermission",
+            "action": "ListPermissionVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceSharePermission": {
+        "DeleteResourceShare": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceSharePermission",
+            "action": "DeleteResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionVersions": {
+        "GetResourceShareAssociations": {
             "access_level": "Undocumented",
-            "action": "ListPermissionVersions",
+            "action": "GetResourceShareAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectResourceShareInvitation": {
+        "GetResourceShareInvitations": {
             "access_level": "Undocumented",
-            "action": "RejectResourceShareInvitation",
+            "action": "GetResourceShareInvitations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReplacePermissionAssociationsWork": {
+        "CreateResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListReplacePermissionAssociationsWork",
+            "action": "CreateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrincipals": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListPrincipals",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "AcceptResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "AcceptResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceShare": {
+        "GetResourcePolicies": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceShare",
+            "action": "GetResourcePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListPermissions": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListPermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "rbin": {
@@ -132476,565 +132476,565 @@
             "orphan": false,
             "resources": [
                 "streamprocessor"
             ]
         }
     },
     "repostspace": {
-        "ListTagsForResource": {
+        "SendInvites": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "SendInvites",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterAdmin": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeregisterAdmin",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterAdmin": {
+        "DeleteSpace": {
             "access_level": "Undocumented",
-            "action": "RegisterAdmin",
+            "action": "DeleteSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendInvites": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "SendInvites",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSpace": {
+        "RegisterAdmin": {
             "access_level": "Undocumented",
-            "action": "DeleteSpace",
+            "action": "RegisterAdmin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSpace": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateSpace",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSpace": {
+        "GetSpace": {
             "access_level": "Undocumented",
-            "action": "CreateSpace",
+            "action": "GetSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSpace": {
+        "UpdateSpace": {
             "access_level": "Undocumented",
-            "action": "GetSpace",
+            "action": "UpdateSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSpaces": {
+        "CreateSpace": {
             "access_level": "Undocumented",
-            "action": "ListSpaces",
+            "action": "CreateSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeregisterAdmin": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeregisterAdmin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListSpaces": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListSpaces",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "resiliencehub": {
-        "CreateResiliencyPolicy": {
+        "ListAppAssessments": {
             "access_level": "Undocumented",
-            "action": "CreateResiliencyPolicy",
+            "action": "ListAppAssessments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersionAppComponents": {
+        "DescribeAppVersionTemplate": {
             "access_level": "Undocumented",
-            "action": "ListAppVersionAppComponents",
+            "action": "DescribeAppVersionTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersionResources": {
+        "DeleteAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "ListAppVersionResources",
+            "action": "DeleteAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "BatchUpdateRecommendationStatus": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "BatchUpdateRecommendationStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAppAssessment": {
+        "DescribeAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "StartAppAssessment",
+            "action": "DescribeAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeDraftAppVersionResourcesImportStatus": {
+        "ListAppAssessmentResourceDrifts": {
             "access_level": "Undocumented",
-            "action": "DescribeDraftAppVersionResourcesImportStatus",
+            "action": "ListAppAssessmentResourceDrifts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSuggestedResiliencyPolicies": {
+        "ListAppVersionAppComponents": {
             "access_level": "Undocumented",
-            "action": "ListSuggestedResiliencyPolicies",
+            "action": "ListAppVersionAppComponents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ImportResourcesToDraftAppVersion": {
+        "CreateAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "ImportResourcesToDraftAppVersion",
+            "action": "CreateAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeResiliencyPolicy": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DescribeResiliencyPolicy",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppInputSources": {
+        "DescribeResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "ListAppInputSources",
+            "action": "DescribeResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListApps": {
+        "ListAppVersions": {
             "access_level": "Undocumented",
-            "action": "ListApps",
+            "action": "ListAppVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAlarmRecommendations": {
+        "CreateAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "ListAlarmRecommendations",
+            "action": "CreateAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAssessments": {
+        "ListAppAssessmentComplianceDrifts": {
             "access_level": "Undocumented",
-            "action": "ListAppAssessments",
+            "action": "ListAppAssessmentComplianceDrifts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSopRecommendations": {
+        "DeleteRecommendationTemplate": {
             "access_level": "Undocumented",
-            "action": "ListSopRecommendations",
+            "action": "DeleteRecommendationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppVersionAppComponent": {
+        "CreateRecommendationTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdateAppVersionAppComponent",
+            "action": "CreateRecommendationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersions": {
+        "DescribeDraftAppVersionResourcesImportStatus": {
             "access_level": "Undocumented",
-            "action": "ListAppVersions",
+            "action": "DescribeDraftAppVersionResourcesImportStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListAppVersionResourceMappings": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListAppVersionResourceMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppVersionResource": {
+        "DescribeAppVersionResourcesResolutionStatus": {
             "access_level": "Undocumented",
-            "action": "CreateAppVersionResource",
+            "action": "DescribeAppVersionResourcesResolutionStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateApp": {
+        "ListApps": {
             "access_level": "Undocumented",
-            "action": "CreateApp",
+            "action": "ListApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResiliencyPolicies": {
+        "ListSopRecommendations": {
             "access_level": "Undocumented",
-            "action": "ListResiliencyPolicies",
+            "action": "ListSopRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResiliencyPolicy": {
+        "CreateResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateResiliencyPolicy",
+            "action": "CreateResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRecommendationTemplates": {
+        "CreateApp": {
             "access_level": "Undocumented",
-            "action": "ListRecommendationTemplates",
+            "action": "CreateApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRecommendationTemplate": {
+        "RemoveDraftAppVersionResourceMappings": {
             "access_level": "Undocumented",
-            "action": "DeleteRecommendationTemplate",
+            "action": "RemoveDraftAppVersionResourceMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppVersionResource": {
+        "ImportResourcesToDraftAppVersion": {
             "access_level": "Undocumented",
-            "action": "DeleteAppVersionResource",
+            "action": "ImportResourcesToDraftAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppVersionResource": {
+        "ListTestRecommendations": {
             "access_level": "Undocumented",
-            "action": "UpdateAppVersionResource",
+            "action": "ListTestRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppAssessment": {
+        "StartAppAssessment": {
             "access_level": "Undocumented",
-            "action": "DeleteAppAssessment",
+            "action": "StartAppAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUnsupportedAppVersionResources": {
+        "DescribeApp": {
             "access_level": "Undocumented",
-            "action": "ListUnsupportedAppVersionResources",
+            "action": "DescribeApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppComponentRecommendations": {
+        "DescribeAppAssessment": {
             "access_level": "Undocumented",
-            "action": "ListAppComponentRecommendations",
+            "action": "DescribeAppAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppInputSource": {
+        "DeleteAppAssessment": {
             "access_level": "Undocumented",
-            "action": "DeleteAppInputSource",
+            "action": "DeleteAppAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppComponentCompliances": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListAppComponentCompliances",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRecommendationTemplate": {
+        "DeleteAppInputSource": {
             "access_level": "Undocumented",
-            "action": "CreateRecommendationTemplate",
+            "action": "DeleteAppInputSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAssessmentComplianceDrifts": {
+        "ResolveAppVersionResources": {
             "access_level": "Undocumented",
-            "action": "ListAppAssessmentComplianceDrifts",
+            "action": "ResolveAppVersionResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddDraftAppVersionResourceMappings": {
+        "ListAppComponentRecommendations": {
             "access_level": "Undocumented",
-            "action": "AddDraftAppVersionResourceMappings",
+            "action": "ListAppComponentRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResolveAppVersionResources": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ResolveAppVersionResources",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateApp": {
+        "UpdateAppVersion": {
             "access_level": "Undocumented",
-            "action": "UpdateApp",
+            "action": "UpdateAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppVersionAppComponent": {
+        "ListResiliencyPolicies": {
             "access_level": "Undocumented",
-            "action": "CreateAppVersionAppComponent",
+            "action": "ListResiliencyPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionAppComponent": {
+        "UpdateAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionAppComponent",
+            "action": "UpdateAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutDraftAppVersionTemplate": {
+        "UpdateApp": {
             "access_level": "Undocumented",
-            "action": "PutDraftAppVersionTemplate",
+            "action": "UpdateApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersionResourceMappings": {
+        "DescribeAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "ListAppVersionResourceMappings",
+            "action": "DescribeAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PublishAppVersion": {
+        "ListAlarmRecommendations": {
             "access_level": "Undocumented",
-            "action": "PublishAppVersion",
+            "action": "ListAlarmRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppAssessment": {
+        "ListAppComponentCompliances": {
             "access_level": "Undocumented",
-            "action": "DescribeAppAssessment",
+            "action": "ListAppComponentCompliances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionResourcesResolutionStatus": {
+        "DeleteResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionResourcesResolutionStatus",
+            "action": "DeleteResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionTemplate": {
+        "DescribeAppVersion": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionTemplate",
+            "action": "DescribeAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchUpdateRecommendationStatus": {
+        "ListAppInputSources": {
             "access_level": "Undocumented",
-            "action": "BatchUpdateRecommendationStatus",
+            "action": "ListAppInputSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersion": {
+        "ListAppVersionResources": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersion",
+            "action": "ListAppVersionResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionResource": {
+        "ListRecommendationTemplates": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionResource",
+            "action": "ListRecommendationTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAssessmentResourceDrifts": {
+        "ListUnsupportedAppVersionResources": {
             "access_level": "Undocumented",
-            "action": "ListAppAssessmentResourceDrifts",
+            "action": "ListUnsupportedAppVersionResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppVersion": {
+        "UpdateResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateAppVersion",
+            "action": "UpdateResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppVersionAppComponent": {
+        "UpdateAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "DeleteAppVersionAppComponent",
+            "action": "UpdateAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveDraftAppVersionResourceMappings": {
+        "PutDraftAppVersionTemplate": {
             "access_level": "Undocumented",
-            "action": "RemoveDraftAppVersionResourceMappings",
+            "action": "PutDraftAppVersionTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeApp": {
+        "ListSuggestedResiliencyPolicies": {
             "access_level": "Undocumented",
-            "action": "DescribeApp",
+            "action": "ListSuggestedResiliencyPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResiliencyPolicy": {
+        "DeleteApp": {
             "access_level": "Undocumented",
-            "action": "DeleteResiliencyPolicy",
+            "action": "DeleteApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApp": {
+        "AddDraftAppVersionResourceMappings": {
             "access_level": "Undocumented",
-            "action": "DeleteApp",
+            "action": "AddDraftAppVersionResourceMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTestRecommendations": {
+        "PublishAppVersion": {
             "access_level": "Undocumented",
-            "action": "ListTestRecommendations",
+            "action": "PublishAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "resource-explorer": {
-        "ListResourceTypes": {
+        "ListResources": {
             "access_level": "Undocumented",
-            "action": "ListResourceTypes",
+            "action": "ListResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResources": {
+        "ListTags": {
             "access_level": "Undocumented",
-            "action": "ListResources",
+            "action": "ListTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTags": {
+        "ListResourceTypes": {
             "access_level": "Undocumented",
-            "action": "ListTags",
+            "action": "ListResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "resource-explorer-2": {
@@ -135988,89 +135988,89 @@
             "condition_keys": [],
             "description": "Grants permission to get all the domain-related billing records for the current AWS account for a specified period",
             "orphan": false,
             "resources": []
         }
     },
     "route53profiles": {
-        "GetProfile": {
+        "GetProfileAssociation": {
             "access_level": "Undocumented",
-            "action": "GetProfile",
+            "action": "GetProfileAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListProfiles": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateProfile": {
+        "ListProfileAssociations": {
             "access_level": "Undocumented",
-            "action": "AssociateProfile",
+            "action": "ListProfileAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProfileResourceAssociation": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateProfileResourceAssociation",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceFromProfile": {
+        "ListProfileResourceAssociations": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceFromProfile",
+            "action": "ListProfileResourceAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProfileResourceAssociation": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetProfileResourceAssociation",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProfile": {
+        "DisassociateProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteProfile",
+            "action": "DisassociateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProfileAssociations": {
+        "DisassociateResourceFromProfile": {
             "access_level": "Undocumented",
-            "action": "ListProfileAssociations",
+            "action": "DisassociateResourceFromProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProfileResourceAssociations": {
+        "UpdateProfileResourceAssociation": {
             "access_level": "Undocumented",
-            "action": "ListProfileResourceAssociations",
+            "action": "UpdateProfileResourceAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProfiles": {
+        "GetProfileResourceAssociation": {
             "access_level": "Undocumented",
-            "action": "ListProfiles",
+            "action": "GetProfileResourceAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "AssociateResourceToProfile": {
             "access_level": "Undocumented",
@@ -136084,41 +136084,41 @@
             "access_level": "Undocumented",
             "action": "CreateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteProfile": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateProfile": {
+        "AssociateProfile": {
             "access_level": "Undocumented",
-            "action": "DisassociateProfile",
+            "action": "AssociateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProfileAssociation": {
+        "GetProfile": {
             "access_level": "Undocumented",
-            "action": "GetProfileAssociation",
+            "action": "GetProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "route53resolver": {
@@ -141138,65 +141138,65 @@
             "orphan": false,
             "resources": [
                 "object"
             ]
         }
     },
     "s3express": {
-        "CreateBucket": {
+        "GetBucketPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateBucket",
+            "action": "GetBucketPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteBucket": {
             "access_level": "Undocumented",
             "action": "DeleteBucket",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAllMyDirectoryBuckets": {
+        "DeleteBucketPolicy": {
             "access_level": "Undocumented",
-            "action": "ListAllMyDirectoryBuckets",
+            "action": "DeleteBucketPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBucketPolicy": {
+        "ListAllMyDirectoryBuckets": {
             "access_level": "Undocumented",
-            "action": "GetBucketPolicy",
+            "action": "ListAllMyDirectoryBuckets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSession": {
+        "PutBucketPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateSession",
+            "action": "PutBucketPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteBucketPolicy": {
+        "CreateSession": {
             "access_level": "Undocumented",
-            "action": "DeleteBucketPolicy",
+            "action": "CreateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutBucketPolicy": {
+        "CreateBucket": {
             "access_level": "Undocumented",
-            "action": "PutBucketPolicy",
+            "action": "CreateBucket",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "sagemaker": {
@@ -145977,137 +145977,137 @@
             "orphan": false,
             "resources": [
                 "schema"
             ]
         }
     },
     "scn": {
-        "ListInstances": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListInstances",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
             "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillOfMaterialsImportJob": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetBillOfMaterialsImportJob",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateBillOfMaterialsImportJob": {
+        "ListInstances": {
             "access_level": "Undocumented",
-            "action": "CreateBillOfMaterialsImportJob",
+            "action": "ListInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateInstance": {
+        "DeleteSSOApplication": {
             "access_level": "Undocumented",
-            "action": "UpdateInstance",
+            "action": "DeleteSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveAdminPermissionsForUser": {
+        "CreateBillOfMaterialsImportJob": {
             "access_level": "Undocumented",
-            "action": "RemoveAdminPermissionsForUser",
+            "action": "CreateBillOfMaterialsImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssignAdminPermissionsToUser": {
+        "RemoveAdminPermissionsForUser": {
             "access_level": "Undocumented",
-            "action": "AssignAdminPermissionsToUser",
+            "action": "RemoveAdminPermissionsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataIntegrationEvent": {
+        "GetBillOfMaterialsImportJob": {
             "access_level": "Undocumented",
-            "action": "SendDataIntegrationEvent",
+            "action": "GetBillOfMaterialsImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeInstance": {
+        "CreateInstance": {
             "access_level": "Undocumented",
-            "action": "DescribeInstance",
+            "action": "CreateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSOApplication": {
+        "ListAdminUsers": {
             "access_level": "Undocumented",
-            "action": "DeleteSSOApplication",
+            "action": "ListAdminUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstance": {
+        "AssignAdminPermissionsToUser": {
             "access_level": "Undocumented",
-            "action": "CreateInstance",
+            "action": "AssignAdminPermissionsToUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstance": {
+        "DescribeInstance": {
             "access_level": "Undocumented",
-            "action": "DeleteInstance",
+            "action": "DescribeInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSSOApplication": {
+        "DeleteInstance": {
             "access_level": "Undocumented",
-            "action": "CreateSSOApplication",
+            "action": "DeleteInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateSSOApplication": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdateInstance": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdminUsers": {
+        "SendDataIntegrationEvent": {
             "access_level": "Undocumented",
-            "action": "ListAdminUsers",
+            "action": "SendDataIntegrationEvent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "sdb": {
@@ -162153,65 +162153,73 @@
             "orphan": false,
             "resources": [
                 "adapter"
             ]
         }
     },
     "thinclient": {
-        "CreateEnvironment": {
+        "DeregisterDevice": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironment",
+            "action": "DeregisterDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDevice": {
+        "ListEnvironments": {
             "access_level": "Undocumented",
-            "action": "GetDevice",
+            "action": "ListEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironments": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListEnvironments",
+            "action": "ListTagsForResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListSoftwareSets": {
             "access_level": "Undocumented",
             "action": "ListSoftwareSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListDeviceSessions": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListDeviceSessions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetEnvironment": {
             "access_level": "Undocumented",
             "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceSessions": {
+        "UpdateSoftwareSet": {
             "access_level": "Undocumented",
-            "action": "ListDeviceSessions",
+            "action": "UpdateSoftwareSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateEnvironment": {
             "access_level": "Undocumented",
@@ -162225,65 +162233,57 @@
             "access_level": "Undocumented",
             "action": "DeleteEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterDevice": {
-            "access_level": "Undocumented",
-            "action": "DeregisterDevice",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "UpdateDevice": {
+        "CreateEnvironment": {
             "access_level": "Undocumented",
-            "action": "UpdateDevice",
+            "action": "CreateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSoftwareSet": {
+        "GetDevice": {
             "access_level": "Undocumented",
-            "action": "UpdateSoftwareSet",
+            "action": "GetDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDevice": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteDevice",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetSoftwareSet": {
             "access_level": "Undocumented",
             "action": "GetSoftwareSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UpdateDevice": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UpdateDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteDevice": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListDevices": {
             "access_level": "Undocumented",
@@ -162657,97 +162657,97 @@
             "orphan": false,
             "resources": [
                 "table"
             ]
         }
     },
     "timestream-influxdb": {
-        "TagResource": {
+        "CreateDbParameterGroup": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateDbParameterGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDbInstance": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteDbInstance",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetDbParameterGroup": {
             "access_level": "Undocumented",
             "action": "GetDbParameterGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetDbInstance": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDbInstance": {
+        "CreateDbInstance": {
             "access_level": "Undocumented",
-            "action": "UpdateDbInstance",
+            "action": "CreateDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListDbInstances": {
             "access_level": "Undocumented",
             "action": "ListDbInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListDbParameterGroups": {
             "access_level": "Undocumented",
             "action": "ListDbParameterGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDbInstance": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateDbInstance",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDbInstance": {
+        "UpdateDbInstance": {
             "access_level": "Undocumented",
-            "action": "GetDbInstance",
+            "action": "UpdateDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDbParameterGroup": {
+        "DeleteDbInstance": {
             "access_level": "Undocumented",
-            "action": "CreateDbParameterGroup",
+            "action": "DeleteDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "tiros": {
@@ -162789,273 +162789,273 @@
             "condition_keys": [],
             "description": "Grants permission to list accounts that might be useful in a new query",
             "orphan": false,
             "resources": []
         }
     },
     "tnb": {
-        "CreateSolNetworkInstance": {
+        "InstantiateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkInstance",
+            "action": "InstantiateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
             "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkInstance": {
+        "ValidateSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkInstance",
+            "action": "ValidateSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionInstance": {
+        "TerminateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionInstance",
+            "action": "TerminateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageContent": {
+        "GetSolFunctionPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageContent",
+            "action": "GetSolFunctionPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolFunctionPackage": {
+        "GetSolNetworkPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "UpdateSolFunctionPackage",
+            "action": "GetSolNetworkPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolNetworkPackageContent": {
+        "DeleteSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "ValidateSolNetworkPackageContent",
+            "action": "DeleteSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolFunctionPackageContent": {
+        "ListSolNetworkOperations": {
             "access_level": "Undocumented",
-            "action": "PutSolFunctionPackageContent",
+            "action": "ListSolNetworkOperations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolFunctionPackageContent": {
+        "CreateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "ValidateSolFunctionPackageContent",
+            "action": "CreateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkInstances": {
+        "GetSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkInstances",
+            "action": "GetSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteSolFunctionPackage": {
             "access_level": "Undocumented",
             "action": "DeleteSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkPackage": {
+        "PutSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkPackage",
+            "action": "PutSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkPackage": {
+        "UpdateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkPackage",
+            "action": "UpdateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageDescriptor": {
+        "PutSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageDescriptor",
+            "action": "PutSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InstantiateSolNetworkInstance": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "InstantiateSolNetworkInstance",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkInstance": {
+        "CreateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkInstance",
+            "action": "CreateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkPackage": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkPackage",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TerminateSolNetworkInstance": {
+        "ListSolNetworkInstances": {
             "access_level": "Undocumented",
-            "action": "TerminateSolNetworkInstance",
+            "action": "ListSolNetworkInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSolNetworkOperation": {
+        "GetSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "CancelSolNetworkOperation",
+            "action": "GetSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkInstance": {
+        "DeleteSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkInstance",
+            "action": "DeleteSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkPackages": {
+        "ListSolFunctionInstances": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkPackages",
+            "action": "ListSolFunctionInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolNetworkPackageContent": {
+        "GetSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "PutSolNetworkPackageContent",
+            "action": "GetSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackage": {
+        "UpdateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackage",
+            "action": "UpdateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkOperation": {
+        "CancelSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkOperation",
+            "action": "CancelSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionInstances": {
+        "ListSolNetworkPackages": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionInstances",
+            "action": "ListSolNetworkPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolFunctionPackage": {
+        "CreateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "CreateSolFunctionPackage",
+            "action": "CreateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageContent": {
+        "GetSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageContent",
+            "action": "GetSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionPackages": {
+        "ValidateSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionPackages",
+            "action": "ValidateSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkOperations": {
+        "UpdateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkOperations",
+            "action": "UpdateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageDescriptor": {
+        "GetSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageDescriptor",
+            "action": "GetSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetSolFunctionInstance": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetSolFunctionInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListSolFunctionPackages": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListSolFunctionPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackage": {
+        "GetSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackage",
+            "action": "GetSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "transcribe": {
@@ -164773,131 +164773,131 @@
             "condition_keys": [],
             "description": "Grants permission to update the risk status in AWS Trusted Advisor Priority",
             "orphan": false,
             "resources": []
         }
     },
     "ts": {
-        "ListTagsForResource": {
+        "GetExecutionOutput": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetExecutionOutput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExecutions": {
+        "GetExecution": {
             "access_level": "Undocumented",
-            "action": "ListExecutions",
+            "action": "GetExecution",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartExecution": {
+        "GetTool": {
             "access_level": "Undocumented",
-            "action": "StartExecution",
+            "action": "GetTool",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTools": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListTools",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "StartExecution": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "StartExecution",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExecutionOutput": {
+        "ListExecutions": {
             "access_level": "Undocumented",
-            "action": "GetExecutionOutput",
+            "action": "ListExecutions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExecution": {
+        "ListTools": {
             "access_level": "Undocumented",
-            "action": "GetExecution",
+            "action": "ListTools",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTool": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetTool",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "user-subscriptions": {
-        "ListUserSubscriptions": {
+        "UpdateClaim": {
             "access_level": "Undocumented",
-            "action": "ListUserSubscriptions",
+            "action": "UpdateClaim",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateClaim": {
+        "DeleteClaim": {
             "access_level": "Undocumented",
-            "action": "CreateClaim",
+            "action": "DeleteClaim",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListClaims": {
             "access_level": "Undocumented",
             "action": "ListClaims",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteClaim": {
+        "CreateClaim": {
             "access_level": "Undocumented",
-            "action": "DeleteClaim",
+            "action": "CreateClaim",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateClaim": {
+        "ListApplicationClaims": {
             "access_level": "Undocumented",
-            "action": "UpdateClaim",
+            "action": "ListApplicationClaims",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListApplicationClaims": {
+        "ListUserSubscriptions": {
             "access_level": "Undocumented",
-            "action": "ListApplicationClaims",
+            "action": "ListUserSubscriptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "vendor-insights": {
@@ -165183,201 +165183,201 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "verifiedpermissions": {
-        "ListIdentitySources": {
+        "IsAuthorizedWithToken": {
             "access_level": "Undocumented",
-            "action": "ListIdentitySources",
+            "action": "IsAuthorizedWithToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicies": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "ListPolicies",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdentitySource": {
+        "GetPolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateIdentitySource",
+            "action": "GetPolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicy": {
+        "ListPolicyTemplates": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicy",
+            "action": "ListPolicyTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IsAuthorizedWithToken": {
+        "UpdatePolicyStore": {
             "access_level": "Undocumented",
-            "action": "IsAuthorizedWithToken",
+            "action": "UpdatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "DeletePolicyStore": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "DeletePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "GetIdentitySource": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "GetIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IsAuthorized": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "IsAuthorized",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyStore": {
+        "CreatePolicyStore": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyStore",
+            "action": "CreatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdentitySource": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateIdentitySource",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyStore": {
+        "UpdatePolicy": {
             "access_level": "Undocumented",
-            "action": "GetPolicyStore",
+            "action": "UpdatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTemplates": {
+        "UpdatePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTemplates",
+            "action": "UpdatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdentitySource": {
+        "DeletePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteIdentitySource",
+            "action": "DeletePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "UpdateIdentitySource": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "UpdateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicyStore": {
+        "DeleteIdentitySource": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicyStore",
+            "action": "DeleteIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyStore": {
+        "PutSchema": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyStore",
+            "action": "PutSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "GetPolicyStore": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "GetPolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyTemplate": {
+        "CreatePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "GetPolicyTemplate",
+            "action": "CreatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicyTemplate": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicyTemplate",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSchema": {
+        "IsAuthorized": {
             "access_level": "Undocumented",
-            "action": "PutSchema",
+            "action": "IsAuthorized",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyStores": {
+        "ListPolicies": {
             "access_level": "Undocumented",
-            "action": "ListPolicyStores",
+            "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdentitySource": {
+        "CreateIdentitySource": {
             "access_level": "Undocumented",
-            "action": "GetIdentitySource",
+            "action": "CreateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyTemplate": {
+        "ListPolicyStores": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyTemplate",
+            "action": "ListPolicyStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyTemplate": {
+        "ListIdentitySources": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyTemplate",
+            "action": "ListIdentitySources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "voiceid": {
@@ -169356,385 +169356,385 @@
             "orphan": false,
             "resources": [
                 "network"
             ]
         }
     },
     "wisdom": {
-        "GetKnowledgeBase": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetKnowledgeBase",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListContentAssociations": {
+        "ListAssistants": {
             "access_level": "Undocumented",
-            "action": "ListContentAssociations",
+            "action": "ListAssistants",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListContentAssociations": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListContentAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateContent": {
+        "ListImportJobs": {
             "access_level": "Undocumented",
-            "action": "UpdateContent",
+            "action": "ListImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetAssistant": {
             "access_level": "Undocumented",
             "action": "GetAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSession": {
+        "GetContent": {
             "access_level": "Undocumented",
-            "action": "CreateSession",
+            "action": "GetContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateKnowledgeBaseTemplateUri": {
+        "DeleteAssistantAssociation": {
             "access_level": "Undocumented",
-            "action": "UpdateKnowledgeBaseTemplateUri",
+            "action": "DeleteAssistantAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListImportJobs": {
+        "GetAssistantAssociation": {
             "access_level": "Undocumented",
-            "action": "ListImportJobs",
+            "action": "GetAssistantAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQuickResponse": {
+        "SearchContent": {
             "access_level": "Undocumented",
-            "action": "DeleteQuickResponse",
+            "action": "SearchContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "QueryAssistant": {
+        "GetContentSummary": {
             "access_level": "Undocumented",
-            "action": "QueryAssistant",
+            "action": "GetContentSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssistant": {
+        "ListAssistantAssociations": {
             "access_level": "Undocumented",
-            "action": "DeleteAssistant",
+            "action": "ListAssistantAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListContents": {
+        "CreateAssistant": {
             "access_level": "Undocumented",
-            "action": "ListContents",
+            "action": "CreateAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKnowledgeBase": {
+        "GetRecommendations": {
             "access_level": "Undocumented",
-            "action": "DeleteKnowledgeBase",
+            "action": "GetRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateContent": {
+        "StartImportJob": {
             "access_level": "Undocumented",
-            "action": "CreateContent",
+            "action": "StartImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQuickResponse": {
+        "PutFeedback": {
             "access_level": "Undocumented",
-            "action": "UpdateQuickResponse",
+            "action": "PutFeedback",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteImportJob": {
+        "DeleteQuickResponse": {
             "access_level": "Undocumented",
-            "action": "DeleteImportJob",
+            "action": "DeleteQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSession": {
+        "DeleteContent": {
             "access_level": "Undocumented",
-            "action": "GetSession",
+            "action": "DeleteContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImportJob": {
+        "CreateContentAssociation": {
             "access_level": "Undocumented",
-            "action": "GetImportJob",
+            "action": "CreateContentAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssistants": {
+        "SearchQuickResponses": {
             "access_level": "Undocumented",
-            "action": "ListAssistants",
+            "action": "SearchQuickResponses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQuickResponses": {
+        "NotifyRecommendationsReceived": {
             "access_level": "Undocumented",
-            "action": "ListQuickResponses",
+            "action": "NotifyRecommendationsReceived",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteContentAssociation": {
+        "CreateKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "DeleteContentAssociation",
+            "action": "CreateKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "NotifyRecommendationsReceived": {
+        "UpdateQuickResponse": {
             "access_level": "Undocumented",
-            "action": "NotifyRecommendationsReceived",
+            "action": "UpdateQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKnowledgeBase": {
+        "CreateContent": {
             "access_level": "Undocumented",
-            "action": "CreateKnowledgeBase",
+            "action": "CreateContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContent": {
+        "GetSession": {
             "access_level": "Undocumented",
-            "action": "GetContent",
+            "action": "GetSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContentAssociation": {
+        "SearchSessions": {
             "access_level": "Undocumented",
-            "action": "GetContentAssociation",
+            "action": "SearchSessions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContentSummary": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetContentSummary",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateContentAssociation": {
+        "UpdateSession": {
             "access_level": "Undocumented",
-            "action": "CreateContentAssociation",
+            "action": "UpdateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKnowledgeBases": {
+        "GetImportJob": {
             "access_level": "Undocumented",
-            "action": "ListKnowledgeBases",
+            "action": "GetImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQuickResponse": {
+        "CreateAssistantAssociation": {
             "access_level": "Undocumented",
-            "action": "CreateQuickResponse",
+            "action": "CreateAssistantAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSession": {
+        "UpdateContent": {
             "access_level": "Undocumented",
-            "action": "UpdateSession",
+            "action": "UpdateContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssistantAssociation": {
+        "DeleteImportJob": {
             "access_level": "Undocumented",
-            "action": "DeleteAssistantAssociation",
+            "action": "DeleteImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssistantAssociations": {
+        "GetQuickResponse": {
             "access_level": "Undocumented",
-            "action": "ListAssistantAssociations",
+            "action": "GetQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchQuickResponses": {
+        "DeleteKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "SearchQuickResponses",
+            "action": "DeleteKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartContentUpload": {
+        "RemoveKnowledgeBaseTemplateUri": {
             "access_level": "Undocumented",
-            "action": "StartContentUpload",
+            "action": "RemoveKnowledgeBaseTemplateUri",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecommendations": {
+        "ListQuickResponses": {
             "access_level": "Undocumented",
-            "action": "GetRecommendations",
+            "action": "ListQuickResponses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssistantAssociation": {
+        "GetContentAssociation": {
             "access_level": "Undocumented",
-            "action": "CreateAssistantAssociation",
+            "action": "GetContentAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteContent": {
+        "QueryAssistant": {
             "access_level": "Undocumented",
-            "action": "DeleteContent",
+            "action": "QueryAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQuickResponse": {
+        "ListContents": {
             "access_level": "Undocumented",
-            "action": "GetQuickResponse",
+            "action": "ListContents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFeedback": {
+        "CreateSession": {
             "access_level": "Undocumented",
-            "action": "PutFeedback",
+            "action": "CreateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartImportJob": {
+        "CreateQuickResponse": {
             "access_level": "Undocumented",
-            "action": "StartImportJob",
+            "action": "CreateQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveKnowledgeBaseTemplateUri": {
+        "DeleteAssistant": {
             "access_level": "Undocumented",
-            "action": "RemoveKnowledgeBaseTemplateUri",
+            "action": "DeleteAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssistantAssociation": {
+        "ListKnowledgeBases": {
             "access_level": "Undocumented",
-            "action": "GetAssistantAssociation",
+            "action": "ListKnowledgeBases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssistant": {
+        "UpdateKnowledgeBaseTemplateUri": {
             "access_level": "Undocumented",
-            "action": "CreateAssistant",
+            "action": "UpdateKnowledgeBaseTemplateUri",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchContent": {
+        "DeleteContentAssociation": {
             "access_level": "Undocumented",
-            "action": "SearchContent",
+            "action": "DeleteContentAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Undocumented",
             "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchSessions": {
+        "StartContentUpload": {
             "access_level": "Undocumented",
-            "action": "SearchSessions",
+            "action": "StartContentUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "workdocs": {
```

### Comparing `iam_actions-1.2.20240519/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240520/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240519/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240520/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240519/iam_actions/generate/generate.py` & `iam_actions-1.2.20240520/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240519/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240520/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240519/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240520/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240519/iam_actions/generate/services.py` & `iam_actions-1.2.20240520/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240519/iam_actions/policies.json` & `iam_actions-1.2.20240520/iam_actions/policies.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240519/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240520/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240519/iam_actions/services.json` & `iam_actions-1.2.20240520/iam_actions/services.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240519/pyproject.toml` & `iam_actions-1.2.20240520/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240519"
+version = "1.2.20240520"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240519/setup.py` & `iam_actions-1.2.20240520/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240519',
+    'version': '1.2.20240520',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240519/PKG-INFO` & `iam_actions-1.2.20240520/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240519
+Version: 1.2.20240520
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

