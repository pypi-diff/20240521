# Comparing `tmp/smp-1.0.1.tar.gz` & `tmp/smp-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smp-1.0.1.tar", max compression
+gzip compressed data, was "smp-1.0.2.tar", max compression
```

## Comparing `smp-1.0.1.tar` & `smp-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11365 2024-05-19 22:32:36.689672 smp-1.0.1/LICENSE
--rw-r--r--   0        0        0     2312 2024-05-19 22:32:36.689672 smp-1.0.1/README.md
--rw-r--r--   0        0        0     1595 2024-05-19 22:32:36.689672 smp-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 22:32:36.689672 smp-1.0.1/smp/__init__.py
--rw-r--r--   0        0        0      695 2024-05-19 22:32:36.689672 smp-1.0.1/smp/error.py
--rw-r--r--   0        0        0      471 2024-05-19 22:32:36.689672 smp-1.0.1/smp/exceptions.py
--rw-r--r--   0        0        0     5090 2024-05-19 22:32:36.689672 smp-1.0.1/smp/header.py
--rw-r--r--   0        0        0     6286 2024-05-19 22:32:36.689672 smp-1.0.1/smp/image_management.py
--rw-r--r--   0        0        0     4882 2024-05-19 22:32:36.689672 smp-1.0.1/smp/message.py
--rw-r--r--   0        0        0     7153 2024-05-19 22:32:36.689672 smp-1.0.1/smp/os_management.py
--rw-r--r--   0        0        0     3135 2024-05-19 22:32:36.689672 smp-1.0.1/smp/packet.py
--rw-r--r--   0        0        0        0 2024-05-19 22:32:36.689672 smp-1.0.1/smp/py.typed
--rw-r--r--   0        0        0     1022 2024-05-19 22:32:36.689672 smp-1.0.1/smp/shell_management.py
--rw-r--r--   0        0        0        0 2024-05-19 22:32:36.689672 smp-1.0.1/smp/user/__init__.py
--rw-r--r--   0        0        0     1321 2024-05-19 22:32:36.689672 smp-1.0.1/smp/user/intercreate.py
--rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 smp-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11365 2024-05-20 23:28:26.282016 smp-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2312 2024-05-20 23:28:26.282016 smp-1.0.2/README.md
+-rw-r--r--   0        0        0     1595 2024-05-20 23:28:26.282016 smp-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-20 23:28:26.282016 smp-1.0.2/smp/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-20 23:28:26.282016 smp-1.0.2/smp/error.py
+-rw-r--r--   0        0        0      471 2024-05-20 23:28:26.282016 smp-1.0.2/smp/exceptions.py
+-rw-r--r--   0        0        0     5090 2024-05-20 23:28:26.282016 smp-1.0.2/smp/header.py
+-rw-r--r--   0        0        0     6286 2024-05-20 23:28:26.282016 smp-1.0.2/smp/image_management.py
+-rw-r--r--   0        0        0     4882 2024-05-20 23:28:26.282016 smp-1.0.2/smp/message.py
+-rw-r--r--   0        0        0     7153 2024-05-20 23:28:26.282016 smp-1.0.2/smp/os_management.py
+-rw-r--r--   0        0        0     3135 2024-05-20 23:28:26.282016 smp-1.0.2/smp/packet.py
+-rw-r--r--   0        0        0        0 2024-05-20 23:28:26.282016 smp-1.0.2/smp/py.typed
+-rw-r--r--   0        0        0     1022 2024-05-20 23:28:26.282016 smp-1.0.2/smp/shell_management.py
+-rw-r--r--   0        0        0        0 2024-05-20 23:28:26.282016 smp-1.0.2/smp/user/__init__.py
+-rw-r--r--   0        0        0     1321 2024-05-20 23:28:26.282016 smp-1.0.2/smp/user/intercreate.py
+-rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 smp-1.0.2/PKG-INFO
```

### Comparing `smp-1.0.1/LICENSE` & `smp-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smp-1.0.1/README.md` & `smp-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `smp-1.0.1/pyproject.toml` & `smp-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smp-1.0.1/smp/error.py` & `smp-1.0.2/smp/error.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.1/smp/header.py` & `smp-1.0.2/smp/header.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.1/smp/image_management.py` & `smp-1.0.2/smp/image_management.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.1/smp/message.py` & `smp-1.0.2/smp/message.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.1/smp/os_management.py` & `smp-1.0.2/smp/os_management.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.1/smp/packet.py` & `smp-1.0.2/smp/packet.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.1/smp/shell_management.py` & `smp-1.0.2/smp/shell_management.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.1/smp/user/intercreate.py` & `smp-1.0.2/smp/user/intercreate.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.1/PKG-INFO` & `smp-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smp
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple Management Protocol (SMP) for remotely managing MCU firmware
 License: Apache-2.0
 Author: J.P. Hutchins
 Author-email: jphutchins@gmail.com
 Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

