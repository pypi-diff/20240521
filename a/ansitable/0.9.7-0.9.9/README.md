# Comparing `tmp/ansitable-0.9.7.tar.gz` & `tmp/ansitable-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/corkep/Dropbox/code/ansitable/dist/tmpnj46ybcf/ansitable-0.9.7.tar", last modified: Thu Oct  6 23:46:20 2022, max compression
+gzip compressed data, was "ansitable-0.9.9.tar", last modified: Thu Oct 19 01:33:09 2023, max compression
```

## Comparing `ansitable-0.9.7.tar` & `ansitable-0.9.9.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwx---   0 corkep     (503) staff       (20)        0 2022-10-06 23:46:20.615333 ansitable-0.9.7/
--rw-rw----   0 corkep     (503) staff       (20)     1068 2020-09-26 22:42:59.000000 ansitable-0.9.7/LICENSE
--rw-r-----   0 corkep     (503) staff       (20)       71 2020-10-11 07:17:31.000000 ansitable-0.9.7/MANIFEST.in
--rw-rw----   0 corkep     (503) staff       (20)    17339 2022-10-06 23:46:20.615017 ansitable-0.9.7/PKG-INFO
--rw-r--r--   0 corkep     (503) staff       (20)    16565 2021-03-21 02:05:54.000000 ansitable-0.9.7/README.md
--rw-r--r--   0 corkep     (503) staff       (20)        6 2022-10-06 23:39:05.000000 ansitable-0.9.7/RELEASE
-drwxrwx---   0 corkep     (503) staff       (20)        0 2022-10-06 23:46:20.613468 ansitable-0.9.7/ansitable/
--rw-rw----   0 corkep     (503) staff       (20)      132 2021-11-29 19:39:00.000000 ansitable-0.9.7/ansitable/__init__.py
--rw-r--r--   0 corkep     (503) staff       (20)    28260 2021-12-07 03:21:33.000000 ansitable-0.9.7/ansitable/table.py
--rw-r--r--   0 corkep     (503) staff       (20)    10083 2022-10-06 23:45:58.000000 ansitable-0.9.7/ansitable/test_ansi.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2022-10-06 23:46:20.614555 ansitable-0.9.7/ansitable.egg-info/
--rw-rw----   0 corkep     (503) staff       (20)    17339 2022-10-06 23:46:20.000000 ansitable-0.9.7/ansitable.egg-info/PKG-INFO
--rw-rw----   0 corkep     (503) staff       (20)      274 2022-10-06 23:46:20.000000 ansitable-0.9.7/ansitable.egg-info/SOURCES.txt
--rw-rw----   0 corkep     (503) staff       (20)        1 2022-10-06 23:46:20.000000 ansitable-0.9.7/ansitable.egg-info/dependency_links.txt
--rw-rw----   0 corkep     (503) staff       (20)        8 2022-10-06 23:46:20.000000 ansitable-0.9.7/ansitable.egg-info/requires.txt
--rw-rw----   0 corkep     (503) staff       (20)       10 2022-10-06 23:46:20.000000 ansitable-0.9.7/ansitable.egg-info/top_level.txt
--rw-rw----   0 corkep     (503) staff       (20)       38 2022-10-06 23:46:20.615418 ansitable-0.9.7/setup.cfg
--rw-rw----   0 corkep     (503) staff       (20)     1992 2021-03-09 02:08:15.000000 ansitable-0.9.7/setup.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-10-19 01:33:09.600169 ansitable-0.9.9/
+-rw-rw----   0 corkep     (503) staff       (20)     1068 2020-09-26 22:42:59.000000 ansitable-0.9.9/LICENSE
+-rw-r--r--   0 corkep     (503) staff       (20)    18497 2023-10-19 01:33:09.599691 ansitable-0.9.9/PKG-INFO
+-rw-r--r--   0 corkep     (503) staff       (20)    16380 2023-01-29 03:12:51.000000 ansitable-0.9.9/README.md
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-10-19 01:33:09.595682 ansitable-0.9.9/ansitable/
+-rw-rw----   0 corkep     (503) staff       (20)      132 2021-11-29 19:39:00.000000 ansitable-0.9.9/ansitable/__init__.py
+-rw-r--r--   0 corkep     (503) staff       (20)    29541 2023-05-07 09:15:13.000000 ansitable-0.9.9/ansitable/table.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-10-19 01:33:09.598415 ansitable-0.9.9/ansitable.egg-info/
+-rw-r--r--   0 corkep     (503) staff       (20)    18497 2023-10-19 01:33:09.000000 ansitable-0.9.9/ansitable.egg-info/PKG-INFO
+-rw-r--r--   0 corkep     (503) staff       (20)      256 2023-10-19 01:33:09.000000 ansitable-0.9.9/ansitable.egg-info/SOURCES.txt
+-rw-r--r--   0 corkep     (503) staff       (20)        1 2023-10-19 01:33:09.000000 ansitable-0.9.9/ansitable.egg-info/dependency_links.txt
+-rw-r--r--   0 corkep     (503) staff       (20)        8 2023-10-19 01:33:09.000000 ansitable-0.9.9/ansitable.egg-info/requires.txt
+-rw-r--r--   0 corkep     (503) staff       (20)       10 2023-10-19 01:33:09.000000 ansitable-0.9.9/ansitable.egg-info/top_level.txt
+-rw-r--r--   0 corkep     (503) staff       (20)     1221 2023-10-19 01:31:59.000000 ansitable-0.9.9/pyproject.toml
+-rw-rw----   0 corkep     (503) staff       (20)       38 2023-10-19 01:33:09.600258 ansitable-0.9.9/setup.cfg
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-10-19 01:33:09.598757 ansitable-0.9.9/tests/
+-rw-r--r--   0 corkep     (503) staff       (20)    10083 2022-10-06 23:45:58.000000 ansitable-0.9.9/tests/test_ansi.py
```

### Comparing `ansitable-0.9.7/LICENSE` & `ansitable-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ansitable-0.9.7/PKG-INFO` & `ansitable-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,51 @@
 Metadata-Version: 2.1
 Name: ansitable
-Version: 0.9.7
-Summary: Quick and easy display of tabular data and matrices with optional ANSI color and borders.
-Home-page: https://github.com/petercorke/ansitable
-Author: Peter Corke
-Author-email: rvc@petercorke.com
-License: MIT
+Version: 0.9.9
+Summary: Quick and easy display of tabular data and matrices with optional ANSI color and borders
+Author-email: Peter Corke <rvc@petercorke.com>
+License: MIT License
+        
+        Copyright (c) 2020 Peter Corke
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/petercorke/ansitable
+Project-URL: Bug Tracker, https://github.com/petercorke/ansitable/issues
+Project-URL: Documentation, https://github.com/petercorke/ansitable
 Project-URL: Source, https://github.com/petercorke/ansitable
-Project-URL: Tracker, https://github.com/petercorke/ansitable/issues
-Keywords: python table tabular matrix array border ansi-color ansi-art color ANSI
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Keywords: table,table layout,table format,tabular,tabular layout,tabular format,ANSI,ANSI art,ANSI box characters,color,ANSI color,matrix format
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.4
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: colored
 
 [![PyPI version fury.io](https://badge.fury.io/py/ansitable.svg)](https://pypi.python.org/pypi/ansitable/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/ansitable)](https://pypistats.org/packages/ansitable)
 [![Anaconda version](https://anaconda.org/conda-forge/ansitable/badges/version.svg)](https://anaconda.org/conda-forge/ansitable)
 [![pyversions](https://img.shields.io/pypi/pyversions/ansitable)](https://pypi.python.org/pypi/ansitable/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/petercorke/ansitable.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/petercorke/ansitable/context:python)
 [![PyPI status](https://img.shields.io/pypi/status/ansitable.svg)](https://pypi.python.org/pypi/ansitable/)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/petercorke/ansitable/graphs/commit-activity)
 [![GitHub license](https://img.shields.io/github/license/Naereen/StrapDown.js.svg)](https://github.com/petercorke/ansitable/blob/master/LICENSE)
 
 - GitHub repository: [https://github.com/petercorke/ansitable](https://github.com/petercorke/ansitable)
 - Dependencies: [`colored`](https://pypi.org/project/colored)
```

### Comparing `ansitable-0.9.7/README.md` & `ansitable-0.9.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [![PyPI version fury.io](https://badge.fury.io/py/ansitable.svg)](https://pypi.python.org/pypi/ansitable/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/ansitable)](https://pypistats.org/packages/ansitable)
 [![Anaconda version](https://anaconda.org/conda-forge/ansitable/badges/version.svg)](https://anaconda.org/conda-forge/ansitable)
 [![pyversions](https://img.shields.io/pypi/pyversions/ansitable)](https://pypi.python.org/pypi/ansitable/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/petercorke/ansitable.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/petercorke/ansitable/context:python)
 [![PyPI status](https://img.shields.io/pypi/status/ansitable.svg)](https://pypi.python.org/pypi/ansitable/)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/petercorke/ansitable/graphs/commit-activity)
 [![GitHub license](https://img.shields.io/github/license/Naereen/StrapDown.js.svg)](https://github.com/petercorke/ansitable/blob/master/LICENSE)
 
 - GitHub repository: [https://github.com/petercorke/ansitable](https://github.com/petercorke/ansitable)
 - Dependencies: [`colored`](https://pypi.org/project/colored)
```

### Comparing `ansitable-0.9.7/ansitable/table.py` & `ansitable-0.9.9/ansitable/table.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,38 +5,40 @@
 
 @author: corkep
 """
 import sys
 
 try:
     from colored import fg, bg, attr
+
     _colored = True
     # print('using colored output')
 except ImportError:
     # print('colored not found')
     _colored = False
 
 # _colored use color ANSI escape sequences via colored package
 # _unicode use box characters for table edges and separators
 #   from ansitable.table import _unicode
 #    _unicode = False
 
 _unicode = True
 
+
 def options(unicode, color=None):
     """
     Control ANSI/Unicode generation
 
     :param unicode: enable generation of Unicode characters
     :type unicode: bool
     :param color: enable generation of ANSI color control sequences, defaults to None
     :type color: bool, optional
 
     ANSItable by default uses Unicode characters to create nice table outlines
-    and the colored package to allow colored text and fields.  For some 
+    and the colored package to allow colored text and fields.  For some
     applications it is useful to turn this off globally, rather than on a
     table by table basis.
 
     Unicode and ANSI color can be controlled individually.  If only one parameter
     is given then:
 
     * ``ansitable.options(True)`` enable Unicode, and ANSI characters if colored
@@ -50,21 +52,33 @@
 
     _unicode = unicode
     if color is None:
         color = False
 
     _colored = color
 
+
 # ------------------------------------------------------------------------- #
 
-class Column():
-    def __init__(self, name, fmt="{}", width=None,
-        colcolor=None, colbgcolor=None, colstyle=None, colalign=">", 
-        headcolor=None, headbgcolor=None, headstyle=None, headalign=">"
-        ):
+
+class Column:
+    def __init__(
+        self,
+        name,
+        fmt="{}",
+        width=None,
+        colcolor=None,
+        colbgcolor=None,
+        colstyle=None,
+        colalign=">",
+        headcolor=None,
+        headbgcolor=None,
+        headstyle=None,
+        headalign=">",
+    ):
         """
         Create a table column
 
         :param name: Name of column, also the column heading
         :type name: str
         :param fmt: Python format string, defaults to "{}"
         :type fmt: str, optional
@@ -115,15 +129,15 @@
         underlined    text is underlined
         blink         text is blinking
         reverse       text and background colors are reversed
         ===========   =============================================
 
         Implementation of these options depends heavily on the terminal emulator
         used.
-        
+
         """
 
         self.name = name
         self.fmt = fmt
         self.formatted = []
         self.fgcolor = []
         self.table = None
@@ -158,53 +172,64 @@
             text += self.table.FG(color)
         if bgcolor is not None:
             text += self.table.BG(bgcolor)
         if style is not None:
             text += self.table.ATTR(styledict[style])
         return text
 
+
 def _spaces(n):
     return " " * n
 
+
 def _aligntext(opt, text, n, color=None):
     gap = n - len(text)
     if color:
         # text = FG(color) + text + ATTR(0)
         text = color[0] + text + color[1]
-    if  opt == '<':
+    if opt == "<":
         return text + _spaces(gap)
-    elif opt == '>':
+    elif opt == ">":
         return _spaces(gap) + text
-    elif opt == '^':
+    elif opt == "^":
         g1 = gap // 2
         g2 = gap - g1
         return _spaces(g1) + text + _spaces(g2)
 
+
 # unicode box drawing characters, see https://en.wikipedia.org/wiki/Box-drawing_character
 #       ascii, thin, thin+round, thick, double
-_tl = [ord('+'), 0x250c, 0x256d, 0x250f, 0x2554]
-_tr = [ord('+'), 0x2510, 0x256e, 0x2513, 0x2557]
-_bl = [ord('+'), 0x2514, 0x2570, 0x2517, 0x255a]
-_br = [ord('+'), 0x2518, 0x256f, 0x251b, 0x255c]
-_lj = [ord('+'), 0x251c, 0x251c, 0x2523, 0x2560]
-_rj = [ord('+'), 0x2524, 0x2524, 0x252b, 0x2563]
-_tj = [ord('+'), 0x252c, 0x252c, 0x2533, 0x2566]
-_bj = [ord('+'), 0x2534, 0x2534, 0x253b, 0x2569]
-_xj = [ord('+'), 0x253c, 0x253c, 0x254b, 0x256c]
-_hl = [ord('-'), 0x2500, 0x2500, 0x2501, 0x2550]
-_vl = [ord('|'), 0x2502, 0x2502, 0x2503, 0x2551]
-
-borderdict = {"ascii": 0, "thin": 1, "round": 2, "thick": 3, "double": 4, "thick-thin": 5, "double-thin":6}
-styledict = {"bold": 1, "dim": 2, "underlined": 4, "blink": 5, "reverse":7}
+_tl = [ord("+"), 0x250C, 0x256D, 0x250F, 0x2554]
+_tr = [ord("+"), 0x2510, 0x256E, 0x2513, 0x2557]
+_bl = [ord("+"), 0x2514, 0x2570, 0x2517, 0x255A]
+_br = [ord("+"), 0x2518, 0x256F, 0x251B, 0x255C]
+_lj = [ord("+"), 0x251C, 0x251C, 0x2523, 0x2560]
+_rj = [ord("+"), 0x2524, 0x2524, 0x252B, 0x2563]
+_tj = [ord("+"), 0x252C, 0x252C, 0x2533, 0x2566]
+_bj = [ord("+"), 0x2534, 0x2534, 0x253B, 0x2569]
+_xj = [ord("+"), 0x253C, 0x253C, 0x254B, 0x256C]
+_hl = [ord("-"), 0x2500, 0x2500, 0x2501, 0x2550]
+_vl = [ord("|"), 0x2502, 0x2502, 0x2503, 0x2551]
+
+borderdict = {
+    "ascii": 0,
+    "thin": 1,
+    "round": 2,
+    "thick": 3,
+    "double": 4,
+    "thick-thin": 5,
+    "double-thin": 6,
+}
+styledict = {"bold": 1, "dim": 2, "underlined": 4, "blink": 5, "reverse": 7}
 
 # ------------------------------------------------------------------------- #
 
-class ANSIMatrix:
 
-    def __init__(self, style='thin', fmt='{:< 10.3g}', squish=100):
+class ANSIMatrix:
+    def __init__(self, style="thin", fmt="{:< 10.3g}", squish=100):
         """
         Create a matrix formatter
 
         :param style: Bracket format, defaults to 'thin'
         :type style: str, optional
         :param fmt: number format string, defaults to '{:< 10.3g}'
         :type fmt: str, optional
@@ -232,25 +257,24 @@
         """
 
         # TODO: add colored fields, specify by tuples (rowstart, rowend, colstart, colend, color)
 
         import numpy as np  # only import if matrix is used
 
         if not _unicode:
-            style = 'ascii'
+            style = "ascii"
         self.style = borderdict[style]
         self.fmt = fmt
         self.width = len(fmt.format(1))
         if squish == 0:
             self.squish = None
         else:
             self.squish = squish * np.finfo(float).eps
-            
 
-    def str(self, matrix, suffix_super='', suffix_sub=''):
+    def str(self, matrix, suffix_super="", suffix_sub=""):
         """
         Output the table as a string
 
         :param matrix: NumPy matrix to format
         :type matrix: 1d or 2d ndarray
         :param suffix_super: Right superscript, defaults to ''
         :type suffix_super: str, optional
@@ -265,27 +289,32 @@
 
         if len(matrix.shape) == 1:
             ncols = matrix.shape[0]
             matrix = matrix.reshape((1, -1))
         elif len(matrix.shape) == 2:
             ncols = matrix.shape[1]
         else:
-            raise ValueError('Only 1D and 2D arrays supported')
+            raise ValueError("Only 1D and 2D arrays supported")
 
         mwidth = ncols * self.width + (ncols - 1)
         if self.squish is None:
             m2 = matrix
         else:
             m2 = np.where(abs(matrix) < self.squish, 0, matrix)
         b = self.style
 
-        s = chr(_tl[b]) + ' ' * mwidth + chr(_tr[b]) + suffix_super + '\n'
+        s = chr(_tl[b]) + " " * mwidth + chr(_tr[b]) + suffix_super + "\n"
         for row in m2:
-            s += chr(_vl[b]) + ' '.join([self.fmt.format(x) for x in row]) + chr(_vl[b]) + '\n'
-        s += chr(_bl[b]) + ' ' * mwidth + chr(_br[b]) + suffix_sub
+            s += (
+                chr(_vl[b])
+                + " ".join([self.fmt.format(x) for x in row])
+                + chr(_vl[b])
+                + "\n"
+            )
+        s += chr(_bl[b]) + " " * mwidth + chr(_br[b]) + suffix_sub
         return s
 
     def print(self, matrix, *pos, file=sys.stdout, **kwargs):
         """
         Print the matrix
 
         :param file: Print the matrix to this file, defaults to stdout
@@ -293,20 +322,33 @@
 
         .. note:: Accepts the same arguments as ``str``.
 
         """
 
         print(self.str(matrix, *pos, **kwargs), file=file)
 
+
 # ------------------------------------------------------------------------- #
 
+
 class ANSITable:
     _color = _colored
 
-    def __init__(self, *pos, colsep = 2, offset=0, border=None, bordercolor=None, ellipsis=True, columns=None, header=True, color=True):
+    def __init__(
+        self,
+        *pos,
+        colsep=2,
+        offset=0,
+        border=None,
+        bordercolor=None,
+        ellipsis=True,
+        columns=None,
+        header=True,
+        color=True,
+    ):
         """
         Create a table object
 
         :param colsep: Separation between columns, defaults to 2
         :type colsep: int, optional
         :param offset: Horizontal offset of the whole table, defaults to 0
         :type offset: int, optional
@@ -349,29 +391,29 @@
         self.ellipsis = ellipsis
         self.rows = []
         self.bordercolor = bordercolor
         self.header = header
         self.color = color and self._color
 
         if border is not None and not _unicode:
-            border = 'ascii'
+            border = "ascii"
         self.border = border
-        
+
         self.nrows = 0
         self.columns = []
         for c in pos:
             if isinstance(c, str):
                 c = Column(c)
                 c.table = self
                 self.columns.append(c)
             elif isinstance(c, Column):
                 c.table = self
                 self.columns.append(c)
             else:
-                raise TypeError('expecting a lists of Column objects')
+                raise TypeError("expecting a lists of Column objects")
         if len(self.columns) == 0 and columns is not None:
             for _ in range(columns):
                 self.columns.append("")
 
     def addcolumn(self, name, **kwargs):
         """
         Add a column to the table
@@ -385,56 +427,63 @@
 
             table = ANSITable()
             table.addcolumnColumn("col1"),
             table.addcolumnColumn("column 2 has a big header", "{:.3g}"),
             table.addcolumnColumn("column 3", "{:-10.4f}")
 
         .. note:: Additional arguments are passed directly to ``Column``.
-    
+
         """
         self.columns.append(Column(name, **kwargs))
 
-    def row(self, *values):
+    def row(self, *values, rowcolor=None, rowbgcolor=None, rowstyle=None,):
         """
         Add a row of data
 
+        :param values: sequence of values, one per column
+        :param rowcolor: Color of row text, defaults to None
+        :type rowcolor: str, optional
+        :param rowbgcolor: Color of row background, defaults to None
+        :type colbgcolor: str, optional
+        :param rowstyle: Row text style, see table below, defaults to None
+        :type colstyle: str, optional
         :raises ValueError: invalid format string for the data provided
 
         ``table.row(d1, d2, ... dN)`` add data items that comprise a row of the
         table.  ``N`` is the number of columns.
 
         The data items can be any type, but the format string specified at
         table creation must be compatible.
         """
-        assert len(values) == len(self.columns), 'wrong number of data items added'
+        assert len(values) == len(self.columns), "wrong number of data items added"
 
         for value, c in zip(values, self.columns):
             if c.fmt is None:
                 s = value
             elif isinstance(c.fmt, str):
                 s = c.fmt.format(value)
             elif callable(c.fmt):
                 s = c.fmt(value)
             else:
-                raise ValueError('fmt must be valid format string or callable')
+                raise ValueError("fmt must be valid format string or callable")
 
             # handle a FG color specifier
-            if s.startswith('<<'):
+            if s.startswith("<<"):
                 # color specifier is given
-                end = s.find('>>')
+                end = s.find(">>")
                 color = s[2:end]
-                s = s[end+2:]
+                s = s[end + 2 :]
             else:
                 color = None
 
             if c.width is not None and len(s) > c.width:
                 if self.ellipsis:
-                    s = s[:c.width - 1] + "\u2026"
+                    s = s[: c.width - 1] + "\u2026"
                 else:
-                    s = s[:c.width]
+                    s = s[: c.width]
             c.maxwidth = max(c.maxwidth, len(s))
 
             c.formatted.append(s)
             c.fgcolor.append(color)
         self.nrows += 1
 
     def rule(self):
@@ -455,27 +504,27 @@
     def _midline(self):
         return self._line(_lj, _xj, _rj)
 
     def _bottomline(self):
         return self._line(_bl, _bj, _br)
 
     def _line(self, left, mid, right):
-        if self.borderdict is  None:
+        if self.borderdict is None:
             return ""
         else:
             b = self.borderdict
             c2 = self.colsep // 2
             text = _spaces(self.offset - 1)
             if self.bordercolor is not None:
                 text += self.FG(self.bordercolor)
             text += chr(left[b])
             for c in self.columns:
                 text += chr(_hl[b]) * (c.width + c2)
                 if not c.last:
-                    text += chr(mid[b]) + chr(_hl[b]) * c2 
+                    text += chr(mid[b]) + chr(_hl[b]) * c2
             text += chr(right[b])
             if self.bordercolor is not None:
                 text += self.ATTR(0)
             return text + "\n"
 
     def _vline(self):
         if self.borderdict is not None:
@@ -502,73 +551,81 @@
                 ansi = c._settyle(row is None)
                 text += ansi
                 if row is None:
                     # header
                     text += _aligntext(c.headalign, c.name, c.width)
                 else:
                     # table row proper
-                    text += _aligntext(c.colalign, c.formatted[row], c.width, 
-                        (self.FG(c.fgcolor[row]), self.ATTR(0)))
+                    text += _aligntext(
+                        c.colalign,
+                        c.formatted[row],
+                        c.width,
+                        (self.FG(c.fgcolor[row]), self.ATTR(0)),
+                    )
                 if len(ansi) > 0:
                     text += self.ATTR(0)
 
                 c2 = self.colsep // 2
                 if not c.last:
-                    text += _spaces(c2) + self._vline() +  _spaces(c2)
+                    text += _spaces(c2) + self._vline() + _spaces(c2)
                 else:
                     text += _spaces(c2) + self._vline()
         else:
             # no border
             text = _spaces(self.offset)
 
             for c in self.columns:
                 ansi = c._settyle(row is None)
                 text += ansi
                 if row is None:
                     # header
                     text += _aligntext(c.headalign, c.name, c.width)
                 else:
                     # table row proper
-                    text += _aligntext(c.colalign, c.formatted[row], c.width, 
-                                (self.FG(c.fgcolor[row]), self.ATTR(0)))
+                    text += _aligntext(
+                        c.colalign,
+                        c.formatted[row],
+                        c.width,
+                        (self.FG(c.fgcolor[row]), self.ATTR(0)),
+                    )
                 if len(ansi) > 0:
                     text += self.ATTR(0)
-                text +=  _spaces(self.colsep)
+                text += _spaces(self.colsep)
 
         return text + "\n"
 
-    def print(self, file=None):
+    def ansi(self, file=None):
         """
         Print the table
 
         :param file: Print the table to this file, defaults to stdout
         :type file: writeable object, optional
 
         Example::
 
             table = ANSITable("col1", "column 2 has a big header", "column 3")
             table.row("aaaaaaaaa", 2.2, 3)
             table.row("bbbbbbbbbbbbb", -5.5, 6)
             table.row("ccccccc", 8.8, -9)
             table.print()
-            
+
             +--------------+---------------------------+----------+
             |         col1 | column 2 has a big header | column 3 |
             +--------------+---------------------------+----------+
             |    aaaaaaaaa |                       2.2 |        3 |
             |bbbbbbbbbbbbb |                      -5.5 |        6 |
             |      ccccccc |                       8.8 |       -9 |
             +--------------+---------------------------+----------+
 
         """
 
         try:
             print(str(self), file=file)
         except UnicodeEncodeError:
-            self.border = 'ascii'
+            self.border = "ascii"
             print(str(self), file=file)
 
     def __str__(self):
         """
         Output the table as a string
 
         :return: ANSI string
@@ -596,15 +653,15 @@
         if self.header:
             text += self._row()
             text += self._midline()
 
         # rows
         for i in range(self.nrows):
             text += self._row(i)
-        
+
         # footer
         text += self._bottomline()
 
         return text
 
     def markdown(self):
         """
@@ -616,48 +673,48 @@
         Example::
 
             table = ANSITable("col1", "column 2 has a big header", "column 3")
             table.row("aaaaaaaaa", 2.2, 3)
             table.row("bbbbbbbbbbbbb", -5.5, 6)
             table.row("ccccccc", 8.8, -9)
             table.markdown()
-            
+
             |          col1 | column 2 has a big header | column 3 |
             | ------------: | ------------------------: | -------: |
             |     aaaaaaaaa |                       2.2 |        3 |
             | bbbbbbbbbbbbb |                      -5.5 |        6 |
             |       ccccccc |                       8.8 |       -9 |
 
         .. note::
             - supports column alignment
             - does not support header alignment, same as column
         """
 
         # markdown table setup
-        s = ''
+        s = ""
 
         # column headers
         for c in self.columns:
-            s += '| ' + _aligntext(c.headalign, c.name, c.width) + ' '
+            s += "| " + _aligntext(c.headalign, c.name, c.width) + " "
         s += "|\n"
 
         for c in self.columns:
-            if c.headalign == '<':
-                bar = ':' + '-' * (c.width - 1)
-            elif c.headalign == '^':
-                bar = ':' + '-' * (c.width - 2) + ':'
-            elif c.headalign == '>':
-                bar = '-' * (c.width - 1) + ':'
-            s += '| ' + bar + ' '
+            if c.headalign == "<":
+                bar = ":" + "-" * (c.width - 1)
+            elif c.headalign == "^":
+                bar = ":" + "-" * (c.width - 2) + ":"
+            elif c.headalign == ">":
+                bar = "-" * (c.width - 1) + ":"
+            s += "| " + bar + " "
         s += "|\n"
 
         # rows
         for i in range(self.nrows):
             for c in self.columns:
-                s += '| ' + _aligntext(c.colalign, c.formatted[i], c.width) + ' '
+                s += "| " + _aligntext(c.colalign, c.formatted[i], c.width) + " "
             s += "|\n"
 
         return s
 
     def latex(self):
         r"""
         Output the table in LaTeX format
@@ -685,48 +742,51 @@
             - supports column alignment
             - supports header alignment
         """
 
         # LaTeX tabular setup
         s = "\\begin{tabular}{ |"
         for c in self.columns:
-            if c.colalign == '<':
-                s += 'l|'
-            elif c.colalign == '^':
-                s += 'c|'
-            elif c.colalign == '>':
-                s += 'r|'
+            if c.colalign == "<":
+                s += "l|"
+            elif c.colalign == "^":
+                s += "c|"
+            elif c.colalign == ">":
+                s += "r|"
         s += " }\\hline\n"
 
         # column headers
         first = True
         for c in self.columns:
             if first:
                 first = False
             else:
-                s += ' & '
+                s += " & "
 
-            s += '\\multicolumn{1}{'
-            if c.headalign == '<':
-                s += '|l|'
-            elif c.headalign == '^':
-                s += '|c|'
-            elif c.headalign == '>':
-                s += '|r|'
+            s += "\\multicolumn{1}{"
+            if c.headalign == "<":
+                s += "|l|"
+            elif c.headalign == "^":
+                s += "|c|"
+            elif c.headalign == ">":
+                s += "|r|"
             s += "}{" + c.name + "}"
 
         s += "\\\\\\hline\\hline\n"
         # rows
         for i in range(self.nrows):
             first = True
             for c in self.columns:
                 if first:
                     first = False
                 else:
-                    s += ' & '
+                    s += " & "
+                if c.formatted[i] is None:
+                    s += "\\hline\n"
+                    break
                 s += c.formatted[i]
             s += " \\\\\n"
         s += "\\hline\n"
         s += "\\end{tabular}\n"
         return s
 
     def FG(self, c):
@@ -741,36 +801,47 @@
         else:
             return ""
 
     def ATTR(self, c):
         if _unicode and self.color and c is not None:
             return attr(c)
         else:
-            return "" 
+            return ""
+
+    def print(self, format="ansi", file=None, **kwargs):
+        if format == "ansi":
+            self.ansi(file=None, **kwargs)
+        elif format == "latex":
+            s = self.latex(**kwargs)
+            print(s, file=file)
+        elif format == "markdown":
+            s = self.markdown(**kwargs)
+            print(s, file=file)
+
 
 if __name__ == "__main__":
 
     import numpy as np
 
     ANSITable._unicode = False
 
     # -------------------------------- test ANSIMatrix
-    m = np.arange(16).reshape((4,4)) /10 - 0.8
-    m[0,0] = 1.23456e-14
+    m = np.arange(16).reshape((4, 4)) / 10 - 0.8
+    m[0, 0] = 1.23456e-14
     print(m)
     print(np.array2string(m))
 
-    formatter = ANSIMatrix(style='thick', squish=True)
+    formatter = ANSIMatrix(style="thick", squish=True)
 
     formatter.print(m)
 
-    formatter.print(m, suffix_super='T', suffix_sub='3')
+    formatter.print(m, suffix_super="T", suffix_sub="3")
 
     m = np.arange(4) / 4 - 0.5
-    formatter.print(m, 'T')
+    formatter.print(m, "T")
 
     # -------------------------------- test ANSITable
 
     table = ANSITable("col1", "column 2 has a big header", "column 3", color=False)
     table.row("aaaaaaaaa", 2.2, 3)
     table.row("bbbbbbbbbbbbb", -5.5, 6)
     table.row("ccccccc", 8.8, -9)
@@ -779,112 +850,109 @@
     table = ANSITable("col1", "column 2 has a big header", "column 3", color=False)
     table.row("aaaaaaaaa", 2.2, 3)
     table.row("<<red>>bbbbbbbbbbbbb", 5.5, 6)
     table.row("<<blue>>ccccccc", 8.8, -9)
     table.print()
 
     table = ANSITable(
-        Column("col1"),
-        Column("column 2 has a big header"),
-        Column("column 3")
+        Column("col1"), Column("column 2 has a big header"), Column("column 3")
     )
     table.row("aaaaaaaaa", 2.2, 3)
     table.row("bbbbbbbbbbbbb", -5.5, 6)
     table.row("ccccccc", 8.8, -9)
     table.print()
 
     table = ANSITable(
         Column("col1"),
         Column("column 2 has a big header", "{:.3g}"),
-        Column("column 3", "{:-10.4f}")
+        Column("column 3", "{:-10.4f}"),
     )
     table.row("aaaaaaaaa", 2.2, 3)
     table.row("bbbbbbbbbbbbb", -5.5, 6)
     table.row("ccccccc", 8.8, -9)
     table.print()
 
     table = ANSITable(
         Column("col1", width=10),
         Column("column 2 has a big header", "{:.3g}"),
-        Column("column 3", "{:-10.4f}")
+        Column("column 3", "{:-10.4f}"),
     )
     table.row("aaaaaaaaa", 2.2, 3)
     table.row("bbbbbbbbbbbbb", -5.5, 6)
     table.row("ccccccc", 8.8, -9)
     table.print()
 
     table = ANSITable(
         Column("col1"),
         Column("column 2 has a big header"),
         Column("column 3"),
-        border="ascii"
+        border="ascii",
     )
     table.row("aaaaaaaaa", 2.2, 3)
     table.row("bbbbbbbbbbbbb", -5.5, 6)
     table.row("ccccccc", 8.8, -9)
     table.print()
 
     table = ANSITable(
         Column("col1"),
         Column("column 2 has a big header"),
         Column("column 3"),
-        border="thick"
+        border="thick",
     )
     table.row("aaaaaaaaa", 2.2, 3)
     table.row("bbbbbbbbbbbbb", -5.5, 6)
     table.row("ccccccc", 8.8, -9)
     table.print()
 
     table = ANSITable(
         Column("col1"),
         Column("column 2 has a big header", colalign="^"),
         Column("column 3"),
-        border="thick"
+        border="thick",
     )
     table.row("aaaaaaaaa", 2.2, 3)
     table.row("bbbbbbbbbbbbb", -5.5, 6)
     table.row("ccccccc", 8.8, -9)
     table.print()
 
     table = ANSITable(
         Column("col1", headalign="<"),
         Column("column 2 has a big header", colalign="^"),
         Column("column 3", colalign="<"),
-        border="thick"
+        border="thick",
     )
     table.row("aaaaaaaaa", 2.2, 3)
     table.row("bbbbbbbbbbbbb", -5.5, 6)
     table.row("ccccccc", 8.8, -9)
     table.print()
 
     table = ANSITable(
         Column("col1", headalign="<"),
         Column("column 2 has a big header", colalign="^", colstyle="reverse"),
         Column("column 3", colalign="<"),
-        border="thick"
+        border="thick",
     )
     table.row("aaaaaaaaa", 2.2, 3)
     table.row("bbbbbbbbbbbbb", -5.5, 6)
     table.row("ccccccc", 8.8, -9)
     table.print()
 
     table = ANSITable(
         Column("col1", headalign="<", colcolor="red", headstyle="underlined"),
         Column("column 2 has a big header", colalign="^", colstyle="reverse"),
         Column("column 3", colalign="<", colbgcolor="green", fmt="{: d}"),
-        border="thick", bordercolor="blue"
+        border="thick",
+        bordercolor="blue",
     )
     table.row("aaaaaaaaa", 2.2, 3)
     table.row("bbbbbbbbbbbbb", -5.5, 6)
     table.rule()
     table.row("ccccccc", 8.8, -9)
     table.print()
 
-
     table = ANSITable("col1", "column 2 has a big header", "column 3")
     table.row("aaaaaaaaa", 2.2, 3)
     table.row("bbbbbbbbbbbbb", -5.5, 6)
     table.row("ccccccc", 8.8, -9)
     table.print()
-    print(table.latex())
-    print(table.markdown())
-
+    table.print(format="latex")
+    table.print(format="markdown")
```

### Comparing `ansitable-0.9.7/ansitable/test_ansi.py` & `ansitable-0.9.9/tests/test_ansi.py`

 * *Files identical despite different names*

### Comparing `ansitable-0.9.7/ansitable.egg-info/PKG-INFO` & `ansitable-0.9.9/ansitable.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,51 @@
 Metadata-Version: 2.1
 Name: ansitable
-Version: 0.9.7
-Summary: Quick and easy display of tabular data and matrices with optional ANSI color and borders.
-Home-page: https://github.com/petercorke/ansitable
-Author: Peter Corke
-Author-email: rvc@petercorke.com
-License: MIT
+Version: 0.9.9
+Summary: Quick and easy display of tabular data and matrices with optional ANSI color and borders
+Author-email: Peter Corke <rvc@petercorke.com>
+License: MIT License
+        
+        Copyright (c) 2020 Peter Corke
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/petercorke/ansitable
+Project-URL: Bug Tracker, https://github.com/petercorke/ansitable/issues
+Project-URL: Documentation, https://github.com/petercorke/ansitable
 Project-URL: Source, https://github.com/petercorke/ansitable
-Project-URL: Tracker, https://github.com/petercorke/ansitable/issues
-Keywords: python table tabular matrix array border ansi-color ansi-art color ANSI
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Keywords: table,table layout,table format,tabular,tabular layout,tabular format,ANSI,ANSI art,ANSI box characters,color,ANSI color,matrix format
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.4
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: colored
 
 [![PyPI version fury.io](https://badge.fury.io/py/ansitable.svg)](https://pypi.python.org/pypi/ansitable/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/ansitable)](https://pypistats.org/packages/ansitable)
 [![Anaconda version](https://anaconda.org/conda-forge/ansitable/badges/version.svg)](https://anaconda.org/conda-forge/ansitable)
 [![pyversions](https://img.shields.io/pypi/pyversions/ansitable)](https://pypi.python.org/pypi/ansitable/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/petercorke/ansitable.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/petercorke/ansitable/context:python)
 [![PyPI status](https://img.shields.io/pypi/status/ansitable.svg)](https://pypi.python.org/pypi/ansitable/)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/petercorke/ansitable/graphs/commit-activity)
 [![GitHub license](https://img.shields.io/github/license/Naereen/StrapDown.js.svg)](https://github.com/petercorke/ansitable/blob/master/LICENSE)
 
 - GitHub repository: [https://github.com/petercorke/ansitable](https://github.com/petercorke/ansitable)
 - Dependencies: [`colored`](https://pypi.org/project/colored)
```

