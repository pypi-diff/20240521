# Comparing `tmp/mypy_boto3_cloudfront-1.34.110.tar.gz` & `tmp/mypy-boto3-cloudfront-1.34.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_cloudfront-1.34.110.tar", last modified: Tue May 21 19:32:44 2024, max compression
+gzip compressed data, was "mypy-boto3-cloudfront-1.34.83.tar", last modified: Thu Apr 11 19:18:06 2024, max compression
```

## Comparing `mypy_boto3_cloudfront-1.34.110.tar` & `mypy-boto3-cloudfront-1.34.83.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:32:44.324801 mypy_boto3_cloudfront-1.34.110/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-21 19:31:54.000000 mypy_boto3_cloudfront-1.34.110/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-05-21 19:32:44.324801 mypy_boto3_cloudfront-1.34.110/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12988 2024-05-21 19:31:54.000000 mypy_boto3_cloudfront-1.34.110/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:32:44.324801 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-21 19:31:54.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-21 19:31:54.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-21 19:31:54.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    83080 2024-05-21 19:31:55.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    83077 2024-05-21 19:31:54.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13468 2024-05-21 19:31:55.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13468 2024-05-21 19:31:55.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-05-21 19:31:55.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-21 19:31:55.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:31:54.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   128158 2024-05-21 19:31:57.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   128158 2024-05-21 19:31:57.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 19:31:54.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-21 19:31:55.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-21 19:31:55.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:32:44.324801 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-05-21 19:32:44.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-21 19:32:44.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:32:44.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:32:44.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-21 19:32:44.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 19:32:44.000000 mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 19:32:44.324801 mypy_boto3_cloudfront-1.34.110/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-21 19:31:54.000000 mypy_boto3_cloudfront-1.34.110/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:06.011387 mypy-boto3-cloudfront-1.34.83/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14554 2024-04-11 19:18:06.011387 mypy-boto3-cloudfront-1.34.83/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:06.011387 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82896 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82893 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-04-11 19:17:12.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-04-11 19:17:12.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   105119 2024-04-11 19:17:14.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105119 2024-04-11 19:17:13.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:06.011387 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14554 2024-04-11 19:18:05.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-11 19:18:05.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:05.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:05.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 19:18:05.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 19:18:05.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:18:06.011387 mypy-boto3-cloudfront-1.34.83/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/setup.py
```

### Comparing `mypy_boto3_cloudfront-1.34.110/LICENSE` & `mypy-boto3-cloudfront-1.34.83/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cloudfront-1.34.110/PKG-INFO` & `mypy-boto3-cloudfront-1.34.83/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudfront
-Version: 1.34.110
-Summary: Type annotations for boto3.CloudFront 1.34.110 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.83
+Summary: Type annotations for boto3.CloudFront 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudfront)](https://pepy.tech/project/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.34.110](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_cloudfront-1.34.110/README.md` & `mypy-boto3-cloudfront-1.34.83/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudfront)](https://pepy.tech/project/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.34.110](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/__init__.py` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/__init__.pyi` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/__main__.py` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudFront 1.34.110\n"
-        "Version:         1.34.110\n"
-        "Builder version: 7.24.0\n"
+        "Type annotations for boto3.CloudFront 1.34.83\n"
+        "Version:         1.34.83\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.110")
+    print("1.34.83")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/client.py` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     ListDistributionsPaginator,
     ListInvalidationsPaginator,
     ListKeyValueStoresPaginator,
     ListStreamingDistributionsPaginator,
 )
 from .type_defs import (
     BlobTypeDef,
-    CachePolicyConfigUnionTypeDef,
+    CachePolicyConfigTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
-    ContinuousDeploymentPolicyConfigUnionTypeDef,
+    ContinuousDeploymentPolicyConfigTypeDef,
     CopyDistributionResultTypeDef,
     CreateCachePolicyResultTypeDef,
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     CreateContinuousDeploymentPolicyResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDistributionWithTagsResultTypeDef,
     CreateFieldLevelEncryptionConfigResultTypeDef,
@@ -55,21 +55,21 @@
     CreatePublicKeyResultTypeDef,
     CreateRealtimeLogConfigResultTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     DescribeFunctionResultTypeDef,
     DescribeKeyValueStoreResultTypeDef,
-    DistributionConfigUnionTypeDef,
+    DistributionConfigTypeDef,
     DistributionConfigWithTagsTypeDef,
     EmptyResponseMetadataTypeDef,
     EndPointTypeDef,
-    FieldLevelEncryptionConfigUnionTypeDef,
-    FieldLevelEncryptionProfileConfigUnionTypeDef,
-    FunctionConfigUnionTypeDef,
+    FieldLevelEncryptionConfigTypeDef,
+    FieldLevelEncryptionProfileConfigTypeDef,
+    FunctionConfigTypeDef,
     GetCachePolicyConfigResultTypeDef,
     GetCachePolicyResultTypeDef,
     GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
     GetContinuousDeploymentPolicyResultTypeDef,
     GetDistributionConfigResultTypeDef,
@@ -91,16 +91,16 @@
     GetPublicKeyResultTypeDef,
     GetRealtimeLogConfigResultTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
     GetStreamingDistributionResultTypeDef,
     ImportSourceTypeDef,
-    InvalidationBatchUnionTypeDef,
-    KeyGroupConfigUnionTypeDef,
+    InvalidationBatchTypeDef,
+    KeyGroupConfigTypeDef,
     ListCachePoliciesResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
     ListDistributionsByOriginRequestPolicyIdResultTypeDef,
@@ -119,22 +119,22 @@
     ListPublicKeysResultTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
     ListStreamingDistributionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlConfigTypeDef,
-    OriginRequestPolicyConfigUnionTypeDef,
+    OriginRequestPolicyConfigTypeDef,
     PublicKeyConfigTypeDef,
     PublishFunctionResultTypeDef,
-    ResponseHeadersPolicyConfigUnionTypeDef,
-    StreamingDistributionConfigUnionTypeDef,
+    ResponseHeadersPolicyConfigTypeDef,
+    StreamingDistributionConfigTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagKeysTypeDef,
-    TagsUnionTypeDef,
+    TagsTypeDef,
     TestFunctionResultTypeDef,
     UpdateCachePolicyResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateContinuousDeploymentPolicyResultTypeDef,
     UpdateDistributionResultTypeDef,
     UpdateDistributionWithStagingConfigResultTypeDef,
     UpdateFieldLevelEncryptionConfigResultTypeDef,
@@ -383,15 +383,15 @@
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#copy_distribution)
         """
 
     def create_cache_policy(
-        self, *, CachePolicyConfig: CachePolicyConfigUnionTypeDef
+        self, *, CachePolicyConfig: CachePolicyConfigTypeDef
     ) -> CreateCachePolicyResultTypeDef:
         """
         Creates a cache policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_cache_policy)
         """
@@ -403,27 +403,27 @@
         Creates a new origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_cloud_front_origin_access_identity)
         """
 
     def create_continuous_deployment_policy(
-        self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef
+        self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef
     ) -> CreateContinuousDeploymentPolicyResultTypeDef:
         """
         Creates a continuous deployment policy that distributes traffic for a custom
         domain name to two different CloudFront
         distributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_continuous_deployment_policy)
         """
 
     def create_distribution(
-        self, *, DistributionConfig: DistributionConfigUnionTypeDef
+        self, *, DistributionConfig: DistributionConfigTypeDef
     ) -> CreateDistributionResultTypeDef:
         """
         Creates a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_distribution)
         """
@@ -435,55 +435,55 @@
         Create a new distribution with tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution_with_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_distribution_with_tags)
         """
 
     def create_field_level_encryption_config(
-        self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef
+        self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef
     ) -> CreateFieldLevelEncryptionConfigResultTypeDef:
         """
         Create a new field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_field_level_encryption_config)
         """
 
     def create_field_level_encryption_profile(
-        self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef
+        self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef
     ) -> CreateFieldLevelEncryptionProfileResultTypeDef:
         """
         Create a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_field_level_encryption_profile)
         """
 
     def create_function(
-        self, *, Name: str, FunctionConfig: FunctionConfigUnionTypeDef, FunctionCode: BlobTypeDef
+        self, *, Name: str, FunctionConfig: FunctionConfigTypeDef, FunctionCode: BlobTypeDef
     ) -> CreateFunctionResultTypeDef:
         """
         Creates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_function)
         """
 
     def create_invalidation(
-        self, *, DistributionId: str, InvalidationBatch: InvalidationBatchUnionTypeDef
+        self, *, DistributionId: str, InvalidationBatch: InvalidationBatchTypeDef
     ) -> CreateInvalidationResultTypeDef:
         """
         Create a new invalidation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_invalidation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_invalidation)
         """
 
     def create_key_group(
-        self, *, KeyGroupConfig: KeyGroupConfigUnionTypeDef
+        self, *, KeyGroupConfig: KeyGroupConfigTypeDef
     ) -> CreateKeyGroupResultTypeDef:
         """
         Creates a key group that you can use with [CloudFront signed URLs and signed
         cookies](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_key_group)
@@ -516,15 +516,15 @@
         Creates a new origin access control in CloudFront.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_origin_access_control)
         """
 
     def create_origin_request_policy(
-        self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef
+        self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef
     ) -> CreateOriginRequestPolicyResultTypeDef:
         """
         Creates an origin request policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_request_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_origin_request_policy)
         """
@@ -555,25 +555,25 @@
         Creates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_realtime_log_config)
         """
 
     def create_response_headers_policy(
-        self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef
+        self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef
     ) -> CreateResponseHeadersPolicyResultTypeDef:
         """
         Creates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_response_headers_policy)
         """
 
     def create_streaming_distribution(
-        self, *, StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef
+        self, *, StreamingDistributionConfig: StreamingDistributionConfigTypeDef
     ) -> CreateStreamingDistributionResultTypeDef:
         """
         This API is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_streaming_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_streaming_distribution)
         """
@@ -1300,17 +1300,15 @@
         `DEVELOPMENT` stage to
         `LIVE`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.publish_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#publish_function)
         """
 
-    def tag_resource(
-        self, *, Resource: str, Tags: TagsUnionTypeDef
-    ) -> EmptyResponseMetadataTypeDef:
+    def tag_resource(self, *, Resource: str, Tags: TagsTypeDef) -> EmptyResponseMetadataTypeDef:
         """
         Add tags to a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#tag_resource)
         """
 
@@ -1331,15 +1329,15 @@
         Remove tags from a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#untag_resource)
         """
 
     def update_cache_policy(
-        self, *, CachePolicyConfig: CachePolicyConfigUnionTypeDef, Id: str, IfMatch: str = ...
+        self, *, CachePolicyConfig: CachePolicyConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateCachePolicyResultTypeDef:
         """
         Updates a cache policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cache_policy)
         """
@@ -1357,27 +1355,27 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cloud_front_origin_access_identity)
         """
 
     def update_continuous_deployment_policy(
         self,
         *,
-        ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef,
+        ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...,
     ) -> UpdateContinuousDeploymentPolicyResultTypeDef:
         """
         Updates a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_continuous_deployment_policy)
         """
 
     def update_distribution(
-        self, *, DistributionConfig: DistributionConfigUnionTypeDef, Id: str, IfMatch: str = ...
+        self, *, DistributionConfig: DistributionConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates the configuration for a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_distribution)
         """
@@ -1392,29 +1390,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution_with_staging_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_distribution_with_staging_config)
         """
 
     def update_field_level_encryption_config(
         self,
         *,
-        FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef,
+        FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,
         Id: str,
         IfMatch: str = ...,
     ) -> UpdateFieldLevelEncryptionConfigResultTypeDef:
         """
         Update a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_field_level_encryption_config)
         """
 
     def update_field_level_encryption_profile(
         self,
         *,
-        FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef,
+        FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,
         Id: str,
         IfMatch: str = ...,
     ) -> UpdateFieldLevelEncryptionProfileResultTypeDef:
         """
         Update a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_profile)
@@ -1422,26 +1420,26 @@
         """
 
     def update_function(
         self,
         *,
         Name: str,
         IfMatch: str,
-        FunctionConfig: FunctionConfigUnionTypeDef,
+        FunctionConfig: FunctionConfigTypeDef,
         FunctionCode: BlobTypeDef,
     ) -> UpdateFunctionResultTypeDef:
         """
         Updates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_function)
         """
 
     def update_key_group(
-        self, *, KeyGroupConfig: KeyGroupConfigUnionTypeDef, Id: str, IfMatch: str = ...
+        self, *, KeyGroupConfig: KeyGroupConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateKeyGroupResultTypeDef:
         """
         Updates a key group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_key_group)
         """
@@ -1469,15 +1467,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_origin_access_control)
         """
 
     def update_origin_request_policy(
         self,
         *,
-        OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef,
+        OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...,
     ) -> UpdateOriginRequestPolicyResultTypeDef:
         """
         Updates an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_request_policy)
@@ -1509,29 +1507,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_realtime_log_config)
         """
 
     def update_response_headers_policy(
         self,
         *,
-        ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef,
+        ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...,
     ) -> UpdateResponseHeadersPolicyResultTypeDef:
         """
         Updates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_response_headers_policy)
         """
 
     def update_streaming_distribution(
         self,
         *,
-        StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef,
+        StreamingDistributionConfig: StreamingDistributionConfigTypeDef,
         Id: str,
         IfMatch: str = ...,
     ) -> UpdateStreamingDistributionResultTypeDef:
         """
         Update a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_streaming_distribution)
```

### Comparing `mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/client.pyi` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     ListDistributionsPaginator,
     ListInvalidationsPaginator,
     ListKeyValueStoresPaginator,
     ListStreamingDistributionsPaginator,
 )
 from .type_defs import (
     BlobTypeDef,
-    CachePolicyConfigUnionTypeDef,
+    CachePolicyConfigTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
-    ContinuousDeploymentPolicyConfigUnionTypeDef,
+    ContinuousDeploymentPolicyConfigTypeDef,
     CopyDistributionResultTypeDef,
     CreateCachePolicyResultTypeDef,
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     CreateContinuousDeploymentPolicyResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDistributionWithTagsResultTypeDef,
     CreateFieldLevelEncryptionConfigResultTypeDef,
@@ -55,21 +55,21 @@
     CreatePublicKeyResultTypeDef,
     CreateRealtimeLogConfigResultTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     DescribeFunctionResultTypeDef,
     DescribeKeyValueStoreResultTypeDef,
-    DistributionConfigUnionTypeDef,
+    DistributionConfigTypeDef,
     DistributionConfigWithTagsTypeDef,
     EmptyResponseMetadataTypeDef,
     EndPointTypeDef,
-    FieldLevelEncryptionConfigUnionTypeDef,
-    FieldLevelEncryptionProfileConfigUnionTypeDef,
-    FunctionConfigUnionTypeDef,
+    FieldLevelEncryptionConfigTypeDef,
+    FieldLevelEncryptionProfileConfigTypeDef,
+    FunctionConfigTypeDef,
     GetCachePolicyConfigResultTypeDef,
     GetCachePolicyResultTypeDef,
     GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
     GetContinuousDeploymentPolicyResultTypeDef,
     GetDistributionConfigResultTypeDef,
@@ -91,16 +91,16 @@
     GetPublicKeyResultTypeDef,
     GetRealtimeLogConfigResultTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
     GetStreamingDistributionResultTypeDef,
     ImportSourceTypeDef,
-    InvalidationBatchUnionTypeDef,
-    KeyGroupConfigUnionTypeDef,
+    InvalidationBatchTypeDef,
+    KeyGroupConfigTypeDef,
     ListCachePoliciesResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
     ListDistributionsByOriginRequestPolicyIdResultTypeDef,
@@ -119,22 +119,22 @@
     ListPublicKeysResultTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
     ListStreamingDistributionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlConfigTypeDef,
-    OriginRequestPolicyConfigUnionTypeDef,
+    OriginRequestPolicyConfigTypeDef,
     PublicKeyConfigTypeDef,
     PublishFunctionResultTypeDef,
-    ResponseHeadersPolicyConfigUnionTypeDef,
-    StreamingDistributionConfigUnionTypeDef,
+    ResponseHeadersPolicyConfigTypeDef,
+    StreamingDistributionConfigTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagKeysTypeDef,
-    TagsUnionTypeDef,
+    TagsTypeDef,
     TestFunctionResultTypeDef,
     UpdateCachePolicyResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateContinuousDeploymentPolicyResultTypeDef,
     UpdateDistributionResultTypeDef,
     UpdateDistributionWithStagingConfigResultTypeDef,
     UpdateFieldLevelEncryptionConfigResultTypeDef,
@@ -380,15 +380,15 @@
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#copy_distribution)
         """
 
     def create_cache_policy(
-        self, *, CachePolicyConfig: CachePolicyConfigUnionTypeDef
+        self, *, CachePolicyConfig: CachePolicyConfigTypeDef
     ) -> CreateCachePolicyResultTypeDef:
         """
         Creates a cache policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_cache_policy)
         """
@@ -400,27 +400,27 @@
         Creates a new origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_cloud_front_origin_access_identity)
         """
 
     def create_continuous_deployment_policy(
-        self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef
+        self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef
     ) -> CreateContinuousDeploymentPolicyResultTypeDef:
         """
         Creates a continuous deployment policy that distributes traffic for a custom
         domain name to two different CloudFront
         distributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_continuous_deployment_policy)
         """
 
     def create_distribution(
-        self, *, DistributionConfig: DistributionConfigUnionTypeDef
+        self, *, DistributionConfig: DistributionConfigTypeDef
     ) -> CreateDistributionResultTypeDef:
         """
         Creates a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_distribution)
         """
@@ -432,55 +432,55 @@
         Create a new distribution with tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution_with_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_distribution_with_tags)
         """
 
     def create_field_level_encryption_config(
-        self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef
+        self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef
     ) -> CreateFieldLevelEncryptionConfigResultTypeDef:
         """
         Create a new field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_field_level_encryption_config)
         """
 
     def create_field_level_encryption_profile(
-        self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef
+        self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef
     ) -> CreateFieldLevelEncryptionProfileResultTypeDef:
         """
         Create a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_field_level_encryption_profile)
         """
 
     def create_function(
-        self, *, Name: str, FunctionConfig: FunctionConfigUnionTypeDef, FunctionCode: BlobTypeDef
+        self, *, Name: str, FunctionConfig: FunctionConfigTypeDef, FunctionCode: BlobTypeDef
     ) -> CreateFunctionResultTypeDef:
         """
         Creates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_function)
         """
 
     def create_invalidation(
-        self, *, DistributionId: str, InvalidationBatch: InvalidationBatchUnionTypeDef
+        self, *, DistributionId: str, InvalidationBatch: InvalidationBatchTypeDef
     ) -> CreateInvalidationResultTypeDef:
         """
         Create a new invalidation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_invalidation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_invalidation)
         """
 
     def create_key_group(
-        self, *, KeyGroupConfig: KeyGroupConfigUnionTypeDef
+        self, *, KeyGroupConfig: KeyGroupConfigTypeDef
     ) -> CreateKeyGroupResultTypeDef:
         """
         Creates a key group that you can use with [CloudFront signed URLs and signed
         cookies](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_key_group)
@@ -513,15 +513,15 @@
         Creates a new origin access control in CloudFront.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_origin_access_control)
         """
 
     def create_origin_request_policy(
-        self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef
+        self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef
     ) -> CreateOriginRequestPolicyResultTypeDef:
         """
         Creates an origin request policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_request_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_origin_request_policy)
         """
@@ -552,25 +552,25 @@
         Creates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_realtime_log_config)
         """
 
     def create_response_headers_policy(
-        self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef
+        self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef
     ) -> CreateResponseHeadersPolicyResultTypeDef:
         """
         Creates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_response_headers_policy)
         """
 
     def create_streaming_distribution(
-        self, *, StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef
+        self, *, StreamingDistributionConfig: StreamingDistributionConfigTypeDef
     ) -> CreateStreamingDistributionResultTypeDef:
         """
         This API is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_streaming_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_streaming_distribution)
         """
@@ -1297,17 +1297,15 @@
         `DEVELOPMENT` stage to
         `LIVE`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.publish_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#publish_function)
         """
 
-    def tag_resource(
-        self, *, Resource: str, Tags: TagsUnionTypeDef
-    ) -> EmptyResponseMetadataTypeDef:
+    def tag_resource(self, *, Resource: str, Tags: TagsTypeDef) -> EmptyResponseMetadataTypeDef:
         """
         Add tags to a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#tag_resource)
         """
 
@@ -1328,15 +1326,15 @@
         Remove tags from a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#untag_resource)
         """
 
     def update_cache_policy(
-        self, *, CachePolicyConfig: CachePolicyConfigUnionTypeDef, Id: str, IfMatch: str = ...
+        self, *, CachePolicyConfig: CachePolicyConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateCachePolicyResultTypeDef:
         """
         Updates a cache policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cache_policy)
         """
@@ -1354,27 +1352,27 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cloud_front_origin_access_identity)
         """
 
     def update_continuous_deployment_policy(
         self,
         *,
-        ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef,
+        ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...,
     ) -> UpdateContinuousDeploymentPolicyResultTypeDef:
         """
         Updates a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_continuous_deployment_policy)
         """
 
     def update_distribution(
-        self, *, DistributionConfig: DistributionConfigUnionTypeDef, Id: str, IfMatch: str = ...
+        self, *, DistributionConfig: DistributionConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates the configuration for a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_distribution)
         """
@@ -1389,29 +1387,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution_with_staging_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_distribution_with_staging_config)
         """
 
     def update_field_level_encryption_config(
         self,
         *,
-        FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef,
+        FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,
         Id: str,
         IfMatch: str = ...,
     ) -> UpdateFieldLevelEncryptionConfigResultTypeDef:
         """
         Update a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_field_level_encryption_config)
         """
 
     def update_field_level_encryption_profile(
         self,
         *,
-        FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef,
+        FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,
         Id: str,
         IfMatch: str = ...,
     ) -> UpdateFieldLevelEncryptionProfileResultTypeDef:
         """
         Update a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_profile)
@@ -1419,26 +1417,26 @@
         """
 
     def update_function(
         self,
         *,
         Name: str,
         IfMatch: str,
-        FunctionConfig: FunctionConfigUnionTypeDef,
+        FunctionConfig: FunctionConfigTypeDef,
         FunctionCode: BlobTypeDef,
     ) -> UpdateFunctionResultTypeDef:
         """
         Updates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_function)
         """
 
     def update_key_group(
-        self, *, KeyGroupConfig: KeyGroupConfigUnionTypeDef, Id: str, IfMatch: str = ...
+        self, *, KeyGroupConfig: KeyGroupConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateKeyGroupResultTypeDef:
         """
         Updates a key group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_key_group)
         """
@@ -1466,15 +1464,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_origin_access_control)
         """
 
     def update_origin_request_policy(
         self,
         *,
-        OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef,
+        OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...,
     ) -> UpdateOriginRequestPolicyResultTypeDef:
         """
         Updates an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_request_policy)
@@ -1506,29 +1504,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_realtime_log_config)
         """
 
     def update_response_headers_policy(
         self,
         *,
-        ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef,
+        ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...,
     ) -> UpdateResponseHeadersPolicyResultTypeDef:
         """
         Updates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_response_headers_policy)
         """
 
     def update_streaming_distribution(
         self,
         *,
-        StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef,
+        StreamingDistributionConfig: StreamingDistributionConfigTypeDef,
         Id: str,
         IfMatch: str = ...,
     ) -> UpdateStreamingDistributionResultTypeDef:
         """
         Update a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_streaming_distribution)
```

### Comparing `mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/literals.py` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,14 @@
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
-    "mailmanager",
     "managedblockchain",
     "managedblockchain-query",
     "marketplace-agreement",
     "marketplace-catalog",
     "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
@@ -434,15 +433,14 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
-    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/literals.pyi` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,14 @@
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
-    "mailmanager",
     "managedblockchain",
     "managedblockchain-query",
     "marketplace-agreement",
     "marketplace-catalog",
     "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
@@ -434,15 +433,14 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
-    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/paginator.py` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/paginator.pyi` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/type_defs.py` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/type_defs.py`

 * *Files 25% similar despite different names*

```diff
@@ -63,48 +63,39 @@
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AliasICPRecordalTypeDef",
-    "AliasesOutputTypeDef",
     "AliasesTypeDef",
-    "CachedMethodsOutputTypeDef",
     "CachedMethodsTypeDef",
     "AssociateAliasRequestRequestTypeDef",
     "BlobTypeDef",
-    "TrustedKeyGroupsOutputTypeDef",
-    "TrustedSignersOutputTypeDef",
     "TrustedKeyGroupsTypeDef",
     "TrustedSignersTypeDef",
-    "CookieNamesOutputTypeDef",
     "CookieNamesTypeDef",
-    "HeadersOutputTypeDef",
     "HeadersTypeDef",
-    "QueryStringNamesOutputTypeDef",
     "QueryStringNamesTypeDef",
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     "CloudFrontOriginAccessIdentitySummaryTypeDef",
     "ConflictingAliasTypeDef",
     "ContentTypeProfileTypeDef",
-    "StagingDistributionDnsNamesOutputTypeDef",
     "StagingDistributionDnsNamesTypeDef",
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
     "SessionStickinessConfigTypeDef",
     "CopyDistributionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "KeyGroupConfigTypeDef",
     "ImportSourceTypeDef",
     "KeyValueStoreTypeDef",
     "OriginAccessControlConfigTypeDef",
     "PublicKeyConfigTypeDef",
     "CustomErrorResponseTypeDef",
     "OriginCustomHeaderTypeDef",
-    "OriginSslProtocolsOutputTypeDef",
     "OriginSslProtocolsTypeDef",
     "DeleteCachePolicyRequestRequestTypeDef",
     "DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "DeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     "DeleteDistributionRequestRequestTypeDef",
     "DeleteFieldLevelEncryptionConfigRequestRequestTypeDef",
     "DeleteFieldLevelEncryptionProfileRequestRequestTypeDef",
@@ -119,22 +110,19 @@
     "DeleteResponseHeadersPolicyRequestRequestTypeDef",
     "DeleteStreamingDistributionRequestRequestTypeDef",
     "DescribeFunctionRequestRequestTypeDef",
     "DescribeKeyValueStoreRequestRequestTypeDef",
     "LoggingConfigTypeDef",
     "ViewerCertificateTypeDef",
     "DistributionIdListTypeDef",
-    "FieldPatternsOutputTypeDef",
     "FieldPatternsTypeDef",
     "KinesisStreamConfigTypeDef",
-    "QueryStringCacheKeysOutputTypeDef",
     "QueryStringCacheKeysTypeDef",
     "FunctionAssociationTypeDef",
     "FunctionMetadataTypeDef",
-    "GeoRestrictionOutputTypeDef",
     "GeoRestrictionTypeDef",
     "GetCachePolicyConfigRequestRequestTypeDef",
     "GetCachePolicyRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyConfigRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyRequestRequestTypeDef",
@@ -144,29 +132,27 @@
     "GetFieldLevelEncryptionConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileRequestRequestTypeDef",
     "GetFieldLevelEncryptionRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
     "GetInvalidationRequestRequestTypeDef",
     "GetKeyGroupConfigRequestRequestTypeDef",
-    "KeyGroupConfigOutputTypeDef",
     "GetKeyGroupRequestRequestTypeDef",
     "GetMonitoringSubscriptionRequestRequestTypeDef",
     "GetOriginAccessControlConfigRequestRequestTypeDef",
     "GetOriginAccessControlRequestRequestTypeDef",
     "GetOriginRequestPolicyConfigRequestRequestTypeDef",
     "GetOriginRequestPolicyRequestRequestTypeDef",
     "GetPublicKeyConfigRequestRequestTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
     "GetRealtimeLogConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyRequestRequestTypeDef",
     "GetStreamingDistributionConfigRequestRequestTypeDef",
     "GetStreamingDistributionRequestRequestTypeDef",
-    "PathsOutputTypeDef",
     "PathsTypeDef",
     "InvalidationSummaryTypeDef",
     "KeyPairIdsTypeDef",
     "KeyValueStoreAssociationTypeDef",
     "LambdaFunctionAssociationTypeDef",
     "ListCachePoliciesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -191,29 +177,24 @@
     "ListPublicKeysRequestRequestTypeDef",
     "ListRealtimeLogConfigsRequestRequestTypeDef",
     "ListResponseHeadersPoliciesRequestRequestTypeDef",
     "ListStreamingDistributionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RealtimeMetricsSubscriptionConfigTypeDef",
     "OriginAccessControlSummaryTypeDef",
-    "StatusCodesOutputTypeDef",
     "StatusCodesTypeDef",
     "OriginGroupMemberTypeDef",
     "OriginShieldTypeDef",
     "S3OriginConfigTypeDef",
     "PublicKeySummaryTypeDef",
     "PublishFunctionRequestRequestTypeDef",
     "QueryArgProfileTypeDef",
-    "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
-    "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
-    "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
-    "ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     "ResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
     "ResponseHeadersPolicyContentTypeOptionsTypeDef",
     "ResponseHeadersPolicyCustomHeaderTypeDef",
     "ResponseHeadersPolicyFrameOptionsTypeDef",
     "ResponseHeadersPolicyReferrerPolicyTypeDef",
@@ -222,265 +203,208 @@
     "ResponseHeadersPolicyXSSProtectionTypeDef",
     "S3OriginTypeDef",
     "StreamingLoggingConfigTypeDef",
     "TagKeysTypeDef",
     "TagTypeDef",
     "UpdateDistributionWithStagingConfigRequestRequestTypeDef",
     "UpdateKeyValueStoreRequestRequestTypeDef",
-    "AllowedMethodsOutputTypeDef",
     "AllowedMethodsTypeDef",
     "TestFunctionRequestRequestTypeDef",
-    "CachePolicyCookiesConfigOutputTypeDef",
-    "CookiePreferenceOutputTypeDef",
-    "OriginRequestPolicyCookiesConfigOutputTypeDef",
     "CachePolicyCookiesConfigTypeDef",
     "CookiePreferenceTypeDef",
     "OriginRequestPolicyCookiesConfigTypeDef",
-    "CachePolicyHeadersConfigOutputTypeDef",
-    "OriginRequestPolicyHeadersConfigOutputTypeDef",
     "CachePolicyHeadersConfigTypeDef",
     "OriginRequestPolicyHeadersConfigTypeDef",
-    "CachePolicyQueryStringsConfigOutputTypeDef",
-    "OriginRequestPolicyQueryStringsConfigOutputTypeDef",
     "CachePolicyQueryStringsConfigTypeDef",
     "OriginRequestPolicyQueryStringsConfigTypeDef",
     "CloudFrontOriginAccessIdentityTypeDef",
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "CloudFrontOriginAccessIdentityListTypeDef",
     "ConflictingAliasesListTypeDef",
-    "ContentTypeProfilesOutputTypeDef",
     "ContentTypeProfilesTypeDef",
     "ContinuousDeploymentSingleWeightConfigTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
     "GetFunctionResultTypeDef",
     "CreateKeyGroupRequestRequestTypeDef",
+    "GetKeyGroupConfigResultTypeDef",
+    "KeyGroupTypeDef",
     "UpdateKeyGroupRequestRequestTypeDef",
     "CreateKeyValueStoreRequestRequestTypeDef",
     "CreateKeyValueStoreResultTypeDef",
     "DescribeKeyValueStoreResultTypeDef",
     "KeyValueStoreListTypeDef",
     "UpdateKeyValueStoreResultTypeDef",
     "CreateOriginAccessControlRequestRequestTypeDef",
     "GetOriginAccessControlConfigResultTypeDef",
     "OriginAccessControlTypeDef",
     "UpdateOriginAccessControlRequestRequestTypeDef",
     "CreatePublicKeyRequestRequestTypeDef",
     "GetPublicKeyConfigResultTypeDef",
     "PublicKeyTypeDef",
     "UpdatePublicKeyRequestRequestTypeDef",
-    "CustomErrorResponsesOutputTypeDef",
     "CustomErrorResponsesTypeDef",
-    "CustomHeadersOutputTypeDef",
     "CustomHeadersTypeDef",
-    "CustomOriginConfigOutputTypeDef",
     "CustomOriginConfigTypeDef",
     "ListDistributionsByCachePolicyIdResultTypeDef",
     "ListDistributionsByKeyGroupResultTypeDef",
     "ListDistributionsByOriginRequestPolicyIdResultTypeDef",
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
-    "EncryptionEntityOutputTypeDef",
     "EncryptionEntityTypeDef",
     "EndPointTypeDef",
-    "FunctionAssociationsOutputTypeDef",
     "FunctionAssociationsTypeDef",
-    "RestrictionsOutputTypeDef",
     "RestrictionsTypeDef",
     "GetDistributionRequestDistributionDeployedWaitTypeDef",
     "GetInvalidationRequestInvalidationCompletedWaitTypeDef",
     "GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
-    "GetKeyGroupConfigResultTypeDef",
-    "KeyGroupConfigUnionTypeDef",
-    "KeyGroupTypeDef",
-    "InvalidationBatchOutputTypeDef",
     "InvalidationBatchTypeDef",
     "InvalidationListTypeDef",
     "KGKeyPairIdsTypeDef",
     "SignerTypeDef",
-    "KeyValueStoreAssociationsOutputTypeDef",
     "KeyValueStoreAssociationsTypeDef",
-    "LambdaFunctionAssociationsOutputTypeDef",
     "LambdaFunctionAssociationsTypeDef",
     "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
     "ListDistributionsRequestListDistributionsPaginateTypeDef",
     "ListInvalidationsRequestListInvalidationsPaginateTypeDef",
     "ListKeyValueStoresRequestListKeyValueStoresPaginateTypeDef",
     "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "MonitoringSubscriptionTypeDef",
     "OriginAccessControlListTypeDef",
-    "OriginGroupFailoverCriteriaOutputTypeDef",
     "OriginGroupFailoverCriteriaTypeDef",
-    "OriginGroupMembersOutputTypeDef",
     "OriginGroupMembersTypeDef",
     "PublicKeyListTypeDef",
-    "QueryArgProfilesOutputTypeDef",
     "QueryArgProfilesTypeDef",
-    "ResponseHeadersPolicyCorsConfigOutputTypeDef",
     "ResponseHeadersPolicyCorsConfigTypeDef",
-    "ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyCustomHeadersConfigTypeDef",
-    "ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     "StreamingDistributionSummaryTypeDef",
-    "StreamingDistributionConfigOutputTypeDef",
     "StreamingDistributionConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "TagsOutputTypeDef",
     "TagsTypeDef",
-    "ForwardedValuesOutputTypeDef",
     "ForwardedValuesTypeDef",
-    "ParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
-    "OriginRequestPolicyConfigOutputTypeDef",
     "ParametersInCacheKeyAndForwardedToOriginTypeDef",
     "OriginRequestPolicyConfigTypeDef",
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     "GetCloudFrontOriginAccessIdentityResultTypeDef",
     "UpdateCloudFrontOriginAccessIdentityResultTypeDef",
     "ListCloudFrontOriginAccessIdentitiesResultTypeDef",
     "ListConflictingAliasesResultTypeDef",
-    "ContentTypeProfileConfigOutputTypeDef",
     "ContentTypeProfileConfigTypeDef",
     "TrafficConfigTypeDef",
+    "CreateKeyGroupResultTypeDef",
+    "GetKeyGroupResultTypeDef",
+    "KeyGroupSummaryTypeDef",
+    "UpdateKeyGroupResultTypeDef",
     "ListKeyValueStoresResultTypeDef",
     "CreateOriginAccessControlResultTypeDef",
     "GetOriginAccessControlResultTypeDef",
     "UpdateOriginAccessControlResultTypeDef",
     "CreatePublicKeyResultTypeDef",
     "GetPublicKeyResultTypeDef",
     "UpdatePublicKeyResultTypeDef",
-    "OriginOutputTypeDef",
     "OriginTypeDef",
-    "EncryptionEntitiesOutputTypeDef",
     "EncryptionEntitiesTypeDef",
     "CreateRealtimeLogConfigRequestRequestTypeDef",
     "RealtimeLogConfigTypeDef",
     "UpdateRealtimeLogConfigRequestRequestTypeDef",
-    "CreateKeyGroupResultTypeDef",
-    "GetKeyGroupResultTypeDef",
-    "KeyGroupSummaryTypeDef",
-    "UpdateKeyGroupResultTypeDef",
-    "InvalidationTypeDef",
     "CreateInvalidationRequestRequestTypeDef",
-    "InvalidationBatchUnionTypeDef",
+    "InvalidationTypeDef",
     "ListInvalidationsResultTypeDef",
     "ActiveTrustedKeyGroupsTypeDef",
     "ActiveTrustedSignersTypeDef",
-    "FunctionConfigOutputTypeDef",
     "FunctionConfigTypeDef",
     "CreateMonitoringSubscriptionRequestRequestTypeDef",
     "CreateMonitoringSubscriptionResultTypeDef",
     "GetMonitoringSubscriptionResultTypeDef",
     "ListOriginAccessControlsResultTypeDef",
-    "OriginGroupOutputTypeDef",
     "OriginGroupTypeDef",
     "ListPublicKeysResultTypeDef",
-    "QueryArgProfileConfigOutputTypeDef",
     "QueryArgProfileConfigTypeDef",
-    "ResponseHeadersPolicyConfigOutputTypeDef",
     "ResponseHeadersPolicyConfigTypeDef",
     "StreamingDistributionListTypeDef",
-    "GetStreamingDistributionConfigResultTypeDef",
     "CreateStreamingDistributionRequestRequestTypeDef",
-    "StreamingDistributionConfigUnionTypeDef",
+    "GetStreamingDistributionConfigResultTypeDef",
     "UpdateStreamingDistributionRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "StreamingDistributionConfigWithTagsTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TagsUnionTypeDef",
-    "CacheBehaviorOutputTypeDef",
-    "DefaultCacheBehaviorOutputTypeDef",
     "CacheBehaviorTypeDef",
     "DefaultCacheBehaviorTypeDef",
-    "CachePolicyConfigOutputTypeDef",
-    "GetOriginRequestPolicyConfigResultTypeDef",
-    "OriginRequestPolicyTypeDef",
     "CachePolicyConfigTypeDef",
     "CreateOriginRequestPolicyRequestRequestTypeDef",
-    "OriginRequestPolicyConfigUnionTypeDef",
+    "GetOriginRequestPolicyConfigResultTypeDef",
+    "OriginRequestPolicyTypeDef",
     "UpdateOriginRequestPolicyRequestRequestTypeDef",
-    "ContinuousDeploymentPolicyConfigOutputTypeDef",
     "ContinuousDeploymentPolicyConfigTypeDef",
-    "OriginsOutputTypeDef",
+    "KeyGroupListTypeDef",
     "OriginsTypeDef",
-    "FieldLevelEncryptionProfileConfigOutputTypeDef",
-    "FieldLevelEncryptionProfileSummaryTypeDef",
     "FieldLevelEncryptionProfileConfigTypeDef",
+    "FieldLevelEncryptionProfileSummaryTypeDef",
     "CreateRealtimeLogConfigResultTypeDef",
     "GetRealtimeLogConfigResultTypeDef",
     "RealtimeLogConfigsTypeDef",
     "UpdateRealtimeLogConfigResultTypeDef",
-    "KeyGroupListTypeDef",
     "CreateInvalidationResultTypeDef",
     "GetInvalidationResultTypeDef",
     "StreamingDistributionTypeDef",
-    "FunctionSummaryTypeDef",
     "CreateFunctionRequestRequestTypeDef",
-    "FunctionConfigUnionTypeDef",
+    "FunctionSummaryTypeDef",
     "UpdateFunctionRequestRequestTypeDef",
-    "OriginGroupsOutputTypeDef",
     "OriginGroupsTypeDef",
-    "FieldLevelEncryptionConfigOutputTypeDef",
-    "FieldLevelEncryptionSummaryTypeDef",
     "FieldLevelEncryptionConfigTypeDef",
+    "FieldLevelEncryptionSummaryTypeDef",
+    "CreateResponseHeadersPolicyRequestRequestTypeDef",
     "GetResponseHeadersPolicyConfigResultTypeDef",
     "ResponseHeadersPolicyTypeDef",
-    "CreateResponseHeadersPolicyRequestRequestTypeDef",
-    "ResponseHeadersPolicyConfigUnionTypeDef",
     "UpdateResponseHeadersPolicyRequestRequestTypeDef",
     "ListStreamingDistributionsResultTypeDef",
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
-    "CacheBehaviorsOutputTypeDef",
     "CacheBehaviorsTypeDef",
     "CachePolicyTypeDef",
+    "CreateCachePolicyRequestRequestTypeDef",
     "GetCachePolicyConfigResultTypeDef",
+    "UpdateCachePolicyRequestRequestTypeDef",
     "CreateOriginRequestPolicyResultTypeDef",
     "GetOriginRequestPolicyResultTypeDef",
     "OriginRequestPolicySummaryTypeDef",
     "UpdateOriginRequestPolicyResultTypeDef",
-    "CachePolicyConfigUnionTypeDef",
-    "CreateCachePolicyRequestRequestTypeDef",
-    "UpdateCachePolicyRequestRequestTypeDef",
     "ContinuousDeploymentPolicyTypeDef",
-    "GetContinuousDeploymentPolicyConfigResultTypeDef",
-    "ContinuousDeploymentPolicyConfigUnionTypeDef",
     "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
+    "GetContinuousDeploymentPolicyConfigResultTypeDef",
     "UpdateContinuousDeploymentPolicyRequestRequestTypeDef",
+    "ListKeyGroupsResultTypeDef",
+    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "FieldLevelEncryptionProfileTypeDef",
     "GetFieldLevelEncryptionProfileConfigResultTypeDef",
-    "FieldLevelEncryptionProfileListTypeDef",
-    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
-    "FieldLevelEncryptionProfileConfigUnionTypeDef",
     "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
+    "FieldLevelEncryptionProfileListTypeDef",
     "ListRealtimeLogConfigsResultTypeDef",
-    "ListKeyGroupsResultTypeDef",
     "CreateStreamingDistributionResultTypeDef",
     "CreateStreamingDistributionWithTagsResultTypeDef",
     "GetStreamingDistributionResultTypeDef",
     "UpdateStreamingDistributionResultTypeDef",
     "CreateFunctionResultTypeDef",
     "DescribeFunctionResultTypeDef",
     "FunctionListTypeDef",
     "PublishFunctionResultTypeDef",
     "TestResultTypeDef",
     "UpdateFunctionResultTypeDef",
+    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "FieldLevelEncryptionTypeDef",
     "GetFieldLevelEncryptionConfigResultTypeDef",
-    "FieldLevelEncryptionListTypeDef",
-    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
-    "FieldLevelEncryptionConfigUnionTypeDef",
     "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    "FieldLevelEncryptionListTypeDef",
     "CreateResponseHeadersPolicyResultTypeDef",
     "GetResponseHeadersPolicyResultTypeDef",
     "ResponseHeadersPolicySummaryTypeDef",
     "UpdateResponseHeadersPolicyResultTypeDef",
-    "DistributionConfigOutputTypeDef",
-    "DistributionSummaryTypeDef",
     "DistributionConfigTypeDef",
+    "DistributionSummaryTypeDef",
     "CachePolicySummaryTypeDef",
     "CreateCachePolicyResultTypeDef",
     "GetCachePolicyResultTypeDef",
     "UpdateCachePolicyResultTypeDef",
     "OriginRequestPolicyListTypeDef",
     "ContinuousDeploymentPolicySummaryTypeDef",
     "CreateContinuousDeploymentPolicyResultTypeDef",
@@ -493,146 +417,94 @@
     "ListFunctionsResultTypeDef",
     "TestFunctionResultTypeDef",
     "CreateFieldLevelEncryptionConfigResultTypeDef",
     "GetFieldLevelEncryptionResultTypeDef",
     "UpdateFieldLevelEncryptionConfigResultTypeDef",
     "ListFieldLevelEncryptionConfigsResultTypeDef",
     "ResponseHeadersPolicyListTypeDef",
-    "DistributionTypeDef",
-    "GetDistributionConfigResultTypeDef",
-    "DistributionListTypeDef",
     "CreateDistributionRequestRequestTypeDef",
-    "DistributionConfigUnionTypeDef",
     "DistributionConfigWithTagsTypeDef",
+    "DistributionTypeDef",
+    "GetDistributionConfigResultTypeDef",
     "UpdateDistributionRequestRequestTypeDef",
+    "DistributionListTypeDef",
     "CachePolicyListTypeDef",
     "ListOriginRequestPoliciesResultTypeDef",
     "ContinuousDeploymentPolicyListTypeDef",
     "ListResponseHeadersPoliciesResultTypeDef",
+    "CreateDistributionWithTagsRequestRequestTypeDef",
     "CopyDistributionResultTypeDef",
     "CreateDistributionResultTypeDef",
     "CreateDistributionWithTagsResultTypeDef",
     "GetDistributionResultTypeDef",
     "UpdateDistributionResultTypeDef",
     "UpdateDistributionWithStagingConfigResultTypeDef",
     "ListDistributionsByRealtimeLogConfigResultTypeDef",
     "ListDistributionsByWebACLIdResultTypeDef",
     "ListDistributionsResultTypeDef",
-    "CreateDistributionWithTagsRequestRequestTypeDef",
     "ListCachePoliciesResultTypeDef",
     "ListContinuousDeploymentPoliciesResultTypeDef",
 )
 
 AliasICPRecordalTypeDef = TypedDict(
     "AliasICPRecordalTypeDef",
     {
         "CNAME": NotRequired[str],
         "ICPRecordalStatus": NotRequired[ICPRecordalStatusType],
     },
 )
-AliasesOutputTypeDef = TypedDict(
-    "AliasesOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
 AliasesTypeDef = TypedDict(
     "AliasesTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[str]],
-    },
-)
-CachedMethodsOutputTypeDef = TypedDict(
-    "CachedMethodsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[MethodType],
+        "Items": NotRequired[List[str]],
     },
 )
 CachedMethodsTypeDef = TypedDict(
     "CachedMethodsTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[MethodType],
+        "Items": List[MethodType],
     },
 )
 AssociateAliasRequestRequestTypeDef = TypedDict(
     "AssociateAliasRequestRequestTypeDef",
     {
         "TargetDistributionId": str,
         "Alias": str,
     },
 )
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
-TrustedKeyGroupsOutputTypeDef = TypedDict(
-    "TrustedKeyGroupsOutputTypeDef",
-    {
-        "Enabled": bool,
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
-TrustedSignersOutputTypeDef = TypedDict(
-    "TrustedSignersOutputTypeDef",
-    {
-        "Enabled": bool,
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
 TrustedKeyGroupsTypeDef = TypedDict(
     "TrustedKeyGroupsTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
-        "Items": NotRequired[Sequence[str]],
+        "Items": NotRequired[List[str]],
     },
 )
 TrustedSignersTypeDef = TypedDict(
     "TrustedSignersTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
-        "Items": NotRequired[Sequence[str]],
-    },
-)
-CookieNamesOutputTypeDef = TypedDict(
-    "CookieNamesOutputTypeDef",
-    {
-        "Quantity": int,
         "Items": NotRequired[List[str]],
     },
 )
 CookieNamesTypeDef = TypedDict(
     "CookieNamesTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[str]],
-    },
-)
-HeadersOutputTypeDef = TypedDict(
-    "HeadersOutputTypeDef",
-    {
-        "Quantity": int,
         "Items": NotRequired[List[str]],
     },
 )
 HeadersTypeDef = TypedDict(
     "HeadersTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[str]],
-    },
-)
-QueryStringNamesOutputTypeDef = TypedDict(
-    "QueryStringNamesOutputTypeDef",
-    {
-        "Quantity": int,
         "Items": NotRequired[List[str]],
     },
 )
 QueryStringNamesTypeDef = TypedDict(
     "QueryStringNamesTypeDef",
     {
         "Quantity": int,
@@ -666,21 +538,14 @@
     "ContentTypeProfileTypeDef",
     {
         "Format": Literal["URLEncoded"],
         "ContentType": str,
         "ProfileId": NotRequired[str],
     },
 )
-StagingDistributionDnsNamesOutputTypeDef = TypedDict(
-    "StagingDistributionDnsNamesOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
 StagingDistributionDnsNamesTypeDef = TypedDict(
     "StagingDistributionDnsNamesTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[str]],
     },
 )
@@ -775,26 +640,19 @@
 OriginCustomHeaderTypeDef = TypedDict(
     "OriginCustomHeaderTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
-OriginSslProtocolsOutputTypeDef = TypedDict(
-    "OriginSslProtocolsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[SslProtocolType],
-    },
-)
 OriginSslProtocolsTypeDef = TypedDict(
     "OriginSslProtocolsTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[SslProtocolType],
+        "Items": List[SslProtocolType],
     },
 )
 DeleteCachePolicyRequestRequestTypeDef = TypedDict(
     "DeleteCachePolicyRequestRequestTypeDef",
     {
         "Id": str,
         "IfMatch": NotRequired[str],
@@ -945,47 +803,33 @@
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[str]],
     },
 )
-FieldPatternsOutputTypeDef = TypedDict(
-    "FieldPatternsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
 FieldPatternsTypeDef = TypedDict(
     "FieldPatternsTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[str]],
     },
 )
 KinesisStreamConfigTypeDef = TypedDict(
     "KinesisStreamConfigTypeDef",
     {
         "RoleARN": str,
         "StreamARN": str,
     },
 )
-QueryStringCacheKeysOutputTypeDef = TypedDict(
-    "QueryStringCacheKeysOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
 QueryStringCacheKeysTypeDef = TypedDict(
     "QueryStringCacheKeysTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[str]],
+        "Items": NotRequired[List[str]],
     },
 )
 FunctionAssociationTypeDef = TypedDict(
     "FunctionAssociationTypeDef",
     {
         "FunctionARN": str,
         "EventType": EventTypeType,
@@ -996,28 +840,20 @@
     {
         "FunctionARN": str,
         "LastModifiedTime": datetime,
         "Stage": NotRequired[FunctionStageType],
         "CreatedTime": NotRequired[datetime],
     },
 )
-GeoRestrictionOutputTypeDef = TypedDict(
-    "GeoRestrictionOutputTypeDef",
-    {
-        "RestrictionType": GeoRestrictionTypeType,
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
 GeoRestrictionTypeDef = TypedDict(
     "GeoRestrictionTypeDef",
     {
         "RestrictionType": GeoRestrictionTypeType,
         "Quantity": int,
-        "Items": NotRequired[Sequence[str]],
+        "Items": NotRequired[List[str]],
     },
 )
 GetCachePolicyConfigRequestRequestTypeDef = TypedDict(
     "GetCachePolicyConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
@@ -1111,22 +947,14 @@
 )
 GetKeyGroupConfigRequestRequestTypeDef = TypedDict(
     "GetKeyGroupConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
-KeyGroupConfigOutputTypeDef = TypedDict(
-    "KeyGroupConfigOutputTypeDef",
-    {
-        "Name": str,
-        "Items": List[str],
-        "Comment": NotRequired[str],
-    },
-)
 GetKeyGroupRequestRequestTypeDef = TypedDict(
     "GetKeyGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 GetMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
@@ -1198,21 +1026,14 @@
 )
 GetStreamingDistributionRequestRequestTypeDef = TypedDict(
     "GetStreamingDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
-PathsOutputTypeDef = TypedDict(
-    "PathsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
 PathsTypeDef = TypedDict(
     "PathsTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[str]],
     },
 )
@@ -1448,26 +1269,19 @@
         "Description": str,
         "Name": str,
         "SigningProtocol": Literal["sigv4"],
         "SigningBehavior": OriginAccessControlSigningBehaviorsType,
         "OriginAccessControlOriginType": OriginAccessControlOriginTypesType,
     },
 )
-StatusCodesOutputTypeDef = TypedDict(
-    "StatusCodesOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[int],
-    },
-)
 StatusCodesTypeDef = TypedDict(
     "StatusCodesTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[int],
+        "Items": List[int],
     },
 )
 OriginGroupMemberTypeDef = TypedDict(
     "OriginGroupMemberTypeDef",
     {
         "OriginId": str,
     },
@@ -1505,63 +1319,35 @@
 QueryArgProfileTypeDef = TypedDict(
     "QueryArgProfileTypeDef",
     {
         "QueryArg": str,
         "ProfileId": str,
     },
 )
-ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[str],
-    },
-)
 ResponseHeadersPolicyAccessControlAllowHeadersTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[str],
     },
 )
-ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[ResponseHeadersPolicyAccessControlAllowMethodsValuesType],
-    },
-)
 ResponseHeadersPolicyAccessControlAllowMethodsTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[ResponseHeadersPolicyAccessControlAllowMethodsValuesType],
     },
 )
-ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[str],
-    },
-)
 ResponseHeadersPolicyAccessControlAllowOriginsTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[str],
     },
 )
-ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
 ResponseHeadersPolicyAccessControlExposeHeadersTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[str]],
     },
 )
@@ -1671,60 +1457,31 @@
     "UpdateKeyValueStoreRequestRequestTypeDef",
     {
         "Name": str,
         "Comment": str,
         "IfMatch": str,
     },
 )
-AllowedMethodsOutputTypeDef = TypedDict(
-    "AllowedMethodsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[MethodType],
-        "CachedMethods": NotRequired[CachedMethodsOutputTypeDef],
-    },
-)
 AllowedMethodsTypeDef = TypedDict(
     "AllowedMethodsTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[MethodType],
+        "Items": List[MethodType],
         "CachedMethods": NotRequired[CachedMethodsTypeDef],
     },
 )
 TestFunctionRequestRequestTypeDef = TypedDict(
     "TestFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
         "EventObject": BlobTypeDef,
         "Stage": NotRequired[FunctionStageType],
     },
 )
-CachePolicyCookiesConfigOutputTypeDef = TypedDict(
-    "CachePolicyCookiesConfigOutputTypeDef",
-    {
-        "CookieBehavior": CachePolicyCookieBehaviorType,
-        "Cookies": NotRequired[CookieNamesOutputTypeDef],
-    },
-)
-CookiePreferenceOutputTypeDef = TypedDict(
-    "CookiePreferenceOutputTypeDef",
-    {
-        "Forward": ItemSelectionType,
-        "WhitelistedNames": NotRequired[CookieNamesOutputTypeDef],
-    },
-)
-OriginRequestPolicyCookiesConfigOutputTypeDef = TypedDict(
-    "OriginRequestPolicyCookiesConfigOutputTypeDef",
-    {
-        "CookieBehavior": OriginRequestPolicyCookieBehaviorType,
-        "Cookies": NotRequired[CookieNamesOutputTypeDef],
-    },
-)
 CachePolicyCookiesConfigTypeDef = TypedDict(
     "CachePolicyCookiesConfigTypeDef",
     {
         "CookieBehavior": CachePolicyCookieBehaviorType,
         "Cookies": NotRequired[CookieNamesTypeDef],
     },
 )
@@ -1738,56 +1495,28 @@
 OriginRequestPolicyCookiesConfigTypeDef = TypedDict(
     "OriginRequestPolicyCookiesConfigTypeDef",
     {
         "CookieBehavior": OriginRequestPolicyCookieBehaviorType,
         "Cookies": NotRequired[CookieNamesTypeDef],
     },
 )
-CachePolicyHeadersConfigOutputTypeDef = TypedDict(
-    "CachePolicyHeadersConfigOutputTypeDef",
-    {
-        "HeaderBehavior": CachePolicyHeaderBehaviorType,
-        "Headers": NotRequired[HeadersOutputTypeDef],
-    },
-)
-OriginRequestPolicyHeadersConfigOutputTypeDef = TypedDict(
-    "OriginRequestPolicyHeadersConfigOutputTypeDef",
-    {
-        "HeaderBehavior": OriginRequestPolicyHeaderBehaviorType,
-        "Headers": NotRequired[HeadersOutputTypeDef],
-    },
-)
 CachePolicyHeadersConfigTypeDef = TypedDict(
     "CachePolicyHeadersConfigTypeDef",
     {
         "HeaderBehavior": CachePolicyHeaderBehaviorType,
         "Headers": NotRequired[HeadersTypeDef],
     },
 )
 OriginRequestPolicyHeadersConfigTypeDef = TypedDict(
     "OriginRequestPolicyHeadersConfigTypeDef",
     {
         "HeaderBehavior": OriginRequestPolicyHeaderBehaviorType,
         "Headers": NotRequired[HeadersTypeDef],
     },
 )
-CachePolicyQueryStringsConfigOutputTypeDef = TypedDict(
-    "CachePolicyQueryStringsConfigOutputTypeDef",
-    {
-        "QueryStringBehavior": CachePolicyQueryStringBehaviorType,
-        "QueryStrings": NotRequired[QueryStringNamesOutputTypeDef],
-    },
-)
-OriginRequestPolicyQueryStringsConfigOutputTypeDef = TypedDict(
-    "OriginRequestPolicyQueryStringsConfigOutputTypeDef",
-    {
-        "QueryStringBehavior": OriginRequestPolicyQueryStringBehaviorType,
-        "QueryStrings": NotRequired[QueryStringNamesOutputTypeDef],
-    },
-)
 CachePolicyQueryStringsConfigTypeDef = TypedDict(
     "CachePolicyQueryStringsConfigTypeDef",
     {
         "QueryStringBehavior": CachePolicyQueryStringBehaviorType,
         "QueryStrings": NotRequired[QueryStringNamesTypeDef],
     },
 )
@@ -1838,21 +1567,14 @@
     {
         "NextMarker": NotRequired[str],
         "MaxItems": NotRequired[int],
         "Quantity": NotRequired[int],
         "Items": NotRequired[List[ConflictingAliasTypeDef]],
     },
 )
-ContentTypeProfilesOutputTypeDef = TypedDict(
-    "ContentTypeProfilesOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[ContentTypeProfileTypeDef]],
-    },
-)
 ContentTypeProfilesTypeDef = TypedDict(
     "ContentTypeProfilesTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[ContentTypeProfileTypeDef]],
     },
 )
@@ -1888,14 +1610,30 @@
 )
 CreateKeyGroupRequestRequestTypeDef = TypedDict(
     "CreateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
     },
 )
+GetKeyGroupConfigResultTypeDef = TypedDict(
+    "GetKeyGroupConfigResultTypeDef",
+    {
+        "KeyGroupConfig": KeyGroupConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+KeyGroupTypeDef = TypedDict(
+    "KeyGroupTypeDef",
+    {
+        "Id": str,
+        "LastModifiedTime": datetime,
+        "KeyGroupConfig": KeyGroupConfigTypeDef,
+    },
+)
 UpdateKeyGroupRequestRequestTypeDef = TypedDict(
     "UpdateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
         "Id": str,
         "IfMatch": NotRequired[str],
     },
@@ -1997,51 +1735,26 @@
     "UpdatePublicKeyRequestRequestTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
         "Id": str,
         "IfMatch": NotRequired[str],
     },
 )
-CustomErrorResponsesOutputTypeDef = TypedDict(
-    "CustomErrorResponsesOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[CustomErrorResponseTypeDef]],
-    },
-)
 CustomErrorResponsesTypeDef = TypedDict(
     "CustomErrorResponsesTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[CustomErrorResponseTypeDef]],
-    },
-)
-CustomHeadersOutputTypeDef = TypedDict(
-    "CustomHeadersOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[OriginCustomHeaderTypeDef]],
+        "Items": NotRequired[List[CustomErrorResponseTypeDef]],
     },
 )
 CustomHeadersTypeDef = TypedDict(
     "CustomHeadersTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[OriginCustomHeaderTypeDef]],
-    },
-)
-CustomOriginConfigOutputTypeDef = TypedDict(
-    "CustomOriginConfigOutputTypeDef",
-    {
-        "HTTPPort": int,
-        "HTTPSPort": int,
-        "OriginProtocolPolicy": OriginProtocolPolicyType,
-        "OriginSslProtocols": NotRequired[OriginSslProtocolsOutputTypeDef],
-        "OriginReadTimeout": NotRequired[int],
-        "OriginKeepaliveTimeout": NotRequired[int],
+        "Items": NotRequired[List[OriginCustomHeaderTypeDef]],
     },
 )
 CustomOriginConfigTypeDef = TypedDict(
     "CustomOriginConfigTypeDef",
     {
         "HTTPPort": int,
         "HTTPSPort": int,
@@ -2075,22 +1788,14 @@
 ListDistributionsByResponseHeadersPolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-EncryptionEntityOutputTypeDef = TypedDict(
-    "EncryptionEntityOutputTypeDef",
-    {
-        "PublicKeyId": str,
-        "ProviderId": str,
-        "FieldPatterns": FieldPatternsOutputTypeDef,
-    },
-)
 EncryptionEntityTypeDef = TypedDict(
     "EncryptionEntityTypeDef",
     {
         "PublicKeyId": str,
         "ProviderId": str,
         "FieldPatterns": FieldPatternsTypeDef,
     },
@@ -2098,32 +1803,19 @@
 EndPointTypeDef = TypedDict(
     "EndPointTypeDef",
     {
         "StreamType": str,
         "KinesisStreamConfig": NotRequired[KinesisStreamConfigTypeDef],
     },
 )
-FunctionAssociationsOutputTypeDef = TypedDict(
-    "FunctionAssociationsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[FunctionAssociationTypeDef]],
-    },
-)
 FunctionAssociationsTypeDef = TypedDict(
     "FunctionAssociationsTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[FunctionAssociationTypeDef]],
-    },
-)
-RestrictionsOutputTypeDef = TypedDict(
-    "RestrictionsOutputTypeDef",
-    {
-        "GeoRestriction": GeoRestrictionOutputTypeDef,
+        "Items": NotRequired[List[FunctionAssociationTypeDef]],
     },
 )
 RestrictionsTypeDef = TypedDict(
     "RestrictionsTypeDef",
     {
         "GeoRestriction": GeoRestrictionTypeDef,
     },
@@ -2146,38 +1838,14 @@
 GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef = TypedDict(
     "GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
     {
         "Id": str,
         "WaiterConfig": NotRequired[WaiterConfigTypeDef],
     },
 )
-GetKeyGroupConfigResultTypeDef = TypedDict(
-    "GetKeyGroupConfigResultTypeDef",
-    {
-        "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-KeyGroupConfigUnionTypeDef = Union[KeyGroupConfigTypeDef, KeyGroupConfigOutputTypeDef]
-KeyGroupTypeDef = TypedDict(
-    "KeyGroupTypeDef",
-    {
-        "Id": str,
-        "LastModifiedTime": datetime,
-        "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
-    },
-)
-InvalidationBatchOutputTypeDef = TypedDict(
-    "InvalidationBatchOutputTypeDef",
-    {
-        "Paths": PathsOutputTypeDef,
-        "CallerReference": str,
-    },
-)
 InvalidationBatchTypeDef = TypedDict(
     "InvalidationBatchTypeDef",
     {
         "Paths": PathsTypeDef,
         "CallerReference": str,
     },
 )
@@ -2202,40 +1870,26 @@
 SignerTypeDef = TypedDict(
     "SignerTypeDef",
     {
         "AwsAccountNumber": NotRequired[str],
         "KeyPairIds": NotRequired[KeyPairIdsTypeDef],
     },
 )
-KeyValueStoreAssociationsOutputTypeDef = TypedDict(
-    "KeyValueStoreAssociationsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[KeyValueStoreAssociationTypeDef]],
-    },
-)
 KeyValueStoreAssociationsTypeDef = TypedDict(
     "KeyValueStoreAssociationsTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[KeyValueStoreAssociationTypeDef]],
     },
 )
-LambdaFunctionAssociationsOutputTypeDef = TypedDict(
-    "LambdaFunctionAssociationsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[LambdaFunctionAssociationTypeDef]],
-    },
-)
 LambdaFunctionAssociationsTypeDef = TypedDict(
     "LambdaFunctionAssociationsTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[LambdaFunctionAssociationTypeDef]],
+        "Items": NotRequired[List[LambdaFunctionAssociationTypeDef]],
     },
 )
 ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef = TypedDict(
     "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
@@ -2279,112 +1933,64 @@
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[OriginAccessControlSummaryTypeDef]],
     },
 )
-OriginGroupFailoverCriteriaOutputTypeDef = TypedDict(
-    "OriginGroupFailoverCriteriaOutputTypeDef",
-    {
-        "StatusCodes": StatusCodesOutputTypeDef,
-    },
-)
 OriginGroupFailoverCriteriaTypeDef = TypedDict(
     "OriginGroupFailoverCriteriaTypeDef",
     {
         "StatusCodes": StatusCodesTypeDef,
     },
 )
-OriginGroupMembersOutputTypeDef = TypedDict(
-    "OriginGroupMembersOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[OriginGroupMemberTypeDef],
-    },
-)
 OriginGroupMembersTypeDef = TypedDict(
     "OriginGroupMembersTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[OriginGroupMemberTypeDef],
+        "Items": List[OriginGroupMemberTypeDef],
     },
 )
 PublicKeyListTypeDef = TypedDict(
     "PublicKeyListTypeDef",
     {
         "MaxItems": int,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[PublicKeySummaryTypeDef]],
     },
 )
-QueryArgProfilesOutputTypeDef = TypedDict(
-    "QueryArgProfilesOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[QueryArgProfileTypeDef]],
-    },
-)
 QueryArgProfilesTypeDef = TypedDict(
     "QueryArgProfilesTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[QueryArgProfileTypeDef]],
     },
 )
-ResponseHeadersPolicyCorsConfigOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyCorsConfigOutputTypeDef",
-    {
-        "AccessControlAllowOrigins": ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef,
-        "AccessControlAllowHeaders": ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef,
-        "AccessControlAllowMethods": ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef,
-        "AccessControlAllowCredentials": bool,
-        "OriginOverride": bool,
-        "AccessControlExposeHeaders": NotRequired[
-            ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef
-        ],
-        "AccessControlMaxAgeSec": NotRequired[int],
-    },
-)
 ResponseHeadersPolicyCorsConfigTypeDef = TypedDict(
     "ResponseHeadersPolicyCorsConfigTypeDef",
     {
         "AccessControlAllowOrigins": ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
         "AccessControlAllowHeaders": ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
         "AccessControlAllowMethods": ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
         "AccessControlAllowCredentials": bool,
         "OriginOverride": bool,
         "AccessControlExposeHeaders": NotRequired[
             ResponseHeadersPolicyAccessControlExposeHeadersTypeDef
         ],
         "AccessControlMaxAgeSec": NotRequired[int],
     },
 )
-ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[ResponseHeadersPolicyCustomHeaderTypeDef]],
-    },
-)
 ResponseHeadersPolicyCustomHeadersConfigTypeDef = TypedDict(
     "ResponseHeadersPolicyCustomHeadersConfigTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[ResponseHeadersPolicyCustomHeaderTypeDef]],
     },
 )
-ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[ResponseHeadersPolicyRemoveHeaderTypeDef]],
-    },
-)
 ResponseHeadersPolicyRemoveHeadersConfigTypeDef = TypedDict(
     "ResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[ResponseHeadersPolicyRemoveHeaderTypeDef]],
     },
 )
@@ -2404,34 +2010,21 @@
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
         "S3Origin": S3OriginTypeDef,
-        "Aliases": AliasesOutputTypeDef,
-        "TrustedSigners": TrustedSignersOutputTypeDef,
+        "Aliases": AliasesTypeDef,
+        "TrustedSigners": TrustedSignersTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
     },
 )
-StreamingDistributionConfigOutputTypeDef = TypedDict(
-    "StreamingDistributionConfigOutputTypeDef",
-    {
-        "CallerReference": str,
-        "S3Origin": S3OriginTypeDef,
-        "Comment": str,
-        "TrustedSigners": TrustedSignersOutputTypeDef,
-        "Enabled": bool,
-        "Aliases": NotRequired[AliasesOutputTypeDef],
-        "Logging": NotRequired[StreamingLoggingConfigTypeDef],
-        "PriceClass": NotRequired[PriceClassType],
-    },
-)
 StreamingDistributionConfigTypeDef = TypedDict(
     "StreamingDistributionConfigTypeDef",
     {
         "CallerReference": str,
         "S3Origin": S3OriginTypeDef,
         "Comment": str,
         "TrustedSigners": TrustedSignersTypeDef,
@@ -2444,64 +2037,29 @@
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "TagKeys": TagKeysTypeDef,
     },
 )
-TagsOutputTypeDef = TypedDict(
-    "TagsOutputTypeDef",
-    {
-        "Items": NotRequired[List[TagTypeDef]],
-    },
-)
 TagsTypeDef = TypedDict(
     "TagsTypeDef",
     {
         "Items": NotRequired[Sequence[TagTypeDef]],
     },
 )
-ForwardedValuesOutputTypeDef = TypedDict(
-    "ForwardedValuesOutputTypeDef",
-    {
-        "QueryString": bool,
-        "Cookies": CookiePreferenceOutputTypeDef,
-        "Headers": NotRequired[HeadersOutputTypeDef],
-        "QueryStringCacheKeys": NotRequired[QueryStringCacheKeysOutputTypeDef],
-    },
-)
 ForwardedValuesTypeDef = TypedDict(
     "ForwardedValuesTypeDef",
     {
         "QueryString": bool,
         "Cookies": CookiePreferenceTypeDef,
         "Headers": NotRequired[HeadersTypeDef],
         "QueryStringCacheKeys": NotRequired[QueryStringCacheKeysTypeDef],
     },
 )
-ParametersInCacheKeyAndForwardedToOriginOutputTypeDef = TypedDict(
-    "ParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
-    {
-        "EnableAcceptEncodingGzip": bool,
-        "HeadersConfig": CachePolicyHeadersConfigOutputTypeDef,
-        "CookiesConfig": CachePolicyCookiesConfigOutputTypeDef,
-        "QueryStringsConfig": CachePolicyQueryStringsConfigOutputTypeDef,
-        "EnableAcceptEncodingBrotli": NotRequired[bool],
-    },
-)
-OriginRequestPolicyConfigOutputTypeDef = TypedDict(
-    "OriginRequestPolicyConfigOutputTypeDef",
-    {
-        "Name": str,
-        "HeadersConfig": OriginRequestPolicyHeadersConfigOutputTypeDef,
-        "CookiesConfig": OriginRequestPolicyCookiesConfigOutputTypeDef,
-        "QueryStringsConfig": OriginRequestPolicyQueryStringsConfigOutputTypeDef,
-        "Comment": NotRequired[str],
-    },
-)
 ParametersInCacheKeyAndForwardedToOriginTypeDef = TypedDict(
     "ParametersInCacheKeyAndForwardedToOriginTypeDef",
     {
         "EnableAcceptEncodingGzip": bool,
         "HeadersConfig": CachePolicyHeadersConfigTypeDef,
         "CookiesConfig": CachePolicyCookiesConfigTypeDef,
         "QueryStringsConfig": CachePolicyQueryStringsConfigTypeDef,
@@ -2553,21 +2111,14 @@
 ListConflictingAliasesResultTypeDef = TypedDict(
     "ListConflictingAliasesResultTypeDef",
     {
         "ConflictingAliasesList": ConflictingAliasesListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ContentTypeProfileConfigOutputTypeDef = TypedDict(
-    "ContentTypeProfileConfigOutputTypeDef",
-    {
-        "ForwardWhenContentTypeIsUnknown": bool,
-        "ContentTypeProfiles": NotRequired[ContentTypeProfilesOutputTypeDef],
-    },
-)
 ContentTypeProfileConfigTypeDef = TypedDict(
     "ContentTypeProfileConfigTypeDef",
     {
         "ForwardWhenContentTypeIsUnknown": bool,
         "ContentTypeProfiles": NotRequired[ContentTypeProfilesTypeDef],
     },
 )
@@ -2575,14 +2126,45 @@
     "TrafficConfigTypeDef",
     {
         "Type": ContinuousDeploymentPolicyTypeType,
         "SingleWeightConfig": NotRequired[ContinuousDeploymentSingleWeightConfigTypeDef],
         "SingleHeaderConfig": NotRequired[ContinuousDeploymentSingleHeaderConfigTypeDef],
     },
 )
+CreateKeyGroupResultTypeDef = TypedDict(
+    "CreateKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "Location": str,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetKeyGroupResultTypeDef = TypedDict(
+    "GetKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+KeyGroupSummaryTypeDef = TypedDict(
+    "KeyGroupSummaryTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+    },
+)
+UpdateKeyGroupResultTypeDef = TypedDict(
+    "UpdateKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListKeyValueStoresResultTypeDef = TypedDict(
     "ListKeyValueStoresResultTypeDef",
     {
         "KeyValueStoreList": KeyValueStoreListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2632,29 +2214,14 @@
     "UpdatePublicKeyResultTypeDef",
     {
         "PublicKey": PublicKeyTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-OriginOutputTypeDef = TypedDict(
-    "OriginOutputTypeDef",
-    {
-        "Id": str,
-        "DomainName": str,
-        "OriginPath": NotRequired[str],
-        "CustomHeaders": NotRequired[CustomHeadersOutputTypeDef],
-        "S3OriginConfig": NotRequired[S3OriginConfigTypeDef],
-        "CustomOriginConfig": NotRequired[CustomOriginConfigOutputTypeDef],
-        "ConnectionAttempts": NotRequired[int],
-        "ConnectionTimeout": NotRequired[int],
-        "OriginShield": NotRequired[OriginShieldTypeDef],
-        "OriginAccessControlId": NotRequired[str],
-    },
-)
 OriginTypeDef = TypedDict(
     "OriginTypeDef",
     {
         "Id": str,
         "DomainName": str,
         "OriginPath": NotRequired[str],
         "CustomHeaders": NotRequired[CustomHeadersTypeDef],
@@ -2662,21 +2229,14 @@
         "CustomOriginConfig": NotRequired[CustomOriginConfigTypeDef],
         "ConnectionAttempts": NotRequired[int],
         "ConnectionTimeout": NotRequired[int],
         "OriginShield": NotRequired[OriginShieldTypeDef],
         "OriginAccessControlId": NotRequired[str],
     },
 )
-EncryptionEntitiesOutputTypeDef = TypedDict(
-    "EncryptionEntitiesOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[EncryptionEntityOutputTypeDef]],
-    },
-)
 EncryptionEntitiesTypeDef = TypedDict(
     "EncryptionEntitiesTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[EncryptionEntityTypeDef]],
     },
 )
@@ -2705,62 +2265,30 @@
         "EndPoints": NotRequired[Sequence[EndPointTypeDef]],
         "Fields": NotRequired[Sequence[str]],
         "Name": NotRequired[str],
         "ARN": NotRequired[str],
         "SamplingRate": NotRequired[int],
     },
 )
-CreateKeyGroupResultTypeDef = TypedDict(
-    "CreateKeyGroupResultTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-        "Location": str,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-GetKeyGroupResultTypeDef = TypedDict(
-    "GetKeyGroupResultTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-KeyGroupSummaryTypeDef = TypedDict(
-    "KeyGroupSummaryTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-    },
-)
-UpdateKeyGroupResultTypeDef = TypedDict(
-    "UpdateKeyGroupResultTypeDef",
+CreateInvalidationRequestRequestTypeDef = TypedDict(
+    "CreateInvalidationRequestRequestTypeDef",
     {
-        "KeyGroup": KeyGroupTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DistributionId": str,
+        "InvalidationBatch": InvalidationBatchTypeDef,
     },
 )
 InvalidationTypeDef = TypedDict(
     "InvalidationTypeDef",
     {
         "Id": str,
         "Status": str,
         "CreateTime": datetime,
-        "InvalidationBatch": InvalidationBatchOutputTypeDef,
-    },
-)
-CreateInvalidationRequestRequestTypeDef = TypedDict(
-    "CreateInvalidationRequestRequestTypeDef",
-    {
-        "DistributionId": str,
         "InvalidationBatch": InvalidationBatchTypeDef,
     },
 )
-InvalidationBatchUnionTypeDef = Union[InvalidationBatchTypeDef, InvalidationBatchOutputTypeDef]
 ListInvalidationsResultTypeDef = TypedDict(
     "ListInvalidationsResultTypeDef",
     {
         "InvalidationList": InvalidationListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2776,22 +2304,14 @@
     "ActiveTrustedSignersTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
         "Items": NotRequired[List[SignerTypeDef]],
     },
 )
-FunctionConfigOutputTypeDef = TypedDict(
-    "FunctionConfigOutputTypeDef",
-    {
-        "Comment": str,
-        "Runtime": FunctionRuntimeType,
-        "KeyValueStoreAssociations": NotRequired[KeyValueStoreAssociationsOutputTypeDef],
-    },
-)
 FunctionConfigTypeDef = TypedDict(
     "FunctionConfigTypeDef",
     {
         "Comment": str,
         "Runtime": FunctionRuntimeType,
         "KeyValueStoreAssociations": NotRequired[KeyValueStoreAssociationsTypeDef],
     },
@@ -2820,22 +2340,14 @@
 ListOriginAccessControlsResultTypeDef = TypedDict(
     "ListOriginAccessControlsResultTypeDef",
     {
         "OriginAccessControlList": OriginAccessControlListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-OriginGroupOutputTypeDef = TypedDict(
-    "OriginGroupOutputTypeDef",
-    {
-        "Id": str,
-        "FailoverCriteria": OriginGroupFailoverCriteriaOutputTypeDef,
-        "Members": OriginGroupMembersOutputTypeDef,
-    },
-)
 OriginGroupTypeDef = TypedDict(
     "OriginGroupTypeDef",
     {
         "Id": str,
         "FailoverCriteria": OriginGroupFailoverCriteriaTypeDef,
         "Members": OriginGroupMembersTypeDef,
     },
@@ -2843,42 +2355,21 @@
 ListPublicKeysResultTypeDef = TypedDict(
     "ListPublicKeysResultTypeDef",
     {
         "PublicKeyList": PublicKeyListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-QueryArgProfileConfigOutputTypeDef = TypedDict(
-    "QueryArgProfileConfigOutputTypeDef",
-    {
-        "ForwardWhenQueryArgProfileIsUnknown": bool,
-        "QueryArgProfiles": NotRequired[QueryArgProfilesOutputTypeDef],
-    },
-)
 QueryArgProfileConfigTypeDef = TypedDict(
     "QueryArgProfileConfigTypeDef",
     {
         "ForwardWhenQueryArgProfileIsUnknown": bool,
         "QueryArgProfiles": NotRequired[QueryArgProfilesTypeDef],
     },
 )
-ResponseHeadersPolicyConfigOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyConfigOutputTypeDef",
-    {
-        "Name": str,
-        "Comment": NotRequired[str],
-        "CorsConfig": NotRequired[ResponseHeadersPolicyCorsConfigOutputTypeDef],
-        "SecurityHeadersConfig": NotRequired[ResponseHeadersPolicySecurityHeadersConfigTypeDef],
-        "ServerTimingHeadersConfig": NotRequired[
-            ResponseHeadersPolicyServerTimingHeadersConfigTypeDef
-        ],
-        "CustomHeadersConfig": NotRequired[ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef],
-        "RemoveHeadersConfig": NotRequired[ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef],
-    },
-)
 ResponseHeadersPolicyConfigTypeDef = TypedDict(
     "ResponseHeadersPolicyConfigTypeDef",
     {
         "Name": str,
         "Comment": NotRequired[str],
         "CorsConfig": NotRequired[ResponseHeadersPolicyCorsConfigTypeDef],
         "SecurityHeadersConfig": NotRequired[ResponseHeadersPolicySecurityHeadersConfigTypeDef],
@@ -2896,43 +2387,40 @@
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[StreamingDistributionSummaryTypeDef]],
     },
 )
-GetStreamingDistributionConfigResultTypeDef = TypedDict(
-    "GetStreamingDistributionConfigResultTypeDef",
+CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
+    "CreateStreamingDistributionRequestRequestTypeDef",
     {
-        "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
     },
 )
-CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
-    "CreateStreamingDistributionRequestRequestTypeDef",
+GetStreamingDistributionConfigResultTypeDef = TypedDict(
+    "GetStreamingDistributionConfigResultTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-StreamingDistributionConfigUnionTypeDef = Union[
-    StreamingDistributionConfigTypeDef, StreamingDistributionConfigOutputTypeDef
-]
 UpdateStreamingDistributionRequestRequestTypeDef = TypedDict(
     "UpdateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
         "Id": str,
         "IfMatch": NotRequired[str],
     },
 )
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
-        "Tags": TagsOutputTypeDef,
+        "Tags": TagsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 StreamingDistributionConfigWithTagsTypeDef = TypedDict(
     "StreamingDistributionConfigWithTagsTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
@@ -2942,62 +2430,14 @@
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "Tags": TagsTypeDef,
     },
 )
-TagsUnionTypeDef = Union[TagsTypeDef, TagsOutputTypeDef]
-CacheBehaviorOutputTypeDef = TypedDict(
-    "CacheBehaviorOutputTypeDef",
-    {
-        "PathPattern": str,
-        "TargetOriginId": str,
-        "ViewerProtocolPolicy": ViewerProtocolPolicyType,
-        "TrustedSigners": NotRequired[TrustedSignersOutputTypeDef],
-        "TrustedKeyGroups": NotRequired[TrustedKeyGroupsOutputTypeDef],
-        "AllowedMethods": NotRequired[AllowedMethodsOutputTypeDef],
-        "SmoothStreaming": NotRequired[bool],
-        "Compress": NotRequired[bool],
-        "LambdaFunctionAssociations": NotRequired[LambdaFunctionAssociationsOutputTypeDef],
-        "FunctionAssociations": NotRequired[FunctionAssociationsOutputTypeDef],
-        "FieldLevelEncryptionId": NotRequired[str],
-        "RealtimeLogConfigArn": NotRequired[str],
-        "CachePolicyId": NotRequired[str],
-        "OriginRequestPolicyId": NotRequired[str],
-        "ResponseHeadersPolicyId": NotRequired[str],
-        "ForwardedValues": NotRequired[ForwardedValuesOutputTypeDef],
-        "MinTTL": NotRequired[int],
-        "DefaultTTL": NotRequired[int],
-        "MaxTTL": NotRequired[int],
-    },
-)
-DefaultCacheBehaviorOutputTypeDef = TypedDict(
-    "DefaultCacheBehaviorOutputTypeDef",
-    {
-        "TargetOriginId": str,
-        "ViewerProtocolPolicy": ViewerProtocolPolicyType,
-        "TrustedSigners": NotRequired[TrustedSignersOutputTypeDef],
-        "TrustedKeyGroups": NotRequired[TrustedKeyGroupsOutputTypeDef],
-        "AllowedMethods": NotRequired[AllowedMethodsOutputTypeDef],
-        "SmoothStreaming": NotRequired[bool],
-        "Compress": NotRequired[bool],
-        "LambdaFunctionAssociations": NotRequired[LambdaFunctionAssociationsOutputTypeDef],
-        "FunctionAssociations": NotRequired[FunctionAssociationsOutputTypeDef],
-        "FieldLevelEncryptionId": NotRequired[str],
-        "RealtimeLogConfigArn": NotRequired[str],
-        "CachePolicyId": NotRequired[str],
-        "OriginRequestPolicyId": NotRequired[str],
-        "ResponseHeadersPolicyId": NotRequired[str],
-        "ForwardedValues": NotRequired[ForwardedValuesOutputTypeDef],
-        "MinTTL": NotRequired[int],
-        "DefaultTTL": NotRequired[int],
-        "MaxTTL": NotRequired[int],
-    },
-)
 CacheBehaviorTypeDef = TypedDict(
     "CacheBehaviorTypeDef",
     {
         "PathPattern": str,
         "TargetOriginId": str,
         "ViewerProtocolPolicy": ViewerProtocolPolicyType,
         "TrustedSigners": NotRequired[TrustedSignersTypeDef],
@@ -3037,127 +2477,96 @@
         "ResponseHeadersPolicyId": NotRequired[str],
         "ForwardedValues": NotRequired[ForwardedValuesTypeDef],
         "MinTTL": NotRequired[int],
         "DefaultTTL": NotRequired[int],
         "MaxTTL": NotRequired[int],
     },
 )
-CachePolicyConfigOutputTypeDef = TypedDict(
-    "CachePolicyConfigOutputTypeDef",
+CachePolicyConfigTypeDef = TypedDict(
+    "CachePolicyConfigTypeDef",
     {
         "Name": str,
         "MinTTL": int,
         "Comment": NotRequired[str],
         "DefaultTTL": NotRequired[int],
         "MaxTTL": NotRequired[int],
         "ParametersInCacheKeyAndForwardedToOrigin": NotRequired[
-            ParametersInCacheKeyAndForwardedToOriginOutputTypeDef
+            ParametersInCacheKeyAndForwardedToOriginTypeDef
         ],
     },
 )
+CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
+    "CreateOriginRequestPolicyRequestRequestTypeDef",
+    {
+        "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
+    },
+)
 GetOriginRequestPolicyConfigResultTypeDef = TypedDict(
     "GetOriginRequestPolicyConfigResultTypeDef",
     {
-        "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
+        "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 OriginRequestPolicyTypeDef = TypedDict(
     "OriginRequestPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
-    },
-)
-CachePolicyConfigTypeDef = TypedDict(
-    "CachePolicyConfigTypeDef",
-    {
-        "Name": str,
-        "MinTTL": int,
-        "Comment": NotRequired[str],
-        "DefaultTTL": NotRequired[int],
-        "MaxTTL": NotRequired[int],
-        "ParametersInCacheKeyAndForwardedToOrigin": NotRequired[
-            ParametersInCacheKeyAndForwardedToOriginTypeDef
-        ],
-    },
-)
-CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
-    "CreateOriginRequestPolicyRequestRequestTypeDef",
-    {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
     },
 )
-OriginRequestPolicyConfigUnionTypeDef = Union[
-    OriginRequestPolicyConfigTypeDef, OriginRequestPolicyConfigOutputTypeDef
-]
 UpdateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "UpdateOriginRequestPolicyRequestRequestTypeDef",
     {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
         "Id": str,
         "IfMatch": NotRequired[str],
     },
 )
-ContinuousDeploymentPolicyConfigOutputTypeDef = TypedDict(
-    "ContinuousDeploymentPolicyConfigOutputTypeDef",
-    {
-        "StagingDistributionDnsNames": StagingDistributionDnsNamesOutputTypeDef,
-        "Enabled": bool,
-        "TrafficConfig": NotRequired[TrafficConfigTypeDef],
-    },
-)
 ContinuousDeploymentPolicyConfigTypeDef = TypedDict(
     "ContinuousDeploymentPolicyConfigTypeDef",
     {
         "StagingDistributionDnsNames": StagingDistributionDnsNamesTypeDef,
         "Enabled": bool,
         "TrafficConfig": NotRequired[TrafficConfigTypeDef],
     },
 )
-OriginsOutputTypeDef = TypedDict(
-    "OriginsOutputTypeDef",
+KeyGroupListTypeDef = TypedDict(
+    "KeyGroupListTypeDef",
     {
+        "MaxItems": int,
         "Quantity": int,
-        "Items": List[OriginOutputTypeDef],
+        "NextMarker": NotRequired[str],
+        "Items": NotRequired[List[KeyGroupSummaryTypeDef]],
     },
 )
 OriginsTypeDef = TypedDict(
     "OriginsTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[OriginTypeDef],
+        "Items": List[OriginTypeDef],
     },
 )
-FieldLevelEncryptionProfileConfigOutputTypeDef = TypedDict(
-    "FieldLevelEncryptionProfileConfigOutputTypeDef",
+FieldLevelEncryptionProfileConfigTypeDef = TypedDict(
+    "FieldLevelEncryptionProfileConfigTypeDef",
     {
         "Name": str,
         "CallerReference": str,
-        "EncryptionEntities": EncryptionEntitiesOutputTypeDef,
+        "EncryptionEntities": EncryptionEntitiesTypeDef,
         "Comment": NotRequired[str],
     },
 )
 FieldLevelEncryptionProfileSummaryTypeDef = TypedDict(
     "FieldLevelEncryptionProfileSummaryTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
         "Name": str,
-        "EncryptionEntities": EncryptionEntitiesOutputTypeDef,
-        "Comment": NotRequired[str],
-    },
-)
-FieldLevelEncryptionProfileConfigTypeDef = TypedDict(
-    "FieldLevelEncryptionProfileConfigTypeDef",
-    {
-        "Name": str,
-        "CallerReference": str,
         "EncryptionEntities": EncryptionEntitiesTypeDef,
         "Comment": NotRequired[str],
     },
 )
 CreateRealtimeLogConfigResultTypeDef = TypedDict(
     "CreateRealtimeLogConfigResultTypeDef",
     {
@@ -3185,23 +2594,14 @@
 UpdateRealtimeLogConfigResultTypeDef = TypedDict(
     "UpdateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-KeyGroupListTypeDef = TypedDict(
-    "KeyGroupListTypeDef",
-    {
-        "MaxItems": int,
-        "Quantity": int,
-        "NextMarker": NotRequired[str],
-        "Items": NotRequired[List[KeyGroupSummaryTypeDef]],
-    },
-)
 CreateInvalidationResultTypeDef = TypedDict(
     "CreateInvalidationResultTypeDef",
     {
         "Location": str,
         "Invalidation": InvalidationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3217,112 +2617,92 @@
     "StreamingDistributionTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "DomainName": str,
         "ActiveTrustedSigners": ActiveTrustedSignersTypeDef,
-        "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
+        "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
         "LastModifiedTime": NotRequired[datetime],
     },
 )
-FunctionSummaryTypeDef = TypedDict(
-    "FunctionSummaryTypeDef",
+CreateFunctionRequestRequestTypeDef = TypedDict(
+    "CreateFunctionRequestRequestTypeDef",
     {
         "Name": str,
-        "FunctionConfig": FunctionConfigOutputTypeDef,
-        "FunctionMetadata": FunctionMetadataTypeDef,
-        "Status": NotRequired[str],
+        "FunctionConfig": FunctionConfigTypeDef,
+        "FunctionCode": BlobTypeDef,
     },
 )
-CreateFunctionRequestRequestTypeDef = TypedDict(
-    "CreateFunctionRequestRequestTypeDef",
+FunctionSummaryTypeDef = TypedDict(
+    "FunctionSummaryTypeDef",
     {
         "Name": str,
         "FunctionConfig": FunctionConfigTypeDef,
-        "FunctionCode": BlobTypeDef,
+        "FunctionMetadata": FunctionMetadataTypeDef,
+        "Status": NotRequired[str],
     },
 )
-FunctionConfigUnionTypeDef = Union[FunctionConfigTypeDef, FunctionConfigOutputTypeDef]
 UpdateFunctionRequestRequestTypeDef = TypedDict(
     "UpdateFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
         "FunctionConfig": FunctionConfigTypeDef,
         "FunctionCode": BlobTypeDef,
     },
 )
-OriginGroupsOutputTypeDef = TypedDict(
-    "OriginGroupsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[OriginGroupOutputTypeDef]],
-    },
-)
 OriginGroupsTypeDef = TypedDict(
     "OriginGroupsTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[OriginGroupTypeDef]],
+        "Items": NotRequired[List[OriginGroupTypeDef]],
     },
 )
-FieldLevelEncryptionConfigOutputTypeDef = TypedDict(
-    "FieldLevelEncryptionConfigOutputTypeDef",
+FieldLevelEncryptionConfigTypeDef = TypedDict(
+    "FieldLevelEncryptionConfigTypeDef",
     {
         "CallerReference": str,
         "Comment": NotRequired[str],
-        "QueryArgProfileConfig": NotRequired[QueryArgProfileConfigOutputTypeDef],
-        "ContentTypeProfileConfig": NotRequired[ContentTypeProfileConfigOutputTypeDef],
+        "QueryArgProfileConfig": NotRequired[QueryArgProfileConfigTypeDef],
+        "ContentTypeProfileConfig": NotRequired[ContentTypeProfileConfigTypeDef],
     },
 )
 FieldLevelEncryptionSummaryTypeDef = TypedDict(
     "FieldLevelEncryptionSummaryTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
         "Comment": NotRequired[str],
-        "QueryArgProfileConfig": NotRequired[QueryArgProfileConfigOutputTypeDef],
-        "ContentTypeProfileConfig": NotRequired[ContentTypeProfileConfigOutputTypeDef],
+        "QueryArgProfileConfig": NotRequired[QueryArgProfileConfigTypeDef],
+        "ContentTypeProfileConfig": NotRequired[ContentTypeProfileConfigTypeDef],
     },
 )
-FieldLevelEncryptionConfigTypeDef = TypedDict(
-    "FieldLevelEncryptionConfigTypeDef",
+CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
+    "CreateResponseHeadersPolicyRequestRequestTypeDef",
     {
-        "CallerReference": str,
-        "Comment": NotRequired[str],
-        "QueryArgProfileConfig": NotRequired[QueryArgProfileConfigTypeDef],
-        "ContentTypeProfileConfig": NotRequired[ContentTypeProfileConfigTypeDef],
+        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
     },
 )
 GetResponseHeadersPolicyConfigResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyConfigResultTypeDef",
     {
-        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
+        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ResponseHeadersPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
-    },
-)
-CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
-    "CreateResponseHeadersPolicyRequestRequestTypeDef",
-    {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
     },
 )
-ResponseHeadersPolicyConfigUnionTypeDef = Union[
-    ResponseHeadersPolicyConfigTypeDef, ResponseHeadersPolicyConfigOutputTypeDef
-]
 UpdateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
     "UpdateResponseHeadersPolicyRequestRequestTypeDef",
     {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
         "Id": str,
         "IfMatch": NotRequired[str],
     },
@@ -3336,44 +2716,51 @@
 )
 CreateStreamingDistributionWithTagsRequestRequestTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
     {
         "StreamingDistributionConfigWithTags": StreamingDistributionConfigWithTagsTypeDef,
     },
 )
-CacheBehaviorsOutputTypeDef = TypedDict(
-    "CacheBehaviorsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[CacheBehaviorOutputTypeDef]],
-    },
-)
 CacheBehaviorsTypeDef = TypedDict(
     "CacheBehaviorsTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[CacheBehaviorTypeDef]],
+        "Items": NotRequired[List[CacheBehaviorTypeDef]],
     },
 )
 CachePolicyTypeDef = TypedDict(
     "CachePolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
+    },
+)
+CreateCachePolicyRequestRequestTypeDef = TypedDict(
+    "CreateCachePolicyRequestRequestTypeDef",
+    {
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
     },
 )
 GetCachePolicyConfigResultTypeDef = TypedDict(
     "GetCachePolicyConfigResultTypeDef",
     {
-        "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateCachePolicyRequestRequestTypeDef = TypedDict(
+    "UpdateCachePolicyRequestRequestTypeDef",
+    {
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
+        "Id": str,
+        "IfMatch": NotRequired[str],
+    },
+)
 CreateOriginRequestPolicyResultTypeDef = TypedDict(
     "CreateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3398,118 +2785,97 @@
     "UpdateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CachePolicyConfigUnionTypeDef = Union[CachePolicyConfigTypeDef, CachePolicyConfigOutputTypeDef]
-CreateCachePolicyRequestRequestTypeDef = TypedDict(
-    "CreateCachePolicyRequestRequestTypeDef",
-    {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
-    },
-)
-UpdateCachePolicyRequestRequestTypeDef = TypedDict(
-    "UpdateCachePolicyRequestRequestTypeDef",
-    {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
-        "Id": str,
-        "IfMatch": NotRequired[str],
-    },
-)
 ContinuousDeploymentPolicyTypeDef = TypedDict(
     "ContinuousDeploymentPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
     },
 )
-GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
-    "GetContinuousDeploymentPolicyConfigResultTypeDef",
+CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
+    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
     },
 )
-ContinuousDeploymentPolicyConfigUnionTypeDef = Union[
-    ContinuousDeploymentPolicyConfigTypeDef, ContinuousDeploymentPolicyConfigOutputTypeDef
-]
-CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
-    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
+GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
+    "GetContinuousDeploymentPolicyConfigResultTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 UpdateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "UpdateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
         "Id": str,
         "IfMatch": NotRequired[str],
     },
 )
+ListKeyGroupsResultTypeDef = TypedDict(
+    "ListKeyGroupsResultTypeDef",
+    {
+        "KeyGroupList": KeyGroupListTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
+    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
+    {
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
+    },
+)
 FieldLevelEncryptionProfileTypeDef = TypedDict(
     "FieldLevelEncryptionProfileTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
     },
 )
 GetFieldLevelEncryptionProfileConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionProfileConfigResultTypeDef",
     {
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
+    "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
+    {
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
+        "Id": str,
+        "IfMatch": NotRequired[str],
+    },
+)
 FieldLevelEncryptionProfileListTypeDef = TypedDict(
     "FieldLevelEncryptionProfileListTypeDef",
     {
         "MaxItems": int,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[FieldLevelEncryptionProfileSummaryTypeDef]],
     },
 )
-CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
-    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
-    {
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
-    },
-)
-FieldLevelEncryptionProfileConfigUnionTypeDef = Union[
-    FieldLevelEncryptionProfileConfigTypeDef, FieldLevelEncryptionProfileConfigOutputTypeDef
-]
-UpdateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
-    "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
-    {
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
-        "Id": str,
-        "IfMatch": NotRequired[str],
-    },
-)
 ListRealtimeLogConfigsResultTypeDef = TypedDict(
     "ListRealtimeLogConfigsResultTypeDef",
     {
         "RealtimeLogConfigs": RealtimeLogConfigsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListKeyGroupsResultTypeDef = TypedDict(
-    "ListKeyGroupsResultTypeDef",
-    {
-        "KeyGroupList": KeyGroupListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 CreateStreamingDistributionResultTypeDef = TypedDict(
     "CreateStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3587,56 +2953,53 @@
     "UpdateFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    {
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+    },
+)
 FieldLevelEncryptionTypeDef = TypedDict(
     "FieldLevelEncryptionTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
     },
 )
 GetFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionConfigResultTypeDef",
     {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    {
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+        "Id": str,
+        "IfMatch": NotRequired[str],
+    },
+)
 FieldLevelEncryptionListTypeDef = TypedDict(
     "FieldLevelEncryptionListTypeDef",
     {
         "MaxItems": int,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[FieldLevelEncryptionSummaryTypeDef]],
     },
 )
-CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
-    {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
-    },
-)
-FieldLevelEncryptionConfigUnionTypeDef = Union[
-    FieldLevelEncryptionConfigTypeDef, FieldLevelEncryptionConfigOutputTypeDef
-]
-UpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
-    {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
-        "Id": str,
-        "IfMatch": NotRequired[str],
-    },
-)
 CreateResponseHeadersPolicyResultTypeDef = TypedDict(
     "CreateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3661,31 +3024,31 @@
     "UpdateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DistributionConfigOutputTypeDef = TypedDict(
-    "DistributionConfigOutputTypeDef",
+DistributionConfigTypeDef = TypedDict(
+    "DistributionConfigTypeDef",
     {
         "CallerReference": str,
-        "Origins": OriginsOutputTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
+        "Origins": OriginsTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
         "Comment": str,
         "Enabled": bool,
-        "Aliases": NotRequired[AliasesOutputTypeDef],
+        "Aliases": NotRequired[AliasesTypeDef],
         "DefaultRootObject": NotRequired[str],
-        "OriginGroups": NotRequired[OriginGroupsOutputTypeDef],
-        "CacheBehaviors": NotRequired[CacheBehaviorsOutputTypeDef],
-        "CustomErrorResponses": NotRequired[CustomErrorResponsesOutputTypeDef],
+        "OriginGroups": NotRequired[OriginGroupsTypeDef],
+        "CacheBehaviors": NotRequired[CacheBehaviorsTypeDef],
+        "CustomErrorResponses": NotRequired[CustomErrorResponsesTypeDef],
         "Logging": NotRequired[LoggingConfigTypeDef],
         "PriceClass": NotRequired[PriceClassType],
         "ViewerCertificate": NotRequired[ViewerCertificateTypeDef],
-        "Restrictions": NotRequired[RestrictionsOutputTypeDef],
+        "Restrictions": NotRequired[RestrictionsTypeDef],
         "WebACLId": NotRequired[str],
         "HttpVersion": NotRequired[HttpVersionType],
         "IsIPV6Enabled": NotRequired[bool],
         "ContinuousDeploymentPolicyId": NotRequired[str],
         "Staging": NotRequired[bool],
     },
 )
@@ -3693,54 +3056,30 @@
     "DistributionSummaryTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
-        "Aliases": AliasesOutputTypeDef,
-        "Origins": OriginsOutputTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
-        "CacheBehaviors": CacheBehaviorsOutputTypeDef,
-        "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
+        "Aliases": AliasesTypeDef,
+        "Origins": OriginsTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
+        "CacheBehaviors": CacheBehaviorsTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
         "ViewerCertificate": ViewerCertificateTypeDef,
-        "Restrictions": RestrictionsOutputTypeDef,
+        "Restrictions": RestrictionsTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "Staging": bool,
-        "OriginGroups": NotRequired[OriginGroupsOutputTypeDef],
-        "AliasICPRecordals": NotRequired[List[AliasICPRecordalTypeDef]],
-    },
-)
-DistributionConfigTypeDef = TypedDict(
-    "DistributionConfigTypeDef",
-    {
-        "CallerReference": str,
-        "Origins": OriginsTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
-        "Comment": str,
-        "Enabled": bool,
-        "Aliases": NotRequired[AliasesTypeDef],
-        "DefaultRootObject": NotRequired[str],
         "OriginGroups": NotRequired[OriginGroupsTypeDef],
-        "CacheBehaviors": NotRequired[CacheBehaviorsTypeDef],
-        "CustomErrorResponses": NotRequired[CustomErrorResponsesTypeDef],
-        "Logging": NotRequired[LoggingConfigTypeDef],
-        "PriceClass": NotRequired[PriceClassType],
-        "ViewerCertificate": NotRequired[ViewerCertificateTypeDef],
-        "Restrictions": NotRequired[RestrictionsTypeDef],
-        "WebACLId": NotRequired[str],
-        "HttpVersion": NotRequired[HttpVersionType],
-        "IsIPV6Enabled": NotRequired[bool],
-        "ContinuousDeploymentPolicyId": NotRequired[str],
-        "Staging": NotRequired[bool],
+        "AliasICPRecordals": NotRequired[List[AliasICPRecordalTypeDef]],
     },
 )
 CachePolicySummaryTypeDef = TypedDict(
     "CachePolicySummaryTypeDef",
     {
         "Type": CachePolicyTypeType,
         "CachePolicy": CachePolicyTypeDef,
@@ -3894,70 +3233,69 @@
     {
         "MaxItems": int,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[ResponseHeadersPolicySummaryTypeDef]],
     },
 )
+CreateDistributionRequestRequestTypeDef = TypedDict(
+    "CreateDistributionRequestRequestTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+    },
+)
+DistributionConfigWithTagsTypeDef = TypedDict(
+    "DistributionConfigWithTagsTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+        "Tags": TagsTypeDef,
+    },
+)
 DistributionTypeDef = TypedDict(
     "DistributionTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "InProgressInvalidationBatches": int,
         "DomainName": str,
-        "DistributionConfig": DistributionConfigOutputTypeDef,
+        "DistributionConfig": DistributionConfigTypeDef,
         "ActiveTrustedSigners": NotRequired[ActiveTrustedSignersTypeDef],
         "ActiveTrustedKeyGroups": NotRequired[ActiveTrustedKeyGroupsTypeDef],
         "AliasICPRecordals": NotRequired[List[AliasICPRecordalTypeDef]],
     },
 )
 GetDistributionConfigResultTypeDef = TypedDict(
     "GetDistributionConfigResultTypeDef",
     {
-        "DistributionConfig": DistributionConfigOutputTypeDef,
+        "DistributionConfig": DistributionConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateDistributionRequestRequestTypeDef = TypedDict(
+    "UpdateDistributionRequestRequestTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+        "Id": str,
+        "IfMatch": NotRequired[str],
+    },
+)
 DistributionListTypeDef = TypedDict(
     "DistributionListTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[DistributionSummaryTypeDef]],
     },
 )
-CreateDistributionRequestRequestTypeDef = TypedDict(
-    "CreateDistributionRequestRequestTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-    },
-)
-DistributionConfigUnionTypeDef = Union[DistributionConfigTypeDef, DistributionConfigOutputTypeDef]
-DistributionConfigWithTagsTypeDef = TypedDict(
-    "DistributionConfigWithTagsTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-        "Tags": TagsTypeDef,
-    },
-)
-UpdateDistributionRequestRequestTypeDef = TypedDict(
-    "UpdateDistributionRequestRequestTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-        "Id": str,
-        "IfMatch": NotRequired[str],
-    },
-)
 CachePolicyListTypeDef = TypedDict(
     "CachePolicyListTypeDef",
     {
         "MaxItems": int,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[CachePolicySummaryTypeDef]],
@@ -3982,14 +3320,20 @@
 ListResponseHeadersPoliciesResultTypeDef = TypedDict(
     "ListResponseHeadersPoliciesResultTypeDef",
     {
         "ResponseHeadersPolicyList": ResponseHeadersPolicyListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
+    "CreateDistributionWithTagsRequestRequestTypeDef",
+    {
+        "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
+    },
+)
 CopyDistributionResultTypeDef = TypedDict(
     "CopyDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4054,20 +3398,14 @@
 ListDistributionsResultTypeDef = TypedDict(
     "ListDistributionsResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
-    "CreateDistributionWithTagsRequestRequestTypeDef",
-    {
-        "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
-    },
-)
 ListCachePoliciesResultTypeDef = TypedDict(
     "ListCachePoliciesResultTypeDef",
     {
         "CachePolicyList": CachePolicyListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/type_defs.pyi` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/type_defs.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -63,48 +63,39 @@
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AliasICPRecordalTypeDef",
-    "AliasesOutputTypeDef",
     "AliasesTypeDef",
-    "CachedMethodsOutputTypeDef",
     "CachedMethodsTypeDef",
     "AssociateAliasRequestRequestTypeDef",
     "BlobTypeDef",
-    "TrustedKeyGroupsOutputTypeDef",
-    "TrustedSignersOutputTypeDef",
     "TrustedKeyGroupsTypeDef",
     "TrustedSignersTypeDef",
-    "CookieNamesOutputTypeDef",
     "CookieNamesTypeDef",
-    "HeadersOutputTypeDef",
     "HeadersTypeDef",
-    "QueryStringNamesOutputTypeDef",
     "QueryStringNamesTypeDef",
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     "CloudFrontOriginAccessIdentitySummaryTypeDef",
     "ConflictingAliasTypeDef",
     "ContentTypeProfileTypeDef",
-    "StagingDistributionDnsNamesOutputTypeDef",
     "StagingDistributionDnsNamesTypeDef",
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
     "SessionStickinessConfigTypeDef",
     "CopyDistributionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "KeyGroupConfigTypeDef",
     "ImportSourceTypeDef",
     "KeyValueStoreTypeDef",
     "OriginAccessControlConfigTypeDef",
     "PublicKeyConfigTypeDef",
     "CustomErrorResponseTypeDef",
     "OriginCustomHeaderTypeDef",
-    "OriginSslProtocolsOutputTypeDef",
     "OriginSslProtocolsTypeDef",
     "DeleteCachePolicyRequestRequestTypeDef",
     "DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "DeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     "DeleteDistributionRequestRequestTypeDef",
     "DeleteFieldLevelEncryptionConfigRequestRequestTypeDef",
     "DeleteFieldLevelEncryptionProfileRequestRequestTypeDef",
@@ -119,22 +110,19 @@
     "DeleteResponseHeadersPolicyRequestRequestTypeDef",
     "DeleteStreamingDistributionRequestRequestTypeDef",
     "DescribeFunctionRequestRequestTypeDef",
     "DescribeKeyValueStoreRequestRequestTypeDef",
     "LoggingConfigTypeDef",
     "ViewerCertificateTypeDef",
     "DistributionIdListTypeDef",
-    "FieldPatternsOutputTypeDef",
     "FieldPatternsTypeDef",
     "KinesisStreamConfigTypeDef",
-    "QueryStringCacheKeysOutputTypeDef",
     "QueryStringCacheKeysTypeDef",
     "FunctionAssociationTypeDef",
     "FunctionMetadataTypeDef",
-    "GeoRestrictionOutputTypeDef",
     "GeoRestrictionTypeDef",
     "GetCachePolicyConfigRequestRequestTypeDef",
     "GetCachePolicyRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyConfigRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyRequestRequestTypeDef",
@@ -144,29 +132,27 @@
     "GetFieldLevelEncryptionConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileRequestRequestTypeDef",
     "GetFieldLevelEncryptionRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
     "GetInvalidationRequestRequestTypeDef",
     "GetKeyGroupConfigRequestRequestTypeDef",
-    "KeyGroupConfigOutputTypeDef",
     "GetKeyGroupRequestRequestTypeDef",
     "GetMonitoringSubscriptionRequestRequestTypeDef",
     "GetOriginAccessControlConfigRequestRequestTypeDef",
     "GetOriginAccessControlRequestRequestTypeDef",
     "GetOriginRequestPolicyConfigRequestRequestTypeDef",
     "GetOriginRequestPolicyRequestRequestTypeDef",
     "GetPublicKeyConfigRequestRequestTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
     "GetRealtimeLogConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyRequestRequestTypeDef",
     "GetStreamingDistributionConfigRequestRequestTypeDef",
     "GetStreamingDistributionRequestRequestTypeDef",
-    "PathsOutputTypeDef",
     "PathsTypeDef",
     "InvalidationSummaryTypeDef",
     "KeyPairIdsTypeDef",
     "KeyValueStoreAssociationTypeDef",
     "LambdaFunctionAssociationTypeDef",
     "ListCachePoliciesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -191,29 +177,24 @@
     "ListPublicKeysRequestRequestTypeDef",
     "ListRealtimeLogConfigsRequestRequestTypeDef",
     "ListResponseHeadersPoliciesRequestRequestTypeDef",
     "ListStreamingDistributionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RealtimeMetricsSubscriptionConfigTypeDef",
     "OriginAccessControlSummaryTypeDef",
-    "StatusCodesOutputTypeDef",
     "StatusCodesTypeDef",
     "OriginGroupMemberTypeDef",
     "OriginShieldTypeDef",
     "S3OriginConfigTypeDef",
     "PublicKeySummaryTypeDef",
     "PublishFunctionRequestRequestTypeDef",
     "QueryArgProfileTypeDef",
-    "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
-    "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
-    "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
-    "ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     "ResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
     "ResponseHeadersPolicyContentTypeOptionsTypeDef",
     "ResponseHeadersPolicyCustomHeaderTypeDef",
     "ResponseHeadersPolicyFrameOptionsTypeDef",
     "ResponseHeadersPolicyReferrerPolicyTypeDef",
@@ -222,265 +203,208 @@
     "ResponseHeadersPolicyXSSProtectionTypeDef",
     "S3OriginTypeDef",
     "StreamingLoggingConfigTypeDef",
     "TagKeysTypeDef",
     "TagTypeDef",
     "UpdateDistributionWithStagingConfigRequestRequestTypeDef",
     "UpdateKeyValueStoreRequestRequestTypeDef",
-    "AllowedMethodsOutputTypeDef",
     "AllowedMethodsTypeDef",
     "TestFunctionRequestRequestTypeDef",
-    "CachePolicyCookiesConfigOutputTypeDef",
-    "CookiePreferenceOutputTypeDef",
-    "OriginRequestPolicyCookiesConfigOutputTypeDef",
     "CachePolicyCookiesConfigTypeDef",
     "CookiePreferenceTypeDef",
     "OriginRequestPolicyCookiesConfigTypeDef",
-    "CachePolicyHeadersConfigOutputTypeDef",
-    "OriginRequestPolicyHeadersConfigOutputTypeDef",
     "CachePolicyHeadersConfigTypeDef",
     "OriginRequestPolicyHeadersConfigTypeDef",
-    "CachePolicyQueryStringsConfigOutputTypeDef",
-    "OriginRequestPolicyQueryStringsConfigOutputTypeDef",
     "CachePolicyQueryStringsConfigTypeDef",
     "OriginRequestPolicyQueryStringsConfigTypeDef",
     "CloudFrontOriginAccessIdentityTypeDef",
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "CloudFrontOriginAccessIdentityListTypeDef",
     "ConflictingAliasesListTypeDef",
-    "ContentTypeProfilesOutputTypeDef",
     "ContentTypeProfilesTypeDef",
     "ContinuousDeploymentSingleWeightConfigTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
     "GetFunctionResultTypeDef",
     "CreateKeyGroupRequestRequestTypeDef",
+    "GetKeyGroupConfigResultTypeDef",
+    "KeyGroupTypeDef",
     "UpdateKeyGroupRequestRequestTypeDef",
     "CreateKeyValueStoreRequestRequestTypeDef",
     "CreateKeyValueStoreResultTypeDef",
     "DescribeKeyValueStoreResultTypeDef",
     "KeyValueStoreListTypeDef",
     "UpdateKeyValueStoreResultTypeDef",
     "CreateOriginAccessControlRequestRequestTypeDef",
     "GetOriginAccessControlConfigResultTypeDef",
     "OriginAccessControlTypeDef",
     "UpdateOriginAccessControlRequestRequestTypeDef",
     "CreatePublicKeyRequestRequestTypeDef",
     "GetPublicKeyConfigResultTypeDef",
     "PublicKeyTypeDef",
     "UpdatePublicKeyRequestRequestTypeDef",
-    "CustomErrorResponsesOutputTypeDef",
     "CustomErrorResponsesTypeDef",
-    "CustomHeadersOutputTypeDef",
     "CustomHeadersTypeDef",
-    "CustomOriginConfigOutputTypeDef",
     "CustomOriginConfigTypeDef",
     "ListDistributionsByCachePolicyIdResultTypeDef",
     "ListDistributionsByKeyGroupResultTypeDef",
     "ListDistributionsByOriginRequestPolicyIdResultTypeDef",
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
-    "EncryptionEntityOutputTypeDef",
     "EncryptionEntityTypeDef",
     "EndPointTypeDef",
-    "FunctionAssociationsOutputTypeDef",
     "FunctionAssociationsTypeDef",
-    "RestrictionsOutputTypeDef",
     "RestrictionsTypeDef",
     "GetDistributionRequestDistributionDeployedWaitTypeDef",
     "GetInvalidationRequestInvalidationCompletedWaitTypeDef",
     "GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
-    "GetKeyGroupConfigResultTypeDef",
-    "KeyGroupConfigUnionTypeDef",
-    "KeyGroupTypeDef",
-    "InvalidationBatchOutputTypeDef",
     "InvalidationBatchTypeDef",
     "InvalidationListTypeDef",
     "KGKeyPairIdsTypeDef",
     "SignerTypeDef",
-    "KeyValueStoreAssociationsOutputTypeDef",
     "KeyValueStoreAssociationsTypeDef",
-    "LambdaFunctionAssociationsOutputTypeDef",
     "LambdaFunctionAssociationsTypeDef",
     "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
     "ListDistributionsRequestListDistributionsPaginateTypeDef",
     "ListInvalidationsRequestListInvalidationsPaginateTypeDef",
     "ListKeyValueStoresRequestListKeyValueStoresPaginateTypeDef",
     "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "MonitoringSubscriptionTypeDef",
     "OriginAccessControlListTypeDef",
-    "OriginGroupFailoverCriteriaOutputTypeDef",
     "OriginGroupFailoverCriteriaTypeDef",
-    "OriginGroupMembersOutputTypeDef",
     "OriginGroupMembersTypeDef",
     "PublicKeyListTypeDef",
-    "QueryArgProfilesOutputTypeDef",
     "QueryArgProfilesTypeDef",
-    "ResponseHeadersPolicyCorsConfigOutputTypeDef",
     "ResponseHeadersPolicyCorsConfigTypeDef",
-    "ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyCustomHeadersConfigTypeDef",
-    "ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     "StreamingDistributionSummaryTypeDef",
-    "StreamingDistributionConfigOutputTypeDef",
     "StreamingDistributionConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "TagsOutputTypeDef",
     "TagsTypeDef",
-    "ForwardedValuesOutputTypeDef",
     "ForwardedValuesTypeDef",
-    "ParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
-    "OriginRequestPolicyConfigOutputTypeDef",
     "ParametersInCacheKeyAndForwardedToOriginTypeDef",
     "OriginRequestPolicyConfigTypeDef",
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     "GetCloudFrontOriginAccessIdentityResultTypeDef",
     "UpdateCloudFrontOriginAccessIdentityResultTypeDef",
     "ListCloudFrontOriginAccessIdentitiesResultTypeDef",
     "ListConflictingAliasesResultTypeDef",
-    "ContentTypeProfileConfigOutputTypeDef",
     "ContentTypeProfileConfigTypeDef",
     "TrafficConfigTypeDef",
+    "CreateKeyGroupResultTypeDef",
+    "GetKeyGroupResultTypeDef",
+    "KeyGroupSummaryTypeDef",
+    "UpdateKeyGroupResultTypeDef",
     "ListKeyValueStoresResultTypeDef",
     "CreateOriginAccessControlResultTypeDef",
     "GetOriginAccessControlResultTypeDef",
     "UpdateOriginAccessControlResultTypeDef",
     "CreatePublicKeyResultTypeDef",
     "GetPublicKeyResultTypeDef",
     "UpdatePublicKeyResultTypeDef",
-    "OriginOutputTypeDef",
     "OriginTypeDef",
-    "EncryptionEntitiesOutputTypeDef",
     "EncryptionEntitiesTypeDef",
     "CreateRealtimeLogConfigRequestRequestTypeDef",
     "RealtimeLogConfigTypeDef",
     "UpdateRealtimeLogConfigRequestRequestTypeDef",
-    "CreateKeyGroupResultTypeDef",
-    "GetKeyGroupResultTypeDef",
-    "KeyGroupSummaryTypeDef",
-    "UpdateKeyGroupResultTypeDef",
-    "InvalidationTypeDef",
     "CreateInvalidationRequestRequestTypeDef",
-    "InvalidationBatchUnionTypeDef",
+    "InvalidationTypeDef",
     "ListInvalidationsResultTypeDef",
     "ActiveTrustedKeyGroupsTypeDef",
     "ActiveTrustedSignersTypeDef",
-    "FunctionConfigOutputTypeDef",
     "FunctionConfigTypeDef",
     "CreateMonitoringSubscriptionRequestRequestTypeDef",
     "CreateMonitoringSubscriptionResultTypeDef",
     "GetMonitoringSubscriptionResultTypeDef",
     "ListOriginAccessControlsResultTypeDef",
-    "OriginGroupOutputTypeDef",
     "OriginGroupTypeDef",
     "ListPublicKeysResultTypeDef",
-    "QueryArgProfileConfigOutputTypeDef",
     "QueryArgProfileConfigTypeDef",
-    "ResponseHeadersPolicyConfigOutputTypeDef",
     "ResponseHeadersPolicyConfigTypeDef",
     "StreamingDistributionListTypeDef",
-    "GetStreamingDistributionConfigResultTypeDef",
     "CreateStreamingDistributionRequestRequestTypeDef",
-    "StreamingDistributionConfigUnionTypeDef",
+    "GetStreamingDistributionConfigResultTypeDef",
     "UpdateStreamingDistributionRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "StreamingDistributionConfigWithTagsTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TagsUnionTypeDef",
-    "CacheBehaviorOutputTypeDef",
-    "DefaultCacheBehaviorOutputTypeDef",
     "CacheBehaviorTypeDef",
     "DefaultCacheBehaviorTypeDef",
-    "CachePolicyConfigOutputTypeDef",
-    "GetOriginRequestPolicyConfigResultTypeDef",
-    "OriginRequestPolicyTypeDef",
     "CachePolicyConfigTypeDef",
     "CreateOriginRequestPolicyRequestRequestTypeDef",
-    "OriginRequestPolicyConfigUnionTypeDef",
+    "GetOriginRequestPolicyConfigResultTypeDef",
+    "OriginRequestPolicyTypeDef",
     "UpdateOriginRequestPolicyRequestRequestTypeDef",
-    "ContinuousDeploymentPolicyConfigOutputTypeDef",
     "ContinuousDeploymentPolicyConfigTypeDef",
-    "OriginsOutputTypeDef",
+    "KeyGroupListTypeDef",
     "OriginsTypeDef",
-    "FieldLevelEncryptionProfileConfigOutputTypeDef",
-    "FieldLevelEncryptionProfileSummaryTypeDef",
     "FieldLevelEncryptionProfileConfigTypeDef",
+    "FieldLevelEncryptionProfileSummaryTypeDef",
     "CreateRealtimeLogConfigResultTypeDef",
     "GetRealtimeLogConfigResultTypeDef",
     "RealtimeLogConfigsTypeDef",
     "UpdateRealtimeLogConfigResultTypeDef",
-    "KeyGroupListTypeDef",
     "CreateInvalidationResultTypeDef",
     "GetInvalidationResultTypeDef",
     "StreamingDistributionTypeDef",
-    "FunctionSummaryTypeDef",
     "CreateFunctionRequestRequestTypeDef",
-    "FunctionConfigUnionTypeDef",
+    "FunctionSummaryTypeDef",
     "UpdateFunctionRequestRequestTypeDef",
-    "OriginGroupsOutputTypeDef",
     "OriginGroupsTypeDef",
-    "FieldLevelEncryptionConfigOutputTypeDef",
-    "FieldLevelEncryptionSummaryTypeDef",
     "FieldLevelEncryptionConfigTypeDef",
+    "FieldLevelEncryptionSummaryTypeDef",
+    "CreateResponseHeadersPolicyRequestRequestTypeDef",
     "GetResponseHeadersPolicyConfigResultTypeDef",
     "ResponseHeadersPolicyTypeDef",
-    "CreateResponseHeadersPolicyRequestRequestTypeDef",
-    "ResponseHeadersPolicyConfigUnionTypeDef",
     "UpdateResponseHeadersPolicyRequestRequestTypeDef",
     "ListStreamingDistributionsResultTypeDef",
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
-    "CacheBehaviorsOutputTypeDef",
     "CacheBehaviorsTypeDef",
     "CachePolicyTypeDef",
+    "CreateCachePolicyRequestRequestTypeDef",
     "GetCachePolicyConfigResultTypeDef",
+    "UpdateCachePolicyRequestRequestTypeDef",
     "CreateOriginRequestPolicyResultTypeDef",
     "GetOriginRequestPolicyResultTypeDef",
     "OriginRequestPolicySummaryTypeDef",
     "UpdateOriginRequestPolicyResultTypeDef",
-    "CachePolicyConfigUnionTypeDef",
-    "CreateCachePolicyRequestRequestTypeDef",
-    "UpdateCachePolicyRequestRequestTypeDef",
     "ContinuousDeploymentPolicyTypeDef",
-    "GetContinuousDeploymentPolicyConfigResultTypeDef",
-    "ContinuousDeploymentPolicyConfigUnionTypeDef",
     "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
+    "GetContinuousDeploymentPolicyConfigResultTypeDef",
     "UpdateContinuousDeploymentPolicyRequestRequestTypeDef",
+    "ListKeyGroupsResultTypeDef",
+    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "FieldLevelEncryptionProfileTypeDef",
     "GetFieldLevelEncryptionProfileConfigResultTypeDef",
-    "FieldLevelEncryptionProfileListTypeDef",
-    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
-    "FieldLevelEncryptionProfileConfigUnionTypeDef",
     "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
+    "FieldLevelEncryptionProfileListTypeDef",
     "ListRealtimeLogConfigsResultTypeDef",
-    "ListKeyGroupsResultTypeDef",
     "CreateStreamingDistributionResultTypeDef",
     "CreateStreamingDistributionWithTagsResultTypeDef",
     "GetStreamingDistributionResultTypeDef",
     "UpdateStreamingDistributionResultTypeDef",
     "CreateFunctionResultTypeDef",
     "DescribeFunctionResultTypeDef",
     "FunctionListTypeDef",
     "PublishFunctionResultTypeDef",
     "TestResultTypeDef",
     "UpdateFunctionResultTypeDef",
+    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "FieldLevelEncryptionTypeDef",
     "GetFieldLevelEncryptionConfigResultTypeDef",
-    "FieldLevelEncryptionListTypeDef",
-    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
-    "FieldLevelEncryptionConfigUnionTypeDef",
     "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    "FieldLevelEncryptionListTypeDef",
     "CreateResponseHeadersPolicyResultTypeDef",
     "GetResponseHeadersPolicyResultTypeDef",
     "ResponseHeadersPolicySummaryTypeDef",
     "UpdateResponseHeadersPolicyResultTypeDef",
-    "DistributionConfigOutputTypeDef",
-    "DistributionSummaryTypeDef",
     "DistributionConfigTypeDef",
+    "DistributionSummaryTypeDef",
     "CachePolicySummaryTypeDef",
     "CreateCachePolicyResultTypeDef",
     "GetCachePolicyResultTypeDef",
     "UpdateCachePolicyResultTypeDef",
     "OriginRequestPolicyListTypeDef",
     "ContinuousDeploymentPolicySummaryTypeDef",
     "CreateContinuousDeploymentPolicyResultTypeDef",
@@ -493,146 +417,94 @@
     "ListFunctionsResultTypeDef",
     "TestFunctionResultTypeDef",
     "CreateFieldLevelEncryptionConfigResultTypeDef",
     "GetFieldLevelEncryptionResultTypeDef",
     "UpdateFieldLevelEncryptionConfigResultTypeDef",
     "ListFieldLevelEncryptionConfigsResultTypeDef",
     "ResponseHeadersPolicyListTypeDef",
-    "DistributionTypeDef",
-    "GetDistributionConfigResultTypeDef",
-    "DistributionListTypeDef",
     "CreateDistributionRequestRequestTypeDef",
-    "DistributionConfigUnionTypeDef",
     "DistributionConfigWithTagsTypeDef",
+    "DistributionTypeDef",
+    "GetDistributionConfigResultTypeDef",
     "UpdateDistributionRequestRequestTypeDef",
+    "DistributionListTypeDef",
     "CachePolicyListTypeDef",
     "ListOriginRequestPoliciesResultTypeDef",
     "ContinuousDeploymentPolicyListTypeDef",
     "ListResponseHeadersPoliciesResultTypeDef",
+    "CreateDistributionWithTagsRequestRequestTypeDef",
     "CopyDistributionResultTypeDef",
     "CreateDistributionResultTypeDef",
     "CreateDistributionWithTagsResultTypeDef",
     "GetDistributionResultTypeDef",
     "UpdateDistributionResultTypeDef",
     "UpdateDistributionWithStagingConfigResultTypeDef",
     "ListDistributionsByRealtimeLogConfigResultTypeDef",
     "ListDistributionsByWebACLIdResultTypeDef",
     "ListDistributionsResultTypeDef",
-    "CreateDistributionWithTagsRequestRequestTypeDef",
     "ListCachePoliciesResultTypeDef",
     "ListContinuousDeploymentPoliciesResultTypeDef",
 )
 
 AliasICPRecordalTypeDef = TypedDict(
     "AliasICPRecordalTypeDef",
     {
         "CNAME": NotRequired[str],
         "ICPRecordalStatus": NotRequired[ICPRecordalStatusType],
     },
 )
-AliasesOutputTypeDef = TypedDict(
-    "AliasesOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
 AliasesTypeDef = TypedDict(
     "AliasesTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[str]],
-    },
-)
-CachedMethodsOutputTypeDef = TypedDict(
-    "CachedMethodsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[MethodType],
+        "Items": NotRequired[List[str]],
     },
 )
 CachedMethodsTypeDef = TypedDict(
     "CachedMethodsTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[MethodType],
+        "Items": List[MethodType],
     },
 )
 AssociateAliasRequestRequestTypeDef = TypedDict(
     "AssociateAliasRequestRequestTypeDef",
     {
         "TargetDistributionId": str,
         "Alias": str,
     },
 )
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
-TrustedKeyGroupsOutputTypeDef = TypedDict(
-    "TrustedKeyGroupsOutputTypeDef",
-    {
-        "Enabled": bool,
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
-TrustedSignersOutputTypeDef = TypedDict(
-    "TrustedSignersOutputTypeDef",
-    {
-        "Enabled": bool,
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
 TrustedKeyGroupsTypeDef = TypedDict(
     "TrustedKeyGroupsTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
-        "Items": NotRequired[Sequence[str]],
+        "Items": NotRequired[List[str]],
     },
 )
 TrustedSignersTypeDef = TypedDict(
     "TrustedSignersTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
-        "Items": NotRequired[Sequence[str]],
-    },
-)
-CookieNamesOutputTypeDef = TypedDict(
-    "CookieNamesOutputTypeDef",
-    {
-        "Quantity": int,
         "Items": NotRequired[List[str]],
     },
 )
 CookieNamesTypeDef = TypedDict(
     "CookieNamesTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[str]],
-    },
-)
-HeadersOutputTypeDef = TypedDict(
-    "HeadersOutputTypeDef",
-    {
-        "Quantity": int,
         "Items": NotRequired[List[str]],
     },
 )
 HeadersTypeDef = TypedDict(
     "HeadersTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[str]],
-    },
-)
-QueryStringNamesOutputTypeDef = TypedDict(
-    "QueryStringNamesOutputTypeDef",
-    {
-        "Quantity": int,
         "Items": NotRequired[List[str]],
     },
 )
 QueryStringNamesTypeDef = TypedDict(
     "QueryStringNamesTypeDef",
     {
         "Quantity": int,
@@ -666,21 +538,14 @@
     "ContentTypeProfileTypeDef",
     {
         "Format": Literal["URLEncoded"],
         "ContentType": str,
         "ProfileId": NotRequired[str],
     },
 )
-StagingDistributionDnsNamesOutputTypeDef = TypedDict(
-    "StagingDistributionDnsNamesOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
 StagingDistributionDnsNamesTypeDef = TypedDict(
     "StagingDistributionDnsNamesTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[str]],
     },
 )
@@ -775,26 +640,19 @@
 OriginCustomHeaderTypeDef = TypedDict(
     "OriginCustomHeaderTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
-OriginSslProtocolsOutputTypeDef = TypedDict(
-    "OriginSslProtocolsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[SslProtocolType],
-    },
-)
 OriginSslProtocolsTypeDef = TypedDict(
     "OriginSslProtocolsTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[SslProtocolType],
+        "Items": List[SslProtocolType],
     },
 )
 DeleteCachePolicyRequestRequestTypeDef = TypedDict(
     "DeleteCachePolicyRequestRequestTypeDef",
     {
         "Id": str,
         "IfMatch": NotRequired[str],
@@ -945,47 +803,33 @@
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[str]],
     },
 )
-FieldPatternsOutputTypeDef = TypedDict(
-    "FieldPatternsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
 FieldPatternsTypeDef = TypedDict(
     "FieldPatternsTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[str]],
     },
 )
 KinesisStreamConfigTypeDef = TypedDict(
     "KinesisStreamConfigTypeDef",
     {
         "RoleARN": str,
         "StreamARN": str,
     },
 )
-QueryStringCacheKeysOutputTypeDef = TypedDict(
-    "QueryStringCacheKeysOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
 QueryStringCacheKeysTypeDef = TypedDict(
     "QueryStringCacheKeysTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[str]],
+        "Items": NotRequired[List[str]],
     },
 )
 FunctionAssociationTypeDef = TypedDict(
     "FunctionAssociationTypeDef",
     {
         "FunctionARN": str,
         "EventType": EventTypeType,
@@ -996,28 +840,20 @@
     {
         "FunctionARN": str,
         "LastModifiedTime": datetime,
         "Stage": NotRequired[FunctionStageType],
         "CreatedTime": NotRequired[datetime],
     },
 )
-GeoRestrictionOutputTypeDef = TypedDict(
-    "GeoRestrictionOutputTypeDef",
-    {
-        "RestrictionType": GeoRestrictionTypeType,
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
 GeoRestrictionTypeDef = TypedDict(
     "GeoRestrictionTypeDef",
     {
         "RestrictionType": GeoRestrictionTypeType,
         "Quantity": int,
-        "Items": NotRequired[Sequence[str]],
+        "Items": NotRequired[List[str]],
     },
 )
 GetCachePolicyConfigRequestRequestTypeDef = TypedDict(
     "GetCachePolicyConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
@@ -1111,22 +947,14 @@
 )
 GetKeyGroupConfigRequestRequestTypeDef = TypedDict(
     "GetKeyGroupConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
-KeyGroupConfigOutputTypeDef = TypedDict(
-    "KeyGroupConfigOutputTypeDef",
-    {
-        "Name": str,
-        "Items": List[str],
-        "Comment": NotRequired[str],
-    },
-)
 GetKeyGroupRequestRequestTypeDef = TypedDict(
     "GetKeyGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 GetMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
@@ -1198,21 +1026,14 @@
 )
 GetStreamingDistributionRequestRequestTypeDef = TypedDict(
     "GetStreamingDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
-PathsOutputTypeDef = TypedDict(
-    "PathsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
 PathsTypeDef = TypedDict(
     "PathsTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[str]],
     },
 )
@@ -1448,26 +1269,19 @@
         "Description": str,
         "Name": str,
         "SigningProtocol": Literal["sigv4"],
         "SigningBehavior": OriginAccessControlSigningBehaviorsType,
         "OriginAccessControlOriginType": OriginAccessControlOriginTypesType,
     },
 )
-StatusCodesOutputTypeDef = TypedDict(
-    "StatusCodesOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[int],
-    },
-)
 StatusCodesTypeDef = TypedDict(
     "StatusCodesTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[int],
+        "Items": List[int],
     },
 )
 OriginGroupMemberTypeDef = TypedDict(
     "OriginGroupMemberTypeDef",
     {
         "OriginId": str,
     },
@@ -1505,63 +1319,35 @@
 QueryArgProfileTypeDef = TypedDict(
     "QueryArgProfileTypeDef",
     {
         "QueryArg": str,
         "ProfileId": str,
     },
 )
-ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[str],
-    },
-)
 ResponseHeadersPolicyAccessControlAllowHeadersTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[str],
     },
 )
-ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[ResponseHeadersPolicyAccessControlAllowMethodsValuesType],
-    },
-)
 ResponseHeadersPolicyAccessControlAllowMethodsTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[ResponseHeadersPolicyAccessControlAllowMethodsValuesType],
     },
 )
-ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[str],
-    },
-)
 ResponseHeadersPolicyAccessControlAllowOriginsTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[str],
     },
 )
-ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[str]],
-    },
-)
 ResponseHeadersPolicyAccessControlExposeHeadersTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[str]],
     },
 )
@@ -1671,60 +1457,31 @@
     "UpdateKeyValueStoreRequestRequestTypeDef",
     {
         "Name": str,
         "Comment": str,
         "IfMatch": str,
     },
 )
-AllowedMethodsOutputTypeDef = TypedDict(
-    "AllowedMethodsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[MethodType],
-        "CachedMethods": NotRequired[CachedMethodsOutputTypeDef],
-    },
-)
 AllowedMethodsTypeDef = TypedDict(
     "AllowedMethodsTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[MethodType],
+        "Items": List[MethodType],
         "CachedMethods": NotRequired[CachedMethodsTypeDef],
     },
 )
 TestFunctionRequestRequestTypeDef = TypedDict(
     "TestFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
         "EventObject": BlobTypeDef,
         "Stage": NotRequired[FunctionStageType],
     },
 )
-CachePolicyCookiesConfigOutputTypeDef = TypedDict(
-    "CachePolicyCookiesConfigOutputTypeDef",
-    {
-        "CookieBehavior": CachePolicyCookieBehaviorType,
-        "Cookies": NotRequired[CookieNamesOutputTypeDef],
-    },
-)
-CookiePreferenceOutputTypeDef = TypedDict(
-    "CookiePreferenceOutputTypeDef",
-    {
-        "Forward": ItemSelectionType,
-        "WhitelistedNames": NotRequired[CookieNamesOutputTypeDef],
-    },
-)
-OriginRequestPolicyCookiesConfigOutputTypeDef = TypedDict(
-    "OriginRequestPolicyCookiesConfigOutputTypeDef",
-    {
-        "CookieBehavior": OriginRequestPolicyCookieBehaviorType,
-        "Cookies": NotRequired[CookieNamesOutputTypeDef],
-    },
-)
 CachePolicyCookiesConfigTypeDef = TypedDict(
     "CachePolicyCookiesConfigTypeDef",
     {
         "CookieBehavior": CachePolicyCookieBehaviorType,
         "Cookies": NotRequired[CookieNamesTypeDef],
     },
 )
@@ -1738,56 +1495,28 @@
 OriginRequestPolicyCookiesConfigTypeDef = TypedDict(
     "OriginRequestPolicyCookiesConfigTypeDef",
     {
         "CookieBehavior": OriginRequestPolicyCookieBehaviorType,
         "Cookies": NotRequired[CookieNamesTypeDef],
     },
 )
-CachePolicyHeadersConfigOutputTypeDef = TypedDict(
-    "CachePolicyHeadersConfigOutputTypeDef",
-    {
-        "HeaderBehavior": CachePolicyHeaderBehaviorType,
-        "Headers": NotRequired[HeadersOutputTypeDef],
-    },
-)
-OriginRequestPolicyHeadersConfigOutputTypeDef = TypedDict(
-    "OriginRequestPolicyHeadersConfigOutputTypeDef",
-    {
-        "HeaderBehavior": OriginRequestPolicyHeaderBehaviorType,
-        "Headers": NotRequired[HeadersOutputTypeDef],
-    },
-)
 CachePolicyHeadersConfigTypeDef = TypedDict(
     "CachePolicyHeadersConfigTypeDef",
     {
         "HeaderBehavior": CachePolicyHeaderBehaviorType,
         "Headers": NotRequired[HeadersTypeDef],
     },
 )
 OriginRequestPolicyHeadersConfigTypeDef = TypedDict(
     "OriginRequestPolicyHeadersConfigTypeDef",
     {
         "HeaderBehavior": OriginRequestPolicyHeaderBehaviorType,
         "Headers": NotRequired[HeadersTypeDef],
     },
 )
-CachePolicyQueryStringsConfigOutputTypeDef = TypedDict(
-    "CachePolicyQueryStringsConfigOutputTypeDef",
-    {
-        "QueryStringBehavior": CachePolicyQueryStringBehaviorType,
-        "QueryStrings": NotRequired[QueryStringNamesOutputTypeDef],
-    },
-)
-OriginRequestPolicyQueryStringsConfigOutputTypeDef = TypedDict(
-    "OriginRequestPolicyQueryStringsConfigOutputTypeDef",
-    {
-        "QueryStringBehavior": OriginRequestPolicyQueryStringBehaviorType,
-        "QueryStrings": NotRequired[QueryStringNamesOutputTypeDef],
-    },
-)
 CachePolicyQueryStringsConfigTypeDef = TypedDict(
     "CachePolicyQueryStringsConfigTypeDef",
     {
         "QueryStringBehavior": CachePolicyQueryStringBehaviorType,
         "QueryStrings": NotRequired[QueryStringNamesTypeDef],
     },
 )
@@ -1838,21 +1567,14 @@
     {
         "NextMarker": NotRequired[str],
         "MaxItems": NotRequired[int],
         "Quantity": NotRequired[int],
         "Items": NotRequired[List[ConflictingAliasTypeDef]],
     },
 )
-ContentTypeProfilesOutputTypeDef = TypedDict(
-    "ContentTypeProfilesOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[ContentTypeProfileTypeDef]],
-    },
-)
 ContentTypeProfilesTypeDef = TypedDict(
     "ContentTypeProfilesTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[ContentTypeProfileTypeDef]],
     },
 )
@@ -1888,14 +1610,30 @@
 )
 CreateKeyGroupRequestRequestTypeDef = TypedDict(
     "CreateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
     },
 )
+GetKeyGroupConfigResultTypeDef = TypedDict(
+    "GetKeyGroupConfigResultTypeDef",
+    {
+        "KeyGroupConfig": KeyGroupConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+KeyGroupTypeDef = TypedDict(
+    "KeyGroupTypeDef",
+    {
+        "Id": str,
+        "LastModifiedTime": datetime,
+        "KeyGroupConfig": KeyGroupConfigTypeDef,
+    },
+)
 UpdateKeyGroupRequestRequestTypeDef = TypedDict(
     "UpdateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
         "Id": str,
         "IfMatch": NotRequired[str],
     },
@@ -1997,51 +1735,26 @@
     "UpdatePublicKeyRequestRequestTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
         "Id": str,
         "IfMatch": NotRequired[str],
     },
 )
-CustomErrorResponsesOutputTypeDef = TypedDict(
-    "CustomErrorResponsesOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[CustomErrorResponseTypeDef]],
-    },
-)
 CustomErrorResponsesTypeDef = TypedDict(
     "CustomErrorResponsesTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[CustomErrorResponseTypeDef]],
-    },
-)
-CustomHeadersOutputTypeDef = TypedDict(
-    "CustomHeadersOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[OriginCustomHeaderTypeDef]],
+        "Items": NotRequired[List[CustomErrorResponseTypeDef]],
     },
 )
 CustomHeadersTypeDef = TypedDict(
     "CustomHeadersTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[OriginCustomHeaderTypeDef]],
-    },
-)
-CustomOriginConfigOutputTypeDef = TypedDict(
-    "CustomOriginConfigOutputTypeDef",
-    {
-        "HTTPPort": int,
-        "HTTPSPort": int,
-        "OriginProtocolPolicy": OriginProtocolPolicyType,
-        "OriginSslProtocols": NotRequired[OriginSslProtocolsOutputTypeDef],
-        "OriginReadTimeout": NotRequired[int],
-        "OriginKeepaliveTimeout": NotRequired[int],
+        "Items": NotRequired[List[OriginCustomHeaderTypeDef]],
     },
 )
 CustomOriginConfigTypeDef = TypedDict(
     "CustomOriginConfigTypeDef",
     {
         "HTTPPort": int,
         "HTTPSPort": int,
@@ -2075,22 +1788,14 @@
 ListDistributionsByResponseHeadersPolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-EncryptionEntityOutputTypeDef = TypedDict(
-    "EncryptionEntityOutputTypeDef",
-    {
-        "PublicKeyId": str,
-        "ProviderId": str,
-        "FieldPatterns": FieldPatternsOutputTypeDef,
-    },
-)
 EncryptionEntityTypeDef = TypedDict(
     "EncryptionEntityTypeDef",
     {
         "PublicKeyId": str,
         "ProviderId": str,
         "FieldPatterns": FieldPatternsTypeDef,
     },
@@ -2098,32 +1803,19 @@
 EndPointTypeDef = TypedDict(
     "EndPointTypeDef",
     {
         "StreamType": str,
         "KinesisStreamConfig": NotRequired[KinesisStreamConfigTypeDef],
     },
 )
-FunctionAssociationsOutputTypeDef = TypedDict(
-    "FunctionAssociationsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[FunctionAssociationTypeDef]],
-    },
-)
 FunctionAssociationsTypeDef = TypedDict(
     "FunctionAssociationsTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[FunctionAssociationTypeDef]],
-    },
-)
-RestrictionsOutputTypeDef = TypedDict(
-    "RestrictionsOutputTypeDef",
-    {
-        "GeoRestriction": GeoRestrictionOutputTypeDef,
+        "Items": NotRequired[List[FunctionAssociationTypeDef]],
     },
 )
 RestrictionsTypeDef = TypedDict(
     "RestrictionsTypeDef",
     {
         "GeoRestriction": GeoRestrictionTypeDef,
     },
@@ -2146,38 +1838,14 @@
 GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef = TypedDict(
     "GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
     {
         "Id": str,
         "WaiterConfig": NotRequired[WaiterConfigTypeDef],
     },
 )
-GetKeyGroupConfigResultTypeDef = TypedDict(
-    "GetKeyGroupConfigResultTypeDef",
-    {
-        "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-KeyGroupConfigUnionTypeDef = Union[KeyGroupConfigTypeDef, KeyGroupConfigOutputTypeDef]
-KeyGroupTypeDef = TypedDict(
-    "KeyGroupTypeDef",
-    {
-        "Id": str,
-        "LastModifiedTime": datetime,
-        "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
-    },
-)
-InvalidationBatchOutputTypeDef = TypedDict(
-    "InvalidationBatchOutputTypeDef",
-    {
-        "Paths": PathsOutputTypeDef,
-        "CallerReference": str,
-    },
-)
 InvalidationBatchTypeDef = TypedDict(
     "InvalidationBatchTypeDef",
     {
         "Paths": PathsTypeDef,
         "CallerReference": str,
     },
 )
@@ -2202,40 +1870,26 @@
 SignerTypeDef = TypedDict(
     "SignerTypeDef",
     {
         "AwsAccountNumber": NotRequired[str],
         "KeyPairIds": NotRequired[KeyPairIdsTypeDef],
     },
 )
-KeyValueStoreAssociationsOutputTypeDef = TypedDict(
-    "KeyValueStoreAssociationsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[KeyValueStoreAssociationTypeDef]],
-    },
-)
 KeyValueStoreAssociationsTypeDef = TypedDict(
     "KeyValueStoreAssociationsTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[KeyValueStoreAssociationTypeDef]],
     },
 )
-LambdaFunctionAssociationsOutputTypeDef = TypedDict(
-    "LambdaFunctionAssociationsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[LambdaFunctionAssociationTypeDef]],
-    },
-)
 LambdaFunctionAssociationsTypeDef = TypedDict(
     "LambdaFunctionAssociationsTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[LambdaFunctionAssociationTypeDef]],
+        "Items": NotRequired[List[LambdaFunctionAssociationTypeDef]],
     },
 )
 ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef = TypedDict(
     "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
@@ -2279,112 +1933,64 @@
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[OriginAccessControlSummaryTypeDef]],
     },
 )
-OriginGroupFailoverCriteriaOutputTypeDef = TypedDict(
-    "OriginGroupFailoverCriteriaOutputTypeDef",
-    {
-        "StatusCodes": StatusCodesOutputTypeDef,
-    },
-)
 OriginGroupFailoverCriteriaTypeDef = TypedDict(
     "OriginGroupFailoverCriteriaTypeDef",
     {
         "StatusCodes": StatusCodesTypeDef,
     },
 )
-OriginGroupMembersOutputTypeDef = TypedDict(
-    "OriginGroupMembersOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[OriginGroupMemberTypeDef],
-    },
-)
 OriginGroupMembersTypeDef = TypedDict(
     "OriginGroupMembersTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[OriginGroupMemberTypeDef],
+        "Items": List[OriginGroupMemberTypeDef],
     },
 )
 PublicKeyListTypeDef = TypedDict(
     "PublicKeyListTypeDef",
     {
         "MaxItems": int,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[PublicKeySummaryTypeDef]],
     },
 )
-QueryArgProfilesOutputTypeDef = TypedDict(
-    "QueryArgProfilesOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[QueryArgProfileTypeDef]],
-    },
-)
 QueryArgProfilesTypeDef = TypedDict(
     "QueryArgProfilesTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[QueryArgProfileTypeDef]],
     },
 )
-ResponseHeadersPolicyCorsConfigOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyCorsConfigOutputTypeDef",
-    {
-        "AccessControlAllowOrigins": ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef,
-        "AccessControlAllowHeaders": ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef,
-        "AccessControlAllowMethods": ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef,
-        "AccessControlAllowCredentials": bool,
-        "OriginOverride": bool,
-        "AccessControlExposeHeaders": NotRequired[
-            ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef
-        ],
-        "AccessControlMaxAgeSec": NotRequired[int],
-    },
-)
 ResponseHeadersPolicyCorsConfigTypeDef = TypedDict(
     "ResponseHeadersPolicyCorsConfigTypeDef",
     {
         "AccessControlAllowOrigins": ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
         "AccessControlAllowHeaders": ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
         "AccessControlAllowMethods": ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
         "AccessControlAllowCredentials": bool,
         "OriginOverride": bool,
         "AccessControlExposeHeaders": NotRequired[
             ResponseHeadersPolicyAccessControlExposeHeadersTypeDef
         ],
         "AccessControlMaxAgeSec": NotRequired[int],
     },
 )
-ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[ResponseHeadersPolicyCustomHeaderTypeDef]],
-    },
-)
 ResponseHeadersPolicyCustomHeadersConfigTypeDef = TypedDict(
     "ResponseHeadersPolicyCustomHeadersConfigTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[ResponseHeadersPolicyCustomHeaderTypeDef]],
     },
 )
-ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[ResponseHeadersPolicyRemoveHeaderTypeDef]],
-    },
-)
 ResponseHeadersPolicyRemoveHeadersConfigTypeDef = TypedDict(
     "ResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[ResponseHeadersPolicyRemoveHeaderTypeDef]],
     },
 )
@@ -2404,34 +2010,21 @@
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
         "S3Origin": S3OriginTypeDef,
-        "Aliases": AliasesOutputTypeDef,
-        "TrustedSigners": TrustedSignersOutputTypeDef,
+        "Aliases": AliasesTypeDef,
+        "TrustedSigners": TrustedSignersTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
     },
 )
-StreamingDistributionConfigOutputTypeDef = TypedDict(
-    "StreamingDistributionConfigOutputTypeDef",
-    {
-        "CallerReference": str,
-        "S3Origin": S3OriginTypeDef,
-        "Comment": str,
-        "TrustedSigners": TrustedSignersOutputTypeDef,
-        "Enabled": bool,
-        "Aliases": NotRequired[AliasesOutputTypeDef],
-        "Logging": NotRequired[StreamingLoggingConfigTypeDef],
-        "PriceClass": NotRequired[PriceClassType],
-    },
-)
 StreamingDistributionConfigTypeDef = TypedDict(
     "StreamingDistributionConfigTypeDef",
     {
         "CallerReference": str,
         "S3Origin": S3OriginTypeDef,
         "Comment": str,
         "TrustedSigners": TrustedSignersTypeDef,
@@ -2444,64 +2037,29 @@
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "TagKeys": TagKeysTypeDef,
     },
 )
-TagsOutputTypeDef = TypedDict(
-    "TagsOutputTypeDef",
-    {
-        "Items": NotRequired[List[TagTypeDef]],
-    },
-)
 TagsTypeDef = TypedDict(
     "TagsTypeDef",
     {
         "Items": NotRequired[Sequence[TagTypeDef]],
     },
 )
-ForwardedValuesOutputTypeDef = TypedDict(
-    "ForwardedValuesOutputTypeDef",
-    {
-        "QueryString": bool,
-        "Cookies": CookiePreferenceOutputTypeDef,
-        "Headers": NotRequired[HeadersOutputTypeDef],
-        "QueryStringCacheKeys": NotRequired[QueryStringCacheKeysOutputTypeDef],
-    },
-)
 ForwardedValuesTypeDef = TypedDict(
     "ForwardedValuesTypeDef",
     {
         "QueryString": bool,
         "Cookies": CookiePreferenceTypeDef,
         "Headers": NotRequired[HeadersTypeDef],
         "QueryStringCacheKeys": NotRequired[QueryStringCacheKeysTypeDef],
     },
 )
-ParametersInCacheKeyAndForwardedToOriginOutputTypeDef = TypedDict(
-    "ParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
-    {
-        "EnableAcceptEncodingGzip": bool,
-        "HeadersConfig": CachePolicyHeadersConfigOutputTypeDef,
-        "CookiesConfig": CachePolicyCookiesConfigOutputTypeDef,
-        "QueryStringsConfig": CachePolicyQueryStringsConfigOutputTypeDef,
-        "EnableAcceptEncodingBrotli": NotRequired[bool],
-    },
-)
-OriginRequestPolicyConfigOutputTypeDef = TypedDict(
-    "OriginRequestPolicyConfigOutputTypeDef",
-    {
-        "Name": str,
-        "HeadersConfig": OriginRequestPolicyHeadersConfigOutputTypeDef,
-        "CookiesConfig": OriginRequestPolicyCookiesConfigOutputTypeDef,
-        "QueryStringsConfig": OriginRequestPolicyQueryStringsConfigOutputTypeDef,
-        "Comment": NotRequired[str],
-    },
-)
 ParametersInCacheKeyAndForwardedToOriginTypeDef = TypedDict(
     "ParametersInCacheKeyAndForwardedToOriginTypeDef",
     {
         "EnableAcceptEncodingGzip": bool,
         "HeadersConfig": CachePolicyHeadersConfigTypeDef,
         "CookiesConfig": CachePolicyCookiesConfigTypeDef,
         "QueryStringsConfig": CachePolicyQueryStringsConfigTypeDef,
@@ -2553,21 +2111,14 @@
 ListConflictingAliasesResultTypeDef = TypedDict(
     "ListConflictingAliasesResultTypeDef",
     {
         "ConflictingAliasesList": ConflictingAliasesListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ContentTypeProfileConfigOutputTypeDef = TypedDict(
-    "ContentTypeProfileConfigOutputTypeDef",
-    {
-        "ForwardWhenContentTypeIsUnknown": bool,
-        "ContentTypeProfiles": NotRequired[ContentTypeProfilesOutputTypeDef],
-    },
-)
 ContentTypeProfileConfigTypeDef = TypedDict(
     "ContentTypeProfileConfigTypeDef",
     {
         "ForwardWhenContentTypeIsUnknown": bool,
         "ContentTypeProfiles": NotRequired[ContentTypeProfilesTypeDef],
     },
 )
@@ -2575,14 +2126,45 @@
     "TrafficConfigTypeDef",
     {
         "Type": ContinuousDeploymentPolicyTypeType,
         "SingleWeightConfig": NotRequired[ContinuousDeploymentSingleWeightConfigTypeDef],
         "SingleHeaderConfig": NotRequired[ContinuousDeploymentSingleHeaderConfigTypeDef],
     },
 )
+CreateKeyGroupResultTypeDef = TypedDict(
+    "CreateKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "Location": str,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetKeyGroupResultTypeDef = TypedDict(
+    "GetKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+KeyGroupSummaryTypeDef = TypedDict(
+    "KeyGroupSummaryTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+    },
+)
+UpdateKeyGroupResultTypeDef = TypedDict(
+    "UpdateKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListKeyValueStoresResultTypeDef = TypedDict(
     "ListKeyValueStoresResultTypeDef",
     {
         "KeyValueStoreList": KeyValueStoreListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2632,29 +2214,14 @@
     "UpdatePublicKeyResultTypeDef",
     {
         "PublicKey": PublicKeyTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-OriginOutputTypeDef = TypedDict(
-    "OriginOutputTypeDef",
-    {
-        "Id": str,
-        "DomainName": str,
-        "OriginPath": NotRequired[str],
-        "CustomHeaders": NotRequired[CustomHeadersOutputTypeDef],
-        "S3OriginConfig": NotRequired[S3OriginConfigTypeDef],
-        "CustomOriginConfig": NotRequired[CustomOriginConfigOutputTypeDef],
-        "ConnectionAttempts": NotRequired[int],
-        "ConnectionTimeout": NotRequired[int],
-        "OriginShield": NotRequired[OriginShieldTypeDef],
-        "OriginAccessControlId": NotRequired[str],
-    },
-)
 OriginTypeDef = TypedDict(
     "OriginTypeDef",
     {
         "Id": str,
         "DomainName": str,
         "OriginPath": NotRequired[str],
         "CustomHeaders": NotRequired[CustomHeadersTypeDef],
@@ -2662,21 +2229,14 @@
         "CustomOriginConfig": NotRequired[CustomOriginConfigTypeDef],
         "ConnectionAttempts": NotRequired[int],
         "ConnectionTimeout": NotRequired[int],
         "OriginShield": NotRequired[OriginShieldTypeDef],
         "OriginAccessControlId": NotRequired[str],
     },
 )
-EncryptionEntitiesOutputTypeDef = TypedDict(
-    "EncryptionEntitiesOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[EncryptionEntityOutputTypeDef]],
-    },
-)
 EncryptionEntitiesTypeDef = TypedDict(
     "EncryptionEntitiesTypeDef",
     {
         "Quantity": int,
         "Items": NotRequired[Sequence[EncryptionEntityTypeDef]],
     },
 )
@@ -2705,62 +2265,30 @@
         "EndPoints": NotRequired[Sequence[EndPointTypeDef]],
         "Fields": NotRequired[Sequence[str]],
         "Name": NotRequired[str],
         "ARN": NotRequired[str],
         "SamplingRate": NotRequired[int],
     },
 )
-CreateKeyGroupResultTypeDef = TypedDict(
-    "CreateKeyGroupResultTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-        "Location": str,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-GetKeyGroupResultTypeDef = TypedDict(
-    "GetKeyGroupResultTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-KeyGroupSummaryTypeDef = TypedDict(
-    "KeyGroupSummaryTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-    },
-)
-UpdateKeyGroupResultTypeDef = TypedDict(
-    "UpdateKeyGroupResultTypeDef",
+CreateInvalidationRequestRequestTypeDef = TypedDict(
+    "CreateInvalidationRequestRequestTypeDef",
     {
-        "KeyGroup": KeyGroupTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DistributionId": str,
+        "InvalidationBatch": InvalidationBatchTypeDef,
     },
 )
 InvalidationTypeDef = TypedDict(
     "InvalidationTypeDef",
     {
         "Id": str,
         "Status": str,
         "CreateTime": datetime,
-        "InvalidationBatch": InvalidationBatchOutputTypeDef,
-    },
-)
-CreateInvalidationRequestRequestTypeDef = TypedDict(
-    "CreateInvalidationRequestRequestTypeDef",
-    {
-        "DistributionId": str,
         "InvalidationBatch": InvalidationBatchTypeDef,
     },
 )
-InvalidationBatchUnionTypeDef = Union[InvalidationBatchTypeDef, InvalidationBatchOutputTypeDef]
 ListInvalidationsResultTypeDef = TypedDict(
     "ListInvalidationsResultTypeDef",
     {
         "InvalidationList": InvalidationListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2776,22 +2304,14 @@
     "ActiveTrustedSignersTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
         "Items": NotRequired[List[SignerTypeDef]],
     },
 )
-FunctionConfigOutputTypeDef = TypedDict(
-    "FunctionConfigOutputTypeDef",
-    {
-        "Comment": str,
-        "Runtime": FunctionRuntimeType,
-        "KeyValueStoreAssociations": NotRequired[KeyValueStoreAssociationsOutputTypeDef],
-    },
-)
 FunctionConfigTypeDef = TypedDict(
     "FunctionConfigTypeDef",
     {
         "Comment": str,
         "Runtime": FunctionRuntimeType,
         "KeyValueStoreAssociations": NotRequired[KeyValueStoreAssociationsTypeDef],
     },
@@ -2820,22 +2340,14 @@
 ListOriginAccessControlsResultTypeDef = TypedDict(
     "ListOriginAccessControlsResultTypeDef",
     {
         "OriginAccessControlList": OriginAccessControlListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-OriginGroupOutputTypeDef = TypedDict(
-    "OriginGroupOutputTypeDef",
-    {
-        "Id": str,
-        "FailoverCriteria": OriginGroupFailoverCriteriaOutputTypeDef,
-        "Members": OriginGroupMembersOutputTypeDef,
-    },
-)
 OriginGroupTypeDef = TypedDict(
     "OriginGroupTypeDef",
     {
         "Id": str,
         "FailoverCriteria": OriginGroupFailoverCriteriaTypeDef,
         "Members": OriginGroupMembersTypeDef,
     },
@@ -2843,42 +2355,21 @@
 ListPublicKeysResultTypeDef = TypedDict(
     "ListPublicKeysResultTypeDef",
     {
         "PublicKeyList": PublicKeyListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-QueryArgProfileConfigOutputTypeDef = TypedDict(
-    "QueryArgProfileConfigOutputTypeDef",
-    {
-        "ForwardWhenQueryArgProfileIsUnknown": bool,
-        "QueryArgProfiles": NotRequired[QueryArgProfilesOutputTypeDef],
-    },
-)
 QueryArgProfileConfigTypeDef = TypedDict(
     "QueryArgProfileConfigTypeDef",
     {
         "ForwardWhenQueryArgProfileIsUnknown": bool,
         "QueryArgProfiles": NotRequired[QueryArgProfilesTypeDef],
     },
 )
-ResponseHeadersPolicyConfigOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyConfigOutputTypeDef",
-    {
-        "Name": str,
-        "Comment": NotRequired[str],
-        "CorsConfig": NotRequired[ResponseHeadersPolicyCorsConfigOutputTypeDef],
-        "SecurityHeadersConfig": NotRequired[ResponseHeadersPolicySecurityHeadersConfigTypeDef],
-        "ServerTimingHeadersConfig": NotRequired[
-            ResponseHeadersPolicyServerTimingHeadersConfigTypeDef
-        ],
-        "CustomHeadersConfig": NotRequired[ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef],
-        "RemoveHeadersConfig": NotRequired[ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef],
-    },
-)
 ResponseHeadersPolicyConfigTypeDef = TypedDict(
     "ResponseHeadersPolicyConfigTypeDef",
     {
         "Name": str,
         "Comment": NotRequired[str],
         "CorsConfig": NotRequired[ResponseHeadersPolicyCorsConfigTypeDef],
         "SecurityHeadersConfig": NotRequired[ResponseHeadersPolicySecurityHeadersConfigTypeDef],
@@ -2896,43 +2387,40 @@
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[StreamingDistributionSummaryTypeDef]],
     },
 )
-GetStreamingDistributionConfigResultTypeDef = TypedDict(
-    "GetStreamingDistributionConfigResultTypeDef",
+CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
+    "CreateStreamingDistributionRequestRequestTypeDef",
     {
-        "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
     },
 )
-CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
-    "CreateStreamingDistributionRequestRequestTypeDef",
+GetStreamingDistributionConfigResultTypeDef = TypedDict(
+    "GetStreamingDistributionConfigResultTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-StreamingDistributionConfigUnionTypeDef = Union[
-    StreamingDistributionConfigTypeDef, StreamingDistributionConfigOutputTypeDef
-]
 UpdateStreamingDistributionRequestRequestTypeDef = TypedDict(
     "UpdateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
         "Id": str,
         "IfMatch": NotRequired[str],
     },
 )
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
-        "Tags": TagsOutputTypeDef,
+        "Tags": TagsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 StreamingDistributionConfigWithTagsTypeDef = TypedDict(
     "StreamingDistributionConfigWithTagsTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
@@ -2942,62 +2430,14 @@
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "Tags": TagsTypeDef,
     },
 )
-TagsUnionTypeDef = Union[TagsTypeDef, TagsOutputTypeDef]
-CacheBehaviorOutputTypeDef = TypedDict(
-    "CacheBehaviorOutputTypeDef",
-    {
-        "PathPattern": str,
-        "TargetOriginId": str,
-        "ViewerProtocolPolicy": ViewerProtocolPolicyType,
-        "TrustedSigners": NotRequired[TrustedSignersOutputTypeDef],
-        "TrustedKeyGroups": NotRequired[TrustedKeyGroupsOutputTypeDef],
-        "AllowedMethods": NotRequired[AllowedMethodsOutputTypeDef],
-        "SmoothStreaming": NotRequired[bool],
-        "Compress": NotRequired[bool],
-        "LambdaFunctionAssociations": NotRequired[LambdaFunctionAssociationsOutputTypeDef],
-        "FunctionAssociations": NotRequired[FunctionAssociationsOutputTypeDef],
-        "FieldLevelEncryptionId": NotRequired[str],
-        "RealtimeLogConfigArn": NotRequired[str],
-        "CachePolicyId": NotRequired[str],
-        "OriginRequestPolicyId": NotRequired[str],
-        "ResponseHeadersPolicyId": NotRequired[str],
-        "ForwardedValues": NotRequired[ForwardedValuesOutputTypeDef],
-        "MinTTL": NotRequired[int],
-        "DefaultTTL": NotRequired[int],
-        "MaxTTL": NotRequired[int],
-    },
-)
-DefaultCacheBehaviorOutputTypeDef = TypedDict(
-    "DefaultCacheBehaviorOutputTypeDef",
-    {
-        "TargetOriginId": str,
-        "ViewerProtocolPolicy": ViewerProtocolPolicyType,
-        "TrustedSigners": NotRequired[TrustedSignersOutputTypeDef],
-        "TrustedKeyGroups": NotRequired[TrustedKeyGroupsOutputTypeDef],
-        "AllowedMethods": NotRequired[AllowedMethodsOutputTypeDef],
-        "SmoothStreaming": NotRequired[bool],
-        "Compress": NotRequired[bool],
-        "LambdaFunctionAssociations": NotRequired[LambdaFunctionAssociationsOutputTypeDef],
-        "FunctionAssociations": NotRequired[FunctionAssociationsOutputTypeDef],
-        "FieldLevelEncryptionId": NotRequired[str],
-        "RealtimeLogConfigArn": NotRequired[str],
-        "CachePolicyId": NotRequired[str],
-        "OriginRequestPolicyId": NotRequired[str],
-        "ResponseHeadersPolicyId": NotRequired[str],
-        "ForwardedValues": NotRequired[ForwardedValuesOutputTypeDef],
-        "MinTTL": NotRequired[int],
-        "DefaultTTL": NotRequired[int],
-        "MaxTTL": NotRequired[int],
-    },
-)
 CacheBehaviorTypeDef = TypedDict(
     "CacheBehaviorTypeDef",
     {
         "PathPattern": str,
         "TargetOriginId": str,
         "ViewerProtocolPolicy": ViewerProtocolPolicyType,
         "TrustedSigners": NotRequired[TrustedSignersTypeDef],
@@ -3037,127 +2477,96 @@
         "ResponseHeadersPolicyId": NotRequired[str],
         "ForwardedValues": NotRequired[ForwardedValuesTypeDef],
         "MinTTL": NotRequired[int],
         "DefaultTTL": NotRequired[int],
         "MaxTTL": NotRequired[int],
     },
 )
-CachePolicyConfigOutputTypeDef = TypedDict(
-    "CachePolicyConfigOutputTypeDef",
+CachePolicyConfigTypeDef = TypedDict(
+    "CachePolicyConfigTypeDef",
     {
         "Name": str,
         "MinTTL": int,
         "Comment": NotRequired[str],
         "DefaultTTL": NotRequired[int],
         "MaxTTL": NotRequired[int],
         "ParametersInCacheKeyAndForwardedToOrigin": NotRequired[
-            ParametersInCacheKeyAndForwardedToOriginOutputTypeDef
+            ParametersInCacheKeyAndForwardedToOriginTypeDef
         ],
     },
 )
+CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
+    "CreateOriginRequestPolicyRequestRequestTypeDef",
+    {
+        "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
+    },
+)
 GetOriginRequestPolicyConfigResultTypeDef = TypedDict(
     "GetOriginRequestPolicyConfigResultTypeDef",
     {
-        "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
+        "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 OriginRequestPolicyTypeDef = TypedDict(
     "OriginRequestPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
-    },
-)
-CachePolicyConfigTypeDef = TypedDict(
-    "CachePolicyConfigTypeDef",
-    {
-        "Name": str,
-        "MinTTL": int,
-        "Comment": NotRequired[str],
-        "DefaultTTL": NotRequired[int],
-        "MaxTTL": NotRequired[int],
-        "ParametersInCacheKeyAndForwardedToOrigin": NotRequired[
-            ParametersInCacheKeyAndForwardedToOriginTypeDef
-        ],
-    },
-)
-CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
-    "CreateOriginRequestPolicyRequestRequestTypeDef",
-    {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
     },
 )
-OriginRequestPolicyConfigUnionTypeDef = Union[
-    OriginRequestPolicyConfigTypeDef, OriginRequestPolicyConfigOutputTypeDef
-]
 UpdateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "UpdateOriginRequestPolicyRequestRequestTypeDef",
     {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
         "Id": str,
         "IfMatch": NotRequired[str],
     },
 )
-ContinuousDeploymentPolicyConfigOutputTypeDef = TypedDict(
-    "ContinuousDeploymentPolicyConfigOutputTypeDef",
-    {
-        "StagingDistributionDnsNames": StagingDistributionDnsNamesOutputTypeDef,
-        "Enabled": bool,
-        "TrafficConfig": NotRequired[TrafficConfigTypeDef],
-    },
-)
 ContinuousDeploymentPolicyConfigTypeDef = TypedDict(
     "ContinuousDeploymentPolicyConfigTypeDef",
     {
         "StagingDistributionDnsNames": StagingDistributionDnsNamesTypeDef,
         "Enabled": bool,
         "TrafficConfig": NotRequired[TrafficConfigTypeDef],
     },
 )
-OriginsOutputTypeDef = TypedDict(
-    "OriginsOutputTypeDef",
+KeyGroupListTypeDef = TypedDict(
+    "KeyGroupListTypeDef",
     {
+        "MaxItems": int,
         "Quantity": int,
-        "Items": List[OriginOutputTypeDef],
+        "NextMarker": NotRequired[str],
+        "Items": NotRequired[List[KeyGroupSummaryTypeDef]],
     },
 )
 OriginsTypeDef = TypedDict(
     "OriginsTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[OriginTypeDef],
+        "Items": List[OriginTypeDef],
     },
 )
-FieldLevelEncryptionProfileConfigOutputTypeDef = TypedDict(
-    "FieldLevelEncryptionProfileConfigOutputTypeDef",
+FieldLevelEncryptionProfileConfigTypeDef = TypedDict(
+    "FieldLevelEncryptionProfileConfigTypeDef",
     {
         "Name": str,
         "CallerReference": str,
-        "EncryptionEntities": EncryptionEntitiesOutputTypeDef,
+        "EncryptionEntities": EncryptionEntitiesTypeDef,
         "Comment": NotRequired[str],
     },
 )
 FieldLevelEncryptionProfileSummaryTypeDef = TypedDict(
     "FieldLevelEncryptionProfileSummaryTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
         "Name": str,
-        "EncryptionEntities": EncryptionEntitiesOutputTypeDef,
-        "Comment": NotRequired[str],
-    },
-)
-FieldLevelEncryptionProfileConfigTypeDef = TypedDict(
-    "FieldLevelEncryptionProfileConfigTypeDef",
-    {
-        "Name": str,
-        "CallerReference": str,
         "EncryptionEntities": EncryptionEntitiesTypeDef,
         "Comment": NotRequired[str],
     },
 )
 CreateRealtimeLogConfigResultTypeDef = TypedDict(
     "CreateRealtimeLogConfigResultTypeDef",
     {
@@ -3185,23 +2594,14 @@
 UpdateRealtimeLogConfigResultTypeDef = TypedDict(
     "UpdateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-KeyGroupListTypeDef = TypedDict(
-    "KeyGroupListTypeDef",
-    {
-        "MaxItems": int,
-        "Quantity": int,
-        "NextMarker": NotRequired[str],
-        "Items": NotRequired[List[KeyGroupSummaryTypeDef]],
-    },
-)
 CreateInvalidationResultTypeDef = TypedDict(
     "CreateInvalidationResultTypeDef",
     {
         "Location": str,
         "Invalidation": InvalidationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3217,112 +2617,92 @@
     "StreamingDistributionTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "DomainName": str,
         "ActiveTrustedSigners": ActiveTrustedSignersTypeDef,
-        "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
+        "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
         "LastModifiedTime": NotRequired[datetime],
     },
 )
-FunctionSummaryTypeDef = TypedDict(
-    "FunctionSummaryTypeDef",
+CreateFunctionRequestRequestTypeDef = TypedDict(
+    "CreateFunctionRequestRequestTypeDef",
     {
         "Name": str,
-        "FunctionConfig": FunctionConfigOutputTypeDef,
-        "FunctionMetadata": FunctionMetadataTypeDef,
-        "Status": NotRequired[str],
+        "FunctionConfig": FunctionConfigTypeDef,
+        "FunctionCode": BlobTypeDef,
     },
 )
-CreateFunctionRequestRequestTypeDef = TypedDict(
-    "CreateFunctionRequestRequestTypeDef",
+FunctionSummaryTypeDef = TypedDict(
+    "FunctionSummaryTypeDef",
     {
         "Name": str,
         "FunctionConfig": FunctionConfigTypeDef,
-        "FunctionCode": BlobTypeDef,
+        "FunctionMetadata": FunctionMetadataTypeDef,
+        "Status": NotRequired[str],
     },
 )
-FunctionConfigUnionTypeDef = Union[FunctionConfigTypeDef, FunctionConfigOutputTypeDef]
 UpdateFunctionRequestRequestTypeDef = TypedDict(
     "UpdateFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
         "FunctionConfig": FunctionConfigTypeDef,
         "FunctionCode": BlobTypeDef,
     },
 )
-OriginGroupsOutputTypeDef = TypedDict(
-    "OriginGroupsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[OriginGroupOutputTypeDef]],
-    },
-)
 OriginGroupsTypeDef = TypedDict(
     "OriginGroupsTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[OriginGroupTypeDef]],
+        "Items": NotRequired[List[OriginGroupTypeDef]],
     },
 )
-FieldLevelEncryptionConfigOutputTypeDef = TypedDict(
-    "FieldLevelEncryptionConfigOutputTypeDef",
+FieldLevelEncryptionConfigTypeDef = TypedDict(
+    "FieldLevelEncryptionConfigTypeDef",
     {
         "CallerReference": str,
         "Comment": NotRequired[str],
-        "QueryArgProfileConfig": NotRequired[QueryArgProfileConfigOutputTypeDef],
-        "ContentTypeProfileConfig": NotRequired[ContentTypeProfileConfigOutputTypeDef],
+        "QueryArgProfileConfig": NotRequired[QueryArgProfileConfigTypeDef],
+        "ContentTypeProfileConfig": NotRequired[ContentTypeProfileConfigTypeDef],
     },
 )
 FieldLevelEncryptionSummaryTypeDef = TypedDict(
     "FieldLevelEncryptionSummaryTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
         "Comment": NotRequired[str],
-        "QueryArgProfileConfig": NotRequired[QueryArgProfileConfigOutputTypeDef],
-        "ContentTypeProfileConfig": NotRequired[ContentTypeProfileConfigOutputTypeDef],
+        "QueryArgProfileConfig": NotRequired[QueryArgProfileConfigTypeDef],
+        "ContentTypeProfileConfig": NotRequired[ContentTypeProfileConfigTypeDef],
     },
 )
-FieldLevelEncryptionConfigTypeDef = TypedDict(
-    "FieldLevelEncryptionConfigTypeDef",
+CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
+    "CreateResponseHeadersPolicyRequestRequestTypeDef",
     {
-        "CallerReference": str,
-        "Comment": NotRequired[str],
-        "QueryArgProfileConfig": NotRequired[QueryArgProfileConfigTypeDef],
-        "ContentTypeProfileConfig": NotRequired[ContentTypeProfileConfigTypeDef],
+        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
     },
 )
 GetResponseHeadersPolicyConfigResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyConfigResultTypeDef",
     {
-        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
+        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ResponseHeadersPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
-    },
-)
-CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
-    "CreateResponseHeadersPolicyRequestRequestTypeDef",
-    {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
     },
 )
-ResponseHeadersPolicyConfigUnionTypeDef = Union[
-    ResponseHeadersPolicyConfigTypeDef, ResponseHeadersPolicyConfigOutputTypeDef
-]
 UpdateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
     "UpdateResponseHeadersPolicyRequestRequestTypeDef",
     {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
         "Id": str,
         "IfMatch": NotRequired[str],
     },
@@ -3336,44 +2716,51 @@
 )
 CreateStreamingDistributionWithTagsRequestRequestTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
     {
         "StreamingDistributionConfigWithTags": StreamingDistributionConfigWithTagsTypeDef,
     },
 )
-CacheBehaviorsOutputTypeDef = TypedDict(
-    "CacheBehaviorsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": NotRequired[List[CacheBehaviorOutputTypeDef]],
-    },
-)
 CacheBehaviorsTypeDef = TypedDict(
     "CacheBehaviorsTypeDef",
     {
         "Quantity": int,
-        "Items": NotRequired[Sequence[CacheBehaviorTypeDef]],
+        "Items": NotRequired[List[CacheBehaviorTypeDef]],
     },
 )
 CachePolicyTypeDef = TypedDict(
     "CachePolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
+    },
+)
+CreateCachePolicyRequestRequestTypeDef = TypedDict(
+    "CreateCachePolicyRequestRequestTypeDef",
+    {
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
     },
 )
 GetCachePolicyConfigResultTypeDef = TypedDict(
     "GetCachePolicyConfigResultTypeDef",
     {
-        "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateCachePolicyRequestRequestTypeDef = TypedDict(
+    "UpdateCachePolicyRequestRequestTypeDef",
+    {
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
+        "Id": str,
+        "IfMatch": NotRequired[str],
+    },
+)
 CreateOriginRequestPolicyResultTypeDef = TypedDict(
     "CreateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3398,118 +2785,97 @@
     "UpdateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CachePolicyConfigUnionTypeDef = Union[CachePolicyConfigTypeDef, CachePolicyConfigOutputTypeDef]
-CreateCachePolicyRequestRequestTypeDef = TypedDict(
-    "CreateCachePolicyRequestRequestTypeDef",
-    {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
-    },
-)
-UpdateCachePolicyRequestRequestTypeDef = TypedDict(
-    "UpdateCachePolicyRequestRequestTypeDef",
-    {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
-        "Id": str,
-        "IfMatch": NotRequired[str],
-    },
-)
 ContinuousDeploymentPolicyTypeDef = TypedDict(
     "ContinuousDeploymentPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
     },
 )
-GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
-    "GetContinuousDeploymentPolicyConfigResultTypeDef",
+CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
+    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
     },
 )
-ContinuousDeploymentPolicyConfigUnionTypeDef = Union[
-    ContinuousDeploymentPolicyConfigTypeDef, ContinuousDeploymentPolicyConfigOutputTypeDef
-]
-CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
-    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
+GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
+    "GetContinuousDeploymentPolicyConfigResultTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 UpdateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "UpdateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
         "Id": str,
         "IfMatch": NotRequired[str],
     },
 )
+ListKeyGroupsResultTypeDef = TypedDict(
+    "ListKeyGroupsResultTypeDef",
+    {
+        "KeyGroupList": KeyGroupListTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
+    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
+    {
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
+    },
+)
 FieldLevelEncryptionProfileTypeDef = TypedDict(
     "FieldLevelEncryptionProfileTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
     },
 )
 GetFieldLevelEncryptionProfileConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionProfileConfigResultTypeDef",
     {
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
+    "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
+    {
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
+        "Id": str,
+        "IfMatch": NotRequired[str],
+    },
+)
 FieldLevelEncryptionProfileListTypeDef = TypedDict(
     "FieldLevelEncryptionProfileListTypeDef",
     {
         "MaxItems": int,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[FieldLevelEncryptionProfileSummaryTypeDef]],
     },
 )
-CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
-    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
-    {
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
-    },
-)
-FieldLevelEncryptionProfileConfigUnionTypeDef = Union[
-    FieldLevelEncryptionProfileConfigTypeDef, FieldLevelEncryptionProfileConfigOutputTypeDef
-]
-UpdateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
-    "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
-    {
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
-        "Id": str,
-        "IfMatch": NotRequired[str],
-    },
-)
 ListRealtimeLogConfigsResultTypeDef = TypedDict(
     "ListRealtimeLogConfigsResultTypeDef",
     {
         "RealtimeLogConfigs": RealtimeLogConfigsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListKeyGroupsResultTypeDef = TypedDict(
-    "ListKeyGroupsResultTypeDef",
-    {
-        "KeyGroupList": KeyGroupListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 CreateStreamingDistributionResultTypeDef = TypedDict(
     "CreateStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3587,56 +2953,53 @@
     "UpdateFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    {
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+    },
+)
 FieldLevelEncryptionTypeDef = TypedDict(
     "FieldLevelEncryptionTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
     },
 )
 GetFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionConfigResultTypeDef",
     {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    {
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+        "Id": str,
+        "IfMatch": NotRequired[str],
+    },
+)
 FieldLevelEncryptionListTypeDef = TypedDict(
     "FieldLevelEncryptionListTypeDef",
     {
         "MaxItems": int,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[FieldLevelEncryptionSummaryTypeDef]],
     },
 )
-CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
-    {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
-    },
-)
-FieldLevelEncryptionConfigUnionTypeDef = Union[
-    FieldLevelEncryptionConfigTypeDef, FieldLevelEncryptionConfigOutputTypeDef
-]
-UpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
-    {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
-        "Id": str,
-        "IfMatch": NotRequired[str],
-    },
-)
 CreateResponseHeadersPolicyResultTypeDef = TypedDict(
     "CreateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3661,31 +3024,31 @@
     "UpdateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DistributionConfigOutputTypeDef = TypedDict(
-    "DistributionConfigOutputTypeDef",
+DistributionConfigTypeDef = TypedDict(
+    "DistributionConfigTypeDef",
     {
         "CallerReference": str,
-        "Origins": OriginsOutputTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
+        "Origins": OriginsTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
         "Comment": str,
         "Enabled": bool,
-        "Aliases": NotRequired[AliasesOutputTypeDef],
+        "Aliases": NotRequired[AliasesTypeDef],
         "DefaultRootObject": NotRequired[str],
-        "OriginGroups": NotRequired[OriginGroupsOutputTypeDef],
-        "CacheBehaviors": NotRequired[CacheBehaviorsOutputTypeDef],
-        "CustomErrorResponses": NotRequired[CustomErrorResponsesOutputTypeDef],
+        "OriginGroups": NotRequired[OriginGroupsTypeDef],
+        "CacheBehaviors": NotRequired[CacheBehaviorsTypeDef],
+        "CustomErrorResponses": NotRequired[CustomErrorResponsesTypeDef],
         "Logging": NotRequired[LoggingConfigTypeDef],
         "PriceClass": NotRequired[PriceClassType],
         "ViewerCertificate": NotRequired[ViewerCertificateTypeDef],
-        "Restrictions": NotRequired[RestrictionsOutputTypeDef],
+        "Restrictions": NotRequired[RestrictionsTypeDef],
         "WebACLId": NotRequired[str],
         "HttpVersion": NotRequired[HttpVersionType],
         "IsIPV6Enabled": NotRequired[bool],
         "ContinuousDeploymentPolicyId": NotRequired[str],
         "Staging": NotRequired[bool],
     },
 )
@@ -3693,54 +3056,30 @@
     "DistributionSummaryTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
-        "Aliases": AliasesOutputTypeDef,
-        "Origins": OriginsOutputTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
-        "CacheBehaviors": CacheBehaviorsOutputTypeDef,
-        "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
+        "Aliases": AliasesTypeDef,
+        "Origins": OriginsTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
+        "CacheBehaviors": CacheBehaviorsTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
         "ViewerCertificate": ViewerCertificateTypeDef,
-        "Restrictions": RestrictionsOutputTypeDef,
+        "Restrictions": RestrictionsTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "Staging": bool,
-        "OriginGroups": NotRequired[OriginGroupsOutputTypeDef],
-        "AliasICPRecordals": NotRequired[List[AliasICPRecordalTypeDef]],
-    },
-)
-DistributionConfigTypeDef = TypedDict(
-    "DistributionConfigTypeDef",
-    {
-        "CallerReference": str,
-        "Origins": OriginsTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
-        "Comment": str,
-        "Enabled": bool,
-        "Aliases": NotRequired[AliasesTypeDef],
-        "DefaultRootObject": NotRequired[str],
         "OriginGroups": NotRequired[OriginGroupsTypeDef],
-        "CacheBehaviors": NotRequired[CacheBehaviorsTypeDef],
-        "CustomErrorResponses": NotRequired[CustomErrorResponsesTypeDef],
-        "Logging": NotRequired[LoggingConfigTypeDef],
-        "PriceClass": NotRequired[PriceClassType],
-        "ViewerCertificate": NotRequired[ViewerCertificateTypeDef],
-        "Restrictions": NotRequired[RestrictionsTypeDef],
-        "WebACLId": NotRequired[str],
-        "HttpVersion": NotRequired[HttpVersionType],
-        "IsIPV6Enabled": NotRequired[bool],
-        "ContinuousDeploymentPolicyId": NotRequired[str],
-        "Staging": NotRequired[bool],
+        "AliasICPRecordals": NotRequired[List[AliasICPRecordalTypeDef]],
     },
 )
 CachePolicySummaryTypeDef = TypedDict(
     "CachePolicySummaryTypeDef",
     {
         "Type": CachePolicyTypeType,
         "CachePolicy": CachePolicyTypeDef,
@@ -3894,70 +3233,69 @@
     {
         "MaxItems": int,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[ResponseHeadersPolicySummaryTypeDef]],
     },
 )
+CreateDistributionRequestRequestTypeDef = TypedDict(
+    "CreateDistributionRequestRequestTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+    },
+)
+DistributionConfigWithTagsTypeDef = TypedDict(
+    "DistributionConfigWithTagsTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+        "Tags": TagsTypeDef,
+    },
+)
 DistributionTypeDef = TypedDict(
     "DistributionTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "InProgressInvalidationBatches": int,
         "DomainName": str,
-        "DistributionConfig": DistributionConfigOutputTypeDef,
+        "DistributionConfig": DistributionConfigTypeDef,
         "ActiveTrustedSigners": NotRequired[ActiveTrustedSignersTypeDef],
         "ActiveTrustedKeyGroups": NotRequired[ActiveTrustedKeyGroupsTypeDef],
         "AliasICPRecordals": NotRequired[List[AliasICPRecordalTypeDef]],
     },
 )
 GetDistributionConfigResultTypeDef = TypedDict(
     "GetDistributionConfigResultTypeDef",
     {
-        "DistributionConfig": DistributionConfigOutputTypeDef,
+        "DistributionConfig": DistributionConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateDistributionRequestRequestTypeDef = TypedDict(
+    "UpdateDistributionRequestRequestTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+        "Id": str,
+        "IfMatch": NotRequired[str],
+    },
+)
 DistributionListTypeDef = TypedDict(
     "DistributionListTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[DistributionSummaryTypeDef]],
     },
 )
-CreateDistributionRequestRequestTypeDef = TypedDict(
-    "CreateDistributionRequestRequestTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-    },
-)
-DistributionConfigUnionTypeDef = Union[DistributionConfigTypeDef, DistributionConfigOutputTypeDef]
-DistributionConfigWithTagsTypeDef = TypedDict(
-    "DistributionConfigWithTagsTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-        "Tags": TagsTypeDef,
-    },
-)
-UpdateDistributionRequestRequestTypeDef = TypedDict(
-    "UpdateDistributionRequestRequestTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-        "Id": str,
-        "IfMatch": NotRequired[str],
-    },
-)
 CachePolicyListTypeDef = TypedDict(
     "CachePolicyListTypeDef",
     {
         "MaxItems": int,
         "Quantity": int,
         "NextMarker": NotRequired[str],
         "Items": NotRequired[List[CachePolicySummaryTypeDef]],
@@ -3982,14 +3320,20 @@
 ListResponseHeadersPoliciesResultTypeDef = TypedDict(
     "ListResponseHeadersPoliciesResultTypeDef",
     {
         "ResponseHeadersPolicyList": ResponseHeadersPolicyListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
+    "CreateDistributionWithTagsRequestRequestTypeDef",
+    {
+        "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
+    },
+)
 CopyDistributionResultTypeDef = TypedDict(
     "CopyDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4054,20 +3398,14 @@
 ListDistributionsResultTypeDef = TypedDict(
     "ListDistributionsResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
-    "CreateDistributionWithTagsRequestRequestTypeDef",
-    {
-        "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
-    },
-)
 ListCachePoliciesResultTypeDef = TypedDict(
     "ListCachePoliciesResultTypeDef",
     {
         "CachePolicyList": CachePolicyListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/waiter.py` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront/waiter.pyi` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront.egg-info/PKG-INFO` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudfront
-Version: 1.34.110
-Summary: Type annotations for boto3.CloudFront 1.34.110 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.83
+Summary: Type annotations for boto3.CloudFront 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudfront)](https://pepy.tech/project/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.34.110](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_cloudfront-1.34.110/mypy_boto3_cloudfront.egg-info/SOURCES.txt` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cloudfront-1.34.110/setup.py` & `mypy-boto3-cloudfront-1.34.83/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudfront",
-    version="1.34.110",
+    version="1.34.83",
     packages=["mypy_boto3_cloudfront"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.CloudFront 1.34.110 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.CloudFront 1.34.83 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

