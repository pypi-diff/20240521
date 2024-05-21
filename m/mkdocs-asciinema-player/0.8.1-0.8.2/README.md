# Comparing `tmp/mkdocs-asciinema-player-0.8.1.tar.gz` & `tmp/mkdocs_asciinema_player-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-asciinema-player-0.8.1.tar", last modified: Thu Mar 28 17:54:50 2024, max compression
+gzip compressed data, was "mkdocs_asciinema_player-0.8.2.tar", last modified: Tue May 21 15:52:34 2024, max compression
```

## Comparing `mkdocs-asciinema-player-0.8.1.tar` & `mkdocs_asciinema_player-0.8.2.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:54:50.439427 mkdocs-asciinema-player-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-28 17:54:37.000000 mkdocs-asciinema-player-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-28 17:54:37.000000 mkdocs-asciinema-player-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-03-28 17:54:50.439427 mkdocs-asciinema-player-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-28 17:54:37.000000 mkdocs-asciinema-player-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-28 17:54:37.000000 mkdocs-asciinema-player-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:54:50.439427 mkdocs-asciinema-player-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:54:50.435426 mkdocs-asciinema-player-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:54:50.435426 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:54:50.435426 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    53739 2024-03-28 17:54:37.000000 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/assets/asciinema-player.css
--rw-r--r--   0 runner    (1001) docker     (127)   158715 2024-03-28 17:54:37.000000 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/assets/asciinema-player.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-03-28 17:54:37.000000 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/assets/terminal-player.css
--rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-03-28 17:54:37.000000 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:54:50.435426 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-28 17:54:37.000000 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/templates/asciinema-player.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:54:50.435426 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/templates/themes/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-28 17:54:37.000000 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/templates/themes/blue.html
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-28 17:54:37.000000 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/templates/themes/night.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:54:50.435426 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-03-28 17:54:50.000000 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-28 17:54:50.000000 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:54:50.000000 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-28 17:54:50.000000 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-28 17:54:50.000000 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-28 17:54:50.000000 mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:52:34.516428 mkdocs_asciinema_player-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-21 15:52:25.000000 mkdocs_asciinema_player-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-21 15:52:25.000000 mkdocs_asciinema_player-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-21 15:52:34.516428 mkdocs_asciinema_player-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-21 15:52:25.000000 mkdocs_asciinema_player-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-21 15:52:25.000000 mkdocs_asciinema_player-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:52:34.516428 mkdocs_asciinema_player-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:52:34.508428 mkdocs_asciinema_player-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:52:34.508428 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:52:34.512428 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    53739 2024-05-21 15:52:25.000000 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/assets/asciinema-player.css
+-rw-r--r--   0 runner    (1001) docker     (127)   158715 2024-05-21 15:52:25.000000 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/assets/asciinema-player.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:52:34.512428 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-05-21 15:52:25.000000 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/assets/fonts/ms-sans-serif-bold.woff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:52:34.512428 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-21 15:52:25.000000 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/assets/icons/close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-21 15:52:25.000000 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/assets/icons/maximize.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-21 15:52:25.000000 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/assets/icons/minimize.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-21 15:52:25.000000 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/assets/terminal-player.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-21 15:52:25.000000 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:52:34.512428 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-21 15:52:25.000000 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/templates/asciinema-player.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:52:34.512428 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/templates/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-21 15:52:25.000000 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/templates/themes/blue.html
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-21 15:52:25.000000 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/templates/themes/night.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:52:34.512428 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-21 15:52:34.000000 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-21 15:52:34.000000 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:52:34.000000 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-21 15:52:34.000000 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-21 15:52:34.000000 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 15:52:34.000000 mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player.egg-info/top_level.txt
```

### Comparing `mkdocs-asciinema-player-0.8.1/LICENSE` & `mkdocs_asciinema_player-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-asciinema-player-0.8.1/PKG-INFO` & `mkdocs_asciinema_player-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-asciinema-player
-Version: 0.8.1
+Version: 0.8.2
 Summary: A Mkdocs Plugin to include asciinema player in your documentation.
 Author-email: Philippe-André De Carvalho <philippe.andre.decarvalho@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Philippe-André De Carvalho
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mkdocs-asciinema-player-0.8.1/README.md` & `mkdocs_asciinema_player-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-asciinema-player-0.8.1/pyproject.toml` & `mkdocs_asciinema_player-0.8.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mkdocs-asciinema-player"
-version = "0.8.1"
+version = "0.8.2"
 description = "A Mkdocs Plugin to include asciinema player in your documentation."
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["mkdocs", "documentation", "asciinema"]
 authors = [
   {name = "Philippe-André De Carvalho", email = "philippe.andre.decarvalho@gmail.com"}
 ]
```

### Comparing `mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/assets/asciinema-player.css` & `mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/assets/asciinema-player.css`

 * *Files identical despite different names*

### Comparing `mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/assets/asciinema-player.min.js` & `mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/assets/asciinema-player.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/assets/terminal-player.css` & `mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/assets/terminal-player.css`

 * *Files identical despite different names*

### Comparing `mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/plugin.py` & `mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/templates/asciinema-player.html` & `mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/templates/asciinema-player.html`

 * *Files identical despite different names*

### Comparing `mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/templates/themes/blue.html` & `mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/templates/themes/blue.html`

 * *Files identical despite different names*

### Comparing `mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player/templates/themes/night.html` & `mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player/templates/themes/night.html`

 * *Files identical despite different names*

### Comparing `mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player.egg-info/PKG-INFO` & `mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-asciinema-player
-Version: 0.8.1
+Version: 0.8.2
 Summary: A Mkdocs Plugin to include asciinema player in your documentation.
 Author-email: Philippe-André De Carvalho <philippe.andre.decarvalho@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Philippe-André De Carvalho
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mkdocs-asciinema-player-0.8.1/src/mkdocs_asciinema_player.egg-info/SOURCES.txt` & `mkdocs_asciinema_player-0.8.2/src/mkdocs_asciinema_player.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,10 +8,14 @@
 src/mkdocs_asciinema_player.egg-info/dependency_links.txt
 src/mkdocs_asciinema_player.egg-info/entry_points.txt
 src/mkdocs_asciinema_player.egg-info/requires.txt
 src/mkdocs_asciinema_player.egg-info/top_level.txt
 src/mkdocs_asciinema_player/assets/asciinema-player.css
 src/mkdocs_asciinema_player/assets/asciinema-player.min.js
 src/mkdocs_asciinema_player/assets/terminal-player.css
+src/mkdocs_asciinema_player/assets/fonts/ms-sans-serif-bold.woff
+src/mkdocs_asciinema_player/assets/icons/close.svg
+src/mkdocs_asciinema_player/assets/icons/maximize.svg
+src/mkdocs_asciinema_player/assets/icons/minimize.svg
 src/mkdocs_asciinema_player/templates/asciinema-player.html
 src/mkdocs_asciinema_player/templates/themes/blue.html
 src/mkdocs_asciinema_player/templates/themes/night.html
```

