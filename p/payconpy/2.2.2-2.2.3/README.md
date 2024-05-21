# Comparing `tmp/payconpy-2.2.2.tar.gz` & `tmp/payconpy-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payconpy-2.2.2.tar", last modified: Tue May 21 15:15:18 2024, max compression
+gzip compressed data, was "payconpy-2.2.3.tar", last modified: Tue May 21 15:17:31 2024, max compression
```

## Comparing `payconpy-2.2.2.tar` & `payconpy-2.2.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.417829 payconpy-2.2.2/
--rw-rw-rw-   0        0        0     1073 2024-03-28 18:34:30.000000 payconpy-2.2.2/LICENSE
--rw-rw-rw-   0        0        0      920 2024-05-21 15:15:18.411279 payconpy-2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      456 2024-04-21 22:27:53.000000 payconpy-2.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 15:15:17.890278 payconpy-2.2.2/payconpy/
-drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.024371 payconpy-2.2.2/payconpy/femails/
--rw-rw-rw-   0        0        0       40 2024-03-28 18:29:40.000000 payconpy-2.2.2/payconpy/femails/__init__.py
--rw-rw-rw-   0        0        0     7021 2024-03-28 18:29:45.000000 payconpy-2.2.2/payconpy/femails/femails.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.044769 payconpy-2.2.2/payconpy/fexceptions/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.2/payconpy/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2023-09-12 12:27:01.000000 payconpy-2.2.2/payconpy/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.056142 payconpy-2.2.2/payconpy/fpdf/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.2/payconpy/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.072878 payconpy-2.2.2/payconpy/fpdf/focr/
--rw-rw-rw-   0        0        0      104 2024-03-28 18:29:53.000000 payconpy-2.2.2/payconpy/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0    10766 2024-05-21 14:26:58.000000 payconpy-2.2.2/payconpy/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.089242 payconpy-2.2.2/payconpy/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.2/payconpy/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     5758 2024-04-21 19:13:23.000000 payconpy-2.2.2/payconpy/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.109237 payconpy-2.2.2/payconpy/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2023-09-12 12:27:01.000000 payconpy-2.2.2/payconpy/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4676 2024-03-28 17:58:49.000000 payconpy-2.2.2/payconpy/fpysimplegui/fpysimplegui.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.129547 payconpy-2.2.2/payconpy/fpython/
--rw-rw-rw-   0        0        0       25 2023-09-12 12:27:01.000000 payconpy-2.2.2/payconpy/fpython/__init__.py
--rw-rw-rw-   0        0        0    56910 2024-05-21 15:14:57.000000 payconpy-2.2.2/payconpy/fpython/fpython.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.187835 payconpy-2.2.2/payconpy/fregex/
--rw-rw-rw-   0        0        0       24 2023-09-12 12:27:01.000000 payconpy-2.2.2/payconpy/fregex/__init__.py
--rw-rw-rw-   0        0        0    10366 2024-03-28 17:52:21.000000 payconpy-2.2.2/payconpy/fregex/fregex.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.241729 payconpy-2.2.2/payconpy/fselenium/
--rw-rw-rw-   0        0        0       27 2023-09-12 12:27:01.000000 payconpy-2.2.2/payconpy/fselenium/__init__.py
--rw-rw-rw-   0        0        0    40190 2024-03-28 20:51:18.000000 payconpy-2.2.2/payconpy/fselenium/fselenium.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.278336 payconpy-2.2.2/payconpy/odoo/
--rw-rw-rw-   0        0        0        0 2024-04-21 19:01:38.000000 payconpy-2.2.2/payconpy/odoo/__init__.py
--rw-rw-rw-   0        0        0    11717 2024-05-13 20:36:27.000000 payconpy-2.2.2/payconpy/odoo/odoo_xmlrpc.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.311315 payconpy-2.2.2/payconpy/openai/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.2/payconpy/openai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.328970 payconpy-2.2.2/payconpy/openai/apis/
--rw-rw-rw-   0        0        0        0 2024-04-21 21:37:31.000000 payconpy-2.2.2/payconpy/openai/apis/__init__.py
--rw-rw-rw-   0        0        0     3192 2024-04-21 21:37:47.000000 payconpy-2.2.2/payconpy/openai/apis/apis.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.360531 payconpy-2.2.2/payconpy/openai/assistants/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.2/payconpy/openai/assistants/__init__.py
--rw-rw-rw-   0        0        0     4085 2023-11-27 13:03:14.000000 payconpy-2.2.2/payconpy/openai/assistants/assistants.py
--rw-rw-rw-   0        0        0     4427 2023-11-27 14:53:41.000000 payconpy-2.2.2/payconpy/openai/get_cost.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.396149 payconpy-2.2.2/payconpy/utils/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.2/payconpy/utils/__init__.py
--rw-rw-rw-   0        0        0   195592 2024-05-21 14:36:04.000000 payconpy-2.2.2/payconpy/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.007547 payconpy-2.2.2/payconpy.egg-info/
--rw-rw-rw-   0        0        0      920 2024-05-21 15:15:17.000000 payconpy-2.2.2/payconpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1013 2024-05-21 15:15:17.000000 payconpy-2.2.2/payconpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 15:15:17.000000 payconpy-2.2.2/payconpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      181 2024-05-21 15:15:17.000000 payconpy-2.2.2/payconpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0      261 2024-05-21 15:15:17.000000 payconpy-2.2.2/payconpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 15:15:18.421159 payconpy-2.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2093 2024-05-21 15:15:11.000000 payconpy-2.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:31.642638 payconpy-2.2.3/
+-rw-rw-rw-   0        0        0     1073 2024-03-28 18:34:30.000000 payconpy-2.2.3/LICENSE
+-rw-rw-rw-   0        0        0      920 2024-05-21 15:17:31.636970 payconpy-2.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2024-04-21 22:27:53.000000 payconpy-2.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:31.286863 payconpy-2.2.3/payconpy/
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:31.392625 payconpy-2.2.3/payconpy/femails/
+-rw-rw-rw-   0        0        0       40 2024-03-28 18:29:40.000000 payconpy-2.2.3/payconpy/femails/__init__.py
+-rw-rw-rw-   0        0        0     7021 2024-03-28 18:29:45.000000 payconpy-2.2.3/payconpy/femails/femails.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:31.409843 payconpy-2.2.3/payconpy/fexceptions/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.3/payconpy/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-09-12 12:27:01.000000 payconpy-2.2.3/payconpy/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:31.418024 payconpy-2.2.3/payconpy/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.3/payconpy/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:31.436638 payconpy-2.2.3/payconpy/fpdf/focr/
+-rw-rw-rw-   0        0        0      104 2024-03-28 18:29:53.000000 payconpy-2.2.3/payconpy/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0    10766 2024-05-21 14:26:58.000000 payconpy-2.2.3/payconpy/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:31.458756 payconpy-2.2.3/payconpy/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.3/payconpy/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     5758 2024-04-21 19:13:23.000000 payconpy-2.2.3/payconpy/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:31.476324 payconpy-2.2.3/payconpy/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2023-09-12 12:27:01.000000 payconpy-2.2.3/payconpy/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4676 2024-03-28 17:58:49.000000 payconpy-2.2.3/payconpy/fpysimplegui/fpysimplegui.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:31.497684 payconpy-2.2.3/payconpy/fpython/
+-rw-rw-rw-   0        0        0       25 2023-09-12 12:27:01.000000 payconpy-2.2.3/payconpy/fpython/__init__.py
+-rw-rw-rw-   0        0        0    56944 2024-05-21 15:17:18.000000 payconpy-2.2.3/payconpy/fpython/fpython.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:31.517552 payconpy-2.2.3/payconpy/fregex/
+-rw-rw-rw-   0        0        0       24 2023-09-12 12:27:01.000000 payconpy-2.2.3/payconpy/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10366 2024-03-28 17:52:21.000000 payconpy-2.2.3/payconpy/fregex/fregex.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:31.536788 payconpy-2.2.3/payconpy/fselenium/
+-rw-rw-rw-   0        0        0       27 2023-09-12 12:27:01.000000 payconpy-2.2.3/payconpy/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    40190 2024-03-28 20:51:18.000000 payconpy-2.2.3/payconpy/fselenium/fselenium.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:31.554424 payconpy-2.2.3/payconpy/odoo/
+-rw-rw-rw-   0        0        0        0 2024-04-21 19:01:38.000000 payconpy-2.2.3/payconpy/odoo/__init__.py
+-rw-rw-rw-   0        0        0    11717 2024-05-13 20:36:27.000000 payconpy-2.2.3/payconpy/odoo/odoo_xmlrpc.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:31.576835 payconpy-2.2.3/payconpy/openai/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.3/payconpy/openai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:31.589104 payconpy-2.2.3/payconpy/openai/apis/
+-rw-rw-rw-   0        0        0        0 2024-04-21 21:37:31.000000 payconpy-2.2.3/payconpy/openai/apis/__init__.py
+-rw-rw-rw-   0        0        0     3192 2024-04-21 21:37:47.000000 payconpy-2.2.3/payconpy/openai/apis/apis.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:31.605959 payconpy-2.2.3/payconpy/openai/assistants/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.3/payconpy/openai/assistants/__init__.py
+-rw-rw-rw-   0        0        0     4085 2023-11-27 13:03:14.000000 payconpy-2.2.3/payconpy/openai/assistants/assistants.py
+-rw-rw-rw-   0        0        0     4427 2023-11-27 14:53:41.000000 payconpy-2.2.3/payconpy/openai/get_cost.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:31.625549 payconpy-2.2.3/payconpy/utils/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.3/payconpy/utils/__init__.py
+-rw-rw-rw-   0        0        0   195592 2024-05-21 14:36:04.000000 payconpy-2.2.3/payconpy/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:17:31.378201 payconpy-2.2.3/payconpy.egg-info/
+-rw-rw-rw-   0        0        0      920 2024-05-21 15:17:30.000000 payconpy-2.2.3/payconpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1013 2024-05-21 15:17:31.000000 payconpy-2.2.3/payconpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 15:17:30.000000 payconpy-2.2.3/payconpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      181 2024-05-21 15:17:30.000000 payconpy-2.2.3/payconpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      261 2024-05-21 15:17:30.000000 payconpy-2.2.3/payconpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 15:17:31.643704 payconpy-2.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     2093 2024-05-21 15:17:24.000000 payconpy-2.2.3/setup.py
```

### Comparing `payconpy-2.2.2/LICENSE` & `payconpy-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.2/PKG-INFO` & `payconpy-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payconpy
-Version: 2.2.2
+Version: 2.2.3
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/payconpy
 Author: Paycon Automações
 Author-email: fernanda.yamamoto@paycon.com.br
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `payconpy-2.2.2/payconpy/femails/femails.py` & `payconpy-2.2.3/payconpy/femails/femails.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.2/payconpy/fexceptions/exceptions.py` & `payconpy-2.2.3/payconpy/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.2/payconpy/fpdf/focr/orc.py` & `payconpy-2.2.3/payconpy/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.2/payconpy/fpdf/pdfutils/pdfutils.py` & `payconpy-2.2.3/payconpy/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.2/payconpy/fpysimplegui/fpysimplegui.py` & `payconpy-2.2.3/payconpy/fpysimplegui/fpysimplegui.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.2/payconpy/fpython/fpython.py` & `payconpy-2.2.3/payconpy/fpython/fpython.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from configparser import RawConfigParser
 from datetime import datetime, date, timedelta
 from fnmatch import fnmatch
 from time import sleep
 import subprocess as sp
 import zipfile
 from rich import print
+from rich.console import Console
 from numpy import unicode_
 ################################## IMPORTS #############################################
 
 def generate_uuid() -> str:
     """Generate uuid
 
     Returns:
```

### Comparing `payconpy-2.2.2/payconpy/fregex/fregex.py` & `payconpy-2.2.3/payconpy/fregex/fregex.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.2/payconpy/fselenium/fselenium.py` & `payconpy-2.2.3/payconpy/fselenium/fselenium.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.2/payconpy/odoo/odoo_xmlrpc.py` & `payconpy-2.2.3/payconpy/odoo/odoo_xmlrpc.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.2/payconpy/openai/apis/apis.py` & `payconpy-2.2.3/payconpy/openai/apis/apis.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.2/payconpy/openai/assistants/assistants.py` & `payconpy-2.2.3/payconpy/openai/assistants/assistants.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.2/payconpy/openai/get_cost.py` & `payconpy-2.2.3/payconpy/openai/get_cost.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.2/payconpy/utils/utils.py` & `payconpy-2.2.3/payconpy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.2/payconpy.egg-info/PKG-INFO` & `payconpy-2.2.3/payconpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payconpy
-Version: 2.2.2
+Version: 2.2.3
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/payconpy
 Author: Paycon Automações
 Author-email: fernanda.yamamoto@paycon.com.br
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `payconpy-2.2.2/payconpy.egg-info/SOURCES.txt` & `payconpy-2.2.3/payconpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.2/setup.py` & `payconpy-2.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '2.2.2'
+version = '2.2.3'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='payconpy',
         version=version,
         url='https://github.com/githubpaycon/payconpy',
```

