# Comparing `tmp/pih-msg_q-0.13.tar.gz` & `tmp/pih-msg_q-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-msg_q-0.13.tar", last modified: Mon May 13 01:54:43 2024, max compression
+gzip compressed data, was "pih-msg_q-0.14.tar", last modified: Mon May 20 23:04:03 2024, max compression
```

## Comparing `pih-msg_q-0.13.tar` & `pih-msg_q-0.14.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 01:54:43.248555 pih-msg_q-0.13/
-drwxrwxrwx   0        0        0        0 2024-05-13 01:54:42.478758 pih-msg_q-0.13/MessageQueueService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-msg_q-0.13/MessageQueueService/__init__.py
--rw-rw-rw-   0        0        0      156 2024-02-15 00:45:45.000000 pih-msg_q-0.13/MessageQueueService/__main__.py
--rw-rw-rw-   0        0        0      441 2024-05-13 01:54:20.000000 pih-msg_q-0.13/MessageQueueService/const.py
--rw-rw-rw-   0        0        0     3701 2024-05-08 06:43:07.000000 pih-msg_q-0.13/MessageQueueService/service.py
--rw-rw-rw-   0        0        0      275 2024-05-13 01:54:43.217303 pih-msg_q-0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 01:54:43.170426 pih-msg_q-0.13/pih_msg_q.egg-info/
--rw-rw-rw-   0        0        0      275 2024-05-13 01:54:41.000000 pih-msg_q-0.13/pih_msg_q.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-05-13 01:54:42.000000 pih-msg_q-0.13/pih_msg_q.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 01:54:42.000000 pih-msg_q-0.13/pih_msg_q.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-05-13 01:54:42.000000 pih-msg_q-0.13/pih_msg_q.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-13 01:54:42.000000 pih-msg_q-0.13/pih_msg_q.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-13 01:54:42.000000 pih-msg_q-0.13/pih_msg_q.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 01:54:43.264181 pih-msg_q-0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 23:04:03.264935 pih-msg_q-0.14/
+drwxrwxrwx   0        0        0        0 2024-05-20 23:04:02.780158 pih-msg_q-0.14/MessageQueueService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-msg_q-0.14/MessageQueueService/__init__.py
+-rw-rw-rw-   0        0        0      156 2024-02-15 00:45:45.000000 pih-msg_q-0.14/MessageQueueService/__main__.py
+-rw-rw-rw-   0        0        0      441 2024-05-20 22:38:29.000000 pih-msg_q-0.14/MessageQueueService/const.py
+-rw-rw-rw-   0        0        0     3702 2024-05-15 05:05:21.000000 pih-msg_q-0.14/MessageQueueService/service.py
+-rw-rw-rw-   0        0        0      275 2024-05-20 23:04:03.178562 pih-msg_q-0.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 23:04:03.084812 pih-msg_q-0.14/pih_msg_q.egg-info/
+-rw-rw-rw-   0        0        0      275 2024-05-20 23:04:02.000000 pih-msg_q-0.14/pih_msg_q.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-20 23:04:02.000000 pih-msg_q-0.14/pih_msg_q.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 23:04:02.000000 pih-msg_q-0.14/pih_msg_q.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-20 23:04:02.000000 pih-msg_q-0.14/pih_msg_q.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 23:04:02.000000 pih-msg_q-0.14/pih_msg_q.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-20 23:04:02.000000 pih-msg_q-0.14/pih_msg_q.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 23:04:03.311848 pih-msg_q-0.14/setup.cfg
```

### Comparing `pih-msg_q-0.13/MessageQueueService/service.py` & `pih-msg_q-0.14/MessageQueueService/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pih.collections import Message
 from MessageQueueService.const import SD
 from pih.tools import ParameterList, while_not_do, ne, js, nn, j
 
 
 SC = A.CT_SC
 
-ISOLATED: bool = True
+ISOLATED: bool = False
 
 from collections import defaultdict
 from time import sleep
 import random
 
 
 class DH:
```

