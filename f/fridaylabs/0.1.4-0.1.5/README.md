# Comparing `tmp/fridaylabs-0.1.4.tar.gz` & `tmp/fridaylabs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fridaylabs-0.1.4.tar", last modified: Tue May 21 06:39:52 2024, max compression
+gzip compressed data, was "fridaylabs-0.1.5.tar", last modified: Tue May 21 20:05:48 2024, max compression
```

## Comparing `fridaylabs-0.1.4.tar` & `fridaylabs-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 06:39:52.887961 fridaylabs-0.1.4/
--rw-r--r--   0 ricky      (501) staff       (20)     1070 2024-05-21 04:23:26.000000 fridaylabs-0.1.4/LICENSE
--rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-21 06:39:52.887669 fridaylabs-0.1.4/PKG-INFO
--rw-r--r--   0 ricky      (501) staff       (20)      792 2024-05-21 05:35:31.000000 fridaylabs-0.1.4/README.md
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 06:39:52.886047 fridaylabs-0.1.4/fridaylabs/
--rw-r--r--   0 ricky      (501) staff       (20)       61 2024-05-21 05:49:44.000000 fridaylabs-0.1.4/fridaylabs/__init__.py
--rw-r--r--   0 ricky      (501) staff       (20)     4742 2024-05-21 06:39:16.000000 fridaylabs-0.1.4/fridaylabs/fridaylabs.py
-drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 06:39:52.887351 fridaylabs-0.1.4/fridaylabs.egg-info/
--rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-21 06:39:52.000000 fridaylabs-0.1.4/fridaylabs.egg-info/PKG-INFO
--rw-r--r--   0 ricky      (501) staff       (20)      243 2024-05-21 06:39:52.000000 fridaylabs-0.1.4/fridaylabs.egg-info/SOURCES.txt
--rw-r--r--   0 ricky      (501) staff       (20)        1 2024-05-21 06:39:52.000000 fridaylabs-0.1.4/fridaylabs.egg-info/dependency_links.txt
--rw-r--r--   0 ricky      (501) staff       (20)        9 2024-05-21 06:39:52.000000 fridaylabs-0.1.4/fridaylabs.egg-info/requires.txt
--rw-r--r--   0 ricky      (501) staff       (20)       11 2024-05-21 06:39:52.000000 fridaylabs-0.1.4/fridaylabs.egg-info/top_level.txt
--rw-r--r--   0 ricky      (501) staff       (20)       38 2024-05-21 06:39:52.888024 fridaylabs-0.1.4/setup.cfg
--rw-r--r--   0 ricky      (501) staff       (20)      693 2024-05-21 06:39:50.000000 fridaylabs-0.1.4/setup.py
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 20:05:48.459944 fridaylabs-0.1.5/
+-rw-r--r--   0 ricky      (501) staff       (20)     1070 2024-05-21 04:23:26.000000 fridaylabs-0.1.5/LICENSE
+-rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-21 20:05:48.459690 fridaylabs-0.1.5/PKG-INFO
+-rw-r--r--   0 ricky      (501) staff       (20)      792 2024-05-21 05:35:31.000000 fridaylabs-0.1.5/README.md
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 20:05:48.458251 fridaylabs-0.1.5/fridaylabs/
+-rw-r--r--   0 ricky      (501) staff       (20)       61 2024-05-21 05:49:44.000000 fridaylabs-0.1.5/fridaylabs/__init__.py
+-rw-r--r--   0 ricky      (501) staff       (20)     4891 2024-05-21 20:05:31.000000 fridaylabs-0.1.5/fridaylabs/fridaylabs.py
+drwxr-xr-x   0 ricky      (501) staff       (20)        0 2024-05-21 20:05:48.459437 fridaylabs-0.1.5/fridaylabs.egg-info/
+-rw-r--r--   0 ricky      (501) staff       (20)     1275 2024-05-21 20:05:48.000000 fridaylabs-0.1.5/fridaylabs.egg-info/PKG-INFO
+-rw-r--r--   0 ricky      (501) staff       (20)      243 2024-05-21 20:05:48.000000 fridaylabs-0.1.5/fridaylabs.egg-info/SOURCES.txt
+-rw-r--r--   0 ricky      (501) staff       (20)        1 2024-05-21 20:05:48.000000 fridaylabs-0.1.5/fridaylabs.egg-info/dependency_links.txt
+-rw-r--r--   0 ricky      (501) staff       (20)        9 2024-05-21 20:05:48.000000 fridaylabs-0.1.5/fridaylabs.egg-info/requires.txt
+-rw-r--r--   0 ricky      (501) staff       (20)       11 2024-05-21 20:05:48.000000 fridaylabs-0.1.5/fridaylabs.egg-info/top_level.txt
+-rw-r--r--   0 ricky      (501) staff       (20)       38 2024-05-21 20:05:48.459998 fridaylabs-0.1.5/setup.cfg
+-rw-r--r--   0 ricky      (501) staff       (20)      693 2024-05-21 20:05:45.000000 fridaylabs-0.1.5/setup.py
```

### Comparing `fridaylabs-0.1.4/LICENSE` & `fridaylabs-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fridaylabs-0.1.4/PKG-INFO` & `fridaylabs-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fridaylabs
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package to interact with FridayLabs AI API
 Home-page: https://github.com/ImJustRicky/fridaylabs-package
 Author: FridayLabs
 Author-email: fridaylabs@fridaylabs.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fridaylabs-0.1.4/README.md` & `fridaylabs-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fridaylabs-0.1.4/fridaylabs/fridaylabs.py` & `fridaylabs-0.1.5/fridaylabs/fridaylabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
                 print(f"{Colors.OKGREEN}{Colors.BOLD}Request successful!{Colors.ENDC}")
             return response.json()
 
         except requests.exceptions.HTTPError as http_err:
             if self.verbose:
                 print(f"{Colors.FAIL}{Colors.BOLD}HTTP error occurred: {Colors.ENDC}{http_err}")
                 self.suggest_solution(response)
+            if response.status_code == 403:
+                return {"error": "Access to this model is restricted. Please check your access rights."}
             raise
 
         except requests.exceptions.RequestException as req_err:
             if self.verbose:
                 print(f"{Colors.FAIL}{Colors.BOLD}Request error occurred: {Colors.ENDC}{req_err}")
                 print(f"{Colors.WARNING}Possible solutions:{Colors.ENDC}")
                 print(f"{Colors.WARNING}1. Check your network connection.{Colors.ENDC}")
```

### Comparing `fridaylabs-0.1.4/fridaylabs.egg-info/PKG-INFO` & `fridaylabs-0.1.5/fridaylabs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fridaylabs
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package to interact with FridayLabs AI API
 Home-page: https://github.com/ImJustRicky/fridaylabs-package
 Author: FridayLabs
 Author-email: fridaylabs@fridaylabs.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fridaylabs-0.1.4/setup.py` & `fridaylabs-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name="fridaylabs",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=["requests"],  # Add any dependencies here
     author="FridayLabs",
     author_email="fridaylabs@fridaylabs.ai",
     description="A package to interact with FridayLabs AI API",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

