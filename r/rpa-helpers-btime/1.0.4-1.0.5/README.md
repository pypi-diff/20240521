# Comparing `tmp/rpa_helpers_btime-1.0.4.tar.gz` & `tmp/rpa_helpers_btime-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_helpers_btime-1.0.4.tar", last modified: Tue May 21 13:50:29 2024, max compression
+gzip compressed data, was "rpa_helpers_btime-1.0.5.tar", last modified: Tue May 21 13:52:10 2024, max compression
```

## Comparing `rpa_helpers_btime-1.0.4.tar` & `rpa_helpers_btime-1.0.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.448415 rpa_helpers_btime-1.0.4/
--rw-rw-rw-   0        0        0      776 2024-05-21 13:50:29.446386 rpa_helpers_btime-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1058 2024-05-21 12:29:56.000000 rpa_helpers_btime-1.0.4/license.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.368676 rpa_helpers_btime-1.0.4/rpa_helpers/
--rw-rw-rw-   0        0        0       23 2024-05-21 13:44:36.000000 rpa_helpers_btime-1.0.4/rpa_helpers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.370679 rpa_helpers_btime-1.0.4/rpa_helpers/src/
--rw-rw-rw-   0        0        0       39 2024-05-15 20:17:49.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.374694 rpa_helpers_btime-1.0.4/rpa_helpers/src/configuration/
--rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/configuration/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-15 18:25:35.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/configuration/configuration.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.375678 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.381600 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/configs/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/configs/__init__.py
--rw-rw-rw-   0        0        0       88 2024-05-15 18:09:08.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/configs/base.py
--rw-rw-rw-   0        0        0      763 2024-05-15 18:09:28.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/configs/connection.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.387601 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/entities/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/entities/__init__.py
--rw-rw-rw-   0        0        0      703 2024-05-15 18:10:41.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/entities/log.py
--rw-rw-rw-   0        0        0      305 2024-05-15 18:10:51.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/entities/rpa.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.393600 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/repository/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/repository/__init__.py
--rw-rw-rw-   0        0        0     1325 2024-05-15 18:24:48.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/repository/repository_log.py
--rw-rw-rw-   0        0        0      853 2024-05-15 18:13:23.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/repository/repository_rpa.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.398599 rpa_helpers_btime-1.0.4/rpa_helpers/src/utils/
--rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/utils/__init__.py
--rw-rw-rw-   0        0        0     3032 2024-05-21 12:22:41.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/utils/decorator_log.py
--rw-rw-rw-   0        0        0     1293 2024-05-15 18:18:58.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/utils/send_email.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.442646 rpa_helpers_btime-1.0.4/rpa_helpers_btime.egg-info/
--rw-rw-rw-   0        0        0      776 2024-05-21 13:50:29.000000 rpa_helpers_btime-1.0.4/rpa_helpers_btime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      908 2024-05-21 13:50:29.000000 rpa_helpers_btime-1.0.4/rpa_helpers_btime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 13:50:29.000000 rpa_helpers_btime-1.0.4/rpa_helpers_btime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      230 2024-05-21 13:50:29.000000 rpa_helpers_btime-1.0.4/rpa_helpers_btime.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-21 13:50:29.000000 rpa_helpers_btime-1.0.4/rpa_helpers_btime.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 13:50:29.449413 rpa_helpers_btime-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1173 2024-05-21 13:50:18.000000 rpa_helpers_btime-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.909069 rpa_helpers_btime-1.0.5/
+-rw-rw-rw-   0        0        0      743 2024-05-21 13:52:10.907068 rpa_helpers_btime-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1058 2024-05-21 12:29:56.000000 rpa_helpers_btime-1.0.5/license.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.815982 rpa_helpers_btime-1.0.5/rpa_helpers/
+-rw-rw-rw-   0        0        0       23 2024-05-21 13:44:36.000000 rpa_helpers_btime-1.0.5/rpa_helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.817982 rpa_helpers_btime-1.0.5/rpa_helpers/src/
+-rw-rw-rw-   0        0        0       39 2024-05-15 20:17:49.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.823006 rpa_helpers_btime-1.0.5/rpa_helpers/src/configuration/
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/configuration/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-15 18:25:35.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/configuration/configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.824988 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.832969 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/configs/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/configs/__init__.py
+-rw-rw-rw-   0        0        0       88 2024-05-15 18:09:08.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/configs/base.py
+-rw-rw-rw-   0        0        0      763 2024-05-15 18:09:28.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/configs/connection.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.837361 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/entities/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/entities/__init__.py
+-rw-rw-rw-   0        0        0      703 2024-05-15 18:10:41.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/entities/log.py
+-rw-rw-rw-   0        0        0      305 2024-05-15 18:10:51.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/entities/rpa.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.858221 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/repository/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/repository/__init__.py
+-rw-rw-rw-   0        0        0     1325 2024-05-15 18:24:48.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/repository/repository_log.py
+-rw-rw-rw-   0        0        0      853 2024-05-15 18:13:23.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/repository/repository_rpa.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.865225 rpa_helpers_btime-1.0.5/rpa_helpers/src/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/utils/__init__.py
+-rw-rw-rw-   0        0        0     3032 2024-05-21 12:22:41.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/utils/decorator_log.py
+-rw-rw-rw-   0        0        0     1293 2024-05-15 18:18:58.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/utils/send_email.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.905065 rpa_helpers_btime-1.0.5/rpa_helpers_btime.egg-info/
+-rw-rw-rw-   0        0        0      743 2024-05-21 13:52:10.000000 rpa_helpers_btime-1.0.5/rpa_helpers_btime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      908 2024-05-21 13:52:10.000000 rpa_helpers_btime-1.0.5/rpa_helpers_btime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 13:52:10.000000 rpa_helpers_btime-1.0.5/rpa_helpers_btime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      213 2024-05-21 13:52:10.000000 rpa_helpers_btime-1.0.5/rpa_helpers_btime.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 13:52:10.000000 rpa_helpers_btime-1.0.5/rpa_helpers_btime.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 13:52:10.910068 rpa_helpers_btime-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1136 2024-05-21 13:52:08.000000 rpa_helpers_btime-1.0.5/setup.py
```

### Comparing `rpa_helpers_btime-1.0.4/PKG-INFO` & `rpa_helpers_btime-1.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-helpers-btime
-Version: 1.0.4
+Version: 1.0.5
 Summary: Esse pacote irá oferecer todas as funcionalidades para auxiliar na programação de rpa.
 Author: Geovanne Zanata
 Author-email: geovanne.zanata@btime.com.br
 Keywords: log,loggers
 License-File: license.txt
 Requires-Dist: colorama==0.4.6
 Requires-Dist: flake8==7.0.0
@@ -14,10 +14,9 @@
 Requires-Dist: rpa_helpers==1.0
 Requires-Dist: setuptools==69.5.1
 Requires-Dist: pycodestyle==2.11.1
 Requires-Dist: pyflakes==3.2.0
 Requires-Dist: SQLAlchemy==2.0.30
 Requires-Dist: typing_extensions==4.11.0
 Requires-Dist: win32-setctime==1.1.0
-Requires-Dist: rpa_helpers==1.0
 
 Default long description if README.md is not found.
```

### Comparing `rpa_helpers_btime-1.0.4/license.txt` & `rpa_helpers_btime-1.0.5/license.txt`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.4/rpa_helpers/src/models/configs/connection.py` & `rpa_helpers_btime-1.0.5/rpa_helpers/src/models/configs/connection.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.4/rpa_helpers/src/models/entities/log.py` & `rpa_helpers_btime-1.0.5/rpa_helpers/src/models/entities/log.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.4/rpa_helpers/src/models/repository/repository_log.py` & `rpa_helpers_btime-1.0.5/rpa_helpers/src/models/repository/repository_log.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.4/rpa_helpers/src/models/repository/repository_rpa.py` & `rpa_helpers_btime-1.0.5/rpa_helpers/src/models/repository/repository_rpa.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.4/rpa_helpers/src/utils/decorator_log.py` & `rpa_helpers_btime-1.0.5/rpa_helpers/src/utils/decorator_log.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.4/rpa_helpers/src/utils/send_email.py` & `rpa_helpers_btime-1.0.5/rpa_helpers/src/utils/send_email.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.4/rpa_helpers_btime.egg-info/PKG-INFO` & `rpa_helpers_btime-1.0.5/rpa_helpers_btime.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-helpers-btime
-Version: 1.0.4
+Version: 1.0.5
 Summary: Esse pacote irá oferecer todas as funcionalidades para auxiliar na programação de rpa.
 Author: Geovanne Zanata
 Author-email: geovanne.zanata@btime.com.br
 Keywords: log,loggers
 License-File: license.txt
 Requires-Dist: colorama==0.4.6
 Requires-Dist: flake8==7.0.0
@@ -14,10 +14,9 @@
 Requires-Dist: rpa_helpers==1.0
 Requires-Dist: setuptools==69.5.1
 Requires-Dist: pycodestyle==2.11.1
 Requires-Dist: pyflakes==3.2.0
 Requires-Dist: SQLAlchemy==2.0.30
 Requires-Dist: typing_extensions==4.11.0
 Requires-Dist: win32-setctime==1.1.0
-Requires-Dist: rpa_helpers==1.0
 
 Default long description if README.md is not found.
```

### Comparing `rpa_helpers_btime-1.0.4/rpa_helpers_btime.egg-info/SOURCES.txt` & `rpa_helpers_btime-1.0.5/rpa_helpers_btime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.4/setup.py` & `rpa_helpers_btime-1.0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # try:
 #     long_description = Path("README.md").read_text()
 # except FileNotFoundError:
 #     long_description = "Default long description if README.md is not found."
 
 setup(
     name="rpa-helpers-btime",
-    version="1.0.4",
+    version="1.0.5",
     description="Esse pacote irá oferecer todas as funcionalidades para auxiliar na programação de rpa.",
     long_description="Default long description if README.md is not found.",
     author="Geovanne Zanata",
     author_email="geovanne.zanata@btime.com.br",
     keywords=['log', 'loggers'],
     packages=find_packages(),
     install_requires=[
@@ -24,10 +24,9 @@
                 'rpa_helpers==1.0',
                 'setuptools==69.5.1',
                 'pycodestyle==2.11.1',
                 'pyflakes==3.2.0',
                 'SQLAlchemy==2.0.30',
                 'typing_extensions==4.11.0',
                 'win32-setctime==1.1.0',
-                'rpa_helpers==1.0',
             ],
 )
```

