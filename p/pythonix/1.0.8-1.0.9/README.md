# Comparing `tmp/pythonix-1.0.8.tar.gz` & `tmp/pythonix-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonix-1.0.8.tar", max compression
+gzip compressed data, was "pythonix-1.0.9.tar", max compression
```

## Comparing `pythonix-1.0.8.tar` & `pythonix-1.0.9.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0     3027 2024-05-08 15:21:18.899631 pythonix-1.0.8/README.md
--rw-r--r--   0        0        0      409 2024-05-16 19:24:04.169631 pythonix-1.0.8/pyproject.toml
--rw-r--r--   0        0        0       24 2024-05-16 16:50:54.529631 pythonix-1.0.8/pythonix/__init__.py
--rw-r--r--   0        0        0      465 2024-05-16 16:50:54.539631 pythonix-1.0.8/pythonix/curry.py
--rw-r--r--   0        0        0      387 2024-05-16 16:50:54.539631 pythonix-1.0.8/pythonix/dict_utils.py
--rw-r--r--   0        0        0      953 2024-05-16 18:06:43.809631 pythonix-1.0.8/pythonix/grammar.py
--rw-r--r--   0        0        0       28 2024-05-16 16:50:54.529631 pythonix-1.0.8/pythonix/internals/__init__.py
--rw-r--r--   0        0        0     8835 2024-05-16 19:05:47.559631 pythonix-1.0.8/pythonix/internals/curry.py
--rw-r--r--   0        0        0     3960 2024-05-16 16:50:54.709631 pythonix-1.0.8/pythonix/internals/dict_utils.py
--rw-r--r--   0        0        0     3634 2024-05-16 18:14:38.709631 pythonix-1.0.8/pythonix/internals/grammar.py
--rw-r--r--   0        0        0     4003 2024-05-16 19:12:13.159631 pythonix-1.0.8/pythonix/internals/mdeq.py
--rw-r--r--   0        0        0     5374 2024-05-16 16:50:54.759631 pythonix-1.0.8/pythonix/internals/op.py
--rw-r--r--   0        0        0     1349 2024-05-16 16:50:42.429631 pythonix-1.0.8/pythonix/internals/pair.py
--rw-r--r--   0        0        0     2802 2024-05-16 16:50:54.619631 pythonix-1.0.8/pythonix/internals/pipe.py
--rw-r--r--   0        0        0     1801 2024-05-16 19:06:43.679631 pythonix-1.0.8/pythonix/internals/prove.py
--rw-r--r--   0        0        0     7203 2024-05-16 16:50:54.819631 pythonix-1.0.8/pythonix/internals/req.py
--rw-r--r--   0        0        0    14294 2024-05-16 19:08:46.789631 pythonix-1.0.8/pythonix/internals/res.py
--rw-r--r--   0        0        0     5041 2024-05-16 19:09:41.649631 pythonix-1.0.8/pythonix/internals/trail.py
--rw-r--r--   0        0        0     2726 2024-05-16 16:26:19.349631 pythonix-1.0.8/pythonix/internals/tup.py
--rw-r--r--   0        0        0      420 2024-05-16 16:50:54.629631 pythonix-1.0.8/pythonix/mdeq.py
--rw-r--r--   0        0        0      251 2024-05-16 16:50:54.619631 pythonix-1.0.8/pythonix/op.py
--rw-r--r--   0        0        0      265 2024-05-16 16:50:54.629631 pythonix-1.0.8/pythonix/pair.py
--rw-r--r--   0        0        0      886 2024-05-16 16:18:58.339631 pythonix-1.0.8/pythonix/pipe.py
--rw-r--r--   0        0        0     2558 2024-05-16 19:23:47.789631 pythonix-1.0.8/pythonix/prelude.py
--rw-r--r--   0        0        0      210 2024-05-16 16:50:54.639631 pythonix-1.0.8/pythonix/prove.py
--rw-r--r--   0        0        0      645 2024-05-16 16:24:04.869631 pythonix-1.0.8/pythonix/req.py
--rw-r--r--   0        0        0     6424 2024-05-16 16:50:54.679631 pythonix-1.0.8/pythonix/res.py
--rw-r--r--   0        0        0      290 2024-05-16 16:50:54.669631 pythonix-1.0.8/pythonix/trail.py
--rw-r--r--   0        0        0      358 2024-05-16 16:50:54.679631 pythonix-1.0.8/pythonix/tup.py
--rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 pythonix-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3027 2024-05-08 15:21:18.899631 pythonix-1.0.9/README.md
+-rw-r--r--   0        0        0      409 2024-05-21 15:50:26.570000 pythonix-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-05-16 16:50:54.529631 pythonix-1.0.9/pythonix/__init__.py
+-rw-r--r--   0        0        0      610 2024-05-21 03:33:06.740000 pythonix-1.0.9/pythonix/curry.py
+-rw-r--r--   0        0        0      596 2024-05-21 15:33:42.330000 pythonix-1.0.9/pythonix/deq.py
+-rw-r--r--   0        0        0      709 2024-05-21 03:10:17.490000 pythonix-1.0.9/pythonix/dict_utils.py
+-rw-r--r--   0        0        0      759 2024-05-19 18:08:28.990000 pythonix-1.0.9/pythonix/fn.py
+-rw-r--r--   0        0        0     1528 2024-05-21 02:08:58.640000 pythonix-1.0.9/pythonix/grammar.py
+-rw-r--r--   0        0        0       28 2024-05-16 16:50:54.529631 pythonix-1.0.9/pythonix/internals/__init__.py
+-rw-r--r--   0        0        0    10528 2024-05-21 03:32:59.410000 pythonix-1.0.9/pythonix/internals/curry.py
+-rw-r--r--   0        0        0     6837 2024-05-21 15:33:22.620000 pythonix-1.0.9/pythonix/internals/deq.py
+-rw-r--r--   0        0        0     4445 2024-05-21 15:46:17.730000 pythonix-1.0.9/pythonix/internals/dict_utils.py
+-rw-r--r--   0        0        0     5075 2024-05-21 14:24:24.050000 pythonix-1.0.9/pythonix/internals/fn.py
+-rw-r--r--   0        0        0    11058 2024-05-19 18:33:10.620000 pythonix-1.0.9/pythonix/internals/grammar.py
+-rw-r--r--   0        0        0    10393 2024-05-17 17:21:29.129631 pythonix-1.0.9/pythonix/internals/op.py
+-rw-r--r--   0        0        0     4844 2024-05-17 17:24:14.659631 pythonix-1.0.9/pythonix/internals/pair.py
+-rw-r--r--   0        0        0     6534 2024-05-21 14:22:43.100000 pythonix-1.0.9/pythonix/internals/pipe.py
+-rw-r--r--   0        0        0     1968 2024-05-18 19:03:33.219631 pythonix-1.0.9/pythonix/internals/prove.py
+-rw-r--r--   0        0        0     7203 2024-05-16 16:50:54.819631 pythonix-1.0.9/pythonix/internals/req.py
+-rw-r--r--   0        0        0    25292 2024-05-21 02:06:29.580000 pythonix-1.0.9/pythonix/internals/res.py
+-rw-r--r--   0        0        0     5041 2024-05-16 19:09:41.649631 pythonix-1.0.9/pythonix/internals/trail.py
+-rw-r--r--   0        0        0     2726 2024-05-16 21:05:40.149631 pythonix-1.0.9/pythonix/internals/tup.py
+-rw-r--r--   0        0        0     1356 2024-05-17 04:15:47.249631 pythonix-1.0.9/pythonix/op.py
+-rw-r--r--   0        0        0      698 2024-05-17 17:26:00.459631 pythonix-1.0.9/pythonix/pair.py
+-rw-r--r--   0        0        0      876 2024-05-17 18:24:21.269631 pythonix-1.0.9/pythonix/pipe.py
+-rw-r--r--   0        0        0      755 2024-05-21 15:50:13.600000 pythonix-1.0.9/pythonix/prelude.py
+-rw-r--r--   0        0        0      210 2024-05-16 16:50:54.639631 pythonix-1.0.9/pythonix/prove.py
+-rw-r--r--   0        0        0      645 2024-05-16 16:24:04.869631 pythonix-1.0.9/pythonix/req.py
+-rw-r--r--   0        0        0     1370 2024-05-21 02:08:25.030000 pythonix-1.0.9/pythonix/res.py
+-rw-r--r--   0        0        0      290 2024-05-16 16:50:54.669631 pythonix-1.0.9/pythonix/trail.py
+-rw-r--r--   0        0        0      358 2024-05-16 16:50:54.679631 pythonix-1.0.9/pythonix/tup.py
+-rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 pythonix-1.0.9/PKG-INFO
```

### Comparing `pythonix-1.0.8/README.md` & `pythonix-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.8/pythonix/internals/prove.py` & `pythonix-1.0.9/pythonix/internals/prove.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,69 @@
-'''Partialized functions for safe and simple assertions
+"""Partialized functions for safe and simple assertions
 
 This module provides ways to perform common assertion patterns like
 equals, type tests, and testing for the presence of elements in data.
 
-Note:
-    All function return values are Ok[None] or Err[AssertionError].
-    Use the res module to handle the outcomes of the assertions.
-'''
+"""
 from typing import Iterable, TypeVar, Callable
 from pythonix.internals.curry import two
 from pythonix.internals.res import safe
 
 Val = TypeVar("Val")
 NewVal = TypeVar("NewVal")
 
 
 @two
 @safe(AssertionError)
 def that(predicate: Callable[[Val], bool], val: Val) -> None:
     """Assert that the provided function is true if given the value.
-    
+
     Note:
         This is useful with a `Do` pipe to check that values match what you expect without
     changing the original value.
 
     Example:
         ```python
         val: int = 10
         is_even = lambda x: x % 2 == 0
         passed_inspection = prove.that(is_even)(val)
         res.unwrap(passed_inspection)
 
         # Bind shorthand
-        Bind(10).do(prove.that(is_even))(q)
+        Bind(10)(prove.that(is_even))(q)
         ```
     """
     assert predicate(val) == True
 
 
 @two
 @safe(AssertionError)
 def equals(left: NewVal, right: Val) -> None:
-    """
-    Assert that two values are equal
+    """Assert that two values are equal.
+
+    Example:
+        ```python
+        expected: int = 10
+        actual: int = 10
+        comparison_result: Res[None, AssertionError] = prove.equals(expected)(actual)
+        res.unwrap(comparison_result)
+        ```
     """
     assert left == right
 
 
 @safe(AssertionError)
 def is_true(val: bool) -> None:
-    """
-    Assert that the provided value is `True`
+    """Assert that the provided value is `True`
+
+    Example:
+        ```python
+        true_value: bool = True
+        comparison_result
+        ```
     """
     assert val == True
 
 
 @two
 @safe(AssertionError)
 def is_an(expected: type[Val], actual: Val) -> None:
```

### Comparing `pythonix-1.0.8/pythonix/internals/req.py` & `pythonix-1.0.9/pythonix/internals/req.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.8/pythonix/internals/trail.py` & `pythonix-1.0.9/pythonix/internals/trail.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.8/pythonix/internals/tup.py` & `pythonix-1.0.9/pythonix/internals/tup.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.8/pythonix/req.py` & `pythonix-1.0.9/pythonix/req.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.8/PKG-INFO` & `pythonix-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonix
-Version: 1.0.8
+Version: 1.0.9
 Summary: Rust and Gleam like functional programming in Python, complete with Results, pipes, and currying
 Author: jhok2013
 Author-email: jhok2013@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

