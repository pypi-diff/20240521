# Comparing `tmp/pygame_canvas-1.4.0.tar.gz` & `tmp/pygame_canvas-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_canvas-1.4.0.tar", last modified: Tue May 21 14:08:54 2024, max compression
+gzip compressed data, was "pygame_canvas-1.4.1.tar", last modified: Tue May 21 14:41:45 2024, max compression
```

## Comparing `pygame_canvas-1.4.0.tar` & `pygame_canvas-1.4.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 14:08:54.879736 pygame_canvas-1.4.0/
--rw-rw-rw-   0        0        0      239 2024-05-21 14:08:54.877702 pygame_canvas-1.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-21 14:08:54.876173 pygame_canvas-1.4.0/pygame_canvas.egg-info/
--rw-rw-rw-   0        0        0      239 2024-05-21 14:08:54.000000 pygame_canvas-1.4.0/pygame_canvas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-05-21 14:08:54.000000 pygame_canvas-1.4.0/pygame_canvas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:08:54.000000 pygame_canvas-1.4.0/pygame_canvas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 14:08:54.000000 pygame_canvas-1.4.0/pygame_canvas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:08:54.000000 pygame_canvas-1.4.0/pygame_canvas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2024-05-21 13:50:24.000000 pygame_canvas-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 14:08:54.880753 pygame_canvas-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      404 2024-05-21 14:07:44.000000 pygame_canvas-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:41:45.926419 pygame_canvas-1.4.1/
+-rw-rw-rw-   0        0        0     1881 2024-05-21 14:41:45.925393 pygame_canvas-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1638 2024-05-21 14:32:25.000000 pygame_canvas-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 14:41:45.924369 pygame_canvas-1.4.1/pygame_canvas.egg-info/
+-rw-rw-rw-   0        0        0     1881 2024-05-21 14:41:45.000000 pygame_canvas-1.4.1/pygame_canvas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-05-21 14:41:45.000000 pygame_canvas-1.4.1/pygame_canvas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:41:45.000000 pygame_canvas-1.4.1/pygame_canvas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 14:41:45.000000 pygame_canvas-1.4.1/pygame_canvas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:41:45.000000 pygame_canvas-1.4.1/pygame_canvas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2024-05-21 13:50:24.000000 pygame_canvas-1.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:41:45.926419 pygame_canvas-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      520 2024-05-21 14:40:37.000000 pygame_canvas-1.4.1/setup.py
```

