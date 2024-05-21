# Comparing `tmp/cam_manager-0.1.0.tar.gz` & `tmp/cam_manager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cam_manager-0.1.0.tar", last modified: Mon May 20 15:51:28 2024, max compression
+gzip compressed data, was "cam_manager-0.1.1.tar", last modified: Tue May 21 13:39:22 2024, max compression
```

## Comparing `cam_manager-0.1.0.tar` & `cam_manager-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:28.840441 cam_manager-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-20 15:51:28.840441 cam_manager-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-20 15:51:24.000000 cam_manager-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:28.836440 cam_manager-0.1.0/cam_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 15:51:24.000000 cam_manager-0.1.0/cam_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-20 15:51:24.000000 cam_manager-0.1.0/cam_manager/cam_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:28.840441 cam_manager-0.1.0/cam_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-20 15:51:28.000000 cam_manager-0.1.0/cam_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-20 15:51:28.000000 cam_manager-0.1.0/cam_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:51:28.000000 cam_manager-0.1.0/cam_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 15:51:28.000000 cam_manager-0.1.0/cam_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 15:51:28.000000 cam_manager-0.1.0/cam_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:51:28.840441 cam_manager-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-20 15:51:24.000000 cam_manager-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:39:22.632524 cam_manager-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-21 13:39:22.632524 cam_manager-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-21 13:39:17.000000 cam_manager-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:39:22.632524 cam_manager-0.1.1/cam_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 13:39:17.000000 cam_manager-0.1.1/cam_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-21 13:39:17.000000 cam_manager-0.1.1/cam_manager/cam_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:39:22.632524 cam_manager-0.1.1/cam_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-21 13:39:22.000000 cam_manager-0.1.1/cam_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-21 13:39:22.000000 cam_manager-0.1.1/cam_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:39:22.000000 cam_manager-0.1.1/cam_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 13:39:22.000000 cam_manager-0.1.1/cam_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-21 13:39:22.000000 cam_manager-0.1.1/cam_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:39:22.632524 cam_manager-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-21 13:39:17.000000 cam_manager-0.1.1/setup.py
```

### Comparing `cam_manager-0.1.0/cam_manager/cam_manager.py` & `cam_manager-0.1.1/cam_manager/cam_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,32 @@
 class CamManager:
     def __init__(self):
         """Initialize the CamManager instance."""
 
         self.cams = {}
         self.active_cam_id = None
 
+    def list_available_cams(self) -> list:
+        """
+        List all available camera devices.
+
+        Returns: list: A list of indices of available camera devices.
+        """
+
+        index = 0
+        arr = []
+        while True:
+            cap = cv2.VideoCapture(index, cv2.CAP_DSHOW)
+            if not cap.isOpened(): break
+
+            arr.append(index)
+            cap.release()
+            index += 1
+        return arr
+
     def add_cam(self, cam_id: int) -> None:
         """
         Add a cam by its ID.
 
         Parameters: cam_id (int): The ID of the cam to be added.
         Returns: None
         """
```

### Comparing `cam_manager-0.1.0/setup.py` & `cam_manager-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(
-    version = "0.1.0",
+    version = "0.1.1",
     name = "cam_manager",
     description = "A camera management library to easily handle cameras with OpenCV.",
 
     long_description = open("README.md").read(),
     long_description_content_type = "text/markdown",
 
     author = "snatev",
```

