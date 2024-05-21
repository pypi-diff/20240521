# Comparing `tmp/sharklog-0.0.1.tar.gz` & `tmp/sharklog-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharklog-0.0.1.tar", last modified: Tue May 21 04:03:48 2024, max compression
+gzip compressed data, was "sharklog-0.0.2.tar", last modified: Tue May 21 08:42:24 2024, max compression
```

## Comparing `sharklog-0.0.1.tar` & `sharklog-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 04:03:48.244716 sharklog-0.0.1/
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     1069 2024-05-21 02:49:41.000000 sharklog-0.0.1/LICENSE
--rw-r--r--   0 jinqi     (1000) jinqi     (1000)     1686 2024-05-21 04:03:48.244716 sharklog-0.0.1/PKG-INFO
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       48 2024-05-21 02:50:05.000000 sharklog-0.0.1/README.md
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      501 2024-05-21 04:03:32.000000 sharklog-0.0.1/pyproject.toml
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       38 2024-05-21 04:03:48.244716 sharklog-0.0.1/setup.cfg
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       38 2024-05-21 03:16:21.000000 sharklog-0.0.1/setup.py
-drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 04:03:48.244716 sharklog-0.0.1/src/
-drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 04:03:48.244716 sharklog-0.0.1/src/sharklog/
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 02:51:49.000000 sharklog-0.0.1/src/sharklog/__init__.py
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      228 2024-05-21 03:04:05.000000 sharklog-0.0.1/src/sharklog/logging.py
-drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 04:03:48.244716 sharklog-0.0.1/src/sharklog.egg-info/
--rw-r--r--   0 jinqi     (1000) jinqi     (1000)     1686 2024-05-21 04:03:48.000000 sharklog-0.0.1/src/sharklog.egg-info/PKG-INFO
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      234 2024-05-21 04:03:48.000000 sharklog-0.0.1/src/sharklog.egg-info/SOURCES.txt
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        1 2024-05-21 04:03:48.000000 sharklog-0.0.1/src/sharklog.egg-info/dependency_links.txt
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        9 2024-05-21 04:03:48.000000 sharklog-0.0.1/src/sharklog.egg-info/top_level.txt
+drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 08:42:24.508790 sharklog-0.0.2/
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     1069 2024-05-21 04:05:28.000000 sharklog-0.0.2/LICENSE
+-rw-r--r--   0 jinqi     (1000) jinqi     (1000)     3248 2024-05-21 08:42:24.508790 sharklog-0.0.2/PKG-INFO
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     1610 2024-05-21 08:40:36.000000 sharklog-0.0.2/README.md
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      501 2024-05-21 06:38:43.000000 sharklog-0.0.2/pyproject.toml
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       38 2024-05-21 08:42:24.508790 sharklog-0.0.2/setup.cfg
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       38 2024-05-21 04:05:28.000000 sharklog-0.0.2/setup.py
+drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 08:42:24.508790 sharklog-0.0.2/src/
+drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 08:42:24.508790 sharklog-0.0.2/src/sharklog/
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 04:05:28.000000 sharklog-0.0.2/src/sharklog/__init__.py
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     1961 2024-05-21 08:33:18.000000 sharklog-0.0.2/src/sharklog/logging.py
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      132 2024-05-21 07:59:56.000000 sharklog-0.0.2/src/sharklog/settings.py
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     1780 2024-05-21 07:45:16.000000 sharklog-0.0.2/src/sharklog/utils.py
+drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 08:42:24.508790 sharklog-0.0.2/src/sharklog.egg-info/
+-rw-r--r--   0 jinqi     (1000) jinqi     (1000)     3248 2024-05-21 08:42:24.000000 sharklog-0.0.2/src/sharklog.egg-info/PKG-INFO
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      281 2024-05-21 08:42:24.000000 sharklog-0.0.2/src/sharklog.egg-info/SOURCES.txt
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        1 2024-05-21 08:42:24.000000 sharklog-0.0.2/src/sharklog.egg-info/dependency_links.txt
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        9 2024-05-21 08:42:24.000000 sharklog-0.0.2/src/sharklog.egg-info/top_level.txt
```

### Comparing `sharklog-0.0.1/LICENSE` & `sharklog-0.0.2/LICENSE`

 * *Files identical despite different names*

