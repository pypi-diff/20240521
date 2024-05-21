# Comparing `tmp/constyle-2.0.3.tar.gz` & `tmp/constyle-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constyle-2.0.3.tar", max compression
+gzip compressed data, was "constyle-2.0.4.tar", max compression
```

## Comparing `constyle-2.0.3.tar` & `constyle-2.0.4.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-04-24 13:19:44.006688 constyle-2.0.3/LICENSE
--rw-r--r--   0        0        0     5429 2023-04-24 13:19:44.006688 constyle-2.0.3/README.md
--rw-r--r--   0        0        0      332 2023-04-24 13:19:44.006688 constyle-2.0.3/constyle/__init__.py
--rw-r--r--   0        0        0     1839 2023-04-24 13:19:44.006688 constyle-2.0.3/constyle/__main__.py
--rw-r--r--   0        0        0     7465 2023-04-24 13:19:44.006688 constyle-2.0.3/constyle/_attributes.py
--rw-r--r--   0        0        0     3015 2023-04-24 13:19:44.006688 constyle-2.0.3/constyle/_style.py
--rw-r--r--   0        0        0     2913 2023-04-24 13:19:44.006688 constyle-2.0.3/constyle/custom_colours.py
--rw-r--r--   0        0        0        1 2023-04-24 13:19:44.006688 constyle-2.0.3/constyle/py.typed
--rw-r--r--   0        0        0      903 2023-04-24 13:19:56.390661 constyle-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     6422 2023-04-24 13:19:57.221118 constyle-2.0.3/setup.py
--rw-r--r--   0        0        0     6361 2023-04-24 13:19:57.221652 constyle-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-21 13:00:04.276417 constyle-2.0.4/LICENSE
+-rw-r--r--   0        0        0     5488 2024-05-21 13:45:05.578077 constyle-2.0.4/README.md
+-rw-r--r--   0        0        0      332 2024-05-21 13:00:04.276417 constyle-2.0.4/constyle/__init__.py
+-rw-r--r--   0        0        0     1839 2024-05-21 13:00:04.276417 constyle-2.0.4/constyle/__main__.py
+-rw-r--r--   0        0        0     7465 2024-05-21 13:00:04.276417 constyle-2.0.4/constyle/_attributes.py
+-rw-r--r--   0        0        0     3173 2024-05-21 13:45:05.578077 constyle-2.0.4/constyle/_style.py
+-rw-r--r--   0        0        0     2913 2024-05-21 13:00:04.276417 constyle-2.0.4/constyle/custom_colours.py
+-rw-r--r--   0        0        0        1 2024-05-21 13:00:04.276417 constyle-2.0.4/constyle/py.typed
+-rw-r--r--   0        0        0      903 2024-05-21 13:45:37.434049 constyle-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6522 1970-01-01 00:00:00.000000 constyle-2.0.4/PKG-INFO
```

### Comparing `constyle-2.0.3/LICENSE` & `constyle-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `constyle-2.0.3/README.md` & `constyle-2.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 ### `Style` objects
 
 You can also use `Style` objects to create a reusable style with any number of attributes.
 
 #### Calling a `Style` object
 
-`Style` objects are callable and take a string as input and return a styled string.
+`Style` objects are callable and take a string as input (or any other object, which will be converted to a string) and return a styled string.
 
 ```py
 warning = Style(Attributes.YELLOW, Attributes.BOLD)
 print(warning('You shall not pass!'))
 ```
 
 #### Adding `Style` objects
```

### Comparing `constyle-2.0.3/constyle/__main__.py` & `constyle-2.0.4/constyle/__main__.py`

 * *Files identical despite different names*

### Comparing `constyle-2.0.3/constyle/_attributes.py` & `constyle-2.0.4/constyle/_attributes.py`

 * *Files identical despite different names*

### Comparing `constyle-2.0.3/constyle/_style.py` & `constyle-2.0.4/constyle/_style.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,21 +35,23 @@
             itertools.chain.from_iterable(
                 attr._params if isinstance(attr, Style) else (attr,) for attr in attrs
             )
         )
         self._prefix = f"\033[{';'.join(str(p) for p in self._params)}m"
         self._end = end
 
-    def __call__(self, string: str) -> str:
+    def __call__(self, string: object) -> str:
         """Apply this style to the given string.
 
+        If the given object isn't a string it will be converted into one.
+
         Args:
             string: The string to apply the style to.
         """
-        return f"{self}{string}{self._end or Style()}" if string else string
+        return f"{self}{string}{self._end or Style()}" if string != "" else string
 
     def __add__(self, other: "Style") -> "Style":
         """Add the attributes of the left and right `Style` operands, returning a new `Style`.
 
         NOTE: The returned `Style` will have the default `end` style and not the `end` style of the left or right operands.
 
         Returns:
@@ -68,16 +70,18 @@
         return (
             isinstance(__o, Style)
             and self._params == __o._params
             and self._end == __o._end
         )
 
 
-def style(string: str, *attrs: "Style", end: "Optional[Style]" = None) -> str:
+def style(string: object, *attrs: "Style", end: "Optional[Style]" = None) -> str:
     """Apply the given attributes to the given string.
 
+    If the given object isn't a string it will be converted into one.
+
     Args:
         string: The string to style.
         *attrs: The attributes/styles to apply.
         end: The style to apply after the string. If None (the default) it will reset all attributes at the end.
     """
     return Style(*attrs, end=end)(string)
```

### Comparing `constyle-2.0.3/constyle/custom_colours.py` & `constyle-2.0.4/constyle/custom_colours.py`

 * *Files identical despite different names*

### Comparing `constyle-2.0.3/pyproject.toml` & `constyle-2.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "constyle"
 # Version is overwritten at build time by CI based on git tag
-version = "2.0.3"
+version = "2.0.4"
 description = "A Python library to add style to your console."
 authors = ["Abraham Murciano <abrahammurciano@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/abrahammurciano/python-constyle"
 documentation = "https://abrahammurciano.github.io/python-constyle/constyle"
 keywords = [
```

### Comparing `constyle-2.0.3/PKG-INFO` & `constyle-2.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: constyle
-Version: 2.0.3
+Version: 2.0.4
 Summary: A Python library to add style to your console.
 Home-page: https://github.com/abrahammurciano/python-constyle
 License: GPLv3
 Keywords: terminal,console,style,color,colors,colour,colours,ansi
 Author: Abraham Murciano
 Author-email: abrahammurciano@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: attributes-doc (>=0.3.0)
 Requires-Dist: importlib-metadata (>=4.11.0)
 Project-URL: Documentation, https://abrahammurciano.github.io/python-constyle/constyle
 Project-URL: Repository, https://github.com/abrahammurciano/python-constyle
 Description-Content-Type: text/markdown
 
 # constyle
@@ -66,15 +68,15 @@
 
 ### `Style` objects
 
 You can also use `Style` objects to create a reusable style with any number of attributes.
 
 #### Calling a `Style` object
 
-`Style` objects are callable and take a string as input and return a styled string.
+`Style` objects are callable and take a string as input (or any other object, which will be converted to a string) and return a styled string.
 
 ```py
 warning = Style(Attributes.YELLOW, Attributes.BOLD)
 print(warning('You shall not pass!'))
 ```
 
 #### Adding `Style` objects
```

