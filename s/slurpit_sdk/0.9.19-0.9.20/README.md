# Comparing `tmp/slurpit_sdk-0.9.19.tar.gz` & `tmp/slurpit_sdk-0.9.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurpit_sdk-0.9.19.tar", max compression
+gzip compressed data, was "slurpit_sdk-0.9.20.tar", max compression
```

## Comparing `slurpit_sdk-0.9.19.tar` & `slurpit_sdk-0.9.20.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1064 2024-05-21 09:07:21.815816 slurpit_sdk-0.9.19/LICENSE
--rw-r--r--   0        0        0      297 2024-05-21 12:06:15.282217 slurpit_sdk-0.9.19/pyproject.toml
--rw-r--r--   0        0        0     1708 2024-05-21 08:19:28.379495 slurpit_sdk-0.9.19/README.md
--rw-r--r--   0        0        0       57 2024-05-21 08:19:28.386498 slurpit_sdk-0.9.19/src/slurpit/__init__.py
--rw-r--r--   0        0        0     2225 2024-05-21 08:19:28.386498 slurpit_sdk-0.9.19/src/slurpit/api.py
--rw-r--r--   0        0        0        0 2024-05-21 08:19:28.387503 slurpit_sdk-0.9.19/src/slurpit/apis/__init__.py
--rw-r--r--   0        0        0     7053 2024-05-21 08:19:28.387503 slurpit_sdk-0.9.19/src/slurpit/apis/baseapi.py
--rw-r--r--   0        0        0    11256 2024-05-21 08:19:28.388668 slurpit_sdk-0.9.19/src/slurpit/apis/deviceapi.py
--rw-r--r--   0        0        0     4068 2024-05-21 08:19:28.388668 slurpit_sdk-0.9.19/src/slurpit/apis/planningapi.py
--rw-r--r--   0        0        0     1198 2024-05-21 08:19:28.389676 slurpit_sdk-0.9.19/src/slurpit/apis/platformapi.py
--rw-r--r--   0        0        0     7944 2024-05-21 08:19:28.389676 slurpit_sdk-0.9.19/src/slurpit/apis/scannerapi.py
--rw-r--r--   0        0        0    14816 2024-05-21 08:19:28.390745 slurpit_sdk-0.9.19/src/slurpit/apis/scraperapi.py
--rw-r--r--   0        0        0     8150 2024-05-21 08:19:28.390745 slurpit_sdk-0.9.19/src/slurpit/apis/templateapi.py
--rw-r--r--   0        0        0     4839 2024-05-21 08:19:28.391749 slurpit_sdk-0.9.19/src/slurpit/apis/userapi.py
--rw-r--r--   0        0        0     4431 2024-05-21 08:19:28.392881 slurpit_sdk-0.9.19/src/slurpit/apis/vaultapi.py
--rw-r--r--   0        0        0        0 2024-05-21 08:19:28.392881 slurpit_sdk-0.9.19/src/slurpit/models/__init__.py
--rw-r--r--   0        0        0       27 2024-05-21 08:19:28.394085 slurpit_sdk-0.9.19/src/slurpit/models/basemodel.py
--rw-r--r--   0        0        0     2606 2024-05-21 08:19:28.394085 slurpit_sdk-0.9.19/src/slurpit/models/device.py
--rw-r--r--   0        0        0     1301 2024-05-21 08:19:28.394085 slurpit_sdk-0.9.19/src/slurpit/models/planning.py
--rw-r--r--   0        0        0      396 2024-05-21 08:19:28.395093 slurpit_sdk-0.9.19/src/slurpit/models/platform.py
--rw-r--r--   0        0        0     2017 2024-05-21 08:19:28.395093 slurpit_sdk-0.9.19/src/slurpit/models/scanner.py
--rw-r--r--   0        0        0     1932 2024-05-21 08:19:28.396093 slurpit_sdk-0.9.19/src/slurpit/models/template.py
--rw-r--r--   0        0        0     2107 2024-05-21 08:19:28.396093 slurpit_sdk-0.9.19/src/slurpit/models/user.py
--rw-r--r--   0        0        0     2738 2024-05-21 08:19:28.396093 slurpit_sdk-0.9.19/src/slurpit/models/vault.py
--rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 slurpit_sdk-0.9.19/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-21 08:59:38.455182 slurpit_sdk-0.9.20/LICENSE
+-rw-r--r--   0        0        0     1712 2024-05-21 12:12:56.770682 slurpit_sdk-0.9.20/README.md
+-rw-r--r--   0        0        0      297 2024-05-21 12:14:07.339204 slurpit_sdk-0.9.20/pyproject.toml
+-rw-r--r--   0        0        0       57 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/__init__.py
+-rw-r--r--   0        0        0     2225 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/api.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:14:07.459205 slurpit_sdk-0.9.20/src/slurpit/apis/__init__.py
+-rw-r--r--   0        0        0     7053 2024-05-14 19:35:54.536903 slurpit_sdk-0.9.20/src/slurpit/apis/baseapi.py
+-rw-r--r--   0        0        0    11256 2024-05-20 10:32:39.146951 slurpit_sdk-0.9.20/src/slurpit/apis/deviceapi.py
+-rw-r--r--   0        0        0     4068 2024-05-21 08:05:20.334037 slurpit_sdk-0.9.20/src/slurpit/apis/planningapi.py
+-rw-r--r--   0        0        0     1198 2024-05-20 12:11:15.309046 slurpit_sdk-0.9.20/src/slurpit/apis/platformapi.py
+-rw-r--r--   0        0        0     7944 2024-05-20 10:32:39.146951 slurpit_sdk-0.9.20/src/slurpit/apis/scannerapi.py
+-rw-r--r--   0        0        0    14816 2024-05-20 12:11:15.309046 slurpit_sdk-0.9.20/src/slurpit/apis/scraperapi.py
+-rw-r--r--   0        0        0     8150 2024-05-21 08:05:20.334037 slurpit_sdk-0.9.20/src/slurpit/apis/templateapi.py
+-rw-r--r--   0        0        0     4839 2024-05-20 10:32:39.146951 slurpit_sdk-0.9.20/src/slurpit/apis/userapi.py
+-rw-r--r--   0        0        0     4431 2024-05-20 10:32:39.146951 slurpit_sdk-0.9.20/src/slurpit/apis/vaultapi.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:14:07.463205 slurpit_sdk-0.9.20/src/slurpit/models/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/models/basemodel.py
+-rw-r--r--   0        0        0     2606 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/models/device.py
+-rw-r--r--   0        0        0     1301 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/models/planning.py
+-rw-r--r--   0        0        0      396 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/models/platform.py
+-rw-r--r--   0        0        0     2017 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/models/scanner.py
+-rw-r--r--   0        0        0     1932 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/models/template.py
+-rw-r--r--   0        0        0     2107 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/models/user.py
+-rw-r--r--   0        0        0     2738 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/models/vault.py
+-rw-r--r--   0        0        0     2209 1970-01-01 00:00:00.000000 slurpit_sdk-0.9.20/PKG-INFO
```

### Comparing `slurpit_sdk-0.9.19/LICENSE` & `slurpit_sdk-0.9.20/LICENSE`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.19/README.md` & `slurpit_sdk-0.9.20/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 The Slurpit SDK is a Python package for interacting with the Slurpit API, enabling developers to easily manage devices and planning resources. It is designed for simplicity and flexibility, offering methods for listing devices, retrieving planning data, and exporting information to CSV format.
 
 ## Installation
 
 You can install the Slurpit SDK using pip with the following command:
 
 ```bash
-pip install slurpkit
+pip install slurpit_sdk
 ```
 
 Alternatively, if you prefer to install from source, clone the repository and run the setup script:
 
 ```bash
-git clone https://gitlab.com/slurpit.io/python-sdk.git
+git clone https://gitlab.com/slurpit.io/slurpit_sdk.git
 cd slurpit
 python setup.py install
 ```
 
 ## Quick Start
 
 To use the SDK, start by importing the package and setting up the API client:
```

### Comparing `slurpit_sdk-0.9.19/src/slurpit/api.py` & `slurpit_sdk-0.9.20/src/slurpit/api.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.19/src/slurpit/apis/baseapi.py` & `slurpit_sdk-0.9.20/src/slurpit/apis/baseapi.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.19/src/slurpit/apis/deviceapi.py` & `slurpit_sdk-0.9.20/src/slurpit/apis/deviceapi.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.19/src/slurpit/apis/planningapi.py` & `slurpit_sdk-0.9.20/src/slurpit/apis/planningapi.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.19/src/slurpit/apis/platformapi.py` & `slurpit_sdk-0.9.20/src/slurpit/apis/platformapi.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.19/src/slurpit/apis/scannerapi.py` & `slurpit_sdk-0.9.20/src/slurpit/apis/scannerapi.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.19/src/slurpit/apis/scraperapi.py` & `slurpit_sdk-0.9.20/src/slurpit/apis/scraperapi.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.19/src/slurpit/apis/templateapi.py` & `slurpit_sdk-0.9.20/src/slurpit/apis/templateapi.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.19/src/slurpit/apis/userapi.py` & `slurpit_sdk-0.9.20/src/slurpit/apis/userapi.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.19/src/slurpit/apis/vaultapi.py` & `slurpit_sdk-0.9.20/src/slurpit/apis/vaultapi.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.19/src/slurpit/models/device.py` & `slurpit_sdk-0.9.20/src/slurpit/models/device.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.19/src/slurpit/models/planning.py` & `slurpit_sdk-0.9.20/src/slurpit/models/planning.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.19/src/slurpit/models/scanner.py` & `slurpit_sdk-0.9.20/src/slurpit/models/scanner.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.19/src/slurpit/models/template.py` & `slurpit_sdk-0.9.20/src/slurpit/models/template.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.19/src/slurpit/models/user.py` & `slurpit_sdk-0.9.20/src/slurpit/models/user.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.19/src/slurpit/models/vault.py` & `slurpit_sdk-0.9.20/src/slurpit/models/vault.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.19/PKG-INFO` & `slurpit_sdk-0.9.20/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurpit_sdk
-Version: 0.9.19
+Version: 0.9.20
 Summary: A robust Python SDK for slurpit
 Author: Slurp'it
 Author-email: info@slurpit.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -18,21 +18,21 @@
 The Slurpit SDK is a Python package for interacting with the Slurpit API, enabling developers to easily manage devices and planning resources. It is designed for simplicity and flexibility, offering methods for listing devices, retrieving planning data, and exporting information to CSV format.
 
 ## Installation
 
 You can install the Slurpit SDK using pip with the following command:
 
 ```bash
-pip install slurpkit
+pip install slurpit_sdk
 ```
 
 Alternatively, if you prefer to install from source, clone the repository and run the setup script:
 
 ```bash
-git clone https://gitlab.com/slurpit.io/python-sdk.git
+git clone https://gitlab.com/slurpit.io/slurpit_sdk.git
 cd slurpit
 python setup.py install
 ```
 
 ## Quick Start
 
 To use the SDK, start by importing the package and setting up the API client:
```

