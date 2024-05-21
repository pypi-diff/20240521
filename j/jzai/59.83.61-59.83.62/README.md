# Comparing `tmp/jzai-59.83.61.tar.gz` & `tmp/jzai-59.83.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzai-59.83.61.tar", last modified: Tue May 21 04:55:56 2024, max compression
+gzip compressed data, was "jzai-59.83.62.tar", last modified: Tue May 21 04:56:40 2024, max compression
```

## Comparing `jzai-59.83.61.tar` & `jzai-59.83.62.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 04:55:56.547855 jzai-59.83.61/
--rw-rw-rw-   0        0        0      202 2024-05-21 04:55:56.546845 jzai-59.83.61/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.61/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 04:55:56.516099 jzai-59.83.61/jzai/
--rw-rw-rw-   0        0        0       38 2024-05-20 08:34:39.000000 jzai-59.83.61/jzai/__init__.py
--rw-rw-rw-   0        0        0     3048 2024-05-21 04:55:43.000000 jzai-59.83.61/jzai/bot.py
--rw-rw-rw-   0        0        0      179 2024-05-21 04:33:28.000000 jzai-59.83.61/jzai/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-21 04:55:56.544361 jzai-59.83.61/jzai.egg-info/
--rw-rw-rw-   0        0        0      202 2024-05-21 04:55:56.000000 jzai-59.83.61/jzai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-05-21 04:55:56.000000 jzai-59.83.61/jzai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 04:55:56.000000 jzai-59.83.61/jzai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-21 04:55:56.000000 jzai-59.83.61/jzai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       52 2024-05-21 04:55:56.000000 jzai-59.83.61/jzai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-21 04:55:56.000000 jzai-59.83.61/jzai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 04:55:56.548885 jzai-59.83.61/setup.cfg
--rw-rw-rw-   0        0        0      449 2024-05-21 04:55:26.000000 jzai-59.83.61/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:56:40.220446 jzai-59.83.62/
+-rw-rw-rw-   0        0        0      202 2024-05-21 04:56:40.219437 jzai-59.83.62/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.62/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 04:56:40.198164 jzai-59.83.62/jzai/
+-rw-rw-rw-   0        0        0       38 2024-05-20 08:34:39.000000 jzai-59.83.62/jzai/__init__.py
+-rw-rw-rw-   0        0        0     3030 2024-05-21 04:56:29.000000 jzai-59.83.62/jzai/bot.py
+-rw-rw-rw-   0        0        0      179 2024-05-21 04:33:28.000000 jzai-59.83.62/jzai/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:56:40.218020 jzai-59.83.62/jzai.egg-info/
+-rw-rw-rw-   0        0        0      202 2024-05-21 04:56:40.000000 jzai-59.83.62/jzai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-05-21 04:56:40.000000 jzai-59.83.62/jzai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 04:56:40.000000 jzai-59.83.62/jzai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-21 04:56:40.000000 jzai-59.83.62/jzai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       52 2024-05-21 04:56:40.000000 jzai-59.83.62/jzai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-21 04:56:40.000000 jzai-59.83.62/jzai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 04:56:40.220446 jzai-59.83.62/setup.cfg
+-rw-rw-rw-   0        0        0      449 2024-05-21 04:56:34.000000 jzai-59.83.62/setup.py
```

### Comparing `jzai-59.83.61/jzai/bot.py` & `jzai-59.83.62/jzai/bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,14 @@
         except Exception as e:
             print(f"Error loading {file_name}: {e}")
             return None
 
 
 
 bot = Bot(name="JZ")
-bot.load_users()
 
 try:
     while True:
         user_input = input("You: ")
         if user_input.lower() == 'exit':
             break
         else:
```

