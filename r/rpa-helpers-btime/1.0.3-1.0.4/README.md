# Comparing `tmp/rpa_helpers_btime-1.0.3.tar.gz` & `tmp/rpa_helpers_btime-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_helpers_btime-1.0.3.tar", last modified: Tue May 21 13:45:56 2024, max compression
+gzip compressed data, was "rpa_helpers_btime-1.0.4.tar", last modified: Tue May 21 13:50:29 2024, max compression
```

## Comparing `rpa_helpers_btime-1.0.3.tar` & `rpa_helpers_btime-1.0.4.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 13:45:56.115684 rpa_helpers_btime-1.0.3/
--rw-rw-rw-   0        0        0      338 2024-05-21 13:45:56.113689 rpa_helpers_btime-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1058 2024-05-21 12:29:56.000000 rpa_helpers_btime-1.0.3/license.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 13:45:56.057299 rpa_helpers_btime-1.0.3/rpa_helpers/
--rw-rw-rw-   0        0        0       23 2024-05-21 13:44:36.000000 rpa_helpers_btime-1.0.3/rpa_helpers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:45:56.059300 rpa_helpers_btime-1.0.3/rpa_helpers/src/
--rw-rw-rw-   0        0        0       39 2024-05-15 20:17:49.000000 rpa_helpers_btime-1.0.3/rpa_helpers/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:45:56.062980 rpa_helpers_btime-1.0.3/rpa_helpers/src/configuration/
--rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.3/rpa_helpers/src/configuration/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-15 18:25:35.000000 rpa_helpers_btime-1.0.3/rpa_helpers/src/configuration/configuration.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:45:56.064989 rpa_helpers_btime-1.0.3/rpa_helpers/src/models/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.3/rpa_helpers/src/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:45:56.068985 rpa_helpers_btime-1.0.3/rpa_helpers/src/models/configs/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.3/rpa_helpers/src/models/configs/__init__.py
--rw-rw-rw-   0        0        0       88 2024-05-15 18:09:08.000000 rpa_helpers_btime-1.0.3/rpa_helpers/src/models/configs/base.py
--rw-rw-rw-   0        0        0      763 2024-05-15 18:09:28.000000 rpa_helpers_btime-1.0.3/rpa_helpers/src/models/configs/connection.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:45:56.075575 rpa_helpers_btime-1.0.3/rpa_helpers/src/models/entities/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.3/rpa_helpers/src/models/entities/__init__.py
--rw-rw-rw-   0        0        0      703 2024-05-15 18:10:41.000000 rpa_helpers_btime-1.0.3/rpa_helpers/src/models/entities/log.py
--rw-rw-rw-   0        0        0      305 2024-05-15 18:10:51.000000 rpa_helpers_btime-1.0.3/rpa_helpers/src/models/entities/rpa.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:45:56.082440 rpa_helpers_btime-1.0.3/rpa_helpers/src/models/repository/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.3/rpa_helpers/src/models/repository/__init__.py
--rw-rw-rw-   0        0        0     1325 2024-05-15 18:24:48.000000 rpa_helpers_btime-1.0.3/rpa_helpers/src/models/repository/repository_log.py
--rw-rw-rw-   0        0        0      853 2024-05-15 18:13:23.000000 rpa_helpers_btime-1.0.3/rpa_helpers/src/models/repository/repository_rpa.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:45:56.087442 rpa_helpers_btime-1.0.3/rpa_helpers/src/utils/
--rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.3/rpa_helpers/src/utils/__init__.py
--rw-rw-rw-   0        0        0     3032 2024-05-21 12:22:41.000000 rpa_helpers_btime-1.0.3/rpa_helpers/src/utils/decorator_log.py
--rw-rw-rw-   0        0        0     1293 2024-05-15 18:18:58.000000 rpa_helpers_btime-1.0.3/rpa_helpers/src/utils/send_email.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:45:56.111665 rpa_helpers_btime-1.0.3/rpa_helpers_btime.egg-info/
--rw-rw-rw-   0        0        0      338 2024-05-21 13:45:55.000000 rpa_helpers_btime-1.0.3/rpa_helpers_btime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      868 2024-05-21 13:45:55.000000 rpa_helpers_btime-1.0.3/rpa_helpers_btime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 13:45:55.000000 rpa_helpers_btime-1.0.3/rpa_helpers_btime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-21 13:45:55.000000 rpa_helpers_btime-1.0.3/rpa_helpers_btime.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 13:45:56.116688 rpa_helpers_btime-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      643 2024-05-21 13:44:49.000000 rpa_helpers_btime-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.448415 rpa_helpers_btime-1.0.4/
+-rw-rw-rw-   0        0        0      776 2024-05-21 13:50:29.446386 rpa_helpers_btime-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1058 2024-05-21 12:29:56.000000 rpa_helpers_btime-1.0.4/license.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.368676 rpa_helpers_btime-1.0.4/rpa_helpers/
+-rw-rw-rw-   0        0        0       23 2024-05-21 13:44:36.000000 rpa_helpers_btime-1.0.4/rpa_helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.370679 rpa_helpers_btime-1.0.4/rpa_helpers/src/
+-rw-rw-rw-   0        0        0       39 2024-05-15 20:17:49.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.374694 rpa_helpers_btime-1.0.4/rpa_helpers/src/configuration/
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/configuration/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-15 18:25:35.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/configuration/configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.375678 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.381600 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/configs/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/configs/__init__.py
+-rw-rw-rw-   0        0        0       88 2024-05-15 18:09:08.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/configs/base.py
+-rw-rw-rw-   0        0        0      763 2024-05-15 18:09:28.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/configs/connection.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.387601 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/entities/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/entities/__init__.py
+-rw-rw-rw-   0        0        0      703 2024-05-15 18:10:41.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/entities/log.py
+-rw-rw-rw-   0        0        0      305 2024-05-15 18:10:51.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/entities/rpa.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.393600 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/repository/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/repository/__init__.py
+-rw-rw-rw-   0        0        0     1325 2024-05-15 18:24:48.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/repository/repository_log.py
+-rw-rw-rw-   0        0        0      853 2024-05-15 18:13:23.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/models/repository/repository_rpa.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.398599 rpa_helpers_btime-1.0.4/rpa_helpers/src/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/utils/__init__.py
+-rw-rw-rw-   0        0        0     3032 2024-05-21 12:22:41.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/utils/decorator_log.py
+-rw-rw-rw-   0        0        0     1293 2024-05-15 18:18:58.000000 rpa_helpers_btime-1.0.4/rpa_helpers/src/utils/send_email.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:50:29.442646 rpa_helpers_btime-1.0.4/rpa_helpers_btime.egg-info/
+-rw-rw-rw-   0        0        0      776 2024-05-21 13:50:29.000000 rpa_helpers_btime-1.0.4/rpa_helpers_btime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      908 2024-05-21 13:50:29.000000 rpa_helpers_btime-1.0.4/rpa_helpers_btime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 13:50:29.000000 rpa_helpers_btime-1.0.4/rpa_helpers_btime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      230 2024-05-21 13:50:29.000000 rpa_helpers_btime-1.0.4/rpa_helpers_btime.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 13:50:29.000000 rpa_helpers_btime-1.0.4/rpa_helpers_btime.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 13:50:29.449413 rpa_helpers_btime-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2024-05-21 13:50:18.000000 rpa_helpers_btime-1.0.4/setup.py
```

### Comparing `rpa_helpers_btime-1.0.3/license.txt` & `rpa_helpers_btime-1.0.4/license.txt`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.3/rpa_helpers/src/models/configs/connection.py` & `rpa_helpers_btime-1.0.4/rpa_helpers/src/models/configs/connection.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.3/rpa_helpers/src/models/entities/log.py` & `rpa_helpers_btime-1.0.4/rpa_helpers/src/models/entities/log.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.3/rpa_helpers/src/models/repository/repository_log.py` & `rpa_helpers_btime-1.0.4/rpa_helpers/src/models/repository/repository_log.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.3/rpa_helpers/src/models/repository/repository_rpa.py` & `rpa_helpers_btime-1.0.4/rpa_helpers/src/models/repository/repository_rpa.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.3/rpa_helpers/src/utils/decorator_log.py` & `rpa_helpers_btime-1.0.4/rpa_helpers/src/utils/decorator_log.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.3/rpa_helpers/src/utils/send_email.py` & `rpa_helpers_btime-1.0.4/rpa_helpers/src/utils/send_email.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.3/rpa_helpers_btime.egg-info/SOURCES.txt` & `rpa_helpers_btime-1.0.4/rpa_helpers_btime.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 rpa_helpers/src/models/repository/repository_rpa.py
 rpa_helpers/src/utils/__init__.py
 rpa_helpers/src/utils/decorator_log.py
 rpa_helpers/src/utils/send_email.py
 rpa_helpers_btime.egg-info/PKG-INFO
 rpa_helpers_btime.egg-info/SOURCES.txt
 rpa_helpers_btime.egg-info/dependency_links.txt
+rpa_helpers_btime.egg-info/requires.txt
 rpa_helpers_btime.egg-info/top_level.txt
```

