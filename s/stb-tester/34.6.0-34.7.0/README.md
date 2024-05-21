# Comparing `tmp/stb-tester-34.6.0.tar.gz` & `tmp/stb-tester-34.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stb-tester-34.6.0.tar", last modified: Wed Feb 28 16:12:53 2024, max compression
+gzip compressed data, was "stb-tester-34.7.0.tar", last modified: Tue May 21 12:23:48 2024, max compression
```

## Comparing `stb-tester-34.6.0.tar` & `stb-tester-34.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2024-02-28 16:12:53.887578 stb-tester-34.6.0/
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       80 2023-09-25 09:09:30.000000 stb-tester-34.6.0/MANIFEST.in
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1635 2024-02-28 16:12:53.887578 stb-tester-34.6.0/PKG-INFO
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       38 2024-02-28 16:12:53.887578 stb-tester-34.6.0/setup.cfg
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1852 2024-02-28 16:03:35.000000 stb-tester-34.6.0/setup.py
-drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2024-02-28 16:12:53.887578 stb-tester-34.6.0/stb_tester.egg-info/
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1635 2024-02-28 16:12:53.000000 stb-tester-34.6.0/stb_tester.egg-info/PKG-INFO
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      261 2024-02-28 16:12:53.000000 stb-tester-34.6.0/stb_tester.egg-info/SOURCES.txt
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)        1 2024-02-28 16:12:53.000000 stb-tester-34.6.0/stb_tester.egg-info/dependency_links.txt
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       16 2024-02-28 16:12:53.000000 stb-tester-34.6.0/stb_tester.egg-info/requires.txt
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)        5 2024-02-28 16:12:53.000000 stb-tester-34.6.0/stb_tester.egg-info/top_level.txt
-drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2024-02-28 16:12:53.887578 stb-tester-34.6.0/stbt/
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    44133 2024-02-28 16:10:16.000000 stb-tester-34.6.0/stbt/__init__.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      708 2023-09-25 09:09:30.000000 stb-tester-34.6.0/stbt/audio.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     5889 2023-09-25 09:09:30.000000 stb-tester-34.6.0/stbt/prometheus.py
--rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       73 2023-09-25 09:09:30.000000 stb-tester-34.6.0/stbt/pylint_plugin.py
+drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2024-05-21 12:23:48.964912 stb-tester-34.7.0/
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       80 2023-09-25 09:09:30.000000 stb-tester-34.7.0/MANIFEST.in
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1635 2024-05-21 12:23:48.964912 stb-tester-34.7.0/PKG-INFO
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       38 2024-05-21 12:23:48.964912 stb-tester-34.7.0/setup.cfg
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1852 2024-05-21 12:23:28.000000 stb-tester-34.7.0/setup.py
+drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2024-05-21 12:23:48.964912 stb-tester-34.7.0/stb_tester.egg-info/
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     1635 2024-05-21 12:23:48.000000 stb-tester-34.7.0/stb_tester.egg-info/PKG-INFO
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      261 2024-05-21 12:23:48.000000 stb-tester-34.7.0/stb_tester.egg-info/SOURCES.txt
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)        1 2024-05-21 12:23:48.000000 stb-tester-34.7.0/stb_tester.egg-info/dependency_links.txt
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       16 2024-05-21 12:23:48.000000 stb-tester-34.7.0/stb_tester.egg-info/requires.txt
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)        5 2024-05-21 12:23:48.000000 stb-tester-34.7.0/stb_tester.egg-info/top_level.txt
+drwxrwxr-x   0 drothlis  (1000) drothlis  (1000)        0 2024-05-21 12:23:48.964912 stb-tester-34.7.0/stbt/
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)    45817 2024-05-15 13:08:24.000000 stb-tester-34.7.0/stbt/__init__.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)      708 2023-09-25 09:09:30.000000 stb-tester-34.7.0/stbt/audio.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)     5889 2023-09-25 09:09:30.000000 stb-tester-34.7.0/stbt/prometheus.py
+-rw-rw-r--   0 drothlis  (1000) drothlis  (1000)       73 2023-09-25 09:09:30.000000 stb-tester-34.7.0/stbt/pylint_plugin.py
```

### Comparing `stb-tester-34.6.0/PKG-INFO` & `stb-tester-34.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stb-tester
-Version: 34.6.0
+Version: 34.7.0
 Summary: Automated GUI testing for Set-Top Boxes
 Home-page: https://stb-tester.com
 Author: Stb-tester.com Ltd.
 Author-email: support@stb-tester.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `stb-tester-34.6.0/setup.py` & `stb-tester-34.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 autocompletion, but without a working implementation.
 
 [Stb-tester Platform]: https://stb-tester.com
 """
 
 setuptools.setup(
     name="stb-tester",
-    version="34.6.0",
+    version="34.7.0",
     author="Stb-tester.com Ltd.",
     author_email="support@stb-tester.com",
     description="Automated GUI testing for Set-Top Boxes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://stb-tester.com",
     packages=["stbt"],
```

### Comparing `stb-tester-34.6.0/stb_tester.egg-info/PKG-INFO` & `stb-tester-34.7.0/stb_tester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stb-tester
-Version: 34.6.0
+Version: 34.7.0
 Summary: Automated GUI testing for Set-Top Boxes
 Home-page: https://stb-tester.com
 Author: Stb-tester.com Ltd.
 Author-email: support@stb-tester.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `stb-tester-34.6.0/stbt/__init__.py` & `stb-tester-34.7.0/stbt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     wait_until)
 
 # The following APIs are not open source, and they require the Stb-tester Node
 # hardware to run. This file contains stubs for local installation, to allow
 # IDE linting & autocompletion.
 __all__ = stbt_core.__all__ + [
     "audio_chunks",
+    "AppleTV",
     "AudioChunk",
     "BadSyncPattern",
     "color_diff",
     "detect_pages",
     "find_regions_by_color",
     "find_selection_from_background",
     "FIRST_FRAME_TIME",
@@ -145,14 +146,65 @@
         "`stbt.%s` is a premium API only available to customers of "
         "Stb-tester.com Ltd. It requires *Stb-tester Node* hardware to run. "
         "See https://stb-tester.com for details on products and pricing. "
         "If you are receiving this error on the *Stb-tester Node* hardware "
         "contact support@stb-tester.com for help" % api_name)
 
 
+class AppleTV:
+    """Control an AppleTV device using pyatv.
+
+    `pyatv`_ is an open source tool for controlling Apple TV devices. It uses
+    AirPlay and other network protocols supported by the Apple TV. This class
+    makes it easy to use pyatv in Stb-tester test scripts.
+
+    pyatv has additional dependencies that are not installed by default in the
+    Stb-tester v34 environment. For instructions on how to install these
+    dependencies, and how to configure the Apple TV's IP address, see
+    :doc:`pyatv`.
+
+    .. warning::
+
+        We have done the "integration" work to make pyatv work on the Stb-tester
+        Node, but we are not the authors of pyatv, and we don't provide support
+        for bugs in pyatv itself.
+
+    :param str address:
+        The IP address of the Apple TV device. If not specified, this is read
+        from "device_under_test.ip_address" in your :ref:`node-specific-config`.
+
+    .. _pyatv: https://pyatv.dev/
+    """
+
+    def __init__(self, address: Optional[str] = None):
+        _raise_premium("AppleTV")
+
+    def launch_app(self, name: str):
+        """Launches the specified app.
+
+        :param name: The name or bundle ID of the app (for example "Netflix" or
+            "com.netflix.Netflix").
+        """
+        return
+
+    def list_apps(self) -> dict[str, str]:
+        """Returns a dict of ``id: name`` with all the apps installed on the
+        Apple TV device.
+        """
+        return {}
+
+    def set_text(self, text: str):
+        """Set the text in a focused text field.
+
+        This only works if a text field is currently focused (for example a
+        search or login field).
+        """
+        return
+
+
 class AudioChunk(numpy.ndarray):
     """A sequence of audio samples.
 
     An ``AudioChunk`` object is what you get from `audio_chunks`. It is a
     subclass of `numpy.ndarray`. An ``AudioChunk`` is a 1-D array containing
     audio samples in 32-bit floating point format (`numpy.float32`) between
     -1.0 and 1.0.
```

### Comparing `stb-tester-34.6.0/stbt/audio.py` & `stb-tester-34.7.0/stbt/audio.py`

 * *Files identical despite different names*

### Comparing `stb-tester-34.6.0/stbt/prometheus.py` & `stb-tester-34.7.0/stbt/prometheus.py`

 * *Files identical despite different names*

