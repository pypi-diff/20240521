# Comparing `tmp/jzai-59.83.57.tar.gz` & `tmp/jzai-59.83.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzai-59.83.57.tar", last modified: Tue May 21 04:19:54 2024, max compression
+gzip compressed data, was "jzai-59.83.58.tar", last modified: Tue May 21 04:23:09 2024, max compression
```

## Comparing `jzai-59.83.57.tar` & `jzai-59.83.58.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 04:19:54.944679 jzai-59.83.57/
--rw-rw-rw-   0        0        0      226 2024-05-21 04:19:54.942664 jzai-59.83.57/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.57/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 04:19:54.909671 jzai-59.83.57/jzai/
--rw-rw-rw-   0        0        0       38 2024-05-20 08:34:39.000000 jzai-59.83.57/jzai/__init__.py
--rw-rw-rw-   0        0        0     8546 2024-05-21 04:17:35.000000 jzai-59.83.57/jzai/bot.py
--rw-rw-rw-   0        0        0      179 2024-05-20 09:00:13.000000 jzai-59.83.57/jzai/cli.py
--rw-rw-rw-   0        0        0      875 2024-05-20 08:31:32.000000 jzai-59.83.57/jzai/db.py
--rw-rw-rw-   0        0        0      248 2024-05-20 08:31:36.000000 jzai-59.83.57/jzai/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 04:19:54.940168 jzai-59.83.57/jzai.egg-info/
--rw-rw-rw-   0        0        0      226 2024-05-21 04:19:54.000000 jzai-59.83.57/jzai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-21 04:19:54.000000 jzai-59.83.57/jzai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 04:19:54.000000 jzai-59.83.57/jzai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-21 04:19:54.000000 jzai-59.83.57/jzai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2024-05-21 04:19:54.000000 jzai-59.83.57/jzai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-21 04:19:54.000000 jzai-59.83.57/jzai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 04:19:54.944679 jzai-59.83.57/setup.cfg
--rw-rw-rw-   0        0        0      411 2024-05-21 04:19:47.000000 jzai-59.83.57/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:23:09.808035 jzai-59.83.58/
+-rw-rw-rw-   0        0        0      226 2024-05-21 04:23:09.806642 jzai-59.83.58/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.58/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 04:23:09.783198 jzai-59.83.58/jzai/
+-rw-rw-rw-   0        0        0       38 2024-05-20 08:34:39.000000 jzai-59.83.58/jzai/__init__.py
+-rw-rw-rw-   0        0        0     8544 2024-05-21 04:22:57.000000 jzai-59.83.58/jzai/bot.py
+-rw-rw-rw-   0        0        0      179 2024-05-20 09:00:13.000000 jzai-59.83.58/jzai/cli.py
+-rw-rw-rw-   0        0        0      875 2024-05-20 08:31:32.000000 jzai-59.83.58/jzai/db.py
+-rw-rw-rw-   0        0        0      248 2024-05-20 08:31:36.000000 jzai-59.83.58/jzai/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:23:09.805509 jzai-59.83.58/jzai.egg-info/
+-rw-rw-rw-   0        0        0      226 2024-05-21 04:23:09.000000 jzai-59.83.58/jzai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-21 04:23:09.000000 jzai-59.83.58/jzai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 04:23:09.000000 jzai-59.83.58/jzai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-21 04:23:09.000000 jzai-59.83.58/jzai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2024-05-21 04:23:09.000000 jzai-59.83.58/jzai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-21 04:23:09.000000 jzai-59.83.58/jzai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 04:23:09.809102 jzai-59.83.58/setup.cfg
+-rw-rw-rw-   0        0        0      411 2024-05-21 04:23:03.000000 jzai-59.83.58/setup.py
```

### Comparing `jzai-59.83.57/jzai/bot.py` & `jzai-59.83.58/jzai/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class Bot:
     def __init__(self, name):
         self.name = name
         self.engine = pyttsx3.init()
         self.users = {}
         self.current_user = None
-        self.conversations = self.load_conversations("./conversations.json")
+        self.conversations = self.load_conversations("conversations.json")
 
     def preprocess_text(self, text):
         # Correct spelling mistakes using TextBlob
         corrected_text = str(TextBlob(text).correct())
 
         # Tokenization
         tokens = word_tokenize(corrected_text)
```

### Comparing `jzai-59.83.57/jzai/db.py` & `jzai-59.83.58/jzai/db.py`

 * *Files identical despite different names*

