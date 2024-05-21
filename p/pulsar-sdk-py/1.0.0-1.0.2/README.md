# Comparing `tmp/pulsar_sdk_py-1.0.0.tar.gz` & `tmp/pulsar_sdk_py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulsar_sdk_py-1.0.0.tar", max compression
+gzip compressed data, was "pulsar_sdk_py-1.0.2.tar", max compression
```

## Comparing `pulsar_sdk_py-1.0.0.tar` & `pulsar_sdk_py-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1049 2024-02-06 15:40:18.498953 pulsar_sdk_py-1.0.0/README.md
--rw-r--r--   0        0        0       34 2023-12-15 00:28:43.487148 pulsar_sdk_py-1.0.0/pulsar_sdk_py/__init__.py
--rw-r--r--   0        0        0       22 2024-01-02 13:52:17.086151 pulsar_sdk_py-1.0.0/pulsar_sdk_py/constants.py
--rw-r--r--   0        0        0        0 2023-07-26 10:51:45.846396 pulsar_sdk_py-1.0.0/pulsar_sdk_py/dataclasses/__init__.py
--rw-r--r--   0        0        0    11192 2024-02-06 13:53:43.442690 pulsar_sdk_py-1.0.0/pulsar_sdk_py/dataclasses/schemas.py
--rw-r--r--   0        0        0     1422 2023-12-22 14:39:40.455443 pulsar_sdk_py-1.0.0/pulsar_sdk_py/dataclasses/serializer.py
--rw-r--r--   0        0        0     5690 2023-12-27 12:10:06.073007 pulsar_sdk_py-1.0.0/pulsar_sdk_py/enums.py
--rw-r--r--   0        0        0      439 2024-01-02 13:52:17.086894 pulsar_sdk_py-1.0.0/pulsar_sdk_py/exceptions.py
--rw-r--r--   0        0        0      634 2023-07-26 10:51:45.846131 pulsar_sdk_py-1.0.0/pulsar_sdk_py/helpers.py
--rw-r--r--   0        0        0       97 2023-12-21 13:07:05.707722 pulsar_sdk_py-1.0.0/pulsar_sdk_py/logger.py
--rw-r--r--   0        0        0     2417 2023-12-22 14:38:55.426933 pulsar_sdk_py-1.0.0/pulsar_sdk_py/pulsar_sdk.py
--rw-r--r--   0        0        0      234 2023-09-27 14:16:52.965531 pulsar_sdk_py-1.0.0/pulsar_sdk_py/rest/__init__.py
--rw-r--r--   0        0        0     3370 2024-01-02 13:52:17.089164 pulsar_sdk_py-1.0.0/pulsar_sdk_py/rest/base.py
--rw-r--r--   0        0        0      710 2023-12-15 15:33:37.112796 pulsar_sdk_py-1.0.0/pulsar_sdk_py/rest/name_service.py
--rw-r--r--   0        0        0     3833 2023-12-22 14:49:26.422139 pulsar_sdk_py-1.0.0/pulsar_sdk_py/rest/nfts.py
--rw-r--r--   0        0        0     1833 2023-12-22 14:49:26.422403 pulsar_sdk_py-1.0.0/pulsar_sdk_py/rest/protocols.py
--rw-r--r--   0        0        0     2454 2023-12-22 14:49:26.422850 pulsar_sdk_py-1.0.0/pulsar_sdk_py/rest/tokens.py
--rw-r--r--   0        0        0      656 2023-12-22 14:49:26.423206 pulsar_sdk_py-1.0.0/pulsar_sdk_py/rest/wallets.py
--rw-r--r--   0        0        0      505 2024-01-18 20:02:14.731137 pulsar_sdk_py-1.0.0/pulsar_sdk_py/sleep.py
--rw-r--r--   0        0        0       77 2023-12-22 14:38:55.427761 pulsar_sdk_py-1.0.0/pulsar_sdk_py/websocket/__init__.py
--rw-r--r--   0        0        0     3285 2024-02-06 13:53:12.121276 pulsar_sdk_py-1.0.0/pulsar_sdk_py/websocket/balances.py
--rw-r--r--   0        0        0    14658 2024-01-31 14:23:57.927885 pulsar_sdk_py-1.0.0/pulsar_sdk_py/websocket/base.py
--rw-r--r--   0        0        0     1580 2023-12-22 14:38:55.428398 pulsar_sdk_py-1.0.0/pulsar_sdk_py/websocket/encryption.py
--rw-r--r--   0        0        0      916 2023-12-22 14:38:55.428645 pulsar_sdk_py-1.0.0/pulsar_sdk_py/websocket/websocket_types.py
--rw-r--r--   0        0        0      799 2024-02-06 15:39:53.464015 pulsar_sdk_py-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 pulsar_sdk_py-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1049 2024-05-21 11:26:41.938139 pulsar_sdk_py-1.0.2/README.md
+-rw-r--r--   0        0        0       34 2024-02-26 12:19:42.401871 pulsar_sdk_py-1.0.2/pulsar_sdk_py/__init__.py
+-rw-r--r--   0        0        0       22 2024-02-26 12:19:42.401940 pulsar_sdk_py-1.0.2/pulsar_sdk_py/constants.py
+-rw-r--r--   0        0        0        0 2024-02-26 12:19:42.402015 pulsar_sdk_py-1.0.2/pulsar_sdk_py/dataclasses/__init__.py
+-rw-r--r--   0        0        0    11200 2024-05-21 09:13:51.818290 pulsar_sdk_py-1.0.2/pulsar_sdk_py/dataclasses/schemas.py
+-rw-r--r--   0        0        0     1422 2024-02-26 12:19:42.402212 pulsar_sdk_py-1.0.2/pulsar_sdk_py/dataclasses/serializer.py
+-rw-r--r--   0        0        0     5690 2024-05-21 09:20:21.624461 pulsar_sdk_py-1.0.2/pulsar_sdk_py/enums.py
+-rw-r--r--   0        0        0      439 2024-02-26 12:19:42.402401 pulsar_sdk_py-1.0.2/pulsar_sdk_py/exceptions.py
+-rw-r--r--   0        0        0      634 2024-02-26 12:19:42.402474 pulsar_sdk_py-1.0.2/pulsar_sdk_py/helpers.py
+-rw-r--r--   0        0        0       97 2024-02-26 12:19:42.402546 pulsar_sdk_py-1.0.2/pulsar_sdk_py/logger.py
+-rw-r--r--   0        0        0     2417 2024-02-26 12:19:42.402672 pulsar_sdk_py-1.0.2/pulsar_sdk_py/pulsar_sdk.py
+-rw-r--r--   0        0        0      234 2024-02-26 12:19:42.402795 pulsar_sdk_py-1.0.2/pulsar_sdk_py/rest/__init__.py
+-rw-r--r--   0        0        0     3370 2024-02-26 12:19:42.402904 pulsar_sdk_py-1.0.2/pulsar_sdk_py/rest/base.py
+-rw-r--r--   0        0        0      710 2024-02-26 12:19:42.402992 pulsar_sdk_py-1.0.2/pulsar_sdk_py/rest/name_service.py
+-rw-r--r--   0        0        0     3833 2024-02-26 12:19:42.403076 pulsar_sdk_py-1.0.2/pulsar_sdk_py/rest/nfts.py
+-rw-r--r--   0        0        0     1833 2024-02-26 12:19:42.403151 pulsar_sdk_py-1.0.2/pulsar_sdk_py/rest/protocols.py
+-rw-r--r--   0        0        0     2454 2024-02-26 12:19:42.403226 pulsar_sdk_py-1.0.2/pulsar_sdk_py/rest/tokens.py
+-rw-r--r--   0        0        0      656 2024-02-26 12:19:42.403297 pulsar_sdk_py-1.0.2/pulsar_sdk_py/rest/wallets.py
+-rw-r--r--   0        0        0      505 2024-02-26 12:19:42.403368 pulsar_sdk_py-1.0.2/pulsar_sdk_py/sleep.py
+-rw-r--r--   0        0        0       77 2024-02-26 12:19:42.403487 pulsar_sdk_py-1.0.2/pulsar_sdk_py/websocket/__init__.py
+-rw-r--r--   0        0        0     3255 2024-05-21 09:13:51.818567 pulsar_sdk_py-1.0.2/pulsar_sdk_py/websocket/balances.py
+-rw-r--r--   0        0        0    14658 2024-02-26 12:19:42.403711 pulsar_sdk_py-1.0.2/pulsar_sdk_py/websocket/base.py
+-rw-r--r--   0        0        0     1580 2024-02-26 12:19:42.403796 pulsar_sdk_py-1.0.2/pulsar_sdk_py/websocket/encryption.py
+-rw-r--r--   0        0        0      916 2024-02-26 12:19:42.403880 pulsar_sdk_py-1.0.2/pulsar_sdk_py/websocket/websocket_types.py
+-rw-r--r--   0        0        0      799 2024-05-21 11:26:37.681667 pulsar_sdk_py-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 pulsar_sdk_py-1.0.2/PKG-INFO
```

### Comparing `pulsar_sdk_py-1.0.0/README.md` & `pulsar_sdk_py-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-1.0.0/pulsar_sdk_py/dataclasses/schemas.py` & `pulsar_sdk_py-1.0.2/pulsar_sdk_py/dataclasses/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     slug_id: str | None = None
     url: str | None = None
     marketplace_id: str | None = None
 
 
 @dataclass
 class NFTCollectionStats:
-    price_timeseries: dict[str, str | None]
+    price_timeseries: dict[str, str | float | None]
 
 
 @dataclass
 class NFTCollection:
     id: str
     address: str | None
     chain: str
```

### Comparing `pulsar_sdk_py-1.0.0/pulsar_sdk_py/dataclasses/serializer.py` & `pulsar_sdk_py-1.0.2/pulsar_sdk_py/dataclasses/serializer.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-1.0.0/pulsar_sdk_py/enums.py` & `pulsar_sdk_py-1.0.2/pulsar_sdk_py/enums.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-1.0.0/pulsar_sdk_py/helpers.py` & `pulsar_sdk_py-1.0.2/pulsar_sdk_py/helpers.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-1.0.0/pulsar_sdk_py/pulsar_sdk.py` & `pulsar_sdk_py-1.0.2/pulsar_sdk_py/pulsar_sdk.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-1.0.0/pulsar_sdk_py/rest/base.py` & `pulsar_sdk_py-1.0.2/pulsar_sdk_py/rest/base.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-1.0.0/pulsar_sdk_py/rest/name_service.py` & `pulsar_sdk_py-1.0.2/pulsar_sdk_py/rest/name_service.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-1.0.0/pulsar_sdk_py/rest/nfts.py` & `pulsar_sdk_py-1.0.2/pulsar_sdk_py/rest/nfts.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-1.0.0/pulsar_sdk_py/rest/protocols.py` & `pulsar_sdk_py-1.0.2/pulsar_sdk_py/rest/protocols.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-1.0.0/pulsar_sdk_py/rest/tokens.py` & `pulsar_sdk_py-1.0.2/pulsar_sdk_py/rest/tokens.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-1.0.0/pulsar_sdk_py/rest/wallets.py` & `pulsar_sdk_py-1.0.2/pulsar_sdk_py/rest/wallets.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-1.0.0/pulsar_sdk_py/websocket/base.py` & `pulsar_sdk_py-1.0.2/pulsar_sdk_py/websocket/base.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-1.0.0/pulsar_sdk_py/websocket/encryption.py` & `pulsar_sdk_py-1.0.2/pulsar_sdk_py/websocket/encryption.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-1.0.0/pulsar_sdk_py/websocket/websocket_types.py` & `pulsar_sdk_py-1.0.2/pulsar_sdk_py/websocket/websocket_types.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-1.0.0/pyproject.toml` & `pulsar_sdk_py-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pulsar-sdk-py"
-version = "1.0.0"
+version = "1.0.2"
 description = ""
 authors = [ "Pulsar <admin@pulsar.finance>",]
 readme = "README.md"
 packages = [
     {include = "pulsar_sdk_py"},
 ]
```

### Comparing `pulsar_sdk_py-1.0.0/PKG-INFO` & `pulsar_sdk_py-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulsar-sdk-py
-Version: 1.0.0
+Version: 1.0.2
 Summary: 
 Author: Pulsar
 Author-email: admin@pulsar.finance
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

