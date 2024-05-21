# Comparing `tmp/pygame_canvas-1.4.2.tar.gz` & `tmp/pygame_canvas-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_canvas-1.4.2.tar", last modified: Tue May 21 14:45:50 2024, max compression
+gzip compressed data, was "pygame_canvas-1.4.3.tar", last modified: Tue May 21 14:49:21 2024, max compression
```

## Comparing `pygame_canvas-1.4.2.tar` & `pygame_canvas-1.4.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 14:45:50.026221 pygame_canvas-1.4.2/
--rw-rw-rw-   0        0        0     1881 2024-05-21 14:45:50.024681 pygame_canvas-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     1638 2024-05-21 14:32:25.000000 pygame_canvas-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 14:45:50.023159 pygame_canvas-1.4.2/pygame_canvas.egg-info/
--rw-rw-rw-   0        0        0     1881 2024-05-21 14:45:49.000000 pygame_canvas-1.4.2/pygame_canvas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-05-21 14:45:49.000000 pygame_canvas-1.4.2/pygame_canvas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:45:49.000000 pygame_canvas-1.4.2/pygame_canvas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 14:45:49.000000 pygame_canvas-1.4.2/pygame_canvas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:45:49.000000 pygame_canvas-1.4.2/pygame_canvas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2024-05-21 13:50:24.000000 pygame_canvas-1.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 14:45:50.026221 pygame_canvas-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      520 2024-05-21 14:45:38.000000 pygame_canvas-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:49:21.239526 pygame_canvas-1.4.3/
+-rw-rw-rw-   0        0        0     1881 2024-05-21 14:49:21.238508 pygame_canvas-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1638 2024-05-21 14:32:25.000000 pygame_canvas-1.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 14:49:21.237244 pygame_canvas-1.4.3/pygame_canvas.egg-info/
+-rw-rw-rw-   0        0        0     1881 2024-05-21 14:49:21.000000 pygame_canvas-1.4.3/pygame_canvas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-05-21 14:49:21.000000 pygame_canvas-1.4.3/pygame_canvas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:49:21.000000 pygame_canvas-1.4.3/pygame_canvas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 14:49:21.000000 pygame_canvas-1.4.3/pygame_canvas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:49:21.000000 pygame_canvas-1.4.3/pygame_canvas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2024-05-21 13:50:24.000000 pygame_canvas-1.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:49:21.239526 pygame_canvas-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      520 2024-05-21 14:49:11.000000 pygame_canvas-1.4.3/setup.py
```

### Comparing `pygame_canvas-1.4.2/PKG-INFO` & `pygame_canvas-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pygame-canvas
-Version: 1.4.2
+Name: pygame_canvas
+Version: 1.4.3
 Summary: A library for canvas operations using pygame
 Home-page: https://x.com/gioseaxmc
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 
 Canvas
```

### Comparing `pygame_canvas-1.4.2/README.md` & `pygame_canvas-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pygame_canvas-1.4.2/pygame_canvas.egg-info/PKG-INFO` & `pygame_canvas-1.4.3/pygame_canvas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pygame-canvas
-Version: 1.4.2
+Name: pygame_canvas
+Version: 1.4.3
 Summary: A library for canvas operations using pygame
 Home-page: https://x.com/gioseaxmc
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 
 Canvas
```

### Comparing `pygame_canvas-1.4.2/setup.py` & `pygame_canvas-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_desc = fh.read()
 
 setup(
-    name='pygame-canvas',
-    version='1.4.2',
+    name='pygame_canvas',
+    version='1.4.3',
     packages=find_packages(),
     include_package_data=True,
     description='A library for canvas operations using pygame',
     long_description=long_desc,
     long_description_content_type='text/markdown',
     url='https://x.com/gioseaxmc',
     install_requires=[
```
