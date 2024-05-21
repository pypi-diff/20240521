# Comparing `tmp/jzai-59.83.53.tar.gz` & `tmp/jzai-59.83.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzai-59.83.53.tar", last modified: Mon May 20 09:00:28 2024, max compression
+gzip compressed data, was "jzai-59.83.54.tar", last modified: Tue May 21 04:04:07 2024, max compression
```

## Comparing `jzai-59.83.53.tar` & `jzai-59.83.54.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 09:00:28.474984 jzai-59.83.53/
--rw-rw-rw-   0        0        0      275 2024-05-20 09:00:28.473973 jzai-59.83.53/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.53/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 09:00:28.452016 jzai-59.83.53/jzai/
--rw-rw-rw-   0        0        0       38 2024-05-20 08:34:39.000000 jzai-59.83.53/jzai/__init__.py
--rw-rw-rw-   0        0        0     7750 2024-05-20 08:58:58.000000 jzai-59.83.53/jzai/bot.py
--rw-rw-rw-   0        0        0      179 2024-05-20 09:00:13.000000 jzai-59.83.53/jzai/cli.py
--rw-rw-rw-   0        0        0      875 2024-05-20 08:31:32.000000 jzai-59.83.53/jzai/db.py
--rw-rw-rw-   0        0        0      248 2024-05-20 08:31:36.000000 jzai-59.83.53/jzai/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-20 09:00:28.472572 jzai-59.83.53/jzai.egg-info/
--rw-rw-rw-   0        0        0      275 2024-05-20 09:00:28.000000 jzai-59.83.53/jzai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-20 09:00:28.000000 jzai-59.83.53/jzai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 09:00:28.000000 jzai-59.83.53/jzai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-20 09:00:28.000000 jzai-59.83.53/jzai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2024-05-20 09:00:28.000000 jzai-59.83.53/jzai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-20 09:00:28.000000 jzai-59.83.53/jzai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 09:00:28.474984 jzai-59.83.53/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-20 09:00:24.000000 jzai-59.83.53/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:04:07.782897 jzai-59.83.54/
+-rw-rw-rw-   0        0        0      275 2024-05-21 04:04:07.781905 jzai-59.83.54/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.54/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 04:04:07.741017 jzai-59.83.54/jzai/
+-rw-rw-rw-   0        0        0       38 2024-05-20 08:34:39.000000 jzai-59.83.54/jzai/__init__.py
+-rw-rw-rw-   0        0        0     7750 2024-05-20 08:58:58.000000 jzai-59.83.54/jzai/bot.py
+-rw-rw-rw-   0        0        0      179 2024-05-20 09:00:13.000000 jzai-59.83.54/jzai/cli.py
+-rw-rw-rw-   0        0        0      875 2024-05-20 08:31:32.000000 jzai-59.83.54/jzai/db.py
+-rw-rw-rw-   0        0        0      248 2024-05-20 08:31:36.000000 jzai-59.83.54/jzai/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:04:07.778908 jzai-59.83.54/jzai.egg-info/
+-rw-rw-rw-   0        0        0      275 2024-05-21 04:04:07.000000 jzai-59.83.54/jzai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-21 04:04:07.000000 jzai-59.83.54/jzai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 04:04:07.000000 jzai-59.83.54/jzai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-21 04:04:07.000000 jzai-59.83.54/jzai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2024-05-21 04:04:07.000000 jzai-59.83.54/jzai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-21 04:04:07.000000 jzai-59.83.54/jzai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 04:04:07.784263 jzai-59.83.54/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-21 04:04:01.000000 jzai-59.83.54/setup.py
```

### Comparing `jzai-59.83.53/jzai/bot.py` & `jzai-59.83.54/jzai/bot.py`

 * *Files identical despite different names*

### Comparing `jzai-59.83.53/jzai/db.py` & `jzai-59.83.54/jzai/db.py`

 * *Files identical despite different names*

