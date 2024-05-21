# Comparing `tmp/mypy_boto3_pi-1.34.110.tar.gz` & `tmp/mypy_boto3_pi-1.34.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_pi-1.34.110.tar", last modified: Tue May 21 19:32:45 2024, max compression
+gzip compressed data, was "mypy_boto3_pi-1.34.90.tar", last modified: Tue Apr 23 19:34:21 2024, max compression
```

## Comparing `mypy_boto3_pi-1.34.110.tar` & `mypy_boto3_pi-1.34.90.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:32:45.788809 mypy_boto3_pi-1.34.110/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-21 19:32:19.000000 mypy_boto3_pi-1.34.110/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-05-21 19:32:45.788809 mypy_boto3_pi-1.34.110/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10227 2024-05-21 19:32:19.000000 mypy_boto3_pi-1.34.110/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:32:45.788809 mypy_boto3_pi-1.34.110/mypy_boto3_pi/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-21 19:32:19.000000 mypy_boto3_pi-1.34.110/mypy_boto3_pi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-21 19:32:19.000000 mypy_boto3_pi-1.34.110/mypy_boto3_pi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-21 19:32:19.000000 mypy_boto3_pi-1.34.110/mypy_boto3_pi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-05-21 19:32:19.000000 mypy_boto3_pi-1.34.110/mypy_boto3_pi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12434 2024-05-21 19:32:19.000000 mypy_boto3_pi-1.34.110/mypy_boto3_pi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-05-21 19:32:19.000000 mypy_boto3_pi-1.34.110/mypy_boto3_pi/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-05-21 19:32:19.000000 mypy_boto3_pi-1.34.110/mypy_boto3_pi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:32:19.000000 mypy_boto3_pi-1.34.110/mypy_boto3_pi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14372 2024-05-21 19:32:20.000000 mypy_boto3_pi-1.34.110/mypy_boto3_pi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14372 2024-05-21 19:32:20.000000 mypy_boto3_pi-1.34.110/mypy_boto3_pi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 19:32:19.000000 mypy_boto3_pi-1.34.110/mypy_boto3_pi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:32:45.788809 mypy_boto3_pi-1.34.110/mypy_boto3_pi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-05-21 19:32:45.000000 mypy_boto3_pi-1.34.110/mypy_boto3_pi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-21 19:32:45.000000 mypy_boto3_pi-1.34.110/mypy_boto3_pi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:32:45.000000 mypy_boto3_pi-1.34.110/mypy_boto3_pi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:32:45.000000 mypy_boto3_pi-1.34.110/mypy_boto3_pi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-21 19:32:45.000000 mypy_boto3_pi-1.34.110/mypy_boto3_pi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 19:32:45.000000 mypy_boto3_pi-1.34.110/mypy_boto3_pi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 19:32:45.788809 mypy_boto3_pi-1.34.110/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-21 19:32:19.000000 mypy_boto3_pi-1.34.110/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:21.568578 mypy_boto3_pi-1.34.90/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 19:33:55.000000 mypy_boto3_pi-1.34.90/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-23 19:34:21.568578 mypy_boto3_pi-1.34.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10226 2024-04-23 19:33:55.000000 mypy_boto3_pi-1.34.90/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:21.568578 mypy_boto3_pi-1.34.90/mypy_boto3_pi/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-23 19:33:55.000000 mypy_boto3_pi-1.34.90/mypy_boto3_pi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-23 19:33:55.000000 mypy_boto3_pi-1.34.90/mypy_boto3_pi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-23 19:33:55.000000 mypy_boto3_pi-1.34.90/mypy_boto3_pi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-04-23 19:33:55.000000 mypy_boto3_pi-1.34.90/mypy_boto3_pi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-04-23 19:33:55.000000 mypy_boto3_pi-1.34.90/mypy_boto3_pi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-04-23 19:33:55.000000 mypy_boto3_pi-1.34.90/mypy_boto3_pi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-04-23 19:33:55.000000 mypy_boto3_pi-1.34.90/mypy_boto3_pi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:33:55.000000 mypy_boto3_pi-1.34.90/mypy_boto3_pi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14205 2024-04-23 19:33:55.000000 mypy_boto3_pi-1.34.90/mypy_boto3_pi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14205 2024-04-23 19:33:55.000000 mypy_boto3_pi-1.34.90/mypy_boto3_pi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 19:33:55.000000 mypy_boto3_pi-1.34.90/mypy_boto3_pi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:21.568578 mypy_boto3_pi-1.34.90/mypy_boto3_pi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-23 19:34:21.000000 mypy_boto3_pi-1.34.90/mypy_boto3_pi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-23 19:34:21.000000 mypy_boto3_pi-1.34.90/mypy_boto3_pi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:21.000000 mypy_boto3_pi-1.34.90/mypy_boto3_pi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:21.000000 mypy_boto3_pi-1.34.90/mypy_boto3_pi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 19:34:21.000000 mypy_boto3_pi-1.34.90/mypy_boto3_pi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 19:34:21.000000 mypy_boto3_pi-1.34.90/mypy_boto3_pi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:34:21.568578 mypy_boto3_pi-1.34.90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-23 19:33:55.000000 mypy_boto3_pi-1.34.90/setup.py
```

### Comparing `mypy_boto3_pi-1.34.110/LICENSE` & `mypy_boto3_pi-1.34.90/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_pi-1.34.110/PKG-INFO` & `mypy_boto3_pi-1.34.90/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pi
-Version: 1.34.110
-Summary: Type annotations for boto3.PI 1.34.110 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.90
+Summary: Type annotations for boto3.PI 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pi)](https://pepy.tech/project/mypy-boto3-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PI 1.34.110](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[boto3.PI 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
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
 [mypy-boto3-pi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_pi-1.34.110/README.md` & `mypy_boto3_pi-1.34.90/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pi)](https://pepy.tech/project/mypy-boto3-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PI 1.34.110](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[boto3.PI 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
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
 [mypy-boto3-pi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_pi-1.34.110/mypy_boto3_pi/__main__.py` & `mypy_boto3_pi-1.34.90/mypy_boto3_pi/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PI 1.34.110\n"
-        "Version:         1.34.110\n"
-        "Builder version: 7.24.0\n"
+        "Type annotations for boto3.PI 1.34.90\n"
+        "Version:         1.34.90\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.110")
+    print("1.34.90")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_pi-1.34.110/mypy_boto3_pi/client.py` & `mypy_boto3_pi-1.34.90/mypy_boto3_pi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import FineGrainedActionType, PeriodAlignmentType, ServiceTypeType, TextFormatType
+from .literals import PeriodAlignmentType, ServiceTypeType, TextFormatType
 from .type_defs import (
     CreatePerformanceAnalysisReportResponseTypeDef,
     DescribeDimensionKeysResponseTypeDef,
     DimensionGroupTypeDef,
     GetDimensionKeyDetailsResponseTypeDef,
     GetPerformanceAnalysisReportResponseTypeDef,
     GetResourceMetadataResponseTypeDef,
@@ -227,15 +227,14 @@
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
         Metrics: Sequence[str],
         MaxResults: int = ...,
         NextToken: str = ...,
-        AuthorizedActions: Sequence[FineGrainedActionType] = ...,
     ) -> ListAvailableResourceDimensionsResponseTypeDef:
         """
         Retrieve the dimensions that can be queried for each specified metric type on a
         specified DB
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.list_available_resource_dimensions)
```

### Comparing `mypy_boto3_pi-1.34.110/mypy_boto3_pi/client.pyi` & `mypy_boto3_pi-1.34.90/mypy_boto3_pi/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import FineGrainedActionType, PeriodAlignmentType, ServiceTypeType, TextFormatType
+from .literals import PeriodAlignmentType, ServiceTypeType, TextFormatType
 from .type_defs import (
     CreatePerformanceAnalysisReportResponseTypeDef,
     DescribeDimensionKeysResponseTypeDef,
     DimensionGroupTypeDef,
     GetDimensionKeyDetailsResponseTypeDef,
     GetPerformanceAnalysisReportResponseTypeDef,
     GetResourceMetadataResponseTypeDef,
@@ -224,15 +224,14 @@
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
         Metrics: Sequence[str],
         MaxResults: int = ...,
         NextToken: str = ...,
-        AuthorizedActions: Sequence[FineGrainedActionType] = ...,
     ) -> ListAvailableResourceDimensionsResponseTypeDef:
         """
         Retrieve the dimensions that can be queried for each specified metric type on a
         specified DB
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.list_available_resource_dimensions)
```

### Comparing `mypy_boto3_pi-1.34.110/mypy_boto3_pi/literals.py` & `mypy_boto3_pi-1.34.90/mypy_boto3_pi/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 __all__ = (
     "AcceptLanguageType",
     "AnalysisStatusType",
     "ContextTypeType",
     "DetailStatusType",
     "FeatureStatusType",
-    "FineGrainedActionType",
     "PeriodAlignmentType",
     "ServiceTypeType",
     "SeverityType",
     "TextFormatType",
     "PIServiceName",
     "ServiceName",
     "ResourceServiceName",
@@ -44,17 +43,14 @@
     "DISABLED",
     "DISABLED_PENDING_REBOOT",
     "ENABLED",
     "ENABLED_PENDING_REBOOT",
     "UNKNOWN",
     "UNSUPPORTED",
 ]
-FineGrainedActionType = Literal[
-    "DescribeDimensionKeys", "GetDimensionKeyDetails", "GetResourceMetrics"
-]
 PeriodAlignmentType = Literal["END_TIME", "START_TIME"]
 ServiceTypeType = Literal["DOCDB", "RDS"]
 SeverityType = Literal["HIGH", "LOW", "MEDIUM"]
 TextFormatType = Literal["MARKDOWN", "PLAIN_TEXT"]
 PIServiceName = Literal["pi"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -273,15 +269,14 @@
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
```

### Comparing `mypy_boto3_pi-1.34.110/mypy_boto3_pi/literals.pyi` & `mypy_boto3_pi-1.34.90/mypy_boto3_pi/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 __all__ = (
     "AcceptLanguageType",
     "AnalysisStatusType",
     "ContextTypeType",
     "DetailStatusType",
     "FeatureStatusType",
-    "FineGrainedActionType",
     "PeriodAlignmentType",
     "ServiceTypeType",
     "SeverityType",
     "TextFormatType",
     "PIServiceName",
     "ServiceName",
     "ResourceServiceName",
@@ -44,17 +43,14 @@
     "DISABLED",
     "DISABLED_PENDING_REBOOT",
     "ENABLED",
     "ENABLED_PENDING_REBOOT",
     "UNKNOWN",
     "UNSUPPORTED",
 ]
-FineGrainedActionType = Literal[
-    "DescribeDimensionKeys", "GetDimensionKeyDetails", "GetResourceMetrics"
-]
 PeriodAlignmentType = Literal["END_TIME", "START_TIME"]
 ServiceTypeType = Literal["DOCDB", "RDS"]
 SeverityType = Literal["HIGH", "LOW", "MEDIUM"]
 TextFormatType = Literal["MARKDOWN", "PLAIN_TEXT"]
 PIServiceName = Literal["pi"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -273,15 +269,14 @@
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
```

### Comparing `mypy_boto3_pi-1.34.110/mypy_boto3_pi/type_defs.py` & `mypy_boto3_pi-1.34.90/mypy_boto3_pi/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AnalysisStatusType,
     ContextTypeType,
     DetailStatusType,
     FeatureStatusType,
-    FineGrainedActionType,
     PeriodAlignmentType,
     ServiceTypeType,
     SeverityType,
     TextFormatType,
 )
 
 if sys.version_info >= (3, 12):
@@ -225,15 +224,14 @@
     "ListAvailableResourceDimensionsRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
         "Metrics": Sequence[str],
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
-        "AuthorizedActions": NotRequired[Sequence[FineGrainedActionType]],
     },
 )
 ListAvailableResourceMetricsRequestRequestTypeDef = TypedDict(
     "ListAvailableResourceMetricsRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
@@ -366,16 +364,16 @@
 DescribeDimensionKeysResponseTypeDef = TypedDict(
     "DescribeDimensionKeysResponseTypeDef",
     {
         "AlignedStartTime": datetime,
         "AlignedEndTime": datetime,
         "PartitionKeys": List[ResponsePartitionKeyTypeDef],
         "Keys": List[DimensionKeyDescriptionTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 DimensionGroupDetailTypeDef = TypedDict(
     "DimensionGroupDetailTypeDef",
     {
         "Group": NotRequired[str],
         "Dimensions": NotRequired[List[DimensionDetailTypeDef]],
@@ -396,31 +394,31 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListAvailableResourceMetricsResponseTypeDef = TypedDict(
     "ListAvailableResourceMetricsResponseTypeDef",
     {
         "Metrics": List[ResponseResourceMetricTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 MetricKeyDataPointsTypeDef = TypedDict(
     "MetricKeyDataPointsTypeDef",
     {
         "Key": NotRequired[ResponseResourceMetricKeyTypeDef],
         "DataPoints": NotRequired[List[DataPointTypeDef]],
     },
 )
 ListPerformanceAnalysisReportsResponseTypeDef = TypedDict(
     "ListPerformanceAnalysisReportsResponseTypeDef",
     {
         "AnalysisReports": List[AnalysisReportSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 InsightTypeDef = TypedDict(
     "InsightTypeDef",
     {
         "InsightId": str,
         "InsightType": NotRequired[str],
@@ -459,19 +457,19 @@
 GetResourceMetricsResponseTypeDef = TypedDict(
     "GetResourceMetricsResponseTypeDef",
     {
         "AlignedStartTime": datetime,
         "AlignedEndTime": datetime,
         "Identifier": str,
         "MetricList": List[MetricKeyDataPointsTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListAvailableResourceDimensionsResponseTypeDef = TypedDict(
     "ListAvailableResourceDimensionsResponseTypeDef",
     {
         "MetricDimensions": List[MetricDimensionGroupsTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy_boto3_pi-1.34.110/mypy_boto3_pi/type_defs.pyi` & `mypy_boto3_pi-1.34.90/mypy_boto3_pi/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AnalysisStatusType,
     ContextTypeType,
     DetailStatusType,
     FeatureStatusType,
-    FineGrainedActionType,
     PeriodAlignmentType,
     ServiceTypeType,
     SeverityType,
     TextFormatType,
 )
 
 if sys.version_info >= (3, 12):
@@ -225,15 +224,14 @@
     "ListAvailableResourceDimensionsRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
         "Metrics": Sequence[str],
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
-        "AuthorizedActions": NotRequired[Sequence[FineGrainedActionType]],
     },
 )
 ListAvailableResourceMetricsRequestRequestTypeDef = TypedDict(
     "ListAvailableResourceMetricsRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
@@ -366,16 +364,16 @@
 DescribeDimensionKeysResponseTypeDef = TypedDict(
     "DescribeDimensionKeysResponseTypeDef",
     {
         "AlignedStartTime": datetime,
         "AlignedEndTime": datetime,
         "PartitionKeys": List[ResponsePartitionKeyTypeDef],
         "Keys": List[DimensionKeyDescriptionTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 DimensionGroupDetailTypeDef = TypedDict(
     "DimensionGroupDetailTypeDef",
     {
         "Group": NotRequired[str],
         "Dimensions": NotRequired[List[DimensionDetailTypeDef]],
@@ -396,31 +394,31 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListAvailableResourceMetricsResponseTypeDef = TypedDict(
     "ListAvailableResourceMetricsResponseTypeDef",
     {
         "Metrics": List[ResponseResourceMetricTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 MetricKeyDataPointsTypeDef = TypedDict(
     "MetricKeyDataPointsTypeDef",
     {
         "Key": NotRequired[ResponseResourceMetricKeyTypeDef],
         "DataPoints": NotRequired[List[DataPointTypeDef]],
     },
 )
 ListPerformanceAnalysisReportsResponseTypeDef = TypedDict(
     "ListPerformanceAnalysisReportsResponseTypeDef",
     {
         "AnalysisReports": List[AnalysisReportSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 InsightTypeDef = TypedDict(
     "InsightTypeDef",
     {
         "InsightId": str,
         "InsightType": NotRequired[str],
@@ -459,19 +457,19 @@
 GetResourceMetricsResponseTypeDef = TypedDict(
     "GetResourceMetricsResponseTypeDef",
     {
         "AlignedStartTime": datetime,
         "AlignedEndTime": datetime,
         "Identifier": str,
         "MetricList": List[MetricKeyDataPointsTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListAvailableResourceDimensionsResponseTypeDef = TypedDict(
     "ListAvailableResourceDimensionsResponseTypeDef",
     {
         "MetricDimensions": List[MetricDimensionGroupsTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy_boto3_pi-1.34.110/mypy_boto3_pi.egg-info/PKG-INFO` & `mypy_boto3_pi-1.34.90/mypy_boto3_pi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pi
-Version: 1.34.110
-Summary: Type annotations for boto3.PI 1.34.110 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.90
+Summary: Type annotations for boto3.PI 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pi)](https://pepy.tech/project/mypy-boto3-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PI 1.34.110](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[boto3.PI 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
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
 [mypy-boto3-pi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_pi-1.34.110/mypy_boto3_pi.egg-info/SOURCES.txt` & `mypy_boto3_pi-1.34.90/mypy_boto3_pi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_pi-1.34.110/setup.py` & `mypy_boto3_pi-1.34.90/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pi",
-    version="1.34.110",
+    version="1.34.90",
     packages=["mypy_boto3_pi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.PI 1.34.110 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.PI 1.34.90 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

