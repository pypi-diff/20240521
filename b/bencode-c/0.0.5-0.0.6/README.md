# Comparing `tmp/bencode_c-0.0.5.tar.gz` & `tmp/bencode_c-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bencode_c-0.0.5.tar", last modified: Mon May 20 23:53:15 2024, max compression
+gzip compressed data, was "bencode_c-0.0.6.tar", last modified: Mon May 20 23:59:49 2024, max compression
```

## Comparing `bencode_c-0.0.5.tar` & `bencode_c-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:53:15.106739 bencode_c-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 23:53:15.106739 bencode_c-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-20 23:53:12.000000 bencode_c-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-20 23:53:12.000000 bencode_c-0.0.5/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 23:53:15.106739 bencode_c-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-20 23:53:12.000000 bencode_c-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:53:15.098739 bencode_c-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:53:15.102739 bencode_c-0.0.5/src/bencode_c/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 23:53:12.000000 bencode_c-0.0.5/src/bencode_c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-20 23:53:12.000000 bencode_c-0.0.5/src/bencode_c/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-20 23:53:12.000000 bencode_c-0.0.5/src/bencode_c/bencode.c
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 23:53:12.000000 bencode_c-0.0.5/src/bencode_c/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-20 23:53:12.000000 bencode_c-0.0.5/src/bencode_c/decode.h
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-05-20 23:53:12.000000 bencode_c-0.0.5/src/bencode_c/encode.h
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 23:53:12.000000 bencode_c-0.0.5/src/bencode_c/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:53:15.102739 bencode_c-0.0.5/src/bencode_c.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 23:53:15.000000 bencode_c-0.0.5/src/bencode_c.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-20 23:53:15.000000 bencode_c-0.0.5/src/bencode_c.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 23:53:15.000000 bencode_c-0.0.5/src/bencode_c.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-20 23:53:15.000000 bencode_c-0.0.5/src/bencode_c.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 23:53:15.000000 bencode_c-0.0.5/src/bencode_c.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:53:15.102739 bencode_c-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-20 23:53:12.000000 bencode_c-0.0.5/tests/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-20 23:53:12.000000 bencode_c-0.0.5/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-20 23:53:12.000000 bencode_c-0.0.5/tests/test_torrent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:59:49.768436 bencode_c-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 23:59:49.768436 bencode_c-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-20 23:59:44.000000 bencode_c-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-20 23:59:44.000000 bencode_c-0.0.6/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 23:59:49.768436 bencode_c-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-20 23:59:44.000000 bencode_c-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:59:49.764436 bencode_c-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:59:49.764436 bencode_c-0.0.6/src/bencode_c/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 23:59:44.000000 bencode_c-0.0.6/src/bencode_c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-20 23:59:44.000000 bencode_c-0.0.6/src/bencode_c/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-20 23:59:44.000000 bencode_c-0.0.6/src/bencode_c/bencode.c
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 23:59:44.000000 bencode_c-0.0.6/src/bencode_c/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-20 23:59:44.000000 bencode_c-0.0.6/src/bencode_c/decode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-05-20 23:59:44.000000 bencode_c-0.0.6/src/bencode_c/encode.h
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 23:59:44.000000 bencode_c-0.0.6/src/bencode_c/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:59:49.768436 bencode_c-0.0.6/src/bencode_c.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 23:59:49.000000 bencode_c-0.0.6/src/bencode_c.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-20 23:59:49.000000 bencode_c-0.0.6/src/bencode_c.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 23:59:49.000000 bencode_c-0.0.6/src/bencode_c.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-20 23:59:49.000000 bencode_c-0.0.6/src/bencode_c.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 23:59:49.000000 bencode_c-0.0.6/src/bencode_c.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:59:49.764436 bencode_c-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-20 23:59:44.000000 bencode_c-0.0.6/tests/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-20 23:59:44.000000 bencode_c-0.0.6/tests/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-20 23:59:44.000000 bencode_c-0.0.6/tests/test_torrent.py
```

### Comparing `bencode_c-0.0.5/PKG-INFO` & `bencode_c-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bencode-c
-Version: 0.0.5
+Version: 0.0.6
 Summary: A fast and correct bencode serialize/deserialize library
 Author-email: trim21 <trim21me@gmail.com>
 License: MIT
 Keywords: bencode,bittorrent,bit-torrent,serialize,deserialize,p2p
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bencode_c-0.0.5/pyproject.toml` & `bencode_c-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pyproject.toml
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bencode-c"
-version = "0.0.5"
+version = "0.0.6"
 description = "A fast and correct bencode serialize/deserialize library"
 license = { text = "MIT" }
 requires-python = ">=3.8,<4.0"
 authors = [
     { name = "trim21", email = "trim21me@gmail.com" },
 ]
 readme = 'readme.md'
```

### Comparing `bencode_c-0.0.5/src/bencode_c/bencode.c` & `bencode_c-0.0.6/src/bencode_c/bencode.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#define Py_LIMITED_API 0x03080000
+#define Py_LIMITED_API 0x03070000
 
 // TODO: should use a extern here
 #include "decode.h"
 #include "encode.h"
 
 static PyMethodDef DemoMethods[] = {
     {"bencode", bencode, METH_O, "encode python object to bytes"},
```

### Comparing `bencode_c-0.0.5/src/bencode_c/decode.h` & `bencode_c-0.0.6/src/bencode_c/decode.h`

 * *Files identical despite different names*

### Comparing `bencode_c-0.0.5/src/bencode_c/encode.h` & `bencode_c-0.0.6/src/bencode_c/encode.h`

 * *Files identical despite different names*

### Comparing `bencode_c-0.0.5/src/bencode_c.egg-info/PKG-INFO` & `bencode_c-0.0.6/src/bencode_c.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bencode-c
-Version: 0.0.5
+Version: 0.0.6
 Summary: A fast and correct bencode serialize/deserialize library
 Author-email: trim21 <trim21me@gmail.com>
 License: MIT
 Keywords: bencode,bittorrent,bit-torrent,serialize,deserialize,p2p
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bencode_c-0.0.5/tests/test_decode.py` & `bencode_c-0.0.6/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `bencode_c-0.0.5/tests/test_encode.py` & `bencode_c-0.0.6/tests/test_encode.py`

 * *Files identical despite different names*

