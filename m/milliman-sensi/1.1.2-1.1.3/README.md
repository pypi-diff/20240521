# Comparing `tmp/milliman_sensi-1.1.2.tar.gz` & `tmp/milliman_sensi-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milliman_sensi-1.1.2.tar", last modified: Fri May  3 09:57:53 2024, max compression
+gzip compressed data, was "milliman_sensi-1.1.3.tar", last modified: Tue May 21 14:51:30 2024, max compression
```

## Comparing `milliman_sensi-1.1.2.tar` & `milliman_sensi-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 09:57:53.191864 milliman_sensi-1.1.2/
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-03 09:57:48.000000 milliman_sensi-1.1.2/LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      822 2024-05-03 09:57:53.191864 milliman_sensi-1.1.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       49 2024-05-03 09:57:48.000000 milliman_sensi-1.1.2/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 09:57:53.191864 milliman_sensi-1.1.2/milliman_sensi/
--rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-05-03 09:57:48.000000 milliman_sensi-1.1.2/milliman_sensi/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-03 09:57:48.000000 milliman_sensi-1.1.2/milliman_sensi/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (127)    31081 2024-05-03 09:57:48.000000 milliman_sensi-1.1.2/milliman_sensi/io.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26358 2024-05-03 09:57:48.000000 milliman_sensi-1.1.2/milliman_sensi/syntax.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18064 2024-05-03 09:57:48.000000 milliman_sensi-1.1.2/milliman_sensi/table_diff.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12750 2024-05-03 09:57:48.000000 milliman_sensi-1.1.2/milliman_sensi/utility.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 09:57:53.191864 milliman_sensi-1.1.2/milliman_sensi.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      822 2024-05-03 09:57:53.000000 milliman_sensi-1.1.2/milliman_sensi.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      384 2024-05-03 09:57:53.000000 milliman_sensi-1.1.2/milliman_sensi.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-03 09:57:53.000000 milliman_sensi-1.1.2/milliman_sensi.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       34 2024-05-03 09:57:53.000000 milliman_sensi-1.1.2/milliman_sensi.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-05-03 09:57:53.000000 milliman_sensi-1.1.2/milliman_sensi.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       79 2024-05-03 09:57:53.191864 milliman_sensi-1.1.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1152 2024-05-03 09:57:49.000000 milliman_sensi-1.1.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 14:51:30.038361 milliman_sensi-1.1.3/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-21 14:51:27.000000 milliman_sensi-1.1.3/LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      822 2024-05-21 14:51:30.038361 milliman_sensi-1.1.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       49 2024-05-21 14:51:27.000000 milliman_sensi-1.1.3/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 14:51:30.038361 milliman_sensi-1.1.3/milliman_sensi/
+-rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-05-21 14:51:27.000000 milliman_sensi-1.1.3/milliman_sensi/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-21 14:51:27.000000 milliman_sensi-1.1.3/milliman_sensi/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30716 2024-05-21 14:51:27.000000 milliman_sensi-1.1.3/milliman_sensi/io.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26358 2024-05-21 14:51:27.000000 milliman_sensi-1.1.3/milliman_sensi/syntax.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18064 2024-05-21 14:51:27.000000 milliman_sensi-1.1.3/milliman_sensi/table_diff.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12750 2024-05-21 14:51:27.000000 milliman_sensi-1.1.3/milliman_sensi/utility.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 14:51:30.038361 milliman_sensi-1.1.3/milliman_sensi.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      822 2024-05-21 14:51:29.000000 milliman_sensi-1.1.3/milliman_sensi.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      384 2024-05-21 14:51:30.000000 milliman_sensi-1.1.3/milliman_sensi.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 14:51:29.000000 milliman_sensi-1.1.3/milliman_sensi.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       34 2024-05-21 14:51:29.000000 milliman_sensi-1.1.3/milliman_sensi.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-05-21 14:51:29.000000 milliman_sensi-1.1.3/milliman_sensi.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       79 2024-05-21 14:51:30.038361 milliman_sensi-1.1.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1152 2024-05-21 14:51:28.000000 milliman_sensi-1.1.3/setup.py
```

### Comparing `milliman_sensi-1.1.2/LICENSE.txt` & `milliman_sensi-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `milliman_sensi-1.1.2/PKG-INFO` & `milliman_sensi-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milliman_sensi
-Version: 1.1.2
+Version: 1.1.3
 Summary: A parser and modifier of the configuration in Milliman-CHESS
 Home-page: https://dev.azure.com/millimanparis/CHESS-Sensitivity-Manager
 Author: Quincy HSIEH
 Author-email: quincy.hsieh@milliman.com
 License: MIT
 Keywords: Milliman CHESS,configuration,parsers,sensitibity
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `milliman_sensi-1.1.2/milliman_sensi/io.py` & `milliman_sensi-1.1.3/milliman_sensi/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,24 +266,14 @@
             sensi_config[sensi_config["Scenario"] == sensi_name].set_index("Stress name")["Apply stress"].to_dict()
         )
         # Add keys from stress dict to sensi list if the value is True or 'true' (case insensitive)
         sensi_list[sensi_name] = [
             stress_name for stress_name, apply_stress in stress_dict.items() if apply_stress.lower() == "true"
         ]
 
-    # Get the list sensi_list_without_stress
-    sensi_list_without_stress = list()
-    logger.debug(f"Getting sensi list without stress")
-    for sensi_name, stress_list in sensi_list.items():
-        if len(stress_list)==0:
-            sensi_list_without_stress.append(sensi_name)
-
-    for s in sensi_list_without_stress:
-        sensi_list.pop(s)
-
     # Get the list param_list
     logger.debug(f"Getting unsorted param list")
     stress_names = list(sensi_param.columns)[1:]
     param_map_unsorted = {}
     for stress_name in stress_names:
         logger.debug(f"Adding the stress {stress_name} to the unsorted param list")
         # Select the rows where parameters are not null for the stress_name
@@ -299,15 +289,15 @@
     # Sort the param map unsorted by the order of the stress names in the 'Stress name' column
     # of the sensi config file where 'Apply stress' is True or 'true' (case insensitive)
     param_map = {
         stress_name: param_map_unsorted[stress_name]
         for stress_name in sensi_config[sensi_config["Apply stress"].str.lower() == "true"]["Stress name"].tolist()
     }
 
-    return sensi_list, sensi_list_without_stress, param_map
+    return sensi_list, sensi_names, param_map
 
 
 def read_sensitivities(env_dir):
     """Reads the sensitivities files
 
     Args:
         env_dir (str): Path to the environment directory
```

### Comparing `milliman_sensi-1.1.2/milliman_sensi/syntax.py` & `milliman_sensi-1.1.3/milliman_sensi/syntax.py`

 * *Files identical despite different names*

### Comparing `milliman_sensi-1.1.2/milliman_sensi/table_diff.py` & `milliman_sensi-1.1.3/milliman_sensi/table_diff.py`

 * *Files identical despite different names*

### Comparing `milliman_sensi-1.1.2/milliman_sensi/utility.py` & `milliman_sensi-1.1.3/milliman_sensi/utility.py`

 * *Files identical despite different names*

### Comparing `milliman_sensi-1.1.2/milliman_sensi.egg-info/PKG-INFO` & `milliman_sensi-1.1.3/milliman_sensi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milliman-sensi
-Version: 1.1.2
+Version: 1.1.3
 Summary: A parser and modifier of the configuration in Milliman-CHESS
 Home-page: https://dev.azure.com/millimanparis/CHESS-Sensitivity-Manager
 Author: Quincy HSIEH
 Author-email: quincy.hsieh@milliman.com
 License: MIT
 Keywords: Milliman CHESS,configuration,parsers,sensitibity
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `milliman_sensi-1.1.2/setup.py` & `milliman_sensi-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.6',
     ]
 
 # calling the setup function
 setup(name='milliman_sensi',
-      version="1.1.2",
+      version="1.1.3",
       description='A parser and modifier of the configuration in Milliman-CHESS',
       long_description="""A parser and modifier of CHESS's configuration
 To parse configuration files and apply them to create new sensitivity tables""",
       url='https://dev.azure.com/millimanparis/CHESS-Sensitivity-Manager',
       author='Quincy HSIEH',
       author_email='quincy.hsieh@milliman.com',
       license='MIT',
```

