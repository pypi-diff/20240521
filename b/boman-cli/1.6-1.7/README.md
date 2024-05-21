# Comparing `tmp/boman-cli-1.6.tar.gz` & `tmp/boman-cli-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boman-cli-1.6.tar", last modified: Mon May 20 13:24:06 2024, max compression
+gzip compressed data, was "boman-cli-1.7.tar", last modified: Tue May 21 05:52:02 2024, max compression
```

## Comparing `boman-cli-1.6.tar` & `boman-cli-1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2024-05-20 13:24:06.644035 boman-cli-1.6/
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2657 2024-05-20 13:24:06.644035 boman-cli-1.6/PKG-INFO
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1607 2024-05-20 13:21:01.000000 boman-cli-1.6/README.md
-drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2024-05-20 13:24:06.640035 boman-cli-1.6/boman_cli.egg-info/
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2657 2024-05-20 13:24:06.000000 boman-cli-1.6/boman_cli.egg-info/PKG-INFO
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)      426 2024-05-20 13:24:06.000000 boman-cli-1.6/boman_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        1 2024-05-20 13:24:06.000000 boman-cli-1.6/boman_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)       53 2024-05-20 13:24:06.000000 boman-cli-1.6/boman_cli.egg-info/entry_points.txt
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)       45 2024-05-20 13:24:06.000000 boman-cli-1.6/boman_cli.egg-info/requires.txt
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        9 2024-05-20 13:24:06.000000 boman-cli-1.6/boman_cli.egg-info/top_level.txt
-drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2024-05-20 13:24:06.640035 boman-cli-1.6/bomancli/
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2353 2024-05-20 12:43:07.000000 boman-cli-1.6/bomancli/Config.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        0 2023-12-12 08:27:09.000000 boman-cli-1.6/bomancli/_init_.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2306 2024-05-14 06:41:19.000000 boman-cli-1.6/bomancli/auth.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1203 2024-03-20 08:09:57.000000 boman-cli-1.6/bomancli/base_logger.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1702 2024-03-23 11:50:57.000000 boman-cli-1.6/bomancli/loc_finder.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)    39585 2024-05-20 13:14:09.000000 boman-cli-1.6/bomancli/main.py
-drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2024-05-20 13:24:06.644035 boman-cli-1.6/bomancli/templates/
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     4529 2024-05-15 08:44:53.000000 boman-cli-1.6/bomancli/templates/template_plan.yaml
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)    25357 2024-05-20 12:42:11.000000 boman-cli-1.6/bomancli/utils.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     7696 2024-02-14 08:06:15.000000 boman-cli-1.6/bomancli/validation.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)      144 2024-05-20 13:24:06.644035 boman-cli-1.6/setup.cfg
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1768 2024-05-20 12:43:34.000000 boman-cli-1.6/setup.py
+drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2024-05-21 05:52:02.903509 boman-cli-1.7/
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2708 2024-05-21 05:52:02.903509 boman-cli-1.7/PKG-INFO
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1651 2024-05-21 05:49:01.000000 boman-cli-1.7/README.md
+drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2024-05-21 05:52:02.887509 boman-cli-1.7/boman_cli.egg-info/
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2708 2024-05-21 05:52:02.000000 boman-cli-1.7/boman_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)      426 2024-05-21 05:52:02.000000 boman-cli-1.7/boman_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        1 2024-05-21 05:52:02.000000 boman-cli-1.7/boman_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)       53 2024-05-21 05:52:02.000000 boman-cli-1.7/boman_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)       76 2024-05-21 05:52:02.000000 boman-cli-1.7/boman_cli.egg-info/requires.txt
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        9 2024-05-21 05:52:02.000000 boman-cli-1.7/boman_cli.egg-info/top_level.txt
+drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2024-05-21 05:52:02.903509 boman-cli-1.7/bomancli/
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2352 2024-05-21 05:48:12.000000 boman-cli-1.7/bomancli/Config.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        0 2023-12-12 08:27:09.000000 boman-cli-1.7/bomancli/_init_.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2306 2024-05-14 06:41:19.000000 boman-cli-1.7/bomancli/auth.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1203 2024-03-20 08:09:57.000000 boman-cli-1.7/bomancli/base_logger.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1702 2024-03-23 11:50:57.000000 boman-cli-1.7/bomancli/loc_finder.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)    39597 2024-05-21 05:49:16.000000 boman-cli-1.7/bomancli/main.py
+drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2024-05-21 05:52:02.903509 boman-cli-1.7/bomancli/templates/
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     4529 2024-05-15 08:44:53.000000 boman-cli-1.7/bomancli/templates/template_plan.yaml
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)    25357 2024-05-20 12:42:11.000000 boman-cli-1.7/bomancli/utils.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     7696 2024-02-14 08:06:15.000000 boman-cli-1.7/bomancli/validation.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)      144 2024-05-21 05:52:02.907509 boman-cli-1.7/setup.cfg
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1800 2024-05-21 05:47:50.000000 boman-cli-1.7/setup.py
```

### Comparing `boman-cli-1.6/PKG-INFO` & `boman-cli-1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boman-cli
-Version: 1.6
+Version: 1.7
 Summary: CLI tool of boman.ai
 Home-page: https://boman.ai
 Author: Sumeru Software Solutions Pvt. Ltd.
 Author-email: support@boman.ai
 License: BSD 2-clause
 Description: # Introduction 
         Boman CLI is a Orchestration script written in python to run security scans on the customer's local or CI/CD environment and upload the results to Boman.ai SaaS server.
@@ -73,21 +73,22 @@
         
         
         
         
         ### Release Note:
         
         
-        ### V1.6:
+        ### V1.7:
         
+            - Fixed docker-request libraries issue
             - Zap Authenticated scan 
             - Fetch Git details
             - custom boman.yaml and zap session script load option
         
-        Released on: 20 May 2024
+        Released on: 21 May 2024
         
         
         
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `boman-cli-1.6/README.md` & `boman-cli-1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -65,18 +65,19 @@
 
 
 
 
 ### Release Note:
 
 
-### V1.6:
+### V1.7:
 
+    - Fixed docker-request libraries issue
     - Zap Authenticated scan 
     - Fetch Git details
     - custom boman.yaml and zap session script load option
 
-Released on: 20 May 2024
+Released on: 21 May 2024
```

### Comparing `boman-cli-1.6/boman_cli.egg-info/PKG-INFO` & `boman-cli-1.7/boman_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boman-cli
-Version: 1.6
+Version: 1.7
 Summary: CLI tool of boman.ai
 Home-page: https://boman.ai
 Author: Sumeru Software Solutions Pvt. Ltd.
 Author-email: support@boman.ai
 License: BSD 2-clause
 Description: # Introduction 
         Boman CLI is a Orchestration script written in python to run security scans on the customer's local or CI/CD environment and upload the results to Boman.ai SaaS server.
@@ -73,21 +73,22 @@
         
         
         
         
         ### Release Note:
         
         
-        ### V1.6:
+        ### V1.7:
         
+            - Fixed docker-request libraries issue
             - Zap Authenticated scan 
             - Fetch Git details
             - custom boman.yaml and zap session script load option
         
-        Released on: 20 May 2024
+        Released on: 21 May 2024
         
         
         
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `boman-cli-1.6/bomancli/Config.py` & `boman-cli-1.7/bomancli/Config.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class Config:
 
     #boman_url
     try:
         docker_client = docker.from_env()
     except Exception as e:
         print('Docker not found in your machine, Pls install')
-        #print(str(e))
+        print(str(e))
         exit(3) ## docker/system error
 
     boman_url = "https://dashboard.boman.ai/v2/"  ## boman server ip // https://dashboard.boman.ai http://192.168.1.6:3000
 
     boman_base_url = "https://dashboard.boman.ai/"
 
     sast_present = None
@@ -109,10 +109,10 @@
     lingu_details = {}
 
     log_stream = None
 
 
     log_level = "INFO"
 
-    version = 'v1.6'
+    version = 'v1.7'
 
     boman_config_file = 'boman.yaml'
```

### Comparing `boman-cli-1.6/bomancli/auth.py` & `boman-cli-1.7/bomancli/auth.py`

 * *Files identical despite different names*

### Comparing `boman-cli-1.6/bomancli/base_logger.py` & `boman-cli-1.7/bomancli/base_logger.py`

 * *Files identical despite different names*

### Comparing `boman-cli-1.6/bomancli/loc_finder.py` & `boman-cli-1.7/bomancli/loc_finder.py`

 * *Files identical despite different names*

### Comparing `boman-cli-1.6/bomancli/main.py` & `boman-cli-1.7/bomancli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -836,20 +836,20 @@
         ##logging.info('jenkins is choosen')
         Config.jenkins = 'yes'
     else:
         ###logging.info('jenkins is not choosen')
         Config.jenkins = 'no'  
 
     ## lingu user id set
-    if args.user_id == '1000:1000':
-        ##logging.info('jenkins is choosen')
-        Config.lingu_user = '1000:1000'
-    else:
-        ###logging.info('jenkins is not choosen')
-        Config.lingu_user = args.user_id  
+    # if args.user_id == '1000:1000':
+    #     ##logging.info('jenkins is choosen')
+    #     Config.lingu_user = '1000:1000'
+    # else:
+    #     ###logging.info('jenkins is not choosen')
+    #     Config.lingu_user = args.user_id  
 
 
     if args.config == 'boman.yaml':
         ##logging.info('jenkins is choosen')
         Config.boman_config_file = 'boman.yaml'
     else:
         ###logging.info('jenkins is not choosen')
```

### Comparing `boman-cli-1.6/bomancli/templates/template_plan.yaml` & `boman-cli-1.7/bomancli/templates/template_plan.yaml`

 * *Files identical despite different names*

### Comparing `boman-cli-1.6/bomancli/utils.py` & `boman-cli-1.7/bomancli/utils.py`

 * *Files identical despite different names*

### Comparing `boman-cli-1.6/bomancli/validation.py` & `boman-cli-1.7/bomancli/validation.py`

 * *Files identical despite different names*

### Comparing `boman-cli-1.6/setup.py` & `boman-cli-1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 import configparser
-from bomancli.Config import Config
+#from bomancli.Config import Config
 
 config = configparser.ConfigParser()
 config.read('setup.cfg')
 environment = config['metadata']['environment']
 version = config['metadata']['version']
 name = config['metadata']['name']
 base_url = config['metadata']['saas_base_url']
-Config.boman_base_url = base_url
+#Config.boman_base_url = base_url
 
 try:
     import pypandoc
     long_description = pypandoc.convert_file('README.md', 'rst')
 except(IOError, ImportError):
     long_description = open('README.md').read()
 
@@ -43,20 +43,19 @@
     url='https://boman.ai',
     author='Sumeru Software Solutions Pvt. Ltd.',
     author_email='support@boman.ai',
     license='BSD 2-clause',
     entry_points = entry_points,
     packages=['bomancli'],
     package_data={'bomancli': ['templates/template_plan.yaml']},
-    install_requires=['docker',
-                      'requests',
+    install_requires=['docker<=7.0.0',
+                      'requests<=2.31.0',
                       'pyyaml',
-                      'coloredlogs','xmltodict'                     
+                      'coloredlogs<=15.0.1','xmltodict<=0.13.0'                     
                       ],
-
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',  
         'Operating System :: OS Independent',        
     ],
 )
```

