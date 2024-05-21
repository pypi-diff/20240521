# Comparing `tmp/manager_cw_bot_api-1.1.1.tar.gz` & `tmp/manager_cw_bot_api-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manager_cw_bot_api-1.1.1.tar", last modified: Tue May 21 20:18:51 2024, max compression
+gzip compressed data, was "manager_cw_bot_api-1.5.0.tar", last modified: Tue May 21 19:16:46 2024, max compression
```

## Comparing `manager_cw_bot_api-1.1.1.tar` & `manager_cw_bot_api-1.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 20:18:51.544115 manager_cw_bot_api-1.1.1/
--rw-rw-rw-   0        0        0     1380 2024-05-21 20:18:51.542113 manager_cw_bot_api-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-21 20:18:51.464910 manager_cw_bot_api-1.1.1/manager_cw_bot_api/
--rw-rw-rw-   0        0        0      571 2024-05-21 18:56:04.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api/__init__.py
--rw-rw-rw-   0        0        0     2276 2024-05-21 20:16:51.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api/analytics.py
--rw-rw-rw-   0        0        0    34869 2024-05-21 20:16:51.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api/business.py
--rw-rw-rw-   0        0        0    30193 2024-05-21 20:16:51.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api/business_handler.py
--rw-rw-rw-   0        0        0    13801 2024-05-19 09:53:59.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api/buttons.py
--rw-rw-rw-   0        0        0     1442 2024-05-21 18:04:37.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api/create_table.py
--rw-rw-rw-   0        0        0      496 2024-05-21 19:13:38.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api/get_business_conn_and_info_conn.py
--rw-rw-rw-   0        0        0     7039 2024-05-16 13:51:37.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api/giga_request.py
--rw-rw-rw-   0        0        0     7145 2024-05-21 18:11:22.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api/gigachatai.py
--rw-rw-rw-   0        0        0      204 2024-05-21 20:16:51.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api/main.py
--rw-rw-rw-   0        0        0     1222 2024-05-19 13:43:08.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api/mysql_connection.py
--rw-rw-rw-   0        0        0     1212 2024-05-21 20:16:51.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api/tests.py
--rw-rw-rw-   0        0        0     9081 2024-05-21 20:16:51.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api/tickets.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:18:51.539111 manager_cw_bot_api-1.1.1/manager_cw_bot_api.egg-info/
--rw-rw-rw-   0        0        0     1380 2024-05-21 20:18:51.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      671 2024-05-21 20:18:51.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 20:18:51.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-21 20:18:51.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-21 20:18:51.000000 manager_cw_bot_api-1.1.1/manager_cw_bot_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 20:18:51.548110 manager_cw_bot_api-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1888 2024-05-21 20:18:22.000000 manager_cw_bot_api-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:16:46.433796 manager_cw_bot_api-1.5.0/
+-rw-rw-rw-   0        0        0     1380 2024-05-21 19:16:46.430800 manager_cw_bot_api-1.5.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-21 19:16:46.385828 manager_cw_bot_api-1.5.0/manager_cw_bot_api/
+-rw-rw-rw-   0        0        0      571 2024-05-21 18:56:04.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api/__init__.py
+-rw-rw-rw-   0        0        0     2278 2024-05-21 17:56:28.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api/analytics.py
+-rw-rw-rw-   0        0        0    34876 2024-05-21 18:04:37.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api/business.py
+-rw-rw-rw-   0        0        0    30194 2024-05-21 18:15:44.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api/business_handler.py
+-rw-rw-rw-   0        0        0    13801 2024-05-19 09:53:59.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api/buttons.py
+-rw-rw-rw-   0        0        0     1442 2024-05-21 18:04:37.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api/create_table.py
+-rw-rw-rw-   0        0        0      496 2024-05-21 19:13:38.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api/get_business_conn_and_info_conn.py
+-rw-rw-rw-   0        0        0     7039 2024-05-16 13:51:37.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api/giga_request.py
+-rw-rw-rw-   0        0        0     7145 2024-05-21 18:11:22.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api/gigachatai.py
+-rw-rw-rw-   0        0        0      205 2024-05-21 18:11:22.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api/main.py
+-rw-rw-rw-   0        0        0     1222 2024-05-19 13:43:08.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api/mysql_connection.py
+-rw-rw-rw-   0        0        0     1213 2024-05-21 19:12:48.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api/tests.py
+-rw-rw-rw-   0        0        0     9083 2024-05-21 18:15:07.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api/tickets.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:16:46.427799 manager_cw_bot_api-1.5.0/manager_cw_bot_api.egg-info/
+-rw-rw-rw-   0        0        0     1380 2024-05-21 19:16:46.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      671 2024-05-21 19:16:46.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 19:16:46.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-21 19:16:46.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-21 19:16:46.000000 manager_cw_bot_api-1.5.0/manager_cw_bot_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 19:16:46.437793 manager_cw_bot_api-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1888 2024-05-21 19:14:53.000000 manager_cw_bot_api-1.5.0/setup.py
```

### Comparing `manager_cw_bot_api-1.1.1/PKG-INFO` & `manager_cw_bot_api-1.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manager_cw_bot_api
-Version: 1.1.1
+Version: 1.5.0
 Summary: Python module for Business users in Telegram (For admin - business-person; Manager CW Bot API). Docs: https://docs.cwr.su/
 Home-page: https://github.com/cwr-su/manager_cw_bot_api
 Download-URL: https://github.com/cwr-su/manager_cw_bot_api/archive/refs/heads/main.zip
 Author: Alexander Laptev, CW
 Author-email: cwr@cwr.su
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `manager_cw_bot_api-1.1.1/manager_cw_bot_api/__init__.py` & `manager_cw_bot_api-1.5.0/manager_cw_bot_api/__init__.py`

 * *Files identical despite different names*

### Comparing `manager_cw_bot_api-1.1.1/manager_cw_bot_api/analytics.py` & `manager_cw_bot_api-1.5.0/manager_cw_bot_api/analytics.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 """
 import datetime
 
 import telebot
 from telebot import types
 import pymysql
 
-from buttons import Buttons
-from mysql_connection import Connection
+from .buttons import Buttons
+from .mysql_connection import Connection
 
 
 class Analytic:
     """
     Analytic Class.
     """
     def __init__(self, bot: telebot.TeleBot, mysql_data: dict,
```

### Comparing `manager_cw_bot_api-1.1.1/manager_cw_bot_api/business.py` & `manager_cw_bot_api-1.5.0/manager_cw_bot_api/business.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 import datetime
 import json
 
 import telebot
 from telebot import types
 import pymysql
 
-from buttons import Buttons
-from create_table import CreateTable
-from tickets import (TicketUserView, TicketAdminView)
-from gigachatai import GigaChatAI
-from analytics import Analytic
-from business_handler import (BusinessHandler, Thanks, Congratulation, ProblemWithBot)
-from mysql_connection import Connection
+from .buttons import Buttons
+from .create_table import CreateTable
+from .tickets import (TicketUserView, TicketAdminView)
+from .gigachatai import GigaChatAI
+from .analytics import Analytic
+from .business_handler import (BusinessHandler, Thanks, Congratulation, ProblemWithBot)
+from .mysql_connection import Connection
 
 
 class Manager(telebot.TeleBot):
     """
     Manager of the Alex's Account and helper 'AI'.
     """
     def __init__(self, bot_token: str, business_conn_id: str, admin_id: int,
```

### Comparing `manager_cw_bot_api-1.1.1/manager_cw_bot_api/business_handler.py` & `manager_cw_bot_api-1.5.0/manager_cw_bot_api/business_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Module of the business handler.
 """
 import telebot
 import json
 from telebot import types
 
-from buttons import Buttons
+from .buttons import Buttons
 
 
 class BusinessHandler:
     """
     Class of the business handler for admin.
     """
     message: types.Message = None
```

### Comparing `manager_cw_bot_api-1.1.1/manager_cw_bot_api/buttons.py` & `manager_cw_bot_api-1.5.0/manager_cw_bot_api/buttons.py`

 * *Files identical despite different names*

### Comparing `manager_cw_bot_api-1.1.1/manager_cw_bot_api/create_table.py` & `manager_cw_bot_api-1.5.0/manager_cw_bot_api/create_table.py`

 * *Files identical despite different names*

### Comparing `manager_cw_bot_api-1.1.1/manager_cw_bot_api/giga_request.py` & `manager_cw_bot_api-1.5.0/manager_cw_bot_api/giga_request.py`

 * *Files identical despite different names*

### Comparing `manager_cw_bot_api-1.1.1/manager_cw_bot_api/gigachatai.py` & `manager_cw_bot_api-1.5.0/manager_cw_bot_api/gigachatai.py`

 * *Files identical despite different names*

### Comparing `manager_cw_bot_api-1.1.1/manager_cw_bot_api/mysql_connection.py` & `manager_cw_bot_api-1.5.0/manager_cw_bot_api/mysql_connection.py`

 * *Files identical despite different names*

### Comparing `manager_cw_bot_api-1.1.1/manager_cw_bot_api/tests.py` & `manager_cw_bot_api-1.5.0/manager_cw_bot_api/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from get_business_conn_and_info_conn import gets
+from .get_business_conn_and_info_conn import gets
 
 
 class Test(unittest.TestCase):
     """
     Class for the unit tests.
     """
     def testGetBusinessConn(self) -> None:
```

### Comparing `manager_cw_bot_api-1.1.1/manager_cw_bot_api/tickets.py` & `manager_cw_bot_api-1.5.0/manager_cw_bot_api/tickets.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import random
 import string
 
 import pymysql
 import telebot
 from telebot import types
 
-from buttons import Buttons
-from mysql_connection import Connection
+from .buttons import Buttons
+from .mysql_connection import Connection
 
 
 class TicketUserView:
     """
     Class of the ticket system UI for users.
     """
```

### Comparing `manager_cw_bot_api-1.1.1/manager_cw_bot_api.egg-info/PKG-INFO` & `manager_cw_bot_api-1.5.0/manager_cw_bot_api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manager_cw_bot_api
-Version: 1.1.1
+Version: 1.5.0
 Summary: Python module for Business users in Telegram (For admin - business-person; Manager CW Bot API). Docs: https://docs.cwr.su/
 Home-page: https://github.com/cwr-su/manager_cw_bot_api
 Download-URL: https://github.com/cwr-su/manager_cw_bot_api/archive/refs/heads/main.zip
 Author: Alexander Laptev, CW
 Author-email: cwr@cwr.su
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `manager_cw_bot_api-1.1.1/manager_cw_bot_api.egg-info/SOURCES.txt` & `manager_cw_bot_api-1.5.0/manager_cw_bot_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manager_cw_bot_api-1.1.1/setup.py` & `manager_cw_bot_api-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """
 :authors: Alexander Laptev, CW
 :license: Apache License, Version 2.0, see LICENSE file
 :copyright: (c) 2024 Alexander Laptev, CW
 """
 
-version = "1.1.1"
+version = "1.5.0"
 '''
 with open('', encoding='utf-8') as file:
     long_description = file.read()
 '''
 
 long_description = '''Python module for Business users in Telegram 
                    (For admin - business-person; Manager CW Bot API).
```

