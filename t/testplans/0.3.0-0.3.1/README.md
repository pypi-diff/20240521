# Comparing `tmp/testplans-0.3.0.tar.gz` & `tmp/testplans-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testplans-0.3.0.tar", last modified: Tue May 21 10:18:24 2024, max compression
+gzip compressed data, was "testplans-0.3.1.tar", last modified: Tue May 21 12:58:16 2024, max compression
```

## Comparing `testplans-0.3.0.tar` & `testplans-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 10:18:24.825012 testplans-0.3.0/
--rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 testplans-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     5494 2024-05-21 10:18:24.824012 testplans-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4584 2024-05-21 10:17:28.000000 testplans-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-21 10:18:24.826015 testplans-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 10:18:24.816006 testplans-0.3.0/testplans/
--rw-rw-rw-   0        0        0      105 2024-02-01 12:13:36.000000 testplans-0.3.0/testplans/__init__.py
--rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.3.0/testplans/_results.py
--rw-rw-rw-   0        0        0     3974 2024-05-08 07:37:04.000000 testplans-0.3.0/testplans/api.py
--rw-rw-rw-   0        0        0     4071 2024-05-20 09:25:50.000000 testplans-0.3.0/testplans/devices.py
--rw-rw-rw-   0        0        0     6659 2024-05-16 15:49:07.000000 testplans-0.3.0/testplans/gui.py
--rw-rw-rw-   0        0        0    12440 2024-05-20 12:17:53.000000 testplans-0.3.0/testplans/main.py
--rw-rw-rw-   0        0        0     1786 2024-05-13 13:45:51.000000 testplans-0.3.0/testplans/models.py
--rw-rw-rw-   0        0        0    14015 2024-05-16 11:59:38.000000 testplans-0.3.0/testplans/tc.py
--rw-rw-rw-   0        0        0    10008 2024-05-21 10:09:16.000000 testplans-0.3.0/testplans/tm.py
-drwxrwxrwx   0        0        0        0 2024-05-21 10:18:24.824012 testplans-0.3.0/testplans.egg-info/
--rw-rw-rw-   0        0        0     5494 2024-05-21 10:18:24.000000 testplans-0.3.0/testplans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-21 10:18:24.000000 testplans-0.3.0/testplans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 10:18:24.000000 testplans-0.3.0/testplans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-21 10:18:24.000000 testplans-0.3.0/testplans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 12:58:16.006371 testplans-0.3.1/
+-rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 testplans-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     5494 2024-05-21 12:58:16.006371 testplans-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4584 2024-05-21 12:57:48.000000 testplans-0.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-21 12:58:16.007385 testplans-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:58:16.000370 testplans-0.3.1/testplans/
+-rw-rw-rw-   0        0        0      105 2024-02-01 12:13:36.000000 testplans-0.3.1/testplans/__init__.py
+-rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.3.1/testplans/_results.py
+-rw-rw-rw-   0        0        0     3974 2024-05-08 07:37:04.000000 testplans-0.3.1/testplans/api.py
+-rw-rw-rw-   0        0        0     4061 2024-05-21 12:55:18.000000 testplans-0.3.1/testplans/devices.py
+-rw-rw-rw-   0        0        0     6659 2024-05-16 15:49:07.000000 testplans-0.3.1/testplans/gui.py
+-rw-rw-rw-   0        0        0    12440 2024-05-21 12:55:18.000000 testplans-0.3.1/testplans/main.py
+-rw-rw-rw-   0        0        0     1786 2024-05-13 13:45:51.000000 testplans-0.3.1/testplans/models.py
+-rw-rw-rw-   0        0        0    14015 2024-05-21 12:55:18.000000 testplans-0.3.1/testplans/tc.py
+-rw-rw-rw-   0        0        0    10008 2024-05-21 10:09:16.000000 testplans-0.3.1/testplans/tm.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:58:16.005370 testplans-0.3.1/testplans.egg-info/
+-rw-rw-rw-   0        0        0     5494 2024-05-21 12:58:15.000000 testplans-0.3.1/testplans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-21 12:58:15.000000 testplans-0.3.1/testplans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 12:58:15.000000 testplans-0.3.1/testplans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-21 12:58:15.000000 testplans-0.3.1/testplans.egg-info/top_level.txt
```

### Comparing `testplans-0.3.0/LICENSE` & `testplans-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `testplans-0.3.0/PKG-INFO` & `testplans-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.3.0
+Version: 0.3.1
 Summary: simple testplan framework for several DUTs
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/testplans
 Keywords: testplan,testplan structure framework,testplan gui,testplan multy dut,testplan several dut
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# testplans (v0.3.0)
+# testplans (v0.3.1)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

### Comparing `testplans-0.3.0/README.md` & `testplans-0.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# testplans (v0.3.0)
+# testplans (v0.3.1)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

### Comparing `testplans-0.3.0/setup.py` & `testplans-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `testplans-0.3.0/testplans/_results.py` & `testplans-0.3.1/testplans/_results.py`

 * *Files identical despite different names*

### Comparing `testplans-0.3.0/testplans/api.py` & `testplans-0.3.1/testplans/api.py`

 * *Files identical despite different names*

### Comparing `testplans-0.3.0/testplans/devices.py` & `testplans-0.3.1/testplans/devices.py`

 * *Files 14% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         """
         this is only for testing purpose
         """
         self.SKIP = not bool(self.SKIP)
 
 
 # =====================================================================================================================
-class DevicesIndexed_Base(BreederObjectList):
+class DevicesBreeder(BreederObjectList):
     def __del__(self):
         self.disconnect__cls()
 
     @classmethod
     def connect__cls(cls) -> None:
         cls.group_call__("connect")
 
@@ -100,28 +100,28 @@
     # DEBUG PURPOSE ---------------------------------------------------------------------------------------------------
     @classmethod
     def _debug__duts__reset_sn(cls) -> None:
         cls.group_call__("_debug__reset_sn", "DUT")
 
 
 # =====================================================================================================================
-class DevicesIndexed_WithDut(DevicesIndexed_Base):
+class DevicesBreeder_WithDut(DevicesBreeder):
     """
     READY TO USE WITH DUT
     """
     # DEFINITIONS ---------------
     CLS_LIST__DUT: Type[DutBase] = DutBase
 
     # JUST SHOW NAMES -----------
     LIST__DUT: List[DutBase]
     DUT: DutBase
 
 
 # =====================================================================================================================
-class DevicesIndexed_Example(DevicesIndexed_WithDut):
+class DevicesBreeder_Example(DevicesBreeder_WithDut):
     """
     JUST an example DUT+some other single dev
     """
     # DEFINITIONS ---------------
     COUNT: int = 2
     CLS_SINGLE__ATC: Type[DeviceBase] = DeviceBase
```

### Comparing `testplans-0.3.0/testplans/gui.py` & `testplans-0.3.1/testplans/gui.py`

 * *Files identical despite different names*

### Comparing `testplans-0.3.0/testplans/main.py` & `testplans-0.3.1/testplans/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 THIS IS THE REAL TESTPLAN!!!
 """
 
 
 # =====================================================================================================================
 # from . import *
 from .tc import TestCaseBase
-from .devices import DutBase, DeviceBase, DevicesIndexed_WithDut, DevicesIndexed_Example
+from .devices import DutBase, DeviceBase, DevicesBreeder_WithDut, DevicesBreeder_Example
 from .gui import TpGuiBase
 from .api import TpApi_Aiohttp, TpApi_FastApi
 from .models import *
 
 from typing import *
 import json
 from pathlib import Path
@@ -71,15 +71,15 @@
 
     # DIRPATH_TPS: Union[str, Path] = "TESTPLANS"
     DIRPATH_TCS: Union[str, Path] = "TESTCASES"
     # DIRPATH_DEVS: Union[str, Path] = "DEVICES"
     SETTINGS_BASE_NAME: Union[str, Path] = "SETTINGS_BASE.json"
     SETTINGS_BASE_FILEPATH: Path
 
-    DEVICES__CLS: Type[DevicesIndexed_WithDut] = DevicesIndexed_Example
+    DEVICES__CLS: Type[DevicesBreeder_WithDut] = DevicesBreeder_Example
 
     # AUX -----------------------------------------------------------
     TCS__CLS: Dict[Union[str, Type[TestCaseBase]], Optional[bool]] = {}     # todo: RENAME TO clss!!!
     # {
     #     Tc1: True,
     #     Tc2: True
     # }
```

### Comparing `testplans-0.3.0/testplans/models.py` & `testplans-0.3.1/testplans/models.py`

 * *Files identical despite different names*

### Comparing `testplans-0.3.0/testplans/tc.py` & `testplans-0.3.1/testplans/tc.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 from enum import Enum, auto
 from PyQt5.QtCore import QThread
 
 from pyqt_templates import *
 from private_values import PrivateJson
 
-# from .devices import DevicesIndexed_WithDut
+# from .devices import DevicesBreeder_WithDut
 from .models import *
 
 from logger_aux import Logger
 from funcs_aux import ResultExpect_Base
 
 
 # =====================================================================================================================
@@ -49,16 +49,16 @@
     SETTINGS_FILES: Union[None, pathlib.Path, List[pathlib.Path]] = None
 
     # AUXILIARY -----------------------------------
     signals: Signals = Signals()  # FIXME: need signal ON BASE CLASS! need only one SlotConnection! need Singleton?
     TCS__INST: List['TestCaseBase'] = None
 
     # INSTANCE ------------------------------------
-    DEVICES__CLS: Type['DevicesIndexed_WithDut'] = None
-    DEVICES__BY_INDEX: 'DevicesIndexed_WithDut' = None
+    DEVICES__CLS: Type['DevicesBreeder_WithDut'] = None
+    DEVICES__BY_INDEX: 'DevicesBreeder_WithDut' = None
 
     SETTINGS: PrivateJson = None
     INDEX: int = 0
 
     result__cls_startup: Optional[bool] = None
     result__cls_teardown: Optional[bool] = None
     __result: Optional[bool]
@@ -82,15 +82,15 @@
 
         # if _settings_files is not None:
         #     self.SETTINGS_FILES = _settings_files
 
         self.SETTINGS = PrivateJson(_dict=self.settings_read())
 
     @classmethod
-    def devices__apply(cls, devices_cls: Type['DevicesIndexed_WithDut'] = None) -> None:
+    def devices__apply(cls, devices_cls: Type['DevicesBreeder_WithDut'] = None) -> None:
         if devices_cls is not None:
             cls.DEVICES__CLS = devices_cls
         if cls.DEVICES__CLS:
             cls._TCS__INST__generate()
 
     @classmethod
     def _TCS__INST__generate(cls) -> None:
```

### Comparing `testplans-0.3.0/testplans/tm.py` & `testplans-0.3.1/testplans/tm.py`

 * *Files identical despite different names*

### Comparing `testplans-0.3.0/testplans.egg-info/PKG-INFO` & `testplans-0.3.1/testplans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.3.0
+Version: 0.3.1
 Summary: simple testplan framework for several DUTs
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/testplans
 Keywords: testplan,testplan structure framework,testplan gui,testplan multy dut,testplan several dut
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# testplans (v0.3.0)
+# testplans (v0.3.1)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

