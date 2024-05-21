# Comparing `tmp/pygame_canvas-1.4.5.tar.gz` & `tmp/pygame_canvas-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_canvas-1.4.5.tar", last modified: Tue May 21 14:55:01 2024, max compression
+gzip compressed data, was "pygame_canvas-1.4.6.tar", last modified: Tue May 21 14:58:22 2024, max compression
```

## Comparing `pygame_canvas-1.4.5.tar` & `pygame_canvas-1.4.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 14:55:01.118874 pygame_canvas-1.4.5/
--rw-rw-rw-   0        0        0     1881 2024-05-21 14:55:01.116836 pygame_canvas-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     1638 2024-05-21 14:32:25.000000 pygame_canvas-1.4.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 14:55:01.091977 pygame_canvas-1.4.5/pygame_canvas/
--rw-rw-rw-   0        0        0        0 2024-05-21 13:46:56.000000 pygame_canvas-1.4.5/pygame_canvas/__init__.py
--rw-rw-rw-   0        0        0    16821 2024-05-21 14:44:17.000000 pygame_canvas-1.4.5/pygame_canvas/pygame_canvas.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:55:01.115811 pygame_canvas-1.4.5/pygame_canvas.egg-info/
--rw-rw-rw-   0        0        0     1881 2024-05-21 14:55:00.000000 pygame_canvas-1.4.5/pygame_canvas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-21 14:55:01.000000 pygame_canvas-1.4.5/pygame_canvas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:55:00.000000 pygame_canvas-1.4.5/pygame_canvas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 14:55:00.000000 pygame_canvas-1.4.5/pygame_canvas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-21 14:55:00.000000 pygame_canvas-1.4.5/pygame_canvas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2024-05-21 13:50:24.000000 pygame_canvas-1.4.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 14:55:01.118874 pygame_canvas-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0      520 2024-05-21 14:54:54.000000 pygame_canvas-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:58:22.042747 pygame_canvas-1.4.6/
+-rw-rw-rw-   0        0        0     1881 2024-05-21 14:58:22.040721 pygame_canvas-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1638 2024-05-21 14:32:25.000000 pygame_canvas-1.4.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 14:58:22.017773 pygame_canvas-1.4.6/pygame_canvas/
+-rw-rw-rw-   0        0        0       27 2024-05-21 14:58:05.000000 pygame_canvas-1.4.6/pygame_canvas/__init__.py
+-rw-rw-rw-   0        0        0    16821 2024-05-21 14:44:17.000000 pygame_canvas-1.4.6/pygame_canvas/pygame_canvas.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:58:22.040214 pygame_canvas-1.4.6/pygame_canvas.egg-info/
+-rw-rw-rw-   0        0        0     1881 2024-05-21 14:58:21.000000 pygame_canvas-1.4.6/pygame_canvas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-21 14:58:21.000000 pygame_canvas-1.4.6/pygame_canvas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:58:21.000000 pygame_canvas-1.4.6/pygame_canvas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 14:58:21.000000 pygame_canvas-1.4.6/pygame_canvas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-21 14:58:21.000000 pygame_canvas-1.4.6/pygame_canvas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2024-05-21 13:50:24.000000 pygame_canvas-1.4.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:58:22.042747 pygame_canvas-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      520 2024-05-21 14:58:13.000000 pygame_canvas-1.4.6/setup.py
```

### Comparing `pygame_canvas-1.4.5/PKG-INFO` & `pygame_canvas-1.4.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame_canvas
-Version: 1.4.5
+Version: 1.4.6
 Summary: A library for canvas operations using pygame
 Home-page: https://x.com/gioseaxmc
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 
 Canvas
```

### Comparing `pygame_canvas-1.4.5/README.md` & `pygame_canvas-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `pygame_canvas-1.4.5/pygame_canvas/pygame_canvas.py` & `pygame_canvas-1.4.6/pygame_canvas/pygame_canvas.py`

 * *Files identical despite different names*

### Comparing `pygame_canvas-1.4.5/pygame_canvas.egg-info/PKG-INFO` & `pygame_canvas-1.4.6/pygame_canvas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame_canvas
-Version: 1.4.5
+Version: 1.4.6
 Summary: A library for canvas operations using pygame
 Home-page: https://x.com/gioseaxmc
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 
 Canvas
```

### Comparing `pygame_canvas-1.4.5/setup.py` & `pygame_canvas-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_desc = fh.read()
 
 setup(
     name='pygame_canvas',
-    version='1.4.5',
+    version='1.4.6',
     packages=find_packages(),
     include_package_data=True,
     description='A library for canvas operations using pygame',
     long_description=long_desc,
     long_description_content_type='text/markdown',
     url='https://x.com/gioseaxmc',
     install_requires=[
```

