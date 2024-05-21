# Comparing `tmp/lyynircmd-1.2.tar.gz` & `tmp/lyynircmd-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyynircmd-1.2.tar", last modified: Wed May  8 00:57:27 2024, max compression
+gzip compressed data, was "lyynircmd-1.3.tar", last modified: Tue May 21 21:47:23 2024, max compression
```

## Comparing `lyynircmd-1.2.tar` & `lyynircmd-1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 00:57:27.619723 lyynircmd-1.2/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyynircmd-1.2/LICENSE
--rw-rw-rw-   0        0        0      146 2024-05-08 00:57:27.619723 lyynircmd-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyynircmd-1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 00:57:27.618137 lyynircmd-1.2/lyynircmd.egg-info/
--rw-rw-rw-   0        0        0      146 2024-05-08 00:57:27.000000 lyynircmd-1.2/lyynircmd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2024-05-08 00:57:27.000000 lyynircmd-1.2/lyynircmd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 00:57:27.000000 lyynircmd-1.2/lyynircmd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-08 00:57:27.000000 lyynircmd-1.2/lyynircmd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      446 2024-05-08 00:57:01.000000 lyynircmd-1.2/lyynircmd.py
--rw-rw-rw-   0        0        0       42 2024-05-08 00:57:27.619723 lyynircmd-1.2/setup.cfg
--rw-rw-rw-   0        0        0      249 2024-05-08 00:57:26.000000 lyynircmd-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:47:23.642782 lyynircmd-1.3/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyynircmd-1.3/LICENSE
+-rw-rw-rw-   0        0        0      146 2024-05-21 21:47:23.641761 lyynircmd-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyynircmd-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 21:47:23.640322 lyynircmd-1.3/lyynircmd.egg-info/
+-rw-rw-rw-   0        0        0      146 2024-05-21 21:47:23.000000 lyynircmd-1.3/lyynircmd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2024-05-21 21:47:23.000000 lyynircmd-1.3/lyynircmd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 21:47:23.000000 lyynircmd-1.3/lyynircmd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-21 21:47:23.000000 lyynircmd-1.3/lyynircmd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1505 2024-05-21 21:46:28.000000 lyynircmd-1.3/lyynircmd.py
+-rw-rw-rw-   0        0        0       42 2024-05-21 21:47:23.642782 lyynircmd-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      249 2024-05-21 21:47:22.000000 lyynircmd-1.3/setup.py
```

### Comparing `lyynircmd-1.2/LICENSE` & `lyynircmd-1.3/LICENSE`

 * *Files identical despite different names*

