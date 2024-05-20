# Comparing `tmp/jeffutils-0.5.8.tar.gz` & `tmp/jeffutils-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.5.8.tar", last modified: Thu May 16 17:55:19 2024, max compression
+gzip compressed data, was "jeffutils-0.5.9.tar", last modified: Mon May 20 22:26:14 2024, max compression
```

## Comparing `jeffutils-0.5.8.tar` & `jeffutils-0.5.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-16 17:55:19.758092 jeffutils-0.5.8/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.5.8/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-16 17:55:19.758092 jeffutils-0.5.8/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.5.8/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.5.8/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-16 17:55:19.758092 jeffutils-0.5.8/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-16 17:55:13.000000 jeffutils-0.5.8/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-16 17:55:19.758092 jeffutils-0.5.8/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-16 17:55:19.758092 jeffutils-0.5.8/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.5.8/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    25427 2024-05-16 17:53:50.000000 jeffutils-0.5.8/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-16 17:55:19.758092 jeffutils-0.5.8/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-16 17:55:19.000000 jeffutils-0.5.8/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-16 17:55:19.000000 jeffutils-0.5.8/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-16 17:55:19.000000 jeffutils-0.5.8/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-16 17:55:19.000000 jeffutils-0.5.8/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-20 22:26:14.645170 jeffutils-0.5.9/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.5.9/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-20 22:26:14.645170 jeffutils-0.5.9/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.5.9/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.5.9/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-20 22:26:14.645170 jeffutils-0.5.9/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-20 22:26:09.000000 jeffutils-0.5.9/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-20 22:26:14.645170 jeffutils-0.5.9/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-20 22:26:14.645170 jeffutils-0.5.9/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.5.9/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    25296 2024-05-20 22:25:58.000000 jeffutils-0.5.9/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-20 22:26:14.645170 jeffutils-0.5.9/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-20 22:26:14.000000 jeffutils-0.5.9/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-20 22:26:14.000000 jeffutils-0.5.9/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-20 22:26:14.000000 jeffutils-0.5.9/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-20 22:26:14.000000 jeffutils-0.5.9/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.5.8/LICENSE.txt` & `jeffutils-0.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.5.8/setup.py` & `jeffutils-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.5.8',
+    version='0.5.9',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.5.8/src/jeffutils/utils.py` & `jeffutils-0.5.9/src/jeffutils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,16 @@
         file.write(string)
         file.write(end)
         if header:
             if end == "\n":
                 file.write("-"*3 + "\n")
             else:
                 file.write("\n" + "-"*3 + "\n")
-                
+            
+
 def get_log_dict(var_names, globals, locals):
     """ takes in a list of strings that represent variable names, and 
     takes in the locals() dictionary. Returns a dictionary of the form:
     {
         var_name1: var_value1,
         var_name2: var_value2,
     }
@@ -137,15 +138,16 @@
         if len(curr_line + curr) > LENGTH_LIM:
             string += curr_line + "\n    "
             curr_line = ""
         curr_line += curr
     
     return string + curr_line
 
-def log_func_vars(func_name, vars, globals, locals, header=True, LOG_TOGGLE=None):
+@print_skip_exceptions(full_stack_trace=False, log_error=True)
+def log_func_vars(func_name, vars, globals, locals, header=True):
     """
     Logs the information in a formatted way.
 
     Parameters:
     func_name (str): The title of the function that is making this log.
     vars (list): a list of strings that represent the variable names to log.
     globals (dict): The global variables dictionary, typically passed as globals().
@@ -158,19 +160,14 @@
     
     Returns:
     str: The formatted log string.
 
     Notes:
     - The function will default to logging the information unless the LOG_TOGGLE dictionary has the function name set to False.
     """
-    if LOG_TOGGLE is None:
-        LOG_TOGGLE = {}
-    # default to logging the function instead of not logging it
-    if not LOG_TOGGLE.get(func_name, True):
-        return
     info_dict = get_log_dict(vars, globals, locals)
     string = get_log_string(func_name, info_dict)
     log_print(string, header=header)
     
     return string
 
 def initialize_log_func_vars_func(LOG_TOGGLE):
```

