# Comparing `tmp/typing_test_sdd-1.0.1.tar.gz` & `tmp/typing_test_sdd-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typing_test_sdd-1.0.1.tar", last modified: Mon May 20 03:30:24 2024, max compression
+gzip compressed data, was "typing_test_sdd-1.0.2.tar", last modified: Tue May 21 12:22:43 2024, max compression
```

## Comparing `typing_test_sdd-1.0.1.tar` & `typing_test_sdd-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:30:24.245149 typing_test_sdd-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-20 03:30:18.000000 typing_test_sdd-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-20 03:30:24.245149 typing_test_sdd-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-20 03:30:18.000000 typing_test_sdd-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 03:30:24.245149 typing_test_sdd-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-20 03:30:18.000000 typing_test_sdd-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:30:24.241149 typing_test_sdd-1.0.1/typing_test_sdd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:30:24.245149 typing_test_sdd-1.0.1/typing_test_sdd/Assets/
--rw-r--r--   0 runner    (1001) docker     (127)    78455 2024-05-20 03:30:18.000000 typing_test_sdd-1.0.1/typing_test_sdd/Assets/main_image.png
--rw-r--r--   0 runner    (1001) docker     (127)    41028 2024-05-20 03:30:18.000000 typing_test_sdd-1.0.1/typing_test_sdd/Assets/polka.png
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 03:30:18.000000 typing_test_sdd-1.0.1/typing_test_sdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-05-20 03:30:18.000000 typing_test_sdd-1.0.1/typing_test_sdd/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    21222 2024-05-20 03:30:18.000000 typing_test_sdd-1.0.1/typing_test_sdd/words.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:30:24.245149 typing_test_sdd-1.0.1/typing_test_sdd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-20 03:30:24.000000 typing_test_sdd-1.0.1/typing_test_sdd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-20 03:30:24.000000 typing_test_sdd-1.0.1/typing_test_sdd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 03:30:24.000000 typing_test_sdd-1.0.1/typing_test_sdd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 03:30:24.000000 typing_test_sdd-1.0.1/typing_test_sdd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 03:30:24.000000 typing_test_sdd-1.0.1/typing_test_sdd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 03:30:24.000000 typing_test_sdd-1.0.1/typing_test_sdd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:22:43.597054 typing_test_sdd-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 12:22:34.000000 typing_test_sdd-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-21 12:22:43.597054 typing_test_sdd-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-21 12:22:34.000000 typing_test_sdd-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 12:22:43.597054 typing_test_sdd-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 12:22:34.000000 typing_test_sdd-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:22:43.593054 typing_test_sdd-1.0.2/typing_test_sdd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:22:43.597054 typing_test_sdd-1.0.2/typing_test_sdd/Assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    78455 2024-05-21 12:22:34.000000 typing_test_sdd-1.0.2/typing_test_sdd/Assets/main_image.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41028 2024-05-21 12:22:34.000000 typing_test_sdd-1.0.2/typing_test_sdd/Assets/polka.png
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 12:22:34.000000 typing_test_sdd-1.0.2/typing_test_sdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-05-21 12:22:34.000000 typing_test_sdd-1.0.2/typing_test_sdd/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21222 2024-05-21 12:22:34.000000 typing_test_sdd-1.0.2/typing_test_sdd/words.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:22:43.597054 typing_test_sdd-1.0.2/typing_test_sdd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-21 12:22:43.000000 typing_test_sdd-1.0.2/typing_test_sdd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-21 12:22:43.000000 typing_test_sdd-1.0.2/typing_test_sdd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 12:22:43.000000 typing_test_sdd-1.0.2/typing_test_sdd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-21 12:22:43.000000 typing_test_sdd-1.0.2/typing_test_sdd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 12:22:43.000000 typing_test_sdd-1.0.2/typing_test_sdd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 12:22:43.000000 typing_test_sdd-1.0.2/typing_test_sdd.egg-info/top_level.txt
```

### Comparing `typing_test_sdd-1.0.1/PKG-INFO` & `typing_test_sdd-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typing_test_sdd
-Version: 1.0.1
+Version: 1.0.2
 Summary: TKinter GUI Typing Test - Gaurav Surve 122SDD2
 Home-page: https://github.com/GauravS2507/Gaurav-Surve-SDD2-Project---Typing-Test
 Author: Gaurav Surve
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Education
```

### Comparing `typing_test_sdd-1.0.1/README.md` & `typing_test_sdd-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `typing_test_sdd-1.0.1/setup.py` & `typing_test_sdd-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="typing_test_sdd",
-    version="1.0.1",
+    version="1.0.2",
     author="Gaurav Surve",
     url="https://github.com/GauravS2507/Gaurav-Surve-SDD2-Project---Typing-Test",
     description="TKinter GUI Typing Test - Gaurav Surve 122SDD2",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     platforms="any",
     include_package_data=True,
     install_requires=[
         "customtkinter",
         "pillow",
     ],
     entry_points={
         "gui_scripts": [
-            "typing-ctk = typing_test:start_app"
+            "typing-ctk = typing_test_sdd:start_app"
         ]
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: End Users/Desktop",
         "Intended Audience :: Education",
         "Operating System :: OS Independent",
```

### Comparing `typing_test_sdd-1.0.1/typing_test_sdd/Assets/main_image.png` & `typing_test_sdd-1.0.2/typing_test_sdd/Assets/main_image.png`

 * *Files identical despite different names*

### Comparing `typing_test_sdd-1.0.1/typing_test_sdd/Assets/polka.png` & `typing_test_sdd-1.0.2/typing_test_sdd/Assets/polka.png`

 * *Files identical despite different names*

### Comparing `typing_test_sdd-1.0.1/typing_test_sdd/main.py` & `typing_test_sdd-1.0.2/typing_test_sdd/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
 def update_current_word():
     current_word_label.configure(text=" ".join(sampled_words[0:3]))
 
 
 # Receives word from JSON File "Words"
 def get_words():
     global sampled_words
-    with open(path.join("typing_test", "words.json")) as file:
+    with open(path.join("typing_test_sdd", "words.json")) as file:
         words = json.load(file)
         sampled_words = random.sample(words, 100)
 
 
 # Countdown Timer
 def update_timer():
     global timer_seconds, timer_update_id, score, Restart_button
@@ -336,15 +336,15 @@
     if action in actions[0:2] and is_on_main_window:
         button.invoke()
     elif action in actions[2:4] and is_on_typing_window:
         button.invoke()
 
 def start_app():
     try:
-        global current_scaling, timer_seconds, score, root, timer_choice, is_on_main_window, is_on_typing_window, scale, actions
+        global current_scaling, timer_seconds, score, root, timer_choice, is_on_main_window, is_on_typing_window, scale, actions 
         get_words()
         timer_seconds = 10
         score = 0  # Keeps score on how many words are right
         is_on_main_window = False
         is_on_typing_window = False
         actions = ["to_typing_window", "do_exit", "do_restart", "to_main_window"]
         current_scaling = "1.0"
```

### Comparing `typing_test_sdd-1.0.1/typing_test_sdd/words.json` & `typing_test_sdd-1.0.2/typing_test_sdd/words.json`

 * *Files identical despite different names*

### Comparing `typing_test_sdd-1.0.1/typing_test_sdd.egg-info/PKG-INFO` & `typing_test_sdd-1.0.2/typing_test_sdd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typing_test_sdd
-Version: 1.0.1
+Version: 1.0.2
 Summary: TKinter GUI Typing Test - Gaurav Surve 122SDD2
 Home-page: https://github.com/GauravS2507/Gaurav-Surve-SDD2-Project---Typing-Test
 Author: Gaurav Surve
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Education
```

