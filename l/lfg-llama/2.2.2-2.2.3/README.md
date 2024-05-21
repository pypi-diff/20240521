# Comparing `tmp/lfg_llama-2.2.2.tar.gz` & `tmp/lfg_llama-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg_llama-2.2.2.tar", last modified: Tue May 21 19:24:02 2024, max compression
+gzip compressed data, was "lfg_llama-2.2.3.tar", last modified: Tue May 21 19:29:31 2024, max compression
```

## Comparing `lfg_llama-2.2.2.tar` & `lfg_llama-2.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 19:24:02.768077 lfg_llama-2.2.2/
--rw-r--r--   0 ob907      (502) staff       (20)     2526 2024-05-21 19:24:02.767892 lfg_llama-2.2.2/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)     2287 2024-05-21 19:22:15.000000 lfg_llama-2.2.2/README.md
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 19:24:02.766560 lfg_llama-2.2.2/lfg/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-2.2.2/lfg/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     2981 2024-05-20 18:00:32.000000 lfg_llama-2.2.2/lfg/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 19:24:02.767657 lfg_llama-2.2.2/lfg_llama.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     2526 2024-05-21 19:24:02.000000 lfg_llama-2.2.2/lfg_llama.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-21 19:24:02.000000 lfg_llama-2.2.2/lfg_llama.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-21 19:24:02.000000 lfg_llama-2.2.2/lfg_llama.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       56 2024-05-21 19:24:02.000000 lfg_llama-2.2.2/lfg_llama.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)        7 2024-05-21 19:24:02.000000 lfg_llama-2.2.2/lfg_llama.egg-info/requires.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-21 19:24:02.000000 lfg_llama-2.2.2/lfg_llama.egg-info/top_level.txt
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-21 19:24:02.768145 lfg_llama-2.2.2/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      484 2024-05-21 19:22:28.000000 lfg_llama-2.2.2/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 19:29:31.910034 lfg_llama-2.2.3/
+-rw-r--r--   0 ob907      (502) staff       (20)     2526 2024-05-21 19:29:31.909832 lfg_llama-2.2.3/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)     2287 2024-05-21 19:24:54.000000 lfg_llama-2.2.3/README.md
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 19:29:31.908555 lfg_llama-2.2.3/lfg/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-2.2.3/lfg/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     2981 2024-05-21 19:27:49.000000 lfg_llama-2.2.3/lfg/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 19:29:31.909587 lfg_llama-2.2.3/lfg_llama.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     2526 2024-05-21 19:29:31.000000 lfg_llama-2.2.3/lfg_llama.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-21 19:29:31.000000 lfg_llama-2.2.3/lfg_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-21 19:29:31.000000 lfg_llama-2.2.3/lfg_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       56 2024-05-21 19:29:31.000000 lfg_llama-2.2.3/lfg_llama.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        7 2024-05-21 19:29:31.000000 lfg_llama-2.2.3/lfg_llama.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-21 19:29:31.000000 lfg_llama-2.2.3/lfg_llama.egg-info/top_level.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-21 19:29:31.910086 lfg_llama-2.2.3/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      484 2024-05-21 19:29:14.000000 lfg_llama-2.2.3/setup.py
```

### Comparing `lfg_llama-2.2.2/PKG-INFO` & `lfg_llama-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 2.2.2
+Version: 2.2.3
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 
-# LFG
-
 <div align="center">
   <img src="logo.png" alt="logo" />
 </div>
 
 <h1 align="center">LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙</h1>
 
 <div align="center">
   LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. Such sales pitch. This interface is using GPT-4o as an engine.
 </div>
+<br />
 
 ![Demo](example.png)
 
 ## Why?
 
 - Firstly, this was created to test Ollama -> Groq
 - I do not like the Github Copilot command-line
```

### Comparing `lfg_llama-2.2.2/README.md` & `lfg_llama-2.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# LFG
-
 <div align="center">
   <img src="logo.png" alt="logo" />
 </div>
 
 <h1 align="center">LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙</h1>
 
 <div align="center">
   LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. Such sales pitch. This interface is using GPT-4o as an engine.
 </div>
+<br />
 
 ![Demo](example.png)
 
 ## Why?
 
 - Firstly, this was created to test Ollama -> Groq
 - I do not like the Github Copilot command-line
```

### Comparing `lfg_llama-2.2.2/lfg/cli.py` & `lfg_llama-2.2.3/lfg/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         print(e.response)
 
 
 def main():
     """Initializes the OpenAI client, and processes the query."""
 
     if len(sys.argv) < 2:
-        print("Usage: lfg <query>")
+        print("Usage: ask <query>")
 
         sys.exit(1)
 
     query = " ".join(sys.argv[1:])
 
     try:
         client = get_openai_client()
```

### Comparing `lfg_llama-2.2.2/lfg_llama.egg-info/PKG-INFO` & `lfg_llama-2.2.3/lfg_llama.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 2.2.2
+Version: 2.2.3
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 
-# LFG
-
 <div align="center">
   <img src="logo.png" alt="logo" />
 </div>
 
 <h1 align="center">LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙</h1>
 
 <div align="center">
   LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. Such sales pitch. This interface is using GPT-4o as an engine.
 </div>
+<br />
 
 ![Demo](example.png)
 
 ## Why?
 
 - Firstly, this was created to test Ollama -> Groq
 - I do not like the Github Copilot command-line
```

