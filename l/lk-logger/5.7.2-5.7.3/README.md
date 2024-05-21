# Comparing `tmp/lk_logger-5.7.2-py3-none-any.whl.zip` & `tmp/lk_logger-5.7.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,30 +1,30 @@
-Zip file size: 44917 bytes, number of entries: 28
+Zip file size: 45114 bytes, number of entries: 28
 -rw-r--r--  2.0 fat      955 b- defN 80-Jan-01 00:00 lk_logger/__init__.py
 -rw-r--r--  2.0 fat       34 b- defN 80-Jan-01 00:00 lk_logger/cache/__init__.py
 -rw-r--r--  2.0 fat     6970 b- defN 80-Jan-01 00:00 lk_logger/cache/cache.py
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 lk_logger/cache/frame.py
 -rw-r--r--  2.0 fat     1875 b- defN 80-Jan-01 00:00 lk_logger/cache/legacy.py
 -rw-r--r--  2.0 fat      762 b- defN 80-Jan-01 00:00 lk_logger/cache/util.py
 -rw-r--r--  2.0 fat     5668 b- defN 80-Jan-01 00:00 lk_logger/config.py
--rw-r--r--  2.0 fat     1230 b- defN 80-Jan-01 00:00 lk_logger/console.py
+-rw-r--r--  2.0 fat     1432 b- defN 80-Jan-01 00:00 lk_logger/console.py
 -rw-r--r--  2.0 fat     4815 b- defN 80-Jan-01 00:00 lk_logger/control.py
 -rw-r--r--  2.0 fat     8737 b- defN 80-Jan-01 00:00 lk_logger/frame_info.py
 -rw-r--r--  2.0 fat    14614 b- defN 80-Jan-01 00:00 lk_logger/logger.py
 -rw-r--r--  2.0 fat    10730 b- defN 80-Jan-01 00:00 lk_logger/markup.py
 -rw-r--r--  2.0 fat    11636 b- defN 80-Jan-01 00:00 lk_logger/message_builder.py
 -rw-r--r--  2.0 fat    13323 b- defN 80-Jan-01 00:00 lk_logger/message_formatter.py
--rw-r--r--  2.0 fat     4034 b- defN 80-Jan-01 00:00 lk_logger/path_helper.py
+-rw-r--r--  2.0 fat     4068 b- defN 80-Jan-01 00:00 lk_logger/path_helper.py
 -rw-r--r--  2.0 fat     2453 b- defN 80-Jan-01 00:00 lk_logger/pipeline.py
--rw-r--r--  2.0 fat     2590 b- defN 80-Jan-01 00:00 lk_logger/printer.py
+-rw-r--r--  2.0 fat     2930 b- defN 80-Jan-01 00:00 lk_logger/printer.py
 -rw-r--r--  2.0 fat       73 b- defN 80-Jan-01 00:00 lk_logger/scanner/__init__.py
 -rw-r--r--  2.0 fat     6407 b- defN 80-Jan-01 00:00 lk_logger/scanner/analyser.py
 -rw-r--r--  2.0 fat     1164 b- defN 80-Jan-01 00:00 lk_logger/scanner/const.py
 -rw-r--r--  2.0 fat     1780 b- defN 80-Jan-01 00:00 lk_logger/scanner/exceptions.py
 -rw-r--r--  2.0 fat     9728 b- defN 80-Jan-01 00:00 lk_logger/scanner/scanner.py
 -rw-r--r--  2.0 fat     3306 b- defN 80-Jan-01 00:00 lk_logger/scanner/symbols.py
 -rw-r--r--  2.0 fat    19638 b- defN 80-Jan-01 00:00 lk_logger/scanner/text_scanner.py
 -rw-r--r--  2.0 fat      517 b- defN 80-Jan-01 00:00 lk_logger/scanner/typehint.py
--rw-r--r--  2.0 fat    10805 b- defN 80-Jan-01 00:00 lk_logger-5.7.2.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 lk_logger-5.7.2.dist-info/WHEEL
-?rw-r--r--  2.0 fat     2253 b- defN 16-Jan-01 00:00 lk_logger-5.7.2.dist-info/RECORD
-28 files, 146185 bytes uncompressed, 41333 bytes compressed:  71.7%
+-rw-r--r--  2.0 fat    10805 b- defN 80-Jan-01 00:00 lk_logger-5.7.3.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 lk_logger-5.7.3.dist-info/WHEEL
+?rw-r--r--  2.0 fat     2253 b- defN 16-Jan-01 00:00 lk_logger-5.7.3.dist-info/RECORD
+28 files, 146761 bytes uncompressed, 41530 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -69,17 +69,17 @@
 
 Filename: lk_logger/scanner/text_scanner.py
 Comment: 
 
 Filename: lk_logger/scanner/typehint.py
 Comment: 
 
-Filename: lk_logger-5.7.2.dist-info/METADATA
+Filename: lk_logger-5.7.3.dist-info/METADATA
 Comment: 
 
-Filename: lk_logger-5.7.2.dist-info/WHEEL
+Filename: lk_logger-5.7.3.dist-info/WHEEL
 Comment: 
 
-Filename: lk_logger-5.7.2.dist-info/RECORD
+Filename: lk_logger-5.7.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lk_logger/__init__.py

```diff
@@ -30,8 +30,8 @@
     else:
         import IPython
         pipeline.add(IPython, bprint, scope=True)
         # pipeline.add('[ipython]', bprint)
 
 
 __init()
-__version__ = '5.7.2'
+__version__ = '5.7.3'
```

## lk_logger/console.py

```diff
@@ -18,16 +18,22 @@
                 self._color_system = 'standard'
         
         # TODO (width):
         #   if width longer than default, use single line style; otherwise
         #   split sourcemap and message into different lines.
         pass
     
-    def print(self, *objects: Any, soft_wrap: bool = True, **kwargs) -> None:
+    def print(
+        self, *objects: Any, soft_wrap: bool = True, **kwargs
+    ) -> None:
         from .message_builder import MessageStruct
+        # pop incompatible arguments
+        # bg: streamlit passes `file` to `sys.stdout` which causes an error here.
+        kwargs.pop('file', None)
+        # kwargs.pop('flush', None)
         if len(objects) == 1 and isinstance(objects[0], MessageStruct):
             super().print(
                 objects[0].text, overflow='fold', soft_wrap=soft_wrap, **kwargs
             )
         else:
             super().print(
                 *objects, overflow='fold', soft_wrap=soft_wrap, **kwargs
```

## lk_logger/path_helper.py

```diff
@@ -1,22 +1,21 @@
-from __future__ import annotations
-
 import os
 import sys
+import typing as t
 
 
 def normpath(path: str) -> str:
     return path.replace('\\', '/').rstrip('/')
 
 
 class PathHelper:
     __project_root: str
-    __external_libs: dict[str, str] | None
+    __external_libs: t.Dict[str, str] | None
     
-    def __init__(self):
+    def __init__(self) -> None:
         self._cwd = os.getcwd()
         self.__project_root = self._find_project_root()
         self.__external_libs = None
     
     @staticmethod
     def _find_project_root() -> str:
         """ find personal-like project root.
@@ -26,38 +25,39 @@
                one of '.idea', '.git', etc. folders.
             2. iterate paths in sys.path, to find a folder which is parent of
                current working dir. (adopted)
                if there are more than one, choose which is shortest.
                if there is none, return current working dir.
         """
         cwd = normpath(os.getcwd())
+        # noinspection PyTypeChecker
         paths = tuple(
             x for x in map(normpath, map(os.path.abspath, sys.path))
             if cwd.startswith(x) and os.path.isdir(x)
         )
         if len(paths) == 0:
             return cwd
         elif len(paths) == 1:
             return paths[0]
         else:
             return min(paths, key=lambda x: len(x))
     
     # -------------------------------------------------------------------------
     
     @property
-    def external_libs(self) -> dict[str, str]:
+    def external_libs(self) -> t.Dict[str, str]:
         if self.__external_libs is None:
             self.__external_libs = self._indexing_external_libs()
         return self.__external_libs
     
     def is_external_lib(self, filepath: str) -> bool:
         return not filepath.startswith(self.__project_root)
     
     @staticmethod
-    def _indexing_external_libs() -> dict[str, str]:
+    def _indexing_external_libs() -> t.Dict[str, str]:
         """
         return:
             dict[str path, str lib_name]
         """
         out = {}
         
         for path in reversed(sys.path):
```

## lk_logger/printer.py

```diff
@@ -43,22 +43,31 @@
 class T:
     Printer = t.Union[BasePrinter, t.Callable[[str], None]]
     Printers = t.Tuple[Printer, ...]
 
 
 class PrinterManager:
     _group: t.List[T.Printers]
+    _is_under_iterating: bool
     
     def __init__(self) -> None:
+        # self.is_scoping = False
         # self._group = [(std_print,)]
         self._group = [()]
+        self._is_under_iterating = False
     
     @property
-    def printers(self) -> T.Printers:
-        return self._group[-1]
+    def printers(self) -> t.Iterator[T.Printer]:
+        # prevent recursive call
+        if self._is_under_iterating:
+            # dprint('under iteration')
+            return ()
+        self._is_under_iterating = True
+        yield from self._group[-1]
+        self._is_under_iterating = False
     
     def add_group(self, printers: T.Printers) -> None:
         self._group.append(printers)
         
     def pop_group(self) -> None:
         self._group.pop()
 
@@ -78,15 +87,15 @@
                         print('bbb')  # p1, p2, p3 called
                     with parallel_printing(p4, inherit=False):
                         print('ccc')  # p4 called
                         with parallel_printing(p5):
                             print('ddd')  # p4, p5 called
     """
     if inherit:
-        printers = printer_manager.printers + printers
+        printers = tuple(printer_manager.printers) + printers
     printer_manager.add_group(printers)
     yield
     printer_manager.pop_group()
 
 
 # -----------------------------------------------------------------------------
 # general
```

## Comparing `lk_logger-5.7.2.dist-info/METADATA` & `lk_logger-5.7.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lk-logger
-Version: 5.7.2
+Version: 5.7.3
 Summary: Python print with source and varnames.
 Home-page: https://github.com/likianta/lk-logger
 License: MIT
 Author: Likianta
 Author-email: likianta@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `lk_logger-5.7.2.dist-info/RECORD` & `lk_logger-5.7.3.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-lk_logger/__init__.py,sha256=U-1ZwuMdW3XFAtS5nSpnZmh4rO97dPgOuSShvcB3jds,955
+lk_logger/__init__.py,sha256=H-RBh2k0tdIU6J9DeO5l2qqufsvutVML4j0fBUknd6I,955
 lk_logger/cache/__init__.py,sha256=jkWi40WfmTt3Akv3YKjJHI6gxPqzXwpFmdF4bIJ-SUs,34
 lk_logger/cache/cache.py,sha256=b2zusDBHjbAVtoP8CdBedPvkujVjNosUNlsUiCPSJeY,6970
 lk_logger/cache/frame.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lk_logger/cache/legacy.py,sha256=kuQrFzJGuTd_NQWrO5Vp6b-Da3X73w60Ae2LxVP3Xb8,1875
 lk_logger/cache/util.py,sha256=6qtnnIhdrKTqyP4Elxd1d3OnkTFROzxAGWYz3c4smDk,762
 lk_logger/config.py,sha256=A2773dLIzjvBtvP9ozDzLF7Z3Vie8VfJQBRcg6ZQzRE,5668
-lk_logger/console.py,sha256=TmWt2SC2UO1en0M_tzlQPd2PuI4FoV1PGkeKrnxd6_c,1230
+lk_logger/console.py,sha256=mreY_6vY56kU0lISyCUoxn5Gq1Ez1oswtdJHKHBd6xI,1432
 lk_logger/control.py,sha256=-372tzbaB9cwPkj2YtDwnOA0avDHysRuu-x_SzNvB68,4815
 lk_logger/frame_info.py,sha256=NcKF6CZLRBB_SfEOLsj7SMR6X27w362t6WhBkpmWxBo,8737
 lk_logger/logger.py,sha256=bXDlcv_sc_ra7qulZNjJ25e94UznVX4hZFBoOCZn4SQ,14614
 lk_logger/markup.py,sha256=mahzUkl-8iED1iNEOjsbm_0h2xs5xRew2oRGPZqvYzo,10730
 lk_logger/message_builder.py,sha256=HNQdiio1oYL-z7bKcX8Pv8sa9oH0m_yOlQ_qIcycsMk,11636
 lk_logger/message_formatter.py,sha256=GxFNcHCWxXsHcnF7O_FNjg14etQRw9AHsAuiMXstF3I,13323
-lk_logger/path_helper.py,sha256=LAZOe5XK_51I0YPA6rUuY0_DKtaMtHyz52xcHqRbxY0,4034
+lk_logger/path_helper.py,sha256=yLghN3s8tbQZqW6w1rt7k866VRRtwdKmfS9CB04TDtQ,4068
 lk_logger/pipeline.py,sha256=dS5_RynnCaxDTM65bxb8YT1fPAyFeH8vzpt8UATmb_o,2453
-lk_logger/printer.py,sha256=O_IFHHKfKdiu-SALeZ2H_maIC0aDwMvM3248ihEUJ68,2590
+lk_logger/printer.py,sha256=jGWPD2KoZjMra27T7DJqMArtJ4xgQ395WPyUfkY-brc,2930
 lk_logger/scanner/__init__.py,sha256=2b0jy5SdPwiVQSV9kL_3Vd4AkbKrRp7npAUWC3Hbyek,73
 lk_logger/scanner/analyser.py,sha256=y3HuYB2DJ4ixwww4c9o6Jq6mPc2eqz88w5Cf84_Pf6E,6407
 lk_logger/scanner/const.py,sha256=npj77J2VntzHArQOaIUIj9IeRQi9hH33_lo2XYLlg-s,1164
 lk_logger/scanner/exceptions.py,sha256=G1wpgEIzTLLrD6Q_m0qGD85v5KnlPm3CV1ZxgvGCVd8,1780
 lk_logger/scanner/scanner.py,sha256=I9tf-ELQOLgZxWM5YNCEP5FvW5JkmIhfVEdhezXGz4M,9728
 lk_logger/scanner/symbols.py,sha256=FhLqVbYRG-a72ZoVgriP4FKmAhweyeyh02IkiLymT2I,3306
 lk_logger/scanner/text_scanner.py,sha256=84ese30Bh-H1ZVxT0jcNhsTwM1nLDkZOrUO1LSdjV6k,19638
 lk_logger/scanner/typehint.py,sha256=CdX-02JvaI8PkEHgTN279e081njEAfNOHaxPXCQkguc,517
-lk_logger-5.7.2.dist-info/METADATA,sha256=kU4rA6MBo9-TeAUJaBP1S2MaxQnEw8z_epUXV6wDUf8,10805
-lk_logger-5.7.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-lk_logger-5.7.2.dist-info/RECORD,,
+lk_logger-5.7.3.dist-info/METADATA,sha256=bpVG_aPJKJEnuiv1lV21WE0GpTTCR22cCNoGbjlyDzo,10805
+lk_logger-5.7.3.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+lk_logger-5.7.3.dist-info/RECORD,,
```

