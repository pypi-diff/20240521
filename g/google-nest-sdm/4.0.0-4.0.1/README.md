# Comparing `tmp/google_nest_sdm-4.0.0.tar.gz` & `tmp/google_nest_sdm-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_nest_sdm-4.0.0.tar", last modified: Sun May 12 21:07:25 2024, max compression
+gzip compressed data, was "google_nest_sdm-4.0.1.tar", last modified: Tue May 21 05:24:11 2024, max compression
```

## Comparing `google_nest_sdm-4.0.0.tar` & `google_nest_sdm-4.0.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:07:25.915898 google_nest_sdm-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-12 21:07:25.915898 google_nest_sdm-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:07:25.911898 google_nest_sdm-4.0.0/google_nest_sdm/
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/camera_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/device_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/device_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/doorbell_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    15691 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    28495 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/event_media.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/google_nest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/google_nest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22767 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/google_nest_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/thermostat_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/transcoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:07:25.915898 google_nest_sdm-4.0.0/google_nest_sdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-12 21:07:25.000000 google_nest_sdm-4.0.0/google_nest_sdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-12 21:07:25.000000 google_nest_sdm-4.0.0/google_nest_sdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 21:07:25.000000 google_nest_sdm-4.0.0/google_nest_sdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-12 21:07:25.000000 google_nest_sdm-4.0.0/google_nest_sdm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-12 21:07:25.000000 google_nest_sdm-4.0.0/google_nest_sdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-12 21:07:25.000000 google_nest_sdm-4.0.0/google_nest_sdm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-12 21:07:25.915898 google_nest_sdm-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:07:25.915898 google_nest_sdm-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_camera_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    23950 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_device_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_device_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_doorbell_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    19502 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    67768 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_event_media.py
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_google_nest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_google_nest_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_thermostat_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_transcoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:24:11.442710 google_nest_sdm-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-21 05:24:11.442710 google_nest_sdm-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:24:11.438710 google_nest_sdm-4.0.1/google_nest_sdm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/camera_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/device_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/doorbell_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15691 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28495 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/event_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/google_nest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/google_nest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23041 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/google_nest_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/thermostat_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/google_nest_sdm/transcoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:24:11.442710 google_nest_sdm-4.0.1/google_nest_sdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-21 05:24:11.000000 google_nest_sdm-4.0.1/google_nest_sdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-21 05:24:11.000000 google_nest_sdm-4.0.1/google_nest_sdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 05:24:11.000000 google_nest_sdm-4.0.1/google_nest_sdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-21 05:24:11.000000 google_nest_sdm-4.0.1/google_nest_sdm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-21 05:24:11.000000 google_nest_sdm-4.0.1/google_nest_sdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 05:24:11.000000 google_nest_sdm-4.0.1/google_nest_sdm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-21 05:24:11.442710 google_nest_sdm-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:24:11.442710 google_nest_sdm-4.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/tests/test_camera_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23950 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/tests/test_device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/tests/test_device_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/tests/test_doorbell_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19502 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67768 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/tests/test_event_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/tests/test_google_nest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28764 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/tests/test_google_nest_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/tests/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/tests/test_thermostat_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-21 05:24:02.000000 google_nest_sdm-4.0.1/tests/test_transcoder.py
```

### Comparing `google_nest_sdm-4.0.0/LICENSE` & `google_nest_sdm-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/PKG-INFO` & `google_nest_sdm-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google_nest_sdm
-Version: 4.0.0
+Version: 4.0.1
 Summary: Library for the Google Nest SDM API
 Home-page: https://github.com/allenporter/python-google_nest_sdm
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.11
```

### Comparing `google_nest_sdm-4.0.0/README.md` & `google_nest_sdm-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/__init__.py` & `google_nest_sdm-4.0.1/google_nest_sdm/__init__.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/auth.py` & `google_nest_sdm-4.0.1/google_nest_sdm/auth.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/camera_traits.py` & `google_nest_sdm-4.0.1/google_nest_sdm/camera_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/device.py` & `google_nest_sdm-4.0.1/google_nest_sdm/device.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/device_manager.py` & `google_nest_sdm-4.0.1/google_nest_sdm/device_manager.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/device_traits.py` & `google_nest_sdm-4.0.1/google_nest_sdm/device_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/diagnostics.py` & `google_nest_sdm-4.0.1/google_nest_sdm/diagnostics.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/doorbell_traits.py` & `google_nest_sdm-4.0.1/google_nest_sdm/doorbell_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/event.py` & `google_nest_sdm-4.0.1/google_nest_sdm/event.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/event_media.py` & `google_nest_sdm-4.0.1/google_nest_sdm/event_media.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/exceptions.py` & `google_nest_sdm-4.0.1/google_nest_sdm/exceptions.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/google_nest.py` & `google_nest_sdm-4.0.1/google_nest_sdm/google_nest.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/google_nest_api.py` & `google_nest_sdm-4.0.1/google_nest_sdm/google_nest_api.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/google_nest_subscriber.py` & `google_nest_sdm-4.0.1/google_nest_sdm/google_nest_subscriber.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,16 @@
 WATCHDOG_RESTART_DELAY_MIN_SECONDS = 10
 WATCHDOG_RESTART_DELAY_MAX_SECONDS = 300
 # Reset watchdog backoff
 WATCHDOG_RESET_THRESHOLD_SECONDS = 60
 
 DEFAULT_MESSAGE_RETENTION_SECONDS = 15 * 60  # 15 minutes
 
+MESSAGE_ACK_TIMEOUT_SECONDS = 30.0
+
 # Note: Users of non-prod instances will have to manually configure a topic
 TOPIC_FORMAT = "projects/sdm-prod/topics/enterprise-{project_id}"
 
 OAUTH2_AUTHORIZE_FORMAT = (
     "https://nestservices.google.com/partnerconnections/{project_id}/auth"
 )
 OAUTH2_TOKEN = "https://www.googleapis.com/oauth2/v4/token"
@@ -195,22 +197,21 @@
         subscription_name: str,
         topic_name: str,
         loop: asyncio.AbstractEventLoop,
     ) -> None:
         """Creates a subscription name if it does not already exist."""
         _validate_subscription_name(subscription_name)
         _validate_topic_name(topic_name)
-        with concurrent.futures.ThreadPoolExecutor(max_workers=1) as executor:
-            await loop.run_in_executor(
-                executor,
-                self._create_subscription,
-                creds,
-                subscription_name,
-                topic_name,
-            )
+        await loop.run_in_executor(
+            None,
+            self._create_subscription,
+            creds,
+            subscription_name,
+            topic_name,
+        )
 
     def _create_subscription(
         self,
         creds: Credentials,
         subscription_name: str,
         topic_name: str,
     ) -> None:
@@ -246,21 +247,20 @@
     async def async_delete_subscription(
         self,
         creds: Credentials,
         subscription_name: str,
         loop: asyncio.AbstractEventLoop,
     ) -> None:
         """Creates a subscription name if it does not already exist."""
-        with concurrent.futures.ThreadPoolExecutor(max_workers=1) as executor:
-            await loop.run_in_executor(
-                executor,
-                self._delete_subscription,
-                creds,
-                subscription_name,
-            )
+        await loop.run_in_executor(
+            None,
+            self._delete_subscription,
+            creds,
+            subscription_name,
+        )
 
     def _delete_subscription(
         self,
         creds: Credentials,
         subscription_name: str,
     ) -> None:
         """Deletes a subscription."""
@@ -277,29 +277,26 @@
         async_callback: Callable[
             [pubsub_v1.subscriber.message.Message], Awaitable[None]
         ],
     ) -> pubsub_v1.subscriber.futures.StreamingPullFuture:
         """Create a new subscriber with a blocking to async bridge."""
 
         def callback_wrapper(message: pubsub_v1.subscriber.message.Message) -> None:
-            if loop.is_closed():
-                return
             future: concurrent.futures.Future = asyncio.run_coroutine_threadsafe(
                 async_callback(message), loop
             )
             future.result()
 
-        with concurrent.futures.ThreadPoolExecutor(max_workers=1) as executor:
-            return await loop.run_in_executor(
-                executor,
-                self._new_subscriber,
-                creds,
-                subscription_name,
-                callback_wrapper,
-            )
+        return await loop.run_in_executor(
+            None,
+            self._new_subscriber,
+            creds,
+            subscription_name,
+            callback_wrapper,
+        )
 
     def _new_subscriber(
         self,
         creds: Credentials,
         subscription_name: str,
         callback_wrapper: Callable[[pubsub_v1.subscriber.message.Message], None],
     ) -> pubsub_v1.subscriber.futures.StreamingPullFuture:
@@ -331,15 +328,15 @@
         watchdog_restart_delay_min_seconds: float = WATCHDOG_RESTART_DELAY_MIN_SECONDS,
     ):
         """Initialize the subscriber for the specified topic."""
         self._auth = auth
         self._subscriber_id = subscriber_id
         self._project_id = project_id
         self._api = GoogleNestAPI(auth, project_id)
-        self._loop = loop or asyncio.get_event_loop()
+        self._loop = loop or asyncio.get_running_loop()
         self._device_manager_task: asyncio.Task[DeviceManager] | None = None
         self._subscriber_factory = subscriber_factory
         self._subscriber_future: (
             pubsub_v1.subscriber.futures.StreamingPullFuture | None
         ) = None  # noqa: E501
         self._callback: Callable[[EventMessage], Awaitable[None]] | None = None
         self._healthy = True
@@ -433,15 +430,15 @@
         except ClientError as err:
             DIAGNOSTICS.increment("start.creds_error")
             raise AuthException(f"Access token failure: {err}") from err
 
         try:
             self._subscriber_future = (
                 await self._subscriber_factory.async_new_subscriber(
-                    creds, self._subscriber_id, self._loop, self._async_message_callback
+                    creds, self._subscriber_id, self._loop, self._async_message_callback_with_timeout
                 )
             )
         except NotFound as err:
             DIAGNOSTICS.increment("start.not_found_error")
             raise ConfigurationException(
                 f"Failed to create subscriber '{self._subscriber_id}' id was not found"
             ) from err
@@ -527,14 +524,27 @@
         """Teardown subscriber."""
         if future.exception():
             ex = future.exception()
             if self._healthy:
                 self._healthy = False
             _LOGGER.debug("Subscriber disconnected, will restart: %s: %s", type(ex), ex)
 
+    async def _async_message_callback_with_timeout(
+        self, message: pubsub_v1.subscriber.message.Message
+    ) -> None:
+        """Handle a received message."""
+        try:
+            async with asyncio.timeout(MESSAGE_ACK_TIMEOUT_SECONDS):
+                print("Async message callback with timeout, ", MESSAGE_ACK_TIMEOUT_SECONDS)
+                await self._async_message_callback(message)
+                print("Done")
+        except TimeoutError as err:
+            DIAGNOSTICS.increment("message_ack_timeout")
+            raise TimeoutError("Message ack timeout processing message") from err
+
     async def _async_message_callback(
         self, message: pubsub_v1.subscriber.message.Message
     ) -> None:
         """Handle a received message."""
         payload = json.loads(bytes.decode(message.data))
         event = EventMessage.create_event(payload, self._auth)
         recv = time.time()
```

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/model.py` & `google_nest_sdm-4.0.1/google_nest_sdm/model.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/registry.py` & `google_nest_sdm-4.0.1/google_nest_sdm/registry.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/structure.py` & `google_nest_sdm-4.0.1/google_nest_sdm/structure.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/thermostat_traits.py` & `google_nest_sdm-4.0.1/google_nest_sdm/thermostat_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/traits.py` & `google_nest_sdm-4.0.1/google_nest_sdm/traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm/transcoder.py` & `google_nest_sdm-4.0.1/google_nest_sdm/transcoder.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm.egg-info/PKG-INFO` & `google_nest_sdm-4.0.1/google_nest_sdm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google_nest_sdm
-Version: 4.0.0
+Version: 4.0.1
 Summary: Library for the Google Nest SDM API
 Home-page: https://github.com/allenporter/python-google_nest_sdm
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.11
```

### Comparing `google_nest_sdm-4.0.0/google_nest_sdm.egg-info/SOURCES.txt` & `google_nest_sdm-4.0.1/google_nest_sdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/pyproject.toml` & `google_nest_sdm-4.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/setup.cfg` & `google_nest_sdm-4.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = google_nest_sdm
-version = 4.0.0
+version = 4.0.1
 description = Library for the Google Nest SDM API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/python-google_nest_sdm
 author = Allen Porter
 author_email = allen.porter@gmail.com
 license = Apache-2.0
```

### Comparing `google_nest_sdm-4.0.0/tests/test_auth.py` & `google_nest_sdm-4.0.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/tests/test_camera_traits.py` & `google_nest_sdm-4.0.1/tests/test_camera_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/tests/test_device.py` & `google_nest_sdm-4.0.1/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/tests/test_device_manager.py` & `google_nest_sdm-4.0.1/tests/test_device_manager.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/tests/test_device_traits.py` & `google_nest_sdm-4.0.1/tests/test_device_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/tests/test_doorbell_traits.py` & `google_nest_sdm-4.0.1/tests/test_doorbell_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/tests/test_event.py` & `google_nest_sdm-4.0.1/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/tests/test_event_media.py` & `google_nest_sdm-4.0.1/tests/test_event_media.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/tests/test_google_nest_api.py` & `google_nest_sdm-4.0.1/tests/test_google_nest_api.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/tests/test_google_nest_subscriber.py` & `google_nest_sdm-4.0.1/tests/test_google_nest_subscriber.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 import json
 from typing import Any, Awaitable, Callable, Dict, Optional
-from unittest.mock import create_autospec, Mock
+from unittest.mock import create_autospec, Mock, patch
 
 import aiohttp
 import pytest
 from google.auth.exceptions import RefreshError, GoogleAuthError, TransportError
 from google.api_core.exceptions import ClientError, Unauthenticated
 from google.cloud import pubsub_v1
 from google.oauth2.credentials import Credentials
@@ -635,14 +635,64 @@
     events = message.event_sessions["CjY5Y3VKaTZwR3o4Y19YbTVfMF..."]
     assert len(events) == 1
     assert "sdm.devices.events.CameraPerson.Person" in events
 
     subscriber.stop_async()
 
 
+async def test_message_ack_timeout(
+    app: aiohttp.web.Application,
+    device_handler: DeviceHandler,
+    structure_handler: StructureHandler,
+    subscriber_factory: FakeSubscriberFactory,
+    subscriber_client: Callable[
+        [Optional[AbstractSubscriberFactory]], Awaitable[GoogleNestSubscriber]
+    ],
+    fake_event_message: Callable[[Dict[str, Any]], EventMessage],
+) -> None:
+
+    device_id = device_handler.add_device(
+        traits={
+            "sdm.devices.traits.Connectivity": {
+                "status": "ONLINE",
+            },
+        }
+    )
+    structure_id = structure_handler.add_structure()
+
+    subscriber = await subscriber_client(subscriber_factory)
+    subscriber.cache_policy.event_cache_size = 5
+    await subscriber.start_async()
+    device_manager = await subscriber.async_get_device_manager()
+    devices = device_manager.devices
+    assert device_id in devices
+
+    async def async_handle_event(_: Any) -> None:
+        await asyncio.sleep(10)
+
+    subscriber.set_update_callback(async_handle_event)
+    event = {
+        "eventId": "0120ecc7-3b57-4eb4-9941-91609f189fb4",
+        "timestamp": "2019-01-01T00:00:01Z",
+        "relationUpdate": {
+            "type": "CREATED",
+            "subject": structure_id,
+            "object": device_id,
+        },
+        "userId": "AVPHwEuBfnPOnTqzVFT4IONX2Qqhu9EJ4ubO-bNnQ-yi",
+    }
+    with patch(
+        "google_nest_sdm.google_nest_subscriber.MESSAGE_ACK_TIMEOUT_SECONDS", 0.01
+    ):
+        with pytest.raises(TimeoutError, match="Message ack timeout"):
+            await subscriber_factory.async_push_event(event)
+
+    subscriber.stop_async()
+
+
 async def test_refresh_hack_on_invalid_thermostat_traits(
     app: aiohttp.web.Application,
     device_handler: DeviceHandler,
     structure_handler: StructureHandler,
     subscriber_client: Callable[[], Awaitable[GoogleNestSubscriber]],
     subscriber_factory: FakeSubscriberFactory,
 ) -> None:
```

### Comparing `google_nest_sdm-4.0.0/tests/test_structure.py` & `google_nest_sdm-4.0.1/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/tests/test_thermostat_traits.py` & `google_nest_sdm-4.0.1/tests/test_thermostat_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.0/tests/test_transcoder.py` & `google_nest_sdm-4.0.1/tests/test_transcoder.py`

 * *Files identical despite different names*

