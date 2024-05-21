# Comparing `tmp/snippet-uiautomator-1.1.0.tar.gz` & `tmp/snippet-uiautomator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snippet-uiautomator-1.1.0.tar", last modified: Thu Mar 14 04:31:53 2024, max compression
+gzip compressed data, was "snippet-uiautomator-1.1.1.tar", last modified: Tue May 21 19:04:47 2024, max compression
```

## Comparing `snippet-uiautomator-1.1.0.tar` & `snippet-uiautomator-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 kolinlu  (523743) primarygroup (89939)        0 2024-03-14 04:31:53.089990 snippet-uiautomator-1.1.0/
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)    11358 2024-03-14 04:13:41.000000 snippet-uiautomator-1.1.0/LICENSE
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)    16244 2024-03-14 04:31:53.085990 snippet-uiautomator-1.1.0/PKG-INFO
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     2981 2024-03-14 04:13:41.000000 snippet-uiautomator-1.1.0/README.md
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)      539 2024-03-14 04:21:50.000000 snippet-uiautomator-1.1.0/pyproject.toml
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)       38 2024-03-14 04:31:53.089990 snippet-uiautomator-1.1.0/setup.cfg
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     1161 2024-03-14 04:21:59.000000 snippet-uiautomator-1.1.0/setup.py
-drwxr-xr-x   0 kolinlu  (523743) primarygroup (89939)        0 2024-03-14 04:31:53.081990 snippet-uiautomator-1.1.0/snippet_uiautomator/
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)      575 2024-03-14 04:13:41.000000 snippet-uiautomator-1.1.0/snippet_uiautomator/__init__.py
-drwxr-xr-x   0 kolinlu  (523743) primarygroup (89939)        0 2024-03-14 04:31:53.077990 snippet-uiautomator-1.1.0/snippet_uiautomator/android/
-drwxr-xr-x   0 kolinlu  (523743) primarygroup (89939)        0 2024-03-14 04:31:53.085990 snippet-uiautomator-1.1.0/snippet_uiautomator/android/app/
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)  2234057 2024-03-14 04:17:37.000000 snippet-uiautomator-1.1.0/snippet_uiautomator/android/app/uiautomator.apk
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     2914 2024-03-14 04:13:41.000000 snippet-uiautomator-1.1.0/snippet_uiautomator/byselector.py
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     5014 2024-03-14 04:13:41.000000 snippet-uiautomator-1.1.0/snippet_uiautomator/configurator.py
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     9025 2024-03-14 04:13:41.000000 snippet-uiautomator-1.1.0/snippet_uiautomator/constants.py
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     2376 2024-03-14 04:13:41.000000 snippet-uiautomator-1.1.0/snippet_uiautomator/errors.py
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     9044 2024-03-14 04:13:41.000000 snippet-uiautomator-1.1.0/snippet_uiautomator/uiautomator.py
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)    12986 2024-03-14 04:13:41.000000 snippet-uiautomator-1.1.0/snippet_uiautomator/uidevice.py
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)    22494 2024-03-14 04:13:41.000000 snippet-uiautomator-1.1.0/snippet_uiautomator/uiobject2.py
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     5390 2024-03-14 04:13:41.000000 snippet-uiautomator-1.1.0/snippet_uiautomator/uiwatcher.py
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     2464 2024-03-14 04:13:41.000000 snippet-uiautomator-1.1.0/snippet_uiautomator/utils.py
-drwxr-xr-x   0 kolinlu  (523743) primarygroup (89939)        0 2024-03-14 04:31:53.085990 snippet-uiautomator-1.1.0/snippet_uiautomator.egg-info/
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)    16244 2024-03-14 04:31:52.000000 snippet-uiautomator-1.1.0/snippet_uiautomator.egg-info/PKG-INFO
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)      630 2024-03-14 04:31:53.000000 snippet-uiautomator-1.1.0/snippet_uiautomator.egg-info/SOURCES.txt
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)        1 2024-03-14 04:31:52.000000 snippet-uiautomator-1.1.0/snippet_uiautomator.egg-info/dependency_links.txt
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)       14 2024-03-14 04:31:52.000000 snippet-uiautomator-1.1.0/snippet_uiautomator.egg-info/requires.txt
--rw-r--r--   0 kolinlu  (523743) primarygroup (89939)       20 2024-03-14 04:31:52.000000 snippet-uiautomator-1.1.0/snippet_uiautomator.egg-info/top_level.txt
+drwxr-xr-x   0 kolinlu  (523743) primarygroup (89939)        0 2024-05-21 19:04:47.163567 snippet-uiautomator-1.1.1/
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)    11358 2024-05-21 16:38:53.000000 snippet-uiautomator-1.1.1/LICENSE
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)    16244 2024-05-21 19:04:47.163567 snippet-uiautomator-1.1.1/PKG-INFO
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     2981 2024-05-21 16:38:53.000000 snippet-uiautomator-1.1.1/README.md
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)      539 2024-05-21 19:03:08.000000 snippet-uiautomator-1.1.1/pyproject.toml
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)       38 2024-05-21 19:04:47.163567 snippet-uiautomator-1.1.1/setup.cfg
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     1161 2024-05-21 19:03:46.000000 snippet-uiautomator-1.1.1/setup.py
+drwxr-xr-x   0 kolinlu  (523743) primarygroup (89939)        0 2024-05-21 19:04:47.159567 snippet-uiautomator-1.1.1/snippet_uiautomator/
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)      575 2024-05-21 16:38:53.000000 snippet-uiautomator-1.1.1/snippet_uiautomator/__init__.py
+drwxr-xr-x   0 kolinlu  (523743) primarygroup (89939)        0 2024-05-21 19:04:47.155567 snippet-uiautomator-1.1.1/snippet_uiautomator/android/
+drwxr-xr-x   0 kolinlu  (523743) primarygroup (89939)        0 2024-05-21 19:04:47.159567 snippet-uiautomator-1.1.1/snippet_uiautomator/android/app/
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)  2233992 2024-05-21 16:38:53.000000 snippet-uiautomator-1.1.1/snippet_uiautomator/android/app/uiautomator.apk
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     2914 2024-05-21 16:38:53.000000 snippet-uiautomator-1.1.1/snippet_uiautomator/byselector.py
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     5014 2024-05-21 16:38:53.000000 snippet-uiautomator-1.1.1/snippet_uiautomator/configurator.py
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     9025 2024-05-21 16:38:53.000000 snippet-uiautomator-1.1.1/snippet_uiautomator/constants.py
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     2376 2024-05-21 16:38:53.000000 snippet-uiautomator-1.1.1/snippet_uiautomator/errors.py
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     9044 2024-05-21 16:38:53.000000 snippet-uiautomator-1.1.1/snippet_uiautomator/uiautomator.py
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)    12986 2024-05-21 16:38:53.000000 snippet-uiautomator-1.1.1/snippet_uiautomator/uidevice.py
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)    22486 2024-05-21 16:38:53.000000 snippet-uiautomator-1.1.1/snippet_uiautomator/uiobject2.py
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     5390 2024-05-21 16:38:53.000000 snippet-uiautomator-1.1.1/snippet_uiautomator/uiwatcher.py
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)     2464 2024-05-21 16:38:53.000000 snippet-uiautomator-1.1.1/snippet_uiautomator/utils.py
+drwxr-xr-x   0 kolinlu  (523743) primarygroup (89939)        0 2024-05-21 19:04:47.159567 snippet-uiautomator-1.1.1/snippet_uiautomator.egg-info/
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)    16244 2024-05-21 19:04:47.000000 snippet-uiautomator-1.1.1/snippet_uiautomator.egg-info/PKG-INFO
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)      630 2024-05-21 19:04:47.000000 snippet-uiautomator-1.1.1/snippet_uiautomator.egg-info/SOURCES.txt
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)        1 2024-05-21 19:04:47.000000 snippet-uiautomator-1.1.1/snippet_uiautomator.egg-info/dependency_links.txt
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)       14 2024-05-21 19:04:47.000000 snippet-uiautomator-1.1.1/snippet_uiautomator.egg-info/requires.txt
+-rw-r--r--   0 kolinlu  (523743) primarygroup (89939)       20 2024-05-21 19:04:47.000000 snippet-uiautomator-1.1.1/snippet_uiautomator.egg-info/top_level.txt
```

### Comparing `snippet-uiautomator-1.1.0/LICENSE` & `snippet-uiautomator-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snippet-uiautomator-1.1.0/PKG-INFO` & `snippet-uiautomator-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snippet-uiautomator
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python wrapper for Android UI Automator
 Home-page: https://github.com/google/snippet-uiautomator
 Author: Google Inc.
 Author-email: kolinlu@google.com
 Maintainer-email: Kolin Lu <kolinlu@google.com>
 License: 
                                          Apache License
```

### Comparing `snippet-uiautomator-1.1.0/README.md` & `snippet-uiautomator-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `snippet-uiautomator-1.1.0/pyproject.toml` & `snippet-uiautomator-1.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "snippet-uiautomator"
 description = "A Python wrapper for Android UI Automator"
 authors = [{ name = "Google Inc." }]
 maintainers = [{ name = "Kolin Lu", email = "kolinlu@google.com" }]
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.7"
-version = "1.1.0"
+version = "1.1.1"
 dependencies = [
     'mobly>=1.12.2',
 ]
 
 [tool.pytest.ini_options]
 addopts = "--cov=snippet_uiautomator --cov-report html"
 pythonpath = "."
```

### Comparing `snippet-uiautomator-1.1.0/setup.py` & `snippet-uiautomator-1.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """Installs Snippet UiAutomator."""
 
 import setuptools
 
 setuptools.setup(
     name='snippet-uiautomator',
-    version='1.1.0',
+    version='1.1.1',
     author='Kolin Lu',
     author_email='kolinlu@google.com',
     description='A Python wrapper for UiAutomator based on Mobly Snippet Lib.',
     license='Apache2.0',
     url='https://github.com/google/snippet-uiautomator',
     packages=['snippet_uiautomator'],
     package_data={'snippet_uiautomator': ['android/app/uiautomator.apk']},
```

### Comparing `snippet-uiautomator-1.1.0/snippet_uiautomator/__init__.py` & `snippet-uiautomator-1.1.1/snippet_uiautomator/__init__.py`

 * *Files identical despite different names*

### Comparing `snippet-uiautomator-1.1.0/snippet_uiautomator/byselector.py` & `snippet-uiautomator-1.1.1/snippet_uiautomator/byselector.py`

 * *Files identical despite different names*

### Comparing `snippet-uiautomator-1.1.0/snippet_uiautomator/configurator.py` & `snippet-uiautomator-1.1.1/snippet_uiautomator/configurator.py`

 * *Files identical despite different names*

### Comparing `snippet-uiautomator-1.1.0/snippet_uiautomator/constants.py` & `snippet-uiautomator-1.1.1/snippet_uiautomator/constants.py`

 * *Files identical despite different names*

### Comparing `snippet-uiautomator-1.1.0/snippet_uiautomator/errors.py` & `snippet-uiautomator-1.1.1/snippet_uiautomator/errors.py`

 * *Files identical despite different names*

### Comparing `snippet-uiautomator-1.1.0/snippet_uiautomator/uiautomator.py` & `snippet-uiautomator-1.1.1/snippet_uiautomator/uiautomator.py`

 * *Files identical despite different names*

### Comparing `snippet-uiautomator-1.1.0/snippet_uiautomator/uidevice.py` & `snippet-uiautomator-1.1.1/snippet_uiautomator/uidevice.py`

 * *Files identical despite different names*

### Comparing `snippet-uiautomator-1.1.0/snippet_uiautomator/uiobject2.py` & `snippet-uiautomator-1.1.1/snippet_uiautomator/uiobject2.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,28 +232,28 @@
       self,
       ui: snippet_client_v2.SnippetClientV2,
       selector: byselector.BySelector,
   ) -> None:
     self._ui = ui
     self._selector = selector
 
-  def close(self, percent: float, speed: Optional[int] = None) -> bool:
+  def close(self, percent: int, speed: Optional[int] = None) -> bool:
     """Performs a pinch close gesture on this object.
 
     Args:
       percent: The size of the pinch as a percentage of this object's size.
       speed: The speed at which to perform this gesture in pixels per second.
 
     Returns:
       True if operation succeeds, False otherwise.
     """
     selector_dict = self._selector.to_dict()
     return self._ui.pinchClose(selector_dict, percent, speed)
 
-  def open(self, percent: float, speed: Optional[int] = None) -> bool:
+  def open(self, percent: int, speed: Optional[int] = None) -> bool:
     """Performs a pinch open gesture on this object.
 
     Args:
       percent: The size of the pinch as a percentage of this object's size.
       speed: The speed at which to perform this gesture in pixels per second.
 
     Returns:
@@ -271,15 +271,15 @@
 
     def __init__(
         self,
         ui: snippet_client_v2.SnippetClientV2,
         selector: byselector.BySelector,
         direction: str,
         margin: Optional[int],
-        percent: Optional[float],
+        percent: Optional[int],
     ) -> None:
       self._ui = ui
       self._device = self._ui._device  # pylint: disable=protected-access
       self._selector = selector
       self._direction = direction
       self._margin = margin
       self._percent = percent
@@ -347,15 +347,15 @@
     self._ui = ui
     self._device = self._ui._device  # pylint: disable=protected-access
     self._selector = selector
     self._margin = None
     self._percent = None
 
   def __call__(
-      self, margin: Optional[int] = None, percent: Optional[float] = None
+      self, margin: Optional[int] = None, percent: Optional[int] = None
   ) -> _Scroll:
     """Sets the margins used for scroll gesture."""
     if margin is not None and percent is not None:
       raise errors.ApiError(
           'Pixel-based and percentage-based margin cannot be mixed',
           self._device,
       )
```

### Comparing `snippet-uiautomator-1.1.0/snippet_uiautomator/uiwatcher.py` & `snippet-uiautomator-1.1.1/snippet_uiautomator/uiwatcher.py`

 * *Files identical despite different names*

### Comparing `snippet-uiautomator-1.1.0/snippet_uiautomator/utils.py` & `snippet-uiautomator-1.1.1/snippet_uiautomator/utils.py`

 * *Files identical despite different names*

### Comparing `snippet-uiautomator-1.1.0/snippet_uiautomator.egg-info/PKG-INFO` & `snippet-uiautomator-1.1.1/snippet_uiautomator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snippet-uiautomator
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python wrapper for Android UI Automator
 Home-page: https://github.com/google/snippet-uiautomator
 Author: Google Inc.
 Author-email: kolinlu@google.com
 Maintainer-email: Kolin Lu <kolinlu@google.com>
 License: 
                                          Apache License
```

### Comparing `snippet-uiautomator-1.1.0/snippet_uiautomator.egg-info/SOURCES.txt` & `snippet-uiautomator-1.1.1/snippet_uiautomator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

