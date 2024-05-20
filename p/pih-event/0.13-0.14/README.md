# Comparing `tmp/pih-event-0.13.tar.gz` & `tmp/pih-event-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-event-0.13.tar", last modified: Wed Apr 10 22:15:38 2024, max compression
+gzip compressed data, was "pih-event-0.14.tar", last modified: Mon May 20 22:50:54 2024, max compression
```

## Comparing `pih-event-0.13.tar` & `pih-event-0.14.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 22:15:38.430850 pih-event-0.13/
-drwxrwxrwx   0        0        0        0 2024-04-10 22:15:37.588012 pih-event-0.13/EventService/
--rw-rw-rw-   0        0        0       26 2024-02-15 08:19:09.000000 pih-event-0.13/EventService/__init__.py
--rw-rw-rw-   0        0        0      147 2024-02-15 07:53:14.000000 pih-event-0.13/EventService/__main__.py
--rw-rw-rw-   0        0        0     5922 2024-04-10 22:03:57.000000 pih-event-0.13/EventService/api.py
--rw-rw-rw-   0        0        0      573 2024-04-10 22:10:47.000000 pih-event-0.13/EventService/const.py
--rw-rw-rw-   0        0        0     1986 2024-03-13 14:07:46.000000 pih-event-0.13/EventService/service.py
--rw-rw-rw-   0        0        0      305 2024-04-10 22:15:38.383961 pih-event-0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 22:15:38.355678 pih-event-0.13/pih_event.egg-info/
--rw-rw-rw-   0        0        0      305 2024-04-10 22:15:37.000000 pih-event-0.13/pih_event.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2024-04-10 22:15:37.000000 pih-event-0.13/pih_event.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 22:15:37.000000 pih-event-0.13/pih_event.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-04-10 22:15:37.000000 pih-event-0.13/pih_event.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-04-10 22:15:37.000000 pih-event-0.13/pih_event.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-10 22:15:37.000000 pih-event-0.13/pih_event.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 22:15:38.446473 pih-event-0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 22:50:54.182740 pih-event-0.14/
+drwxrwxrwx   0        0        0        0 2024-05-20 22:50:53.751860 pih-event-0.14/EventService/
+-rw-rw-rw-   0        0        0       26 2024-02-15 08:19:09.000000 pih-event-0.14/EventService/__init__.py
+-rw-rw-rw-   0        0        0      147 2024-02-15 07:53:14.000000 pih-event-0.14/EventService/__main__.py
+-rw-rw-rw-   0        0        0     5922 2024-04-10 22:03:57.000000 pih-event-0.14/EventService/api.py
+-rw-rw-rw-   0        0        0      573 2024-05-20 22:38:29.000000 pih-event-0.14/EventService/const.py
+-rw-rw-rw-   0        0        0     1986 2024-03-13 14:07:46.000000 pih-event-0.14/EventService/service.py
+-rw-rw-rw-   0        0        0      305 2024-05-20 22:50:54.151521 pih-event-0.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 22:50:54.104615 pih-event-0.14/pih_event.egg-info/
+-rw-rw-rw-   0        0        0      305 2024-05-20 22:50:52.000000 pih-event-0.14/pih_event.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2024-05-20 22:50:53.000000 pih-event-0.14/pih_event.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 22:50:52.000000 pih-event-0.14/pih_event.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-20 22:50:52.000000 pih-event-0.14/pih_event.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-20 22:50:52.000000 pih-event-0.14/pih_event.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-20 22:50:52.000000 pih-event-0.14/pih_event.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 22:50:54.245241 pih-event-0.14/setup.cfg
```

### Comparing `pih-event-0.13/EventService/api.py` & `pih-event-0.14/EventService/api.py`

 * *Files identical despite different names*

### Comparing `pih-event-0.13/EventService/const.py` & `pih-event-0.14/EventService/const.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pih.collections.service import ServiceDescription
 
 
 NAME: str = "Event"
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.13"
+VERSION: str = "0.14"
 
 CONFIG_FOLDER_NAME: str = "telegram_send_config"
 
 PACKAGES: tuple[str, ...] = ("telegram-send",)
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
```

### Comparing `pih-event-0.13/EventService/service.py` & `pih-event-0.14/EventService/service.py`

 * *Files identical despite different names*

