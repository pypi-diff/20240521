# Comparing `tmp/jzai-59.83.59.tar.gz` & `tmp/jzai-59.83.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzai-59.83.59.tar", last modified: Tue May 21 04:32:07 2024, max compression
+gzip compressed data, was "jzai-59.83.60.tar", last modified: Tue May 21 04:34:42 2024, max compression
```

## Comparing `jzai-59.83.59.tar` & `jzai-59.83.60.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 04:32:07.026105 jzai-59.83.59/
--rw-rw-rw-   0        0        0      226 2024-05-21 04:32:07.023960 jzai-59.83.59/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.59/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 04:32:07.021950 jzai-59.83.59/jzai.egg-info/
--rw-rw-rw-   0        0        0      226 2024-05-21 04:32:06.000000 jzai-59.83.59/jzai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-05-21 04:32:06.000000 jzai-59.83.59/jzai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 04:32:06.000000 jzai-59.83.59/jzai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-21 04:32:06.000000 jzai-59.83.59/jzai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2024-05-21 04:32:06.000000 jzai-59.83.59/jzai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 04:32:06.000000 jzai-59.83.59/jzai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 04:32:07.026105 jzai-59.83.59/setup.cfg
--rw-rw-rw-   0        0        0      411 2024-05-21 04:31:59.000000 jzai-59.83.59/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:34:42.248086 jzai-59.83.60/
+-rw-rw-rw-   0        0        0      226 2024-05-21 04:34:42.246994 jzai-59.83.60/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.60/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 04:34:42.219010 jzai-59.83.60/jzai/
+-rw-rw-rw-   0        0        0       38 2024-05-20 08:34:39.000000 jzai-59.83.60/jzai/__init__.py
+-rw-rw-rw-   0        0        0     8539 2024-05-21 04:27:33.000000 jzai-59.83.60/jzai/bot.py
+-rw-rw-rw-   0        0        0      179 2024-05-21 04:33:28.000000 jzai-59.83.60/jzai/cli.py
+-rw-rw-rw-   0        0        0      875 2024-05-20 08:31:32.000000 jzai-59.83.60/jzai/db.py
+-rw-rw-rw-   0        0        0      248 2024-05-20 08:31:36.000000 jzai-59.83.60/jzai/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:34:42.244702 jzai-59.83.60/jzai.egg-info/
+-rw-rw-rw-   0        0        0      226 2024-05-21 04:34:42.000000 jzai-59.83.60/jzai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-21 04:34:42.000000 jzai-59.83.60/jzai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 04:34:42.000000 jzai-59.83.60/jzai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-21 04:34:42.000000 jzai-59.83.60/jzai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2024-05-21 04:34:42.000000 jzai-59.83.60/jzai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-21 04:34:42.000000 jzai-59.83.60/jzai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 04:34:42.249097 jzai-59.83.60/setup.cfg
+-rw-rw-rw-   0        0        0      411 2024-05-21 04:34:37.000000 jzai-59.83.60/setup.py
```

