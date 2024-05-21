# Comparing `tmp/live-cells-py-0.1.1.tar.gz` & `tmp/live-cells-py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "live-cells-py-0.1.1.tar", last modified: Mon May 20 10:15:15 2024, max compression
+gzip compressed data, was "live-cells-py-0.1.2.tar", last modified: Tue May 21 10:51:51 2024, max compression
```

## Comparing `live-cells-py-0.1.1.tar` & `live-cells-py-0.1.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-20 10:15:15.421495 live-cells-py-0.1.1/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1467 2024-04-28 07:59:50.000000 live-cells-py-0.1.1/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)     2547 2024-05-20 10:15:15.421495 live-cells-py-0.1.1/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     2061 2024-05-20 10:06:58.000000 live-cells-py-0.1.1/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-20 10:15:15.417495 live-cells-py-0.1.1/live_cells/
--rw-rw-r--   0 alex      (1000) alex      (1000)      459 2024-05-18 07:08:40.000000 live-cells-py-0.1.1/live_cells/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3059 2024-05-18 08:25:30.000000 live-cells-py-0.1.1/live_cells/boolean.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1353 2024-05-19 07:48:09.000000 live-cells-py-0.1.1/live_cells/cell.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1057 2024-04-25 18:05:02.000000 live-cells-py-0.1.1/live_cells/changes_only_state.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      749 2024-04-22 18:28:23.000000 live-cells-py-0.1.1/live_cells/compute_cell.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2272 2024-04-23 18:32:10.000000 live-cells-py-0.1.1/live_cells/compute_state.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2381 2024-05-18 08:15:52.000000 live-cells-py-0.1.1/live_cells/computed.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1020 2024-05-18 07:10:34.000000 live-cells-py-0.1.1/live_cells/constant_cell.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2261 2024-05-13 17:15:45.000000 live-cells-py-0.1.1/live_cells/dependent_cell.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2387 2024-04-25 18:04:48.000000 live-cells-py-0.1.1/live_cells/dynamic_compute_cell.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2729 2024-05-18 08:18:54.000000 live-cells-py-0.1.1/live_cells/error_handling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      760 2024-05-18 08:31:00.000000 live-cells-py-0.1.1/live_cells/exceptions.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1391 2024-05-13 17:15:59.000000 live-cells-py-0.1.1/live_cells/extension.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      627 2024-05-13 17:22:46.000000 live-cells-py-0.1.1/live_cells/keys.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2628 2024-05-19 12:21:22.000000 live-cells-py-0.1.1/live_cells/maybe.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4995 2024-05-18 07:04:57.000000 live-cells-py-0.1.1/live_cells/mutable_cell.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2063 2024-05-12 11:45:46.000000 live-cells-py-0.1.1/live_cells/numeric.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3485 2024-04-25 18:05:08.000000 live-cells-py-0.1.1/live_cells/observer_state.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1781 2024-05-18 08:26:58.000000 live-cells-py-0.1.1/live_cells/peek_cell.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      900 2024-03-28 08:57:30.000000 live-cells-py-0.1.1/live_cells/persistent_stateful_cell.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7043 2024-05-18 12:27:50.000000 live-cells-py-0.1.1/live_cells/stateful_cell.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2805 2024-05-19 12:13:59.000000 live-cells-py-0.1.1/live_cells/tracking.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5605 2024-05-19 12:23:41.000000 live-cells-py-0.1.1/live_cells/watch.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-20 10:15:15.417495 live-cells-py-0.1.1/live_cells_py.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     2547 2024-05-20 10:15:15.000000 live-cells-py-0.1.1/live_cells_py.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      998 2024-05-20 10:15:15.000000 live-cells-py-0.1.1/live_cells_py.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2024-05-20 10:15:15.000000 live-cells-py-0.1.1/live_cells_py.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2024-05-20 10:15:15.000000 live-cells-py-0.1.1/live_cells_py.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2024-05-20 10:15:15.421495 live-cells-py-0.1.1/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      745 2024-05-20 10:12:18.000000 live-cells-py-0.1.1/setup.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-20 10:15:15.417495 live-cells-py-0.1.1/tests/
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2024-03-27 12:59:32.000000 live-cells-py-0.1.1/tests/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      505 2024-05-19 11:46:14.000000 live-cells-py-0.1.1/tests/conftest.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3789 2024-05-13 17:11:46.000000 live-cells-py-0.1.1/tests/test_boolean.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8570 2024-05-10 11:21:20.000000 live-cells-py-0.1.1/tests/test_computed_cells.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      779 2024-03-27 13:10:42.000000 live-cells-py-0.1.1/tests/test_constant_cells.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7204 2024-05-16 18:32:45.000000 live-cells-py-0.1.1/tests/test_error_handling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6846 2024-03-28 17:31:45.000000 live-cells-py-0.1.1/tests/test_mutable_cell.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5292 2024-05-12 07:30:49.000000 live-cells-py-0.1.1/tests/test_numeric.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11209 2024-05-19 12:08:16.000000 live-cells-py-0.1.1/tests/test_watch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4174 2024-05-16 18:49:53.000000 live-cells-py-0.1.1/tests/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-21 10:51:51.200289 live-cells-py-0.1.2/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1467 2024-04-28 07:59:50.000000 live-cells-py-0.1.2/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)     2547 2024-05-21 10:51:51.200289 live-cells-py-0.1.2/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2061 2024-05-20 10:06:58.000000 live-cells-py-0.1.2/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-21 10:51:51.200289 live-cells-py-0.1.2/live_cells/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      459 2024-05-18 07:08:40.000000 live-cells-py-0.1.2/live_cells/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3059 2024-05-18 08:25:30.000000 live-cells-py-0.1.2/live_cells/boolean.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1353 2024-05-19 07:48:09.000000 live-cells-py-0.1.2/live_cells/cell.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1057 2024-04-25 18:05:02.000000 live-cells-py-0.1.2/live_cells/changes_only_state.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      749 2024-04-22 18:28:23.000000 live-cells-py-0.1.2/live_cells/compute_cell.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2272 2024-04-23 18:32:10.000000 live-cells-py-0.1.2/live_cells/compute_state.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2381 2024-05-18 08:15:52.000000 live-cells-py-0.1.2/live_cells/computed.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1020 2024-05-18 07:10:34.000000 live-cells-py-0.1.2/live_cells/constant_cell.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2261 2024-05-13 17:15:45.000000 live-cells-py-0.1.2/live_cells/dependent_cell.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2387 2024-04-25 18:04:48.000000 live-cells-py-0.1.2/live_cells/dynamic_compute_cell.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2729 2024-05-18 08:18:54.000000 live-cells-py-0.1.2/live_cells/error_handling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      760 2024-05-18 08:31:00.000000 live-cells-py-0.1.2/live_cells/exceptions.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1391 2024-05-13 17:15:59.000000 live-cells-py-0.1.2/live_cells/extension.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      627 2024-05-13 17:22:46.000000 live-cells-py-0.1.2/live_cells/keys.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2628 2024-05-19 12:21:22.000000 live-cells-py-0.1.2/live_cells/maybe.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4995 2024-05-18 07:04:57.000000 live-cells-py-0.1.2/live_cells/mutable_cell.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2063 2024-05-12 11:45:46.000000 live-cells-py-0.1.2/live_cells/numeric.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3485 2024-04-25 18:05:08.000000 live-cells-py-0.1.2/live_cells/observer_state.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1781 2024-05-18 08:26:58.000000 live-cells-py-0.1.2/live_cells/peek_cell.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      900 2024-03-28 08:57:30.000000 live-cells-py-0.1.2/live_cells/persistent_stateful_cell.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7043 2024-05-18 12:27:50.000000 live-cells-py-0.1.2/live_cells/stateful_cell.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3016 2024-05-21 10:50:15.000000 live-cells-py-0.1.2/live_cells/tracking.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5605 2024-05-19 12:23:41.000000 live-cells-py-0.1.2/live_cells/watch.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-21 10:51:51.200289 live-cells-py-0.1.2/live_cells_py.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     2547 2024-05-21 10:51:51.000000 live-cells-py-0.1.2/live_cells_py.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      998 2024-05-21 10:51:51.000000 live-cells-py-0.1.2/live_cells_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2024-05-21 10:51:51.000000 live-cells-py-0.1.2/live_cells_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2024-05-21 10:51:51.000000 live-cells-py-0.1.2/live_cells_py.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2024-05-21 10:51:51.200289 live-cells-py-0.1.2/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)      745 2024-05-21 10:51:22.000000 live-cells-py-0.1.2/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-21 10:51:51.200289 live-cells-py-0.1.2/tests/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2024-03-27 12:59:32.000000 live-cells-py-0.1.2/tests/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      505 2024-05-19 11:46:14.000000 live-cells-py-0.1.2/tests/conftest.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3789 2024-05-13 17:11:46.000000 live-cells-py-0.1.2/tests/test_boolean.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8570 2024-05-10 11:21:20.000000 live-cells-py-0.1.2/tests/test_computed_cells.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      779 2024-03-27 13:10:42.000000 live-cells-py-0.1.2/tests/test_constant_cells.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7204 2024-05-16 18:32:45.000000 live-cells-py-0.1.2/tests/test_error_handling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6846 2024-03-28 17:31:45.000000 live-cells-py-0.1.2/tests/test_mutable_cell.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5292 2024-05-12 07:30:49.000000 live-cells-py-0.1.2/tests/test_numeric.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11209 2024-05-19 12:08:16.000000 live-cells-py-0.1.2/tests/test_watch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4174 2024-05-16 18:49:53.000000 live-cells-py-0.1.2/tests/util.py
```

### Comparing `live-cells-py-0.1.1/LICENSE` & `live-cells-py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/PKG-INFO` & `live-cells-py-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: live-cells-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: A reactive programming library for Python ported from Live Cells for Dart
 Home-page: https://github.com/alex-gutev/live_cells_py
 Author: Alexander Gutev
 Author-email: alex.gutev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `live-cells-py-0.1.1/README.md` & `live-cells-py-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/boolean.py` & `live-cells-py-0.1.2/live_cells/boolean.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/cell.py` & `live-cells-py-0.1.2/live_cells/cell.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/changes_only_state.py` & `live-cells-py-0.1.2/live_cells/changes_only_state.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/compute_cell.py` & `live-cells-py-0.1.2/live_cells/compute_cell.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/compute_state.py` & `live-cells-py-0.1.2/live_cells/compute_state.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/computed.py` & `live-cells-py-0.1.2/live_cells/computed.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/constant_cell.py` & `live-cells-py-0.1.2/live_cells/constant_cell.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/dependent_cell.py` & `live-cells-py-0.1.2/live_cells/dependent_cell.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/dynamic_compute_cell.py` & `live-cells-py-0.1.2/live_cells/dynamic_compute_cell.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/error_handling.py` & `live-cells-py-0.1.2/live_cells/error_handling.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/exceptions.py` & `live-cells-py-0.1.2/live_cells/exceptions.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/extension.py` & `live-cells-py-0.1.2/live_cells/extension.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/keys.py` & `live-cells-py-0.1.2/live_cells/keys.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/maybe.py` & `live-cells-py-0.1.2/live_cells/maybe.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/mutable_cell.py` & `live-cells-py-0.1.2/live_cells/mutable_cell.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/numeric.py` & `live-cells-py-0.1.2/live_cells/numeric.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/observer_state.py` & `live-cells-py-0.1.2/live_cells/observer_state.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/peek_cell.py` & `live-cells-py-0.1.2/live_cells/peek_cell.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/persistent_stateful_cell.py` & `live-cells-py-0.1.2/live_cells/persistent_stateful_cell.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/stateful_cell.py` & `live-cells-py-0.1.2/live_cells/stateful_cell.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells/tracking.py` & `live-cells-py-0.1.2/live_cells/tracking.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,28 +40,37 @@
         """Track the cell `arg` as a dependency.
 
         If a cell dependency tracker, registered with `with_tracker`, is in
         effect it is called with `arg`.
 
         """
 
-        if cls._data.track is not None:
-            return cls._data.track(arg)
+        tracker = cls._tracker
+
+        if tracker is not None:
+            return tracker(arg)
 
         return arg.value
 
+    @classmethod
+    @property
+    def _tracker(cls):
+        """The argument cell tracker callback currently in effect."""
+
+        return cls._data.track if hasattr(cls._data, 'track') else None
+
     def __init__(self, tracker, override=False):
         def track_fn(cell):
             tracker(cell)
             return cell.value
 
         self._tracker = tracker if (override or tracker is None) else track_fn
 
     def __enter__(self):
-        self._previous = ArgumentTracker._data.track
+        self._previous = ArgumentTracker._tracker
         ArgumentTracker._data.track = self._tracker
 
     def __exit__(self, exception_type, exception_value, exception_traceback):
         ArgumentTracker._data.track = self._previous
 
 def with_tracker(tracker):
     """Install a cell dependency `tracker` to be in effect within the decorated function.
```

### Comparing `live-cells-py-0.1.1/live_cells/watch.py` & `live-cells-py-0.1.2/live_cells/watch.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/live_cells_py.egg-info/PKG-INFO` & `live-cells-py-0.1.2/live_cells_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: live-cells-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: A reactive programming library for Python ported from Live Cells for Dart
 Home-page: https://github.com/alex-gutev/live_cells_py
 Author: Alexander Gutev
 Author-email: alex.gutev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `live-cells-py-0.1.1/live_cells_py.egg-info/SOURCES.txt` & `live-cells-py-0.1.2/live_cells_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/setup.py` & `live-cells-py-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Load the long_description from README.md
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='live-cells-py',
-    version='0.1.1',
+    version='0.1.2',
     author='Alexander Gutev',
     author_email='alex.gutev@gmail.com',
     description="A reactive programming library for Python ported from Live Cells for Dart",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alex-gutev/live_cells_py",
     packages=setuptools.find_packages(),
```

### Comparing `live-cells-py-0.1.1/tests/test_boolean.py` & `live-cells-py-0.1.2/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/tests/test_computed_cells.py` & `live-cells-py-0.1.2/tests/test_computed_cells.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/tests/test_constant_cells.py` & `live-cells-py-0.1.2/tests/test_constant_cells.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/tests/test_error_handling.py` & `live-cells-py-0.1.2/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/tests/test_mutable_cell.py` & `live-cells-py-0.1.2/tests/test_mutable_cell.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/tests/test_numeric.py` & `live-cells-py-0.1.2/tests/test_numeric.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/tests/test_watch.py` & `live-cells-py-0.1.2/tests/test_watch.py`

 * *Files identical despite different names*

### Comparing `live-cells-py-0.1.1/tests/util.py` & `live-cells-py-0.1.2/tests/util.py`

 * *Files identical despite different names*

