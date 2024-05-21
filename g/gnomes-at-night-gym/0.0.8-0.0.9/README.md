# Comparing `tmp/gnomes_at_night_gym-0.0.8.tar.gz` & `tmp/gnomes_at_night_gym-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnomes_at_night_gym-0.0.8.tar", last modified: Mon Feb 12 05:10:51 2024, max compression
+gzip compressed data, was "gnomes_at_night_gym-0.0.9.tar", last modified: Tue Apr  9 18:44:35 2024, max compression
```

## Comparing `gnomes_at_night_gym-0.0.8.tar` & `gnomes_at_night_gym-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 vivianchen   (503) staff       (20)        0 2024-02-12 05:10:51.830271 gnomes_at_night_gym-0.0.8/
--rw-r--r--   0 vivianchen   (503) staff       (20)      477 2024-02-12 05:10:51.829874 gnomes_at_night_gym-0.0.8/PKG-INFO
--rw-r--r--   0 vivianchen   (503) staff       (20)      710 2023-11-07 04:01:40.000000 gnomes_at_night_gym-0.0.8/README.md
-drwxr-xr-x   0 vivianchen   (503) staff       (20)        0 2024-02-12 05:10:51.818071 gnomes_at_night_gym-0.0.8/gnomes_at_night_gym/
--rw-r--r--   0 vivianchen   (503) staff       (20)      302 2023-11-26 17:49:16.000000 gnomes_at_night_gym-0.0.8/gnomes_at_night_gym/__init__.py
-drwxr-xr-x   0 vivianchen   (503) staff       (20)        0 2024-02-12 05:10:51.826213 gnomes_at_night_gym-0.0.8/gnomes_at_night_gym/envs/
--rw-r--r--   0 vivianchen   (503) staff       (20)      151 2023-11-26 17:52:05.000000 gnomes_at_night_gym-0.0.8/gnomes_at_night_gym/envs/__init__.py
--rw-r--r--   0 vivianchen   (503) staff       (20)    24387 2023-11-26 17:48:48.000000 gnomes_at_night_gym-0.0.8/gnomes_at_night_gym/envs/gnomesAtNightEnv_5A.py
--rw-r--r--   0 vivianchen   (503) staff       (20)    25370 2024-02-12 05:07:04.000000 gnomes_at_night_gym-0.0.8/gnomes_at_night_gym/envs/gnomesAtNightEnv_9A.py
-drwxr-xr-x   0 vivianchen   (503) staff       (20)        0 2024-02-12 05:10:51.824786 gnomes_at_night_gym-0.0.8/gnomes_at_night_gym.egg-info/
--rw-r--r--   0 vivianchen   (503) staff       (20)      477 2024-02-12 05:10:51.000000 gnomes_at_night_gym-0.0.8/gnomes_at_night_gym.egg-info/PKG-INFO
--rw-r--r--   0 vivianchen   (503) staff       (20)      397 2024-02-12 05:10:51.000000 gnomes_at_night_gym-0.0.8/gnomes_at_night_gym.egg-info/SOURCES.txt
--rw-r--r--   0 vivianchen   (503) staff       (20)        1 2024-02-12 05:10:51.000000 gnomes_at_night_gym-0.0.8/gnomes_at_night_gym.egg-info/dependency_links.txt
--rw-r--r--   0 vivianchen   (503) staff       (20)       46 2024-02-12 05:10:51.000000 gnomes_at_night_gym-0.0.8/gnomes_at_night_gym.egg-info/requires.txt
--rw-r--r--   0 vivianchen   (503) staff       (20)       20 2024-02-12 05:10:51.000000 gnomes_at_night_gym-0.0.8/gnomes_at_night_gym.egg-info/top_level.txt
--rw-r--r--   0 vivianchen   (503) staff       (20)       38 2024-02-12 05:10:51.830338 gnomes_at_night_gym-0.0.8/setup.cfg
--rw-r--r--   0 vivianchen   (503) staff       (20)      707 2024-02-12 05:10:26.000000 gnomes_at_night_gym-0.0.8/setup.py
+drwxr-xr-x   0 vivianchen   (503) staff       (20)        0 2024-04-09 18:44:35.299968 gnomes_at_night_gym-0.0.9/
+-rw-r--r--   0 vivianchen   (503) staff       (20)      477 2024-04-09 18:44:35.299718 gnomes_at_night_gym-0.0.9/PKG-INFO
+-rw-r--r--   0 vivianchen   (503) staff       (20)     1752 2024-04-09 18:36:33.000000 gnomes_at_night_gym-0.0.9/README.md
+drwxr-xr-x   0 vivianchen   (503) staff       (20)        0 2024-04-09 18:44:35.294904 gnomes_at_night_gym-0.0.9/gnomes_at_night_gym/
+-rw-r--r--   0 vivianchen   (503) staff       (20)      447 2024-04-09 18:22:27.000000 gnomes_at_night_gym-0.0.9/gnomes_at_night_gym/__init__.py
+drwxr-xr-x   0 vivianchen   (503) staff       (20)        0 2024-04-09 18:44:35.299335 gnomes_at_night_gym-0.0.9/gnomes_at_night_gym/envs/
+-rw-r--r--   0 vivianchen   (503) staff       (20)      245 2024-04-09 18:22:18.000000 gnomes_at_night_gym-0.0.9/gnomes_at_night_gym/envs/__init__.py
+-rw-r--r--   0 vivianchen   (503) staff       (20)    24387 2023-11-26 17:48:48.000000 gnomes_at_night_gym-0.0.9/gnomes_at_night_gym/envs/gnomesAtNightEnv_5A.py
+-rw-r--r--   0 vivianchen   (503) staff       (20)    25370 2024-02-12 05:07:04.000000 gnomes_at_night_gym-0.0.9/gnomes_at_night_gym/envs/gnomesAtNightEnv_9A.py
+-rw-r--r--   0 vivianchen   (503) staff       (20)    59975 2024-04-09 18:04:46.000000 gnomes_at_night_gym-0.0.9/gnomes_at_night_gym/envs/gnomesAtNightEnv_9_multistep.py
+drwxr-xr-x   0 vivianchen   (503) staff       (20)        0 2024-04-09 18:44:35.297986 gnomes_at_night_gym-0.0.9/gnomes_at_night_gym.egg-info/
+-rw-r--r--   0 vivianchen   (503) staff       (20)      477 2024-04-09 18:44:35.000000 gnomes_at_night_gym-0.0.9/gnomes_at_night_gym.egg-info/PKG-INFO
+-rw-r--r--   0 vivianchen   (503) staff       (20)      454 2024-04-09 18:44:35.000000 gnomes_at_night_gym-0.0.9/gnomes_at_night_gym.egg-info/SOURCES.txt
+-rw-r--r--   0 vivianchen   (503) staff       (20)        1 2024-04-09 18:44:35.000000 gnomes_at_night_gym-0.0.9/gnomes_at_night_gym.egg-info/dependency_links.txt
+-rw-r--r--   0 vivianchen   (503) staff       (20)       46 2024-04-09 18:44:35.000000 gnomes_at_night_gym-0.0.9/gnomes_at_night_gym.egg-info/requires.txt
+-rw-r--r--   0 vivianchen   (503) staff       (20)       20 2024-04-09 18:44:35.000000 gnomes_at_night_gym-0.0.9/gnomes_at_night_gym.egg-info/top_level.txt
+-rw-r--r--   0 vivianchen   (503) staff       (20)       38 2024-04-09 18:44:35.300036 gnomes_at_night_gym-0.0.9/setup.cfg
+-rw-r--r--   0 vivianchen   (503) staff       (20)      808 2024-04-09 18:41:33.000000 gnomes_at_night_gym-0.0.9/setup.py
```

### Comparing `gnomes_at_night_gym-0.0.8/gnomes_at_night_gym/envs/gnomesAtNightEnv_5A.py` & `gnomes_at_night_gym-0.0.9/gnomes_at_night_gym/envs/gnomesAtNightEnv_5A.py`

 * *Files identical despite different names*

### Comparing `gnomes_at_night_gym-0.0.8/gnomes_at_night_gym/envs/gnomesAtNightEnv_9A.py` & `gnomes_at_night_gym-0.0.9/gnomes_at_night_gym/envs/gnomesAtNightEnv_9A.py`

 * *Files identical despite different names*

### Comparing `gnomes_at_night_gym-0.0.8/setup.py` & `gnomes_at_night_gym-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 long_description = """
 ## Installation
 
 You can install the package using pip:
 
 ```pip install gnomes-at-night-gym```
@@ -14,18 +14,19 @@
 ```python
 import gnomes_at_night_gym
 env = gym.make("gnomes_at_night_gym:Board9A-v0", render_mode="rgb_array", round=1)
 """
 
 setup(
     name="gnomes_at_night_gym",
-    version="0.0.8",
+    version="0.0.9",
     description='An environment for Gnomes at Night based on OpenAI gym.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Shenghui Chen',
     install_requires=[
         "gymnasium==0.29.1", 
         "pygame==2.5.2", 
         "numpy==1.26.1"
     ],
+    packages=find_packages(include=['gnomes_at_night_gym', 'gnomes_at_night_gym.*']),
 )
```

