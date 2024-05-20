# Comparing `tmp/pih-0.36.9.tar.gz` & `tmp/pih-0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-0.36.9.tar", last modified: Wed Apr 17 14:06:34 2024, max compression
+gzip compressed data, was "pih-0.37.tar", last modified: Mon May 20 23:05:23 2024, max compression
```

## Comparing `pih-0.36.9.tar` & `pih-0.37.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 14:06:34.243077 pih-0.36.9/
--rw-rw-rw-   0        0        0      249 2024-04-17 14:06:34.196313 pih-0.36.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 14:06:32.211168 pih-0.36.9/pih/
--rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.36.9/pih/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:06:32.514860 pih-0.36.9/pih/collections/
--rw-rw-rw-   0        0        0    28524 2024-04-17 05:26:38.000000 pih-0.36.9/pih/collections/__init__.py
--rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.36.9/pih/collections/service.py
--rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.36.9/pih/console_api.py
--rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.36.9/pih/console_api_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:06:33.819127 pih-0.36.9/pih/consts/
--rw-rw-rw-   0        0        0    25249 2024-04-17 14:05:45.000000 pih-0.36.9/pih/consts/__init__.py
--rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.36.9/pih/consts/ad.py
--rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.36.9/pih/consts/addresses.py
--rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.36.9/pih/consts/date_time.py
--rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.36.9/pih/consts/document.py
--rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.36.9/pih/consts/errors.py
--rw-rw-rw-   0        0        0    30004 2024-04-15 23:46:38.000000 pih-0.36.9/pih/consts/events.py
--rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.36.9/pih/consts/facade.py
--rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.36.9/pih/consts/file.py
--rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.36.9/pih/consts/hosts.py
--rw-rw-rw-   0        0        0      187 2024-04-17 05:22:16.000000 pih-0.36.9/pih/consts/iot.py
--rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.36.9/pih/consts/names.py
--rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.36.9/pih/consts/password.py
--rw-rw-rw-   0        0        0    11944 2024-04-10 22:09:05.000000 pih-0.36.9/pih/consts/paths.py
--rw-rw-rw-   0        0        0    11122 2024-04-16 01:31:15.000000 pih-0.36.9/pih/consts/polibase.py
--rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.36.9/pih/consts/python.py
--rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.36.9/pih/consts/recognize.py
--rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.36.9/pih/consts/rpc.py
--rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.36.9/pih/consts/service.py
--rw-rw-rw-   0        0        0     6540 2024-04-17 04:46:50.000000 pih-0.36.9/pih/consts/service_commands.py
--rw-rw-rw-   0        0        0    12239 2024-04-17 13:50:24.000000 pih-0.36.9/pih/consts/service_roles.py
--rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.36.9/pih/consts/settings.py
--rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.36.9/pih/consts/ssh_hosts.py
--rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.36.9/pih/consts/zabbix.py
--rw-rw-rw-   0        0        0   549782 2024-04-17 12:36:18.000000 pih-0.36.9/pih/pih.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:06:33.993085 pih-0.36.9/pih/rpc/
--rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.36.9/pih/rpc/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.36.9/pih/rpc/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.36.9/pih/rpc/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.36.9/pih/service_example.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:06:34.102456 pih-0.36.9/pih/tools/
--rw-rw-rw-   0        0        0    51621 2024-04-16 02:10:50.000000 pih-0.36.9/pih/tools/__init__.py
--rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.36.9/pih/tools/service.py
--rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.36.9/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:06:34.164949 pih-0.36.9/pih.egg-info/
--rw-rw-rw-   0        0        0      249 2024-04-17 14:06:31.000000 pih-0.36.9/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      956 2024-04-17 14:06:31.000000 pih-0.36.9/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 14:06:31.000000 pih-0.36.9/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-17 14:06:31.000000 pih-0.36.9/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-17 14:06:31.000000 pih-0.36.9/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 14:06:34.243077 pih-0.36.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 23:05:23.483360 pih-0.37/
+-rw-rw-rw-   0        0        0      247 2024-05-20 23:05:23.436483 pih-0.37/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 23:05:20.538872 pih-0.37/pih/
+-rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.37/pih/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:05:21.285612 pih-0.37/pih/collections/
+-rw-rw-rw-   0        0        0    30339 2024-05-17 03:55:00.000000 pih-0.37/pih/collections/__init__.py
+-rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.37/pih/collections/service.py
+-rw-rw-rw-   0        0        0   104237 2024-05-17 04:58:32.000000 pih-0.37/pih/console_api.py
+-rw-rw-rw-   0        0        0     2549 2024-05-19 11:56:07.000000 pih-0.37/pih/console_api_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:05:22.951668 pih-0.37/pih/consts/
+-rw-rw-rw-   0        0        0    26747 2024-05-20 22:38:29.000000 pih-0.37/pih/consts/__init__.py
+-rw-rw-rw-   0        0        0     3694 2024-05-18 23:37:39.000000 pih-0.37/pih/consts/ad.py
+-rw-rw-rw-   0        0        0     1768 2024-05-08 05:34:18.000000 pih-0.37/pih/consts/addresses.py
+-rw-rw-rw-   0        0        0      974 2024-04-21 23:56:33.000000 pih-0.37/pih/consts/date_time.py
+-rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.37/pih/consts/document.py
+-rw-rw-rw-   0        0        0      936 2024-05-20 02:54:33.000000 pih-0.37/pih/consts/errors.py
+-rw-rw-rw-   0        0        0    30003 2024-04-22 02:31:56.000000 pih-0.37/pih/consts/events.py
+-rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.37/pih/consts/facade.py
+-rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.37/pih/consts/file.py
+-rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.37/pih/consts/hosts.py
+-rw-rw-rw-   0        0        0      194 2024-04-17 15:27:11.000000 pih-0.37/pih/consts/iot.py
+-rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.37/pih/consts/names.py
+-rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.37/pih/consts/password.py
+-rw-rw-rw-   0        0        0    12272 2024-05-13 03:26:35.000000 pih-0.37/pih/consts/paths.py
+-rw-rw-rw-   0        0        0    16020 2024-05-20 22:44:51.000000 pih-0.37/pih/consts/polibase.py
+-rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.37/pih/consts/python.py
+-rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.37/pih/consts/recognize.py
+-rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.37/pih/consts/rpc.py
+-rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.37/pih/consts/service.py
+-rw-rw-rw-   0        0        0     6540 2024-04-17 04:46:50.000000 pih-0.37/pih/consts/service_commands.py
+-rw-rw-rw-   0        0        0    12120 2024-05-12 15:14:12.000000 pih-0.37/pih/consts/service_roles.py
+-rw-rw-rw-   0        0        0    17765 2024-05-20 04:39:33.000000 pih-0.37/pih/consts/settings.py
+-rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.37/pih/consts/ssh_hosts.py
+-rw-rw-rw-   0        0        0      233 2024-05-17 04:55:05.000000 pih-0.37/pih/consts/style.py
+-rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.37/pih/consts/zabbix.py
+-rw-rw-rw-   0        0        0   572231 2024-05-20 02:59:52.000000 pih-0.37/pih/pih.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:05:23.186465 pih-0.37/pih/rpc/
+-rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.37/pih/rpc/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.37/pih/rpc/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.37/pih/rpc/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.37/pih/service_example.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:05:23.342733 pih-0.37/pih/tools/
+-rw-rw-rw-   0        0        0    59031 2024-05-20 00:30:59.000000 pih-0.37/pih/tools/__init__.py
+-rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.37/pih/tools/service.py
+-rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.37/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:05:23.405234 pih-0.37/pih.egg-info/
+-rw-rw-rw-   0        0        0      247 2024-05-20 23:05:19.000000 pih-0.37/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      976 2024-05-20 23:05:19.000000 pih-0.37/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 23:05:19.000000 pih-0.37/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 23:05:19.000000 pih-0.37/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-20 23:05:19.000000 pih-0.37/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 23:05:23.498986 pih-0.37/setup.cfg
```

### Comparing `pih-0.36.9/pih/collections/__init__.py` & `pih-0.37/pih/collections/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import ipih
+
+from enum import Enum
+from collections import namedtuple
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta, date
-from enum import Enum
 from typing import Any, Tuple, List, Callable, TypeVar, Generic
-from collections import namedtuple
 
 
 @dataclass
 class Host:
     name: str
     aliases: str | tuple[str, ...] | None = None
     ip: str | None = None
@@ -41,14 +43,53 @@
     category: str | None = None
     product_name: str | None = None
     product_id: str | None = None
     biz_type: int | None = None
 
 
 @dataclass
+class IOTDeviceStatusProperty:
+    code: str | None = None
+    name: str | None = None
+    type: str | None = None
+    unit: str | None = None
+
+
+@dataclass
+class IOTDeviceStatusIntegerProperty(IOTDeviceStatusProperty):
+
+    min: int | float | None = None
+    max: int | float | None = None
+    scale: int | float | None = None
+    step: int | float | None = None
+
+
+"""
+@dataclass
+class IOTDeviceStatusProperty:
+    code: str | None = None
+    name: str | None = None
+    type: str | None = None
+    values: tuple[IOTDeviceStatusPropertyValue, ...] | None = None
+"""
+
+
+@dataclass
+class IOTDeviceStatusValue:
+    code: str | None = None
+    value: Any = None
+
+
+@dataclass
+class IOTDeviceStatus:
+    timestamp: int = 0
+    values: tuple[IOTDeviceStatusValue, ...] | None = None
+
+
+@dataclass
 class ZabbixMetricsValue:
     value: Any | None = None
     clock: datetime | int | None = None
 
 
 @dataclass
 class ZabbixMetrics:
@@ -241,14 +282,15 @@
     fields: FieldItemList | None = None
     data: T | None = None
 
     def __len__(self):
         return len(self.data)
 
     def __iadd__(self, value):
+        self.data = self.data or []
         if (
             isinstance(value, Result)
             and isinstance(self.data, list)
             and isinstance(value.data, list)
         ):
             self.data += value.data
         return self
@@ -282,14 +324,18 @@
 
 @dataclass
 class User(UserBase):
     samAccountName: str | None = None
     mail: str | None = None
     telephoneNumber: str | None = None
     userAccountControl: int | None = None
+    
+    @property
+    def login(self) -> str:
+        return self.samAccountName
 
 
 Rect = namedtuple("Rect", ["left", "top", "width", "height"])
 
 
 @dataclass
 class IndicationDevice:
@@ -374,14 +420,18 @@
     description: str | None = None
 
 
 @dataclass
 class Computer(ComputerDescription):
     samAccountName: str | None = None
     accessable: bool | None = None
+    
+    @property
+    def login(self) -> str:
+        return self.samAccountName
 
 
 @dataclass
 class Server(Computer):
     pass
 
 
@@ -399,14 +449,29 @@
 
 @dataclass
 class ResourceDescriptionDelegated(ResourceDescription):
     delegator: str | None = None
 
 
 @dataclass
+class ZabbixResourceDescription(ResourceDescription):
+    zabbix_host_name: str | None = None
+
+    def get_zabbix_host_name(self) -> str:
+        return self.zabbix_host_name or self.address
+
+
+@dataclass
+class ZabbixResourceDescriptionDelegated(
+    ZabbixResourceDescription, ResourceDescriptionDelegated
+):
+    pass
+
+
+@dataclass
 class SiteResourceDescription(ResourceDescription):
     check_certificate_status: bool = False
     check_free_space_status: bool = False
     driver_name: str | None = None
     internal: bool = False
 
 
@@ -499,14 +564,15 @@
     beginDate: str | datetime | None = None
     completeDate: str | datetime | None = None
     status: int | None = None
     cabinetID: int | None = None
     doctorID: int | None = None
     doctorFullName: str | None = None
     serviceGroupID: int | None = None
+    comment: str | None = None
 
 
 @dataclass
 class CardRegistryFolderStatistics:
     name: str | None = None
     count: int = 0
 
@@ -540,14 +606,16 @@
 
 
 @dataclass
 class Message:
     message: str | None = None
     recipient: str | None = None
     sender: str | None = None
+    image_url: str | None = None
+    location: tuple[float, float] | None = None
 
 
 @dataclass
 class DelayedMessage(Message):
     date: Any | None = None
     type: int | None = None
 
@@ -585,14 +653,15 @@
 @dataclass
 class PolibasePersonVisit(PolibasePersonVisitDS):
     registrationDate: datetime | None = None
     beginDate: datetime | None = None
     completeDate: datetime | None = None
     beginDate2: datetime | None = None
     completeDate2: datetime | None = None
+    Comment: str | None = None
 
 
 @dataclass
 class PolibasePersonQuest:
     step: int | None = None
     stepConfirmed: bool | None = None
     timestamp: int | None = None
@@ -699,32 +768,32 @@
     name: str
     list: List[TimeTrackingResultByPerson] = field(default_factory=list)
 
 
 @dataclass
 class RobocopyJobDescription:
     name: str | None = None
-    start_datetime: str | None = None
+    start_cron_string: str | None = None
     host: str | None = None
     run_from_system_account: bool = False
     run_with_elevetion: bool = False
     live: bool = False
     exclude: bool = False
 
     def clone(
         self,
         job_name: str,
-        start_datetime: str | None = None,
+        start_cron_string: str | None = None,
         host: str | None = None,
         live: bool | None = None,
         exclude: bool = False,
     ):
         return RobocopyJobDescription(
             job_name,
-            start_datetime,
+            start_cron_string,
             host or self.host,
             self.run_from_system_account,
             self.run_with_elevetion,
             self.live if live is None else live,
             self.exclude if exclude is None else exclude,
         )
 
@@ -1007,14 +1076,26 @@
 
 @dataclass
 class IntStorageVariableHolder(StorageVariableHolder):
     default_value: int = 0
 
 
 @dataclass
+class VariantableStorageVariable:
+    variants: tuple[Any, ...]| None = None
+
+
+@dataclass
+class IntVariantableStorageVariableHolder(
+    VariantableStorageVariable, IntStorageVariableHolder
+):
+    variants: tuple[int, ...] | None = None
+
+
+@dataclass
 class MinIntStorageVariableHolder(IntStorageVariableHolder):
     min_value: int = 0
 
 
 @dataclass
 class IntStorageVariableHolderWithMin(IntStorageVariableHolder):
     min_value: int = 0
```

### Comparing `pih-0.36.9/pih/collections/service.py` & `pih-0.37/pih/collections/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.9/pih/console_api.py` & `pih-0.37/pih/console_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,47 +20,45 @@
     User,
     Result,
     EventDS,
     UserBase,
     FullName,
     MarkGroup,
     ZabbixHost,
-    ZabbixMetrics,
-    ZabbixMetricsValue,
     Workstation,
     PrinterReport,
     FieldItemList,
     DiskStatistics,
     ResourceStatus,
     PersonDivision,
+    ZabbixMetrics,
     EventDescription,
     RobocopyJobStatus,
     LoginPasswordPair,
     SiteResourceStatus,
     CTIndicationsValue,
-    DisksStatisticsStatus,
+    ZabbixMetricsValue,
     ComputerDescription,
     TimeSeriesStatistics,
     StorageVariableHolder,
+    DisksStatisticsStatus,
     ExpiredTimestampVariableHolder,
-    ChillerIndicationsValueContainer,
 )
 from pih.tools import (
     j,
     e,
-    i,
     lw,
     nl,
     js,
     nn,
     ne,
+    nns,
     jnl,
     esc,
     one,
-    b as mb,
     while_not_do,
     BitMask as BM,
 )
 
 
 LINE: str = "........................................................"
 
@@ -239,19 +237,34 @@
                     )
                     if isinstance(resource, SiteResourceStatus):
                         if resource.check_free_space_status:
                             free_space_result_list: str = (
                                 resource.free_space_status.split(" ")
                             )
                             result.append(
-                                f"      Cвободное место: {free_space_result_list[0]} ({free_space_result_list[1]})"
+                                j(
+                                    (
+                                        " " * 6,
+                                        "Cвободное место: ",
+                                        free_space_result_list[0],
+                                        "(",
+                                        free_space_result_list[1],
+                                        ")",
+                                    )
+                                )
                             )
                         if resource.check_certificate_status:
                             result.append(
-                                f"      Сертификат доступен до: {resource.certificate_status}"
+                                j(
+                                    (
+                                        " " * 6,
+                                        "Сертификат доступен до: ",
+                                        resource.certificate_status,
+                                    )
+                                )
                             )
                     return jnl(result)
 
                 force_update = force_update or (
                     ask_for_update_before and self.yes_no("Обновить перед получением")
                 )
                 if force_update:
@@ -377,19 +390,24 @@
                                 )
                             )
                         )
                     with self.output.make_indent(4):
                         self.output.write_result(A.R_IND.last_ct_value_containers(True))
                         self.output.write_image(
                             self.bold("График показаний"),
-                            A.D_CO.file_to_base64(
-                                A.PTH_STAT.get_file_path(A.CT_STAT.Types.CT_DAY)
+                            nns(
+                                A.D_CO.file_to_base64(
+                                    nns(
+                                        A.PTH_STAT.get_file_path(A.CT_STAT.Types.CT_DAY)
+                                    )
+                                )
                             ),
                         )
                     self.output.separated_line()
+                    """
                     with self.output.make_indent(2):
                         self.output.write_line(
                             js(
                                 (
                                     "",
                                     A.CT_V.BULLET,
                                     self.bold("Показания в техническом помещении МРТ"),
@@ -405,15 +423,17 @@
                     path: str = A.PTH_IND.CHILLER_DATA_IMAGE_LAST
                     modification_timstamp: float = A.PTH.get_modification_time(path)
                     file_creating_datetime: datetime | None = datetime.fromtimestamp(
                         modification_timstamp
                         if modification_timstamp > 0
                         else A.PTH.get_creation_time(path)
                     )
+                    """
                     with self.output.make_indent(4):
+                        """
                         if not A.C_IND.chiller_on():
                             self.output.write_line(
                                 js(("", A.CT_V.WARNING, "Чиллер выключен"))
                             )
                         else:
                             with self.output.make_indent(2, True):
                                 self.output.write_result(
@@ -443,58 +463,49 @@
                                             A.D_F.datetime(file_creating_datetime),
                                         )
                                     ),
                                     A.D_CO.file_to_base64(
                                         A.PTH_IND.CHILLER_DATA_IMAGE_LAST_RESULT
                                     ),
                                 )
-                                self.output.write_line(
-                                    self.bold("Текущая выработка фильтра чиллера МРТ:")
-                                )
-                                statistics: TimeSeriesStatistics = (
-                                    A.D_STAT.for_chiller_filter()
-                                )
-                                total_seconds: int = (
-                                    A.D.now() - statistics.values[-1]
-                                ).total_seconds()
+                        """
+                        self.output.write_line(
+                            self.bold("Текущая выработка фильтра чиллера МРТ:")
+                        )
+                        statistics: TimeSeriesStatistics = A.D_STAT.for_chiller_filter()
+                        total_seconds: int = (
+                            A.D.now() - statistics.values[-1]
+                        ).total_seconds()
 
-                                def repr_value(title: str, value: int) -> str:
-                                    return js(
-                                        (
-                                            "",
-                                            A.CT_V.BULLET,
-                                            j((title, A.CT.SPLITTER)),
-                                            self.bold(
-                                                js(
-                                                    (
-                                                        str(
-                                                            int(
-                                                                100
-                                                                * (
-                                                                    total_seconds
-                                                                    / value
-                                                                )
-                                                            )
-                                                        ),
-                                                        "%",
-                                                    )
-                                                )
-                                            ),
+                        def repr_value(title: str, value: int) -> str:
+                            return js(
+                                (
+                                    "",
+                                    A.CT_V.BULLET,
+                                    j((title, A.CT.SPLITTER)),
+                                    self.bold(
+                                        js(
+                                            (
+                                                str(int(100 * (total_seconds / value))),
+                                                "%",
+                                            )
                                         )
-                                    )
-
-                                self.output.write_line(
-                                    jnl(
-                                        (
-                                            repr_value("Минимальная", statistics.max),
-                                            repr_value("Средняя", statistics.avg),
-                                            repr_value("Максимальная", statistics.min),
-                                        ),
-                                    )
+                                    ),
                                 )
+                            )
+
+                        self.output.write_line(
+                            jnl(
+                                (
+                                    repr_value("Минимальная", statistics.max),
+                                    repr_value("Средняя", statistics.avg),
+                                    repr_value("Максимальная", statistics.min),
+                                ),
+                            )
+                        )
             if CheckableSections.TIMESTAMPS in checkable_section_list:
                 if len(checkable_section_list) > 1:
                     if self.session.is_mobile:
                         self.output.new_line()
                     self.output.separated_line()
                     self.output.write_line(
                         js((A.CT_V.BLUE_ROMB, self.bold("Временные метки")))
@@ -1059,67 +1070,66 @@
                         label_function(item, metrics_list)
                     ),
                     value_list_result,
                 )
 
         A.D.every(every_action, metrics_list)
 
-    def polibase_restart(self) -> None:
+    def polibase_restart(self, test: bool = False) -> None:
         if self.yes_no("Перезапустить сервер Polibase"):
             check_word: str = A.CT_P.NAME
-            test: bool = not (
-                check_word
-                == self.input.input(
-                    f"Введите контрольное слово: {self.bold(check_word)}"
+            if check_word == self.input.input(
+                js(("Введите контрольное слово:", self.bold(check_word)))
+            ):
+                notify: bool = test or self.yes_no("Уведомить пользователей", True)
+                title: str = j(("Перезапуск Polibas", [1, 2][test]))
+                polibase_host: str = (
+                    A.CT_H.POLIBASE_TEST.NAME if test else A.CT_H.POLIBASE.NAME
                 )
-            )
-            notify: bool = test or self.yes_no("Уведомить пользователей", True)
-            title: str = f"Перезапуск Polibase{' test' if test else ''}"
-            polibase_host: str = (
-                A.CT_H.POLIBASE_TEST.NAME if test else A.CT_H.POLIBASE.NAME
-            )
-            self.output.write_line(
-                A.L.it(
-                    f"{title}: Начат процесс закрытия программы Polibase на компьютерах."
+                self.output.write_line(
+                    A.L.it(
+                        f"{title}: Начат процесс закрытия программы Polibase на компьютерах."
+                    )
                 )
-            )
-            A.A_P.client_program_close_for_all(notify, None, test)
-            self.output.new_line()
-            self.output.write_line(
-                A.L.it(f"{title}: Начат процесс перезагрузки сервера Polibase.")
-            )
-            A.A_P.restart(test)
-            while_not_do(
-                lambda: not A.C_R.accessibility_by_ping(polibase_host), sleep_time=5
-            )
-            self.output.new_line()
-            self.output.write_line(
-                A.L.it(f"{title}: Начат процесс загрузки сервера Polibase.")
-            )
-            while_not_do(
-                lambda: A.C_R.accessibility_by_ping(polibase_host), sleep_time=5
-            )
-            self.output.new_line()
-            A.E.wait_server_start(polibase_host)
-            self.output.write_line(
-                A.L.it(f"{title}: Завершен процесс загрузки сервера Polibase.")
-            )
-            A.ME_P.notify_about_polibase_restarted(test)
+                A.A_P.client_program_close_for_all(notify, None, test)
+                self.output.new_line()
+                self.output.write_line(
+                    A.L.it(f"{title}: Начат процесс перезагрузки сервера Polibase.")
+                )
+                A.A_P.restart(test)
+                while_not_do(
+                    lambda: not A.C_R.accessibility_by_ping(polibase_host), sleep_time=5
+                )
+                self.output.new_line()
+                self.output.write_line(
+                    A.L.it(f"{title}: Начат процесс загрузки сервера Polibase.")
+                )
+                while_not_do(
+                    lambda: A.C_R.accessibility_by_ping(polibase_host), sleep_time=5
+                )
+                self.output.new_line()
+                A.E.wait_server_start(polibase_host)
+                self.output.write_line(
+                    A.L.it(f"{title}: Завершен процесс загрузки сервера Polibase.")
+                )
+                A.ME_P.notify_about_polibase_restarted(test)
+            else:
+                self.output.error("Контрольное слово не коректно")
 
     def polibase_client_program_close(
         self, search_value: str | None = None, for_all: bool = False
     ) -> None:
         if for_all:
             check_word: str = A.CT_P.NAME
             test: bool = not (
                 check_word
                 == (
                     search_value
                     or self.input.input(
-                        f"Введите контрольное слово - {self.bold(check_word)}"
+                        js(("Введите контрольное слово:", self.bold(check_word)))
                     )
                 )
             )
             A.A_P.client_program_close_for_all(
                 True,
                 self.input.input("Введите сообщение для пользователей Polibase"),
                 test,
@@ -1249,22 +1259,23 @@
 
     def find_free_mark(self, value: str | None = None) -> None:
         self.output.mark.result(
             A.R_M.by_any(value or self.input.mark.any()),
             "Список свободных карт доступа:",
         )
 
-    def find_user(self, value: str | None = None) -> None:
+    def user_find(self, value: str | None = None) -> None:
         try:
             self.output.user.result(
                 A.R_U.by_any(value or self.input.user.title_any()),
                 "Найденые пользователи:",
             )
         except NotFound as error:
             self.output.error(error.get_details())
+            raise error
 
     def create_password(self) -> str:
         password: str | None = None
         password_settings: PasswordSettings = PASSWORD.get(
             self.input.indexed_field_list(
                 "Выберите тип пароля", A.CT_FC.POLICY.PASSWORD_TYPE
             )
@@ -1348,58 +1359,58 @@
                             self.output.error("Телефон не указан")
                 except NotFound:
                     self.output.error("Карта доступа, с введенным номером не найдена")
         except KeyboardInterrupt:
             pass
 
     def bold(self, value: str) -> str:
-        return self.output.bold(value)
+        return A.D.bold(value)
 
     def italic(self, value: str) -> str:
-        return self.output.italic(value)
+        return A.D.italics(value)
 
     def create_new_mark(self):
         self.full_name: str | None = None
         self.mark_tab_number: str | None = None
         self.telephone_number: str | None = None
         self.mark_person_division_id: int | None = None
 
         def get_full_name() -> ActionValue:
-            self.output.header("Заполните ФИО персоны")
+            self.output.paragraph("Заполните ФИО персоны")
             self.full_name = self.input.full_name(True)
             user_exists: bool = not A.C.MARK.exists_by_full_name(self.full_name)
             if user_exists:
                 self.output.error(
                     "Персона с данной фамилией, именем и отчеством уже есть!"
                 )
                 if not self.yes_no("Продолжить"):
                     self.session.exit()
             return self.output.get_action_value(
                 "ФИО персоны", A.D.fullname_to_string(self.full_name)
             )
 
         def get_telephone_number() -> ActionValue:
-            self.output.header("Заполните номер телефона")
+            self.output.paragraph("Заполните номер телефона")
             self.telephone_number = self.input.telephone_number()
             return self.output.get_action_value(
                 "Номер телефона", self.telephone_number, False
             )
 
         def get_tab_number() -> ActionValue:
-            self.output.header("Выбор группы и номера для карты доступа")
+            self.output.paragraph("Выбор группы и номера для карты доступа")
             free_mark: Mark = self.input.mark.free()
             group_name: str = free_mark.GroupName
             self.mark_tab_number = free_mark.TabNumber
             self.output.value("Группа карты доступа", group_name)
             return self.output.get_action_value(
                 "Номер карты пропуска", self.mark_tab_number
             )
 
         def get_division() -> ActionValue:
-            self.output.header("Выбор подразделения")
+            self.output.paragraph("Выбор подразделения")
             person_division: PersonDivision = self.input.mark.person_division()
             self.mark_person_division_id = person_division.id
             return self.output.get_action_value(
                 "Подразделение, к которому прикреплена персона", person_division.name
             )
 
         ActionStack(
@@ -1522,15 +1533,15 @@
                                 self.user_given_name,
                                 " (",
                                 self.user_description,
                                 "): ",
                             )
                         )
                         if self.session.is_mobile:
-                            self.output.write_line(nl(i(prefix)))
+                            self.output.write_line(nl(A.D_F.italics(prefix)))
                         message = message or self.input.message(
                             f"введите сообщение для компьютера {recipient.name}",
                             None if self.session.is_mobile else prefix,
                         )
                         if A.ME_WS.to_workstation(recipient, message):
                             self.output.good("Сообщение отправлено")
                             message = None
@@ -1753,17 +1764,14 @@
         except NotFound as error:
             self.output.error(error.get_details())
 
     @property
     def session(self) -> Session:
         return self.pih.session
 
-    def b(self, value: Any) -> str:
-        return mb(value) if self.session.is_mobile else str(value)
-
     def create_new_user(self) -> None:
         self.full_name: FullName | None = None
         self.mark_tab_number: str | None = None
         self.telephone_number: str | None = None
         self.mark_person_division_id: int | None = None
         self.user_is_exists: bool = False
         self.login: str | None = None
@@ -1795,15 +1803,15 @@
                         self.session.exit()
                 return self.output.get_action_value(
                     js(("ФИО", "пользователя" if as_pc_user else "персоны")),
                     A.D.fullname_to_string(self.full_name),
                 )
 
         def get_login(as_pc_user: bool = True) -> ActionValue:
-            self.output.header(
+            self.output.paragraph(
                 js(
                     (
                         "Создание логина для аккаунта",
                         "пользователя" if as_pc_user else "корпоративной почты",
                     )
                 )
             )
@@ -1820,56 +1828,56 @@
                             ),
                         )
                     ),
                     self.login,
                 )
 
         def get_telephone_number() -> ActionValue:
-            self.output.header("Заполнение номера телефона")
+            self.output.paragraph("Заполнение номера телефона")
             with self.output.make_indent(2):
                 self.telephone_number = self.input.telephone_number()
                 return self.output.get_action_value(
                     "Номер телефона", self.telephone_number, False
                 )
 
         def get_description(as_pc_user: bool = True) -> ActionValue:
-            self.output.header(
+            self.output.paragraph(
                 js(("Заполнение описания", "пользователя" if as_pc_user else "персоны"))
             )
             with self.output.make_indent(2):
                 self.description = self.input.description()
                 return self.output.get_action_value(
                     js(("Описание", "пользователя" if as_pc_user else "персоны")),
                     self.description,
                     False,
                 )
 
         def get_additional_information() -> ActionValue:
-            self.output.header("Заполнение дополнительную информацию")
+            self.output.paragraph("Заполнение дополнительную информацию")
             with self.output.make_indent(2):
                 self.additional_information = self.input.input(
                     "Дополнительную информация"
                 )
                 return self.output.get_action_value(
                     "Дополнительную информация", self.additional_information, False
                 )
 
         def get_template_user_container_or_user_container() -> ActionValue:
-            self.output.header("Выбор контейнера для пользователя")
+            self.output.paragraph("Выбор контейнера для пользователя")
             with self.output.make_indent(2):
                 self.user_container, self.use_template_user = (
                     self.input.user.template(),
                     True,
                 )
                 return self.output.get_action_value(
                     "Контейнер пользователя", self.user_container.description  # type: ignore
                 )
 
         def get_password(as_pc_user: bool = True) -> ActionValue:
-            self.output.header(
+            self.output.paragraph(
                 js(
                     (
                         "Создание пароля для",
                         (
                             "аккаунта пользователя"
                             if as_pc_user
                             else "аккаунта корпоративной почты"
@@ -1894,15 +1902,15 @@
                         )
                     ),
                     self.corporate_email,
                 )
 
         def get_mark_person_division() -> ActionValue | None:
             if self.need_to_create_mark and A.D.is_none(self.mark_person_division_id):
-                self.output.header("Выбор подразделения")
+                self.output.paragraph("Выбор подразделения")
                 with self.output.make_indent(2):
                     mark_person_division: PersonDivision = (
                         self.input.mark.person_division(False)
                     )
                     self.mark_person_division_id = mark_person_division.id
                     return self.output.get_action_value(
                         "Подразделение персоны, которой принадлежит карта доступа",
@@ -1910,26 +1918,26 @@
                     )
             return None
 
         def get_tab_number() -> ActionValue | None:
             full_name_string: str = A.D.fullname_to_string(self.full_name)  # type: ignore
             mark: Mark | None = A.R_M.by_name(full_name_string, True).data  # type: ignore
             with self.output.make_indent(2):
-                self.output.header("Создание карты доступа")
+                self.output.paragraph("Создание карты доступа")
                 if nn(mark):
                     if self.yes_no(
                         f"Найдена карта доступа для персоны {full_name_string} с номером {mark.TabNumber}. Использовать",
                         True,
                     ):
                         self.need_to_create_mark = False
                         self.mark_tab_number = mark.TabNumber  # type: ignore
                         self.mark_person_division_id = mark.DivisionID  # type: ignore
                         return None
                 self.need_to_create_mark = self.yes_no(
-                    js(("Создать карту доступа для персоны", self.b(full_name_string))),
+                    js(("Создать карту доступа для персоны", self.output.bold(full_name_string))),
                     True,
                 )
                 if self.need_to_create_mark:
                     free_mark: Mark = self.input.mark.free()
                     self.mark_tab_number = free_mark.TabNumber
                     self.mark_person_division_id = free_mark.DivisionID
                     self.output.value("Группа карты доступа", free_mark.GroupName)  # type: ignore
```

### Comparing `pih-0.36.9/pih/console_api_wrapper.py` & `pih-0.37/pih/console_api_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,78 @@
+from pih import strdict, isolate, delay
 from pih.tools import *
 from pih.collections import *
+from pih.consts.errors import NotFound
 from pih import A, PIH, OutputStub
 
 from typing import Any
 
 output_stub: OutputStub = OutputStub()
 
 
 class Stub(PIH):
-    def arg(self) -> Any | None:
-        return self.session.arg()
+
+    def arg(self, index: int = 0) -> Any | None:
+        return self.session.arg(index)
+
+    @property
+    def arg_list(self) -> list[str] | None:
+        return self.session.arg_list
 
     def __init__(self):
         self.is_force: bool = False
 
+    def write_line(self, value: str) -> None:
+        self.output.write_line(value)
+
 
 if not A.SE.is_mobile:
     self: Stub = Stub()
-b = output_stub.b
-i = output_stub.i
+#b = output_stub.b
+#i = output_stub.i
 
 
-def execute(file_search_request: str) -> None:
+def execute(file_search_request: str, parameters: strdict | None = None) -> None:
     with A.ER.detect_interruption():
         A.R_F.execute(
             file_search_request,
-            parameters={"self": self},
+            parameters={"self": self} | A.D.map(A.D.as_value, (parameters or {})),
             stdout_redirect=False,
             catch_exceptions=True,
         )
 
 
 def execute_file(
     use_authentification: bool,
     title: str | None,
     file_search_request: str,
     show_loading_delay: float | None = None,
     loading_text: str | None = None,
-    done_text: str | None = None
+    done_text: str | None = "Выполнено!",
+    parameters: strdict | None = None,
 ) -> None:
     A.O.init()
+    if ne(title):
+        A.O.head(title)  # type: ignore
     if not use_authentification or A.SE.authenticate():
+        if not use_authentification:
+            A.SE.fill_access_groups()
         A.O.clear_screen()
         A.O.pih_title()
         if ne(title):
             A.O.head1(title)  # type: ignore
         if n(show_loading_delay):
-            execute(file_search_request)
+            execute(file_search_request, parameters)
         else:
             with A.O.make_loading(
                 show_loading_delay, loading_text or "Идёт выполнение файла"
             ):
-                execute(file_search_request)
-        A.O.good(done_text or "Выполнено!")
+                execute(file_search_request, parameters)
+        if nn(done_text):
+            A.O.good(done_text)
         A.SE.exit(0)
     A.SE.exit(0, "Выход")
 
 
 def include(
     value: str, class_name: str | None = None, global_dict: dict[str, Any] | None = None
 ) -> Any | dict[str, Any] | None:
```

### Comparing `pih-0.36.9/pih/consts/__init__.py` & `pih-0.37/pih/consts/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from enum import Enum, auto, IntEnum
 
-from pih.tools import j
+from pih.tools import j, js
 from pih.consts import *
 from pih.consts.names import *
 from pih.consts.paths import *
 from pih.collections import (
     ActionDescription,
     ResourceDescription,
     MedicalResearchType,
     SiteResourceDescription,
+    ZabbixResourceDescription,
     MinIntStorageVariableHolder,
     ResourceDescriptionDelegated,
     OrderedNameCaptionDescription,
+    ZabbixResourceDescriptionDelegated,
     IconedOrderedNameCaptionDescription,
 )
 from pih.consts.password import *
 from pih.consts.date_time import *
 from pih.consts.service_commands import *
 
-VERSION: str = "0.36.9"
+VERSION: str = "0.37"
+
 
 class DATA:
     # deprecated
     class EXTRACTOR:
         USER_NAME_FULL: str = "user_name_full"
         USER_NAME: str = "user_name"
         AS_IS: str = "as_is"
@@ -61,14 +64,19 @@
 
 class FONT:
     FOR_PDF: str = "DejaVuSerif"
 
 
 class SessionFlags(IntEnum):
     CLI = 512
+    OUTSIDE = 8192
+    
+class SESSION_TYPE:
+    MOBILE: str = "mobile"
+    OUTSIDE: str = "outside"
 
 
 class URLS:
     PYPI: str = "https://pypi.python.org/pypi/pih/json"
 
 
 class EmailVerificationMethods(IntEnum):
@@ -93,14 +101,21 @@
         7: "Files were copied, a file mismatch was present, and additional files were present.",
     }
 
 
 class CHARSETS:
     WINDOWS_ALTERNATIVE: str = "CP866"
     UTF8: str = "utf-8"
+    
+class INPUT_TYPE:
+    NO: int = -1
+    NORMAL: int = 0
+    INDEX: int = 1
+    QUESTION: int = 2
+
 
 class WINDOWS:
 
     NAME: str = "Windows"
 
     class ENVIROMENT_VARIABLES:
         PATH: str = "PATH"
@@ -117,26 +132,35 @@
         TASK_SCHEDULER: str = "schtasks"
 
     class PROCESSES:
         POWER_SHELL_REMOTE_SESSION: str = "wsmprovhost.exe"
 
     class PORT:
         SMB: int = 445
-
+        
 
 class CONST(DATE_TIME):
-    
+
+    class ADDRESS:
+
+        LOCATION: tuple[float, float] = (43.10077173904819, 131.90206595788635)
+        TEXT: str = (
+            "- г. Владивосток, ул. Запорожская, 7\n- Поликлиника: пн-сб с 8 до 20\n- Приемное отделение: круглосуточно, без праздников и выходных"
+        )
+
     EMAIL_SPLITTER: str = "@"
     ISOLATED_ARG_NAME: str = "isolated"
     ARGUMENT_PREFIX: str = "--"
     SPLITTER: str = ":"
-    UNKNOWN: str = "?"
+    NAME_SPLITTER: str = "_"
+    UNKNOWN_VALUE: str = "?"
 
     class PORT:
         HTTP: int = 80
+        HTTPS: int = 443
         SMTP: int = 587
         IMAP: int = 993
         SNMP: int = 161
 
     class FILES:
         SECTION: str = "Мобильные файлы"
 
@@ -149,26 +173,26 @@
     # in seconds
     HEART_BEAT_PERIOD: int = 60
 
     NEW_LINE: str = "\n"
 
     class TEST:
         WORKSTATION_MAME: str = Hosts.DEVELOPER.NAME
-        USER: str | None = "nak"
+        USER: str | None = "nikita"
         EMAIL_ADDRESS: str | None = "nak@pacifichosp.com"
         PIN: int = 100310
         NAME: str = "test"
 
     GROUP_PREFIX: str = "group:"
 
     SITE_PROTOCOL: str = "https://"
     UNTRUST_SITE_PROTOCOL: str = "http://"
 
     INTERNATIONAL_TELEPHONE_NUMBER_PREFIX: str = "7"
-    TELEPHONE_NUMBER_PREFIX: str = f"+{INTERNATIONAL_TELEPHONE_NUMBER_PREFIX}"
+    TELEPHONE_NUMBER_PREFIX: str = j(("+", INTERNATIONAL_TELEPHONE_NUMBER_PREFIX))
     INTERNAL_TELEPHONE_NUMBER_PREFIX: str = "тел."
 
     class CACHE:
         class TTL:
             # in seconds
             WORKSTATIONS: int = 60
             USERS: int = 300
@@ -181,17 +205,18 @@
         REPORT_DAY_PERIOD_DEFAULT: int = 15
 
     class MESSAGE:
         class WHATSAPP:
             SITE_NAME: str = "https://wa.me/"
             SEND_MESSAGE_TO_TEMPLATE: str = SITE_NAME + "{}?text={}"
             GROUP_SUFFIX: str = "@g.us"
+            OUTSIDE_SUFFIX: str = "@outside"
+            CLI_SUFFIX: str = "@cli"
 
             class GROUP(Enum):
-                # IT: str = "120363163438805316@g.us"
                 PIH_CLI = "120363163438805316@g.us"
                 REGISTRATOR_CLI = "120363212130686795@g.us"
                 RD = "79146947050-1595848245@g.us"
                 MAIN = "79644300470-1447044803@g.us"
                 EMAIL_CONTROL = "120363159605715569@g.us"
                 CT_INDICATIONS = "120363084280723039@g.us"
                 DOCUMENTS_WORK_STACK = "120363115241877592@g.us"
@@ -201,32 +226,40 @@
                 SCANNED_DOCUMENT_HELPER_CLI = "120363220286578760@g.us"
 
             class WAPPI:
 
                 DATETIME_FORMAT: str = "%Y-%m-%dT%H:%M:%SZ"
                 NAME: str = "Wappi"
                 DESCRIPTION: str = "Сервис по отправке сообщений"
+                SEND: str = "send?"
 
                 PROFILE_SUFFIX: str = "profile_id="
                 URL_API: str = "https://wappi.pro/api"
-                URL_API_SYNC: str = f"{URL_API}/sync"
-                URL_MESSAGE: str = f"{URL_API_SYNC}/message"
+                URL_API_SYNC: str = j((URL_API, "/sync"))
+                URL_MESSAGE: str = j((URL_API_SYNC, "/message"))
                 STATUS: str = j(
                     (j((URL_API_SYNC, "get", "status"), "/"), "?", PROFILE_SUFFIX)
                 )
-                URL_SEND_MESSAGE: str = f"{URL_MESSAGE}/send?{PROFILE_SUFFIX}"
-                URL_SEND_VIDEO: str = f"{URL_MESSAGE}/video/send?{PROFILE_SUFFIX}"
-                URL_SEND_IMAGE: str = f"{URL_MESSAGE}/img/send?{PROFILE_SUFFIX}"
-                URL_SEND_DOCUMENT: str = f"{URL_MESSAGE}/document/send?{PROFILE_SUFFIX}"
-                URL_SEND_LIST_MESSAGE: str = f"{URL_MESSAGE}/list/send?{PROFILE_SUFFIX}"
-                URL_SEND_BUTTONS_MESSAGE: str = (
-                    f"{URL_MESSAGE}/buttons/send?{PROFILE_SUFFIX}"
+                URL_SEND_MESSAGE: str = j((URL_MESSAGE, "/", SEND, PROFILE_SUFFIX))
+                URL_SEND_LOCATION: str = j(
+                    (URL_MESSAGE, "/location/", SEND, PROFILE_SUFFIX)
+                )
+                URL_SEND_VIDEO: str = j((URL_MESSAGE, "/video/", SEND, PROFILE_SUFFIX))
+                URL_SEND_IMAGE: str = j((URL_MESSAGE, "/img/", SEND, PROFILE_SUFFIX))
+                URL_SEND_DOCUMENT: str = j(
+                    (URL_MESSAGE, "/document/", SEND, PROFILE_SUFFIX)
+                )
+                URL_SEND_LIST_MESSAGE: str = j(
+                    (URL_MESSAGE, "/list/", SEND, PROFILE_SUFFIX)
                 )
-                URL_GET_MESSAGES: str = f"{URL_MESSAGE}s/get?{PROFILE_SUFFIX}"
-                URL_GET_STATUS: str = f"{URL_API_SYNC}/get/status?{PROFILE_SUFFIX}"
+                URL_SEND_BUTTONS_MESSAGE: str = j(
+                    (URL_MESSAGE, "/buttons/", SEND, PROFILE_SUFFIX)
+                )
+                URL_GET_MESSAGES: str = j((URL_MESSAGE, "s/get?", PROFILE_SUFFIX))
+                URL_GET_STATUS: str = j((URL_API_SYNC, "/get/status?", PROFILE_SUFFIX))
                 CONTACT_SUFFIX: str = "@c.us"
 
                 class Profiles(Enum):
                     IT = "e6706eaf-ae17"
                     CALL_CENTRE = "285c71a4-05f7"
                     MARKETER = "c31db01c-b6d6"
                     DEFAULT = CALL_CENTRE
@@ -266,15 +299,14 @@
             "psservice",
             "psshutdown",
             "pssuspend",
         ]
 
         NO_BANNER: str = "-nobanner"
         ACCEPTEULA: str = "-accepteula"
-    
 
     class MSG:
         NAME: str = "msg"
         EXECUTOR: str = NAME
 
     class BARCODE_READER:
         PREFIX: str = "("
@@ -373,69 +405,83 @@
             "77.88.55.242", "Интернет соединение"
         )
 
         VPN_PACS_SPB: ResourceDescriptionDelegated = ResourceDescriptionDelegated(
             "192.168.5.3", "VPN соединение для PACS SPB", (2, 100, 5), Hosts.WS255.NAME
         )
 
-        PACS_SPB: ResourceDescriptionDelegated = ResourceDescriptionDelegated(
-            "10.76.12.124:4242", "Соединение PACS SPB", (2, 100, 5), Hosts.WS255.NAME
+        PACS_SPB: ZabbixResourceDescriptionDelegated = (
+            ZabbixResourceDescriptionDelegated(
+                "10.76.12.124:4242",
+                "Соединение PACS SPB",
+                (2, 100, 5),
+                Hosts.WS255.NAME,
+                "PACS_SPB",
+            )
         )
 
         POLIBASE1: ResourceDescription = ResourceDescription(
             Hosts.POLIBASE1.NAME,
             "Polibase",
             inaccessibility_check_values=(2, 10000, 15),
         )
 
         POLIBASE2: ResourceDescription = ResourceDescription(
             Hosts.POLIBASE2.NAME,
             "Polibase reserved",
             inaccessibility_check_values=(2, 10000, 15),
         )
 
-        POLIBASE: ResourceDescription = ResourceDescription(
-            Hosts.POLIBASE.ALIAS,
-            "Polibase",
-            inaccessibility_check_values=(2, 10000, 15),
+        POLIBASE: ZabbixResourceDescription = ZabbixResourceDescription(
+            POLIBASE1.address,
+            POLIBASE1.name,
+            POLIBASE1.inaccessibility_check_values,
+            Hosts.POLIBASE1.ALIAS,
         )
 
         SITE_LIST: list[SiteResourceDescription] = [
             SiteResourceDescription(
                 ADDRESSES.SITE_ADDRESS,
-                f"Сайт компании: {ADDRESSES.SITE_ADDRESS}",
+                js(("Сайт компании:", ADDRESSES.SITE_ADDRESS)),
                 inaccessibility_check_values=(1, 20, 15),
                 check_certificate_status=True,
                 check_free_space_status=True,
                 driver_name="/dev/mapper/centos-root",
             ),
             SiteResourceDescription(
                 ADDRESSES.EMAIL_SERVER_ADDRESS,
-                f"Сайт корпоративной почты: {ADDRESSES.EMAIL_SERVER_ADDRESS}",
+                js(("Сайт корпоративной почты:", ADDRESSES.EMAIL_SERVER_ADDRESS)),
                 check_certificate_status=True,
                 check_free_space_status=True,
                 driver_name="/dev/mapper/centos_tenant26--02-var",
             ),
             SiteResourceDescription(
                 ADDRESSES.API_SITE_ADDRESS,
-                f"Api сайта {ADDRESSES.SITE_ADDRESS}: {ADDRESSES.API_SITE_ADDRESS}",
+                js(
+                    (
+                        "Api сайта",
+                        j((ADDRESSES.SITE_ADDRESS, ":")),
+                        ADDRESSES.API_SITE_ADDRESS,
+                    )
+                ),
                 check_certificate_status=True,
                 check_free_space_status=False,
             ),
             SiteResourceDescription(
-                ADDRESSES.BITRIX_SITE_URL, f"Сайт ЦМРТ24: {ADDRESSES.BITRIX_SITE_URL}"
+                ADDRESSES.BITRIX_SITE_URL,
+                js(("Сайт ЦМРТ24:", ADDRESSES.BITRIX_SITE_URL)),
             ),
             SiteResourceDescription(
                 ADDRESSES.OMS_SITE_ADDRESS,
-                f"Внутренний сайт омс: {ADDRESSES.OMS_SITE_ADDRESS}",
+                js(("Внутренний сайт омс:", ADDRESSES.OMS_SITE_ADDRESS)),
                 internal=True,
             ),
             SiteResourceDescription(
                 ADDRESSES.WIKI_SITE_ADDRESS,
-                f"Внутренний сайт Вики: {ADDRESSES.WIKI_SITE_ADDRESS}",
+                js(("Внутренний сайт Вики:", ADDRESSES.WIKI_SITE_ADDRESS)),
                 internal=True,
             ),
         ]
 
 
 class CheckableSections(IntEnum):
     RESOURCES = auto()
@@ -458,14 +504,19 @@
 class MarkType(IntEnum):
     NORMAL = auto()
     FREE = auto()
     GUEST = auto()
     TEMPORARY = auto()
 
 
+class MARK_VARIANT:
+    BRACELET: str = "-0-"
+    CARD: str = ""
+
+
 class PolibasePersonInformationQuestStatus(IntEnum):
     UNKNOWN = -1
     GOOD = 0
     EMAIL_IS_EMPTY = 1
     EMAIL_IS_WRONG = 2
     EMAIL_IS_NOT_ACCESSABLE = 4
```

### Comparing `pih-0.36.9/pih/consts/ad.py` & `pih-0.37/pih/consts/ad.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from enum import Enum, auto
 
 class AD:
     
     ADMINISTRATOR_LOGIN: str = "Administrator"
     SPLITTER: str = "."
     OU: str = "OU="
+    INCATIVE_OU_NAME: str = j((OU, "Inactive"))
     SEARCH_ATTRIBUTES: list[str] = [USER_PROPERTIES.LOGIN, USER_PROPERTIES.NAME]
     SEARCH_ATTRIBUTE_DEFAULT: str = SEARCH_ATTRIBUTES[0]
     USER_HOME_FOLDER_DISK: str = "U:"
     SEARCH_ALL_PATTERN: str = "*"
     LOCATION_JOINER: str = ":"
     TEMPLATED_USER_SERACH_TEMPLATE: str = j(("_", SEARCH_ALL_PATTERN, "_"))
```

### Comparing `pih-0.36.9/pih/consts/addresses.py` & `pih-0.37/pih/consts/addresses.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from pih.tools import j, js, jp
+from pih.tools import j, jp
 from pih.consts import CONST
 
 
 class ADDRESSES:
 
     REMOTE_PREFIX: str = "remote"
     SITE_NAME: str = "pacifichosp"
     SITE_ADDRESS: str = jp((SITE_NAME, "com"))
     EMAIL_SERVER_ADDRESS: str = jp(("mail", SITE_ADDRESS))
     RECEPTION_NAME: str = "reception"
+    CALL_CENTRE: str = "callcentre"
     ADD_EMAIL_NAME: str = "add_email"
     RECEPTION_LOGIN: str = jp((RECEPTION_NAME, SITE_NAME))
 
     WIKI_SITE_NAME: str = "wiki"
     WIKI_SITE_ADDRESS: str = WIKI_SITE_NAME
     OMS_SITE_NAME: str = "oms"
     OMS_SITE_ADDRESS: str = OMS_SITE_NAME
@@ -31,15 +32,18 @@
     MAIL_RU_IMAP_SERVER: str = jp(("imap", MAIL_RU_NAME))
 
     NAS: str = j(("nas", ADDRESSES.SITE_ADDRESS), CONST.EMAIL_SPLITTER)
     IT: str = j(("it", ADDRESSES.SITE_ADDRESS), CONST.EMAIL_SPLITTER)
     RECEPTION: str = j(
         (ADDRESSES.RECEPTION_NAME, ADDRESSES.SITE_ADDRESS), CONST.EMAIL_SPLITTER
     )
+    CALL_CENTRE: str = j(
+        (ADDRESSES.CALL_CENTRE, ADDRESSES.SITE_ADDRESS), CONST.EMAIL_SPLITTER
+    )
     ADD_EMAIL: str = j(
         (ADDRESSES.ADD_EMAIL_NAME, ADDRESSES.SITE_ADDRESS), CONST.EMAIL_SPLITTER
     )
-    EXTERNAL: str = js(
+    EXTERNAL: str = j(
         ("mail.", ADDRESSES.SITE_NAME, CONST.EMAIL_SPLITTER, MAIL_RU_NAME)
     )
 
     EXTERNAL_SERVER: str = MAIL_RU_IMAP_SERVER
```

### Comparing `pih-0.36.9/pih/consts/date_time.py` & `pih-0.37/pih/consts/date_time.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,8 +12,9 @@
     DATE_PART_DELIMITER: str = "."
     YEARLESS_DATE_FORMAT: str = f"{DAY_FORMAT}{DATE_PART_DELIMITER}%m"
     DATE_FORMAT: str = f"{YEARLESS_DATE_FORMAT}{DATE_PART_DELIMITER}%Y"
     DAYLESS_DATE_FORMAT: str = f"%m{DATE_PART_DELIMITER}%Y"
 
     DATETIME_ONLY_HOUR_FORMAT: str = f"{DATE_FORMAT} {HOUR_TIME_FORMAT}"
     DATETIME_SECOND_ZEROS_FORMAT: str = f"{DATE_FORMAT} {SECOND_ZEROS_TIME_FORMAT}"
+    DATETIME_SECONDLESS_FORMAT: str = f"{DATE_FORMAT} {SECONDLESS_TIME_FORMAT}"
     DATETIME_FORMAT: str = f"{DATE_FORMAT} {TIME_FORMAT}"
```

### Comparing `pih-0.36.9/pih/consts/errors.py` & `pih-0.37/pih/consts/errors.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.9/pih/consts/events.py` & `pih-0.37/pih/consts/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
     POLIBASE_PERSONS_WITH_OLD_FORMAT_BARCODE_WAS_DETECTED = EventDescription(
         "Полибейс: обнаружены пациенты со старым форматом или отсутствующим штрих-кодом",
         LogMessageChannels.POLIBASE,
         LogMessageFlags.SILENCE,
         (PARAM_ITEMS.PERSON_PIN,),
     )
 
-    POLIBASE_PERSONS_BONUS_CARD_WAS_CREATED = EventDescription(
+    POLIBASE_PERSON_BONUS_CARD_WAS_CREATED = EventDescription(
         "Бонусная карта для клиента {} была создана",
         LogMessageChannels.POLIBASE,
         (LogMessageFlags.NOTIFICATION, LogMessageFlags.SAVE),
         (
             PARAM_ITEMS.PERSON_PIN.configurate(key=True),
             ParamItem("url", "").configurate(visible=False),
         ),
```

### Comparing `pih-0.36.9/pih/consts/hosts.py` & `pih-0.37/pih/consts/hosts.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.9/pih/consts/names.py` & `pih-0.37/pih/consts/names.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.9/pih/consts/password.py` & `pih-0.37/pih/consts/password.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.9/pih/consts/paths.py` & `pih-0.37/pih/consts/paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,27 +228,39 @@
 class PATH_APP_DATA:
     NAME: str = "data"
     FOLDER: str = os.path.join(PATH_APP.FOLDER, NAME)
 
     OCR_RESULT_NAME: str = "ocr result"
     OCR_RESULT_FOLDER: str = os.path.join(FOLDER, OCR_RESULT_NAME)
 
+    @staticmethod
+    def LOCATION_IMAGE_PATH(index: int) -> str:
+        return PathTool.path(
+            os.path.join(
+                PATH_APP_DATA.FOLDER,
+                "location",
+                PathTool.add_extension(str(index), FILE.EXTENSION.JPG),
+            )
+        )
+
 
 class PATH_STATISTICS:
     NAME: str = "statistics"
     CHART_FILE_NAME_PREFIX: str = "chart_"
     FOLDER: str = os.path.join(PATH_APP_DATA.FOLDER, NAME)
 
     @staticmethod
     def get_file_path(name: str | Enum) -> str:
-        from pih.tools import PathTool, EnumTool, j
+        from pih.tools import EnumTool
 
         name = EnumTool.get(name)
         return PathTool.path(
-            os.path.join(PATH_STATISTICS.FOLDER, j((name, FILE.EXTENSION.PNG), "."))
+            os.path.join(
+                PATH_STATISTICS.FOLDER, PathTool.add_extension(name, FILE.EXTENSION.PNG)
+            )
         )
 
 
 class PATH_INDICATIONS:
     NAME: str = "indications"
     FOLDER: str = os.path.join(PATH_APP_DATA.FOLDER, NAME)
```

### Comparing `pih-0.36.9/pih/consts/service.py` & `pih-0.37/pih/consts/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.9/pih/consts/service_commands.py` & `pih-0.37/pih/consts/service_commands.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.9/pih/consts/service_roles.py` & `pih-0.37/pih/consts/service_roles.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 from pih.collections.service import ServiceDescription
 from pih.consts.service_commands import ServiceCommands
 from ipih import SERVICE_ADMIN_HOST_NAME, SERVICE_ADMIN_GRPC_PORT
 
 class ServiceRoles(ServiceRoleBase):
 
     SERVICE_ADMIN = ServiceDescription(
-        name="ServiceAdmin",
+        "ServiceAdmin",
         host=SERVICE_ADMIN_HOST_NAME,
         port=RPC.PORT(SERVICE_ADMIN_GRPC_PORT),
         commands=(
             ServiceCommands.on_service_starts,
             ServiceCommands.on_service_stops,
             ServiceCommands.get_service_information_list,
             ServiceCommands.heart_beat,
         ),
     )
 
     EVENT = ServiceDescription(
-        name="Event",
+        "Event",
         commands=(ServiceCommands.send_log_message, ServiceCommands.send_event),
     )
 
     DS = ServiceDescription(
-        name="DataSource",
+        "DataSource",
         commands=(
             ServiceCommands.register_polibase_person_information_quest,
             ServiceCommands.search_polibase_person_information_quests,
             ServiceCommands.update_polibase_person_information_quest,
             #
             ServiceCommands.update_polibase_person_visit_to_data_stogare,
             ServiceCommands.search_polibase_person_visits_in_data_storage,
@@ -68,15 +68,15 @@
             ServiceCommands.execute_data_source_query,
             ServiceCommands.joke,
             ServiceCommands.get_event_count,
         ),
     )
 
     AD = ServiceDescription(
-        name="ActiveDirectory",
+        "ActiveDirectory",
         commands=(
             ServiceCommands.authenticate,
             ServiceCommands.check_user_exists_by_login,
             ServiceCommands.get_user_by_full_name,
             ServiceCommands.get_users_by_name,
             ServiceCommands.get_user_by_login,
             ServiceCommands.get_user_by_telephone_number,
@@ -97,45 +97,45 @@
             ServiceCommands.drop_user_cache,
             ServiceCommands.drop_workstaion_cache,
             ServiceCommands.get_user_list_by_property,
         ),
     )
 
     RECOGNIZE = ServiceDescription(
-        name="Recognize",
+        "Recognize",
         commands=(
             ServiceCommands.get_barcode_list_information,
             ServiceCommands.document_type_exists,
             ServiceCommands.recognize_document,
         ),
     )
 
     FILE_WATCHDOG = ServiceDescription(
-        name="FileWatchdog", commands=(ServiceCommands.listen_for_new_files,)
+        "FileWatchdog", commands=(ServiceCommands.listen_for_new_files,)
     )
 
     """
     FILE_ORGANIZER = ServiceDescription(
-        name="FileOrganizer",
+        "FileOrganizer",
         description="File organizer service",
         host=HOSTS.WS255.NAME,
     )
     """
 
     MAIL = ServiceDescription(
-        name="Mail",
+        "Mail",
         commands=(
             ServiceCommands.check_email_accessibility,
             ServiceCommands.send_email,
             ServiceCommands.get_email_information,
         ),
     )
 
     DOCS = ServiceDescription(
-        name="Docs",
+        "Docs",
         commands=(
             ServiceCommands.get_inventory_report,
             ServiceCommands.create_user_document,
             ServiceCommands.save_time_tracking_report,
             ServiceCommands.create_barcodes_for_inventory,
             ServiceCommands.create_barcode_for_polibase_person,
             ServiceCommands.create_qr_code,
@@ -148,15 +148,15 @@
             ServiceCommands.create_statistics_chart,
             ServiceCommands.save_xlsx,
             ServiceCommands.drop_note_cache,
         ),
     )
 
     MARK = ServiceDescription(
-        name="Mark",
+        "Mark",
         commands=(
             ServiceCommands.get_free_mark_list,
             ServiceCommands.get_temporary_mark_list,
             ServiceCommands.get_mark_person_division_list,
             ServiceCommands.get_time_tracking,
             ServiceCommands.get_mark_list,
             ServiceCommands.get_mark_by_tab_number,
@@ -173,15 +173,15 @@
             ServiceCommands.make_mark_as_temporary,
             ServiceCommands.remove_mark_by_tab_number,
             ServiceCommands.door_command,
         ),
     )
 
     POLIBASE = ServiceDescription(
-        name="Polibase",
+        "Polibase",
         commands=(
             ServiceCommands.get_polibase_person_by_pin,
             ServiceCommands.get_polibase_persons_by_pin,
             ServiceCommands.get_polibase_persons_by_telephone_number,
             ServiceCommands.get_polibase_persons_by_name,
             ServiceCommands.get_polibase_persons_by_card_registry_folder_name,
             ServiceCommands.get_polibase_person_registrator_by_pin,
@@ -203,131 +203,133 @@
             ServiceCommands.execute_polibase_query,
             ServiceCommands.update_person_change_date,
             ServiceCommands.get_polibase_person_pin_by_login,
             ServiceCommands.get_polibase_person_user_login_and_worstation_name_pair_list,
             ServiceCommands.get_bonus_list,
         ),
     )
+    
+    GATEWAY = ServiceDescription("Gateway")
 
-    MESSAGE_RECEIVER = ServiceDescription(name="MessageReceiver")
+    MESSAGE_RECEIVER = ServiceDescription("MessageReceiver")
 
-    WEB_SERVER = ServiceDescription(name="WebServer")
+    WEB_SERVER = ServiceDescription("WebServer")
 
     CHECKER = ServiceDescription(
-        name="Checker", commands=(ServiceCommands.get_resource_status_list,)
+        "Checker", commands=(ServiceCommands.get_resource_status_list,)
     )
 
-    AUTOMATION = ServiceDescription(name="Automation")
+    AUTOMATION = ServiceDescription("Automation")
 
-    MOBILE_HELPER = ServiceDescription(name="MobileHelper", standalone_name="mio")
+    MOBILE_HELPER = ServiceDescription("MobileHelper", standalone_name="mio")
 
     POLIBASE_AUTOMATION = ServiceDescription(
-        name="PolibaseAutomation", description="Polibase automation service"
+        "PolibaseAutomation", description="Polibase automation service"
     )
 
     MESSAGE_QUEUE = ServiceDescription(
-        name="MessageQueue",
+        "MessageQueue",
         commands=(ServiceCommands.add_message_to_queue,),
     )
 
-    NOTIFICATION_AUTOMATION = ServiceDescription(name="NotificationAutomation")
+    NOTIFICATION_AUTOMATION = ServiceDescription("NotificationAutomation")
 
     REVIEW_AUTOMATION = ServiceDescription(
-        name="ReviewNotification"
+        "ReviewNotification"
     )
 
     WS = ServiceDescription(
-        name="WS",
+        "WS",
         commands=(
             ServiceCommands.reboot,
             ServiceCommands.shutdown,
             ServiceCommands.send_message_to_user_or_workstation,
             ServiceCommands.kill_process,
         ),
     )
 
     BACKUP = ServiceDescription(
-        name="Backup",
+        "Backup",
         commands=(
             ServiceCommands.robocopy_start_job,
             ServiceCommands.robocopy_get_job_status_list,
         ),
         standalone_name="bck",
     )
 
     PRINTER = ServiceDescription(
-        name="Printer",
+        "Printer",
         commands=(ServiceCommands.printers_report, ServiceCommands.printer_snmp_call),
     )
     
     
     ZABBIX = ServiceDescription(
-        name="Zabbix",
+        "Zabbix",
     )
     
     IOTDevices = ServiceDescription(
-        name="IOTDevices",
+        "IOTDevices",
     )
 
     POLIBASE_DATABASE = ServiceDescription(
-        name="PolibaseDatabase",
+        "PolibaseDatabase",
         commands=(ServiceCommands.create_polibase_database_backup,),
     )
 
     SSH = ServiceDescription(
-        name="SSH",
+        "SSH",
         commands=(
             ServiceCommands.execute_ssh_command,
             ServiceCommands.get_certificate_information,
             ServiceCommands.get_unix_free_space_information_by_drive_name,
             ServiceCommands.mount_facade_for_linux_host,
         ),
     )
 
     """
     POLIBASE_PERSON_INFORMATION_QUEST = ServiceDescription(
-        name="PolibasePersonInformationQuest",
+        "PolibasePersonInformationQuest",
         description="Polibase Person Information Quest service",
         host=Hosts.BACKUP_WORKER.NAME,
         commands=(ServiceCommands.start_polibase_person_information_quest,),
     )
     """
 
     WS735 = ServiceDescription(
-        name="ws735",
+        "ws735",
         description="ws-735 service",
         host=Hosts.WS735.NAME,
         commands=(ServiceCommands.print_image,)
     )
 
     RECOGNIZE_TEST = ServiceDescription(
-        name="RecognizeTest",
+        "RecognizeTest",
         description="Recognize test service",
         host=Hosts.WS255.NAME,
         auto_start=False,
         auto_restart=False,
         visible_for_admin=False,
     )
 
     """INDICATIONS = ServiceDescription(
-        name="Indications",
+        "Indications",
         description="Indications service",
         host=HOSTS.WS255.NAME,
     )"""
 
     MEDICAL_AUTOMATION = ServiceDescription(
-        name="MedicalAutomation",
+        "MedicalAutomation",
         description="Medical Automation service",
         host=Hosts.BACKUP_WORKER.NAME,
     )
 
-    REGISTRATOR_HELPER = ServiceDescription(name="RegistratorHelper")
+    REGISTRATOR_HELPER = ServiceDescription("RegistratorHelper")
 
     DEVELOPER = ServiceDescription(
-        name="Developer",
+        "Developer",
         description="Developer service",
         host=Hosts.DEVELOPER.NAME,
         port=RPC.PORT(1),
         visible_for_admin=False,
         auto_start=False,
         auto_restart=False,
         commands=(ServiceCommands.test,),
```

### Comparing `pih-0.36.9/pih/consts/settings.py` & `pih-0.37/pih/consts/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,45 @@
 from enum import Enum
+from pih.consts import CONST
 from pih.consts.polibase import POLIBASE
 from pih.collections import (
     StorageVariableHolder,
     IntStorageVariableHolder,
     BoolStorageVariableHolder,
     TimeStorageVariableHolder,
     FloatStorageVariableHolder,
     IntListStorageVariableHolder,
     DateListStorageVariableHolder,
+    IntVariantableStorageVariableHolder,
     StringListStorageVariableHolder,
 )
 
 
 class SETTINGS(Enum):
+
+    BONUS_PROGRAM_TEXT = StorageVariableHolder(
+        "BONUS_PROGRAM_TEXT",
+        POLIBASE.BONUS_PROGRAM_TEXT,
+    )
+
+    UNISENDER_API_KEY = StorageVariableHolder(
+        "UNISENDER_API_KEY",
+        "65ddrin3zh791hxarbkwe4fmah5p44hkg4cjwsuy",
+    )
+
+    UNISENDER_API_LIST_IDS = StorageVariableHolder(
+        "UNISENDER_API_LIST_IDS",
+        "761",
+    )
+
+    PIH_CLI_ADMINISTRATOR_LOGIN = StorageVariableHolder(
+        "PIH_CLI_ADMINISTRATOR_LOGIN",
+        "nak",
+    )
+
     REVIEW_ACTION_URL = StorageVariableHolder(
         "REVIEW_ACTION_URL",
         POLIBASE.REVIEW_ACTION_URL,
     )
 
     REVIEW_ACTION_URL_FOR_INPATIENT = StorageVariableHolder(
         "REVIEW_ACTION_URL_FOR_INPATIENT",
@@ -101,39 +124,46 @@
         "POLIBASE_PERSON_REVIEW_NOTIFICATION_TEXT",
         POLIBASE.PERSON_REVIEW_NOTIFICATION_TEXT,
     )
 
     TIME_TRACKING_FOR_POLYCLINIC = StringListStorageVariableHolder(
         "TIME_TRACKING_FOR_POLYCLINIC",
         (
-            "190",
             "035",
+            "045",
             "058",
             "101-0-",
+            "124",
             "125",
             "131",
+            "137",
             "139",
             "177",
-            "124",
             "183",
-            "045"
+            "190",
         ),
     )
 
     POLIBASE_PERSON_REVIEW_NOTIFICATION_START_TIME = TimeStorageVariableHolder(
-        "POLIBASE_PERSON_REVIEW_NOTIFICATION_START_TIME", "23:00"
+        "POLIBASE_PERSON_REVIEW_NOTIFICATION_START_TIME", "20:00"
     )
     #
     RESOURCE_MANAGER_CHECK_SITE_CERTIFICATE_START_TIME = TimeStorageVariableHolder(
         "RESOURCE_MANAGER_CHECK_SITE_CERTIFICATE_START_TIME", "8:00"
     )
     #
     POLIBASE_CREATION_DB_DUMP_START_TIME = TimeStorageVariableHolder(
         "POLIBASE_CREATION_DB_DUMP_START_TIME", "20:30"
     )
+    POLIBASE_DB_DUMP_ARCHIVE_COMPRESSION_LEVEL = IntVariantableStorageVariableHolder(
+        "POLIBASE_DB_DUMP_ARCHIVE_COMPRESSION_LEVEL", 5, variants=(0, 1, 3, 5, 7, 9)
+    )
+    POLIBASE_DB_DUMP_ARCHIVE_CREATION_PARAMETERS = StorageVariableHolder(
+        "POLIBASE_DB_DUMP_ARCHIVE_CREATION_PARAMETERS", None
+    )
     #
     RESOURCE_MANAGER_CHECK_SITE_FREE_SPACE_PERIOD_IN_MINUTES = IntStorageVariableHolder(
         "RESOURCE_MANAGER_CHECK_SITE_FREE_SPACE_PERIOD_IN_MINUTES", 15
     )
     #
     PRINTER_REPORT_PERIOD_IN_MINUTES = IntStorageVariableHolder(
         "PRINTER_REPORT_PERIOD_IN_MINUTES", 5
@@ -197,14 +227,19 @@
         "POLIBASE_PERSON_VISIT_REMINDER_TEXT",
         POLIBASE.PERSON_VISIT_NOTIFICATION_HEADER
         + "*{name}*, напоминаем Вам о записи сегодня {visit_time}. Вы записаны на {appointment_information}."
         + POLIBASE.PERSON_VISIT_NOTIFICATION_TEXT_CANCEL_OR_REPLACE_RECEPTION
         + POLIBASE.HAVE_A_GOOD_DAY,
     )
 
+    POLIBASE_PERSON_PRERECORDING_VISIT_NOTIFICATION = StorageVariableHolder(
+        "POLIBASE_PERSON_PRERECORDING_VISIT_NOTIFICATION",
+        POLIBASE.POLIBASE_PERSON_PRERECORDING_VISIT_NOTIFICATION,
+    )
+
     POLIBASE_PERSON_TAKE_TELEGRAM_BOT_URL_TEXT = StorageVariableHolder(
         "POLIBASE_PERSON_TAKE_TELEGRAM_BOT_URL_TEXT",
         POLIBASE.TAKE_TELEGRAM_BOT_URL_TEXT,
     )
 
     POLIBASE_PERSON_TAKE_TELEGRAM_BOT_URL_PERSONLESS_TEXT = StorageVariableHolder(
         "POLIBASE_PERSON_TAKE_TELEGRAM_BOT_URL_PERSONLESS_TEXT",
@@ -212,31 +247,126 @@
     )
 
     POLIBASE_PERSON_TAKE_REVIEW_ACTION_URL_TEXT = StorageVariableHolder(
         "POLIBASE_PERSON_TAKE_REVIEW_ACTION_URL_TEXT",
         POLIBASE.TAKE_REVIEW_ACTION_URL_TEXT,
     )
 
+    POLIBASE_PERSON_ANSWER_TAX_CERTIFICATE_TEXT = StorageVariableHolder(
+        "POLIBASE_PERSON_PERSON_TAX_CERTIFICATE_TEXT",
+        POLIBASE.PERSON_TAX_CERTIFICATE_TEXT,
+    )
+
     POLIBASE_PERSON_REVIEW_NOTIFICATION_DOCTOR_PERSON_PIN_LIST = (
         IntListStorageVariableHolder(
             "POLIBASE_PERSON_REVIEW_NOTIFICATION_DOCTOR_PERSON_PIN_LIST",
             POLIBASE.POLIBASE_PERSON_REVIEW_NOTIFICATION_DOCTOR_PERSON_PIN_LIST,
             "Список врачей, участвующих в отзывах",
         )
     )
 
-    BONUS_DOCTOR_PERSON_PIN_LIST = IntListStorageVariableHolder(
-        "BONUS_DOCTOR_PERSON_PIN_LIST",
-        POLIBASE.BONUS_DOCTOR_PERSON_PIN_LIST,
+    TELEGRAM_BOT_URL = StorageVariableHolder(
+        "TELEGRAM_BOT_URL", POLIBASE.TELEGRAM_BOT_URL
+    )
+
+    TAX_CERTIFICATE_URL = StorageVariableHolder(
+        "TAX_CERTIFICATE_URL", POLIBASE.TAX_CERTIFICATE_URL
+    )
+
+    BONUS_PROGRAM_IS_ON = BoolStorageVariableHolder(
+        "BONUS_PROGRAM_IS_ON",
+        False,
+    )
+
+    BONUS_PROGRAM_TEST_POLIBASE_PERSON_PIN = IntStorageVariableHolder(
+        "BONUS_PROGRAM_TEST_POLIBASE_PERSON_PIN",
+        37068,
+    )
+
+    BONUS_PROGRAM_DISCOUNT_PERCENT = IntStorageVariableHolder(
+        "BONUS_PROGRAM_DISCOUNT_PERCENT",
+        50,
+    )
+
+    BONUS_PROGRAM_CASHBACK_PERCENT = IntStorageVariableHolder(
+        "BONUS_PROGRAM_CASHBACK_PERCENT",
+        3,
+    )
+
+    BONUS_PROGRAM_BONUS_MINIMUM = IntStorageVariableHolder(
+        "BONUS_PROGRAM_BONUS_MINIMUM",
+        10,
+    )
+
+    BONUS_PROGRAM_NOTIFICATION_COUNT_MAX = IntStorageVariableHolder(
+        "BONUS_PROGRAM_NOTIFICATION_COUNT_MAX",
+        3,
+    )
+
+    BONUS_PROGRAM_DOCTOR_PERSON_PIN_LIST = IntListStorageVariableHolder(
+        "BONUS_PROGRAM_DOCTOR_PERSON_PIN_LIST",
+        POLIBASE.BONUS_PROGRAM_DOCTOR_PERSON_PIN_LIST,
     )
 
     POLIBASE_DOCTEMPLATE_THRESHOLD = IntStorageVariableHolder(
         "POLIBASE_DOCTEMPLATE_THRESHOLD", 100
     )
 
+    POLIBASE_ANSWER_PERSON_TAX_CERTIFICATE_VARIANTS = StringListStorageVariableHolder(
+        "POLIBASE_ANSWER_PERSON_TAX_CERTIFICATE_VARIANTS",
+        POLIBASE.TAX_CERTIFICATE_VARIANTS,
+    )
+
+    POLIBASE_PERSON_ANSWER_VISIT_MODIFICATION_VARIANTS = (
+        StringListStorageVariableHolder(
+            "POLIBASE_PERSON_ANSWER_VISIT_MODIFICATION_VARIANTS",
+            POLIBASE.PERSON_VISIT_MODIFICATION_VARIANTS,
+        )
+    )
+
+    POLIBASE_PERSON_ANSWER_HOW_TO_GET_VARIANTS = StringListStorageVariableHolder(
+        "POLIBASE_PERSON_ANSWER_HOW_TO_GET_VARIANTS",
+        POLIBASE.ANSWER_HOW_TO_GET_VARIANTS,
+    )
+
+    POLIBASE_PERSON_ANSWER_OTHER_QUESTION_TEXT = StorageVariableHolder(
+        "POLIBASE_PERSON_ANSWER_OTHER_QUESTION_TEXT",
+        POLIBASE.ANSWER_OTHER_QUESTION_TEXT,
+    )
+
+    POLIBASE_PERSON_ANSWER_VISIT_MODIFICATION_TEXT = StorageVariableHolder(
+        "POLIBASE_PERSON_ANSWER_VISIT_MODIFICATION_TEXT",
+        POLIBASE.ANSWER_VISIT_MODIFICATION_TEXT,
+    )
+
+    POLIBASE_PERSON_ANSWER_HOW_TO_GET_TEXT = StorageVariableHolder(
+        "POLIBASE_PERSON_ANSWER_HOW_TO_GET_TEXT",
+        CONST.ADDRESS.TEXT,
+    )
+
+    POLIBASE_PERSON_ANSWER_HOW_TO_GET_TEXT1 = StorageVariableHolder(
+        "POLIBASE_PERSON_ANSWER_HOW_TO_GET_TEXT1",
+        "Схема входов",
+    )
+
+    POLIBASE_PERSON_ANSWER_HOW_TO_GET_TEXT2 = StorageVariableHolder(
+        "POLIBASE_PERSON_ANSWER_HOW_TO_GET_TEXT2",
+        "Схема маршрута ж/д вокзал – больница Pacific Hospital.\nАвтобусы: *13*, *49* (ост. Диагностический центр)",
+    )
+
+    POLIBASE_PERSON_ANSWER_HOW_TO_GET_TEXT3 = StorageVariableHolder(
+        "POLIBASE_PERSON_ANSWER_HOW_TO_GET_TEXT3",
+        "Схема маршрута ж/д вокзал - больница Pacific Hospital на такси (средняя цена от 150 руб)",
+    )
+
+    POLIBASE_PERSON_ANSWER_HOW_TO_GET_TEXT4 = StorageVariableHolder(
+        "POLIBASE_PERSON_ANSWER_HOW_TO_GET_TEXT4",
+        "Схема маршрута Автовокзал – больница Pacific Hospital.\nАвтобусы: *77* (ост. Мариинский театр)",
+    )
+
     POLIBASE_PERSON_YES_ANSWER_VARIANTS = StringListStorageVariableHolder(
         "POLIBASE_PERSON_YES_ANSWER_VARIANTS", POLIBASE.YES_ANSWER
     )
 
     POLIBASE_PERSON_NO_ANSWER_VARIANTS = StringListStorageVariableHolder(
         "POLIBASE_PERSON_NO_ANSWER_VARIANTS", POLIBASE.NO_ANSWER
     )
```

### Comparing `pih-0.36.9/pih/pih.py` & `pih-0.37/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,20 +41,21 @@
 import os
 
 import ipih
 from pih.rpc import *
 from pih.tools import *
 from pih.consts import *
 from pih.collections import *
+from pih.consts.style import *
+from pih.consts.iot import IOT
 from pih.consts.errors import *
 from pih.consts.polibase import *
 from pih.consts.python import PYTHON
 from pih.consts.events import Events
 from pih.consts.zabbix import ZABBIX
-from pih.consts.iot import IOT
 from pih.consts.settings import SETTINGS
 from pih.consts.ssh_hosts import SSHHosts
 from pih.consts.rpc import RPC as CONST_RPC
 from pih.consts.addresses import ADDRESSES, EMAIL_COLLECTION
 from pih.tools.service import ServiceRoleTool, ServiceTool, ServiceAdminTool
 from pih.consts.service import SUPPORT_NAME_PREFIX, EVENT_LISTENER_NAME_PREFIX
 
@@ -65,17 +66,14 @@
 
     wrapper: Callable
 
     def submit(self, fn, /, *args, **kwargs):
         return super().submit(PIHThreadPoolExecutor.wrapper(fn), *args, **kwargs)
 
 
-CACHE: dict[str, bool] = {}
-
-
 class PIHThread(Thread):
     def __init__(
         self,
         target: Callable,
         auto_start: bool = True,
         group=None,
         name=None,
@@ -97,19 +95,20 @@
             daemon=daemon,
         )
         if auto_start:
             self.start()
 
 
 class OutputStubAbstract:
+
     def b(self, value: str) -> str:
-        pass
+        raise NotImplemented()
 
     def i(self, value: str) -> str:
-        pass
+        raise NotImplemented()
 
 
 class OutputStub(OutputStubAbstract):
 
     def b(self, value: Any) -> str:
         return str(value)
 
@@ -177,15 +176,15 @@
 
     def set_indent(self, count: int = 1) -> None:
         raise NotImplemented()
 
     def bold(self, value: str) -> str:
         raise NotImplemented()
 
-    def header(self, caption: str) -> None:
+    def paragraph(self, caption: str) -> None:
         raise NotImplemented()
 
     def reset_indent(self) -> None:
         raise NotImplemented()
 
     def restore_indent(self) -> None:
         raise NotImplemented()
@@ -216,15 +215,46 @@
         text_after: str | None = None,
     ) -> None:
         raise NotImplemented()
 
     def write_line(self, text: str) -> None:
         raise NotImplemented()
 
-    def index(self, index: int, text: str, max_index: int | None = None) -> None:
+    def index(
+        self,
+        text: str,
+        min_value: int | None = None,
+        max_value: int | None = None,
+    ) -> None:
+        raise NotImplemented()
+
+    def indexed_item(
+        self,
+        index: int,
+        text: str,
+        min_value: int | None = None,
+        max_value: int | None = None,
+    ) -> None:
+        raise NotImplemented()
+
+    def indexed_item_str(
+        self,
+        index: int | None,
+        text: str,
+        min_value: int | None = None,
+        max_value: int | None = None,
+    ) -> str:
+        raise NotImplemented()
+
+    def index_str(
+        self,
+        caption: str,
+        min_value: int,
+        max_value: int,
+    ) -> str:
         raise NotImplemented()
 
     def input(self, caption: str) -> None:
         raise NotImplemented()
 
     def input_str(
         self,
@@ -402,19 +432,20 @@
 
 class MarkOutputBase(MarkOutputAbstract):
     def __init__(self):
         self.parent: OutputBase
 
 
 class MarkOutput(MarkOutputBase):
+
     def by_any(self, value: str) -> None:
         try:
             self.result(PIH.RESULT.MARK.by_any(value), "Найденные карты доступа:", True)
         except NotFound as error:
-            self.parent.error(error.get_details())
+            raise error
 
     def result(
         self, result: Result[list[Mark]], caption: str, use_index: bool = False
     ) -> None:
         self.parent.table_with_caption_first_title_is_centered(
             result, caption, use_index
         )
@@ -632,40 +663,45 @@
         by_index: bool = False,
     ) -> str:
         raise NotImplemented()
 
     def indexed_field_list(self, caption: str, list: FieldItemList) -> str:
         raise NotImplemented()
 
+    def date_period(
+        self, start_date_value: str | None = None, end_date_value: str | None = None
+    ) -> tuple[datetime, datetime]:
+        raise NotImplemented()
+
     def index(
         self,
         caption: str,
-        data: list,
-        label_function: Callable[[Any, int], str] = None,
+        data: list[Any],
+        label_function: Callable[[Any, int], str] | None = None,
         use_zero_index: bool = False,
     ) -> int:
         raise NotImplemented()
 
     def item_by_index(
         self,
         caption: str,
         data: list[Any],
-        label_function: Callable[[Any, int], str] = None,
+        label_function: Callable[[Any, int], str] | None = None,
         use_zero_index: bool = False,
     ) -> Any:
         raise NotImplemented()
 
     def tab_number(self, check: bool = True) -> str:
         raise NotImplemented()
 
     def password(
         self,
         secret: bool = True,
         check: bool = False,
-        settings: PasswordSettings = None,
+        settings: PasswordSettings | None = None,
         is_new: bool = True,
     ) -> str:
         raise NotImplemented()
 
     def same_if_empty(self, caption: str, src_value: str) -> str:
         raise NotImplemented()
 
@@ -677,15 +713,15 @@
 
     def yes_no(
         self,
         text: str = " ",
         enter_for_yes: bool = False,
         yes_label: str | None = None,
         no_label: str | None = None,
-        yes_checker: Callable[[str], bool] = None,
+        yes_checker: Callable[[str], bool] | None = None,
     ) -> bool:
         raise NotImplemented()
 
     def message_for_user_by_login(self, login: str) -> str:
         raise NotImplemented()
 
     def polibase_person_any(self, title: str | None = None) -> str:
@@ -778,55 +814,55 @@
 
 
 class InputBase(InputAbstract):
     def __init__(self):
         self.output: OutputBase
         self.mark: MarkInputBase
         self.user: UserInputBase
+        self.type: int = INPUT_TYPE.NO
 
 
 class OutputBase(OutputAbstract, OutputExtendedAbstract):
     def __init__(
         self,
         user_output: UserOutputBase | None = None,
         mark_output: MarkOutputBase | None = None,
     ):
         self.text_before: str = ""
         self.text_after: str = ""
         self.indent_symbol: str = " "
         self.indent_value: int = 0
-        self.user: UserOutputBase = user_output
+        self.user: UserOutputBase | None = user_output
         self.user.parent = self
-        self.mark: MarkOutputBase = mark_output
+        self.mark: MarkOutputBase | None = mark_output
         self.mark.parent = self
         self.personalize = False
+        # self.parent: InputBase | None = None
 
 
 class SessionAbstract:
     def run_forever_untill_enter_not_pressed(self) -> None:
         raise NotImplemented()
 
-    def exit(self, timeout: int = None, message: str | None = None) -> None:
+    def exit(self, timeout: float | None = None, message: str | None = None) -> None:
         raise NotImplemented()
 
     def get_login(self) -> str:
         raise NotImplemented()
 
     def get_user(self) -> User:
         raise NotImplemented()
 
     def user_given_name(self) -> str:
         raise NotImplemented()
 
     def start(self, login: str, notify: bool = True) -> None:
         raise NotImplemented()
 
-    def say_hello(
-        self, telephone_number: str | None = None, greeting: bool = True
-    ) -> None:
+    def hello(self, greeting: bool = True, fill_groups: bool = False) -> None:
         raise NotImplemented()
 
     @property
     def argv(self) -> list[str]:
         raise NotImplemented()
 
     def arg(self, index: int = None, default_value: str | None = None) -> str:
@@ -864,15 +900,23 @@
         self.flags: int = flags
 
     def add_allowed_group(self, value: AD.Groups) -> None:
         self.allowed_groups.append(value)
 
     @property
     def is_mobile(self) -> bool:
-        return self.name == "mobile"
+        return self.name == SESSION_TYPE.MOBILE
+
+    @property
+    def is_outside(self) -> bool:
+        return self.name == SESSION_TYPE.OUTSIDE
+
+    @property
+    def am_i_admin(self) -> bool:
+        return AD.Groups.Admin in self.allowed_groups
 
 
 class Session(SessionBase):
     def __init__(
         self, input: InputBase | None = None, output: OutputBase | None = None
     ):
         super().__init__(input, output)
@@ -886,20 +930,18 @@
     def run_forever_untill_enter_not_pressed(self) -> None:
         try:
             self.output.green("Нажмите Ввод для выхода...")
             input()
         except KeyboardInterrupt:
             pass
 
-    def exit(self, timeout: int = None, message: str | None = None) -> None:
-        if message is not None:
+    def exit(self, timeout: float | None = None, message: str | None = None) -> None:
+        if nn(message):
             self.output.error(message)
-        if timeout is None:
-            timeout = 5
-        sleep(timeout)
+        sleep(timeout or 5)
         exit()
 
     def get_login(self) -> str:
         if n(self.login):
             self.start(PIH.SYS.get_login())
         return self.login
 
@@ -914,28 +956,37 @@
 
     def start(self, login: str, notify: bool = True) -> None:
         if n(self.login):
             self.login = login
             if notify:
                 PIH.EVENT.start_session()
 
-    def say_hello(self, _: str | None = None, greeting: bool = True) -> None:
+    def hello(self, greeting: bool = True, fill_access_groups: bool = False) -> None:
         user: User = self.get_user()
-        if nn(user):
-            if greeting:
-                self.output.good(js(("Добро пожаловать,", user.name)))
-                self.output.new_line()
+        if n(user):
+            self.output.error("Ты кто такой? Давай, до свидания...")
+            self.exit()
             return
-        self.output.error(f"Ты кто такой? Давай, до свидания...")
-        self.exit()
+        if greeting:
+            self.output.good(js(("Добро пожаловать,", user.name)))
+            self.output.new_line()
+        if fill_access_groups:
+            self.fill_access_groups()
+
+    def fill_access_groups(self) -> None:
+        PIH.CHECK.ACCESS.action_for_all_groups(self, False, False, False, True)
 
     @property
     def argv(self) -> list[str]:
         return sys.argv[1:] if len(sys.argv) > 1 else []
 
+    @property
+    def arg_list(self) -> list[str]:
+        return self.argv
+
     def arg(self, index: int = 0, default_value: Any = None) -> str | Namespace:
         return DataTool.by_index(self.argv, index, default_value)
 
     @property
     def arg_namespace(self) -> Namespace:
         return self.arg_parser.parse_args()
 
@@ -980,27 +1031,35 @@
                 return True
             self.output.green("Инициализация...")
             self.output.clear_screen()
             self.output.pih_title()
             if PIH.SERVICE.check_on_accessibility(ServiceRoles.AD):
                 login: str = PIH.SYS.get_login()
                 self.output.head1(
-                    f"{FullNameTool.to_given_name(PIH.RESULT.USER.by_login(login, cached=False).data.name)}, пожалуйста, пройдите аутентификацию..."
+                    j(
+                        (
+                            FullNameTool.to_given_name(
+                                PIH.RESULT.USER.by_login(login, cached=False).data.name
+                            ),
+                            " пожалуйста, пройдите аутентификацию...",
+                        )
+                    )
                 )
                 self.output.new_line()
-                if not self.input.yes_no(f"Использовать логин '{login}'", True):
+                if not self.input.yes_no(js(("Использовать логин", escs(login))), True):
                     login = PIH.input.login()
                 password: str = PIH.input.password(is_new=False)
                 if DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.authenticate, (login, password)
                     )
                 ):
                     self.authenticated = True
                     self.start(login, False)
+                    self.fill_access_groups()
                     PIH.EVENT.login()
                     self.output.good(
                         self.output.text_black(
                             f"Добро пожаловать, {self.get_user().name}..."
                         )
                     )
                     return True
@@ -1042,17 +1101,17 @@
             self.set_indent(indent)
 
     def set_indent(self, value: int) -> None:
         self.indent_value = value
         self.text_before = self.indent_symbol * value
 
     def bold(self, value: str) -> str:
-        return j((CSI, "1m", value, CSI, "0m"))
+        return j((CSI, "1m", value, CSI, "22m"))
 
-    def italic(self, value: str) -> str:
+    def italics(self, value: str) -> str:
         return value
 
     def reset_indent(self) -> None:
         self.indent_value = 0
         self.text_before = ""
 
     @property
@@ -1091,37 +1150,70 @@
         text: str,
         text_before: str | None = None,
         text_after: str | None = None,
     ) -> None:
         self.write_line(self.color_str(color, text, text_before, text_after))
 
     def write_line(self, text: str) -> None:
+        text = PIH.DATA.FORMAT.console_message(text)
         print(
             jnl(
                 DataTool.map(
                     lambda item: j((self.text_before, item)), text.splitlines()
                 )
             )
         )
 
     @contextmanager
     def personalized(self):
         pass
 
-    def index(self, index: int, text: str, max_index: int | None = None) -> None:
+    def indexed_item_str(
+        self,
+        index: int | None,
+        text: str,
+        min_value: int | None = None,
+        max_value: int | None = None,
+    ) -> str:
         indent: str = ""
-        if max_index is not None:
-            indent = " " * (len(str(max_index)) - len(str(index)))
-        if index is None:
-            self.write_line(j((indent, text)))
-        else:
-            self.write_line(j((index, ". ", indent, text)))
+        if nn(max_value):
+            indent = " " * (len(str(max_value)) - len(str(index)))
+        return j((indent, text)) if n(index) else j((index, ". ", indent, text))
+
+    def indexed_item(
+        self,
+        index: int,
+        text: str,
+        min_value: int | None = None,
+        max_value: int | None = None,
+    ) -> None:
+        self.write_line(self.indexed_item_str(index, text, min_value, max_value))
+
+    def index(
+        self,
+        caption: str,
+        min_value: int,
+        max_value: int,
+    ) -> None:
+        self.write_line(self.index_str(caption, min_value, max_value))
+
+    def index_str(
+        self,
+        text: str,
+        min_value: int,
+        max_value: int,
+    ) -> str:
+        return js(
+            (j((text, ", отправив число")), "(от", min_value, "до", j((max_value, ")")))
+        )
 
     def input(self, caption: str) -> None:
-        self.write_line(self.input_str(caption, self.text_before, text_after=":"))
+        self.write_line(
+            self.input_str(caption, self.text_before, text_after=CONST.SPLITTER)
+        )
 
     def input_str(
         self,
         caption: str,
         text_before: str | None = None,
         text_after: str | None = None,
     ) -> str:
@@ -1212,21 +1304,23 @@
 
     def white(
         self, text: str, text_before: str | None = None, text_after: str | None = None
     ) -> None:
         self.write_line(self.white_str(text, text_before, text_after))
 
     def draw_line(
-        self, color: str = Back.LIGHTBLUE_EX, char: str = " ", width: int = 80
+        self, color: int = Back.LIGHTBLUE_EX, char: str = " ", width: int = 80
     ) -> None:
         self.write_line("") if color is None else self.color(color, char * width)
 
     def line(self) -> None:
         self.new_line()
-        self.draw_line(Back.WHITE, self.text_color(Fore.BLACK, "_"), width=128)
+        self.draw_line(
+            Back.WHITE, self.text_color(Fore.BLACK, CONST.NAME_SPLITTER), width=128
+        )
         self.new_line()
 
     def magenta_str(
         self, text: str, text_before: str | None = None, text_after: str | None = None
     ) -> str:
         return self.color_str(Back.LIGHTMAGENTA_EX, text, text_before, text_after)
 
@@ -1275,15 +1369,15 @@
     ) -> str:
         return self.color_str(Style.BRIGHT, text, text_before, text_after)
 
     @staticmethod
     def get_number(value: int) -> str:
         return CONST.VISUAL.NUMBER_SYMBOLS[value]
 
-    def header(self, caption: str) -> None:
+    def paragraph(self, caption: str) -> None:
         self.head2(caption)
 
     @contextmanager
     def make_separated_lines(self):
         yield True
 
     @contextmanager
@@ -1322,15 +1416,15 @@
         data: list = DataTool.as_list(result.data)
         result_string_list: list[str] | None = None
         if e(data):
             self.new_line()
             self.write_line(empty_result_text)
         else:
             if ne(title):
-                self.write_line(self.bold(title))
+                self.write_line(b(title))
             with self.make_indent(2, True):
                 for index, data_item in enumerate(data):
                     result_string_list = []
                     if use_index and len(data) > 1:
                         result_string_list.append(j((self.text_before, index + 1, ":")))
                     if n(label_function):
                         field: FieldItem
@@ -1353,15 +1447,15 @@
                             if e(item_data_value):
                                 if data_label_function is None:
                                     continue
                             default_value_label_function: Callable[
                                 [int, FieldItem, Result[T], Any], tuple[bool, str]
                             ] = lambda _, field, __, data_value: (
                                 True,
-                                j((self.bold(field.caption), ": ", data_value)),
+                                j((b(field.caption), ": ", data_value)),
                             )
                             result_data_label_function: Callable[
                                 [int, FieldItem, T, Any], tuple[bool, str]
                             ] = (data_label_function or default_value_label_function)
                             label_value_result: tuple[bool, str | None] = (
                                 result_data_label_function(
                                     index, field, data_item, item_data_value
@@ -1488,15 +1582,15 @@
     ) -> None:
         group_name: str = group.GroupName
         self.table_with_caption_last_title_is_centered(
             result,
             js(
                 (
                     "Свободные карты доступа для группы доступа",
-                    j((self.b(group_name), ":")),
+                    j((b(group_name), ":")),
                 )
             ),
             use_index,
         )
 
     def temporary_marks(
         self,
@@ -1641,20 +1735,23 @@
 
 class Input(InputBase):
     def __init__(
         self, user_input: UserInputBase, mark_input: MarkInputBase, output: OutputBase
     ):
         self.output: OutputBase = output
         self.answer: str | None = None
+        self.index_min_value: int = -1
+        self.index_max_value: int = -1
         if nn(user_input):
             self.user: UserInputBase = user_input
             self.user.parent = self
         if nn(mark_input):
             self.mark: MarkInputBase = mark_input
             self.mark.parent = self
+        # self.output.parent = self
 
     def input(
         self,
         caption: str | None = None,
         new_line: bool = True,
         check_function: Callable[[str], str] | None = None,
     ) -> str:
@@ -1662,25 +1759,95 @@
             while True:
                 if new_line and nn(caption):
                     with self.output.make_indent(0):
                         self.output.input(caption)
                 value: str = (
                     input(self.output.text_before)
                     if new_line
-                    else input(self.output.text_before + caption)
+                    else input(js((self.output.text_before + caption)))
                 )
                 if nn(check_function):
                     value_after: str = check_function(value)
                     if nn(value_after):
                         return value_after
                 else:
                     return value
         except KeyboardInterrupt as _:
             raise KeyboardInterrupt()
 
+    def date_period(
+        self, start_date_string: str | None = None, end_date_string: str | None = None
+    ) -> tuple[date, date]:
+        today_date: date = PIH.DATA.today()
+
+        def get_date_format(value: str) -> str:
+            value = value.strip()
+            return (
+                CONST.YEARLESS_DATE_FORMAT
+                if value.count(CONST.DATE_PART_DELIMITER) == 1 or value.count(" ") == 1
+                else CONST.DATE_FORMAT
+            )
+
+        value: str | None = start_date_string
+        format: str | None = None if e(value) else get_date_format(nns(value))
+        start_date: date | None = PIH.DATA.EXTRACT.date(value, nns(format))
+        if ne(start_date):
+            if format == CONST.YEARLESS_DATE_FORMAT:
+                start_date = nnt(start_date).replace(today_date.year)
+        value = end_date_string
+        format = None if e(value) else get_date_format(value)
+        end_date: date | None = PIH.DATA.EXTRACT.date(value, nns(format))
+        if ne(end_date):
+            if format == CONST.YEARLESS_DATE_FORMAT:
+                end_date = end_date.replace(today_date.year)
+        while True:
+            if e(start_date):
+                value = self.input(
+                    j(
+                        (
+                            "Введите начало периода, в формате ",
+                            b("ДЕНЬ.МЕСЯЦ"),
+                            ", например ",
+                            PIH.DATA.today_string(CONST.YEARLESS_DATE_FORMAT),
+                        )
+                    )
+                )
+                value = PIH.DATA.FORMAT.to_date(value)
+                format = get_date_format(value)
+                if format == CONST.YEARLESS_DATE_FORMAT:
+                    value = jp((value, today_date.year))
+                start_date = PIH.DATA.EXTRACT.date(value, CONST.DATE_FORMAT)
+                if e(start_date) or nnt(start_date) > nnt(today_date):
+                    continue
+            if e(end_date) or nnt(start_date) > nnt(end_date):
+                if not self.yes_no(
+                    "Использовать сегодняшнюю дату",
+                    no_label=j(
+                        (
+                            "Введите окончание периода, в формате ",
+                            b("ДЕНЬ.МЕСЯЦ"),
+                            ", например ",
+                            PIH.DATA.today_string(CONST.YEARLESS_DATE_FORMAT),
+                        )
+                    ),
+                ):
+                    value = PIH.DATA.FORMAT.to_date(self.answer)
+                    format = get_date_format(value)
+                    if format == CONST.YEARLESS_DATE_FORMAT:
+                        value = jp((value, today_date.year))
+                    end_date = PIH.DATA.EXTRACT.date(value, CONST.DATE_FORMAT)
+                    if e(end_date):
+                        continue
+                else:
+                    end_date = PIH.DATA.today(as_datetime=True)
+            if not (e(start_date) or e(end_date)):
+                break
+
+        return (start_date, end_date)
+
     def polibase_persons_by_any(
         self, value: str | None = None, title: str | None = None, use_all: bool = False
     ) -> list[PolibasePerson]:
         result: Result[list[PolibasePerson]] = PIH.RESULT.POLIBASE.persons_by_any(
             value or self.polibase_person_any(title)
         )
         label_function: Callable[[Any, int], str] | None = (
@@ -1692,27 +1859,27 @@
             result.data.append(None)
         polibase_person: PolibasePerson = self.item_by_index(
             "Выберите пользователя, введя индекс", result.data, label_function
         )
         return result.data if n(polibase_person) else [polibase_person]
 
     def telephone_number(
-        self, format: bool = True, telephone_prefix: str = CONST.TELEPHONE_NUMBER_PREFIX
+        self, format: bool = True, prefix: str | None = CONST.TELEPHONE_NUMBER_PREFIX
     ) -> str:
         while True:
             self.output.input("Введите номер телефона")
-            use_telephone_prefix: bool = telephone_prefix is not None
-            telephone_number: str = self.input(telephone_prefix, False)
+            use_telephone_prefix: bool = nn(prefix)
+            telephone_number: str = self.input(prefix, False)
             if use_telephone_prefix:
-                if not telephone_number.startswith(telephone_prefix):
-                    telephone_number = telephone_prefix + telephone_number
+                if not telephone_number.startswith(prefix):
+                    telephone_number = j((prefix, telephone_number))
             check: bool | None = None
             if format:
                 telehone_number_after_fix = PIH.DATA.FORMAT.telephone_number(
-                    telephone_number, telephone_prefix
+                    telephone_number, prefix
                 )
                 check = PIH.CHECK.telephone_number(telehone_number_after_fix)
                 if check and telehone_number_after_fix != telephone_number:
                     telephone_number = telehone_number_after_fix
                     self.output.value("Телефон отформатирован", telephone_number)
             if check or PIH.CHECK.telephone_number(telephone_number):
                 return telephone_number
@@ -1786,66 +1953,102 @@
         caption: str,
         data: list[Any],
         label_function: Callable[[Any, int], str] | None = None,
         use_zero_index: bool = False,
         use_free_input: bool = False,
         text_after: str | None = None,
         allow_choose_all: bool = False,
+        sticky_items: tuple[int, ...] | None = None,
     ) -> int | str:
+        NO_INDEX: int = -1
+        length: int = len(data)
         use_zero_index = allow_choose_all or use_zero_index
+        zero_index_value: int = int(use_zero_index)
         value: str | None = None
-        selected_index: int = -1
-        length: int = len(data)
+        selected_index: int = NO_INDEX
         has_error: bool = False
-        zero_index_value: int = int(use_zero_index)
-        min_value: int = 1 - zero_index_value
-        max_value: int = length - zero_index_value + int(allow_choose_all)
-        index_caption: str = js((caption, "(от", min_value, "до", j((max_value, ")"))))
+        self.index_min_value = 1 - zero_index_value
+        self.index_max_value = length - zero_index_value + int(allow_choose_all)
         if allow_choose_all:
             data.insert(0, jnl(("Выбрать всё", "...")))
+        if length == 1 and not use_free_input:
+            return 0
         with self.output.make_indent(1, True):
             while True:
-                if (
-                    not has_error
-                    and nn(label_function)
-                    and length > 1
-                    or use_free_input
-                ):
+                if not has_error and length > 1 or use_free_input:
+                    data_label_list: list[str] = []
                     for index, item in enumerate(data):
-                        self.output.index(
+                        data_label: str = (
+                            item
+                            if n(label_function) or (allow_choose_all and index == 0)
+                            else label_function(item, index)
+                        )
+                        self.output.indexed_item(
                             (
                                 index + 1 - zero_index_value
                                 if length > 1 or use_free_input
                                 else None
                             ),
-                            (
-                                item
-                                if allow_choose_all and index == 0
-                                else label_function(item, index)
-                            ),
-                            max_value,
-                        )
-                if length == 1 and not use_free_input:
-                    return zero_index_value
-                selected_index = PIH.DATA.EXTRACT.decimal(
-                    value := (
-                        self.input(index_caption)
-                        if n(text_after)
-                        else self.input(j((index_caption, text_after)))
-                    ),
-                    min_value,
-                    max_value,
-                    simple=True,
+                            data_label,
+                            self.index_min_value,
+                            self.index_max_value,
+                        )
+                        data_label_list.append(data_label)
+
+                selected_index = nni(
+                    PIH.DATA.EXTRACT.decimal(
+                        value := self.input(
+                            j(
+                                (
+                                    self.output.index_str(
+                                        caption,
+                                        self.index_min_value,
+                                        self.index_max_value,
+                                    ),
+                                    text_after,
+                                )
+                            )
+                        ),
+                        self.index_min_value,
+                        self.index_max_value,
+                        simple=True,
+                    ),
+                    selected_index,
                 )
-                if e(selected_index):
+                if selected_index == NO_INDEX:
                     if use_free_input:
                         return value
-                    selected_index = -1
+                    else:
+                        data_label_filtered_list: list[Any] = PIH.DATA.filter_by_string(
+                            value, data_label_list
+                        )
+                        if ne(data_label_filtered_list):
+                            if ne(sticky_items) and len(data_label_filtered_list) > 1:
+                                for index, item in enumerate(sticky_items):
+                                    data_label_filtered_list.insert(
+                                        index, data_label_list[item]
+                                    )
+                            return data_label_list.index(
+                                data_label_filtered_list[
+                                    int(
+                                        self.index(
+                                            caption,
+                                            data_label_filtered_list,
+                                            None,
+                                            use_zero_index,
+                                            use_free_input,
+                                            text_after,
+                                            allow_choose_all,
+                                            sticky_items,
+                                        )
+                                    )
+                                ]
+                            )
                 try:
-                    selected_index = int(selected_index) - min_value
+                    selected_index = int(selected_index) - self.index_min_value
                     if (
                         selected_index >= 0
                         and selected_index < length + zero_index_value
                     ):
                         return selected_index
                 except ValueError:
                     has_error = True
@@ -1854,22 +2057,24 @@
     def item_by_index(
         self,
         caption: str,
         data: list[Any],
         label_function: Callable[[Any, int], str] | None = None,
         use_zero_index: bool = False,
         allow_choose_all: bool = False,
+        sticky_items: tuple[int, ...] | None = None,
     ) -> Any | list[Any]:
         index: int = self.index(
             caption,
             data,
             label_function,
             use_zero_index,
             allow_choose_all=allow_choose_all,
-        )
+            sticky_items=sticky_items,
+        )  # type: ignore
         return data[1:] if allow_choose_all and index == 0 else data[index]
 
     def tab_number(self, check: bool = True) -> str:
         tab_number: str | None = None
         while True:
             tab_number = self.input("Введите номер карты доступа")
             if check:
@@ -1937,18 +2142,20 @@
         text: str = " ",
         enter_for_yes: bool = False,
         yes_label: str | None = None,
         no_label: str | None = None,
         yes_checker: Callable[[str], bool] | None = None,
     ) -> bool:
         text = self.output.blue_str(self.output.text_color(Fore.WHITE, text))
+        if nn(no_label):
+            no_label = j((no_label, " "))
         self.output.write_line(
-            f"{text}? \n{self.output.green_str(self.output.text_black('Да (1 или Ввод)'))} / {self.output.red_str(self.output.text_black('Нет (Остальное)'), '')}"
+            f"{text}? \n{self.output.green_str(self.output.text_black('Да (1 или Ввод)'))} / {self.output.red_str(no_label or self.output.text_black('Нет (Остальное)'), '')}"
             if enter_for_yes
-            else f"{text}? \n{self.output.red_str('Да (1)')} / {self.output.green_str(self.output.text_black('Нет (Остальное или Ввод)'), '')}"
+            else f"{text}? \n{self.output.red_str('Да (1)')} / {self.output.green_str(no_label or self.output.text_black('Нет (Остальное или Ввод)'), '')}"
         )
         answer: str = self.input()
         answer = answer.lower()
         self.answer = answer
         return (
             answer == "y"
             or answer == "yes"
@@ -1982,23 +2189,21 @@
         result: datetime = DateTimeTool.now(second=0)
         temp_datetime: datetime = result
         if n(use_date):
             use_date = not self.yes_no(
                 js(
                     (
                         "Использовать текущую дату",
-                        self.output.bold(
-                            DateTimeTool.datetime_to_string(result, CONST.DATE_FORMAT)
-                        ),
+                        b(DateTimeTool.datetime_to_string(result, CONST.DATE_FORMAT)),
                     )
                 )
             )
         while use_date and True:
             date_value: str | None = self.input(
-                js(("Введите дату в формате", self.output.bold("День.Месяц.Год")))
+                js(("Введите дату в формате", b("День.Месяц.Год")))
             ).lower()
             date_value = date_value.replace("ю", ".")
             dot_list: int = date_value.split(".")
             dot_count: int = len(dot_list)
             for i in range(dot_count):
                 dot_list = ListTool.not_empty_items(
                     DataTool.map(
@@ -2023,25 +2228,25 @@
                     break
         if ask_time_input and self.yes_no(js("Ввести время")):
             if n(use_time):
                 use_time = not self.yes_no(
                     js(
                         (
                             "Использовать текущее время",
-                            self.output.bold(
+                            b(
                                 DateTimeTool.datetime_to_string(
                                     result, CONST.SECONDLESS_TIME_FORMAT
                                 )
                             ),
                         )
                     )
                 )
             while use_time and True:
                 time_value: str | None = self.input(
-                    js(("Введите время в формате", self.output.bold("Час:Минуты")))
+                    js(("Введите время в формате", b("Час:Минуты")))
                 )
                 dot_list: int = time_value.split(":")
                 dot_count: int = len(dot_list)
                 for i in range(dot_count):
                     dot_list = ListTool.not_empty_items(
                         DataTool.map(
                             lambda item: str(PIH.DATA.EXTRACT.decimal(item)), dot_list
@@ -2062,20 +2267,27 @@
                             result = result.replace(minute=temp_datetime.minute)
                         break
         else:
             result = result.replace(minute=0, hour=0)
         return result
 
     def choose_file(
-        self, use_search_request: bool | None = None, allow_choose_all: bool = False
+        self,
+        use_search_request: bool | str | None = None,
+        allow_choose_all: bool = False,
     ) -> File | list[File]:
         if n(use_search_request):
-            use_search_request = self.yes_no("Использовать поиск")
+            use_search_request = self.yes_no("Использовать поиск", enter_for_yes=True)
         file_list: list[File] | None = None
-        search_request: str = self.input("Введите поисковый запрос")
+
+        search_request: str | None = None
+        if isinstance(use_search_request, str):
+            search_request = use_search_request
+        elif use_search_request:
+            search_request = self.input("Введите поисковый запрос")
         with self.output.make_loading(1, "Идет загрузка файлов. Ожидайте"):
             file_list = PIH.RESULT.FILES.find(
                 value=(search_request if use_search_request else None)
             ).data
         if e(file_list):
             self.output.error(
                 js(
@@ -2089,63 +2301,69 @@
             file_list = PIH.RESULT.FILES.all().data
 
         def label_function(file: File, _) -> str:
             title_list: list[str] = file.title.split(CONST.SPLITTER)
             if len(title_list) == 3:
                 return j(
                     (
-                        self.output.bold(title_list[0].upper()),
+                        b(title_list[0].upper()),
                         ": ",
                         title_list[-1],
                         " (",
                         title_list[-2],
                         ")",
                     )
                 )
-            return self.output.bold(title_list[1])
+            return b(title_list[1])
 
         return self.item_by_index(
             "Выберите файл",
             file_list,  # type: ignore
             label_function,
             allow_choose_all=allow_choose_all,
         )
 
     def choose_note(
-        self, use_search_request: bool | None = None, allow_choose_all: bool = False
+        self,
+        use_search_request: bool | str | None = None,
+        allow_choose_all: bool = False,
     ) -> Note:
         if n(use_search_request):
-            use_search_request = self.yes_no("Использвать поиск")
-        note_list: list[File] | None = None
-        search_request: str = self.input("Введите поисковый запрос")
+            use_search_request = self.yes_no("Использовать поиск", enter_for_yes=True)
+        note_list: list[Note] | None = None
+        search_request: str | None = None
+        if isinstance(use_search_request, str):
+            search_request = use_search_request
+        elif use_search_request:
+            search_request = self.input("Введите поисковый запрос")
         with self.output.make_loading(1, "Идет загрузка заметок. Ожидайте"):
             note_list = PIH.RESULT.NOTES.find(
                 search_request if use_search_request else None
             ).data
-            if e(note_list):
-                self.output.error(
-                    js(
-                        (
-                            "Файл с именем",
-                            esc(search_request),
-                            "не найден",
-                        )
+        if e(note_list):
+            self.output.error(
+                js(
+                    (
+                        "Файл с именем",
+                        esc(search_request),
+                        "не найден",
                     )
                 )
-                note_list = PIH.RESULT.NOTES.all().data
+            )
+            note_list = PIH.RESULT.NOTES.all().data
 
-            def label_function(note: Note, _) -> str:
-                return self.output.bold(note.title)
+        def label_function(note: Note, _) -> str:
+            return b(note.title)
 
-            return self.item_by_index(
-                "Выберите файл",
-                note_list,
-                label_function,
-                allow_choose_all=allow_choose_all,
-            )
+        return self.item_by_index(
+            "Выберите файл",
+            note_list,
+            label_function,
+            allow_choose_all=allow_choose_all,
+        )
 
 
 class MarkInput(MarkInputBase):
     def __init__(self, input: Input | None = None):
         self.parent = input
 
     def free(self, group: MarkGroup | None = None) -> Mark:
@@ -2298,17 +2516,15 @@
             result.data.append(None)
         result_data: User | None = self.parent.item_by_index(
             "Выберите пользователя, введя индекс",
             result.data,
             (
                 (
                     lambda item, _: (
-                        "Все"
-                        if n(item)
-                        else j((item.name, " (", item.samAccountName, ")"))
+                        "Все" if n(item) else j((item.name, " (", item.login, ")"))
                     )
                 )
                 if len(result.data) > 1
                 else None
             ),
         )
         return result.data if n(result_data) else [result_data]
@@ -2396,24 +2612,24 @@
             need_enter_login: bool = False
             if self.parent.yes_no(
                 "Удалить неактивных пользователей, чтобы освободить логин", True
             ):
                 user_for_remove: User = self.parent.item_by_index(
                     "Выберите пользователя для удаления, выбрав индекс",
                     inactive_user_list,
-                    lambda user, _: f"{user.name} ({user.samAccountName})",
+                    lambda user, _: f"{user.name} ({user.login})",
                 )
                 self.parent.output.new_line()
                 self.parent.output.value(
                     "Пользователь для удаления", user_for_remove.name
                 )
                 if self.parent.yes_no("Удалить неактивного пользователя", True):
                     if PIH.ACTION.USER.remove(user_for_remove):
                         self.parent.output.good("Удален")
-                        login_string = user_for_remove.samAccountName
+                        login_string = user_for_remove.login
                         inactive_user_list.remove(user_for_remove)
                     else:
                         self.parent.output.error("Ошибка")
                 else:
                     need_enter_login = True
             else:
                 need_enter_login = True
@@ -2598,14 +2814,43 @@
             ).data
             return nn(result) and (
                 n(result.timeout)
                 or (DateTimeTool.now() - result.timestamp).total_seconds()
                 < result.timeout
             )
 
+    class CACHE:
+
+        class TYPE:
+            REALTIME: int = 0
+            LOCAL: int = 1
+            REMOTE: int = 2
+
+        cache_type: int = TYPE.REALTIME
+
+        local_cache: dict[str, dict[str, bool]] = defaultdict(lambda: defaultdict(str))
+
+        @staticmethod
+        def get(section: str, name: str) -> bool | None:
+            if PIH.CACHE.cache_type == PIH.CACHE.TYPE.REALTIME:
+                return (
+                    PIH.CACHE.local_cache[section][name]
+                    if name in PIH.CACHE.local_cache[section]
+                    else None
+                )
+            if PIH.CACHE.cache_type == PIH.CACHE.TYPE.REMOTE:
+                return PIH.DATA.VARIABLE.value(name, section=section)
+
+        @staticmethod
+        def set(section: str, name: str, value: bool) -> None:
+            if PIH.CACHE.cache_type == PIH.CACHE.TYPE.REALTIME:
+                PIH.CACHE.local_cache[section][name] = value
+            if PIH.CACHE.cache_type == PIH.CACHE.TYPE.REMOTE:
+                PIH.DATA.VARIABLE.set(name, value, section=section)
+
     class ERROR:
         notify_about_error: bool = True
 
         @staticmethod
         def rpc(
             context: grpc.RpcContext | None = None,
             message: str = "",
@@ -2643,24 +2888,25 @@
             try:
                 yield True
             except Exception as error:
                 PIH.ERROR.global_except_hook(error)
             finally:
                 if nn(final_action):
                     final_action()
-
-        """
+                    
         @staticmethod
-        def wrap(action: Callable[[Any], Any]) -> Callable[[Any], Any]:
-            def internal_action() -> Any:
-                with PIH.ERROR.detect():
-                    return action
-
-            return internal_action()
-        """
+        @contextmanager
+        def detect_suppressing(final_action: Callable[[], None] | None = None):
+            try:
+                yield True
+            except BaseException:
+                pass
+            finally:
+                if nn(final_action):
+                    final_action()
 
         @staticmethod
         def wrap(action: Callable[[Any], Any]) -> Callable[[Any], Any]:
             def internal_action(*args, **kwargs) -> Any:
                 with PIH.ERROR.detect():
                     return action(*args, **kwargs)
 
@@ -2742,29 +2988,45 @@
         )
 
         class POLIBASE:
 
             @staticmethod
             def create_not_found_error(
                 title: str | None, value: str, start: str = "Пациент"
-            ) -> str:
+            ) -> NotFound:
                 title = title or "поисковым запросом"
-                return NotFound(f'{start} с {title} "{value}" не найден', value)
+                return NotFound(
+                    js((start, "с", title, escs(value), "не найден!")), value
+                )
 
         class USER:
+
             @staticmethod
-            def get_not_found_error(title: str, active: bool, value: str) -> str:
+            def create_not_found_error(
+                title: str, active: bool, value: str
+            ) -> NotFound:
                 start: str | None = None
                 if n(active):
                     start = "Пользователь"
                 elif active:
                     start = "Активный пользователь"
                 else:
                     start = "Неактивный пользователь"
-                return NotFound(f"{start} с {title} '{value}' не найден", value)
+                return NotFound(
+                    js((start, "с", title, escs(value), "не найден!")), value
+                )
+
+        class WORKSTATION:
+
+            @staticmethod
+            def create_not_found_error(title: str, value: str) -> NotFound:
+                start: str = "Компьютер"
+                return NotFound(
+                    js((start, "с", title, escs(value), "не найден!")), value
+                )
 
     class UPDATER:
 
         @staticmethod
         @cache
         def versions(package_name: str) -> list[str]:
             url: str = j(("https://pypi.org/pypi/", package_name, "/json"))
@@ -2852,30 +3114,43 @@
                         if n(version)
                         else (j((package_name_or_path, "==", version)),)
                     )
                 )
             )
 
         @staticmethod
-        def package_exists(package_name: str) -> bool:
-            executor_path: str = PYTHON.EXECUTOR
-            if PIH.SYS.is_virtual_environment():
-                executor_path = sys.executable
-            complete_process: CompletedProcess = PIH.EXECUTOR.execute(
+        def _cache_name(
+            virtual_environment: bool,
+            host: str | None,
+            name: str,
+            version: str | None = None,
+        ) -> str:
+            return j(
                 (
-                    executor_path,
-                    "-m",
-                    PYTHON.PIP,
-                    PYTHON.COMMAND.SHOW,
-                    package_name,
+                    "package",
+                    [None, "venv"][virtual_environment],
+                    host,
+                    name,
+                    version,
                 ),
-                True,
-                True,
+                CONST.SPLITTER,
             )
-            return complete_process.stdout.find(package_name) != -1
+
+        @staticmethod
+        def package_exists(name: str) -> bool:
+            is_virtual_environment: bool = PIH.SYS.is_virtual_environment()
+            cache_name: str = PIH.UPDATER._cache_name(
+                is_virtual_environment, PIH.SYS.host(), name
+            )
+            cache_value: bool | None = PIH.CACHE.get(PIH.UPDATER.__name__, cache_name)
+            if nn(cache_value):
+                return cache_value
+            result: bool = nn(importlib.util.find_spec(name))
+            PIH.CACHE.set(PIH.UPDATER.__name__, cache_name, result)
+            return result
 
         @staticmethod
         def localy(version: str | None = None, show_output: bool = False) -> bool:
             return PIH.UPDATER.package_operation(
                 name=PIH.NAME, version=version, show_output=show_output
             )
 
@@ -2966,24 +3241,18 @@
                 if is_pih_package:
                     return None
                 # Use VSCode for Windows
                 host_is_linux = False
             else:
                 if n(host_is_linux):
                     host_is_linux = PIH.SYS.is_linux(host)
-            cache_name: str = jp(
-                (
-                    "package",
-                    [None, "venv"][virtual_environment],
-                    host,
-                    name,
-                    version,
-                )
+            cache_name: str = PIH.UPDATER._cache_name(
+                virtual_environment, host, name, version
             )
-            if cache_name not in CACHE:
+            if n(PIH.CACHE.get(PIH.UPDATER.__name__, cache_name)):
                 result: bool | None = False
                 host_is_local: bool = e(host) or PIH.SYS.host_is_local(host)
                 command_list: tuple[str, ...] = (
                     PIH.UPDATER.command_for_package_operation(
                         name,
                         version,
                         host_is_local,
@@ -3008,18 +3277,21 @@
                             else PIH.EXECUTOR.create_command_for_psexec(
                                 command_list, host, interactive=True
                             )
                         ),
                         show_output,
                     )
                     result = PIH.DATA.CHECK.returncode(complete_process)
-                CACHE[cache_name] = result
-            return CACHE[cache_name]
+                PIH.CACHE.set(PIH.UPDATER.__name__, cache_name, result)
+            return result
 
     class SETTINGS:
+
+        NAME: str = "settings"
+
         @staticmethod
         def to_datetime(value: SETTINGS) -> datetime:
             return PIH.DATA.CONVERT.settings_to_datetime(value)
 
         @staticmethod
         def to_datetime_list(value: SETTINGS) -> list[datetime]:
             return PIH.DATA.CONVERT.settings_to_datetime_list(value)
@@ -3035,14 +3307,18 @@
         @staticmethod
         def get(settings_item: SETTINGS | StorageVariableHolder | str) -> Any:
             if isinstance(settings_item, str):
                 return PIH.RESULT.SETTINGS.get_by_name(settings_item).data
             return PIH.RESULT.SETTINGS.get(settings_item).data
 
         @staticmethod
+        def all() -> list[strdict]:
+            return PIH.RESULT.SETTINGS.get_by_name(None).data
+
+        @staticmethod
         def init() -> None:
             for setting_item in SETTINGS:
                 if setting_item.value.auto_init:
                     PIH.SETTINGS.set_default(setting_item)
 
         @staticmethod
         def find(value: str | None) -> list[SETTINGS]:
@@ -3067,36 +3343,53 @@
             @staticmethod
             def reboot_time() -> datetime:
                 return PIH.DATA.CONVERT.settings_to_datetime(
                     SETTINGS.WORKSTATION_REBOOT_TIME
                 )
 
         class USER:
+
+            @staticmethod
+            def _get_access_group_name(value: AD.Groups):
+                return j((PIH.CHECK.ACCESS.NAME, value.name), CONST.NAME_SPLITTER)
+
             @staticmethod
             def use_cache() -> bool:
                 return PIH.SETTINGS.get(SETTINGS.USER_USE_CACHE)
 
             @staticmethod
-            def get_section(login: str) -> str:
-                return j((login, "_settings"))
+            def _get_section_name(login_holder: User | str) -> str:
+                return j(
+                    (
+                        (
+                            login_holder.login
+                            if isinstance(login_holder, User)
+                            else login_holder
+                        ),
+                        PIH.SETTINGS.NAME,
+                    ),
+                    CONST.NAME_SPLITTER,
+                )
 
             @staticmethod
-            def set(login: str, name: str, value: Any) -> bool:
+            def set(login_holder: User | str, name: str, value: Any) -> bool:
                 return PIH.ACTION.DATA_STORAGE.value(
-                    value, name, PIH.SETTINGS.USER.get_section(login)
+                    value, name, PIH.SETTINGS.USER._get_section_name(login_holder)
                 )
 
             @staticmethod
             def get(
-                login: str,
+                login_holder: User | str,
                 name: str,
                 class_type_holder: Any | Callable[[Any], Any] | None = None,
             ) -> Any:
                 return PIH.RESULT.DATA_STORAGE.value(
-                    name, class_type_holder, PIH.SETTINGS.USER.get_section(login)
+                    name,
+                    class_type_holder,
+                    PIH.SETTINGS.USER._get_section_name(login_holder),
                 ).data
 
         class INDICATION:
             @staticmethod
             def ct_notification_start_time() -> list[datetime]:
                 return PIH.DATA.CONVERT.settings_to_datetime(
                     SETTINGS.INDICATION_CT_NOTIFICATION_START_TIME
@@ -3157,25 +3450,25 @@
                             if notification_confirmed
                             else SETTINGS.POLIBASE_PERSON_REVIEW_NOTIFICATION_TEXT
                         )
                     ).format(name=FullNameTool.to_given_name(person))
 
             class VISIT:
                 @staticmethod
-                def offer_telegram_bot_url_text(person_full_name: str | None) -> str:
+                def offer_telegram_bot_url_text(person: PolibasePerson | None) -> str:
                     return (
                         PIH.SETTINGS.get(
                             SETTINGS.POLIBASE_PERSON_TAKE_TELEGRAM_BOT_URL_PERSONLESS_TEXT
                         )
-                        if n(person_full_name)
+                        if n(person)
                         else str(
                             PIH.SETTINGS.get(
                                 SETTINGS.POLIBASE_PERSON_TAKE_TELEGRAM_BOT_URL_TEXT
                             )
-                        ).format(name=FullNameTool.to_given_name(person_full_name))
+                        ).format(name=FullNameTool.to_given_name(person))
                     )
 
     class EXECUTOR:
         @staticmethod
         def kill_process_by_port(value: int) -> bool | None:
             pid: str = (
                 str(
@@ -3289,16 +3582,16 @@
                         True,
                     )
                     stderr: str = complete_process.stderr
                     if ne(stderr):
                         if stderr.find(js(("could not start", executor_name))) != -1:
                             continue
                     result = str(complete_process.stdout)
-                    if nn(result):
-                        return parse_version(result)
+            if nn(result):
+                return parse_version(result)
             return None
 
         @staticmethod
         def get_disk_statistics_list(host: str) -> list[DiskStatistics]:
             output: str = PIH.EXECUTOR.execute(
                 js(
                     (
@@ -3729,27 +4022,30 @@
             if nn(parameters):
                 for key, value in parameters.items():
                     result_parameters[key] = value
             if "self" not in result_parameters:
                 result_parameters["self"] = OutputStub()
             if "self" in result_parameters:
                 if use_default_stdout:
-                    OutputStub().set_to(result_parameters["self"])
+                    OutputStub().set_to(globals()["self"])
 
             def action() -> None:
+
                 try:
                     exec(
                         text,
                         globals(),
                         result_parameters,
                     )
                 except Exception as exception:
                     if catch_exceptions:
                         raise exception
 
+                    PIH.ERROR.global_except_hook(exception, PIH.SYS.host())
+
             if stdout_redirect or n(stdout_redirect):
                 stdout = StringIO()
                 with redirect_stdout(stdout):
                     action()
                     if n(stdout_redirect):
                         return globals()
                     return stdout.getvalue()
@@ -3799,15 +4095,15 @@
 
             return PIH.DATA.EXTRACT.returncode(
                 PIH.EXECUTOR.execute(
                     PIH.EXECUTOR.create_command_for_executor(
                         CONST.PSTOOLS.PS_KILL_EXECUTOR,
                         (
                             (
-                                (str(name_or_pid),)
+                                str(name_or_pid)
                                 if local
                                 else (host or PIH.SYS.host(), "-t", str(name_or_pid))
                             ),
                         ),
                         show_output,
                     )
                 )
@@ -3898,15 +4194,15 @@
             if not ignore_send_once and BM.has(
                 EnumTool.get(value).flags, LogMessageFlags.SEND_ONCE
             ):
                 if PIH.CHECK.EVENTS.has_by_key(value, parameters):
                     return False
 
             def internal_send_command(
-                command_name: str, parameters: dict[str, Any], flags: int | None
+                command_name: str, parameters: strdict, flags: int | None
             ) -> Any:
                 try:
                     return DataTool.rpc_decode(
                         PIH.SERVICE.call_command(
                             ServiceCommands.send_event,
                             (command_name, parameters, flags),
                         )
@@ -3966,15 +4262,15 @@
 
         class BUILDER:
             @staticmethod
             def create_parameters_map(
                 event: Events,
                 parameters: tuple[Any, ...] | None = None,
                 check_for_parameters_count: bool = True,
-            ) -> dict:
+            ) -> strdict:
                 event_description: EventDescription = EnumTool.get(event)
                 parameter_pattern_list: list = DataTool.as_list(
                     event_description.params
                 )
                 parameters = parameters or ()
                 if check_for_parameters_count and len(parameter_pattern_list) > len(
                     parameters
@@ -4051,15 +4347,15 @@
                     if actual:
                         try:
                             user: User = PIH.RESULT.USER.by_polibase_pin(
                                 registrator_person.pin
                             ).data
                             workstation: Workstation = (
                                 PIH.RESULT.get_first_item(
-                                    PIH.RESULT.WORKSTATION.by_login(user.samAccountName)
+                                    PIH.RESULT.WORKSTATION.by_login(user.login)
                                 )
                                 or PIH.RESULT.WORKSTATION.by_name(
                                     CONST.TEST.WORKSTATION_MAME
                                 ).data
                             )
                             if nn(workstation):
                                 workstation_name = workstation.name
@@ -4375,19 +4671,15 @@
                 ),
             )
 
         @staticmethod
         def polibase_person_answered(who: PolibasePerson, answer: str) -> None:
             PIH.EVENT.send(
                 Events.POLIBASE_PERSON_ANSWERED,
-                (
-                    who.pin,
-                    who.telephoneNumber,
-                    answer,
-                ),
+                (who.pin, who.telephoneNumber, answer),
             )
 
         @staticmethod
         def resource_accessible(resource: ResourceStatus, at_first_time: bool) -> None:
             PIH.EVENT.send(
                 Events.RESOURCE_ACCESSABLE, (resource.name, resource, at_first_time)
             )
@@ -4570,24 +4862,24 @@
             login: str, password: str, additional_information: str
         ) -> None:
             it_user_list: list[User] = PIH.RESULT.USER.by_job_position(
                 AD.JobPositions.IT
             ).data
             me_user_login: str = PIH.session.get_login()
             it_user_list = DataTool.filter(
-                lambda user: user.samAccountName != me_user_login, it_user_list
+                lambda user: user.login != me_user_login, it_user_list
             )
             it_user: User = it_user_list[0]
             user: User = PIH.RESULT.USER.by_login(login).data
             PIH.EVENT.send(
                 Events.IT_NOTIFY_ABOUT_CREATE_USER,
                 (
                     user.name,
                     user.description,
-                    user.samAccountName,
+                    user.login,
                     password,
                     user.telephoneNumber,
                     user.mail,
                     additional_information,
                 ),
             )
             PIH.EVENT.send(
@@ -4610,15 +4902,15 @@
             telephone_number: str,
         ) -> None:
             it_user_list: list[User] = PIH.RESULT.USER.by_job_position(
                 AD.JobPositions.IT
             ).data
             me_user_login: str = PIH.session.get_login()
             it_user_list = DataTool.filter(
-                lambda user: user.samAccountName != me_user_login, it_user_list
+                lambda user: user.login != me_user_login, it_user_list
             )
             it_user: User = it_user_list[0]
             PIH.EVENT.send(
                 Events.IT_NOTIFY_ABOUT_CREATE_PERSON,
                 (
                     FullNameTool.fullname_to_string(full_name),
                     email_address,
@@ -5156,15 +5448,15 @@
                         or nn(service_description.standalone_name)
                         and service_description.use_standalone
                     )
                     if PIH.SYS.is_virtual_environment():
                         ipih_install = False
                         pih_install = False
                         if as_standalone:
-                            A.O.error(
+                            PIH.output.error(
                                 js(
                                     (
                                         "Sorry, you can not start service",
                                         esc(service_description.name),
                                         "in standalone mode for virtual environment.",
                                         nl(),
                                         "Service will be started in normal mode.",
@@ -5705,15 +5997,15 @@
             file_path: str | None, directory_path: str | None = None
         ) -> str:
             return j(
                 (
                     PIH.PATH.DIRECTORY_INFO_SECTION,
                     (directory_path or PIH.PATH.get_file_directory(file_path)),
                 ),
-                "_",
+                CONST.NAME_SPLITTER,
             )
 
         @staticmethod
         def confirm_file(path: str) -> bool:
             path = PIH.PATH.path(path)
             file_info: tuple[str, float] = (
                 PathTool.get_file_name(path, True),
@@ -5793,22 +6085,49 @@
                     PathTool.replace_prohibited_symbols_from_path_with_symbol(
                         PathTool.add_extension(name, FILE.EXTENSION.PNG)
                     ),
                 )
 
     class DATA(
         DataTool,
-        StringTool,
         ListTool,
-        DateTimeTool,
         EnumTool,
+        StringTool,
+        DateTimeTool,
         FullNameTool,
         ServiceRoleTool,
     ):
 
+        class IOTDevices:
+
+            @staticmethod
+            def status_value(device_id: str, status_value_code: str) -> Any:
+                status: IOTDeviceStatus | None = PIH.RESULT.IOTDevices.status(
+                    device_id
+                ).data
+                if n(status):
+                    return None
+                status_properties: list[IOTDeviceStatusProperty] | None = (
+                    PIH.RESULT.IOTDevices.status_properties(device_id).data
+                )
+                if n(status_properties):
+                    return None
+                for status_item in nnl(nnt(status).values):
+                    if status_item.code == status_value_code:
+                        for status_property_item in status_properties:
+                            if status_property_item.code == status_value_code:
+                                if status_property_item.type == "Integer":
+                                    status_property_item_integer: (
+                                        IOTDeviceStatusIntegerProperty
+                                    ) = status_property_item
+                                    return float(status_item.value) / pow(
+                                        10, status_property_item_integer.scale
+                                    )
+                return None
+
         class EVENT:
 
             @staticmethod
             def remove_save_flag(value: Events) -> int:
                 return BM.remove(EnumTool.get(value).flags, LogMessageFlags.SAVE)
 
         class JOURNAL:
@@ -6526,14 +6845,23 @@
                     date_extract_pattern: str = "[0-9]{1,2}\\.[0-9]{1,2}\\.[0-9]{4}"
                     date_list: list[str] = re.findall(date_extract_pattern, value)
                     if ne(date_list):
                         result = PIH.DATA.EXTRACT.datetime(date_list[0], format)
                 return result
 
             @staticmethod
+            def date(value: str | None, format: str) -> date | None:
+                datetime_value: datetime | None = PIH.DATA.EXTRACT.datetime(
+                    value, format
+                )
+                if nn(datetime_value):
+                    return datetime_value.date()
+                return None
+
+            @staticmethod
             def boolean(value: int | str | None) -> bool | None:
                 if e(value):
                     return False
                 if isinstance(value, str):
                     value = value.lower()
                     if value in ["1", "yes", "да"]:
                         return True
@@ -6952,14 +7280,18 @@
             def returncode(value: CompletedProcess) -> bool:
                 return PIH.DATA.EXTRACT.returncode(value, check_on_success=True)
 
             @staticmethod
             def complete_process_wrong_descriptor(value: CompletedProcess) -> bool:
                 return value.returncode == 2250
 
+            @staticmethod
+            def now(cron_string: str, value: datetime | None = None) -> bool:
+                return PIH.DATA.is_now(cron_string, value)
+
             class VARIABLE:
                 class TIMESTAMP:
                     class EXPIRED:
                         @staticmethod
                         def exists(name: str) -> bool:
                             return ne(PIH.DATA.VARIABLE.TIMESTAMP.EXPIRED.holder(name))
 
@@ -7056,30 +7388,84 @@
 
                 @staticmethod
                 def chiller_value_valid(value: ChillerIndicationsValue) -> bool:
                     return ne(value.temperature)
 
         class FORMAT:
 
+            class IOTDevices:
+
+                @staticmethod
+                def status_value(device_id: str, code: str) -> str | None:
+                    value: Any = PIH.DATA.IOTDevices.status_value(device_id, code)
+                    if n(value):
+                        return None
+                    status_properties: list[IOTDeviceStatusProperty] | None = (
+                        PIH.RESULT.IOTDevices.status_properties(device_id).data
+                    )
+                    if n(status_properties):
+                        return None
+                    for status_property_item in status_properties:
+                        if status_property_item.code == code:
+                            return js((value, status_property_item.unit))
+                    return None
+
+            @staticmethod
+            def console_message(text: str) -> str:
+                return (
+                    text.replace(BOLD_BEGIN, Style.BRIGHT)
+                    .replace(BOLD_END, Style.RESET_ALL)
+                    .replace(ITALICS_BEGIN, "")
+                    .replace(ITALICS_END, "")
+                )
+
+            @staticmethod
+            def as_plain_message(text: str) -> str:
+                return (
+                    text.replace(BOLD_BEGIN, "")
+                    .replace(BOLD_END, "")
+                    .replace(ITALICS_BEGIN, "")
+                    .replace(ITALICS_END, "")
+                )
+
+            @staticmethod
+            def whatsapp_message(value: str | None) -> str | None:
+                if n(value):
+                    return value
+                b: str = MESSAGE.WHATSAPP.STYLE.BOLD
+                i: str = MESSAGE.WHATSAPP.STYLE.ITALIC
+                return (
+                    value.replace(BOLD_BEGIN, b)
+                    .replace(BOLD_END, b)
+                    .replace(ITALICS_BEGIN, i)
+                    .replace(ITALICS_END, i)
+                )
+
+            @staticmethod
+            def bold(value: str) -> str:
+                return b(value)
+
+            @staticmethod
+            def italics(value: Any) -> str:
+                return StringTool.italics(value)
+
             @staticmethod
             def wappi_status(
                 value: WappiStatus | CONST.MESSAGE.WHATSAPP.WAPPI.Profiles,
-                output_stub: OutputStub | None = None,
             ) -> str:
-                output_stub = output_stub or PIH.output
                 profile: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | None = None
                 if isinstance(value, CONST.MESSAGE.WHATSAPP.WAPPI.Profiles):
                     profile = value
                     value = PIH.MESSAGE.WHATSAPP.WAPPI.get_status(value)
                 title: str = j(
                     (
                         "Статус ",
                         CONST.MESSAGE.WHATSAPP.WAPPI.NAME,
                         ": ",
-                        output_stub.b(value.name or ("" if n(profile) else profile.name)),  # type: ignore
+                        b(value.name or ("" if n(profile) else profile.name)),  # type: ignore
                         nl(),
                     )
                 )
                 if value.authorized:
                     payment_expired_at: datetime = DateTimeTool.datetime_from_string(
                         value.payment_expired_at, CONST.MESSAGE.WHATSAPP.WAPPI.DATETIME_FORMAT  # type: ignore
                     )  # type: ignore
@@ -7185,15 +7571,15 @@
                     if from_environment
                     else PIH.DATA.VARIABLE.value(variable_name)
                 )
 
             @staticmethod
             def variable_name(value: str) -> str:
                 value = value.lower()
-                return re.sub("[\\\\.\\-@:]", "_", value)
+                return re.sub("[\\\\.\\-@:]", CONST.NAME_SPLITTER, value)
 
             @staticmethod
             def statistics(value: MATERIALIZED_RESOURCES.Types) -> str | None:
                 statistics: TimeSeriesStatistics | None = PIH.DATA.STATISTICS.by_name(
                     value.name
                 )
                 if n(statistics):
@@ -7210,21 +7596,17 @@
                         f" {CONST.VISUAL.BULLET} Минимально: {count * to_days(statistics.min)}",
                         f" {CONST.VISUAL.BULLET} В среднем: {count * to_days(statistics.avg)}",
                     ),
                     nl(),
                 )
 
             @staticmethod
-            def yes_no(value: bool, symbolic: bool = False) -> str:
+            def yes_no(value: bool | None, symbolic: bool = False) -> str:
                 c: Callable[
-                    [
-                        bool,
-                        Callable[[], Any] | Any,
-                        Callable[[], Any] | Any,
-                    ],
+                    [bool, Callable[[], Any] | Any, Callable[[], Any] | Any, None],
                     Any,
                 ] = DataTool.check
                 return c(
                     value,
                     c(symbolic, CONST.VISUAL.YES, "Да"),
                     c(symbolic, CONST.VISUAL.NO, "Нет"),
                 )
@@ -7293,15 +7675,15 @@
 
             @staticmethod
             def index(value: int) -> str:
                 return str(value + 1) if value > 0 else ""
 
             @staticmethod
             def user_principal_name(login: str) -> str:
-                return j((login, AD.DOMAIN_MAIN), A.CT.EMAIL_SPLITTER)
+                return j((login, AD.DOMAIN_MAIN), CONST.EMAIL_SPLITTER)
 
             @staticmethod
             def as_string(
                 value: Any,
                 escaped_string: bool = False,
                 mapper: Callable[[Any], str] | None = None,
             ) -> str | None:
@@ -7358,15 +7740,15 @@
                 )
 
             @staticmethod
             def by_formatter_name(value: Enum | str, data: Any) -> str | None:
                 if isinstance(value, str):
                     value = EnumTool.get_by_value(DATA.FORMATTER, value) or value
                 if isinstance(value, str):
-                    name: str = j((PIH.DATA.STATISTICS.NAME, "_"))
+                    name: str = j((PIH.DATA.STATISTICS.NAME, CONST.NAME_SPLITTER))
                     index: int = value.lower().find(name)
                     if index != -1:
                         index += len(name)
                         value: MATERIALIZED_RESOURCES.Types | None = (
                             EnumTool.get_by_value_or_key(
                                 MATERIALIZED_RESOURCES.Types, value[index:].upper()
                             )
@@ -7511,29 +7893,29 @@
 
             @staticmethod
             def email(
                 value: str,
                 use_default_domain: bool = False,
                 email_correction: bool = False,
             ) -> str:
-                if use_default_domain and value.find(A.CT.EMAIL_SPLITTER) == -1:
+                if use_default_domain and value.find(CONST.EMAIL_SPLITTER) == -1:
                     value = PIH.DATA.FORMAT.email(
-                        j((value, ADDRESSES.SITE_ADDRESS), A.CT.EMAIL_SPLITTER)
+                        j((value, ADDRESSES.SITE_ADDRESS), CONST.EMAIL_SPLITTER)
                     )
                 if email_correction:
                     for char in '"(),:;<>[\\] ':
                         value = value.replace(char, "")
                     value = value.replace("/", ".")
-                    email_name, email_domain = value.split(A.CT.EMAIL_SPLITTER)
+                    email_name, email_domain = value.split(CONST.EMAIL_SPLITTER)
                     PIH.RESULT.FILES.execute("@email_correction")
                     for email_correction_item in EMAIL_CORRECTION:
                         if email_domain in email_correction_item[0]:
                             email_domain = email_correction_item[1]
                             break
-                    value = j((email_name, email_domain), A.CT.EMAIL_SPLITTER)
+                    value = j((email_name, email_domain), CONST.EMAIL_SPLITTER)
                 return value.lower()
 
             @staticmethod
             def name(
                 value: str,
                 remove_non_alpha: bool = False,
                 name_part_minimal_length: int | None = None,
@@ -7690,15 +8072,15 @@
                 result = PIH.DATA.FORMAT.telephone_number(result) if format else result
                 PIH.DATA.TELEPHONE_NUMBER.cache[value] = result
                 return result
 
             @staticmethod
             def by_workstation_name(value: str) -> str:
                 workstation: Workstation = PIH.RESULT.WORKSTATION.by_name(value).data
-                return PIH.DATA.TELEPHONE_NUMBER.by_login(workstation.samAccountName)
+                return PIH.DATA.TELEPHONE_NUMBER.by_login(workstation.login)
 
             @staticmethod
             def by_mark_tab_number(value: str, format: bool = True) -> str:
                 result: str = PIH.DATA.MARK.by_tab_number(value).telephoneNumber
                 return PIH.DATA.FORMAT.telephone_number(result) if format else result
 
             @staticmethod
@@ -7954,25 +8336,68 @@
         class IOTDevices:
 
             @staticmethod
             def _call(
                 command: IOT.Commands, parameters: tuple[Any, ...] | None = None
             ) -> bool:
                 return PIH.SERVICE.call_command_for_service(
-                    ServiceRoles.IOT,
+                    ServiceRoles.IOTDevices,
                     ServiceCommands.serve_command,
                     (command.name, *(parameters or ())),
                 )
 
             @staticmethod
+            def status(id: str) -> Result[IOTDeviceStatus]:
+                def mapper(value: strdict) -> IOTDeviceStatus:
+                    values: list[IOTDeviceStatusValue] = []
+                    for status_item in value["result"]:
+                        values.append(
+                            DataTool.fill_data_from_source(
+                                IOTDeviceStatusValue(), status_item
+                            )
+                        )
+                    return IOTDeviceStatus(value["t"] / 1000, tuple(values))
+
+                return DataTool.to_result(
+                    PIH.RESULT.IOTDevices._call(IOT.Commands.device_status, (id,)),
+                    mapper,
+                )
+
+            @staticmethod
             def devices() -> Result[list[IOTDevice]]:
                 return DataTool.to_result(
                     PIH.RESULT.IOTDevices._call(IOT.Commands.device_list), IOTDevice
                 )
 
+            @staticmethod
+            def status_properties(id: str) -> Result[list[IOTDeviceStatusProperty]]:
+                def mapper(value: strdict) -> list[IOTDeviceStatusProperty]:
+                    values: list[IOTDeviceStatusProperty] = []
+                    for status_item in value["result"]["status"]:
+                        if lw(status_item["type"]) == "integer":
+                            values.append(
+                                DataTool.fill_data_from_source(
+                                    IOTDeviceStatusIntegerProperty(
+                                        status_item["code"],
+                                        status_item["name"],
+                                        status_item["type"],
+                                    ),
+                                    DataTool.rpc_decode(status_item["values"]),
+                                    skip_not_none=True,
+                                )
+                            )
+                    return values
+
+                return DataTool.to_result(
+                    PIH.RESULT.IOTDevices._call(
+                        IOT.Commands.device_status_properties, (id,)
+                    ),
+                    mapper,
+                )
+
         class ZABBIX:
 
             @staticmethod
             def _call(
                 command: ZABBIX.Commands, parameters: tuple[Any, ...] | None = None
             ) -> str | None:
                 return PIH.SERVICE.call_command_for_service(
@@ -8129,15 +8554,22 @@
                     count_as_result,
                 )
 
             @staticmethod
             def get(
                 event_type: Events | None = None,
                 parameters: tuple[Any, ...] | None = None,
-                timestamp: datetime | date | str | int | None = None,
+                timestamp: (
+                    datetime
+                    | date
+                    | str
+                    | int
+                    | tuple[date | datetime, date | datetime]
+                    | None
+                ) = None,
                 count_as_result: bool = False,
             ) -> Result[list[EventDS] | int]:
                 def extract_function(data: Any, count_as_result: bool) -> EventDS | int:
                     if count_as_result:
                         return data
                     result: EventDS = DataTool.fill_data_from_source(EventDS(), data)
                     # from json string to python object
@@ -8399,15 +8831,19 @@
             def find(
                 value: str | None = None,
                 command_type: CommandTypes | None = None,
                 exclude_private_files: bool = False,
             ) -> Result[list[File]]:
                 value = lw(value)
                 search_function: Callable[[File], bool] = (
-                    lambda item: lw(item.title).find(value) != -1
+                    lambda item: StringTool.full_right_intersection_by_tokens(
+                        nns(item.title),
+                        nns(value),
+                        (" ", CONST.NAME_SPLITTER, CONST.SPLITTER, ","),
+                    )
                 )
                 was_updated: bool = False
                 section: str = CONST.FILES.SECTION
                 if section not in PIH.RESULT.NOTES._local_database_cache or e(
                     PIH.RESULT.NOTES._local_database_cache[section]
                 ):
                     PIH.ACTION.FILES.cache_local_database()
@@ -8876,16 +9312,20 @@
                 return DataTool.to_result(
                     PIH.SERVICE.call_command(
                         ServiceCommands.get_settings_value, (key, default_value)
                     )
                 )
 
             @staticmethod
-            def get(settings_item: SETTINGS | StorageVariableHolder) -> Result[Any]:
+            def get(
+                settings_item: SETTINGS | StorageVariableHolder | None,
+            ) -> Result[Any] | Result[list[strdict]]:
                 settings_item = EnumTool.get(settings_item)
+                if n(settings_item):
+                    PIH.RESULT.SETTINGS.get_by_name(None)
                 return PIH.RESULT.SETTINGS.get_by_name(
                     settings_item.key_name or settings_item.name,
                     settings_item.default_value,
                 )
 
             @staticmethod
             def get_by_name(value: str, default_value: Any = None) -> Result[Any]:
@@ -8954,15 +9394,15 @@
                 result: Result[Workstation] = ResultTool.with_first_item(
                     ResultTool.filter(
                         lambda item: item.name.lower() == value,
                         PIH.RESULT.COMPUTER.by_container_dn(container_dn, class_type),
                     )
                 )
                 if e(result):
-                    raise NotFound(f"Компьютер с именем {value} не найден")
+                    raise PIH.ERROR.WORKSTATION.create_not_found_error("именем", value)
                 return result
 
         class WORKSTATION:
             CONTAINER_DN: str = AD.WORKSTATIONS_CONTAINER_DN
 
             @staticmethod
             def all_description() -> Result[list[ComputerDescription]]:
@@ -9018,15 +9458,15 @@
                             )
                             if internal_telephone_number == value:
                                 result_worksation = workstation
                                 break
                 if result_worksation is not None:
                     return Result(result.fields, workstation)
                 else:
-                    raise PIH.ERROR.USER.get_not_found_error(
+                    raise PIH.ERROR.USER.create_not_found_error(
                         "внутренним номером телефона", True, str(value)
                     )
 
             @staticmethod
             def by_any(value: int | str | User | None) -> Result[list[Workstation]]:
                 if n(value):
                     return PIH.RESULT.WORKSTATION.all()
@@ -9037,35 +9477,51 @@
                             return ResultTool.as_list(
                                 PIH.RESULT.WORKSTATION.by_internal_telephone_number(
                                     int(value)
                                 )
                             )
                         except NotFound as _:
                             return PIH.RESULT.WORKSTATION.by_login(
-                                PIH.RESULT.USER.by_tab_number(value).data.samAccountName
+                                PIH.RESULT.USER.by_tab_number(value).data.login
                             )
                     if PIH.CHECK.WORKSTATION.name(value):
                         return ResultTool.as_list(PIH.RESULT.WORKSTATION.by_name(value))
                 try:
                     if value_is_user:
-                        value = value.samAccountName
+                        value = value.login
                     return PIH.RESULT.WORKSTATION.by_login(value)
                 except NotFound as _:
-                    raise NotFound(f"Компьютер с параметром поиска {value} не найден")
+                    try:
+                        return PIH.RESULT.WORKSTATION.by_user_name(value)
+                    except NotFound as _:
+                        raise PIH.ERROR.WORKSTATION.create_not_found_error(
+                            "параметром поиска", value
+                        )
+
+            @staticmethod
+            def by_user_name(value: str) -> Result[list[Workstation]]:
+                class DH:
+                    result: Result[list[Workstation]] = Result()
+
+                def action(user: User, fields: FieldItemList) -> None:
+                    if n(DH.result.fields):
+                        DH.result.fields = fields
+                    DH.result += PIH.RESULT.WORKSTATION.by_login(user.login)
+
+                ResultTool.every_with_fields(action, PIH.RESULT.USER.by_name(value))
+                return DH.result
 
             @staticmethod
             def by_name(value: str) -> Result[Workstation]:
                 try:
                     return PIH.RESULT.COMPUTER.by_name(
                         value, PIH.RESULT.WORKSTATION.CONTAINER_DN, Workstation
                     )
                 except NotFound as _:
-                    raise NotFound(
-                        js(("Рабочая станция с именем", escs(value), "не найден"))
-                    )
+                    raise PIH.ERROR.WORKSTATION.create_not_found_error("именем", value)
 
             @staticmethod
             def all() -> Result[list[Workstation]]:
                 return PIH.RESULT.COMPUTER.by_container_dn(
                     PIH.RESULT.WORKSTATION.CONTAINER_DN, Workstation
                 )
 
@@ -9296,23 +9752,25 @@
                 return DataTool.to_result(
                     PIH.SERVICE.call_command(ServiceCommands.printers_report),
                     PrinterReport,
                 )
 
         class MARK:
             @staticmethod
-            def by_tab_number(value: str) -> Result[Mark]:
+            def by_tab_number(value: str | int) -> Result[Mark]:
                 result: Result[Mark] = DataTool.to_result(
                     PIH.SERVICE.call_command(
-                        ServiceCommands.get_mark_by_tab_number, value
+                        ServiceCommands.get_mark_by_tab_number, str(value)
                     ),
                     Mark,
                 )
                 if e(result):
-                    raise NotFound(f"Карта доступа с номером '{value}' не найдена")
+                    raise NotFound(
+                        js(("Карта доступа с номером", escs(value), "не найдена"))
+                    )
                 return result
 
             @staticmethod
             def by_division(division_or_id: PersonDivision | int) -> Result[list[Mark]]:
                 division_id: int = DataTool.check(
                     isinstance(division_or_id, PersonDivision),
                     lambda: division_or_id.id,
@@ -9892,28 +10350,30 @@
                 value: str, active: bool | None = None, cached: bool | None = None
             ) -> Result[User]:
                 try:
                     return ResultTool.with_first_item(
                         PIH.RESULT.USER.by_login_pattern(value, active, cached)
                     )
                 except NotFound as _:
-                    raise PIH.ERROR.USER.get_not_found_error("логином", active, value)
+                    raise PIH.ERROR.USER.create_not_found_error(
+                        "логином", active, value
+                    )
 
             @staticmethod
             def by_login_pattern(
                 value: str, active: bool | None = None, cached: bool | None = None
             ) -> Result[list[User]]:
                 result: Result[list[User]] = DataTool.to_result(
                     PIH.SERVICE.call_command(
                         ServiceCommands.get_user_by_login, (value, active, cached)
                     ),
                     User,
                 )
                 if e(result):
-                    raise PIH.ERROR.USER.get_not_found_error(
+                    raise PIH.ERROR.USER.create_not_found_error(
                         "шаблоном логина", active, value
                     )
                 return result
 
             @staticmethod
             def by_telephone_number(
                 value: str, active: bool | None = None
@@ -9922,15 +10382,15 @@
                     PIH.SERVICE.call_command(
                         ServiceCommands.get_user_by_telephone_number, (value, active)
                     ),
                     User,
                     True,
                 )
                 if e(result):
-                    raise PIH.ERROR.USER.get_not_found_error(
+                    raise PIH.ERROR.USER.create_not_found_error(
                         "номером телефона", active, value
                     )
                 return result
 
             @staticmethod
             def by_internal_telephone_number(value: int) -> Result[User]:
                 workstation_list: list[Workstation] = PIH.RESULT.WORKSTATION.all().data
@@ -9949,19 +10409,19 @@
                             )
                             if internal_telephone_number == value:
                                 result_worksation = workstation
                                 break
                 if (
                     result_worksation is not None
                     and result_worksation.accessable
-                    and ne(result_worksation.samAccountName)
+                    and ne(result_worksation.login)
                 ):
-                    return PIH.RESULT.USER.by_login(workstation.samAccountName)
+                    return PIH.RESULT.USER.by_login(workstation.login)
                 else:
-                    raise PIH.ERROR.USER.get_not_found_error(
+                    raise PIH.ERROR.USER.create_not_found_error(
                         "внутренним номером телефона", True, str(value)
                     )
 
             @staticmethod
             def by_polibase_pin(value: int) -> Result[User]:
                 return ResultTool.with_first_item(
                     PIH.RESULT.USER.by_name(
@@ -9976,34 +10436,34 @@
                     PIH.SERVICE.call_command(
                         ServiceCommands.get_user_by_workstation, value
                     ),
                     Workstation,
                     True,
                 ).data
                 if e(user_workstation):
-                    details: str = f"Компьютер с именем '{value}' не найден!"
-                    raise NotFound(details)
-                if e(user_workstation.samAccountName):
+                    raise PIH.ERROR.WORKSTATION.create_not_found_error("именем", value)
+                if e(user_workstation.login):
                     raise NotFound(
-                        f"За компьютером {value} нет залогиненного пользователя", value
+                        js(("За компьютером", value, "нет залогиненного пользователя")),
+                        value,
                     )
-                return PIH.RESULT.USER.by_login(user_workstation.samAccountName)
+                return PIH.RESULT.USER.by_login(user_workstation.login)
 
             @staticmethod
             def by_any(value: Any, active: bool | None = None) -> Result[list[User]]:
                 def by_number(value: int) -> Result[list[User]]:
                     try:
                         return ResultTool.as_list(PIH.RESULT.USER.by_tab_number(value))
                     except NotFound as _:
                         try:
                             return ResultTool.as_list(
                                 PIH.RESULT.USER.by_login(
                                     PIH.RESULT.WORKSTATION.by_internal_telephone_number(
                                         value
-                                    ).data.samAccountName
+                                    ).data.login
                                 )
                             )
                         except:
                             return ResultTool.as_list(
                                 PIH.RESULT.USER.by_polibase_pin(value)
                             )
 
@@ -10061,15 +10521,15 @@
                         )
                     init_or_add(lambda: PIH.RESULT.USER.by_login_pattern(value, active))
                     init_or_add(lambda: PIH.RESULT.USER.by_name(value, active))
                     if ne(DH.result):
                         return DH.result
                 elif isinstance(value, int):
                     return by_number(value)
-                raise PIH.ERROR.USER.get_not_found_error(
+                raise PIH.ERROR.USER.create_not_found_error(
                     "поисковым значением", active, value
                 )
 
             @staticmethod
             def by_job_position(value: AD.JobPositions) -> Result[list[User]]:
                 UCH = PIH.CHECK.USER
                 return ResultTool.filter(
@@ -10117,48 +10577,51 @@
                     ),
                     User,
                     get_first,
                 )
 
             @staticmethod
             def by_name(
-                value: str, active: bool | None = None, cached: bool | None = None
+                value: str,
+                active: bool | None = None,
+                cached: bool | None = None,
+                strict_comparison: bool = False,
             ) -> Result[list[User]]:
                 result: Result[list[User]] = DataTool.to_result(
                     PIH.SERVICE.call_command(
-                        ServiceCommands.get_users_by_name, (value, active, cached)
+                        ServiceCommands.get_users_by_name,
+                        (value, active, cached, strict_comparison),
                     ),
                     User,
                 )
                 if e(result):
-                    raise PIH.ERROR.USER.get_not_found_error("именем", active, value)
+                    raise PIH.ERROR.USER.create_not_found_error("именем", active, value)
                 return result
 
             @staticmethod
             def all(active: bool | None = None) -> Result[list[User]]:
-                return PIH.RESULT.USER.by_name(AD.SEARCH_ALL_PATTERN, active)
+                return PIH.RESULT.USER.by_name(None, active)
 
             @staticmethod
             def list_with_telephone_number(
                 active: bool | None = None,
             ) -> Result[list[User]]:
                 def user_with_telephone_number(user: User) -> bool:
                     return PIH.CHECK.telephone_number(user.telephoneNumber)
 
                 return ResultTool.filter(
                     lambda user: user_with_telephone_number(user),
                     PIH.RESULT.USER.all(active),
                 )
 
             @staticmethod
-            def by_tab_number(value: str) -> Result[User]:
+            def by_tab_number(value: str | int) -> Result[User]:
                 result: Result[Mark] = PIH.RESULT.MARK.by_tab_number(value)
                 if e(result):
-                    details: str = f"Карта доступа с номером {value} не найдена"
-                    raise NotFound(details)
+                    raise NotFound(js(("Карта доступа с номером", value, "не найдена")))
                 return PIH.RESULT.USER.by_mark(result.data)
 
             @staticmethod
             def by_mark(value: Mark) -> Result[User]:
                 return Result(
                     FIELD_COLLECTION.AD.USER,
                     DataTool.check(
@@ -10418,15 +10881,15 @@
                 value: str,
                 cached: bool = True,
                 verification_method: EmailVerificationMethods | None = None,
             ) -> bool:
                 def internal_accessability(
                     value: str, verification_method: EmailVerificationMethods
                 ) -> bool:
-                    domain: str = value.split(A.CT.EMAIL_SPLITTER)[1]
+                    domain: str = value.split(CONST.EMAIL_SPLITTER)[1]
                     if domain == "icloud.com":
                         verification_method = EmailVerificationMethods.NORMAL
                     return DataTool.rpc_decode(
                         PIH.SERVICE.call_command(
                             ServiceCommands.check_email_accessibility,
                             (value, verification_method, cached),
                         )
@@ -10435,147 +10898,211 @@
                 # if not internal_accessability(value, verification_method):
                 verification_method = (
                     verification_method or EmailVerificationMethods.DEFAULT
                 )
                 return internal_accessability(value, verification_method)
                 # return True
 
-        class FILE:
+        class FILES:
+
             @staticmethod
             def excel_file(path: str) -> bool:
                 return os.path.isfile(path) and PathTool.get_extension(path) in [
                     FILE.EXTENSION.EXCEL_OLD,
                     FILE.EXTENSION.EXCEL_NEW,
                 ]
 
+            @staticmethod
+            def exists(name: str) -> bool:
+                return ne(PIH.RESULT.FILES.find(name))
+
         class ACCESS:
+
+            NAME: str = "access"
+
+            @staticmethod
+            def _get_cache_for_group(
+                value: AD.Groups,
+                session: SessionBase | None = None,
+            ) -> bool | None:
+                user: User = (session or PIH.session).get_user()
+                return PIH.SETTINGS.USER.get(
+                    user, PIH.SETTINGS.USER._get_access_group_name(value)
+                )
+
             @staticmethod
-            def by_group(
+            def _set_cache_for_group(
                 group: AD.Groups,
+                session: SessionBase,
+                value: bool,
+            ) -> None:
+                PIH.SETTINGS.USER.set(
+                    session.get_user(),
+                    PIH.SETTINGS.USER._get_access_group_name(group),
+                    value,
+                )
+
+            @staticmethod
+            def action_for_all_groups(
+                session: SessionBase | None = None,
+                exit_on_access_denied: bool = False,
+                notify_on_fail: bool = True,
+                notify_on_success: bool = True,
+                cached: bool = True,
+            ) -> None:
+                for group in AD.Groups:
+                    PIH.CHECK.ACCESS.action_for_group(
+                        group,
+                        session,
+                        exit_on_access_denied,
+                        notify_on_fail,
+                        notify_on_success,
+                        cached,
+                    )
+
+            @staticmethod
+            def action_for_group(
+                value: AD.Groups,
+                session: SessionBase | None = None,
                 exit_on_access_denied: bool = False,
-                session: SessionBase = None,
                 notify_on_fail: bool = True,
                 notify_on_success: bool = True,
+                cached: bool = True,
             ) -> bool:
                 session = session or PIH.session
                 user: User = session.get_user()
                 result: bool = False
                 notify: bool = notify_on_success or notify_on_fail
-                if group in session.allowed_groups:
+                if value in session.allowed_groups:
                     result = True
                     notify = False
                 else:
-                    result = PIH.CHECK.USER.by_group(user, group)
+                    result = (
+                        PIH.CHECK.ACCESS._get_cache_for_group(value, session)
+                        if cached
+                        else PIH.CHECK.USER.by_group(user, value)
+                    )
+                    if n(result):
+                        result = PIH.CHECK.USER.by_group(user, value)
                     if result:
-                        session.add_allowed_group(group)
+                        session.add_allowed_group(value)
                 if notify:
                     PIH.LOG.it_bot(
-                        f"Запрос на доступа к группе: {group.name} от пользователя {user.name} ({user.samAccountName}). Доступ {'разрешен' if result else 'отклонен'}.",
+                        js(
+                            (
+                                "Запрос на доступа к группе: ",
+                                value.name,
+                                " от пользователя ",
+                                user.name,
+                                j(("(", user.login, ").")),
+                                "Доступ ",
+                                ["отклонен", "разрешен"][result],
+                            )
+                        ),
                         LogMessageFlags.NORMAL if result else LogMessageFlags.ERROR,
                     )
                 if not result and exit_on_access_denied:
                     session.exit(5, "Функционал недоступен...")
+                PIH.CHECK.ACCESS._set_cache_for_group(value, session, result)
                 return result
 
             @staticmethod
             def admin(
                 exit_on_access_denied: bool = False,
                 session: SessionBase = None,
                 notify_on_fail: bool = True,
                 notify_on_success: bool = True,
             ) -> bool:
-                return PIH.CHECK.ACCESS.by_group(
+                return PIH.CHECK.ACCESS.action_for_group(
                     AD.Groups.Admin,
-                    exit_on_access_denied,
                     session,
+                    exit_on_access_denied,
                     notify_on_fail,
                     notify_on_success,
                 )
 
             @staticmethod
             def service_admin(
                 session: SessionBase = None,
                 notify_on_fail: bool = True,
                 notify_on_success: bool = True,
             ) -> bool:
-                return PIH.CHECK.ACCESS.by_group(
+                return PIH.CHECK.ACCESS.action_for_group(
                     AD.Groups.ServiceAdmin,
-                    False,
                     session,
+                    False,
                     notify_on_fail,
                     notify_on_success,
                 )
 
             @staticmethod
             def inventory(
                 session: SessionBase = None,
                 notify_on_fail: bool = True,
                 notify_on_success: bool = True,
             ) -> bool:
-                return PIH.CHECK.ACCESS.by_group(
+                return PIH.CHECK.ACCESS.action_for_group(
                     AD.Groups.Inventory,
-                    False,
                     session,
+                    False,
                     notify_on_fail,
                     notify_on_success,
                 )
 
             @staticmethod
             def polibase(
                 session: SessionBase = None,
                 notify_on_fail: bool = True,
                 notify_on_success: bool = True,
             ) -> bool:
-                return PIH.CHECK.ACCESS.by_group(
+                return PIH.CHECK.ACCESS.action_for_group(
                     AD.Groups.Polibase,
-                    False,
                     session,
+                    False,
                     notify_on_fail,
                     notify_on_success,
                 )
 
             @staticmethod
             def card_registry(
                 session: SessionBase = None,
                 notify_on_fail: bool = True,
                 notify_on_success: bool = True,
             ) -> bool:
-                return PIH.CHECK.ACCESS.by_group(
+                return PIH.CHECK.ACCESS.action_for_group(
                     AD.Groups.CardRegistry,
-                    False,
                     session,
+                    False,
                     notify_on_fail,
                     notify_on_success,
                 )
 
         class USER:
             @staticmethod
             def doctor(user: User) -> bool:
-                distinguishedName: str = user.distinguishedName
-                return not (
-                    distinguishedName.find("Доктор") == -1
-                    and distinguishedName.find("Оператор") == -1
+                distinguishedName: str = lw(user.distinguishedName)
+                return (
+                    distinguishedName.find("доктор") != -1
+                    or distinguishedName.find("оператор") != -1
                 )
 
             @staticmethod
             def by_group(user: User, value: AD.Groups) -> bool:
                 return ne(
                     ResultTool.filter(
-                        lambda check_user: check_user.samAccountName
-                        == user.samAccountName,
+                        lambda check_user: check_user.login == user.login,
                         PIH.RESULT.USER.by_group(value),
                     )
                 )
 
             @staticmethod
-            def has_property(user: User, value: AD.UserProperies) -> bool:
+            def property(user: User, value: AD.UserProperies) -> bool:
                 return ne(
                     ResultTool.filter(
-                        lambda check_user: check_user.samAccountName
-                        == user.samAccountName,
+                        lambda check_user: check_user.login == user.login,
                         PIH.RESULT.USER.by_property(value),
                     )
                 )
 
             @staticmethod
             def exists_by_login(value: str) -> bool:
                 return DataTool.rpc_decode(
@@ -10590,32 +11117,28 @@
 
             @staticmethod
             def active(value: User) -> bool:
                 return value.distinguishedName.find(AD.ACTIVE_USERS_CONTAINER_DN) != -1
 
             @staticmethod
             def template(value: User) -> bool:
-                name: str = value.samAccountName
-                return name[0] == "_" and name[-1] == "_"
+                login: str = value.login
+                return (
+                    login[0] == CONST.NAME_SPLITTER and login[-1] == CONST.NAME_SPLITTER
+                )
 
             @staticmethod
             def exists_by_full_name(value: FullName) -> bool:
                 return ne(PIH.RESULT.USER.by_full_name(value))
 
             @staticmethod
             def search_attribute(value: str) -> bool:
                 return value in AD.SEARCH_ATTRIBUTES
 
             @staticmethod
-            def property(
-                value: str | None, default_value: str = USER_PROPERTIES.PASSWORD
-            ) -> str:
-                return value or default_value
-
-            @staticmethod
             def accessibility() -> bool:
                 return PIH.SERVICE.check_on_accessibility(ServiceRoles.AD)
 
         class MESSAGE:
             class WHATSAPP:
                 class WAPPI:
                     @staticmethod
@@ -10633,22 +11156,16 @@
                         cached: bool = True,
                     ) -> bool:
                         def internal_accessibility(
                             profile: (
                                 CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None
                             ) = None,
                         ) -> bool:
-                            profile = EnumTool.get_by_value(
-                                CONST.MESSAGE.WHATSAPP.WAPPI.Profiles,
-                                profile
-                                or CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT,
-                            )
-                            profile_value: str = EnumTool.get_value(
-                                profile,
-                                EnumTool.get(profile),
+                            profile, profile_value = (
+                                PIH.MESSAGE.WHATSAPP.WAPPI._get_profile_value(profile)
                             )
                             url: str = j(
                                 (
                                     CONST.MESSAGE.WHATSAPP.WAPPI.URL_GET_STATUS,
                                     profile_value,
                                 )
                             )
@@ -10695,20 +11212,22 @@
 
             @staticmethod
             def accessibility() -> bool:
                 return PIH.SERVICE.check_on_accessibility(ServiceRoles.MARK)
 
             @staticmethod
             def tab_number(value: str) -> bool:
+                if value.endswith(MARK_VARIANT.BRACELET):
+                    value = value.split(MARK_VARIANT.BRACELET)[0]
                 return value.isdecimal()
 
         class TIME_TRACKING:
             @staticmethod
             def accessibility() -> bool:
-                return PIH.CHECK.ACCESS.by_group(AD.Groups.TimeTrackingReport)
+                return PIH.CHECK.ACCESS.action_for_group(AD.Groups.TimeTrackingReport)
 
         class INVENTORY:
             @staticmethod
             def is_report_file(file_path: str) -> bool:
                 return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.check_inventory_report, file_path
@@ -10782,14 +11301,16 @@
                             )
                         )
                         return ne(result) and (
                             True if state is None else result.data.status == state
                         )
 
             class DATABASE:
+
+                @staticmethod
                 def creation_start_time(value: datetime) -> bool:
                     return DateTimeTool.is_equal_by_time(
                         value,
                         PIH.SETTINGS.to_datetime(
                             SETTINGS.POLIBASE_CREATION_DB_DUMP_START_TIME
                         ),
                     )
@@ -10845,34 +11366,34 @@
                     ResultTool.filter(
                         lambda workstation: name == workstation.name.lower(),
                         PIH.RESULT.WORKSTATION.all_description(),
                     )
                 )
 
             @staticmethod
-            def has_property(
+            def property(
                 workstation: ComputerDescription, property: AD.ComputerProperties
             ) -> bool:
                 return BM.has(workstation.properties, property)
 
             @staticmethod
             def watchable(workstation: ComputerDescription) -> bool:
-                return PIH.CHECK.WORKSTATION.has_property(
+                return PIH.CHECK.WORKSTATION.property(
                     workstation, AD.ComputerProperties.Watchable
                 )
 
             @staticmethod
             def shutdownable(workstation: ComputerDescription) -> bool:
-                return PIH.CHECK.WORKSTATION.has_property(
+                return PIH.CHECK.WORKSTATION.property(
                     workstation, AD.ComputerProperties.Shutdownable
                 )
 
             @staticmethod
             def rebootable(workstation: ComputerDescription) -> bool:
-                return PIH.CHECK.WORKSTATION.has_property(
+                return PIH.CHECK.WORKSTATION.property(
                     workstation, AD.ComputerProperties.Rebootable
                 )
 
         @staticmethod
         def telephone_number(value: str | int, international: bool = False) -> bool:
             return (
                 ne(value)
@@ -11170,15 +11691,15 @@
                 timeout: int = 60,
             ) -> None:
                 session = session or PIH.session
                 filter_user_login_list: list[str] = (
                     None
                     if filter_group is None
                     else ResultTool.map(
-                        lambda item: item.samAccountName.lower(),
+                        lambda item: item.login.lower(),
                         PIH.RESULT.USER.by_group(filter_group),
                     ).data
                 )
                 filter_user_login_list_is_empty: bool = e(filter_user_login_list)
                 to_all_user_workstation_name_list_is_empty: bool = e(
                     to_all_user_workstation_name_list
                 )
@@ -11186,15 +11707,15 @@
                 def filter_function(workstation: Workstation) -> bool:
                     workstation_name: str = workstation.name.lower()
                     if test:
                         return workstation_name == CONST.TEST.WORKSTATION_MAME
                     return workstation.accessable and (
                         (
                             filter_user_login_list_is_empty
-                            or workstation.samAccountName in filter_user_login_list
+                            or workstation.login in filter_user_login_list
                         )
                         or (
                             to_all_user_workstation_name_list_is_empty
                             or workstation_name in to_all_user_workstation_name_list
                         )
                     )
 
@@ -11235,26 +11756,26 @@
 
                     result_message: str = (
                         f"Сообщение от {session.user_given_name} ({PIH.DATA.FORMAT.description(session.get_user().description)}):"
                     )
                     result_message += f" День добрый, "
                     user: User | None = (
                         None
-                        if e(workstation.samAccountName)
+                        if e(workstation.login)
                         else PIH.RESULT.USER.by_login(
-                            workstation.samAccountName, True, True
+                            workstation.login, True, True
                         ).data
                     )
                     result_message += DataTool.if_not_empty(
                         user, lambda user: f"{FullNameTool.to_given_name(user)}, ", ""
                     )
                     result_message += message
                     PIH.MESSAGE.WORKSTATION.executor.submit(
                         PIH.ERROR.wrap(internal_send_message),
-                        workstation.samAccountName,
+                        workstation.login,
                         workstation.name.lower(),
                         result_message,
                     )
 
                 ResultTool.every(
                     every_action,
                     ResultTool.filter(filter_function, PIH.RESULT.WORKSTATION.all()),
@@ -11264,15 +11785,15 @@
             def to_user(
                 value: User | str,
                 message: str,
                 timeout: int = 60,
                 method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE,
             ) -> bool:
                 return PIH.MESSAGE.WORKSTATION.to_user_or_workstation(
-                    value.samAccountName if isinstance(value, User) else value,
+                    value.login if isinstance(value, User) else value,
                     None,
                     message,
                     timeout,
                     method_type,
                 )
 
             @staticmethod
@@ -11298,15 +11819,15 @@
             ) -> bool:
                 user: User | None = None
                 try:
                     user = PIH.RESULT.USER.by_workstation_name(value).data
                 except NotFound as _:
                     pass
                 return PIH.MESSAGE.WORKSTATION.to_user_or_workstation(
-                    None if n(user) else user.samAccountName,
+                    None if n(user) else user.login,
                     value,
                     message,
                     timeout,
                     method_type,
                 )
 
             @staticmethod
@@ -11384,58 +11905,74 @@
                 return PIH.MESSAGE.WORKSTATION.to_user_or_workstation(
                     value, None, message, timeout, method_type
                 )
 
         class WHATSAPP:
             class WAPPI:
                 class QUEUE:
-                    @staticmethod
-                    def add(
-                        message: Message,
-                        recipient: str,
-                        sender: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles,
-                        high_priority: bool = False,
-                    ) -> bool:
-                        return PIH.MESSAGE.WHATSAPP.WAPPI.QUEUE.add_message(
-                            Message(message, recipient, sender.value), high_priority
-                        )
 
                     @staticmethod
-                    def add_message(
-                        message: Message, high_priority: bool = False
-                    ) -> bool:
+                    def add(value: Message, high_priority: bool = False) -> bool:
+                        value.message = PIH.DATA.FORMAT.whatsapp_message(value.message)
                         return DataTool.rpc_decode(
                             PIH.SERVICE.call_command(
                                 ServiceCommands.add_message_to_queue,
-                                (message, high_priority),
+                                (value, high_priority),
                             )
                         )
 
                 WAPPI_PROFILE_MAP: dict | None = None
 
                 @staticmethod
+                def _get_header(
+                    profile: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles,
+                ) -> strdict:
+                    return {
+                        "accept": "application/json",
+                        "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORIZATION[
+                            profile
+                        ],
+                        "Content-Type": "application/json",
+                    }
+
+                @staticmethod
+                def _get_profile_value(
+                    profile: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles,
+                ) -> tuple[CONST.MESSAGE.WHATSAPP.WAPPI.Profiles, str]:
+                    return (
+                        profile := EnumTool.get_by_value(
+                            CONST.MESSAGE.WHATSAPP.WAPPI.Profiles,
+                            profile or CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT,
+                        ),
+                        EnumTool.get_value(
+                            profile,
+                            EnumTool.get(profile),
+                        ),
+                    )
+
+                @staticmethod
                 def get_wappi_collection() -> dict:
                     WP = CONST.MESSAGE.WHATSAPP.WAPPI
                     result: dict = PIH.MESSAGE.WHATSAPP.WAPPI.WAPPI_PROFILE_MAP or {
                         WP.Profiles.IT: PIH.DATA.TELEPHONE_NUMBER.it_administrator(),
                         WP.Profiles.CALL_CENTRE: PIH.DATA.TELEPHONE_NUMBER.call_centre_administrator(),
                         WP.Profiles.MARKETER: PIH.DATA.TELEPHONE_NUMBER.marketer_administrator(),
                     }
                     if PIH.MESSAGE.WHATSAPP.WAPPI.WAPPI_PROFILE_MAP is None:
                         PIH.MESSAGE.WHATSAPP.WAPPI.WAPPI_PROFILE_MAP = result
                     return result
 
                 @staticmethod
                 def send_to_group(
-                    group: CONST.MESSAGE.WHATSAPP.GROUP,
+                    group: CONST.MESSAGE.WHATSAPP.GROUP | str,
                     message: str,
                     profile: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles = CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.IT,
                 ) -> bool:
                     return PIH.MESSAGE.WHATSAPP.WAPPI.send(
-                        group.value, message, profile
+                        EnumTool.get(group), message, profile
                     )
 
                 @staticmethod
                 def get_profile_id(
                     telephone_number: str,
                 ) -> CONST.MESSAGE.WHATSAPP.WAPPI.Profiles:
                     if PIH.CHECK.telephone_number_international(telephone_number):
@@ -11451,24 +11988,25 @@
                     return None
 
                 @staticmethod
                 def get_message_list(
                     telephone_number: str,
                     profile: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | None = None,
                 ) -> list[WhatsAppMessage]:
-                    profile = EnumTool.get_by_value(
-                        CONST.MESSAGE.WHATSAPP.WAPPI.Profiles,
-                        profile or CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT,
-                    )
-                    profile_value: str = EnumTool.get_value(
-                        profile,
-                        EnumTool.get(profile),
+                    profile, profile_value = (
+                        PIH.MESSAGE.WHATSAPP.WAPPI._get_profile_value(profile)
                     )
-                    url: str = (
-                        f"{CONST.MESSAGE.WHATSAPP.WAPPI.URL_GET_MESSAGES}{profile_value}&chat_id={telephone_number}{CONST.MESSAGE.WHATSAPP.WAPPI.CONTACT_SUFFIX}"
+                    url: str = j(
+                        (
+                            CONST.MESSAGE.WHATSAPP.WAPPI.URL_GET_MESSAGES,
+                            profile_value,
+                            "&chat_id=",
+                            telephone_number,
+                            CONST.MESSAGE.WHATSAPP.WAPPI.CONTACT_SUFFIX,
+                        )
                     )
                     headers: dict = {
                         "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORIZATION[
                             profile
                         ],
                         "Content-Type": "application/json",
                     }
@@ -11488,198 +12026,184 @@
                             for message_item in response_result[key]:
                                 if message_item["type"] == "chat":
                                     result.append(
                                         WhatsAppMessage(
                                             message_item["body"],
                                             message_item["fromMe"],
                                             str(message_item["from"]).split(
-                                                A.CT.EMAIL_SPLITTER
+                                                CONST.EMAIL_SPLITTER
                                             )[0],
                                             str(message_item["to"]).split(
-                                                A.CT.EMAIL_SPLITTER
+                                                CONST.EMAIL_SPLITTER
                                             )[0],
                                             profile,
                                             message_item["time"],
                                         )
                                     )
                     return result
 
                 @staticmethod
-                def send(
-                    telephone_number: str,
-                    message: Any,
+                def send_location(
+                    recipient: str,
+                    value: tuple[float, float],
+                    address: str,
                     profile: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None = None,
                 ) -> bool:
-                    profile = EnumTool.get_by_value(
-                        CONST.MESSAGE.WHATSAPP.WAPPI.Profiles,
-                        profile or CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT,
+                    profile, profile_value = (
+                        PIH.MESSAGE.WHATSAPP.WAPPI._get_profile_value(profile)
                     )
-                    profile_value: str = EnumTool.get_value(
-                        profile,
-                        EnumTool.get(profile),
+                    payload: strdict = {"recipient": recipient}
+                    payload["latitude"] = value[0]
+                    payload["longitude"] = value[1]
+                    payload["address"] = address
+                    url: str = j(
+                        (CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_LOCATION, profile_value)
+                    )
+                    try:
+                        response: Response = requests.post(
+                            url,
+                            data=dumps(payload),
+                            headers=PIH.MESSAGE.WHATSAPP.WAPPI._get_header(profile),
+                        )
+                    except ConnectTimeout:
+                        return False
+                    if response.status_code == CONST.ERROR.WAPPI.PROFILE_NOT_PAID:
+                        PIH.LOG.resources(
+                            "Аккаунт Wappi (сервис для отправики сообщений через WhatsApp) не оплачен",
+                            LogMessageFlags.ERROR,
+                        )
+                    return response.status_code == 200
+
+                @staticmethod
+                def send(
+                    recipient: str,
+                    value: str,
+                    profile: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None = None,
+                ) -> bool:
+                    profile, profile_value = (
+                        PIH.MESSAGE.WHATSAPP.WAPPI._get_profile_value(profile)
                     )
                     url: str | None = None
-                    payload: dict = {"recipient": telephone_number}
-                    if isinstance(message, str):
-                        payload["body"] = message
+                    payload: dict = {"recipient": recipient}
+                    if isinstance(value, str):
+                        payload["body"] = value
                         url = CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_MESSAGE
-                    elif isinstance(
-                        message,
-                        (WhatsAppMessageListPayload, WhatsAppMessageButtonsPayload),
-                    ):
-                        for item_name in message.__dataclass_fields__:
-                            item_value: Any = message.__getattribute__(item_name)
-                            if ne(item_value):
-                                if item_name == "buttons":
-                                    payload[item_name] = list(
-                                        map(lambda button: button.__dict__, item_value)
-                                    )
-                                else:
-                                    payload[item_name] = item_value
-                        if isinstance(message, WhatsAppMessageListPayload):
-                            url = CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_LIST_MESSAGE
-                        else:
-                            url = CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_BUTTONS_MESSAGE
-                    url += profile_value
-                    headers: dict = {
-                        "accept": "application/json",
-                        "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORIZATION[
-                            profile
-                        ],
-                        "Content-Type": "application/json",
-                    }
+                    url = j((url, profile_value))
                     try:
                         response: Response = requests.post(
-                            url, data=dumps(payload), headers=headers
+                            url,
+                            data=dumps(payload),
+                            headers=PIH.MESSAGE.WHATSAPP.WAPPI._get_header(profile),
                         )
                     except ConnectTimeout:
                         return False
                     if response.status_code == CONST.ERROR.WAPPI.PROFILE_NOT_PAID:
                         PIH.LOG.resources(
                             "Аккаунт Wappi (сервис для отправики сообщений через WhatsApp) не оплачен",
                             LogMessageFlags.ERROR,
                         )
                     return response.status_code == 200
 
                 @staticmethod
                 def get_status(
                     profile: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None = None,
                 ) -> WappiStatus:
-                    profile = EnumTool.get_by_value(
-                        CONST.MESSAGE.WHATSAPP.WAPPI.Profiles,
-                        profile or CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT,
-                    )
-                    profile_value: str = EnumTool.get_value(
-                        profile,
-                        EnumTool.get(profile),
+                    profile, profile_value = (
+                        PIH.MESSAGE.WHATSAPP.WAPPI._get_profile_value(profile)
                     )
                     url: str = j((CONST.MESSAGE.WHATSAPP.WAPPI.STATUS, profile_value))
-                    headers: dict = {
-                        "accept": "application/json",
-                        "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORIZATION[
-                            profile
-                        ],
-                        "Content-Type": "application/json",
-                    }
                     try:
-                        response: Response = requests.get(url, headers=headers)
+                        response: Response = requests.get(
+                            url, headers=PIH.MESSAGE.WHATSAPP.WAPPI._get_header(profile)
+                        )
                     except ConnectTimeout:
                         return False
                     return DataTool.fill_data_from_source(
                         WappiStatus(), json.loads(response.text)
                     )
 
                 @staticmethod
                 def send_base64_file(
                     url: str,
-                    telephone_number: str,
+                    recipient: str,
                     caption: str,
                     file_name: str | None,
                     base64_content: str,
                     profile: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None = None,
                 ) -> bool:
-                    profile = EnumTool.get_by_value(
-                        CONST.MESSAGE.WHATSAPP.WAPPI.Profiles,
-                        profile or CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT,
+                    profile, profile_value = (
+                        PIH.MESSAGE.WHATSAPP.WAPPI._get_profile_value(profile)
                     )
-                    profile_value: str = EnumTool.get_value(
-                        profile,
-                        EnumTool.get(profile),
-                    )
-                    payload: dict = {
-                        "recipient": telephone_number,
+                    payload: strdict = {
+                        "recipient": recipient,
                         "caption": caption,
                         "b64_file": base64_content,
                     }
                     if ne(file_name):
                         payload["file_name"] = file_name
-                    headers: dict = {
-                        "accept": "application/json",
-                        "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORIZATION[
-                            profile
-                        ],
-                        "Content-Type": "application/json",
-                    }
-                    url = url + profile_value
+
+                    url = j((url, profile_value))
                     try:
                         response: Response = requests.post(
-                            url, data=dumps(payload), headers=headers
+                            url,
+                            data=dumps(payload),
+                            headers=PIH.MESSAGE.WHATSAPP.WAPPI._get_header(profile),
                         )
                     except ConnectTimeout:
                         return False
                     if response.status_code == CONST.ERROR.WAPPI.PROFILE_NOT_PAID:
                         PIH.LOG.resources(
                             "Аккаунт Wappi (сервис для отправики сообщений через WhatsApp) не оплачен",
                             LogMessageFlags.ERROR,
                         )
                     return response.status_code == 200
 
                 @staticmethod
                 def send_video(
-                    telephone_number: str,
+                    recipient: str,
                     caption: str,
                     base64_content: str,
-                    profile: Any = None,
+                    profile: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None = None,
                 ) -> bool:
                     return PIH.MESSAGE.WHATSAPP.WAPPI.send_base64_file(
                         CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_VIDEO,
-                        telephone_number,
+                        recipient,
                         caption,
                         None,
                         base64_content,
                         profile,
                     )
 
                 @staticmethod
                 def send_image(
-                    telephone_number: str,
+                    recipient: str,
                     caption: str,
                     base64_content: str,
-                    profile: Any = None,
+                    profile: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None = None,
                 ) -> bool:
                     return PIH.MESSAGE.WHATSAPP.WAPPI.send_base64_file(
                         CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_IMAGE,
-                        telephone_number,
+                        recipient,
                         caption,
                         None,
                         base64_content,
                         profile,
                     )
 
                 @staticmethod
                 def send_document(
-                    telephone_number: str,
+                    recipient: str,
                     caption: str,
                     file_name: str,
                     base64_content: str,
-                    profile: Any = None,
+                    profile: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None = None,
                 ) -> bool:
                     return PIH.MESSAGE.WHATSAPP.WAPPI.send_base64_file(
                         CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_DOCUMENT,
-                        telephone_number,
+                        recipient,
                         caption,
                         file_name,
                         base64_content,
                         profile,
                     )
 
             @staticmethod
@@ -11700,84 +12224,90 @@
 
                     pwk.sendwhatmsg_instantly(telephone_number, message)
                 except Exception as уrror:
                     PIH.output.error("Ошибка при отправке сообщения!")
 
             @staticmethod
             def send(
-                telephone_number: str,
+                recipient: str,
                 message: Any,
                 via_wappi: bool = True,
                 use_alternative: bool = True,
-                wappi_profile: Any = None,
+                wappi_profile: (
+                    CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None
+                ) = None,
             ) -> bool:
                 wappi_profile = EnumTool.get_value(
                     wappi_profile,
                     EnumTool.get(CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT),
                 )
                 result: bool = False
-                telephone_number = PIH.DATA.FORMAT.telephone_number(telephone_number)
+                recipient = PIH.DATA.FORMAT.telephone_number(recipient)
                 if via_wappi:
                     result = PIH.MESSAGE.WHATSAPP.WAPPI.send(
-                        telephone_number, message, wappi_profile
+                        recipient, message, wappi_profile
                     )
                 if result:
                     return result
                 if use_alternative or not via_wappi:
-                    return PIH.MESSAGE.WHATSAPP.send_via_browser(
-                        telephone_number, message
-                    )
+                    return PIH.MESSAGE.WHATSAPP.send_via_browser(recipient, message)
                 return False
 
             @staticmethod
             def send_video(
-                telephone_number: str,
+                recipient: str,
                 caption: str,
                 base64_value: str,
-                wappi_profile: Any = None,
+                wappi_profile: (
+                    CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None
+                ) = None,
             ) -> bool:
                 wappi_profile = EnumTool.get_value(
                     wappi_profile,
                     EnumTool.get(CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT),
                 )
-                telephone_number = PIH.DATA.FORMAT.telephone_number(telephone_number)
+                recipient = PIH.DATA.FORMAT.telephone_number(recipient)
                 return PIH.MESSAGE.WHATSAPP.WAPPI.send_video(
-                    telephone_number, caption, base64_value, wappi_profile
+                    recipient, caption, base64_value, wappi_profile
                 )
 
             @staticmethod
             def send_image(
-                telephone_number: str,
+                recipient: str,
                 caption: str,
                 base64_value: str,
-                wappi_profile: Any = None,
+                wappi_profile: (
+                    CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None
+                ) = None,
             ) -> bool:
                 wappi_profile = EnumTool.get_value(
                     wappi_profile,
                     EnumTool.get(CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT),
                 )
-                telephone_number = PIH.DATA.FORMAT.telephone_number(telephone_number)
+                recipient = PIH.DATA.FORMAT.telephone_number(recipient)
                 return PIH.MESSAGE.WHATSAPP.WAPPI.send_image(
-                    telephone_number, caption, base64_value, wappi_profile
+                    recipient, caption, base64_value, wappi_profile
                 )
 
             @staticmethod
             def send_document(
-                telephone_number: str,
+                recipient: str,
                 caption: str,
                 base64_value: str,
-                wappi_profile: Any = None,
+                wappi_profile: (
+                    CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None
+                ) = None,
             ) -> bool:
                 wappi_profile = EnumTool.get_value(
                     wappi_profile,
                     EnumTool.get(CONST.MESSAGE.WHATSAPP.WAPPI.Profiles.DEFAULT),
                 )
-                telephone_number = PIH.DATA.FORMAT.telephone_number(telephone_number)
+                recipient = PIH.DATA.FORMAT.telephone_number(recipient)
                 return PIH.MESSAGE.WHATSAPP.WAPPI.send_document(
-                    telephone_number, caption, base64_value, wappi_profile
+                    recipient, caption, base64_value, wappi_profile
                 )
 
             @staticmethod
             def send_to_user(
                 user: User,
                 message: Any,
                 via_wappi: bool = True,
@@ -12035,14 +12565,24 @@
                         )
                     ),
                 ),
             ).data
 
     class ACTION:
 
+        @staticmethod
+        def _call(service_role: ServiceRoles, *args) -> bool:
+            return DataTool.rpc_decode(
+                PIH.SERVICE.call(
+                    service_role,
+                    ServiceCommands.serve_command,
+                    *args,
+                )
+            )
+
         class ZABBIX:
 
             @staticmethod
             def send(host: str, key: str, value: Any) -> bool:
                 return DataTool.rpc_decode(
                     PIH.SERVICE.call(
                         ServiceRoles.ZABBIX,
@@ -12112,15 +12652,15 @@
                     EnumTool.get(tag)
                 )
                 PIH.EVENT.send(
                     Events.ADD_JOURNAL_RECORD,
                     (
                         tag_value[0],
                         journal_type_value[0],
-                        applicant_user.samAccountName,
+                        applicant_user.login,
                         escape_string(title),
                         escape_string(text),
                         js((tag_value[1].icon, tag_value[1].caption)),
                         journal_type_value[1].caption,
                         parameters,
                     ),
                 )
@@ -12172,15 +12712,15 @@
                     return None
                 PIH.EVENT.send(
                     Events.ACTION_WAS_DONE,
                     (
                         EnumTool.get(_action).description,
                         _action.name,
                         user.name,
-                        user.samAccountName,
+                        user.login,
                         parameters,
                         forced,
                     ),
                 )
                 return True
 
             @staticmethod
@@ -12434,25 +12974,40 @@
                     data: dict = PIH.SERVICE.call_command(
                         ServiceCommands.register_chiller_indications_value,
                         (value, forced),
                     )
                     return ne(data)
 
         class MOBILE_INPUT_OUTPUT:
+
+            @staticmethod
+            def send_outside(
+                value: str, recipient: str, flags: int | None = None
+            ) -> None:
+                PIH.ACTION.MOBILE_INPUT_OUTPUT.send(
+                    value,
+                    recipient,
+                    flags=BM.add(
+                        (flags or 0), (SessionFlags.OUTSIDE, SessionFlags.CLI)
+                    ),
+                    use_command_prefix=False,
+                )
+
             @staticmethod
-            def send_command_to(
+            def send(
                 value: str,
                 recipient: str | Enum,
                 chat_id: str | Enum | None = None,
                 flags: int | None = None,
                 return_result_key: str | None = None,
                 args: tuple[Any, ...] | None = None,
+                use_command_prefix: bool = True,
             ) -> None:
                 recipient = EnumTool.get(recipient)
-                if not value.startswith(PIH.NAME):
+                if use_command_prefix and not value.startswith(PIH.NAME):
                     value = js((PIH.NAME, value))
                 PIH.EVENT.whatsapp_message_received(
                     WhatsAppMessage(
                         value,
                         False,
                         recipient,
                         recipient,
@@ -12461,24 +13016,14 @@
                         EnumTool.get(chat_id),
                         flags,
                         return_result_key,
                         args,
                     )
                 )
 
-            @staticmethod
-            def write(
-                telephone_number: str,
-                message: Any,
-                profile: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None = None,
-            ) -> bool:
-                return PIH.MESSAGE.WHATSAPP.WAPPI.send(
-                    telephone_number, message, profile
-                )
-
         class BACKUP:
             @staticmethod
             def start_robocopy_job(
                 name: str | None = None,
                 source: str | None = None,
                 destination: str | None = None,
                 force: bool = False,
@@ -12573,14 +13118,20 @@
                     PIH.SERVICE.call_command(
                         ServiceCommands.set_settings_value, (key, value)
                     )
                 )
 
             @staticmethod
             def set(settings_item: SETTINGS | str, value: Any) -> bool:
+                settings_item_value = EnumTool.get(settings_item)
+                if isinstance(settings_item_value, VariantableStorageVariable):
+                    if value not in settings_item_value.variants:
+                        raise NotFound(
+                            js((value, "not in", settings_item_value.variants))
+                        )
                 return PIH.ACTION.SETTINGS.key(
                     if_else(
                         isinstance(settings_item, str),
                         settings_item,
                         lambda: settings_item.value.key_name or settings_item.name,
                     ),
                     value,
@@ -12665,16 +13216,16 @@
                     )
                 )
 
         class TIME_TRACKING:
             @staticmethod
             def save_report(
                 path: str,
-                start_date: datetime,
-                end_date: datetime,
+                start_date: datetime | date,
+                end_date: datetime | date,
                 tab_number_list: list[str] | None = None,
                 plain_format: bool = False,
             ) -> bool:
                 return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.save_time_tracking_report,
                         (
@@ -13187,14 +13738,29 @@
     def person_barcode(person_pin: int) -> str:
         return PIH.PATH.join(
             PATH_POLIBASE.person_folder(person_pin),
             POLIBASE.BARCODE.get_file_name(person_pin, with_extension=True),
         )
 
 
+def pih_package_name(standalone_name: str) -> str:
+    return PIH.PATH.FACADE.DITRIBUTIVE.NAME(standalone_name)
+
+
+def import_from(file_name: str, *args) -> list[Any]:
+    import_result: strdict = PIH.RESULT.FILES.execute(file_name, stdout_redirect=False)
+    result: list[Any] = []
+    if n(args):
+        return import_result
+    for item in args:
+        if item in import_result:
+            result.append(import_result[item])
+    return result
+
+
 class A:
 
     root = PIH()
 
     NAME = PIH.NAME
 
     IW = root.INPUT_WAIT
@@ -13234,14 +13800,16 @@
     D_MR = D.MATERIALIZED_RESOURCES
     D_FL = D.FILTER
     D_Ex = D.EXTRACT
     D_Ex_E = D_Ex.EVENT
     D_M = D.MARK
     D_C = D.CHECK
     D_STAT = D.STATISTICS
+    D_IOT = D.IOTDevices
+
     D_U = D.USER
     D_J = D.JOURNAL
     A = root.ACTION
     A_F = A.FILES
 
     A_DOC = A.DOCUMENTS
     A_SSH = A.SSH
@@ -13297,22 +13865,24 @@
     C_ME = C.MESSAGE
     C_ME_WH = C_ME.WHATSAPP
     C_ME_WH_W = C_ME_WH.WAPPI
     C_N = C.NOTES
     C_J = C.JOURNALS
     C_EML = C.EMAIL
     C_RCG = C.RECOGNIZE
+    C_F = C.FILES
     #
     A_DR = A.DOOR
     A_M = A.MARK
     A_COMP = A.COMPUTER
     A_U = A.USER
     C_U = C.USER
     D_F = D.FORMAT
     D_F_B = D_F.BACKUP
+    D_F_IOT = D_F.IOTDevices
     D_CO = D.CONVERT
     A_P = A.POLIBASE
     A_INV = A.INVENTORY
     C_E = C.EVENTS
     C_P = C.POLIBASE
     C_P_DB = C_P.DATABASE
     D_P = D.POLIBASE
@@ -13474,14 +14044,39 @@
     sc: ServiceCommands,
     type: int = SUBSCRIBTION_TYPE.ON_RESULT,
     name: str | None = None,
 ) -> bool:
     return A.SRV_A.subscribe_on(sc, type, name)
 
 
+def send_message(
+    value: str | Message,
+    recipient: str | Enum | None = None,
+    sender: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None = None,
+    queued: bool = False,
+) -> bool:
+    if isinstance(value, Message):
+        queued = True
+    if nn(recipient):
+        recipient = EnumTool.get(recipient)
+    if queued:
+        return PIH.MESSAGE.WHATSAPP.WAPPI.QUEUE.add(
+            value
+            if isinstance(value, Message)
+            else Message(
+                value,
+                recipient,
+                EnumTool.get(sender),
+            )
+        )
+    return PIH.MESSAGE.WHATSAPP.WAPPI.send(
+        recipient, PIH.DATA.FORMAT.whatsapp_message(value), sender
+    )
+
+
 def serve(
     service_role_or_description: ServiceRoles | ServiceDescriptionBase,
     call_handler: Callable[[ServiceCommands, ParameterList], Any] | None = None,
     starts_handler: Callable[[IService], None] | Callable[[], None] | None = None,
     started_handler: Callable[[], None] | None = None,
     max_workers: int | None = None,
     stop_before: bool = True,
@@ -13501,7 +14096,14 @@
         internal_starts_handler,
         max_workers,
         stop_before=True,
         isolate=isolate,
         as_standalone=as_standalone,
         show_output=show_output,
     )
+
+
+def isolate(
+    *service_role_or_description: tuple[ServiceRoles | ServiceDescriptionBase, ...],
+) -> None:
+    for item in service_role_or_description:
+        PIH.SERVICE.ADMIN.isolate(item)
```

### Comparing `pih-0.36.9/pih/rpc/__init__.py` & `pih-0.37/pih/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.9/pih/rpc/rpcCommandCall_pb2.py` & `pih-0.37/pih/rpc/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.9/pih/rpc/rpcCommandCall_pb2_grpc.py` & `pih-0.37/pih/rpc/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.9/pih/tools/__init__.py` & `pih-0.37/pih/tools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 import os
 import sys
 import json
 import shlex
+import pycron
 import socket
 import string
 import random
 import ntpath
 import pathlib
 import calendar
 import platform
@@ -17,14 +18,15 @@
 from operator import itemgetter
 from contextlib import contextmanager
 from inspect import isfunction, isclass
 from typing import Any, Callable, Tuple, List
 from datetime import date, datetime, timedelta
 
 from pih.consts.password import RULES
+from pih.consts.style import *
 from pih.consts.date_time import DATE_TIME
 from pih.consts.names import FieldCollectionAliases
 
 from pih.collections import (
     R,
     T,
     User,
@@ -33,18 +35,21 @@
     FieldItem,
     FieldItemList,
     PolibasePerson,
 )
 
 
 def if_else(
-    check_value: bool,
+    check_value: bool | None,
     true_value: Callable[[], Any] | Any,
     false_value: Callable[[], Any] | Any = None,
+    none_value: Callable[[], Any] | Any = None,
 ) -> Any:
+    if n(check_value) and nn(none_value):
+        return none_value() if callable(none_value) else none_value
     return (
         (true_value() if callable(true_value) else true_value)
         if check_value
         else (
             false_value()
             if not n(false_value) and callable(false_value)
             else false_value
@@ -98,23 +103,27 @@
     return value
 
 
 def nnt(value: T | None) -> T:
     return value
 
 
-def nns(value: Any) -> str:
-    return value
+def nns(value: Any, default_value: str | None = None) -> str:
+    if value == "":
+        return value
+    return value or default_value
 
 
 def nnb(value: Any) -> bytes:
     return value
 
 
-def nni(value: Any) -> int:
+def nni(value: Any, default_value: int | None = None) -> int:
+    if n(value) and nn(default_value):
+        return nni(default_value)
     return value
 
 
 def nndt(value: Any) -> datetime:
     return value
 
 
@@ -273,14 +282,29 @@
         return [] if n(value) else list(map(function, DataTool.as_list(value)))
 
     @staticmethod
     def filter(function: Callable[[Any], bool], value: list[Any] | Any) -> list[Any]:
         return [] if n(value) else list(filter(function, DataTool.as_list(value)))
 
     @staticmethod
+    def filter_by_string(
+        string: str,
+        value: list[Any] | Any,
+        label_function: Callable[[Any], str] | None = None,
+    ) -> list[Any]:
+        string = lw(string)
+        return DataTool.filter(
+            lambda item: (
+                lw(item if n(label_function) else label_function(item)).find(string)
+            )
+            != -1,
+            value,
+        )
+
+    @staticmethod
     def as_value(
         function_or_value: Callable[[], str] | Callable[[Any], str] | str | None,
         parameters: Any = None,
     ) -> str:
         return (
             (function_or_value() if n(parameters) else function_or_value(parameters))
             if callable(function_or_value)
@@ -303,15 +327,17 @@
         if n(data):
             return default_value
         if len(data) <= index:
             return default_value
         return data[index]
 
     @staticmethod
-    def rpc_encode(data: dict | None, ensure_ascii: bool = True) -> str | None:
+    def rpc_encode(
+        data: dict[str, Any] | None, ensure_ascii: bool = True
+    ) -> str | None:
         return (
             None
             if n(data)
             else json.dumps(data, cls=PIHEncoder, ensure_ascii=ensure_ascii)
         )
 
     @staticmethod
@@ -530,19 +556,20 @@
                 return arg_name in value.__members__
         except TypeError:
             pass
         return arg_name in value
 
     @staticmethod
     def check(
-        check_value: bool,
+        check_value: bool | None,
         true_value: Callable[[], Any] | Any,
         false_value: Callable[[], Any] | Any = None,
+        none_value: Callable[[], Any] | Any = None,
     ) -> Any:
-        return if_else(check_value, true_value, false_value)
+        return if_else(check_value, true_value, false_value, none_value)
 
     @staticmethod
     def check_not_none(
         check_value: Any | list[Any] | tuple[Any, ...] | None,
         true_value: Callable[[], Any] | Any,
         false_value: Callable[[], Any] | Any = None,
         check_all: bool = False,
@@ -613,15 +640,15 @@
     def is_fullname(value: str, split_symbol: str = SPLIT_SYMBOL) -> bool:
         return (
             len(ListTool.not_empty_items(value.split(split_symbol)))
             >= FullNameTool.FULL_NAME_LENGTH
         )
 
     @staticmethod
-    def is_equal(fn_a: FullName, fn_b: FullName) -> bool:
+    def is_equal_by_fullname(fn_a: FullName, fn_b: FullName) -> bool:
         return (
             fn_a.first_name == fn_b.first_name
             and fn_a.middle_name == fn_b.middle_name
             and fn_a.last_name == fn_b.last_name
         )
 
     @staticmethod
@@ -668,24 +695,28 @@
             if isinstance(bit, int):
                 value |= bit
             elif isinstance(bit, Enum):
                 value |= bit.value
         return value
 
     @staticmethod
+    def set_index(value: int, index: int) -> int:
+        return BitMask.add(value, 2**index)
+
+    @staticmethod
     def set(bit: int | tuple[Enum, ...] | Enum | list[Enum] | list[int]) -> int:
         return BitMask.add(0, bit)
 
     @staticmethod
     def value(bit: int | tuple[Enum, ...] | Enum | list[Enum] | list[int]) -> int:
         return BitMask.add(0, bit)
 
     @staticmethod
     def has(
-        value: int | tuple[Enum, ...] | Enum | list[Enum] | list[int],
+        value: int | tuple[Enum, ...] | Enum | list[Enum] | list[int] | None,
         bit: int | tuple[Enum, ...] | Enum | list[Enum] | list[int],
     ) -> bool:
         if n(value):
             return False
         value = BitMask.value(value)
         bits: list[int] = bit if isinstance(bit, (list, tuple)) else [bit]
         result: bool = False
@@ -702,15 +733,17 @@
         return result
 
     @staticmethod
     def has_index(value: int, index: int) -> bool:
         return BitMask.has(value, pow(2, index))
 
     @staticmethod
-    def remove(value: int, bit: int | Enum) -> int:
+    def remove(value: int | tuple[Enum, ...], bit: int | Enum) -> int:
+        if not isinstance(value, int):
+            value = BitMask.value(value)
         if isinstance(bit, Enum):
             bit = bit.value
         if BitMask.has(value, bit):
             value ^= bit
         return value
 
 
@@ -835,14 +868,34 @@
         result: Result[list[T]],
         use_index: bool = False,
     ) -> Result[list[T]]:
         result.data = DataTool.every(action_function, result.data, use_index)
         return result
 
     @staticmethod
+    def every_with_fields(
+        action_function: Callable[[T, int, FieldItemList], None] | Callable[[T], None],
+        result: Result[list[T]],
+        use_index: bool = False,
+    ) -> Result[list[T]]:
+        return (
+            ResultTool.every(
+                lambda item, index: action_function(item, index, result.fields),
+                result,
+                use_index,
+            )
+            if use_index
+            else ResultTool.every(
+                lambda item: action_function(item, result.fields),
+                result,
+                use_index,
+            )
+        )
+
+    @staticmethod
     def do_while(result: Result[list[T]], check_function: Callable[[T], bool]) -> Any:
         result_data: Any = None
         for item in result.data:
             if check_function(item):
                 result_data = item
                 break
         return result_data
@@ -879,15 +932,15 @@
 
 def lw(
     value: str | list[str] | tuple[str, ...] | None
 ) -> str | list[str] | tuple[str, ...]:
     if n(value):
         return ""
     if isinstance(value, str):
-        return value.lower()
+        return lw([value])[0]
     return DataTool.map(str.lower, value)
 
 
 def e(value: Any | Result[Any]) -> bool:
     return (
         ResultTool.is_empty(value)
         if isinstance(value, Result)
@@ -907,28 +960,28 @@
     strip_value: str = value.strip()
     index: int = value.find(strip_value)
     left: str = value[0:index]
     right: str = value[index + len(strip_value) :]
     return (left, strip_value, right)
 
 
+def b(value: Any) -> str:
+    return j((BOLD_BEGIN, str(value).strip(), BOLD_END))
+
+
 def i(value: Any) -> str:
-    if ne(value):
-        value = str(value).strip()
-        if value.find("_") == -1:
-            return j(("_", value, "_"))
-    return value or ""
+    return j((ITALICS_BEGIN, str(value).strip(), ITALICS_END))
 
 
-def b(value: Any) -> str:
-    if ne(value):
-        left, value, right = separate_on_parts(value)
-        if value.find("*") == -1:
-            return j((left, "*", value, "*", right))
-    return value or ""
+def surround_text_with(text: Any, value: str) -> str:
+    if ne(text):
+        left, text, right = separate_on_parts(text)
+        if text.find(value) == -1:
+            return j((left, value, text, value, right))
+    return text or ""
 
 
 def lnk(value: str) -> str:
     return j(("{", value, "}"))
 
 
 def esc(value: Any, single: bool = False) -> str:
@@ -943,17 +996,52 @@
 def escs(
     value: Any,
 ) -> str:
     return esc(value, True)
 
 
 class ListTool:
+
     @staticmethod
     def diff(a: list[Any], b: list[Any]) -> list[Any]:
-        return [i for i in a + b if i not in a or i not in b]
+        return [i for i in a + b if not (i in a and i in b)]
+
+    @staticmethod
+    def list_str_diff(
+        a: list[str],
+        b: list[str],
+    ) -> list[str]:
+        def compare_function(value1: str, value2: list[str]) -> bool:
+            for item in value2:
+                if StringTool.contains(value1, item, True):
+                    return True
+            return False
+
+        return [
+            i for i in a + b if not (compare_function(i, a) and compare_function(i, b))
+        ]
+
+    @staticmethod
+    def intersection(a: list[Any], b: list[Any]) -> bool:
+        return len(ListTool.diff(a, b)) < (len(a) + len(b))
+
+    @staticmethod
+    def list_of_str_intersection(a: list[str], b: list[str]) -> bool:
+        return ListTool.list_str_intersection_ratio(a, b) < (len(a) + len(b))
+
+    @staticmethod
+    def list_str_intersection_ratio(
+        a: list[str],
+        b: list[str],
+    ) -> int:
+        return len(ListTool.list_str_diff(a, b))
+
+    @staticmethod
+    def str_list_equal(a: list[str], b: list[str]) -> bool:
+        return len(ListTool.list_str_diff(a, b)) == 0
 
     @staticmethod
     def to_dict_with_none_value(
         value: list[Any], modificator: Callable[[Any], Any] | None = None
     ) -> dict[Any, None]:
         return {item if n(modificator) else modificator(item): None for item in value}  # type: ignore
 
@@ -967,14 +1055,129 @@
 
     @staticmethod
     def not_less_length_items(value: list[Any], length: int) -> list[Any]:
         return list(filter(lambda item: ne(item) and len(item) >= length, value))
 
 
 class StringTool:
+
+    @staticmethod
+    def bold(value: Any) -> str:
+        return j((BOLD_BEGIN, str(value).strip(), BOLD_END))
+
+    @staticmethod
+    def italics(value: Any) -> str:
+        return j((ITALICS_BEGIN, str(value).strip(), ITALICS_END))
+
+    @staticmethod
+    def split(value: str, delimiters: tuple[str, ...] | str) -> list[str]:
+        if isinstance(delimiters, str):
+            delimiters = (delimiters,)
+        for delimiter in delimiters:
+            value = js(value.split(delimiter))
+        return StringTool.space_format(value).split(" ")
+
+    @staticmethod
+    def _comparation_ratio_by_tokens(
+        a: str,
+        b: str,
+        token_delimiter: str | tuple[str, ...] = " ",
+    ) -> tuple[int, list[str], list[str]]:
+        if isinstance(token_delimiter, str):
+            token_delimiter = (token_delimiter,)
+        a = lw(a)
+        b = lw(b)
+        a_list: list[str] = StringTool.split(a, token_delimiter)
+        b_list: list[str] = StringTool.split(b, token_delimiter)
+        a_list = ListTool.not_empty_items(list(set(a_list)))
+        b_list = ListTool.not_empty_items(list(set(b_list)))
+        return (
+            ListTool.list_str_intersection_ratio(a_list, b_list),
+            a_list,
+            b_list,
+        )
+
+    @staticmethod
+    def equal_by_tokens(
+        a: str,
+        b: str,
+        token_delimiter: str | tuple[str, ...] = " ",
+    ) -> bool:
+        return StringTool._comparation_ratio_by_tokens(a, b, token_delimiter)[0] == 0
+
+    @staticmethod
+    def intersection_by_tokens(
+        a: str,
+        b: str,
+        token_delimiter: str | tuple[str, ...] = " ",
+    ) -> bool:
+        result: tuple[int, list[str], list[str]] = (
+            StringTool._comparation_ratio_by_tokens(a, b, token_delimiter)
+        )
+        return result[0] < (len(result[1]) + len(result[2]))
+
+    @staticmethod
+    def full_right_intersection_by_tokens(
+        a: str,
+        b: str,
+        token_delimiter: str | tuple[str, ...] = " ",
+    ) -> bool:
+        if a.find(b) != -1:
+            return True
+        result: tuple[int, list[str], list[str]] = (
+            StringTool._comparation_ratio_by_tokens(a, b, token_delimiter)
+        )
+        return result[0] == (len(result[1]) - len(result[2]))
+
+    @staticmethod
+    def has_one_of(text: str, variants: list[str]) -> bool:
+        def mapper(value: str) -> str:
+            value = value.replace(" ", "[ ,]*")
+            value_variable_list: list[str] = ListTool.not_empty_items(value.split("|"))
+            if len(value_variable_list) > 1:
+                value = j(
+                    (
+                        value_variable_list[0],
+                        r"(?:\(|",
+                        j(value_variable_list[1:], "|"),
+                        "|$)",
+                    )
+                )
+            return value
+
+        return nn(
+            re.search(
+                j(
+                    (
+                        r"\b(",
+                        j(
+                            DataTool.map(
+                                mapper,
+                                variants,
+                            ),
+                            "|",
+                        ),
+                        r")\b",
+                    )
+                ),
+                text,
+                flags=re.IGNORECASE,
+            )
+        )
+
+    @staticmethod
+    def space_format(value: str | None) -> str | None:
+        if n(value):
+            return value
+        return nns(value).replace("\xa0", " ")
+
+    @staticmethod
+    def split_by_space(value: str | None) -> list[str]:
+        return StringTool.space_format((value or "")).split(" ")
+
     @staticmethod
     def contains(value1: str, value2: str, start_with: bool = False) -> bool:
         if n(value1) or n(value2):
             return False
 
         def eq(value1: str, value2: str) -> bool:
             return (
@@ -1136,58 +1339,67 @@
         result: str = ""
         for item in value:
             result += dictionary[item] if item in dictionary else item
         return result
 
 
 class DateTimeTool:
+
+    @staticmethod
+    def is_now(cron_string: str, value: datetime | None = None) -> bool:
+        cron_string = cron_string.strip()
+        as_time_list: list[str] = cron_string.split(":")
+        if len(as_time_list) > 1:
+            cron_string = js((as_time_list[1], as_time_list[0], "*", "*", "*"))
+        else:
+            length: int = len(cron_string.split(" "))
+            need_length: int = 5
+            if length < need_length:
+                cron_string = j((cron_string, " *" * (need_length - length)))
+        return pycron.is_now(cron_string, value)
+
     @staticmethod
     def day_count(date: date | datetime, month_count: int) -> int:
         result: int = 0
         year: int = date.year
         month: int = date.month
         current_month: int = month
         for _ in range(month_count):
             if current_month > 12:
                 year += 1
                 current_month = 1
             result += calendar.monthrange(year, current_month)[1]
             current_month += 1
-        # return month_count*31
         return result
 
     @staticmethod
     def add_months(date: date | datetime, value: int) -> date | datetime:
         return date + timedelta(days=DateTimeTool.day_count(date, value))
 
     @staticmethod
     def seconds_to_days(value: int) -> float:
         return value / 60 / 60 / 24
 
     @staticmethod
-    def yesterday() -> datetime:
-        return DateTimeTool.today(-1, as_datetime=True)
+    def yesterday(as_datetime: bool = False) -> datetime | date:
+        return DateTimeTool.today(-1, as_datetime=as_datetime)
 
     @staticmethod
     def begin_date(value: datetime | date | None = None) -> datetime | date:
         value = value or DateTimeTool.today(as_datetime=True)
-        return (
-            value.replace(hour=0, minute=0, second=0, microsecond=0)
-            if isinstance(value, datetime)
-            else value
-        )
+        if isinstance(value, date):
+            value = datetime.combine(value, datetime.min.time())
+        return value.replace(hour=0, minute=0, second=0, microsecond=0)
 
     @staticmethod
     def end_date(value: datetime | date | None = None) -> datetime | date:
         value = value or DateTimeTool.today(as_datetime=True)
-        return (
-            value.replace(hour=23, minute=59, second=59, microsecond=0)
-            if isinstance(value, datetime)
-            else value
-        )
+        if isinstance(value, date):
+            value = datetime.combine(value, datetime.min.time())
+        return value.replace(hour=23, minute=59, second=59, microsecond=0)
 
     @staticmethod
     def timestamp() -> int:
         return int(datetime.now().timestamp())
 
     @staticmethod
     def date_or_today_string(value: datetime | None, format: str | None = None) -> str:
@@ -1201,25 +1413,27 @@
     def today_string(format: str | None = None, delta_days: int = 0) -> str:
         return DateTimeTool.datetime_to_string(
             DateTimeTool.today(delta_days, as_datetime=True), format
         )
 
     @staticmethod
     def datetime_to_string(
-        date: datetime | None, format: str | None = None
+        date: datetime | date | None, format: str | None = None
     ) -> str | None:
         if n(date):
             return None
         return DataTool.check_not_none(
             format, lambda: date.strftime(format), lambda: date.isoformat()
         )
 
     @staticmethod
-    def date_to_string(date: datetime, format: str | None = None) -> str:
-        return DateTimeTool.datetime_to_string(date.date(), format)
+    def date_to_string(date: datetime | date, format: str | None = None) -> str:
+        return DateTimeTool.datetime_to_string(
+            date.date() if isinstance(date, datetime) else date, format
+        )
 
     @staticmethod
     def to_date_string(isoformat_date_string: str) -> str:
         return isoformat_date_string.split(DATE_TIME.SPLITTER)[0]
 
     @staticmethod
     def today(delta_days: int = 0, as_datetime: bool = False) -> date | datetime:
@@ -1285,15 +1499,17 @@
         return result.date()
 
     @staticmethod
     def date_from_string(value: str) -> date | None:
         return DateTimeTool.datetime_or_date_from_string(value, as_date=True)
 
     @staticmethod
-    def is_equal_by_time(date: datetime, value: tuple | list | datetime) -> bool | None:
+    def is_equal_by_time(
+        date: datetime, value: datetime | tuple[int, int] | list[int]
+    ) -> bool | None:
         if isinstance(value, (tuple, list)):
             return date.hour == value[0] and date.minute == value[1]
         if isinstance(value, datetime):
             return date.hour == value.hour and date.minute == value.minute
         return None
```

### Comparing `pih-0.36.9/pih/tools/service.py` & `pih-0.37/pih/tools/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.9/pih/widgets.py` & `pih-0.37/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.9/pih.egg-info/SOURCES.txt` & `pih-0.37/pih.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -30,13 +30,14 @@
 pih/consts/recognize.py
 pih/consts/rpc.py
 pih/consts/service.py
 pih/consts/service_commands.py
 pih/consts/service_roles.py
 pih/consts/settings.py
 pih/consts/ssh_hosts.py
+pih/consts/style.py
 pih/consts/zabbix.py
 pih/rpc/__init__.py
 pih/rpc/rpcCommandCall_pb2.py
 pih/rpc/rpcCommandCall_pb2_grpc.py
 pih/tools/__init__.py
 pih/tools/service.py
```

