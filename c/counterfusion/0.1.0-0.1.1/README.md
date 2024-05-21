# Comparing `tmp/counterfusion-0.1.0.tar.gz` & `tmp/counterfusion-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\gitproj\Counterfusion\dist\.tmp-z6vl3wkk\counterfusion-0.1.0.tar", last modified: Wed May 15 13:40:42 2024, max compression
+gzip compressed data, was "counterfusion-0.1.1.tar", last modified: Tue May 21 10:15:44 2024, max compression
```

## Comparing `counterfusion-0.1.0.tar` & `counterfusion-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 13:40:42.111630 counterfusion-0.1.0/
--rw-rw-rw-   0        0        0      510 2024-05-01 18:07:03.000000 counterfusion-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      227 2024-05-15 13:40:42.107620 counterfusion-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3611 2024-05-01 19:20:44.000000 counterfusion-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 13:40:42.051663 counterfusion-0.1.0/counterfusion/
-drwxrwxrwx   0        0        0        0 2024-05-15 13:40:42.104627 counterfusion-0.1.0/counterfusion/counterfusion.egg-info/
--rw-rw-rw-   0        0        0      227 2024-05-15 13:40:41.000000 counterfusion-0.1.0/counterfusion/counterfusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2024-05-15 13:40:42.000000 counterfusion-0.1.0/counterfusion/counterfusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 13:40:41.000000 counterfusion-0.1.0/counterfusion/counterfusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-15 13:40:42.000000 counterfusion-0.1.0/counterfusion/counterfusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 13:40:42.000000 counterfusion-0.1.0/counterfusion/counterfusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      400 2024-05-15 13:37:11.000000 counterfusion-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 13:40:42.112629 counterfusion-0.1.0/setup.cfg
+drwxrwxr-x   0 lx        (1000) lx        (1000)        0 2024-05-21 10:15:44.062579 counterfusion-0.1.1/
+-rw-rw-r--   0 lx        (1000) lx        (1000)      510 2024-05-21 09:11:18.000000 counterfusion-0.1.1/LICENSE
+-rw-rw-r--   0 lx        (1000) lx        (1000)     3961 2024-05-21 10:15:44.058579 counterfusion-0.1.1/PKG-INFO
+-rw-rw-r--   0 lx        (1000) lx        (1000)     3611 2024-05-21 09:11:18.000000 counterfusion-0.1.1/README.md
+drwxrwxr-x   0 lx        (1000) lx        (1000)        0 2024-05-21 10:15:44.058579 counterfusion-0.1.1/counterfusion/
+-rw-rw-r--   0 lx        (1000) lx        (1000)      759 2024-05-21 09:11:18.000000 counterfusion-0.1.1/counterfusion/__init__.py
+-rw-rw-r--   0 lx        (1000) lx        (1000)     3841 2024-05-21 09:11:18.000000 counterfusion-0.1.1/counterfusion/algorithm.py
+-rw-rw-r--   0 lx        (1000) lx        (1000)    23233 2024-05-21 09:11:18.000000 counterfusion-0.1.1/counterfusion/interface.py
+-rw-rw-r--   0 lx        (1000) lx        (1000)     4952 2024-05-21 09:11:18.000000 counterfusion-0.1.1/counterfusion/utils.py
+drwxrwxr-x   0 lx        (1000) lx        (1000)        0 2024-05-21 10:15:44.058579 counterfusion-0.1.1/counterfusion.egg-info/
+-rw-rw-r--   0 lx        (1000) lx        (1000)     3961 2024-05-21 10:15:44.000000 counterfusion-0.1.1/counterfusion.egg-info/PKG-INFO
+-rw-rw-r--   0 lx        (1000) lx        (1000)      313 2024-05-21 10:15:44.000000 counterfusion-0.1.1/counterfusion.egg-info/SOURCES.txt
+-rw-rw-r--   0 lx        (1000) lx        (1000)        1 2024-05-21 10:15:44.000000 counterfusion-0.1.1/counterfusion.egg-info/dependency_links.txt
+-rw-rw-r--   0 lx        (1000) lx        (1000)       32 2024-05-21 10:15:44.000000 counterfusion-0.1.1/counterfusion.egg-info/requires.txt
+-rw-rw-r--   0 lx        (1000) lx        (1000)       14 2024-05-21 10:15:44.000000 counterfusion-0.1.1/counterfusion.egg-info/top_level.txt
+-rw-rw-r--   0 lx        (1000) lx        (1000)       38 2024-05-21 10:15:44.062579 counterfusion-0.1.1/setup.cfg
+-rw-rw-r--   0 lx        (1000) lx        (1000)      664 2024-05-21 10:15:12.000000 counterfusion-0.1.1/setup.py
```

### Comparing `counterfusion-0.1.0/README.md` & `counterfusion-0.1.1/README.md`

 * *Files identical despite different names*

