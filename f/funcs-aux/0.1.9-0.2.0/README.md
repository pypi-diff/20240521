# Comparing `tmp/funcs_aux-0.1.9.tar.gz` & `tmp/funcs_aux-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs_aux-0.1.9.tar", last modified: Mon May 20 09:21:49 2024, max compression
+gzip compressed data, was "funcs_aux-0.2.0.tar", last modified: Tue May 21 10:03:17 2024, max compression
```

## Comparing `funcs_aux-0.1.9.tar` & `funcs_aux-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 09:21:49.707684 funcs_aux-0.1.9/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     1883 2024-05-20 09:21:49.707684 funcs_aux-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-05-20 09:19:27.000000 funcs_aux-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 09:21:49.701104 funcs_aux-0.1.9/funcs_aux/
--rw-rw-rw-   0        0        0      422 2024-05-17 14:27:50.000000 funcs_aux-0.1.9/funcs_aux/__init__.py
--rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.1.9/funcs_aux/arrays.py
--rw-rw-rw-   0        0        0     7187 2024-05-16 15:01:48.000000 funcs_aux-0.1.9/funcs_aux/breeder_names.py
--rw-rw-rw-   0        0        0     9034 2024-05-20 09:17:18.000000 funcs_aux-0.1.9/funcs_aux/breeder_objects.py
--rw-rw-rw-   0        0        0     5211 2024-03-22 14:19:18.000000 funcs_aux-0.1.9/funcs_aux/iterables.py
--rw-rw-rw-   0        0        0     9678 2024-05-17 09:54:30.000000 funcs_aux-0.1.9/funcs_aux/results.py
--rw-rw-rw-   0        0        0     1920 2024-03-01 08:45:13.000000 funcs_aux-0.1.9/funcs_aux/strings.py
-drwxrwxrwx   0        0        0        0 2024-05-20 09:21:49.707684 funcs_aux-0.1.9/funcs_aux.egg-info/
--rw-rw-rw-   0        0        0     1883 2024-05-20 09:21:49.000000 funcs_aux-0.1.9/funcs_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-05-20 09:21:49.000000 funcs_aux-0.1.9/funcs_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 09:21:49.000000 funcs_aux-0.1.9/funcs_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-20 09:21:49.000000 funcs_aux-0.1.9/funcs_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 09:21:49.709124 funcs_aux-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 10:03:17.027619 funcs_aux-0.2.0/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1883 2024-05-21 10:03:17.027120 funcs_aux-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-05-21 10:02:53.000000 funcs_aux-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 10:03:17.019652 funcs_aux-0.2.0/funcs_aux/
+-rw-rw-rw-   0        0        0      460 2024-05-21 07:34:52.000000 funcs_aux-0.2.0/funcs_aux/__init__.py
+-rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.2.0/funcs_aux/arrays.py
+-rw-rw-rw-   0        0        0     9034 2024-05-20 09:17:18.000000 funcs_aux-0.2.0/funcs_aux/breeder_objects.py
+-rw-rw-rw-   0        0        0     9791 2024-05-21 09:50:09.000000 funcs_aux-0.2.0/funcs_aux/breeder_str.py
+-rw-rw-rw-   0        0        0     5211 2024-03-22 14:19:18.000000 funcs_aux-0.2.0/funcs_aux/iterables.py
+-rw-rw-rw-   0        0        0     9678 2024-05-17 09:54:30.000000 funcs_aux-0.2.0/funcs_aux/results.py
+-rw-rw-rw-   0        0        0     1920 2024-03-01 08:45:13.000000 funcs_aux-0.2.0/funcs_aux/strings.py
+drwxrwxrwx   0        0        0        0 2024-05-21 10:03:17.026076 funcs_aux-0.2.0/funcs_aux.egg-info/
+-rw-rw-rw-   0        0        0     1883 2024-05-21 10:03:16.000000 funcs_aux-0.2.0/funcs_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-21 10:03:16.000000 funcs_aux-0.2.0/funcs_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 10:03:16.000000 funcs_aux-0.2.0/funcs_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-21 10:03:16.000000 funcs_aux-0.2.0/funcs_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 10:03:17.028480 funcs_aux-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.2.0/setup.py
```

### Comparing `funcs_aux-0.1.9/LICENSE` & `funcs_aux-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.9/PKG-INFO` & `funcs_aux-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.1.9
+Version: 0.2.0
 Summary: useful funcs in one place
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/funcs_aux
 Keywords: functions,auxiliary,auxiliary funcs,np funcs,collections funcs,strings funcs,result object
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# funcs_aux (v0.1.9)
+# funcs_aux (v0.2.0)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.1.9/README.md` & `funcs_aux-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# funcs_aux (v0.1.9)
+# funcs_aux (v0.2.0)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.1.9/funcs_aux/arrays.py` & `funcs_aux-0.2.0/funcs_aux/arrays.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.9/funcs_aux/breeder_names.py` & `funcs_aux-0.2.0/funcs_aux/breeder_str.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,31 +13,44 @@
 class Exx__ItemNotExists(Exception):
     """
     not exists INDEX (out of range) or NAME not in defined values
     """
     pass
 
 
+class Exx__StartOuterNONE_UsedInStackByRecreation(Exception):
+    """
+    in stack it will be recreate automatically! so dont use in pure single BreederStrSeries!
+    """
+    pass
+
+
 # =====================================================================================================================
-class NamesIndexed_Templated(NamedTuple):
+class BreederStrSeries(NamedTuple):
     """
     PATTERN FOR BREEDING ONE TYPE OF TEMPLATE STYLE
-    used and created special for NamesIndexed_Base
+    used and created special for BreederStrStack
     """
-    START_OUTER: int
+    START_OUTER: int | None  # None used only for recreation in Stack!!! for auto
     COUNT: int
     TEMPLATE: str = "%s"
     START_INNER: int = 1    # just a starting number in values!
 
-    def __contains__(self, item: Union[int, str]) -> bool:
+    def _raise_if_start_outer_none(self) -> NoReturn | None:
+        if self.START_OUTER is None:
+            raise Exx__StartOuterNONE_UsedInStackByRecreation()
+
+    def __contains__(self, item: Union[int, str]) -> Union[bool, NoReturn]:
         """
         :param item: one of: 1=OUTER_INDEX (not self-INNER!!!) or 2=ORIGINAL value_NAME
             couse of we usually need to compare OUTER indexes or original VALUES!
         :return:
         """
+        self._raise_if_start_outer_none()
+
         if isinstance(item, int):
             return self.START_OUTER <= item < (self.START_OUTER + self.COUNT)
 
         elif isinstance(item, str):
             return item in self.get_dict__outer().values()
 
     def __getitem__(self, item: Union[int, str]) -> Union[int, str, NoReturn]:
@@ -55,25 +68,29 @@
             for key, value in _DATA.items():
                 if item == value:
                     return key
 
         msg = f"{item=}"
         raise Exx__ItemNotExists(msg)
 
-    def get_dict__outer(self) -> Dict[int, str]:
+    def get_dict__outer(self) -> Dict[int, str] | NoReturn:
+        self._raise_if_start_outer_none()
+
         result_outer_sub = {}
         for index in range(self.COUNT):
             pos = index + self.START_INNER
             value = self.TEMPLATE % pos
 
             index_outer = index + self.START_OUTER
             result_outer_sub.update({index_outer: value})
         return result_outer_sub
 
-    def get_dict__inner(self) -> Dict[int, str]:
+    def get_dict__inner(self) -> Dict[int, str] | NoReturn:
+        self._raise_if_start_outer_none()
+
         result_inner = {}
         for index in range(self.COUNT):
             pos = index + self.START_INNER
             value = self.TEMPLATE % pos
 
             result_inner.update({pos: value})
         return result_inner
@@ -104,88 +121,125 @@
                 else:
                     result += 1
         else:
             raise Exx__ItemNotExists()
 
 
 # =====================================================================================================================
-class NamesIndexed_Base:
+class BreederStrStack:
     """
     created specially for applying in Gui tableModels (PyQt5) as header structure
 
     VULNERABILITIES # FIXME:
     ------------------------
     1. if exists same names cause of patterns - it would return always first index!
-        class NamesIndexed_Example2(NamesIndexed_Base):
-            TAIL = NamesIndexed_Templated(2, 2, "%s")
-            TAIL2 = NamesIndexed_Templated(4, 2, "%s")
+        class BreederStrStack_Example2(BreederStrStack):
+            TAIL = BreederStrSeries(2, 2, "%s")
+            TAIL2 = BreederStrSeries(4, 2, "%s")
 
-        NamesIndexed_Example2()["2"] = 1
+        BreederStrStack_Example2()["2"] = 1
 
     DEFINE
     ------
     !. names (as attributes)
         - dont use underscore as first simble
         - it will be as value for index
     1. dont keep SKIPPED indexes - use all final range!
-    2. NamesIndexed_Templated
+    2. BreederStrSeries
      - use if need template for some range
      - use any count of such items
 
     USAGE
     -----
     1. COMPARE BY INDEXES OVER NAME
     if colIndex == MyHeders.attr0:
         pass
 
     2. GET HEADER NAME BY INDEX or INDEX by NAME!
     headerName = MyHeders[colIndex]
     headerIndex = MyHeders[colName]
+
+    RULES
+    -----
+    1. use always any ANNOTATIONS for your indexes!!
+    2. hide names by using underscore!
+    3. use None for AUTOINDEX!!!
+    4. nesting available with correct order!
+        class ClsFirst(BreederStrStack):
+            atr1: int
+            atr3: int = None
+
+        class ClsLast(BreederStrStack):
+            atr2: int = None
+            atr4: int
+
+        for key, value in ClsLast.annotations__get_nested_list().items():
+            print(f"{key}:{value}")
+
+        # atr1:<class 'int'>
+        # atr3:<class 'int'>
+        # atr2:<class 'int'>
+        # atr4:<class 'int'>
     """
-    _DATA: Dict[int, str] = {}
+    # settings ----------------------
+    _RAISE_IF_INDEX_SKIPPED: bool = True
+
+    # aux ----------------------
+    _DATA: dict[int, str] = {}
 
     def __init__(self):
+        index_last = 0
         result = {}
 
         # ATTRS ------------------
         attrs: List[str] = []
-        for attr in dir(self):
+        for attr in self.annotations__get_nested():
             if not attr.startswith("_") and not callable(getattr(self, attr)):
                 attrs.append(attr)
 
         # WORK -------------------
-        for value in attrs:
-            index = getattr(self, value)
+        for attr in attrs:
+            index = getattr(self, attr)
+
+            # apply AUTO ----------
+            if index is None:
+                index = index_last + 1
+                index_last = index
+                setattr(self, attr, index)
+
+            # work INT ----------
             if isinstance(index, int):
                 if index in result:
                     msg = f"{index=} from {result=}"
                     raise Exx__IndexOverlayed(msg)
-                result.update({index: value})
-            elif isinstance(index, NamesIndexed_Templated):
-                result_sub = index.get_dict__outer()
-                for index in result_sub:
-                    if index in result:
-                        msg = f"{index=} from {result_sub=}"
-                        raise Exx__IndexOverlayed(msg)
-                result.update(result_sub)
-
-        # CHECK SKIPPED -----------
-        index_prev = None
-        for index in sorted(result):
-            if index_prev is None:
-                index_prev = index
-                continue
+                result.update({index: attr})
+                index_last = index
 
-            if index - index_prev != 1:
-                msg = f"index [{index-1}]"
-                raise Exx__IndexNotSet(msg)
-            index_prev = index
+            # work BreederStrSeries ----------
+            if isinstance(index, BreederStrSeries):
+                # apply AUTO by recreation
+                if index.START_OUTER is None:
+                    index = BreederStrSeries(index_last + 1, index.COUNT, index.TEMPLATE, index.START_INNER)
+                    setattr(self, attr, index)
+
+                # work
+                result_sub_dict = index.get_dict__outer()
+                for key, value in result_sub_dict.items():
+                    if key in result:
+                        msg = f"{key=} from {result_sub_dict=}"
+                        raise Exx__IndexOverlayed(msg)
+                    result.update({key: value})
+                    index_last = key
 
         # RESULT -------------------
-        self._DATA = result
+        self._DATA = dict(sorted(result.items()))
+
+        # CHECK SKIPPED -----------
+        if self._RAISE_IF_INDEX_SKIPPED:
+            self.raise_if_index_skipped()
 
     def __getitem__(self, item: Union[int, str]) -> Union[int, str]:
         if item in self._DATA:
             return self._DATA[item]
 
         if item in self._DATA.values():
             for name, value in self._DATA.items():
@@ -201,24 +255,50 @@
         :return:
         """
         return item in self._DATA or item in self._DATA.values()
 
     def count(self) -> int:
         return len(self._DATA)
 
+    @classmethod
+    def raise_if_index_skipped(cls) -> None | NoReturn:
+        index_prev = None
+        for index in cls._DATA:
+            if index_prev is None:
+                index_prev = index
+                continue
+
+            if index - index_prev != 1:
+                msg = f"index [{index-1}]"
+                raise Exx__IndexNotSet(msg)
+            index_prev = index
+
+    @classmethod
+    def annotations__get_nested(cls) -> dict[str, Any]:
+        """
+        get all annotations in correct order!
+        """
+        result = {}
+        for cls_i in cls.__mro__:
+            if cls_i == BreederStrStack:
+                break
+
+            result = dict(**cls_i.__annotations__, **result)
+        return result
+
 
 # =====================================================================================================================
-class NamesIndexed_Example(NamesIndexed_Base):
-    name0 = 0
-    name1 = 1
-    TAIL = NamesIndexed_Templated(2, 2, "%s")
+class BreederStrStack_Example(BreederStrStack):
+    name0: int = 0
+    name1: int = 1
+    TAIL: BreederStrSeries = BreederStrSeries(2, 2, "%s")
 
 
-class NamesIndexed_Example__BestUsage(NamesIndexed_Base):
-    INDEX = 0
-    TESTCASE = 1
-    ASYNC = 2
-    STARTUP = 3
-    DUTS = NamesIndexed_Templated(4, 10, "TC_DUT_%s")
+class BreederStrStack_Example__BestUsage(BreederStrStack):
+    INDEX: int = 0
+    TESTCASE: int = None
+    ASYNC: int = None
+    STARTUP: int = None
+    DUTS: BreederStrSeries = BreederStrSeries(None, 10, "TC_DUT_%s")
 
 
 # =====================================================================================================================
```

### Comparing `funcs_aux-0.1.9/funcs_aux/breeder_objects.py` & `funcs_aux-0.2.0/funcs_aux/breeder_objects.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.9/funcs_aux/iterables.py` & `funcs_aux-0.2.0/funcs_aux/iterables.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.9/funcs_aux/results.py` & `funcs_aux-0.2.0/funcs_aux/results.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.9/funcs_aux/strings.py` & `funcs_aux-0.2.0/funcs_aux/strings.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.9/funcs_aux.egg-info/PKG-INFO` & `funcs_aux-0.2.0/funcs_aux.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.1.9
+Version: 0.2.0
 Summary: useful funcs in one place
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/funcs_aux
 Keywords: functions,auxiliary,auxiliary funcs,np funcs,collections funcs,strings funcs,result object
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# funcs_aux (v0.1.9)
+# funcs_aux (v0.2.0)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.1.9/setup.py` & `funcs_aux-0.2.0/setup.py`

 * *Files identical despite different names*

