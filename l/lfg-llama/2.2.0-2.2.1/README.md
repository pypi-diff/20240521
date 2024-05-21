# Comparing `tmp/lfg_llama-2.2.0.tar.gz` & `tmp/lfg_llama-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg_llama-2.2.0.tar", last modified: Tue May 21 16:34:15 2024, max compression
+gzip compressed data, was "lfg_llama-2.2.1.tar", last modified: Tue May 21 18:58:01 2024, max compression
```

## Comparing `lfg_llama-2.2.0.tar` & `lfg_llama-2.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 16:34:15.286441 lfg_llama-2.2.0/
--rw-r--r--   0 ob907      (502) staff       (20)     2409 2024-05-21 16:34:15.286249 lfg_llama-2.2.0/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)     2170 2024-05-21 16:33:54.000000 lfg_llama-2.2.0/README.md
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 16:34:15.284912 lfg_llama-2.2.0/lfg/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-2.2.0/lfg/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     2981 2024-05-20 18:00:32.000000 lfg_llama-2.2.0/lfg/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 16:34:15.286022 lfg_llama-2.2.0/lfg_llama.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     2409 2024-05-21 16:34:15.000000 lfg_llama-2.2.0/lfg_llama.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-21 16:34:15.000000 lfg_llama-2.2.0/lfg_llama.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-21 16:34:15.000000 lfg_llama-2.2.0/lfg_llama.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       56 2024-05-21 16:34:15.000000 lfg_llama-2.2.0/lfg_llama.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)        7 2024-05-21 16:34:15.000000 lfg_llama-2.2.0/lfg_llama.egg-info/requires.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-21 16:34:15.000000 lfg_llama-2.2.0/lfg_llama.egg-info/top_level.txt
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-21 16:34:15.286488 lfg_llama-2.2.0/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      484 2024-05-21 16:34:06.000000 lfg_llama-2.2.0/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 18:58:01.790080 lfg_llama-2.2.1/
+-rw-r--r--   0 ob907      (502) staff       (20)     2409 2024-05-21 18:58:01.789866 lfg_llama-2.2.1/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)     2170 2024-05-21 18:57:32.000000 lfg_llama-2.2.1/README.md
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 18:58:01.788652 lfg_llama-2.2.1/lfg/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-2.2.1/lfg/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     2981 2024-05-20 18:00:32.000000 lfg_llama-2.2.1/lfg/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 18:58:01.789666 lfg_llama-2.2.1/lfg_llama.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     2409 2024-05-21 18:58:01.000000 lfg_llama-2.2.1/lfg_llama.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-21 18:58:01.000000 lfg_llama-2.2.1/lfg_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-21 18:58:01.000000 lfg_llama-2.2.1/lfg_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       56 2024-05-21 18:58:01.000000 lfg_llama-2.2.1/lfg_llama.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        7 2024-05-21 18:58:01.000000 lfg_llama-2.2.1/lfg_llama.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-21 18:58:01.000000 lfg_llama-2.2.1/lfg_llama.egg-info/top_level.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-21 18:58:01.790161 lfg_llama-2.2.1/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      484 2024-05-21 18:57:38.000000 lfg_llama-2.2.1/setup.py
```

### Comparing `lfg_llama-2.2.0/PKG-INFO` & `lfg_llama-2.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 2.2.0
+Version: 2.2.1
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 
 # LFG
 
 > LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 
-![Demo](example.gif)
+![Demo](example.png)
 
 LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. Such sales pitch. This interface is using GPT-4o as an engine.
 
 ## Why?
 
 - Firstly, this was created to test Ollama -> Groq
 - I do not like the Github Copilot command-line
```

### Comparing `lfg_llama-2.2.0/README.md` & `lfg_llama-2.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # LFG
 
 > LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 
-![Demo](example.gif)
+![Demo](example.png)
 
 LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. Such sales pitch. This interface is using GPT-4o as an engine.
 
 ## Why?
 
 - Firstly, this was created to test Ollama -> Groq
 - I do not like the Github Copilot command-line
```

### Comparing `lfg_llama-2.2.0/lfg/cli.py` & `lfg_llama-2.2.1/lfg/cli.py`

 * *Files identical despite different names*

### Comparing `lfg_llama-2.2.0/lfg_llama.egg-info/PKG-INFO` & `lfg_llama-2.2.1/lfg_llama.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 2.2.0
+Version: 2.2.1
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 
 # LFG
 
 > LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 
-![Demo](example.gif)
+![Demo](example.png)
 
 LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. Such sales pitch. This interface is using GPT-4o as an engine.
 
 ## Why?
 
 - Firstly, this was created to test Ollama -> Groq
 - I do not like the Github Copilot command-line
```

