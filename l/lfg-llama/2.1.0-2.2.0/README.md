# Comparing `tmp/lfg_llama-2.1.0.tar.gz` & `tmp/lfg_llama-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg_llama-2.1.0.tar", last modified: Mon May 20 18:04:06 2024, max compression
+gzip compressed data, was "lfg_llama-2.2.0.tar", last modified: Tue May 21 16:34:15 2024, max compression
```

## Comparing `lfg_llama-2.1.0.tar` & `lfg_llama-2.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-20 18:04:06.711848 lfg_llama-2.1.0/
--rw-r--r--   0 ob907      (502) staff       (20)     2329 2024-05-20 18:04:06.711636 lfg_llama-2.1.0/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)     2090 2024-05-20 18:02:28.000000 lfg_llama-2.1.0/README.md
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-20 18:04:06.710467 lfg_llama-2.1.0/lfg/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-2.1.0/lfg/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     2981 2024-05-20 18:00:32.000000 lfg_llama-2.1.0/lfg/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-20 18:04:06.711402 lfg_llama-2.1.0/lfg_llama.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     2329 2024-05-20 18:04:06.000000 lfg_llama-2.1.0/lfg_llama.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-20 18:04:06.000000 lfg_llama-2.1.0/lfg_llama.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-20 18:04:06.000000 lfg_llama-2.1.0/lfg_llama.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-20 18:04:06.000000 lfg_llama-2.1.0/lfg_llama.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)        7 2024-05-20 18:04:06.000000 lfg_llama-2.1.0/lfg_llama.egg-info/requires.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-20 18:04:06.000000 lfg_llama-2.1.0/lfg_llama.egg-info/top_level.txt
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-20 18:04:06.711905 lfg_llama-2.1.0/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      464 2024-05-20 18:00:42.000000 lfg_llama-2.1.0/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 16:34:15.286441 lfg_llama-2.2.0/
+-rw-r--r--   0 ob907      (502) staff       (20)     2409 2024-05-21 16:34:15.286249 lfg_llama-2.2.0/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)     2170 2024-05-21 16:33:54.000000 lfg_llama-2.2.0/README.md
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 16:34:15.284912 lfg_llama-2.2.0/lfg/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-2.2.0/lfg/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     2981 2024-05-20 18:00:32.000000 lfg_llama-2.2.0/lfg/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 16:34:15.286022 lfg_llama-2.2.0/lfg_llama.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     2409 2024-05-21 16:34:15.000000 lfg_llama-2.2.0/lfg_llama.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-21 16:34:15.000000 lfg_llama-2.2.0/lfg_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-21 16:34:15.000000 lfg_llama-2.2.0/lfg_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       56 2024-05-21 16:34:15.000000 lfg_llama-2.2.0/lfg_llama.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        7 2024-05-21 16:34:15.000000 lfg_llama-2.2.0/lfg_llama.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-21 16:34:15.000000 lfg_llama-2.2.0/lfg_llama.egg-info/top_level.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-21 16:34:15.286488 lfg_llama-2.2.0/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      484 2024-05-21 16:34:06.000000 lfg_llama-2.2.0/setup.py
```

### Comparing `lfg_llama-2.1.0/PKG-INFO` & `lfg_llama-2.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 2.1.0
+Version: 2.2.0
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 
 # LFG
@@ -47,34 +47,39 @@
 
 Add the token to your .bashrc/.zshrc and reload your terminal.
 
 ```
 export OPENAI_API_KEY={replace_me}
 ```
 
-```
-$ lfg query
+You can use either of these commands
+
+```bash
+$ lfg <query>
+$ ask <query>
 ```
 
 Now you can use the executable
 
 ```bash
+$ ask kill port 3000
+
 fuser -k 3000/tcp
 
 Explanation:
 The `fuser` command identifies processes using files or sockets. The `-k` option is used to kill th
 ose processes. Here, `3000/tcp` specifies the TCP port number 3000. This command effectively kills
 any process currently using port 3000.
 
 ```
 
 Change the LLM
 
 ```bash
-$ lfg list ec2 pipe json jq get name
+$ ask list ec2 pipe json jq get name
 
 aws ec2 describe-instances --query "Reservations[].Instances[].{Name:Tags[?Key=='Name']|[0].Value}"
  --output json | jq -r '.[].Name'
 
 Explanation:
 This command uses the AWS CLI to list EC2 instances and their corresponding 'Name' tag values in JS
 ON format. The `--query` option filters the output to only include the 'Name' tag for each instance
```

### Comparing `lfg_llama-2.1.0/README.md` & `lfg_llama-2.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -38,34 +38,39 @@
 
 Add the token to your .bashrc/.zshrc and reload your terminal.
 
 ```
 export OPENAI_API_KEY={replace_me}
 ```
 
-```
-$ lfg query
+You can use either of these commands
+
+```bash
+$ lfg <query>
+$ ask <query>
 ```
 
 Now you can use the executable
 
 ```bash
+$ ask kill port 3000
+
 fuser -k 3000/tcp
 
 Explanation:
 The `fuser` command identifies processes using files or sockets. The `-k` option is used to kill th
 ose processes. Here, `3000/tcp` specifies the TCP port number 3000. This command effectively kills
 any process currently using port 3000.
 
 ```
 
 Change the LLM
 
 ```bash
-$ lfg list ec2 pipe json jq get name
+$ ask list ec2 pipe json jq get name
 
 aws ec2 describe-instances --query "Reservations[].Instances[].{Name:Tags[?Key=='Name']|[0].Value}"
  --output json | jq -r '.[].Name'
 
 Explanation:
 This command uses the AWS CLI to list EC2 instances and their corresponding 'Name' tag values in JS
 ON format. The `--query` option filters the output to only include the 'Name' tag for each instance
```

### Comparing `lfg_llama-2.1.0/lfg/cli.py` & `lfg_llama-2.2.0/lfg/cli.py`

 * *Files identical despite different names*

### Comparing `lfg_llama-2.1.0/lfg_llama.egg-info/PKG-INFO` & `lfg_llama-2.2.0/lfg_llama.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 2.1.0
+Version: 2.2.0
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 
 # LFG
@@ -47,34 +47,39 @@
 
 Add the token to your .bashrc/.zshrc and reload your terminal.
 
 ```
 export OPENAI_API_KEY={replace_me}
 ```
 
-```
-$ lfg query
+You can use either of these commands
+
+```bash
+$ lfg <query>
+$ ask <query>
 ```
 
 Now you can use the executable
 
 ```bash
+$ ask kill port 3000
+
 fuser -k 3000/tcp
 
 Explanation:
 The `fuser` command identifies processes using files or sockets. The `-k` option is used to kill th
 ose processes. Here, `3000/tcp` specifies the TCP port number 3000. This command effectively kills
 any process currently using port 3000.
 
 ```
 
 Change the LLM
 
 ```bash
-$ lfg list ec2 pipe json jq get name
+$ ask list ec2 pipe json jq get name
 
 aws ec2 describe-instances --query "Reservations[].Instances[].{Name:Tags[?Key=='Name']|[0].Value}"
  --output json | jq -r '.[].Name'
 
 Explanation:
 This command uses the AWS CLI to list EC2 instances and their corresponding 'Name' tag values in JS
 ON format. The `--query` option filters the output to only include the 'Name' tag for each instance
```

