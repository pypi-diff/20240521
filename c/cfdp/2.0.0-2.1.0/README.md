# Comparing `tmp/cfdp-2.0.0.tar.gz` & `tmp/cfdp-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfdp-2.0.0.tar", last modified: Mon May 15 20:53:00 2023, max compression
+gzip compressed data, was "cfdp-2.1.0.tar", last modified: Tue May 21 20:33:49 2024, max compression
```

## Comparing `cfdp-2.0.0.tar` & `cfdp-2.1.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.016820 cfdp-2.0.0/
--rw-r--r--   0 artur     (1000) artur     (1000)     1066 2023-05-15 19:26:16.000000 cfdp-2.0.0/LICENSE.txt
--rw-r--r--   0 artur     (1000) artur     (1000)     2487 2023-05-15 20:53:00.016820 cfdp-2.0.0/PKG-INFO
--rw-r--r--   0 artur     (1000) artur     (1000)     2276 2023-05-15 19:26:16.000000 cfdp-2.0.0/README.md
--rw-r--r--   0 artur     (1000) artur     (1000)      261 2023-05-15 20:52:42.000000 cfdp-2.0.0/pyproject.toml
--rw-r--r--   0 artur     (1000) artur     (1000)       38 2023-05-15 20:53:00.016820 cfdp-2.0.0/setup.cfg
-drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.010153 cfdp-2.0.0/src/
-drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.010153 cfdp-2.0.0/src/cfdp/
--rw-r--r--   0 artur     (1000) artur     (1000)      185 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/__init__.py
--rw-r--r--   0 artur     (1000) artur     (1000)     3533 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/constants.py
--rw-r--r--   0 artur     (1000) artur     (1000)    19844 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/core.py
--rw-r--r--   0 artur     (1000) artur     (1000)     1438 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/event.py
-drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.013487 cfdp-2.0.0/src/cfdp/filestore/
--rw-r--r--   0 artur     (1000) artur     (1000)       71 2023-03-14 21:54:24.000000 cfdp-2.0.0/src/cfdp/filestore/__init__.py
--rw-r--r--   0 artur     (1000) artur     (1000)     1184 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/filestore/base.py
--rw-r--r--   0 artur     (1000) artur     (1000)     5551 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/filestore/native.py
-drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.013487 cfdp-2.0.0/src/cfdp/machines/
--rw-r--r--   0 artur     (1000) artur     (1000)      124 2023-03-14 21:54:24.000000 cfdp-2.0.0/src/cfdp/machines/__init__.py
--rw-r--r--   0 artur     (1000) artur     (1000)    10633 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/machines/base.py
--rw-r--r--   0 artur     (1000) artur     (1000)     5695 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/machines/receiver1.py
--rw-r--r--   0 artur     (1000) artur     (1000)    21150 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/machines/receiver2.py
--rw-r--r--   0 artur     (1000) artur     (1000)     6383 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/machines/sender1.py
--rw-r--r--   0 artur     (1000) artur     (1000)    17933 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/machines/sender2.py
--rw-r--r--   0 artur     (1000) artur     (1000)     1278 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/machines/timer.py
-drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.013487 cfdp-2.0.0/src/cfdp/meta/
--rw-r--r--   0 artur     (1000) artur     (1000)       73 2023-03-14 21:54:24.000000 cfdp-2.0.0/src/cfdp/meta/__init__.py
--rw-r--r--   0 artur     (1000) artur     (1000)      279 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/meta/datafield.py
--rw-r--r--   0 artur     (1000) artur     (1000)     5339 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/meta/filestore.py
--rw-r--r--   0 artur     (1000) artur     (1000)    21597 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/meta/message.py
-drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.013487 cfdp-2.0.0/src/cfdp/pdu/
--rw-r--r--   0 artur     (1000) artur     (1000)      177 2023-03-14 21:54:24.000000 cfdp-2.0.0/src/cfdp/pdu/__init__.py
--rw-r--r--   0 artur     (1000) artur     (1000)     3329 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/ack.py
--rw-r--r--   0 artur     (1000) artur     (1000)     4258 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/eof.py
--rw-r--r--   0 artur     (1000) artur     (1000)     3278 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/filedata.py
--rw-r--r--   0 artur     (1000) artur     (1000)     3574 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/finished.py
--rw-r--r--   0 artur     (1000) artur     (1000)     5151 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/header.py
--rw-r--r--   0 artur     (1000) artur     (1000)     3681 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/keep_alive.py
--rw-r--r--   0 artur     (1000) artur     (1000)     7088 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/metadata.py
--rw-r--r--   0 artur     (1000) artur     (1000)     8221 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/nak.py
--rw-r--r--   0 artur     (1000) artur     (1000)     2750 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/pdu/prompt.py
--rw-r--r--   0 artur     (1000) artur     (1000)     3380 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/transaction.py
-drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.013487 cfdp-2.0.0/src/cfdp/transport/
--rw-r--r--   0 artur     (1000) artur     (1000)        0 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/transport/__init__.py
--rw-r--r--   0 artur     (1000) artur     (1000)      532 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/transport/base.py
--rw-r--r--   0 artur     (1000) artur     (1000)     1241 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/transport/spp.py
--rw-r--r--   0 artur     (1000) artur     (1000)     1995 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/transport/udp.py
--rw-r--r--   0 artur     (1000) artur     (1000)     1488 2023-05-15 19:26:16.000000 cfdp-2.0.0/src/cfdp/transport/zmq.py
-drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.010153 cfdp-2.0.0/src/cfdp.egg-info/
--rw-r--r--   0 artur     (1000) artur     (1000)     2487 2023-05-15 20:53:00.000000 cfdp-2.0.0/src/cfdp.egg-info/PKG-INFO
--rw-r--r--   0 artur     (1000) artur     (1000)     1162 2023-05-15 20:53:00.000000 cfdp-2.0.0/src/cfdp.egg-info/SOURCES.txt
--rw-r--r--   0 artur     (1000) artur     (1000)        1 2023-05-15 20:53:00.000000 cfdp-2.0.0/src/cfdp.egg-info/dependency_links.txt
--rw-r--r--   0 artur     (1000) artur     (1000)        5 2023-05-15 20:53:00.000000 cfdp-2.0.0/src/cfdp.egg-info/top_level.txt
-drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2023-05-15 20:53:00.016820 cfdp-2.0.0/tests/
--rw-r--r--   0 artur     (1000) artur     (1000)    23479 2023-05-15 19:26:16.000000 cfdp-2.0.0/tests/test_series_F1.py
--rw-r--r--   0 artur     (1000) artur     (1000)    26767 2023-05-15 19:26:16.000000 cfdp-2.0.0/tests/test_series_F2.py
--rw-r--r--   0 artur     (1000) artur     (1000)    20780 2023-05-15 19:26:16.000000 cfdp-2.0.0/tests/test_series_F3.py
--rw-r--r--   0 artur     (1000) artur     (1000)    12808 2023-05-15 19:26:16.000000 cfdp-2.0.0/tests/test_series_F4.py
--rw-r--r--   0 artur     (1000) artur     (1000)     1328 2023-05-15 19:26:16.000000 cfdp-2.0.0/tests/test_spp.py
--rw-r--r--   0 artur     (1000) artur     (1000)     1984 2023-05-15 19:26:16.000000 cfdp-2.0.0/tests/test_zmq.py
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2024-05-21 20:33:49.538093 cfdp-2.1.0/
+-rw-r--r--   0 artur     (1000) artur     (1000)     1066 2023-05-15 19:26:16.000000 cfdp-2.1.0/LICENSE.txt
+-rw-r--r--   0 artur     (1000) artur     (1000)     2487 2024-05-21 20:33:49.538093 cfdp-2.1.0/PKG-INFO
+-rw-r--r--   0 artur     (1000) artur     (1000)     2276 2023-05-15 19:26:16.000000 cfdp-2.1.0/README.md
+-rw-r--r--   0 artur     (1000) artur     (1000)      261 2024-05-21 20:06:26.000000 cfdp-2.1.0/pyproject.toml
+-rw-r--r--   0 artur     (1000) artur     (1000)       38 2024-05-21 20:33:49.538093 cfdp-2.1.0/setup.cfg
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2024-05-21 20:33:49.524759 cfdp-2.1.0/src/
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2024-05-21 20:33:49.528093 cfdp-2.1.0/src/cfdp/
+-rw-r--r--   0 artur     (1000) artur     (1000)      185 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/__init__.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     3533 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/constants.py
+-rw-r--r--   0 artur     (1000) artur     (1000)    19844 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/core.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     1438 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/event.py
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2024-05-21 20:33:49.528093 cfdp-2.1.0/src/cfdp/filestore/
+-rw-r--r--   0 artur     (1000) artur     (1000)       71 2023-03-14 21:54:24.000000 cfdp-2.1.0/src/cfdp/filestore/__init__.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     1184 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/filestore/base.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     5551 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/filestore/native.py
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2024-05-21 20:33:49.528093 cfdp-2.1.0/src/cfdp/machines/
+-rw-r--r--   0 artur     (1000) artur     (1000)      124 2023-03-14 21:54:24.000000 cfdp-2.1.0/src/cfdp/machines/__init__.py
+-rw-r--r--   0 artur     (1000) artur     (1000)    10633 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/machines/base.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     5695 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/machines/receiver1.py
+-rw-r--r--   0 artur     (1000) artur     (1000)    21150 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/machines/receiver2.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     6383 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/machines/sender1.py
+-rw-r--r--   0 artur     (1000) artur     (1000)    17933 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/machines/sender2.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     1278 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/machines/timer.py
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2024-05-21 20:33:49.528093 cfdp-2.1.0/src/cfdp/meta/
+-rw-r--r--   0 artur     (1000) artur     (1000)       73 2023-03-14 21:54:24.000000 cfdp-2.1.0/src/cfdp/meta/__init__.py
+-rw-r--r--   0 artur     (1000) artur     (1000)      279 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/meta/datafield.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     5339 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/meta/filestore.py
+-rw-r--r--   0 artur     (1000) artur     (1000)    21597 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/meta/message.py
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2024-05-21 20:33:49.534759 cfdp-2.1.0/src/cfdp/pdu/
+-rw-r--r--   0 artur     (1000) artur     (1000)      177 2023-03-14 21:54:24.000000 cfdp-2.1.0/src/cfdp/pdu/__init__.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     3329 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/pdu/ack.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     4258 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/pdu/eof.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     3278 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/pdu/filedata.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     3574 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/pdu/finished.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     5151 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/pdu/header.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     3681 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/pdu/keep_alive.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     7088 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/pdu/metadata.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     8221 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/pdu/nak.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     2750 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/pdu/prompt.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     3380 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/transaction.py
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2024-05-21 20:33:49.534759 cfdp-2.1.0/src/cfdp/transport/
+-rw-r--r--   0 artur     (1000) artur     (1000)        0 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/transport/__init__.py
+-rw-r--r--   0 artur     (1000) artur     (1000)      532 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/transport/base.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     1304 2024-05-21 20:00:42.000000 cfdp-2.1.0/src/cfdp/transport/spacepacket.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     1995 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/transport/udp.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     1488 2023-05-15 19:26:16.000000 cfdp-2.1.0/src/cfdp/transport/zmq.py
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2024-05-21 20:33:49.534759 cfdp-2.1.0/src/cfdp.egg-info/
+-rw-r--r--   0 artur     (1000) artur     (1000)     2487 2024-05-21 20:33:49.000000 cfdp-2.1.0/src/cfdp.egg-info/PKG-INFO
+-rw-r--r--   0 artur     (1000) artur     (1000)     1178 2024-05-21 20:33:49.000000 cfdp-2.1.0/src/cfdp.egg-info/SOURCES.txt
+-rw-r--r--   0 artur     (1000) artur     (1000)        1 2024-05-21 20:33:49.000000 cfdp-2.1.0/src/cfdp.egg-info/dependency_links.txt
+-rw-r--r--   0 artur     (1000) artur     (1000)        5 2024-05-21 20:33:49.000000 cfdp-2.1.0/src/cfdp.egg-info/top_level.txt
+drwxr-xr-x   0 artur     (1000) artur     (1000)        0 2024-05-21 20:33:49.534759 cfdp-2.1.0/tests/
+-rw-r--r--   0 artur     (1000) artur     (1000)    23479 2023-05-15 19:26:16.000000 cfdp-2.1.0/tests/test_series_F1.py
+-rw-r--r--   0 artur     (1000) artur     (1000)    26767 2023-05-15 19:26:16.000000 cfdp-2.1.0/tests/test_series_F2.py
+-rw-r--r--   0 artur     (1000) artur     (1000)    20780 2023-05-15 19:26:16.000000 cfdp-2.1.0/tests/test_series_F3.py
+-rw-r--r--   0 artur     (1000) artur     (1000)    12808 2023-05-15 19:26:16.000000 cfdp-2.1.0/tests/test_series_F4.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     1459 2024-05-21 20:26:43.000000 cfdp-2.1.0/tests/test_spacepacket.py
+-rw-r--r--   0 artur     (1000) artur     (1000)     1984 2023-05-15 19:26:16.000000 cfdp-2.1.0/tests/test_zmq.py
```

### Comparing `cfdp-2.0.0/LICENSE.txt` & `cfdp-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/PKG-INFO` & `cfdp-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfdp
-Version: 2.0.0
+Version: 2.1.0
 Summary: CCSDS File Delivery Protocol
 Author-email: LibreCube <info@librecube.org>
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Python CFDP
```

### Comparing `cfdp-2.0.0/README.md` & `cfdp-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/constants.py` & `cfdp-2.1.0/src/cfdp/constants.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/core.py` & `cfdp-2.1.0/src/cfdp/core.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/event.py` & `cfdp-2.1.0/src/cfdp/event.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/filestore/base.py` & `cfdp-2.1.0/src/cfdp/filestore/base.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/filestore/native.py` & `cfdp-2.1.0/src/cfdp/filestore/native.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/machines/base.py` & `cfdp-2.1.0/src/cfdp/machines/base.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/machines/receiver1.py` & `cfdp-2.1.0/src/cfdp/machines/receiver1.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/machines/receiver2.py` & `cfdp-2.1.0/src/cfdp/machines/receiver2.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/machines/sender1.py` & `cfdp-2.1.0/src/cfdp/machines/sender1.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/machines/sender2.py` & `cfdp-2.1.0/src/cfdp/machines/sender2.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/machines/timer.py` & `cfdp-2.1.0/src/cfdp/machines/timer.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/meta/filestore.py` & `cfdp-2.1.0/src/cfdp/meta/filestore.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/meta/message.py` & `cfdp-2.1.0/src/cfdp/meta/message.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/pdu/ack.py` & `cfdp-2.1.0/src/cfdp/pdu/ack.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/pdu/eof.py` & `cfdp-2.1.0/src/cfdp/pdu/eof.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/pdu/filedata.py` & `cfdp-2.1.0/src/cfdp/pdu/filedata.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/pdu/finished.py` & `cfdp-2.1.0/src/cfdp/pdu/finished.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/pdu/header.py` & `cfdp-2.1.0/src/cfdp/pdu/header.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/pdu/keep_alive.py` & `cfdp-2.1.0/src/cfdp/pdu/keep_alive.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/pdu/metadata.py` & `cfdp-2.1.0/src/cfdp/pdu/metadata.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/pdu/nak.py` & `cfdp-2.1.0/src/cfdp/pdu/nak.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/pdu/prompt.py` & `cfdp-2.1.0/src/cfdp/pdu/prompt.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/transaction.py` & `cfdp-2.1.0/src/cfdp/transaction.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/transport/base.py` & `cfdp-2.1.0/src/cfdp/transport/base.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/transport/spp.py` & `cfdp-2.1.0/src/cfdp/transport/spacepacket.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import spp
+from spacepacket import SpacePacketProtocolEntity, SpacePacket, SequenceFlags
 
 from .base import Transport
 
 
-class SppTransport(Transport):
+class SpacePacketTransport(Transport):
     """Space Packet Protocol Transport for CFDP PDUs.
 
     This transport protocol needs another transport protocol below it.
     """
 
     def __init__(self, apid, transport, packet_type):
         super().__init__()
         self.apid = apid
         self.transport = transport
         self.packet_type = packet_type
-        self.spp_entity = spp.SpacePacketProtocolEntity(apid=apid, transport=transport)
+        self.spp_entity = SpacePacketProtocolEntity(apid=apid, transport=transport)
         self.spp_entity.indication = self._incoming_pdu_handler
         self._packet_sequence_count = 0
 
     def _get_next_packet_sequence_count(self):
         self._packet_sequence_count += 1
         return self._packet_sequence_count
 
     def request(self, pdu):
-        space_packet = spp.SpacePacket(
+        space_packet = SpacePacket(
             packet_type=self.packet_type,
             packet_sec_hdr_flag=False,
             apid=self.apid,
-            sequence_flags=spp.SequenceFlags.UNSEGMENTED,
+            sequence_flags=SequenceFlags.UNSEGMENTED,
             packet_sequence_count=self._get_next_packet_sequence_count(),
             packet_data_field=pdu,
         )
         self.spp_entity.request(space_packet)
 
     def _incoming_pdu_handler(self, space_packet):
         data = space_packet.packet_data_field
```

### Comparing `cfdp-2.0.0/src/cfdp/transport/udp.py` & `cfdp-2.1.0/src/cfdp/transport/udp.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp/transport/zmq.py` & `cfdp-2.1.0/src/cfdp/transport/zmq.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/src/cfdp.egg-info/PKG-INFO` & `cfdp-2.1.0/src/cfdp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfdp
-Version: 2.0.0
+Version: 2.1.0
 Summary: CCSDS File Delivery Protocol
 Author-email: LibreCube <info@librecube.org>
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Python CFDP
```

### Comparing `cfdp-2.0.0/src/cfdp.egg-info/SOURCES.txt` & `cfdp-2.1.0/src/cfdp.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 src/cfdp/pdu/header.py
 src/cfdp/pdu/keep_alive.py
 src/cfdp/pdu/metadata.py
 src/cfdp/pdu/nak.py
 src/cfdp/pdu/prompt.py
 src/cfdp/transport/__init__.py
 src/cfdp/transport/base.py
-src/cfdp/transport/spp.py
+src/cfdp/transport/spacepacket.py
 src/cfdp/transport/udp.py
 src/cfdp/transport/zmq.py
 tests/test_series_F1.py
 tests/test_series_F2.py
 tests/test_series_F3.py
 tests/test_series_F4.py
-tests/test_spp.py
+tests/test_spacepacket.py
 tests/test_zmq.py
```

### Comparing `cfdp-2.0.0/tests/test_series_F1.py` & `cfdp-2.1.0/tests/test_series_F1.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/tests/test_series_F2.py` & `cfdp-2.1.0/tests/test_series_F2.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/tests/test_series_F3.py` & `cfdp-2.1.0/tests/test_series_F3.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/tests/test_series_F4.py` & `cfdp-2.1.0/tests/test_series_F4.py`

 * *Files identical despite different names*

### Comparing `cfdp-2.0.0/tests/test_spp.py` & `cfdp-2.1.0/tests/test_spacepacket.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import os
 import time
 
+import spacepacket
+
 import cfdp
-import spp
-from cfdp.transport.spp import SppTransport
+from cfdp.transport.spacepacket import SpacePacketTransport
 from cfdp.transport.udp import UdpTransport
 from cfdp.filestore import NativeFileStore
 
-from utils import RemoteEntitySpp
+from utils import RemoteEntitySpacePacket
 
 
-def test_spp():
-    remote_entity = RemoteEntitySpp()
+def test_spacepacket():
+    remote_entity = RemoteEntitySpacePacket()
     remote_entity.up()
 
     udp_transport = UdpTransport(routing={"*": [("127.0.0.1", 5222)]})
     udp_transport.bind("127.0.0.1", 5111)
 
-    spp_transport = SppTransport(
-        apid=222, transport=udp_transport, packet_type=spp.PacketType.TELECOMMAND
+    spacepacket_transport = SpacePacketTransport(
+        apid=222,
+        transport=udp_transport,
+        packet_type=spacepacket.PacketType.TELECOMMAND,
     )
 
     cfdp_entity = cfdp.CfdpEntity(
-        entity_id=2, filestore=NativeFileStore("./files/local"), transport=spp_transport
+        entity_id=2,
+        filestore=NativeFileStore("./files/local"),
+        transport=spacepacket_transport,
     )
 
     transaction_id = cfdp_entity.put(
         destination_id=2,
         source_filename="/medium.txt",
         destination_filename="/medium.txt",
         transmission_mode=cfdp.TransmissionMode.ACKNOWLEDGED,
@@ -46,9 +51,9 @@
 
 
 if __name__ == "__main__":
     import logging
 
     logging.basicConfig(level=logging.DEBUG)
 
-    print("Test Spp Transport " + 50 * "=")
-    test_spp()
+    print("Test spacepacket Transport " + 50 * "=")
+    test_spacepacket()
```

### Comparing `cfdp-2.0.0/tests/test_zmq.py` & `cfdp-2.1.0/tests/test_zmq.py`

 * *Files identical despite different names*

