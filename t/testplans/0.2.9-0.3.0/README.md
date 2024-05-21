# Comparing `tmp/testplans-0.2.9.tar.gz` & `tmp/testplans-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testplans-0.2.9.tar", last modified: Wed May  8 10:45:20 2024, max compression
+gzip compressed data, was "testplans-0.3.0.tar", last modified: Tue May 21 10:18:24 2024, max compression
```

## Comparing `testplans-0.2.9.tar` & `testplans-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 10:45:20.597301 testplans-0.2.9/
--rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 testplans-0.2.9/LICENSE
--rw-rw-rw-   0        0        0     5494 2024-05-08 10:45:20.596800 testplans-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     4584 2024-05-08 10:43:50.000000 testplans-0.2.9/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 10:45:20.597301 testplans-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:45:20.591714 testplans-0.2.9/testplans/
--rw-rw-rw-   0        0        0      105 2024-02-01 12:13:36.000000 testplans-0.2.9/testplans/__init__.py
--rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.2.9/testplans/_results.py
--rw-rw-rw-   0        0        0     3974 2024-05-08 07:37:04.000000 testplans-0.2.9/testplans/api.py
--rw-rw-rw-   0        0        0     7686 2024-04-22 13:45:33.000000 testplans-0.2.9/testplans/devices.py
--rw-rw-rw-   0        0        0     6347 2024-04-22 14:33:47.000000 testplans-0.2.9/testplans/gui.py
--rw-rw-rw-   0        0        0    11898 2024-05-08 10:43:49.000000 testplans-0.2.9/testplans/main.py
--rw-rw-rw-   0        0        0     1561 2024-04-22 14:50:31.000000 testplans-0.2.9/testplans/models.py
--rw-rw-rw-   0        0        0    12340 2024-05-08 10:43:49.000000 testplans-0.2.9/testplans/tc.py
--rw-rw-rw-   0        0        0     8975 2024-04-26 12:19:02.000000 testplans-0.2.9/testplans/tm.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:45:20.595738 testplans-0.2.9/testplans.egg-info/
--rw-rw-rw-   0        0        0     5494 2024-05-08 10:45:20.000000 testplans-0.2.9/testplans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-08 10:45:20.000000 testplans-0.2.9/testplans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 10:45:20.000000 testplans-0.2.9/testplans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-08 10:45:20.000000 testplans-0.2.9/testplans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 10:18:24.825012 testplans-0.3.0/
+-rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 testplans-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     5494 2024-05-21 10:18:24.824012 testplans-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4584 2024-05-21 10:17:28.000000 testplans-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-21 10:18:24.826015 testplans-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 10:18:24.816006 testplans-0.3.0/testplans/
+-rw-rw-rw-   0        0        0      105 2024-02-01 12:13:36.000000 testplans-0.3.0/testplans/__init__.py
+-rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.3.0/testplans/_results.py
+-rw-rw-rw-   0        0        0     3974 2024-05-08 07:37:04.000000 testplans-0.3.0/testplans/api.py
+-rw-rw-rw-   0        0        0     4071 2024-05-20 09:25:50.000000 testplans-0.3.0/testplans/devices.py
+-rw-rw-rw-   0        0        0     6659 2024-05-16 15:49:07.000000 testplans-0.3.0/testplans/gui.py
+-rw-rw-rw-   0        0        0    12440 2024-05-20 12:17:53.000000 testplans-0.3.0/testplans/main.py
+-rw-rw-rw-   0        0        0     1786 2024-05-13 13:45:51.000000 testplans-0.3.0/testplans/models.py
+-rw-rw-rw-   0        0        0    14015 2024-05-16 11:59:38.000000 testplans-0.3.0/testplans/tc.py
+-rw-rw-rw-   0        0        0    10008 2024-05-21 10:09:16.000000 testplans-0.3.0/testplans/tm.py
+drwxrwxrwx   0        0        0        0 2024-05-21 10:18:24.824012 testplans-0.3.0/testplans.egg-info/
+-rw-rw-rw-   0        0        0     5494 2024-05-21 10:18:24.000000 testplans-0.3.0/testplans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-21 10:18:24.000000 testplans-0.3.0/testplans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 10:18:24.000000 testplans-0.3.0/testplans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-21 10:18:24.000000 testplans-0.3.0/testplans.egg-info/top_level.txt
```

### Comparing `testplans-0.2.9/LICENSE` & `testplans-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `testplans-0.2.9/PKG-INFO` & `testplans-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.2.9
+Version: 0.3.0
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
 
-# testplans (v0.2.9)
+# testplans (v0.3.0)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

### Comparing `testplans-0.2.9/README.md` & `testplans-0.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# testplans (v0.2.9)
+# testplans (v0.3.0)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

### Comparing `testplans-0.2.9/setup.py` & `testplans-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.9/testplans/_results.py` & `testplans-0.3.0/testplans/_results.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.9/testplans/api.py` & `testplans-0.3.0/testplans/api.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.9/testplans/gui.py` & `testplans-0.3.0/testplans/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,16 +126,22 @@
         # print(f"BTN_select_tc_on_duts__toggled {state=}")
         # self.TV.horizontalHeader().setSectionHidden(self.TM.ADDITIONAL_COLUMNS - 1, not state)
         self.TV.horizontalHeader().setSectionsClickable(state)
         self.TM.open__settings = state
         self.TM._data_reread()
 
     def TV_hh_sectionClicked(self, index: int) -> None:
-        if index > 1:
-            dut = self.DATA.DEVICES__CLS.LIST__DUT[index - self.TM.HEADERS.DUTS.START_OUTER]
+        if index == self.TM.HEADERS.STARTUP:
+            pass
+
+        if index == self.TM.HEADERS.TEARDOWN:
+            pass
+
+        if index in self.TM.HEADERS.DUTS:
+            dut = self.DATA.DEVICES__CLS.LIST__DUT[self.TM.HEADERS.DUTS.get_listed_index__by_outer(index)]
             dut._bebug__SKIP_reverse()
             self.TM._data_reread()
 
     def TV_selectionChanged(self, first: QItemSelection, last: QItemSelection) -> None:
         # print("selectionChanged")
         # print(f"{first=}")  # first=<PyQt5.QtCore.QItemSelection object at 0x000001C79A107460>
         # ObjectInfo(first.indexes()[0]).print(_log_iter=True, skip_fullnames=["takeFirst", "takeLast"])
@@ -145,18 +151,21 @@
             return
 
         index: QModelIndex = first.indexes()[0]
 
         row = index.row()
         col = index.column()
 
-        if col < self.TM.HEADERS.DUTS.START_OUTER:
-            return
-
         tc = list(self.DATA.TCS__CLS)[row]
-        dut = self.DATA.DEVICES__CLS.LIST__DUT[col - self.TM.HEADERS.DUTS.START_OUTER]
-        self.PTE.setPlainText(tc.TCS__INST[dut.INDEX].info_pretty())
 
-        # print(f"{row=}/{section=}/{dut=}/{tc=}")
+        if col == self.TM.HEADERS.STARTUP:
+            self.PTE.setPlainText(str(tc.result__cls_startup))
+
+        if col in self.TM.HEADERS.DUTS:
+            dut = self.DATA.DEVICES__CLS.LIST__DUT[col - self.TM.HEADERS.DUTS.START_OUTER]
+            self.PTE.setPlainText(tc.TCS__INST[dut.INDEX].info_pretty())
+
+        if col == self.TM.HEADERS.TEARDOWN:
+            self.PTE.setPlainText(str(tc.result__cls_teardown))
 
 
 # =====================================================================================================================
```

### Comparing `testplans-0.2.9/testplans/main.py` & `testplans-0.3.0/testplans/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# =====================================================================================================================
+"""
+THIS IS THE REAL TESTPLAN!!!
+"""
+
+
+# =====================================================================================================================
 # from . import *
 from .tc import TestCaseBase
 from .devices import DutBase, DeviceBase, DevicesIndexed_WithDut, DevicesIndexed_Example
 from .gui import TpGuiBase
 from .api import TpApi_Aiohttp, TpApi_FastApi
 from .models import *
 
@@ -94,15 +101,15 @@
         self.SETTINGS_BASE_FILEPATH = self.DIRPATH_TCS.joinpath(self.SETTINGS_BASE_NAME)
 
         if not self.DIRPATH_TCS.exists():
             msg = f"[ERROR] not found path {self.DIRPATH_TCS.name=}"
             print(msg)
             raise Exx__TcsPathNotExists(msg)
 
-        self.DEVICES__CLS.generate__devices()
+        self.DEVICES__CLS.generate__objects()
 
         self.tcs__reinit()
         self.slots_connect()
 
         if self.START__GUI_AND_API:
             self.start__gui_and_api()
 
@@ -240,39 +247,42 @@
             return
 
         if self.tp__startup():
             for step, tc in enumerate(self.TCS__CLS, start=1):
                 self.progress = int(step / len(self.TCS__CLS) * 100) - 1
                 self.tc_active = tc
                 tc.run__cls()
+                if not tc.result__cls_teardown:
+                    break
 
         # FINISH TP ---------------------------------------------------
         self.tp__teardown()
         self.LOGGER.debug("TP FINISH")
 
     # =================================================================================================================
-    def get__info__stand(self) -> ModelStand:
+    def get__info__stand(self) -> ModelStandInfo:
         result = {
-            "name": self.STAND_NAME,
-            "description": self.STAND_DESCRIPTION,
-            "sn": self.STAND_SN,
-            "settings": TestCaseBase.settings_read(files=self.SETTINGS_BASE_FILEPATH),
+            "STAND_NAME": self.STAND_NAME,
+            "STAND_DESCRIPTION": self.STAND_DESCRIPTION,
+            "STAND_SN": self.STAND_SN,
+            "STAND_SETTINGS": TestCaseBase.settings_read(files=self.SETTINGS_BASE_FILEPATH),
         }
-        return ModelStand(**result)
+        return ModelStandInfo(**result)
 
     def get__info(self) -> ModelTpInfo:
         """
         get info/structure about stand/TP
         """
         TP_TCS = []
         for tc in self.TCS__CLS:
             TP_TCS.append(tc.get__info())
 
         result = {
-            "STAND": self.get__info__stand(),
+            **self.get__info__stand().dict(),
+
             "TESTCASES": TP_TCS,
             # "TP_DUTS": [],      # TODO: decide how to use
             # [
             #     # [{DUT1}, {DUT2}, …]
             #     {
             #         DUT_ID: 1  # ??? 	# aux
             #         DUT_SKIP: False
@@ -285,27 +295,29 @@
     # -----------------------------------------------------------------------------------------------------------------
     def get__results(self) -> ModelTpResults:
         """
         get all results for stand/TP
         """
         TCS_RESULTS = []
         for tc in self.TCS__CLS:
-            TCS_RESULTS.append(tc.results_get_all())
+            TCS_RESULTS.append(tc.results__get_all())
 
         result = {
-            "STAND": self.get__info__stand(),
+            **self.get__info__stand().dict(),
             "TESTCASES": TCS_RESULTS,
             }
         return ModelTpResults(**result)
 
     # -----------------------------------------------------------------------------------------------------------------
     def post__tc_results(self, tc_inst: TestCaseBase) -> None:
-        if not self.api_client:
+        # CHECK ------------------------------------------
+        if not self.api_client or tc_inst.result is None:
             return
 
+        # WORK ------------------------------------------
         body = {
             "STAND_NAME": self.STAND_NAME,
             "STAND_DESCRIPTION": self.STAND_DESCRIPTION,
             **tc_inst.get__results().dict(),
         }
         self.api_client.send(body=body)
```

### Comparing `testplans-0.2.9/testplans/tc.py` & `testplans-0.3.0/testplans/tc.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,35 +7,40 @@
 from pyqt_templates import *
 from private_values import PrivateJson
 
 # from .devices import DevicesIndexed_WithDut
 from .models import *
 
 from logger_aux import Logger
+from funcs_aux import ResultExpect_Base
 
 
 # =====================================================================================================================
-class _TestCaseBase(Logger):
+TYPE__RESULT = Union[None, bool, ResultExpect_Base]
+
+
+# =====================================================================================================================
+class _TestCaseBase0(Logger):
     # just to use in Signals before defining exact
     pass
 
 
 # class Settings(PrivateJson):
 #     value1: int = 0
 #     value2: int
 
 
 # =====================================================================================================================
 class Signals(SignalsTemplate):
-    signal__tc_state_changed = pyqtSignal(_TestCaseBase)
+    signal__tc_state_changed = pyqtSignal(_TestCaseBase0)
 
 
 # =====================================================================================================================
-class TestCaseBase(_TestCaseBase, QThread):
-    LOG_ENABLE = True
+class _TestCaseBase(_TestCaseBase0, QThread):
+    LOG_ENABLE = False
     LOG_USE_FILE = False
 
     # SETTINGS ------------------------------------
     NAME: str = ""      # set auto!
     DESCRIPTION: str = ""
     SKIP: Optional[bool] = None     # access only over CLASS attribute! not instance!!!
     skip_tc_dut: Optional[bool] = None
@@ -51,15 +56,17 @@
     DEVICES__CLS: Type['DevicesIndexed_WithDut'] = None
     DEVICES__BY_INDEX: 'DevicesIndexed_WithDut' = None
 
     SETTINGS: PrivateJson = None
     INDEX: int = 0
 
     result__cls_startup: Optional[bool] = None
+    result__cls_teardown: Optional[bool] = None
     __result: Optional[bool]
+    __timestamp: float | None = None
     details: Dict[str, Any]
     exx: Optional[Exception]
     progress: int
 
     # =================================================================================================================
     # def __init__(self, dut: Any, _settings_files: Union[None, pathlib.Path, List[pathlib.Path]] = None):
     def __init__(self, index: int = 0):
@@ -102,14 +109,28 @@
     def DUT(self) -> Optional['DutBase']:
         """
         this is only for convenience!
         but recommended to use from DEVICES__BY_INDEX! - # TODO: solve it!!!
         """
         return self.DEVICES__BY_INDEX.DUT
 
+    @property
+    def timestamp(self) -> float | None:
+        """
+        None - not even started
+        float - was started!
+            stable - finished
+            UnStable - in progress (active thread)
+        """
+        if self.__timestamp:
+            return self.__timestamp
+
+        if self.isRunning():
+            return time.time()
+
     # =================================================================================================================
     @classmethod
     def settings_read(cls, files: Union[None, pathlib.Path, List[pathlib.Path]] = None) -> dict:
         result = {}
 
         _settings_files = files or cls.SETTINGS_FILES
         if _settings_files:
@@ -122,38 +143,40 @@
                         file_data = json.loads(file.read_text())
                         result.update(file_data)
         return result
 
     def clear(self) -> None:
         self.LOGGER.debug("clear")
 
+        self.__timestamp = None
         self.result = None
         self.details = {}
         self.exx = None
         self.progress = 0
 
     @classmethod
     def clear__cls(cls):
         cls.result__cls_startup = None
-        # for tc in cls.TCS__INST:
-        #     tc.clear()
+        cls.result__cls_teardown = None
+        for tc in cls.TCS__INST:
+            tc.clear()
 
     # @classmethod
     # @property
     # def NAME(cls):
     #     return cls.__name__
     #     # return pathlib.Path(__file__).name    # work as last destination where property starts!
 
     # RESULT ----------------------------------------------------------------------------------------------------------
     @property
-    def result(self) -> Optional[bool]:
+    def result(self) -> TYPE__RESULT:
         return self.__result
 
     @result.setter
-    def result(self, value: Optional[bool]) -> None:
+    def result(self, value: TYPE__RESULT) -> None:
         self.__result = value
         self.signals.signal__tc_state_changed.emit(self)
 
     # # ---------------------------------------------------------
     # @classmethod
     # @property
     # def result__cls_startup(cls) -> Optional[bool]:
@@ -169,97 +192,29 @@
     def details_update(self, details: Dict[str, Any]) -> None:
         self.LOGGER.debug("")
 
         self.details.update(details)
         # self.signals.signal__tc_state_changed.emit(self)
 
     # =================================================================================================================
-    def info_pretty(self) -> str:
-        self.LOGGER.debug("")
-
-        # fixme: ref from info_get
-        result = ""
-
-        result += f"NAME={self.NAME}\n"
-        result += f"DESCRIPTION={self.DESCRIPTION}\n"
-        result += f"SKIP={self.SKIP}\n"
-        result += f"skip_tc_dut={self.skip_tc_dut}\n"
-        result += f"ASYNC={self.ASYNC}\n"
-        result += f"INDEX={self.INDEX}\n"
-        result += f"result={self.result}\n"
-        result += f"progress={self.progress}\n"
-        result += f"exx={self.exx}\n"
-
-        result += f"SETTINGS=====================\n"
-        if self.SETTINGS:
-            for name, value in self.SETTINGS.dict.items():
-                result += f"{name}: {value}\n"
-
-        result += f"details=====================\n"
-        for name, value in self.details.items():
-            result += f"{name}: {value}\n"
-        return result
-
-    @classmethod
-    def get__info(cls) -> ModelTcClsInfo:
-        """
-        get info/structure about TcCls
-        """
-        result = {
-            "name": cls.NAME,
-            "description": cls.DESCRIPTION,
-            "is_async": cls.ASYNC,
-            "is_skipped": cls.SKIP,
-            "settings": cls.settings_read(),
-        }
-
-        return ModelTcClsInfo(**result)
-
-    # =================================================================================================================
-    def get__results(self) -> ModelTcInstResult:
-        self.LOGGER.debug("")
-
-        result = {
-            **self.get__info().dict(),
-
-            "DEVICE": self.DUT.get__info(),
-
-            # RESULTS
-            "is_active": self.isRunning(),
-            "is_async": self.ASYNC,
-            "is_skipped": self.SKIP,
-
-            "progress": self.progress,
-            "result": self.result,
-            "details": self.details,
-        }
-        return ModelTcInstResult(**result)
-
-    @classmethod
-    def results_get_all(cls) -> List[Dict[str, Any]]:
-        results = []
-        for tc_inst in cls.TCS__INST:
-            results.append(tc_inst.get__results().dict())
-        return results
-
-    # =================================================================================================================
     def terminate(self) -> None:
         self.LOGGER.debug("")
 
         super().terminate()
 
         progress = self.progress
         self.teardown()
         self.progress = progress
 
     @classmethod
     def terminate__cls(cls) -> None:
         for tc_inst in cls.TCS__INST:
             try:
-                tc_inst.terminate()
+                if tc_inst.isRunning() and not tc_inst.isFinished():
+                    tc_inst.terminate()
             except:
                 pass
 
         cls.teardown__cls()
 
     # =================================================================================================================
     def run(self) -> None:
@@ -271,15 +226,15 @@
             return
 
         # WORK --------
         self.LOGGER.debug("run-startup")
         if self.startup():
             try:
                 self.LOGGER.debug("run-run_wrapped START")
-                self.result = self.run_wrapped()
+                self.result = self.run__wrapped()
                 self.LOGGER.debug(f"run-run_wrapped FINISHED WITH {self.result=}")
             except Exception as exx:
                 self.exx = exx
         self.LOGGER.debug("run-teardown")
         self.teardown()
 
     @classmethod
@@ -292,21 +247,15 @@
 
         print(f"run__cls=START={cls.NAME=}={'='*50}")
         if cls.SKIP:
             print(f"run__cls=SKIP={cls.NAME=}={'='*50}")
             return
 
         # ---------------------------------
-        print(f"run__cls=clear__cls")
-        cls.clear__cls()
-
-        print(f"run__cls=startup__cls")
-        cls.result__cls_startup = cls.startup__cls()
-        print(f"run__cls={cls.result__cls_startup=}")
-        if cls.result__cls_startup:
+        if cls.startup__cls():
             # BATCH --------------------------
             for tc_inst in cls.TCS__INST:
                 if tc_inst.skip_tc_dut:
                     continue
 
                 print(f"run__cls=tc_inst.start({tc_inst.INDEX=})")
                 tc_inst.start()
@@ -317,45 +266,150 @@
             # WAIT --------------------------
             if cls.ASYNC:
                 for tc_inst in cls.TCS__INST:
                     print(f"run__cls=tc_inst.wait({tc_inst.INDEX=})inPARALLEL")
                     tc_inst.wait()
 
         # FINISH -------------------------------------------------
-        print(f"run__cls=teardown__cls")
         cls.teardown__cls()
         print(f"run__cls=FINISH={cls.NAME=}={'='*50}")
 
+    # STARTUP/TEARDOWN ------------------------------------------------------------------------------------------------
+    @classmethod
+    def startup__cls(cls) -> TYPE__RESULT:
+        """before batch work
+        """
+        print(f"startup__cls")
+        cls.clear__cls()
+
+        result = cls.startup__cls__wrapped()
+        print(f"result__cls_startup={result}")
+        cls.result__cls_startup = result
+        return result
+
+    def startup(self) -> TYPE__RESULT:
+        self.LOGGER.debug("")
+        self.progress = 1
+        return self.startup__wrapped()
+
+    def teardown(self) -> TYPE__RESULT:
+        self.LOGGER.debug("")
+        self.__timestamp = time.time()
+        self.progress = 99
+        result = self.teardown__wrapped()
+        self.progress = 100
+        return result
+
+    @classmethod
+    def teardown__cls(cls) -> TYPE__RESULT:
+        print(f"run__cls=teardown__cls")
+        result = cls.teardown__cls__wrapped()
+        if not result:
+            print(f"[FAIL] teardown__cls {cls.NAME}")
+
+        cls.result__cls_teardown = result
+        return result
+
     # REDEFINE ========================================================================================================
     pass
     pass
     pass
     pass
     pass
     pass
 
-    # STARTUP/TEARDOWN ------------------------------------------------------------------------------------------------
     @classmethod
-    def startup__cls(cls) -> bool:
-        """before batch work
-        """
+    def startup__cls__wrapped(cls) -> TYPE__RESULT:
         return True
 
-    def startup(self) -> bool:
-        self.LOGGER.debug("")
-        self.progress = 1
+    def startup__wrapped(cls) -> TYPE__RESULT:
+        return True
+
+    def run__wrapped(self) -> TYPE__RESULT:
+        return True
+
+    def teardown__wrapped(cls) -> TYPE__RESULT:
+        return True
+
+    @classmethod
+    def teardown__cls__wrapped(cls) -> TYPE__RESULT:
         return True
 
-    def teardown(self):
+
+# =====================================================================================================================
+class Info(_TestCaseBase):
+    """
+    separated class for gen results/info by models!
+    """
+    # =================================================================================================================
+    def info_pretty(self) -> str:
         self.LOGGER.debug("")
-        self.progress = 100
+
+        # fixme: ref from info_get
+        result = ""
+
+        result += f"DUT_INDEX={self.INDEX}\n"
+        result += f"TC_NAME={self.NAME}\n"
+        result += f"TC_DESCRIPTION={self.DESCRIPTION}\n"
+        result += f"TC_SKIP={self.SKIP}\n"
+        result += f"tc_skip_dut={self.skip_tc_dut}\n"
+        result += f"TC_ASYNC={self.ASYNC}\n"
+        result += f"tc_result={self.result}\n"
+        result += f"tc_progress={self.progress}\n"
+        result += f"tc_exx={self.exx}\n"
+
+        result += f"SETTINGS=====================\n"
+        if self.SETTINGS:
+            for name, value in self.SETTINGS.dict.items():
+                result += f"{name}: {value}\n"
+
+        result += f"details=====================\n"
+        for name, value in self.details.items():
+            result += f"{name}: {value}\n"
+        return result
 
     @classmethod
-    def teardown__cls(cls):
-        pass
+    def get__info(cls) -> ModelTcInfo:
+        """
+        get info/structure about TcCls
+        """
+        result = {
+            "TC_NAME": cls.NAME,
+            "TC_DESCRIPTION": cls.DESCRIPTION,
+            "TC_ASYNC": cls.ASYNC,
+            "TC_SKIP": cls.SKIP,
+            "TC_SETTINGS": cls.settings_read(),
+        }
+
+        return ModelTcInfo(**result)
+
+    # =================================================================================================================
+    def get__results(self) -> ModelTcResultFull:
+        self.LOGGER.debug("")
+
+        result = {
+            **self.get__info().dict(),
+            **self.DUT.get__info().dict(),
+
+            # RESULTS
+            "tc_timestamp": self.timestamp,
+            "tc_active": self.isRunning(),
+            "tc_progress": self.progress,
+            "tc_result": bool(self.result),
+            "tc_details": self.details,
+        }
+        return ModelTcResultFull(**result)
+
+    @classmethod
+    def results__get_all(cls) -> List[Dict[str, Any]]:
+        results = []
+        for tc_inst in cls.TCS__INST:
+            results.append(tc_inst.get__results().dict())
+        return results
+
 
-    # RUN -------------------------------------------------------------------------------------------------------------
-    def run_wrapped(self) -> bool:
-        pass
+class TestCaseBase(Info):
+    """
+    """
 
 
 # =====================================================================================================================
```

### Comparing `testplans-0.2.9/testplans/tm.py` & `testplans-0.3.0/testplans/tm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import *
 
 from PyQt5.QtCore import *
 from PyQt5.QtGui import *
 
 from pyqt_templates import TableModelTemplate
-from funcs_aux import NamesIndexed_Base, NamesIndexed_Templated
+from funcs_aux import BreederStrSeries, BreederStrStack, ResultExpect_Base
 
 # from .tp import TpMultyDutBase
 
 
 # =====================================================================================================================
 class TpTableModel(TableModelTemplate):
     DATA: "TpMultyDutBase"
@@ -16,19 +16,20 @@
 
     # AUX -------------------------------------------
     open__settings: Optional[bool] = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        class Headers(NamesIndexed_Base):
-            TESTCASE = 0
-            ASYNC = 1
-            STARTUP = 2
-            DUTS = NamesIndexed_Templated(3, self.DATA.DEVICES__CLS.COUNT)
+        class Headers(BreederStrStack):
+            TESTCASE: int = 0
+            ASYNC: None = None
+            STARTUP: None = None
+            DUTS: BreederStrSeries = BreederStrSeries(None, self.DATA.DEVICES__CLS.COUNT)
+            TEARDOWN: None = None
             # FIXME: need resolve COUNT over DevicesIndexed!!!
 
         self.HEADERS = Headers()
 
     def rowCount(self, parent: QModelIndex = None, *args, **kwargs) -> int:
         return len(self.DATA.TCS__CLS)
 
@@ -79,26 +80,33 @@
         # -------------------------------------------------------------------------------------------------------------
         if role == Qt.DisplayRole:
             if col == self.HEADERS.TESTCASE:
                 return f'{tc.NAME}\n{tc.DESCRIPTION}'
             if col == self.HEADERS.ASYNC:
                 return '+' if tc.ASYNC else '-'
             if col == self.HEADERS.STARTUP:
-                if tc.result__cls_startup is True:
+                if tc.result__cls_startup is None:
+                    return
+                elif bool(tc.result__cls_startup) is True:
                     return '+'
-                elif tc.result__cls_startup is False:
+                elif bool(tc.result__cls_startup) is False:
                     return '-'
-                else:
-                    return
             if col in self.HEADERS.DUTS:
                 if tc_inst:
                     if tc_inst.result is None:
                         return ""
                     else:
                         return f'{tc_inst.result}'
+            if col == self.HEADERS.TEARDOWN:
+                if tc.result__cls_teardown is None:
+                    return
+                elif bool(tc.result__cls_teardown) is True:
+                    return '+'
+                elif bool(tc.result__cls_teardown) is False:
+                    return '-'
 
         # -------------------------------------------------------------------------------------------------------------
         if role == Qt.TextAlignmentRole:
             """
             VARIANTS ALIGN
             --------------
             not exists NAME!!!} = 0         # (LEFT+TOP) [[[[[[[[DEFAULT IS [LEFT+TOP]]]]]]]]]
@@ -133,42 +141,55 @@
                 return QColor('#a2a2a2')
 
         # -------------------------------------------------------------------------------------------------------------
         if role == Qt.BackgroundColorRole:
             if tc.SKIP:
                 return QColor('#e2e2e2')
             if col == self.HEADERS.STARTUP:
-                if tc.result__cls_startup is True:
+                if tc.result__cls_startup is None:
+                    return
+                elif bool(tc.result__cls_startup) is True:
                     return QColor("#50FF50")
-                if tc.result__cls_startup is False:
+                elif bool(tc.result__cls_startup) is False:
                     return QColor("#FF5050")
             if col in self.HEADERS.DUTS:
                 if tc_inst.skip_tc_dut or not dut.connect() or dut.SKIP:
                     return QColor('#e2e2e2')
-                if tc_inst.result is True:
+                elif tc_inst.isRunning():
+                    return QColor("#FFFF50")
+                elif bool(tc_inst.result) is True:
                     return QColor("#00FF00")
-                if tc_inst.result is False:
+                elif bool(tc_inst.result) is False:
+                    if tc_inst.result is None:
+                        return
+                    else:
+                        return QColor("#FF5050")
+                # elif
+            if col == self.HEADERS.TEARDOWN:
+                if tc.result__cls_teardown is None:
+                    return
+                elif bool(tc.result__cls_teardown) is True:
+                    return QColor("#50FF50")
+                elif bool(tc.result__cls_teardown) is False:
                     return QColor("#FF5050")
-                if tc_inst.progress > 0:
-                    return QColor("#FFFF50")
 
         # -------------------------------------------------------------------------------------------------------------
         if role == Qt.CheckStateRole:
             if self.open__settings:
                 if col == self.HEADERS.TESTCASE:
                     if tc.SKIP:
                         return Qt.Unchecked
                     else:
                         return Qt.Checked
-                if col == self.HEADERS.ASYNC:
+                elif col == self.HEADERS.ASYNC:
                     if tc.ASYNC:
                         return Qt.Checked
                     else:
                         return Qt.Unchecked
-                if col in self.HEADERS.DUTS:
+                elif col in self.HEADERS.DUTS:
                     if not tc_inst.SKIP and not dut.SKIP:
                         if tc_inst.skip_tc_dut:
                             return Qt.Unchecked
                         else:
                             return Qt.Checked
 
         # -------------------------------------------------------------------------------------------------------------
```

### Comparing `testplans-0.2.9/testplans.egg-info/PKG-INFO` & `testplans-0.3.0/testplans.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.2.9
+Version: 0.3.0
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
 
-# testplans (v0.2.9)
+# testplans (v0.3.0)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

