# Comparing `tmp/rpa_helpers_btime-1.0.0.tar.gz` & `tmp/rpa_helpers_btime-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_helpers_btime-1.0.0.tar", last modified: Tue May 21 12:44:25 2024, max compression
+gzip compressed data, was "rpa_helpers_btime-1.0.1.tar", last modified: Tue May 21 13:37:11 2024, max compression
```

## Comparing `rpa_helpers_btime-1.0.0.tar` & `rpa_helpers_btime-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 12:44:25.154560 rpa_helpers_btime-1.0.0/
--rw-rw-rw-   0        0        0      432 2024-05-21 12:44:25.151554 rpa_helpers_btime-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1058 2024-05-21 12:29:56.000000 rpa_helpers_btime-1.0.0/license.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 12:44:25.073218 rpa_helpers_btime-1.0.0/rpa_helpers/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:22:04.000000 rpa_helpers_btime-1.0.0/rpa_helpers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:44:25.075215 rpa_helpers_btime-1.0.0/rpa_helpers/src/
--rw-rw-rw-   0        0        0       39 2024-05-15 20:17:49.000000 rpa_helpers_btime-1.0.0/rpa_helpers/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:44:25.079140 rpa_helpers_btime-1.0.0/rpa_helpers/src/configuration/
--rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.0/rpa_helpers/src/configuration/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-15 18:25:35.000000 rpa_helpers_btime-1.0.0/rpa_helpers/src/configuration/configuration.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:44:25.081417 rpa_helpers_btime-1.0.0/rpa_helpers/src/models/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.0/rpa_helpers/src/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:44:25.087421 rpa_helpers_btime-1.0.0/rpa_helpers/src/models/configs/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.0/rpa_helpers/src/models/configs/__init__.py
--rw-rw-rw-   0        0        0       88 2024-05-15 18:09:08.000000 rpa_helpers_btime-1.0.0/rpa_helpers/src/models/configs/base.py
--rw-rw-rw-   0        0        0      763 2024-05-15 18:09:28.000000 rpa_helpers_btime-1.0.0/rpa_helpers/src/models/configs/connection.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:44:25.093545 rpa_helpers_btime-1.0.0/rpa_helpers/src/models/entities/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.0/rpa_helpers/src/models/entities/__init__.py
--rw-rw-rw-   0        0        0      703 2024-05-15 18:10:41.000000 rpa_helpers_btime-1.0.0/rpa_helpers/src/models/entities/log.py
--rw-rw-rw-   0        0        0      305 2024-05-15 18:10:51.000000 rpa_helpers_btime-1.0.0/rpa_helpers/src/models/entities/rpa.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:44:25.100471 rpa_helpers_btime-1.0.0/rpa_helpers/src/models/repository/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.0/rpa_helpers/src/models/repository/__init__.py
--rw-rw-rw-   0        0        0     1325 2024-05-15 18:24:48.000000 rpa_helpers_btime-1.0.0/rpa_helpers/src/models/repository/repository_log.py
--rw-rw-rw-   0        0        0      853 2024-05-15 18:13:23.000000 rpa_helpers_btime-1.0.0/rpa_helpers/src/models/repository/repository_rpa.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:44:25.107443 rpa_helpers_btime-1.0.0/rpa_helpers/src/utils/
--rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.0/rpa_helpers/src/utils/__init__.py
--rw-rw-rw-   0        0        0     3032 2024-05-21 12:22:41.000000 rpa_helpers_btime-1.0.0/rpa_helpers/src/utils/decorator_log.py
--rw-rw-rw-   0        0        0     1293 2024-05-15 18:18:58.000000 rpa_helpers_btime-1.0.0/rpa_helpers/src/utils/send_email.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:44:25.148521 rpa_helpers_btime-1.0.0/rpa_helpers_btime.egg-info/
--rw-rw-rw-   0        0        0      432 2024-05-21 12:44:24.000000 rpa_helpers_btime-1.0.0/rpa_helpers_btime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      868 2024-05-21 12:44:24.000000 rpa_helpers_btime-1.0.0/rpa_helpers_btime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 12:44:24.000000 rpa_helpers_btime-1.0.0/rpa_helpers_btime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-21 12:44:24.000000 rpa_helpers_btime-1.0.0/rpa_helpers_btime.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 12:44:25.155571 rpa_helpers_btime-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      444 2024-05-21 12:34:56.000000 rpa_helpers_btime-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:37:11.782921 rpa_helpers_btime-1.0.1/
+-rw-rw-rw-   0        0        0      338 2024-05-21 13:37:11.780909 rpa_helpers_btime-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1058 2024-05-21 12:29:56.000000 rpa_helpers_btime-1.0.1/license.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 13:37:11.715637 rpa_helpers_btime-1.0.1/rpa_helpers/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:22:04.000000 rpa_helpers_btime-1.0.1/rpa_helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:37:11.716638 rpa_helpers_btime-1.0.1/rpa_helpers/src/
+-rw-rw-rw-   0        0        0       39 2024-05-15 20:17:49.000000 rpa_helpers_btime-1.0.1/rpa_helpers/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:37:11.720636 rpa_helpers_btime-1.0.1/rpa_helpers/src/configuration/
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.1/rpa_helpers/src/configuration/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-15 18:25:35.000000 rpa_helpers_btime-1.0.1/rpa_helpers/src/configuration/configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:37:11.723230 rpa_helpers_btime-1.0.1/rpa_helpers/src/models/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.1/rpa_helpers/src/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:37:11.729240 rpa_helpers_btime-1.0.1/rpa_helpers/src/models/configs/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.1/rpa_helpers/src/models/configs/__init__.py
+-rw-rw-rw-   0        0        0       88 2024-05-15 18:09:08.000000 rpa_helpers_btime-1.0.1/rpa_helpers/src/models/configs/base.py
+-rw-rw-rw-   0        0        0      763 2024-05-15 18:09:28.000000 rpa_helpers_btime-1.0.1/rpa_helpers/src/models/configs/connection.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:37:11.735742 rpa_helpers_btime-1.0.1/rpa_helpers/src/models/entities/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.1/rpa_helpers/src/models/entities/__init__.py
+-rw-rw-rw-   0        0        0      703 2024-05-15 18:10:41.000000 rpa_helpers_btime-1.0.1/rpa_helpers/src/models/entities/log.py
+-rw-rw-rw-   0        0        0      305 2024-05-15 18:10:51.000000 rpa_helpers_btime-1.0.1/rpa_helpers/src/models/entities/rpa.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:37:11.743692 rpa_helpers_btime-1.0.1/rpa_helpers/src/models/repository/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.1/rpa_helpers/src/models/repository/__init__.py
+-rw-rw-rw-   0        0        0     1325 2024-05-15 18:24:48.000000 rpa_helpers_btime-1.0.1/rpa_helpers/src/models/repository/repository_log.py
+-rw-rw-rw-   0        0        0      853 2024-05-15 18:13:23.000000 rpa_helpers_btime-1.0.1/rpa_helpers/src/models/repository/repository_rpa.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:37:11.752226 rpa_helpers_btime-1.0.1/rpa_helpers/src/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.1/rpa_helpers/src/utils/__init__.py
+-rw-rw-rw-   0        0        0     3032 2024-05-21 12:22:41.000000 rpa_helpers_btime-1.0.1/rpa_helpers/src/utils/decorator_log.py
+-rw-rw-rw-   0        0        0     1293 2024-05-15 18:18:58.000000 rpa_helpers_btime-1.0.1/rpa_helpers/src/utils/send_email.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:37:11.778027 rpa_helpers_btime-1.0.1/rpa_helpers_btime.egg-info/
+-rw-rw-rw-   0        0        0      338 2024-05-21 13:37:11.000000 rpa_helpers_btime-1.0.1/rpa_helpers_btime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2024-05-21 13:37:11.000000 rpa_helpers_btime-1.0.1/rpa_helpers_btime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 13:37:11.000000 rpa_helpers_btime-1.0.1/rpa_helpers_btime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 13:37:11.000000 rpa_helpers_btime-1.0.1/rpa_helpers_btime.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 13:37:11.783925 rpa_helpers_btime-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      643 2024-05-21 13:35:03.000000 rpa_helpers_btime-1.0.1/setup.py
```

### Comparing `rpa_helpers_btime-1.0.0/license.txt` & `rpa_helpers_btime-1.0.1/license.txt`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.0/rpa_helpers/src/models/configs/connection.py` & `rpa_helpers_btime-1.0.1/rpa_helpers/src/models/configs/connection.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.0/rpa_helpers/src/models/entities/log.py` & `rpa_helpers_btime-1.0.1/rpa_helpers/src/models/entities/log.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.0/rpa_helpers/src/models/repository/repository_log.py` & `rpa_helpers_btime-1.0.1/rpa_helpers/src/models/repository/repository_log.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.0/rpa_helpers/src/models/repository/repository_rpa.py` & `rpa_helpers_btime-1.0.1/rpa_helpers/src/models/repository/repository_rpa.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.0/rpa_helpers/src/utils/decorator_log.py` & `rpa_helpers_btime-1.0.1/rpa_helpers/src/utils/decorator_log.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.0/rpa_helpers/src/utils/send_email.py` & `rpa_helpers_btime-1.0.1/rpa_helpers/src/utils/send_email.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.0/rpa_helpers_btime.egg-info/SOURCES.txt` & `rpa_helpers_btime-1.0.1/rpa_helpers_btime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

