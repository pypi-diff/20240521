# Comparing `tmp/neofetch-win-1.3.3.tar.gz` & `tmp/neofetch_win-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neofetch-win-1.3.3.tar", last modified: Mon Jul  4 11:59:28 2022, max compression
+gzip compressed data, was "neofetch_win-1.4.0.tar", last modified: Mon May 20 23:41:28 2024, max compression
```

## Comparing `neofetch-win-1.3.3.tar` & `neofetch_win-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-07-04 11:59:28.427387 neofetch-win-1.3.3/
--rw-rw-rw-   0        0        0    35823 2019-05-07 15:25:03.000000 neofetch-win-1.3.3/LICENSE
--rw-rw-rw-   0        0        0       62 2019-05-11 09:28:42.000000 neofetch-win-1.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0      246 2022-07-04 11:59:28.426389 neofetch-win-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     1549 2020-10-07 19:16:19.000000 neofetch-win-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2022-07-04 11:59:28.420400 neofetch-win-1.3.3/neofetch_win/
--rw-rw-rw-   0        0        0       71 2022-07-04 11:58:54.000000 neofetch-win-1.3.3/neofetch_win/__init__.py
--rw-rw-rw-   0        0        0      229 2019-05-07 15:25:03.000000 neofetch-win-1.3.3/neofetch_win/argpar.py
--rw-rw-rw-   0        0        0     1579 2022-02-10 21:17:51.000000 neofetch-win-1.3.3/neofetch_win/art.py
--rw-rw-rw-   0        0        0     1893 2022-02-10 21:22:16.000000 neofetch-win-1.3.3/neofetch_win/main.py
--rw-rw-rw-   0        0        0     8200 2022-07-04 11:58:54.000000 neofetch-win-1.3.3/neofetch_win/neofetch.py
-drwxrwxrwx   0        0        0        0 2022-07-04 11:59:28.426389 neofetch-win-1.3.3/neofetch_win.egg-info/
--rw-rw-rw-   0        0        0      246 2022-07-04 11:59:27.000000 neofetch-win-1.3.3/neofetch_win.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2022-07-04 11:59:28.000000 neofetch-win-1.3.3/neofetch_win.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-04 11:59:27.000000 neofetch-win-1.3.3/neofetch_win.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2022-07-04 11:59:27.000000 neofetch-win-1.3.3/neofetch_win.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2022-07-04 11:59:28.000000 neofetch-win-1.3.3/neofetch_win.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-07-04 11:59:28.000000 neofetch-win-1.3.3/neofetch_win.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       23 2022-05-24 11:43:00.000000 neofetch-win-1.3.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-07-04 11:59:28.427387 neofetch-win-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      912 2019-05-10 20:39:11.000000 neofetch-win-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:41:28.836151 neofetch_win-1.4.0/
+-rw-rw-rw-   0        0        0     1090 2024-05-20 21:49:59.000000 neofetch_win-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1836 2024-05-20 23:41:28.834582 neofetch_win-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1494 2024-05-20 23:26:31.000000 neofetch_win-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 23:41:28.804461 neofetch_win-1.4.0/neofetch_win/
+-rw-rw-rw-   0        0        0       79 2024-05-20 23:31:00.000000 neofetch_win-1.4.0/neofetch_win/__init__.py
+-rw-rw-rw-   0        0        0     1933 2024-05-20 23:37:19.000000 neofetch_win-1.4.0/neofetch_win/__main__.py
+-rw-rw-rw-   0        0        0     2506 2024-05-20 23:10:30.000000 neofetch_win-1.4.0/neofetch_win/art.py
+-rw-rw-rw-   0        0        0     9326 2024-05-20 23:39:10.000000 neofetch_win-1.4.0/neofetch_win/neofetch.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:41:28.834077 neofetch_win-1.4.0/neofetch_win.egg-info/
+-rw-rw-rw-   0        0        0     1836 2024-05-20 23:41:28.000000 neofetch_win-1.4.0/neofetch_win.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2024-05-20 23:41:28.000000 neofetch_win-1.4.0/neofetch_win.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 23:41:28.000000 neofetch_win-1.4.0/neofetch_win.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-20 23:41:28.000000 neofetch_win-1.4.0/neofetch_win.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 23:41:28.000000 neofetch_win-1.4.0/neofetch_win.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-20 23:41:28.000000 neofetch_win-1.4.0/neofetch_win.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1340 2024-05-20 23:40:09.000000 neofetch_win-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 23:41:28.836151 neofetch_win-1.4.0/setup.cfg
```

### Comparing `neofetch-win-1.3.3/README.md` & `neofetch_win-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-# neofetch-win
+# neofetch_win
 neofetch, but for Windows
 
-#### | ENGLISH | [简体中文](./zh-cn-README.md) |
-
 ![PreviewImage](https://i.alexflipnote.dev/vfgQo1y.png)
 
 This was made to have the command [neofetch](https://github.com/dylanaraps/neofetch) available on the Windows CMD.
 If you wish to contribute, feel free to do so.
 
 ## Requirement
-- Python 3.6 or up
+- Python 3.11 or up
 
 ## Install
 - Open CMD as admin
 - Type the following command: `pip install neofetch-win`
 - Now you can type `neofetch` in CMD to see results
 
 ### Available colours
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

