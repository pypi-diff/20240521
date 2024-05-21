# Comparing `tmp/payconpy-2.2.0.tar.gz` & `tmp/payconpy-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payconpy-2.2.0.tar", last modified: Tue May 21 14:28:39 2024, max compression
+gzip compressed data, was "payconpy-2.2.1.tar", last modified: Tue May 21 14:36:22 2024, max compression
```

## Comparing `payconpy-2.2.0.tar` & `payconpy-2.2.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 14:28:39.001614 payconpy-2.2.0/
--rw-rw-rw-   0        0        0     1073 2024-03-28 18:34:30.000000 payconpy-2.2.0/LICENSE
--rw-rw-rw-   0        0        0      920 2024-05-21 14:28:38.997311 payconpy-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      456 2024-04-21 22:27:53.000000 payconpy-2.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.566334 payconpy-2.2.0/payconpy/
-drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.697411 payconpy-2.2.0/payconpy/femails/
--rw-rw-rw-   0        0        0       40 2024-03-28 18:29:40.000000 payconpy-2.2.0/payconpy/femails/__init__.py
--rw-rw-rw-   0        0        0     7021 2024-03-28 18:29:45.000000 payconpy-2.2.0/payconpy/femails/femails.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.733703 payconpy-2.2.0/payconpy/fexceptions/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.0/payconpy/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2023-09-12 12:27:01.000000 payconpy-2.2.0/payconpy/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.745331 payconpy-2.2.0/payconpy/fpdf/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.0/payconpy/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.758402 payconpy-2.2.0/payconpy/fpdf/focr/
--rw-rw-rw-   0        0        0      104 2024-03-28 18:29:53.000000 payconpy-2.2.0/payconpy/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0    10766 2024-05-21 14:26:58.000000 payconpy-2.2.0/payconpy/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.773180 payconpy-2.2.0/payconpy/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.0/payconpy/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     5758 2024-04-21 19:13:23.000000 payconpy-2.2.0/payconpy/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.803471 payconpy-2.2.0/payconpy/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2023-09-12 12:27:01.000000 payconpy-2.2.0/payconpy/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4676 2024-03-28 17:58:49.000000 payconpy-2.2.0/payconpy/fpysimplegui/fpysimplegui.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.835330 payconpy-2.2.0/payconpy/fpython/
--rw-rw-rw-   0        0        0       25 2023-09-12 12:27:01.000000 payconpy-2.2.0/payconpy/fpython/__init__.py
--rw-rw-rw-   0        0        0    57479 2024-04-21 19:22:58.000000 payconpy-2.2.0/payconpy/fpython/fpython.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.857219 payconpy-2.2.0/payconpy/fregex/
--rw-rw-rw-   0        0        0       24 2023-09-12 12:27:01.000000 payconpy-2.2.0/payconpy/fregex/__init__.py
--rw-rw-rw-   0        0        0    10366 2024-03-28 17:52:21.000000 payconpy-2.2.0/payconpy/fregex/fregex.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.883751 payconpy-2.2.0/payconpy/fselenium/
--rw-rw-rw-   0        0        0       27 2023-09-12 12:27:01.000000 payconpy-2.2.0/payconpy/fselenium/__init__.py
--rw-rw-rw-   0        0        0    40190 2024-03-28 20:51:18.000000 payconpy-2.2.0/payconpy/fselenium/fselenium.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.900819 payconpy-2.2.0/payconpy/odoo/
--rw-rw-rw-   0        0        0        0 2024-04-21 19:01:38.000000 payconpy-2.2.0/payconpy/odoo/__init__.py
--rw-rw-rw-   0        0        0    11717 2024-05-13 20:36:27.000000 payconpy-2.2.0/payconpy/odoo/odoo_xmlrpc.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.928147 payconpy-2.2.0/payconpy/openai/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.0/payconpy/openai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.942894 payconpy-2.2.0/payconpy/openai/apis/
--rw-rw-rw-   0        0        0        0 2024-04-21 21:37:31.000000 payconpy-2.2.0/payconpy/openai/apis/__init__.py
--rw-rw-rw-   0        0        0     3192 2024-04-21 21:37:47.000000 payconpy-2.2.0/payconpy/openai/apis/apis.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.966015 payconpy-2.2.0/payconpy/openai/assistants/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.0/payconpy/openai/assistants/__init__.py
--rw-rw-rw-   0        0        0     4085 2023-11-27 13:03:14.000000 payconpy-2.2.0/payconpy/openai/assistants/assistants.py
--rw-rw-rw-   0        0        0     4427 2023-11-27 14:53:41.000000 payconpy-2.2.0/payconpy/openai/get_cost.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.986075 payconpy-2.2.0/payconpy/utils/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.0/payconpy/utils/__init__.py
--rw-rw-rw-   0        0        0   147726 2024-04-22 17:45:30.000000 payconpy-2.2.0/payconpy/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.680312 payconpy-2.2.0/payconpy.egg-info/
--rw-rw-rw-   0        0        0      920 2024-05-21 14:28:37.000000 payconpy-2.2.0/payconpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1013 2024-05-21 14:28:37.000000 payconpy-2.2.0/payconpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:28:37.000000 payconpy-2.2.0/payconpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      181 2024-05-21 14:28:37.000000 payconpy-2.2.0/payconpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0      261 2024-05-21 14:28:37.000000 payconpy-2.2.0/payconpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 14:28:39.001614 payconpy-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2093 2024-05-21 14:28:20.000000 payconpy-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.516488 payconpy-2.2.1/
+-rw-rw-rw-   0        0        0     1073 2024-03-28 18:34:30.000000 payconpy-2.2.1/LICENSE
+-rw-rw-rw-   0        0        0      920 2024-05-21 14:36:22.509534 payconpy-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2024-04-21 22:27:53.000000 payconpy-2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.224937 payconpy-2.2.1/payconpy/
+drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.294963 payconpy-2.2.1/payconpy/femails/
+-rw-rw-rw-   0        0        0       40 2024-03-28 18:29:40.000000 payconpy-2.2.1/payconpy/femails/__init__.py
+-rw-rw-rw-   0        0        0     7021 2024-03-28 18:29:45.000000 payconpy-2.2.1/payconpy/femails/femails.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.309196 payconpy-2.2.1/payconpy/fexceptions/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.1/payconpy/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-09-12 12:27:01.000000 payconpy-2.2.1/payconpy/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.316289 payconpy-2.2.1/payconpy/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.1/payconpy/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.332482 payconpy-2.2.1/payconpy/fpdf/focr/
+-rw-rw-rw-   0        0        0      104 2024-03-28 18:29:53.000000 payconpy-2.2.1/payconpy/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0    10766 2024-05-21 14:26:58.000000 payconpy-2.2.1/payconpy/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.361816 payconpy-2.2.1/payconpy/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.1/payconpy/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     5758 2024-04-21 19:13:23.000000 payconpy-2.2.1/payconpy/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.376094 payconpy-2.2.1/payconpy/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2023-09-12 12:27:01.000000 payconpy-2.2.1/payconpy/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4676 2024-03-28 17:58:49.000000 payconpy-2.2.1/payconpy/fpysimplegui/fpysimplegui.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.389529 payconpy-2.2.1/payconpy/fpython/
+-rw-rw-rw-   0        0        0       25 2023-09-12 12:27:01.000000 payconpy-2.2.1/payconpy/fpython/__init__.py
+-rw-rw-rw-   0        0        0    57479 2024-04-21 19:22:58.000000 payconpy-2.2.1/payconpy/fpython/fpython.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.407232 payconpy-2.2.1/payconpy/fregex/
+-rw-rw-rw-   0        0        0       24 2023-09-12 12:27:01.000000 payconpy-2.2.1/payconpy/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10366 2024-03-28 17:52:21.000000 payconpy-2.2.1/payconpy/fregex/fregex.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.420760 payconpy-2.2.1/payconpy/fselenium/
+-rw-rw-rw-   0        0        0       27 2023-09-12 12:27:01.000000 payconpy-2.2.1/payconpy/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    40190 2024-03-28 20:51:18.000000 payconpy-2.2.1/payconpy/fselenium/fselenium.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.433200 payconpy-2.2.1/payconpy/odoo/
+-rw-rw-rw-   0        0        0        0 2024-04-21 19:01:38.000000 payconpy-2.2.1/payconpy/odoo/__init__.py
+-rw-rw-rw-   0        0        0    11717 2024-05-13 20:36:27.000000 payconpy-2.2.1/payconpy/odoo/odoo_xmlrpc.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.450056 payconpy-2.2.1/payconpy/openai/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.1/payconpy/openai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.461006 payconpy-2.2.1/payconpy/openai/apis/
+-rw-rw-rw-   0        0        0        0 2024-04-21 21:37:31.000000 payconpy-2.2.1/payconpy/openai/apis/__init__.py
+-rw-rw-rw-   0        0        0     3192 2024-04-21 21:37:47.000000 payconpy-2.2.1/payconpy/openai/apis/apis.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.479353 payconpy-2.2.1/payconpy/openai/assistants/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.1/payconpy/openai/assistants/__init__.py
+-rw-rw-rw-   0        0        0     4085 2023-11-27 13:03:14.000000 payconpy-2.2.1/payconpy/openai/assistants/assistants.py
+-rw-rw-rw-   0        0        0     4427 2023-11-27 14:53:41.000000 payconpy-2.2.1/payconpy/openai/get_cost.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.496783 payconpy-2.2.1/payconpy/utils/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.1/payconpy/utils/__init__.py
+-rw-rw-rw-   0        0        0   195592 2024-05-21 14:36:04.000000 payconpy-2.2.1/payconpy/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.282790 payconpy-2.2.1/payconpy.egg-info/
+-rw-rw-rw-   0        0        0      920 2024-05-21 14:36:21.000000 payconpy-2.2.1/payconpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1013 2024-05-21 14:36:22.000000 payconpy-2.2.1/payconpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:36:21.000000 payconpy-2.2.1/payconpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      181 2024-05-21 14:36:21.000000 payconpy-2.2.1/payconpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      261 2024-05-21 14:36:21.000000 payconpy-2.2.1/payconpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:36:22.517513 payconpy-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2093 2024-05-21 14:36:12.000000 payconpy-2.2.1/setup.py
```

### Comparing `payconpy-2.2.0/LICENSE` & `payconpy-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.0/PKG-INFO` & `payconpy-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payconpy
-Version: 2.2.0
+Version: 2.2.1
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/payconpy
 Author: Paycon Automações
 Author-email: fernanda.yamamoto@paycon.com.br
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `payconpy-2.2.0/payconpy/femails/femails.py` & `payconpy-2.2.1/payconpy/femails/femails.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.0/payconpy/fexceptions/exceptions.py` & `payconpy-2.2.1/payconpy/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.0/payconpy/fpdf/focr/orc.py` & `payconpy-2.2.1/payconpy/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.0/payconpy/fpdf/pdfutils/pdfutils.py` & `payconpy-2.2.1/payconpy/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.0/payconpy/fpysimplegui/fpysimplegui.py` & `payconpy-2.2.1/payconpy/fpysimplegui/fpysimplegui.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.0/payconpy/fpython/fpython.py` & `payconpy-2.2.1/payconpy/fpython/fpython.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.0/payconpy/fregex/fregex.py` & `payconpy-2.2.1/payconpy/fregex/fregex.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.0/payconpy/fselenium/fselenium.py` & `payconpy-2.2.1/payconpy/fselenium/fselenium.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.0/payconpy/odoo/odoo_xmlrpc.py` & `payconpy-2.2.1/payconpy/odoo/odoo_xmlrpc.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.0/payconpy/openai/apis/apis.py` & `payconpy-2.2.1/payconpy/openai/apis/apis.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.0/payconpy/openai/assistants/assistants.py` & `payconpy-2.2.1/payconpy/openai/assistants/assistants.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.0/payconpy/openai/get_cost.py` & `payconpy-2.2.1/payconpy/openai/get_cost.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.0/payconpy.egg-info/PKG-INFO` & `payconpy-2.2.1/payconpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payconpy
-Version: 2.2.0
+Version: 2.2.1
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/payconpy
 Author: Paycon Automações
 Author-email: fernanda.yamamoto@paycon.com.br
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `payconpy-2.2.0/payconpy.egg-info/SOURCES.txt` & `payconpy-2.2.1/payconpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.0/setup.py` & `payconpy-2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '2.2.0'
+version = '2.2.1'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='payconpy',
         version=version,
         url='https://github.com/githubpaycon/payconpy',
```

