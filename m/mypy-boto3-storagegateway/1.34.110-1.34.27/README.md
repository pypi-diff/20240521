# Comparing `tmp/mypy_boto3_storagegateway-1.34.110.tar.gz` & `tmp/mypy-boto3-storagegateway-1.34.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_storagegateway-1.34.110.tar", last modified: Tue May 21 19:32:46 2024, max compression
+gzip compressed data, was "mypy-boto3-storagegateway-1.34.27.tar", last modified: Wed Jan 24 20:33:19 2024, max compression
```

## Comparing `mypy_boto3_storagegateway-1.34.110.tar` & `mypy-boto3-storagegateway-1.34.27.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:32:46.500812 mypy_boto3_storagegateway-1.34.110/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-21 19:32:31.000000 mypy_boto3_storagegateway-1.34.110/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14472 2024-05-21 19:32:46.500812 mypy_boto3_storagegateway-1.34.110/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-05-21 19:32:31.000000 mypy_boto3_storagegateway-1.34.110/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:32:46.500812 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-21 19:32:31.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-21 19:32:31.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-21 19:32:31.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68503 2024-05-21 19:32:32.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    68500 2024-05-21 19:32:31.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-05-21 19:32:32.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-05-21 19:32:32.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13148 2024-05-21 19:32:32.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13136 2024-05-21 19:32:32.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:32:31.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    69649 2024-05-21 19:32:34.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    69649 2024-05-21 19:32:33.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 19:32:31.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:32:46.500812 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14472 2024-05-21 19:32:46.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-21 19:32:46.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:32:46.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:32:46.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-21 19:32:46.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 19:32:46.000000 mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 19:32:46.500812 mypy_boto3_storagegateway-1.34.110/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-21 19:32:31.000000 mypy_boto3_storagegateway-1.34.110/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:19.894194 mypy-boto3-storagegateway-1.34.27/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-24 20:33:04.000000 mypy-boto3-storagegateway-1.34.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14469 2024-01-24 20:33:19.894194 mypy-boto3-storagegateway-1.34.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12886 2024-01-24 20:33:04.000000 mypy-boto3-storagegateway-1.34.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:19.894194 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-01-24 20:33:04.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-01-24 20:33:04.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-24 20:33:04.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68473 2024-01-24 20:33:05.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68470 2024-01-24 20:33:05.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-01-24 20:33:05.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-01-24 20:33:05.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13148 2024-01-24 20:33:05.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13136 2024-01-24 20:33:05.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:04.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    68278 2024-01-24 20:33:07.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68278 2024-01-24 20:33:07.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-24 20:33:04.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:19.894194 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14469 2024-01-24 20:33:19.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-24 20:33:19.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 20:33:19.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 20:33:19.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-24 20:33:19.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-24 20:33:19.000000 mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-24 20:33:19.894194 mypy-boto3-storagegateway-1.34.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-01-24 20:33:04.000000 mypy-boto3-storagegateway-1.34.27/setup.py
```

### Comparing `mypy_boto3_storagegateway-1.34.110/LICENSE` & `mypy-boto3-storagegateway-1.34.27/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_storagegateway-1.34.110/PKG-INFO` & `mypy-boto3-storagegateway-1.34.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-storagegateway
-Version: 1.34.110
-Summary: Type annotations for boto3.StorageGateway 1.34.110 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.27
+Summary: Type annotations for boto3.StorageGateway 1.34.27 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-storagegateway)](https://pepy.tech/project/mypy-boto3-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.StorageGateway 1.34.110](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[boto3.StorageGateway 1.34.27](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_storagegateway-1.34.110/README.md` & `mypy-boto3-storagegateway-1.34.27/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-storagegateway)](https://pepy.tech/project/mypy-boto3-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.StorageGateway 1.34.110](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[boto3.StorageGateway 1.34.27](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/__init__.py` & `mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/__init__.pyi` & `mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/client.py` & `mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     AddTagsToResourceOutputTypeDef,
     AddUploadBufferOutputTypeDef,
     AddWorkingStorageOutputTypeDef,
     AssignTapePoolOutputTypeDef,
     AssociateFileSystemOutputTypeDef,
     AttachVolumeOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
-    BandwidthRateLimitIntervalUnionTypeDef,
+    BandwidthRateLimitIntervalTypeDef,
     CacheAttributesTypeDef,
     CancelArchivalOutputTypeDef,
     CancelRetrievalOutputTypeDef,
     CreateCachediSCSIVolumeOutputTypeDef,
     CreateNFSFileShareOutputTypeDef,
     CreateSMBFileShareOutputTypeDef,
     CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
@@ -92,15 +92,15 @@
     DescribeTapesOutputTypeDef,
     DescribeUploadBufferOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeWorkingStorageOutputTypeDef,
     DetachVolumeOutputTypeDef,
     DisableGatewayOutputTypeDef,
     DisassociateFileSystemOutputTypeDef,
-    EndpointNetworkConfigurationUnionTypeDef,
+    EndpointNetworkConfigurationTypeDef,
     JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
     ListFileSharesOutputTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListLocalDisksOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
@@ -115,15 +115,15 @@
     RemoveTagsFromResourceOutputTypeDef,
     ResetCacheOutputTypeDef,
     RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointOutputTypeDef,
     SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayOutputTypeDef,
-    SMBLocalGroupsUnionTypeDef,
+    SMBLocalGroupsTypeDef,
     StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayOutputTypeDef,
     TagTypeDef,
     UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitOutputTypeDef,
     UpdateBandwidthRateLimitScheduleOutputTypeDef,
     UpdateChapCredentialsOutputTypeDef,
@@ -255,15 +255,15 @@
         Password: str,
         ClientToken: str,
         GatewayARN: str,
         LocationARN: str,
         Tags: Sequence[TagTypeDef] = ...,
         AuditDestinationARN: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
-        EndpointNetworkConfiguration: EndpointNetworkConfigurationUnionTypeDef = ...,
+        EndpointNetworkConfiguration: EndpointNetworkConfigurationTypeDef = ...,
     ) -> AssociateFileSystemOutputTypeDef:
         """
         Associate an Amazon FSx file system with the FSx File Gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.associate_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#associate_file_system)
         """
@@ -1129,15 +1129,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_bandwidth_rate_limit)
         """
 
     def update_bandwidth_rate_limit_schedule(
         self,
         *,
         GatewayARN: str,
-        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalUnionTypeDef],
+        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef],
     ) -> UpdateBandwidthRateLimitScheduleOutputTypeDef:
         """
         Updates the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_bandwidth_rate_limit_schedule)
         """
@@ -1284,15 +1284,15 @@
         list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_file_share_visibility)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_smb_file_share_visibility)
         """
 
     def update_smb_local_groups(
-        self, *, GatewayARN: str, SMBLocalGroups: SMBLocalGroupsUnionTypeDef
+        self, *, GatewayARN: str, SMBLocalGroups: SMBLocalGroupsTypeDef
     ) -> UpdateSMBLocalGroupsOutputTypeDef:
         """
         Updates the list of Active Directory users and groups that have special
         permissions for SMB file shares on the
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_local_groups)
```

### Comparing `mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/client.pyi` & `mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     AddTagsToResourceOutputTypeDef,
     AddUploadBufferOutputTypeDef,
     AddWorkingStorageOutputTypeDef,
     AssignTapePoolOutputTypeDef,
     AssociateFileSystemOutputTypeDef,
     AttachVolumeOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
-    BandwidthRateLimitIntervalUnionTypeDef,
+    BandwidthRateLimitIntervalTypeDef,
     CacheAttributesTypeDef,
     CancelArchivalOutputTypeDef,
     CancelRetrievalOutputTypeDef,
     CreateCachediSCSIVolumeOutputTypeDef,
     CreateNFSFileShareOutputTypeDef,
     CreateSMBFileShareOutputTypeDef,
     CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
@@ -92,15 +92,15 @@
     DescribeTapesOutputTypeDef,
     DescribeUploadBufferOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeWorkingStorageOutputTypeDef,
     DetachVolumeOutputTypeDef,
     DisableGatewayOutputTypeDef,
     DisassociateFileSystemOutputTypeDef,
-    EndpointNetworkConfigurationUnionTypeDef,
+    EndpointNetworkConfigurationTypeDef,
     JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
     ListFileSharesOutputTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListLocalDisksOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
@@ -115,15 +115,15 @@
     RemoveTagsFromResourceOutputTypeDef,
     ResetCacheOutputTypeDef,
     RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointOutputTypeDef,
     SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayOutputTypeDef,
-    SMBLocalGroupsUnionTypeDef,
+    SMBLocalGroupsTypeDef,
     StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayOutputTypeDef,
     TagTypeDef,
     UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitOutputTypeDef,
     UpdateBandwidthRateLimitScheduleOutputTypeDef,
     UpdateChapCredentialsOutputTypeDef,
@@ -252,15 +252,15 @@
         Password: str,
         ClientToken: str,
         GatewayARN: str,
         LocationARN: str,
         Tags: Sequence[TagTypeDef] = ...,
         AuditDestinationARN: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
-        EndpointNetworkConfiguration: EndpointNetworkConfigurationUnionTypeDef = ...,
+        EndpointNetworkConfiguration: EndpointNetworkConfigurationTypeDef = ...,
     ) -> AssociateFileSystemOutputTypeDef:
         """
         Associate an Amazon FSx file system with the FSx File Gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.associate_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#associate_file_system)
         """
@@ -1126,15 +1126,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_bandwidth_rate_limit)
         """
 
     def update_bandwidth_rate_limit_schedule(
         self,
         *,
         GatewayARN: str,
-        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalUnionTypeDef],
+        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef],
     ) -> UpdateBandwidthRateLimitScheduleOutputTypeDef:
         """
         Updates the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_bandwidth_rate_limit_schedule)
         """
@@ -1281,15 +1281,15 @@
         list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_file_share_visibility)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_smb_file_share_visibility)
         """
 
     def update_smb_local_groups(
-        self, *, GatewayARN: str, SMBLocalGroups: SMBLocalGroupsUnionTypeDef
+        self, *, GatewayARN: str, SMBLocalGroups: SMBLocalGroupsTypeDef
     ) -> UpdateSMBLocalGroupsOutputTypeDef:
         """
         Updates the list of Active Directory users and groups that have special
         permissions for SMB file shares on the
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_local_groups)
```

### Comparing `mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/literals.py` & `mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,17 +75,15 @@
     "bucket-owner-read",
     "private",
     "public-read",
     "public-read-write",
 ]
 PoolStatusType = Literal["ACTIVE", "DELETED"]
 RetentionLockTypeType = Literal["COMPLIANCE", "GOVERNANCE", "NONE"]
-SMBSecurityStrategyType = Literal[
-    "ClientSpecified", "MandatoryEncryption", "MandatoryEncryptionNoAes128", "MandatorySigning"
-]
+SMBSecurityStrategyType = Literal["ClientSpecified", "MandatoryEncryption", "MandatorySigning"]
 TapeStorageClassType = Literal["DEEP_ARCHIVE", "GLACIER"]
 StorageGatewayServiceName = Literal["storagegateway"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -106,15 +104,14 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
-    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -125,15 +122,14 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
-    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -151,15 +147,14 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
-    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -172,26 +167,24 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
-    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
-    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -252,14 +245,15 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -301,15 +295,14 @@
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
@@ -389,15 +382,14 @@
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
@@ -441,15 +433,14 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
-    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/literals.pyi` & `mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -75,17 +75,15 @@
     "bucket-owner-read",
     "private",
     "public-read",
     "public-read-write",
 ]
 PoolStatusType = Literal["ACTIVE", "DELETED"]
 RetentionLockTypeType = Literal["COMPLIANCE", "GOVERNANCE", "NONE"]
-SMBSecurityStrategyType = Literal[
-    "ClientSpecified", "MandatoryEncryption", "MandatoryEncryptionNoAes128", "MandatorySigning"
-]
+SMBSecurityStrategyType = Literal["ClientSpecified", "MandatoryEncryption", "MandatorySigning"]
 TapeStorageClassType = Literal["DEEP_ARCHIVE", "GLACIER"]
 StorageGatewayServiceName = Literal["storagegateway"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -106,15 +104,14 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
-    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -125,15 +122,14 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
-    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -151,15 +147,14 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
-    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -172,26 +167,24 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
-    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
-    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -252,14 +245,15 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -301,15 +295,14 @@
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
@@ -389,15 +382,14 @@
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
@@ -441,15 +433,14 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
-    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/paginator.py` & `mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/paginator.pyi` & `mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/type_defs.py` & `mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: TagTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     ActiveDirectoryStatusType,
     AvailabilityMonitorTestStatusType,
     CaseSensitivityType,
     FileShareTypeType,
     GatewayCapacityType,
@@ -46,15 +46,14 @@
     "AddUploadBufferInputRequestTypeDef",
     "AddWorkingStorageInputRequestTypeDef",
     "AssignTapePoolInputRequestTypeDef",
     "CacheAttributesTypeDef",
     "EndpointNetworkConfigurationTypeDef",
     "AttachVolumeInputRequestTypeDef",
     "AutomaticTapeCreationRuleTypeDef",
-    "BandwidthRateLimitIntervalOutputTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
     "VolumeiSCSIAttributesTypeDef",
     "CancelArchivalInputRequestTypeDef",
     "CancelRetrievalInputRequestTypeDef",
     "ChapInfoTypeDef",
     "NFSFileShareDefaultsTypeDef",
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
@@ -76,15 +75,15 @@
     "DescribeFileSystemAssociationsInputRequestTypeDef",
     "DescribeGatewayInformationInputRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
     "DescribeNFSFileSharesInputRequestTypeDef",
     "DescribeSMBFileSharesInputRequestTypeDef",
     "DescribeSMBSettingsInputRequestTypeDef",
-    "SMBLocalGroupsOutputTypeDef",
+    "SMBLocalGroupsTypeDef",
     "DescribeSnapshotScheduleInputRequestTypeDef",
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeTapeArchivesInputRequestTypeDef",
     "TapeArchiveTypeDef",
     "DescribeTapeRecoveryPointsInputRequestTypeDef",
     "TapeRecoveryPointInfoTypeDef",
@@ -94,15 +93,14 @@
     "DescribeVTLDevicesInputRequestTypeDef",
     "DescribeWorkingStorageInputRequestTypeDef",
     "DetachVolumeInputRequestTypeDef",
     "DeviceiSCSIAttributesTypeDef",
     "DisableGatewayInputRequestTypeDef",
     "DisassociateFileSystemInputRequestTypeDef",
     "DiskTypeDef",
-    "EndpointNetworkConfigurationOutputTypeDef",
     "FileShareInfoTypeDef",
     "FileSystemAssociationStatusDetailTypeDef",
     "FileSystemAssociationSummaryTypeDef",
     "GatewayInfoTypeDef",
     "JoinDomainInputRequestTypeDef",
     "ListAutomaticTapeCreationPoliciesInputRequestTypeDef",
     "ListFileSharesInputRequestTypeDef",
@@ -121,15 +119,14 @@
     "VolumeInfoTypeDef",
     "NotifyWhenUploadedInputRequestTypeDef",
     "RefreshCacheInputRequestTypeDef",
     "RemoveTagsFromResourceInputRequestTypeDef",
     "ResetCacheInputRequestTypeDef",
     "RetrieveTapeArchiveInputRequestTypeDef",
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
-    "SMBLocalGroupsTypeDef",
     "SetLocalConsolePasswordInputRequestTypeDef",
     "SetSMBGuestPasswordInputRequestTypeDef",
     "ShutdownGatewayInputRequestTypeDef",
     "StartAvailabilityMonitorTestInputRequestTypeDef",
     "StartGatewayInputRequestTypeDef",
     "UpdateBandwidthRateLimitInputRequestTypeDef",
     "UpdateChapCredentialsInputRequestTypeDef",
@@ -221,23 +218,24 @@
     "SMBFileShareInfoTypeDef",
     "UpdateFileSystemAssociationInputRequestTypeDef",
     "UpdateSMBFileShareInputRequestTypeDef",
     "AssociateFileSystemInputRequestTypeDef",
     "AutomaticTapeCreationPolicyInfoTypeDef",
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
-    "BandwidthRateLimitIntervalUnionTypeDef",
+    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     "CachediSCSIVolumeTypeDef",
     "StorediSCSIVolumeTypeDef",
     "DescribeChapCredentialsOutputTypeDef",
     "CreateNFSFileShareInputRequestTypeDef",
     "NFSFileShareInfoTypeDef",
     "UpdateNFSFileShareInputRequestTypeDef",
     "DescribeGatewayInformationOutputTypeDef",
     "DescribeSMBSettingsOutputTypeDef",
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
     "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
     "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
     "DescribeTapesInputDescribeTapesPaginateTypeDef",
     "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
     "ListFileSharesInputListFileSharesPaginateTypeDef",
     "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
     "ListGatewaysInputListGatewaysPaginateTypeDef",
@@ -246,28 +244,24 @@
     "ListTapesInputListTapesPaginateTypeDef",
     "ListVolumesInputListVolumesPaginateTypeDef",
     "DescribeTapeArchivesOutputTypeDef",
     "DescribeTapeRecoveryPointsOutputTypeDef",
     "DescribeTapesOutputTypeDef",
     "VTLDeviceTypeDef",
     "ListLocalDisksOutputTypeDef",
-    "EndpointNetworkConfigurationUnionTypeDef",
     "ListFileSharesOutputTypeDef",
     "FileSystemAssociationInfoTypeDef",
     "ListFileSystemAssociationsOutputTypeDef",
     "ListGatewaysOutputTypeDef",
     "ListTapePoolsOutputTypeDef",
     "ListTapesOutputTypeDef",
     "ListVolumeRecoveryPointsOutputTypeDef",
     "ListVolumesOutputTypeDef",
-    "SMBLocalGroupsUnionTypeDef",
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
     "DescribeSMBFileSharesOutputTypeDef",
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
-    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     "DescribeCachediSCSIVolumesOutputTypeDef",
     "DescribeStorediSCSIVolumesOutputTypeDef",
     "DescribeNFSFileSharesOutputTypeDef",
     "DescribeVTLDevicesOutputTypeDef",
     "DescribeFileSystemAssociationsOutputTypeDef",
 )
 
@@ -278,18 +272,18 @@
         "Value": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
+        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
-        "HostId": NotRequired[str],
     },
 )
 AddCacheInputRequestTypeDef = TypedDict(
     "AddCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
@@ -345,34 +339,22 @@
         "TapeBarcodePrefix": str,
         "PoolId": str,
         "TapeSizeInBytes": int,
         "MinimumNumTapes": int,
         "Worm": NotRequired[bool],
     },
 )
-BandwidthRateLimitIntervalOutputTypeDef = TypedDict(
-    "BandwidthRateLimitIntervalOutputTypeDef",
-    {
-        "StartHourOfDay": int,
-        "StartMinuteOfHour": int,
-        "EndHourOfDay": int,
-        "EndMinuteOfHour": int,
-        "DaysOfWeek": List[int],
-        "AverageUploadRateLimitInBitsPerSec": NotRequired[int],
-        "AverageDownloadRateLimitInBitsPerSec": NotRequired[int],
-    },
-)
 BandwidthRateLimitIntervalTypeDef = TypedDict(
     "BandwidthRateLimitIntervalTypeDef",
     {
         "StartHourOfDay": int,
         "StartMinuteOfHour": int,
         "EndHourOfDay": int,
         "EndMinuteOfHour": int,
-        "DaysOfWeek": Sequence[int],
+        "DaysOfWeek": List[int],
         "AverageUploadRateLimitInBitsPerSec": NotRequired[int],
         "AverageDownloadRateLimitInBitsPerSec": NotRequired[int],
     },
 )
 VolumeiSCSIAttributesTypeDef = TypedDict(
     "VolumeiSCSIAttributesTypeDef",
     {
@@ -557,16 +539,16 @@
 )
 DescribeSMBSettingsInputRequestTypeDef = TypedDict(
     "DescribeSMBSettingsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
-SMBLocalGroupsOutputTypeDef = TypedDict(
-    "SMBLocalGroupsOutputTypeDef",
+SMBLocalGroupsTypeDef = TypedDict(
+    "SMBLocalGroupsTypeDef",
     {
         "GatewayAdmins": NotRequired[List[str]],
     },
 )
 DescribeSnapshotScheduleInputRequestTypeDef = TypedDict(
     "DescribeSnapshotScheduleInputRequestTypeDef",
     {
@@ -716,20 +698,14 @@
         "DiskStatus": NotRequired[str],
         "DiskSizeInBytes": NotRequired[int],
         "DiskAllocationType": NotRequired[str],
         "DiskAllocationResource": NotRequired[str],
         "DiskAttributeList": NotRequired[List[str]],
     },
 )
-EndpointNetworkConfigurationOutputTypeDef = TypedDict(
-    "EndpointNetworkConfigurationOutputTypeDef",
-    {
-        "IpAddresses": NotRequired[List[str]],
-    },
-)
 FileShareInfoTypeDef = TypedDict(
     "FileShareInfoTypeDef",
     {
         "FileShareType": NotRequired[FileShareTypeType],
         "FileShareARN": NotRequired[str],
         "FileShareId": NotRequired[str],
         "FileShareStatus": NotRequired[str],
@@ -940,20 +916,14 @@
 RetrieveTapeRecoveryPointInputRequestTypeDef = TypedDict(
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
     {
         "TapeARN": str,
         "GatewayARN": str,
     },
 )
-SMBLocalGroupsTypeDef = TypedDict(
-    "SMBLocalGroupsTypeDef",
-    {
-        "GatewayAdmins": NotRequired[Sequence[str]],
-    },
-)
 SetLocalConsolePasswordInputRequestTypeDef = TypedDict(
     "SetLocalConsolePasswordInputRequestTypeDef",
     {
         "GatewayARN": str,
         "LocalConsolePassword": str,
     },
 )
@@ -1803,21 +1773,25 @@
         "GatewayARN": str,
     },
 )
 DescribeBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
     {
         "GatewayARN": str,
-        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalOutputTypeDef],
+        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-BandwidthRateLimitIntervalUnionTypeDef = Union[
-    BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef
-]
+UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
+    {
+        "GatewayARN": str,
+        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalTypeDef],
+    },
+)
 CachediSCSIVolumeTypeDef = TypedDict(
     "CachediSCSIVolumeTypeDef",
     {
         "VolumeARN": NotRequired[str],
         "VolumeId": NotRequired[str],
         "VolumeType": NotRequired[str],
         "VolumeStatus": NotRequired[str],
@@ -1967,18 +1941,25 @@
     {
         "GatewayARN": str,
         "DomainName": str,
         "ActiveDirectoryStatus": ActiveDirectoryStatusType,
         "SMBGuestPasswordSet": bool,
         "SMBSecurityStrategy": SMBSecurityStrategyType,
         "FileSharesVisible": bool,
-        "SMBLocalGroups": SMBLocalGroupsOutputTypeDef,
+        "SMBLocalGroups": SMBLocalGroupsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
+    {
+        "GatewayARN": str,
+        "SMBLocalGroups": SMBLocalGroupsTypeDef,
+    },
+)
 DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef = TypedDict(
     "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
     {
         "TapeARNs": NotRequired[Sequence[str]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
@@ -2092,17 +2073,14 @@
     "ListLocalDisksOutputTypeDef",
     {
         "GatewayARN": str,
         "Disks": List[DiskTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-EndpointNetworkConfigurationUnionTypeDef = Union[
-    EndpointNetworkConfigurationTypeDef, EndpointNetworkConfigurationOutputTypeDef
-]
 ListFileSharesOutputTypeDef = TypedDict(
     "ListFileSharesOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileShareInfoList": List[FileShareInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2114,15 +2092,15 @@
         "FileSystemAssociationARN": NotRequired[str],
         "LocationARN": NotRequired[str],
         "FileSystemAssociationStatus": NotRequired[str],
         "AuditDestinationARN": NotRequired[str],
         "GatewayARN": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
         "CacheAttributes": NotRequired[CacheAttributesTypeDef],
-        "EndpointNetworkConfiguration": NotRequired[EndpointNetworkConfigurationOutputTypeDef],
+        "EndpointNetworkConfiguration": NotRequired[EndpointNetworkConfigurationTypeDef],
         "FileSystemAssociationStatusDetails": NotRequired[
             List[FileSystemAssociationStatusDetailTypeDef]
         ],
     },
 )
 ListFileSystemAssociationsOutputTypeDef = TypedDict(
     "ListFileSystemAssociationsOutputTypeDef",
@@ -2170,43 +2148,28 @@
     {
         "GatewayARN": str,
         "Marker": str,
         "VolumeInfos": List[VolumeInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-SMBLocalGroupsUnionTypeDef = Union[SMBLocalGroupsTypeDef, SMBLocalGroupsOutputTypeDef]
-UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
-    {
-        "GatewayARN": str,
-        "SMBLocalGroups": SMBLocalGroupsTypeDef,
-    },
-)
 DescribeSMBFileSharesOutputTypeDef = TypedDict(
     "DescribeSMBFileSharesOutputTypeDef",
     {
         "SMBFileShareInfoList": List[SMBFileShareInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListAutomaticTapeCreationPoliciesOutputTypeDef = TypedDict(
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     {
         "AutomaticTapeCreationPolicyInfos": List[AutomaticTapeCreationPolicyInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
-    {
-        "GatewayARN": str,
-        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalUnionTypeDef],
-    },
-)
 DescribeCachediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesOutputTypeDef",
     {
         "CachediSCSIVolumes": List[CachediSCSIVolumeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway/type_defs.pyi` & `mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: TagTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     ActiveDirectoryStatusType,
     AvailabilityMonitorTestStatusType,
     CaseSensitivityType,
     FileShareTypeType,
     GatewayCapacityType,
@@ -46,15 +46,14 @@
     "AddUploadBufferInputRequestTypeDef",
     "AddWorkingStorageInputRequestTypeDef",
     "AssignTapePoolInputRequestTypeDef",
     "CacheAttributesTypeDef",
     "EndpointNetworkConfigurationTypeDef",
     "AttachVolumeInputRequestTypeDef",
     "AutomaticTapeCreationRuleTypeDef",
-    "BandwidthRateLimitIntervalOutputTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
     "VolumeiSCSIAttributesTypeDef",
     "CancelArchivalInputRequestTypeDef",
     "CancelRetrievalInputRequestTypeDef",
     "ChapInfoTypeDef",
     "NFSFileShareDefaultsTypeDef",
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
@@ -76,15 +75,15 @@
     "DescribeFileSystemAssociationsInputRequestTypeDef",
     "DescribeGatewayInformationInputRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
     "DescribeNFSFileSharesInputRequestTypeDef",
     "DescribeSMBFileSharesInputRequestTypeDef",
     "DescribeSMBSettingsInputRequestTypeDef",
-    "SMBLocalGroupsOutputTypeDef",
+    "SMBLocalGroupsTypeDef",
     "DescribeSnapshotScheduleInputRequestTypeDef",
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeTapeArchivesInputRequestTypeDef",
     "TapeArchiveTypeDef",
     "DescribeTapeRecoveryPointsInputRequestTypeDef",
     "TapeRecoveryPointInfoTypeDef",
@@ -94,15 +93,14 @@
     "DescribeVTLDevicesInputRequestTypeDef",
     "DescribeWorkingStorageInputRequestTypeDef",
     "DetachVolumeInputRequestTypeDef",
     "DeviceiSCSIAttributesTypeDef",
     "DisableGatewayInputRequestTypeDef",
     "DisassociateFileSystemInputRequestTypeDef",
     "DiskTypeDef",
-    "EndpointNetworkConfigurationOutputTypeDef",
     "FileShareInfoTypeDef",
     "FileSystemAssociationStatusDetailTypeDef",
     "FileSystemAssociationSummaryTypeDef",
     "GatewayInfoTypeDef",
     "JoinDomainInputRequestTypeDef",
     "ListAutomaticTapeCreationPoliciesInputRequestTypeDef",
     "ListFileSharesInputRequestTypeDef",
@@ -121,15 +119,14 @@
     "VolumeInfoTypeDef",
     "NotifyWhenUploadedInputRequestTypeDef",
     "RefreshCacheInputRequestTypeDef",
     "RemoveTagsFromResourceInputRequestTypeDef",
     "ResetCacheInputRequestTypeDef",
     "RetrieveTapeArchiveInputRequestTypeDef",
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
-    "SMBLocalGroupsTypeDef",
     "SetLocalConsolePasswordInputRequestTypeDef",
     "SetSMBGuestPasswordInputRequestTypeDef",
     "ShutdownGatewayInputRequestTypeDef",
     "StartAvailabilityMonitorTestInputRequestTypeDef",
     "StartGatewayInputRequestTypeDef",
     "UpdateBandwidthRateLimitInputRequestTypeDef",
     "UpdateChapCredentialsInputRequestTypeDef",
@@ -221,23 +218,24 @@
     "SMBFileShareInfoTypeDef",
     "UpdateFileSystemAssociationInputRequestTypeDef",
     "UpdateSMBFileShareInputRequestTypeDef",
     "AssociateFileSystemInputRequestTypeDef",
     "AutomaticTapeCreationPolicyInfoTypeDef",
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
-    "BandwidthRateLimitIntervalUnionTypeDef",
+    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     "CachediSCSIVolumeTypeDef",
     "StorediSCSIVolumeTypeDef",
     "DescribeChapCredentialsOutputTypeDef",
     "CreateNFSFileShareInputRequestTypeDef",
     "NFSFileShareInfoTypeDef",
     "UpdateNFSFileShareInputRequestTypeDef",
     "DescribeGatewayInformationOutputTypeDef",
     "DescribeSMBSettingsOutputTypeDef",
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
     "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
     "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
     "DescribeTapesInputDescribeTapesPaginateTypeDef",
     "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
     "ListFileSharesInputListFileSharesPaginateTypeDef",
     "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
     "ListGatewaysInputListGatewaysPaginateTypeDef",
@@ -246,28 +244,24 @@
     "ListTapesInputListTapesPaginateTypeDef",
     "ListVolumesInputListVolumesPaginateTypeDef",
     "DescribeTapeArchivesOutputTypeDef",
     "DescribeTapeRecoveryPointsOutputTypeDef",
     "DescribeTapesOutputTypeDef",
     "VTLDeviceTypeDef",
     "ListLocalDisksOutputTypeDef",
-    "EndpointNetworkConfigurationUnionTypeDef",
     "ListFileSharesOutputTypeDef",
     "FileSystemAssociationInfoTypeDef",
     "ListFileSystemAssociationsOutputTypeDef",
     "ListGatewaysOutputTypeDef",
     "ListTapePoolsOutputTypeDef",
     "ListTapesOutputTypeDef",
     "ListVolumeRecoveryPointsOutputTypeDef",
     "ListVolumesOutputTypeDef",
-    "SMBLocalGroupsUnionTypeDef",
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
     "DescribeSMBFileSharesOutputTypeDef",
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
-    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     "DescribeCachediSCSIVolumesOutputTypeDef",
     "DescribeStorediSCSIVolumesOutputTypeDef",
     "DescribeNFSFileSharesOutputTypeDef",
     "DescribeVTLDevicesOutputTypeDef",
     "DescribeFileSystemAssociationsOutputTypeDef",
 )
 
@@ -278,18 +272,18 @@
         "Value": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
+        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
-        "HostId": NotRequired[str],
     },
 )
 AddCacheInputRequestTypeDef = TypedDict(
     "AddCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
@@ -345,34 +339,22 @@
         "TapeBarcodePrefix": str,
         "PoolId": str,
         "TapeSizeInBytes": int,
         "MinimumNumTapes": int,
         "Worm": NotRequired[bool],
     },
 )
-BandwidthRateLimitIntervalOutputTypeDef = TypedDict(
-    "BandwidthRateLimitIntervalOutputTypeDef",
-    {
-        "StartHourOfDay": int,
-        "StartMinuteOfHour": int,
-        "EndHourOfDay": int,
-        "EndMinuteOfHour": int,
-        "DaysOfWeek": List[int],
-        "AverageUploadRateLimitInBitsPerSec": NotRequired[int],
-        "AverageDownloadRateLimitInBitsPerSec": NotRequired[int],
-    },
-)
 BandwidthRateLimitIntervalTypeDef = TypedDict(
     "BandwidthRateLimitIntervalTypeDef",
     {
         "StartHourOfDay": int,
         "StartMinuteOfHour": int,
         "EndHourOfDay": int,
         "EndMinuteOfHour": int,
-        "DaysOfWeek": Sequence[int],
+        "DaysOfWeek": List[int],
         "AverageUploadRateLimitInBitsPerSec": NotRequired[int],
         "AverageDownloadRateLimitInBitsPerSec": NotRequired[int],
     },
 )
 VolumeiSCSIAttributesTypeDef = TypedDict(
     "VolumeiSCSIAttributesTypeDef",
     {
@@ -557,16 +539,16 @@
 )
 DescribeSMBSettingsInputRequestTypeDef = TypedDict(
     "DescribeSMBSettingsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
-SMBLocalGroupsOutputTypeDef = TypedDict(
-    "SMBLocalGroupsOutputTypeDef",
+SMBLocalGroupsTypeDef = TypedDict(
+    "SMBLocalGroupsTypeDef",
     {
         "GatewayAdmins": NotRequired[List[str]],
     },
 )
 DescribeSnapshotScheduleInputRequestTypeDef = TypedDict(
     "DescribeSnapshotScheduleInputRequestTypeDef",
     {
@@ -716,20 +698,14 @@
         "DiskStatus": NotRequired[str],
         "DiskSizeInBytes": NotRequired[int],
         "DiskAllocationType": NotRequired[str],
         "DiskAllocationResource": NotRequired[str],
         "DiskAttributeList": NotRequired[List[str]],
     },
 )
-EndpointNetworkConfigurationOutputTypeDef = TypedDict(
-    "EndpointNetworkConfigurationOutputTypeDef",
-    {
-        "IpAddresses": NotRequired[List[str]],
-    },
-)
 FileShareInfoTypeDef = TypedDict(
     "FileShareInfoTypeDef",
     {
         "FileShareType": NotRequired[FileShareTypeType],
         "FileShareARN": NotRequired[str],
         "FileShareId": NotRequired[str],
         "FileShareStatus": NotRequired[str],
@@ -940,20 +916,14 @@
 RetrieveTapeRecoveryPointInputRequestTypeDef = TypedDict(
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
     {
         "TapeARN": str,
         "GatewayARN": str,
     },
 )
-SMBLocalGroupsTypeDef = TypedDict(
-    "SMBLocalGroupsTypeDef",
-    {
-        "GatewayAdmins": NotRequired[Sequence[str]],
-    },
-)
 SetLocalConsolePasswordInputRequestTypeDef = TypedDict(
     "SetLocalConsolePasswordInputRequestTypeDef",
     {
         "GatewayARN": str,
         "LocalConsolePassword": str,
     },
 )
@@ -1803,21 +1773,25 @@
         "GatewayARN": str,
     },
 )
 DescribeBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
     {
         "GatewayARN": str,
-        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalOutputTypeDef],
+        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-BandwidthRateLimitIntervalUnionTypeDef = Union[
-    BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef
-]
+UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
+    {
+        "GatewayARN": str,
+        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalTypeDef],
+    },
+)
 CachediSCSIVolumeTypeDef = TypedDict(
     "CachediSCSIVolumeTypeDef",
     {
         "VolumeARN": NotRequired[str],
         "VolumeId": NotRequired[str],
         "VolumeType": NotRequired[str],
         "VolumeStatus": NotRequired[str],
@@ -1967,18 +1941,25 @@
     {
         "GatewayARN": str,
         "DomainName": str,
         "ActiveDirectoryStatus": ActiveDirectoryStatusType,
         "SMBGuestPasswordSet": bool,
         "SMBSecurityStrategy": SMBSecurityStrategyType,
         "FileSharesVisible": bool,
-        "SMBLocalGroups": SMBLocalGroupsOutputTypeDef,
+        "SMBLocalGroups": SMBLocalGroupsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
+    {
+        "GatewayARN": str,
+        "SMBLocalGroups": SMBLocalGroupsTypeDef,
+    },
+)
 DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef = TypedDict(
     "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
     {
         "TapeARNs": NotRequired[Sequence[str]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
@@ -2092,17 +2073,14 @@
     "ListLocalDisksOutputTypeDef",
     {
         "GatewayARN": str,
         "Disks": List[DiskTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-EndpointNetworkConfigurationUnionTypeDef = Union[
-    EndpointNetworkConfigurationTypeDef, EndpointNetworkConfigurationOutputTypeDef
-]
 ListFileSharesOutputTypeDef = TypedDict(
     "ListFileSharesOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileShareInfoList": List[FileShareInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2114,15 +2092,15 @@
         "FileSystemAssociationARN": NotRequired[str],
         "LocationARN": NotRequired[str],
         "FileSystemAssociationStatus": NotRequired[str],
         "AuditDestinationARN": NotRequired[str],
         "GatewayARN": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
         "CacheAttributes": NotRequired[CacheAttributesTypeDef],
-        "EndpointNetworkConfiguration": NotRequired[EndpointNetworkConfigurationOutputTypeDef],
+        "EndpointNetworkConfiguration": NotRequired[EndpointNetworkConfigurationTypeDef],
         "FileSystemAssociationStatusDetails": NotRequired[
             List[FileSystemAssociationStatusDetailTypeDef]
         ],
     },
 )
 ListFileSystemAssociationsOutputTypeDef = TypedDict(
     "ListFileSystemAssociationsOutputTypeDef",
@@ -2170,43 +2148,28 @@
     {
         "GatewayARN": str,
         "Marker": str,
         "VolumeInfos": List[VolumeInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-SMBLocalGroupsUnionTypeDef = Union[SMBLocalGroupsTypeDef, SMBLocalGroupsOutputTypeDef]
-UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
-    {
-        "GatewayARN": str,
-        "SMBLocalGroups": SMBLocalGroupsTypeDef,
-    },
-)
 DescribeSMBFileSharesOutputTypeDef = TypedDict(
     "DescribeSMBFileSharesOutputTypeDef",
     {
         "SMBFileShareInfoList": List[SMBFileShareInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListAutomaticTapeCreationPoliciesOutputTypeDef = TypedDict(
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     {
         "AutomaticTapeCreationPolicyInfos": List[AutomaticTapeCreationPolicyInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
-    {
-        "GatewayARN": str,
-        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalUnionTypeDef],
-    },
-)
 DescribeCachediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesOutputTypeDef",
     {
         "CachediSCSIVolumes": List[CachediSCSIVolumeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway.egg-info/PKG-INFO` & `mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-storagegateway
-Version: 1.34.110
-Summary: Type annotations for boto3.StorageGateway 1.34.110 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.27
+Summary: Type annotations for boto3.StorageGateway 1.34.27 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-storagegateway)](https://pepy.tech/project/mypy-boto3-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.StorageGateway 1.34.110](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[boto3.StorageGateway 1.34.27](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_storagegateway-1.34.110/mypy_boto3_storagegateway.egg-info/SOURCES.txt` & `mypy-boto3-storagegateway-1.34.27/mypy_boto3_storagegateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_storagegateway-1.34.110/setup.py` & `mypy-boto3-storagegateway-1.34.27/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-storagegateway",
-    version="1.34.110",
+    version="1.34.27",
     packages=["mypy_boto3_storagegateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.StorageGateway 1.34.110 service generated with mypy-boto3-builder 7.24.0",
+    description=(
+        "Type annotations for boto3.StorageGateway 1.34.27 service generated with"
+        " mypy-boto3-builder 7.23.1"
+    ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

