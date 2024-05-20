# Comparing `tmp/pih-web-0.12.tar.gz` & `tmp/pih-web-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-web-0.12.tar", last modified: Wed May 15 04:30:02 2024, max compression
+gzip compressed data, was "pih-web-0.13.tar", last modified: Mon May 20 23:17:12 2024, max compression
```

## Comparing `pih-web-0.12.tar` & `pih-web-0.13.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 04:30:02.866446 pih-web-0.12/
--rw-rw-rw-   0        0        0      377 2024-05-15 04:30:02.788307 pih-web-0.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 04:30:02.146662 pih-web-0.12/WebServerService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-web-0.12/WebServerService/__init__.py
--rw-rw-rw-   0        0        0      151 2024-02-14 00:18:05.000000 pih-web-0.12/WebServerService/__main__.py
--rw-rw-rw-   0        0        0      523 2024-05-15 04:23:07.000000 pih-web-0.12/WebServerService/const.py
--rw-rw-rw-   0        0        0     4960 2024-05-15 04:23:16.000000 pih-web-0.12/WebServerService/service.py
-drwxrwxrwx   0        0        0        0 2024-05-15 04:30:02.757174 pih-web-0.12/pih_web.egg-info/
--rw-rw-rw-   0        0        0      377 2024-05-15 04:30:01.000000 pih-web-0.12/pih_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2024-05-15 04:30:01.000000 pih-web-0.12/pih_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 04:30:01.000000 pih-web-0.12/pih_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-15 04:30:01.000000 pih-web-0.12/pih_web.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2024-05-15 04:30:01.000000 pih-web-0.12/pih_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-15 04:30:01.000000 pih-web-0.12/pih_web.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 04:30:02.866446 pih-web-0.12/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 23:17:12.382248 pih-web-0.13/
+-rw-rw-rw-   0        0        0      377 2024-05-20 23:17:12.366623 pih-web-0.13/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 23:17:11.990595 pih-web-0.13/WebServerService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-web-0.13/WebServerService/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-02-14 00:18:05.000000 pih-web-0.13/WebServerService/__main__.py
+-rw-rw-rw-   0        0        0      523 2024-05-20 22:40:33.000000 pih-web-0.13/WebServerService/const.py
+-rw-rw-rw-   0        0        0     4960 2024-05-15 04:23:16.000000 pih-web-0.13/WebServerService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:17:12.335376 pih-web-0.13/pih_web.egg-info/
+-rw-rw-rw-   0        0        0      377 2024-05-20 23:17:11.000000 pih-web-0.13/pih_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2024-05-20 23:17:11.000000 pih-web-0.13/pih_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 23:17:11.000000 pih-web-0.13/pih_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-20 23:17:11.000000 pih-web-0.13/pih_web.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2024-05-20 23:17:11.000000 pih-web-0.13/pih_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-20 23:17:11.000000 pih-web-0.13/pih_web.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 23:17:12.397876 pih-web-0.13/setup.cfg
```

### Comparing `pih-web-0.12/WebServerService/const.py` & `pih-web-0.13/WebServerService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME: str = "WebServer"
 
 HOST = Hosts.WS255
 
 PACKAGES: tuple[str, ...] = ("fastapi", "uvicorn", "python-multipart", "dicttoxml")
 
-VERSION: str = "0.12"
+VERSION: str = "0.13"
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Web Server service",
     host=HOST.NAME,
     use_standalone=True,
     standalone_name="web",
```

### Comparing `pih-web-0.12/WebServerService/service.py` & `pih-web-0.13/WebServerService/service.py`

 * *Files identical despite different names*

