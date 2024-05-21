# Comparing `tmp/pazok_lib-0.0.0.tar.gz` & `tmp/pazok_lib-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pazok_lib-0.0.0.tar", last modified: Tue May 21 17:03:43 2024, max compression
+gzip compressed data, was "pazok_lib-3.9.tar", last modified: Tue May 21 18:59:29 2024, max compression
```

## Comparing `pazok_lib-0.0.0.tar` & `pazok_lib-3.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 17:03:43.439449 pazok_lib-0.0.0/
--rw-rw-rw-   0        0        0        0 2024-05-21 16:02:56.000000 pazok_lib-0.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      264 2024-05-21 17:03:43.438450 pazok_lib-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      717 2024-05-21 16:42:50.000000 pazok_lib-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 17:03:43.437321 pazok_lib-0.0.0/pazok_lib.egg-info/
--rw-rw-rw-   0        0        0      264 2024-05-21 17:03:43.000000 pazok_lib-0.0.0/pazok_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2024-05-21 17:03:43.000000 pazok_lib-0.0.0/pazok_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 17:03:43.000000 pazok_lib-0.0.0/pazok_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 17:03:43.000000 pazok_lib-0.0.0/pazok_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 17:03:43.440449 pazok_lib-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      350 2024-05-21 17:02:54.000000 pazok_lib-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:59:29.077574 pazok_lib-3.9/
+-rw-rw-rw-   0        0        0       29 2024-05-21 18:45:40.000000 pazok_lib-3.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      888 2024-05-21 18:59:29.074581 pazok_lib-3.9/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2024-05-21 16:42:50.000000 pazok_lib-3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 18:59:29.070592 pazok_lib-3.9/pazok_lib.egg-info/
+-rw-rw-rw-   0        0        0      888 2024-05-21 18:59:29.000000 pazok_lib-3.9/pazok_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2024-05-21 18:59:29.000000 pazok_lib-3.9/pazok_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 18:59:29.000000 pazok_lib-3.9/pazok_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 18:59:29.000000 pazok_lib-3.9/pazok_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 18:59:29.077574 pazok_lib-3.9/setup.cfg
+-rw-rw-rw-   0        0        0      361 2024-05-21 18:58:43.000000 pazok_lib-3.9/setup.py
```

### Comparing `pazok_lib-0.0.0/README.md` & `pazok_lib-3.9/README.md`

 * *Files identical despite different names*

