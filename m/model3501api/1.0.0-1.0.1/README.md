# Comparing `tmp/model3501api-1.0.0.tar.gz` & `tmp/model3501api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\model3501api-1.0.0.tar", last modified: Tue May 21 09:23:58 2024, max compression
+gzip compressed data, was "dist\model3501api-1.0.1.tar", last modified: Tue May 21 11:17:01 2024, max compression
```

## Comparing `model3501api-1.0.0.tar` & `model3501api-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 09:23:58.338870 model3501api-1.0.0/
--rw-rw-rw-   0        0        0      465 2024-05-21 09:23:58.336355 model3501api-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      716 2024-05-16 08:39:40.000000 model3501api-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 09:23:58.333359 model3501api-1.0.0/model3501api.egg-info/
--rw-rw-rw-   0        0        0      465 2024-05-21 09:23:58.000000 model3501api-1.0.0/model3501api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2024-05-21 09:23:58.000000 model3501api-1.0.0/model3501api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 09:23:58.000000 model3501api-1.0.0/model3501api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-21 09:23:58.000000 model3501api-1.0.0/model3501api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-21 09:23:58.000000 model3501api-1.0.0/model3501api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 09:23:58.330355 model3501api-1.0.0/model3501lib/
--rw-rw-rw-   0        0        0      557 2024-05-21 07:05:43.000000 model3501api-1.0.0/model3501lib/__init__.py
--rw-rw-rw-   0        0        0     1502 2024-05-21 06:59:38.000000 model3501api-1.0.0/model3501lib/cdstress_off.py
--rw-rw-rw-   0        0        0     1443 2024-05-21 06:58:03.000000 model3501api-1.0.0/model3501lib/cdstress_on.py
--rw-rw-rw-   0        0        0     3123 2024-05-21 06:43:11.000000 model3501api-1.0.0/model3501lib/emulate_charge.py
--rw-rw-rw-   0        0        0     2063 2024-05-21 05:17:14.000000 model3501api-1.0.0/model3501lib/getpower_role.py
--rw-rw-rw-   0        0        0     1762 2024-05-21 05:16:55.000000 model3501api-1.0.0/model3501lib/getrdo.py
--rw-rw-rw-   0        0        0     1582 2024-05-21 07:04:52.000000 model3501api-1.0.0/model3501lib/pdcaptive_cables.py
--rw-rw-rw-   0        0        0     1565 2024-05-21 07:05:26.000000 model3501api-1.0.0/model3501lib/pdcharger_port.py
--rw-rw-rw-   0        0        0     1523 2024-05-21 05:16:38.000000 model3501api-1.0.0/model3501lib/set_speed.py
--rw-rw-rw-   0        0        0       42 2024-05-21 09:23:58.339878 model3501api-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      723 2024-05-21 09:23:43.000000 model3501api-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:17:01.464074 model3501api-1.0.1/
+-rw-rw-rw-   0        0        0     7042 2024-05-21 11:17:01.462071 model3501api-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6582 2024-05-21 11:12:31.000000 model3501api-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 11:17:01.462071 model3501api-1.0.1/model3501api.egg-info/
+-rw-rw-rw-   0        0        0     7042 2024-05-21 11:17:01.000000 model3501api-1.0.1/model3501api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-05-21 11:17:01.000000 model3501api-1.0.1/model3501api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 11:17:01.000000 model3501api-1.0.1/model3501api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-21 11:17:01.000000 model3501api-1.0.1/model3501api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-21 11:17:01.000000 model3501api-1.0.1/model3501api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 11:17:01.461072 model3501api-1.0.1/model3501lib/
+-rw-rw-rw-   0        0        0      557 2024-05-21 07:05:43.000000 model3501api-1.0.1/model3501lib/__init__.py
+-rw-rw-rw-   0        0        0     1502 2024-05-21 06:59:38.000000 model3501api-1.0.1/model3501lib/cdstress_off.py
+-rw-rw-rw-   0        0        0     1443 2024-05-21 06:58:03.000000 model3501api-1.0.1/model3501lib/cdstress_on.py
+-rw-rw-rw-   0        0        0     3123 2024-05-21 06:43:11.000000 model3501api-1.0.1/model3501lib/emulate_charge.py
+-rw-rw-rw-   0        0        0     2063 2024-05-21 05:17:14.000000 model3501api-1.0.1/model3501lib/getpower_role.py
+-rw-rw-rw-   0        0        0     1762 2024-05-21 05:16:55.000000 model3501api-1.0.1/model3501lib/getrdo.py
+-rw-rw-rw-   0        0        0     1582 2024-05-21 07:04:52.000000 model3501api-1.0.1/model3501lib/pdcaptive_cables.py
+-rw-rw-rw-   0        0        0     1565 2024-05-21 07:05:26.000000 model3501api-1.0.1/model3501lib/pdcharger_port.py
+-rw-rw-rw-   0        0        0     1523 2024-05-21 05:16:38.000000 model3501api-1.0.1/model3501lib/set_speed.py
+-rw-rw-rw-   0        0        0       42 2024-05-21 11:17:01.465076 model3501api-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      877 2024-05-21 11:16:35.000000 model3501api-1.0.1/setup.py
```

### Comparing `model3501api-1.0.0/model3501lib/__init__.py` & `model3501api-1.0.1/model3501lib/__init__.py`

 * *Files identical despite different names*

### Comparing `model3501api-1.0.0/model3501lib/cdstress_off.py` & `model3501api-1.0.1/model3501lib/cdstress_off.py`

 * *Files identical despite different names*

### Comparing `model3501api-1.0.0/model3501lib/cdstress_on.py` & `model3501api-1.0.1/model3501lib/cdstress_on.py`

 * *Files identical despite different names*

### Comparing `model3501api-1.0.0/model3501lib/emulate_charge.py` & `model3501api-1.0.1/model3501lib/emulate_charge.py`

 * *Files identical despite different names*

### Comparing `model3501api-1.0.0/model3501lib/getpower_role.py` & `model3501api-1.0.1/model3501lib/getpower_role.py`

 * *Files identical despite different names*

### Comparing `model3501api-1.0.0/model3501lib/getrdo.py` & `model3501api-1.0.1/model3501lib/getrdo.py`

 * *Files identical despite different names*

### Comparing `model3501api-1.0.0/model3501lib/pdcaptive_cables.py` & `model3501api-1.0.1/model3501lib/pdcaptive_cables.py`

 * *Files identical despite different names*

### Comparing `model3501api-1.0.0/model3501lib/pdcharger_port.py` & `model3501api-1.0.1/model3501lib/pdcharger_port.py`

 * *Files identical despite different names*

### Comparing `model3501api-1.0.0/model3501lib/set_speed.py` & `model3501api-1.0.1/model3501lib/set_speed.py`

 * *Files identical despite different names*

