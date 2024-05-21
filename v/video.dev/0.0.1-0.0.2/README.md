# Comparing `tmp/video.dev-0.0.1.tar.gz` & `tmp/video.dev-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video.dev-0.0.1.tar", last modified: Tue May 21 07:14:19 2024, max compression
+gzip compressed data, was "video.dev-0.0.2.tar", last modified: Tue May 21 08:01:10 2024, max compression
```

## Comparing `video.dev-0.0.1.tar` & `video.dev-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2024-05-21 07:14:19.845101 video.dev-0.0.1/
--rw-r--r--   0 atul       (501) staff       (20)        0 2024-05-21 04:26:45.000000 video.dev-0.0.1/LICENSE
--rw-r--r--   0 atul       (501) staff       (20)      285 2024-05-21 07:14:19.844980 video.dev-0.0.1/PKG-INFO
--rw-r--r--   0 atul       (501) staff       (20)        0 2024-05-21 04:26:34.000000 video.dev-0.0.1/README.md
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2024-05-21 07:14:19.842776 video.dev-0.0.1/cli/
--rw-r--r--   0 atul       (501) staff       (20)        0 2024-05-21 05:24:24.000000 video.dev-0.0.1/cli/__init__.py
--rw-r--r--   0 atul       (501) staff       (20)      272 2024-05-21 04:39:25.000000 video.dev-0.0.1/cli/main.py
--rw-r--r--   0 atul       (501) staff       (20)       38 2024-05-21 07:14:19.845150 video.dev-0.0.1/setup.cfg
--rw-r--r--   0 atul       (501) staff       (20)      612 2024-05-21 07:14:14.000000 video.dev-0.0.1/setup.py
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2024-05-21 07:14:19.843886 video.dev-0.0.1/video.dev.egg-info/
--rw-r--r--   0 atul       (501) staff       (20)      285 2024-05-21 07:14:19.000000 video.dev-0.0.1/video.dev.egg-info/PKG-INFO
--rw-r--r--   0 atul       (501) staff       (20)      330 2024-05-21 07:14:19.000000 video.dev-0.0.1/video.dev.egg-info/SOURCES.txt
--rw-r--r--   0 atul       (501) staff       (20)        1 2024-05-21 07:14:19.000000 video.dev-0.0.1/video.dev.egg-info/dependency_links.txt
--rw-r--r--   0 atul       (501) staff       (20)       45 2024-05-21 07:14:19.000000 video.dev-0.0.1/video.dev.egg-info/entry_points.txt
--rw-r--r--   0 atul       (501) staff       (20)        6 2024-05-21 07:14:19.000000 video.dev-0.0.1/video.dev.egg-info/requires.txt
--rw-r--r--   0 atul       (501) staff       (20)       16 2024-05-21 07:14:19.000000 video.dev-0.0.1/video.dev.egg-info/top_level.txt
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2024-05-21 07:14:19.844089 video.dev-0.0.1/videodotdev/
--rw-r--r--   0 atul       (501) staff       (20)       34 2024-05-21 05:23:32.000000 video.dev-0.0.1/videodotdev/__init__.py
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2024-05-21 07:14:19.844687 video.dev-0.0.1/videodotdev/sdk/
--rw-r--r--   0 atul       (501) staff       (20)       29 2024-05-21 05:20:36.000000 video.dev-0.0.1/videodotdev/sdk/__init__.py
--rw-r--r--   0 atul       (501) staff       (20)      149 2024-05-21 05:21:26.000000 video.dev-0.0.1/videodotdev/sdk/main.py
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2024-05-21 08:01:10.621811 video.dev-0.0.2/
+-rw-r--r--   0 atul       (501) staff       (20)        0 2024-05-21 04:26:45.000000 video.dev-0.0.2/LICENSE
+-rw-r--r--   0 atul       (501) staff       (20)      294 2024-05-21 08:01:10.621658 video.dev-0.0.2/PKG-INFO
+-rw-r--r--   0 atul       (501) staff       (20)        0 2024-05-21 04:26:34.000000 video.dev-0.0.2/README.md
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2024-05-21 08:01:10.619490 video.dev-0.0.2/cli/
+-rw-r--r--   0 atul       (501) staff       (20)        0 2024-05-21 05:24:24.000000 video.dev-0.0.2/cli/__init__.py
+-rw-r--r--   0 atul       (501) staff       (20)      272 2024-05-21 04:39:25.000000 video.dev-0.0.2/cli/main.py
+-rw-r--r--   0 atul       (501) staff       (20)       38 2024-05-21 08:01:10.621872 video.dev-0.0.2/setup.cfg
+-rw-r--r--   0 atul       (501) staff       (20)      619 2024-05-21 08:01:07.000000 video.dev-0.0.2/setup.py
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2024-05-21 08:01:10.620555 video.dev-0.0.2/video.dev.egg-info/
+-rw-r--r--   0 atul       (501) staff       (20)      294 2024-05-21 08:01:10.000000 video.dev-0.0.2/video.dev.egg-info/PKG-INFO
+-rw-r--r--   0 atul       (501) staff       (20)      330 2024-05-21 08:01:10.000000 video.dev-0.0.2/video.dev.egg-info/SOURCES.txt
+-rw-r--r--   0 atul       (501) staff       (20)        1 2024-05-21 08:01:10.000000 video.dev-0.0.2/video.dev.egg-info/dependency_links.txt
+-rw-r--r--   0 atul       (501) staff       (20)       43 2024-05-21 08:01:10.000000 video.dev-0.0.2/video.dev.egg-info/entry_points.txt
+-rw-r--r--   0 atul       (501) staff       (20)        6 2024-05-21 08:01:10.000000 video.dev-0.0.2/video.dev.egg-info/requires.txt
+-rw-r--r--   0 atul       (501) staff       (20)       16 2024-05-21 08:01:10.000000 video.dev-0.0.2/video.dev.egg-info/top_level.txt
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2024-05-21 08:01:10.620685 video.dev-0.0.2/videodotdev/
+-rw-r--r--   0 atul       (501) staff       (20)       34 2024-05-21 05:23:32.000000 video.dev-0.0.2/videodotdev/__init__.py
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2024-05-21 08:01:10.621217 video.dev-0.0.2/videodotdev/sdk/
+-rw-r--r--   0 atul       (501) staff       (20)       29 2024-05-21 05:20:36.000000 video.dev-0.0.2/videodotdev/sdk/__init__.py
+-rw-r--r--   0 atul       (501) staff       (20)      149 2024-05-21 05:21:26.000000 video.dev-0.0.2/videodotdev/sdk/main.py
```

### Comparing `video.dev-0.0.1/setup.py` & `video.dev-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='video.dev',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'typer',
     ],
     entry_points={
         'console_scripts': [
-            'videodotdev=cli.main:app',
+            'video-dev=cli.main:app',
         ]
     },
     author='video.dev Team',
     author_email='developer@video.dev',
     description='video.dev command-line tool.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='MIT',
-    keywords='video.dev command-line',
+    keywords='video.dev CLI and Python Client',
     url='https://video.dev',
 )
```

