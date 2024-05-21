# Comparing `tmp/slist-0.3.7.tar.gz` & `tmp/slist-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slist-0.3.7.tar", max compression
+gzip compressed data, was "slist-0.3.8.tar", max compression
```

## Comparing `slist-0.3.7.tar` & `slist-0.3.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2024-05-21 16:45:58.660165 slist-0.3.7/LICENSE
--rw-r--r--   0        0        0     2692 2024-05-21 16:45:58.660165 slist-0.3.7/README.md
--rw-r--r--   0        0        0     2484 2024-05-21 16:45:58.660165 slist-0.3.7/pyproject.toml
--rw-r--r--   0        0        0    29092 2024-05-21 16:45:58.660165 slist-0.3.7/slist/__init__.py
--rw-r--r--   0        0        0        0 2024-05-21 16:45:58.660165 slist-0.3.7/slist/py.typed
--rw-r--r--   0        0        0     1415 2024-05-21 16:45:58.660165 slist-0.3.7/slist/pydantic_compat.py
--rw-r--r--   0        0        0        0 2024-05-21 16:45:58.660165 slist-0.3.7/tests/__init__.py
--rw-r--r--   0        0        0      429 2024-05-21 16:45:58.660165 slist-0.3.7/tests/test_docs.py
--rw-r--r--   0        0        0      525 2024-05-21 16:45:58.660165 slist-0.3.7/tests/test_mypy.py
--rw-r--r--   0        0        0     8441 2024-05-21 16:45:58.660165 slist-0.3.7/tests/test_slist.py
--rw-r--r--   0        0        0     3625 1970-01-01 00:00:00.000000 slist-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-21 16:48:16.503397 slist-0.3.8/LICENSE
+-rw-r--r--   0        0        0     2692 2024-05-21 16:48:16.503397 slist-0.3.8/README.md
+-rw-r--r--   0        0        0     2484 2024-05-21 16:48:16.503397 slist-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0    29255 2024-05-21 16:48:16.503397 slist-0.3.8/slist/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:48:16.503397 slist-0.3.8/slist/py.typed
+-rw-r--r--   0        0        0     1415 2024-05-21 16:48:16.503397 slist-0.3.8/slist/pydantic_compat.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:48:16.503397 slist-0.3.8/tests/__init__.py
+-rw-r--r--   0        0        0      429 2024-05-21 16:48:16.503397 slist-0.3.8/tests/test_docs.py
+-rw-r--r--   0        0        0      525 2024-05-21 16:48:16.503397 slist-0.3.8/tests/test_mypy.py
+-rw-r--r--   0        0        0     8441 2024-05-21 16:48:16.503397 slist-0.3.8/tests/test_slist.py
+-rw-r--r--   0        0        0     3625 1970-01-01 00:00:00.000000 slist-0.3.8/PKG-INFO
```

### Comparing `slist-0.3.7/LICENSE` & `slist-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `slist-0.3.7/README.md` & `slist-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `slist-0.3.7/pyproject.toml` & `slist-0.3.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "slist"
-version = "0.3.7"
+version = "0.3.8"
 homepage = "https://github.com/thejaminator/slist"
 description = "A typesafe list with more method chaining!"
 authors = ["James Chua <chuajamessh@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `slist-0.3.7/slist/__init__.py` & `slist-0.3.8/slist/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -658,14 +658,18 @@
         for fut in futures:
             results.append(fut.result())
         return Slist(results)
 
     async def par_map_async(self, func: Callable[[A], typing.Awaitable[B]]) -> Slist[B]:
         """Applies the async function to each element. Awaits for all results."""
         return Slist(await asyncio.gather(*[func(item) for item in self]))
+    
+    async def gather(self: Sequence[typing.Awaitable[A]]) -> Slist[A]:
+        """Awaits for all results"""
+        return Slist(await asyncio.gather(*self))
 
     def filter_text_search(self, key: Callable[[A], str], search: List[str]) -> Slist[A]:
         """Filters a list of text with text terms"""
 
         def matches_search(text: str) -> bool:
             if search:
                 search_regex = re.compile("|".join(search), re.IGNORECASE)
```

### Comparing `slist-0.3.7/slist/pydantic_compat.py` & `slist-0.3.8/slist/pydantic_compat.py`

 * *Files identical despite different names*

### Comparing `slist-0.3.7/tests/test_mypy.py` & `slist-0.3.8/tests/test_mypy.py`

 * *Files identical despite different names*

### Comparing `slist-0.3.7/tests/test_slist.py` & `slist-0.3.8/tests/test_slist.py`

 * *Files identical despite different names*

### Comparing `slist-0.3.7/PKG-INFO` & `slist-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slist
-Version: 0.3.7
+Version: 0.3.8
 Summary: A typesafe list with more method chaining!
 Home-page: https://github.com/thejaminator/slist
 License: MIT
 Author: James Chua
 Author-email: chuajamessh@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

