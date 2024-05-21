# Comparing `tmp/jzai-59.83.58.tar.gz` & `tmp/jzai-59.83.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzai-59.83.58.tar", last modified: Tue May 21 04:23:09 2024, max compression
+gzip compressed data, was "jzai-59.83.59.tar", last modified: Tue May 21 04:32:07 2024, max compression
```

## Comparing `jzai-59.83.58.tar` & `jzai-59.83.59.tar`

### file list

```diff
@@ -1,18 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 04:23:09.808035 jzai-59.83.58/
--rw-rw-rw-   0        0        0      226 2024-05-21 04:23:09.806642 jzai-59.83.58/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.58/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 04:23:09.783198 jzai-59.83.58/jzai/
--rw-rw-rw-   0        0        0       38 2024-05-20 08:34:39.000000 jzai-59.83.58/jzai/__init__.py
--rw-rw-rw-   0        0        0     8544 2024-05-21 04:22:57.000000 jzai-59.83.58/jzai/bot.py
--rw-rw-rw-   0        0        0      179 2024-05-20 09:00:13.000000 jzai-59.83.58/jzai/cli.py
--rw-rw-rw-   0        0        0      875 2024-05-20 08:31:32.000000 jzai-59.83.58/jzai/db.py
--rw-rw-rw-   0        0        0      248 2024-05-20 08:31:36.000000 jzai-59.83.58/jzai/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 04:23:09.805509 jzai-59.83.58/jzai.egg-info/
--rw-rw-rw-   0        0        0      226 2024-05-21 04:23:09.000000 jzai-59.83.58/jzai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-21 04:23:09.000000 jzai-59.83.58/jzai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 04:23:09.000000 jzai-59.83.58/jzai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-21 04:23:09.000000 jzai-59.83.58/jzai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2024-05-21 04:23:09.000000 jzai-59.83.58/jzai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-21 04:23:09.000000 jzai-59.83.58/jzai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 04:23:09.809102 jzai-59.83.58/setup.cfg
--rw-rw-rw-   0        0        0      411 2024-05-21 04:23:03.000000 jzai-59.83.58/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:32:07.026105 jzai-59.83.59/
+-rw-rw-rw-   0        0        0      226 2024-05-21 04:32:07.023960 jzai-59.83.59/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.59/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 04:32:07.021950 jzai-59.83.59/jzai.egg-info/
+-rw-rw-rw-   0        0        0      226 2024-05-21 04:32:06.000000 jzai-59.83.59/jzai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-05-21 04:32:06.000000 jzai-59.83.59/jzai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 04:32:06.000000 jzai-59.83.59/jzai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-21 04:32:06.000000 jzai-59.83.59/jzai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2024-05-21 04:32:06.000000 jzai-59.83.59/jzai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 04:32:06.000000 jzai-59.83.59/jzai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 04:32:07.026105 jzai-59.83.59/setup.cfg
+-rw-rw-rw-   0        0        0      411 2024-05-21 04:31:59.000000 jzai-59.83.59/setup.py
```

