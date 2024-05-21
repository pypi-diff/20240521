# Comparing `tmp/rpa_helpers_btime-1.0.8.tar.gz` & `tmp/rpa_helpers_btime-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_helpers_btime-1.0.8.tar", last modified: Tue May 21 14:07:05 2024, max compression
+gzip compressed data, was "rpa_helpers_btime-1.0.9.tar", last modified: Tue May 21 14:09:36 2024, max compression
```

## Comparing `rpa_helpers_btime-1.0.8.tar` & `rpa_helpers_btime-1.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 14:07:05.633784 rpa_helpers_btime-1.0.8/
--rw-rw-rw-   0        0        0      748 2024-05-21 14:07:05.630501 rpa_helpers_btime-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1058 2024-05-21 12:29:56.000000 rpa_helpers_btime-1.0.8/license.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 14:07:05.565346 rpa_helpers_btime-1.0.8/rpa_helpers/
--rw-rw-rw-   0        0        0       35 2024-05-21 13:53:04.000000 rpa_helpers_btime-1.0.8/rpa_helpers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:07:05.567789 rpa_helpers_btime-1.0.8/rpa_helpers/src/
--rw-rw-rw-   0        0        0       51 2024-05-21 13:52:57.000000 rpa_helpers_btime-1.0.8/rpa_helpers/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:07:05.570801 rpa_helpers_btime-1.0.8/rpa_helpers/src/configuration/
--rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.8/rpa_helpers/src/configuration/__init__.py
--rw-rw-rw-   0        0        0      184 2024-05-21 14:01:28.000000 rpa_helpers_btime-1.0.8/rpa_helpers/src/configuration/configuration.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:07:05.571804 rpa_helpers_btime-1.0.8/rpa_helpers/src/models/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.8/rpa_helpers/src/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:07:05.578369 rpa_helpers_btime-1.0.8/rpa_helpers/src/models/configs/
--rw-rw-rw-   0        0        0        0 2024-05-14 19:21:02.000000 rpa_helpers_btime-1.0.8/rpa_helpers/src/models/configs/__init__.py
--rw-rw-rw-   0        0        0       84 2024-05-14 19:23:16.000000 rpa_helpers_btime-1.0.8/rpa_helpers/src/models/configs/base.py
--rw-rw-rw-   0        0        0      841 2024-05-21 14:03:11.000000 rpa_helpers_btime-1.0.8/rpa_helpers/src/models/configs/connection.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:07:05.586173 rpa_helpers_btime-1.0.8/rpa_helpers/src/models/entities/
--rw-rw-rw-   0        0        0        0 2024-05-14 19:21:02.000000 rpa_helpers_btime-1.0.8/rpa_helpers/src/models/entities/__init__.py
--rw-rw-rw-   0        0        0      760 2024-05-21 14:03:36.000000 rpa_helpers_btime-1.0.8/rpa_helpers/src/models/entities/log.py
--rw-rw-rw-   0        0        0      297 2024-05-21 14:03:28.000000 rpa_helpers_btime-1.0.8/rpa_helpers/src/models/entities/rpa.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:07:05.592143 rpa_helpers_btime-1.0.8/rpa_helpers/src/models/repository/
--rw-rw-rw-   0        0        0        0 2024-05-14 19:21:02.000000 rpa_helpers_btime-1.0.8/rpa_helpers/src/models/repository/__init__.py
--rw-rw-rw-   0        0        0     1436 2024-05-21 14:03:43.000000 rpa_helpers_btime-1.0.8/rpa_helpers/src/models/repository/repository_log.py
--rw-rw-rw-   0        0        0      935 2024-05-21 14:03:47.000000 rpa_helpers_btime-1.0.8/rpa_helpers/src/models/repository/repository_rpa.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:07:05.598162 rpa_helpers_btime-1.0.8/rpa_helpers/src/utils/
--rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.8/rpa_helpers/src/utils/__init__.py
--rw-rw-rw-   0        0        0     3056 2024-05-21 13:53:17.000000 rpa_helpers_btime-1.0.8/rpa_helpers/src/utils/decorator_log.py
--rw-rw-rw-   0        0        0     1293 2024-05-15 18:18:58.000000 rpa_helpers_btime-1.0.8/rpa_helpers/src/utils/send_email.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:07:05.628509 rpa_helpers_btime-1.0.8/rpa_helpers_btime.egg-info/
--rw-rw-rw-   0        0        0      748 2024-05-21 14:07:05.000000 rpa_helpers_btime-1.0.8/rpa_helpers_btime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      908 2024-05-21 14:07:05.000000 rpa_helpers_btime-1.0.8/rpa_helpers_btime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:07:05.000000 rpa_helpers_btime-1.0.8/rpa_helpers_btime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      218 2024-05-21 14:07:05.000000 rpa_helpers_btime-1.0.8/rpa_helpers_btime.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-21 14:07:05.000000 rpa_helpers_btime-1.0.8/rpa_helpers_btime.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 14:07:05.634480 rpa_helpers_btime-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1140 2024-05-21 14:07:02.000000 rpa_helpers_btime-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:09:36.349830 rpa_helpers_btime-1.0.9/
+-rw-rw-rw-   0        0        0      773 2024-05-21 14:09:36.348773 rpa_helpers_btime-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1058 2024-05-21 12:29:56.000000 rpa_helpers_btime-1.0.9/license.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 14:09:36.289703 rpa_helpers_btime-1.0.9/rpa_helpers/
+-rw-rw-rw-   0        0        0       35 2024-05-21 13:53:04.000000 rpa_helpers_btime-1.0.9/rpa_helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:09:36.289703 rpa_helpers_btime-1.0.9/rpa_helpers/src/
+-rw-rw-rw-   0        0        0       51 2024-05-21 13:52:57.000000 rpa_helpers_btime-1.0.9/rpa_helpers/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:09:36.289703 rpa_helpers_btime-1.0.9/rpa_helpers/src/configuration/
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.9/rpa_helpers/src/configuration/__init__.py
+-rw-rw-rw-   0        0        0      184 2024-05-21 14:01:28.000000 rpa_helpers_btime-1.0.9/rpa_helpers/src/configuration/configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:09:36.298105 rpa_helpers_btime-1.0.9/rpa_helpers/src/models/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.9/rpa_helpers/src/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:09:36.303653 rpa_helpers_btime-1.0.9/rpa_helpers/src/models/configs/
+-rw-rw-rw-   0        0        0        0 2024-05-14 19:21:02.000000 rpa_helpers_btime-1.0.9/rpa_helpers/src/models/configs/__init__.py
+-rw-rw-rw-   0        0        0       84 2024-05-14 19:23:16.000000 rpa_helpers_btime-1.0.9/rpa_helpers/src/models/configs/base.py
+-rw-rw-rw-   0        0        0      841 2024-05-21 14:03:11.000000 rpa_helpers_btime-1.0.9/rpa_helpers/src/models/configs/connection.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:09:36.303653 rpa_helpers_btime-1.0.9/rpa_helpers/src/models/entities/
+-rw-rw-rw-   0        0        0        0 2024-05-14 19:21:02.000000 rpa_helpers_btime-1.0.9/rpa_helpers/src/models/entities/__init__.py
+-rw-rw-rw-   0        0        0      760 2024-05-21 14:03:36.000000 rpa_helpers_btime-1.0.9/rpa_helpers/src/models/entities/log.py
+-rw-rw-rw-   0        0        0      297 2024-05-21 14:03:28.000000 rpa_helpers_btime-1.0.9/rpa_helpers/src/models/entities/rpa.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:09:36.316597 rpa_helpers_btime-1.0.9/rpa_helpers/src/models/repository/
+-rw-rw-rw-   0        0        0        0 2024-05-14 19:21:02.000000 rpa_helpers_btime-1.0.9/rpa_helpers/src/models/repository/__init__.py
+-rw-rw-rw-   0        0        0     1436 2024-05-21 14:03:43.000000 rpa_helpers_btime-1.0.9/rpa_helpers/src/models/repository/repository_log.py
+-rw-rw-rw-   0        0        0      935 2024-05-21 14:03:47.000000 rpa_helpers_btime-1.0.9/rpa_helpers/src/models/repository/repository_rpa.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:09:36.320222 rpa_helpers_btime-1.0.9/rpa_helpers/src/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.9/rpa_helpers/src/utils/__init__.py
+-rw-rw-rw-   0        0        0     3056 2024-05-21 13:53:17.000000 rpa_helpers_btime-1.0.9/rpa_helpers/src/utils/decorator_log.py
+-rw-rw-rw-   0        0        0     1293 2024-05-15 18:18:58.000000 rpa_helpers_btime-1.0.9/rpa_helpers/src/utils/send_email.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:09:36.347766 rpa_helpers_btime-1.0.9/rpa_helpers_btime.egg-info/
+-rw-rw-rw-   0        0        0      773 2024-05-21 14:09:36.000000 rpa_helpers_btime-1.0.9/rpa_helpers_btime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      908 2024-05-21 14:09:36.000000 rpa_helpers_btime-1.0.9/rpa_helpers_btime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:09:36.000000 rpa_helpers_btime-1.0.9/rpa_helpers_btime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      227 2024-05-21 14:09:36.000000 rpa_helpers_btime-1.0.9/rpa_helpers_btime.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 14:09:36.000000 rpa_helpers_btime-1.0.9/rpa_helpers_btime.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:09:36.349830 rpa_helpers_btime-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1170 2024-05-21 14:09:26.000000 rpa_helpers_btime-1.0.9/setup.py
```

### Comparing `rpa_helpers_btime-1.0.8/PKG-INFO` & `rpa_helpers_btime-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-helpers-btime
-Version: 1.0.8
+Version: 1.0.9
 Summary: Esse pacote irá oferecer todas as funcionalidades para auxiliar na programação de rpa.
 Author: Geovanne Zanata
 Author-email: geovanne.zanata@btime.com.br
 Keywords: log,loggers
 License-File: license.txt
 Requires-Dist: colorama==0.4.6
 Requires-Dist: flake8==7.0.0
@@ -14,9 +14,10 @@
 Requires-Dist: setuptools==69.5.1
 Requires-Dist: pycodestyle==2.11.1
 Requires-Dist: pyflakes==3.2.0
 Requires-Dist: SQLAlchemy==2.0.30
 Requires-Dist: typing_extensions==4.11.0
 Requires-Dist: win32-setctime==1.1.0
 Requires-Dist: python-dotenv==0.21.0
+Requires-Dist: psycopg2
 
 Default long description if README.md is not found.
```

### Comparing `rpa_helpers_btime-1.0.8/license.txt` & `rpa_helpers_btime-1.0.9/license.txt`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.8/rpa_helpers/src/models/configs/connection.py` & `rpa_helpers_btime-1.0.9/rpa_helpers/src/models/configs/connection.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.8/rpa_helpers/src/models/entities/log.py` & `rpa_helpers_btime-1.0.9/rpa_helpers/src/models/entities/log.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.8/rpa_helpers/src/models/repository/repository_log.py` & `rpa_helpers_btime-1.0.9/rpa_helpers/src/models/repository/repository_log.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.8/rpa_helpers/src/models/repository/repository_rpa.py` & `rpa_helpers_btime-1.0.9/rpa_helpers/src/models/repository/repository_rpa.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.8/rpa_helpers/src/utils/decorator_log.py` & `rpa_helpers_btime-1.0.9/rpa_helpers/src/utils/decorator_log.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.8/rpa_helpers/src/utils/send_email.py` & `rpa_helpers_btime-1.0.9/rpa_helpers/src/utils/send_email.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.8/rpa_helpers_btime.egg-info/PKG-INFO` & `rpa_helpers_btime-1.0.9/rpa_helpers_btime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-helpers-btime
-Version: 1.0.8
+Version: 1.0.9
 Summary: Esse pacote irá oferecer todas as funcionalidades para auxiliar na programação de rpa.
 Author: Geovanne Zanata
 Author-email: geovanne.zanata@btime.com.br
 Keywords: log,loggers
 License-File: license.txt
 Requires-Dist: colorama==0.4.6
 Requires-Dist: flake8==7.0.0
@@ -14,9 +14,10 @@
 Requires-Dist: setuptools==69.5.1
 Requires-Dist: pycodestyle==2.11.1
 Requires-Dist: pyflakes==3.2.0
 Requires-Dist: SQLAlchemy==2.0.30
 Requires-Dist: typing_extensions==4.11.0
 Requires-Dist: win32-setctime==1.1.0
 Requires-Dist: python-dotenv==0.21.0
+Requires-Dist: psycopg2
 
 Default long description if README.md is not found.
```

### Comparing `rpa_helpers_btime-1.0.8/rpa_helpers_btime.egg-info/SOURCES.txt` & `rpa_helpers_btime-1.0.9/rpa_helpers_btime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.8/setup.py` & `rpa_helpers_btime-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # try:
 #     long_description = Path("README.md").read_text()
 # except FileNotFoundError:
 #     long_description = "Default long description if README.md is not found."
 
 setup(
     name="rpa-helpers-btime",
-    version="1.0.8",
+    version="1.0.9",
     description="Esse pacote irá oferecer todas as funcionalidades para auxiliar na programação de rpa.",
     long_description="Default long description if README.md is not found.",
     author="Geovanne Zanata",
     author_email="geovanne.zanata@btime.com.br",
     keywords=['log', 'loggers'],
     packages=find_packages(),
     install_requires=[
@@ -23,10 +23,11 @@
                 'mccabe==0.7.0',
                 'setuptools==69.5.1',
                 'pycodestyle==2.11.1',
                 'pyflakes==3.2.0',
                 'SQLAlchemy==2.0.30',
                 'typing_extensions==4.11.0',
                 'win32-setctime==1.1.0',
-                'python-dotenv==0.21.0'
+                'python-dotenv==0.21.0',
+                'psycopg2',
             ],
 )
```

