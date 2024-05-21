# Comparing `tmp/nurmoai-0.1.0.tar.gz` & `tmp/nurmoai-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nurmoai-0.1.0.tar", last modified: Tue May 21 14:32:49 2024, max compression
+gzip compressed data, was "nurmoai-1.0.0.tar", last modified: Tue May 21 14:35:51 2024, max compression
```

## Comparing `nurmoai-0.1.0.tar` & `nurmoai-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-21 14:32:49.481718 nurmoai-0.1.0/
--rw-r--r--   0 runner    (1000) runner    (1000)     1713 2024-05-21 14:32:49.481718 nurmoai-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1465 2024-05-21 14:12:38.000000 nurmoai-0.1.0/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-21 14:32:49.477718 nurmoai-0.1.0/nurmo/
--rw-r--r--   0 runner    (1000) runner    (1000)       26 2024-05-21 14:07:07.000000 nurmoai-0.1.0/nurmo/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1011 2024-05-21 14:06:11.000000 nurmoai-0.1.0/nurmo/nurmo.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-21 14:32:49.477718 nurmoai-0.1.0/nurmoai.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1713 2024-05-21 14:32:49.000000 nurmoai-0.1.0/nurmoai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      220 2024-05-21 14:32:49.000000 nurmoai-0.1.0/nurmoai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-21 14:32:49.000000 nurmoai-0.1.0/nurmoai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-05-21 14:32:49.000000 nurmoai-0.1.0/nurmoai.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-05-21 14:32:49.000000 nurmoai-0.1.0/nurmoai.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)      544 2024-02-27 23:10:40.000000 nurmoai-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-21 14:32:49.481718 nurmoai-0.1.0/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      425 2024-05-21 14:06:39.000000 nurmoai-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-21 14:35:51.553445 nurmoai-1.0.0/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1713 2024-05-21 14:35:51.553445 nurmoai-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1465 2024-05-21 14:12:38.000000 nurmoai-1.0.0/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-21 14:35:51.549445 nurmoai-1.0.0/nurmo/
+-rw-r--r--   0 runner    (1000) runner    (1000)       26 2024-05-21 14:07:07.000000 nurmoai-1.0.0/nurmo/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1022 2024-05-21 14:34:44.000000 nurmoai-1.0.0/nurmo/nurmo.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-21 14:35:51.553445 nurmoai-1.0.0/nurmoai.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1713 2024-05-21 14:35:51.000000 nurmoai-1.0.0/nurmoai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      220 2024-05-21 14:35:51.000000 nurmoai-1.0.0/nurmoai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-21 14:35:51.000000 nurmoai-1.0.0/nurmoai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-05-21 14:35:51.000000 nurmoai-1.0.0/nurmoai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-05-21 14:35:51.000000 nurmoai-1.0.0/nurmoai.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)      544 2024-02-27 23:10:40.000000 nurmoai-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-21 14:35:51.553445 nurmoai-1.0.0/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      425 2024-05-21 14:35:04.000000 nurmoai-1.0.0/setup.py
```

### Comparing `nurmoai-0.1.0/PKG-INFO` & `nurmoai-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nurmoai
-Version: 0.1.0
+Version: 1.0.0
 Summary: A Python client for the NurmoAI API.
 Home-page: https://nurmo.app
 Author: Reksely
 Author-email: reksely@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.25.1
```

### Comparing `nurmoai-0.1.0/README.md` & `nurmoai-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nurmoai-0.1.0/nurmo/nurmo.py` & `nurmoai-1.0.0/nurmo/nurmo.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 
 class NurmoAI:
     def __init__(self, api_key=None):
         self.api_key = api_key if api_key is not None else os.environ.get('NURMO_KEY')
         self.base_url = 'https://api.nurmo.app/chat/completions'
 
     def create_completion(self, messages, model, character=None):
-        headers = {'Authorization': self.api_key}
-
+        headers = {'Authorization': f'Bearer {self.api_key}'}
         if character is None:
             raise ValueError("Please provide a character name.")
 
         data = {'model': model, 'messages': messages, character: character}
 
         response = requests.post(self.base_url, json=data, headers=headers)
         response_text = response.text
```

### Comparing `nurmoai-0.1.0/nurmoai.egg-info/PKG-INFO` & `nurmoai-1.0.0/nurmoai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nurmoai
-Version: 0.1.0
+Version: 1.0.0
 Summary: A Python client for the NurmoAI API.
 Home-page: https://nurmo.app
 Author: Reksely
 Author-email: reksely@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.25.1
```

### Comparing `nurmoai-0.1.0/pyproject.toml` & `nurmoai-1.0.0/pyproject.toml`

 * *Files identical despite different names*

