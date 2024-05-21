# Comparing `tmp/jzai-59.83.55.tar.gz` & `tmp/jzai-59.83.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzai-59.83.55.tar", last modified: Tue May 21 04:05:51 2024, max compression
+gzip compressed data, was "jzai-59.83.56.tar", last modified: Tue May 21 04:08:29 2024, max compression
```

## Comparing `jzai-59.83.55.tar` & `jzai-59.83.56.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 04:05:51.632968 jzai-59.83.55/
--rw-rw-rw-   0        0        0      275 2024-05-21 04:05:51.629953 jzai-59.83.55/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.55/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 04:05:51.594503 jzai-59.83.55/jzai/
--rw-rw-rw-   0        0        0       38 2024-05-20 08:34:39.000000 jzai-59.83.55/jzai/__init__.py
--rw-rw-rw-   0        0        0     7748 2024-05-21 04:05:31.000000 jzai-59.83.55/jzai/bot.py
--rw-rw-rw-   0        0        0      179 2024-05-20 09:00:13.000000 jzai-59.83.55/jzai/cli.py
--rw-rw-rw-   0        0        0      875 2024-05-20 08:31:32.000000 jzai-59.83.55/jzai/db.py
--rw-rw-rw-   0        0        0      248 2024-05-20 08:31:36.000000 jzai-59.83.55/jzai/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 04:05:51.627439 jzai-59.83.55/jzai.egg-info/
--rw-rw-rw-   0        0        0      275 2024-05-21 04:05:51.000000 jzai-59.83.55/jzai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-21 04:05:51.000000 jzai-59.83.55/jzai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 04:05:51.000000 jzai-59.83.55/jzai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-21 04:05:51.000000 jzai-59.83.55/jzai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2024-05-21 04:05:51.000000 jzai-59.83.55/jzai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-21 04:05:51.000000 jzai-59.83.55/jzai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 04:05:51.632968 jzai-59.83.55/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-21 04:05:47.000000 jzai-59.83.55/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:08:29.308411 jzai-59.83.56/
+-rw-rw-rw-   0        0        0      275 2024-05-21 04:08:29.307402 jzai-59.83.56/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.56/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 04:08:29.252652 jzai-59.83.56/jzai/
+-rw-rw-rw-   0        0        0       38 2024-05-20 08:34:39.000000 jzai-59.83.56/jzai/__init__.py
+-rw-rw-rw-   0        0        0     7750 2024-05-21 04:08:11.000000 jzai-59.83.56/jzai/bot.py
+-rw-rw-rw-   0        0        0      179 2024-05-20 09:00:13.000000 jzai-59.83.56/jzai/cli.py
+-rw-rw-rw-   0        0        0      875 2024-05-20 08:31:32.000000 jzai-59.83.56/jzai/db.py
+-rw-rw-rw-   0        0        0      248 2024-05-20 08:31:36.000000 jzai-59.83.56/jzai/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:08:29.304865 jzai-59.83.56/jzai.egg-info/
+-rw-rw-rw-   0        0        0      275 2024-05-21 04:08:29.000000 jzai-59.83.56/jzai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-21 04:08:29.000000 jzai-59.83.56/jzai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 04:08:29.000000 jzai-59.83.56/jzai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-21 04:08:29.000000 jzai-59.83.56/jzai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2024-05-21 04:08:29.000000 jzai-59.83.56/jzai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-21 04:08:29.000000 jzai-59.83.56/jzai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 04:08:29.309836 jzai-59.83.56/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-21 04:08:23.000000 jzai-59.83.56/setup.py
```

### Comparing `jzai-59.83.55/jzai/bot.py` & `jzai-59.83.56/jzai/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class Bot:
     def __init__(self, name):
         self.name = name
         self.engine = pyttsx3.init()
         self.users = {}
         self.current_user = None
-        self.conversations = self.load_conversations("conversations.json")
+        self.conversations = self.load_conversations("./conversations.json")
 
     def preprocess_text(self, text):
         # Correct spelling mistakes using TextBlob
         corrected_text = str(TextBlob(text).correct())
 
         # Tokenization
         tokens = word_tokenize(corrected_text)
```

### Comparing `jzai-59.83.55/jzai/db.py` & `jzai-59.83.56/jzai/db.py`

 * *Files identical despite different names*

