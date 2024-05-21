# Comparing `tmp/pyselenscrapr-0.0.8.tar.gz` & `tmp/pyselenscrapr-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyselenscrapr-0.0.8.tar", last modified: Tue May 21 10:23:09 2024, max compression
+gzip compressed data, was "pyselenscrapr-0.0.81.tar", last modified: Tue May 21 10:24:22 2024, max compression
```

## Comparing `pyselenscrapr-0.0.8.tar` & `pyselenscrapr-0.0.81.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:23:09.778756 pyselenscrapr-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:23:09.770755 pyselenscrapr-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:23:09.774756 pyselenscrapr-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-21 10:23:09.778756 pyselenscrapr-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:23:09.774756 pyselenscrapr-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:23:09.774756 pyselenscrapr-0.0.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/docs/source/pyselenscrapr.rst
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:23:09.778756 pyselenscrapr-0.0.8/pyselenscrapr/
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/pyselenscrapr/ScrapingBackend.py
--rw-r--r--   0 runner    (1001) docker     (127)    14546 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/pyselenscrapr/ScrapingBot.py
--rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/pyselenscrapr/ScrapingLogic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/pyselenscrapr/ScrapingStep.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/pyselenscrapr/ScrapingStepGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/pyselenscrapr/ScrapingStepLoop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/pyselenscrapr/ScrapingStepPagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/pyselenscrapr/ValidationError.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/pyselenscrapr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:23:09.778756 pyselenscrapr-0.0.8/pyselenscrapr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-21 10:23:09.000000 pyselenscrapr-0.0.8/pyselenscrapr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-21 10:23:09.000000 pyselenscrapr-0.0.8/pyselenscrapr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 10:23:09.000000 pyselenscrapr-0.0.8/pyselenscrapr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-21 10:23:09.000000 pyselenscrapr-0.0.8/pyselenscrapr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 10:23:09.000000 pyselenscrapr-0.0.8/pyselenscrapr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-21 10:22:52.000000 pyselenscrapr-0.0.8/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 10:23:09.778756 pyselenscrapr-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:24:22.867324 pyselenscrapr-0.0.81/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:24:22.859325 pyselenscrapr-0.0.81/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:24:22.863324 pyselenscrapr-0.0.81/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-21 10:24:22.867324 pyselenscrapr-0.0.81/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:24:22.863324 pyselenscrapr-0.0.81/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:24:22.863324 pyselenscrapr-0.0.81/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/docs/source/pyselenscrapr.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:24:22.863324 pyselenscrapr-0.0.81/pyselenscrapr/
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/pyselenscrapr/ScrapingBackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14546 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/pyselenscrapr/ScrapingBot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/pyselenscrapr/ScrapingLogic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/pyselenscrapr/ScrapingStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/pyselenscrapr/ScrapingStepGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/pyselenscrapr/ScrapingStepLoop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/pyselenscrapr/ScrapingStepPagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/pyselenscrapr/ValidationError.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/pyselenscrapr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:24:22.867324 pyselenscrapr-0.0.81/pyselenscrapr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-21 10:24:22.000000 pyselenscrapr-0.0.81/pyselenscrapr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-21 10:24:22.000000 pyselenscrapr-0.0.81/pyselenscrapr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 10:24:22.000000 pyselenscrapr-0.0.81/pyselenscrapr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-21 10:24:22.000000 pyselenscrapr-0.0.81/pyselenscrapr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 10:24:22.000000 pyselenscrapr-0.0.81/pyselenscrapr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-21 10:24:11.000000 pyselenscrapr-0.0.81/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 10:24:22.867324 pyselenscrapr-0.0.81/setup.cfg
```

### Comparing `pyselenscrapr-0.0.8/.github/workflows/pypi.yml` & `pyselenscrapr-0.0.81/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.8/LICENSE` & `pyselenscrapr-0.0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.8/PKG-INFO` & `pyselenscrapr-0.0.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyselenscrapr
-Version: 0.0.8
+Version: 0.0.81
 Summary: A web scraping library for selenium and beautifulsoup
 Author-email: donnercody <donnercody86@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: beautifulsoup4
```

### Comparing `pyselenscrapr-0.0.8/README.rst` & `pyselenscrapr-0.0.81/README.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.8/docs/Makefile` & `pyselenscrapr-0.0.81/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.8/docs/make.bat` & `pyselenscrapr-0.0.81/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.8/docs/source/conf.py` & `pyselenscrapr-0.0.81/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import sys
 sys.path.insert(0, os.path.abspath(os.path.join("..", "..")))
 
 project = 'PySelenScrapr'
 copyright = '2024, Thoren Lederer'
 author = 'donnercody'
 
-release = '0.0.8'
-version = '0.0.8'
+release = '0.0.81'
+version = '0.0.81'
 
 # -- General configuration
 
 extensions = [
     'sphinx.ext.duration',
     'sphinx.ext.doctest',
     'sphinx.ext.autodoc',
```

### Comparing `pyselenscrapr-0.0.8/docs/source/index.rst` & `pyselenscrapr-0.0.81/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.8/docs/source/pyselenscrapr.rst` & `pyselenscrapr-0.0.81/docs/source/pyselenscrapr.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.8/docs/source/usage.rst` & `pyselenscrapr-0.0.81/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.8/pyselenscrapr/ScrapingBackend.py` & `pyselenscrapr-0.0.81/pyselenscrapr/ScrapingBackend.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.8/pyselenscrapr/ScrapingBot.py` & `pyselenscrapr-0.0.81/pyselenscrapr/ScrapingBot.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.8/pyselenscrapr/ScrapingLogic.py` & `pyselenscrapr-0.0.81/pyselenscrapr/ScrapingLogic.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.8/pyselenscrapr/ScrapingStep.py` & `pyselenscrapr-0.0.81/pyselenscrapr/ScrapingStep.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.8/pyselenscrapr/ScrapingStepLoop.py` & `pyselenscrapr-0.0.81/pyselenscrapr/ScrapingStepLoop.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.8/pyselenscrapr/ScrapingStepPagination.py` & `pyselenscrapr-0.0.81/pyselenscrapr/ScrapingStepPagination.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,26 +37,22 @@
     def finished(self):
         for i in self._executionList:
             if i is None:
                 return False
         return True
 
     def _get_next_page(self):
-        # TODO: remove because of testing
-        return 500
-        """
         for i in range(1, len(self._executionList)):
             if self._pagination_mode == ScrapingStepPaginationMode.RandomPages:
                 r = random.randint(1, len(self._executionList)-1)
                 if self._executionList[r] is None:
                     return r
             else:
                 if self._executionList[i] is None:
                     return i
-                """
         return None
 
     def _sleep(self, t):
         time.sleep(t)
 
     def can_retry(self):
         return False
```

### Comparing `pyselenscrapr-0.0.8/pyselenscrapr.egg-info/PKG-INFO` & `pyselenscrapr-0.0.81/pyselenscrapr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyselenscrapr
-Version: 0.0.8
+Version: 0.0.81
 Summary: A web scraping library for selenium and beautifulsoup
 Author-email: donnercody <donnercody86@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: beautifulsoup4
```

### Comparing `pyselenscrapr-0.0.8/pyselenscrapr.egg-info/SOURCES.txt` & `pyselenscrapr-0.0.81/pyselenscrapr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.8/sample.py` & `pyselenscrapr-0.0.81/sample.py`

 * *Files identical despite different names*

