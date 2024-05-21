# Comparing `tmp/bencode_c-0.0.6.tar.gz` & `tmp/bencode_c-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bencode_c-0.0.6.tar", last modified: Mon May 20 23:59:49 2024, max compression
+gzip compressed data, was "bencode_c-0.0.7.tar", last modified: Tue May 21 01:18:50 2024, max compression
```

## Comparing `bencode_c-0.0.6.tar` & `bencode_c-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:59:49.768436 bencode_c-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 23:59:49.768436 bencode_c-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-20 23:59:44.000000 bencode_c-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-20 23:59:44.000000 bencode_c-0.0.6/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 23:59:49.768436 bencode_c-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-20 23:59:44.000000 bencode_c-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:59:49.764436 bencode_c-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:59:49.764436 bencode_c-0.0.6/src/bencode_c/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 23:59:44.000000 bencode_c-0.0.6/src/bencode_c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-20 23:59:44.000000 bencode_c-0.0.6/src/bencode_c/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-20 23:59:44.000000 bencode_c-0.0.6/src/bencode_c/bencode.c
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 23:59:44.000000 bencode_c-0.0.6/src/bencode_c/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-20 23:59:44.000000 bencode_c-0.0.6/src/bencode_c/decode.h
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-05-20 23:59:44.000000 bencode_c-0.0.6/src/bencode_c/encode.h
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 23:59:44.000000 bencode_c-0.0.6/src/bencode_c/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:59:49.768436 bencode_c-0.0.6/src/bencode_c.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 23:59:49.000000 bencode_c-0.0.6/src/bencode_c.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-20 23:59:49.000000 bencode_c-0.0.6/src/bencode_c.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 23:59:49.000000 bencode_c-0.0.6/src/bencode_c.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-20 23:59:49.000000 bencode_c-0.0.6/src/bencode_c.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 23:59:49.000000 bencode_c-0.0.6/src/bencode_c.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:59:49.764436 bencode_c-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-20 23:59:44.000000 bencode_c-0.0.6/tests/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-20 23:59:44.000000 bencode_c-0.0.6/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-20 23:59:44.000000 bencode_c-0.0.6/tests/test_torrent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:18:50.175282 bencode_c-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-21 01:18:50.175282 bencode_c-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-21 01:18:43.000000 bencode_c-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 01:18:43.000000 bencode_c-0.0.7/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 01:18:50.175282 bencode_c-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-21 01:18:43.000000 bencode_c-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:18:50.171282 bencode_c-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:18:50.171282 bencode_c-0.0.7/src/bencode_c/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-21 01:18:43.000000 bencode_c-0.0.7/src/bencode_c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-21 01:18:43.000000 bencode_c-0.0.7/src/bencode_c/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-21 01:18:43.000000 bencode_c-0.0.7/src/bencode_c/bencode.c
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-21 01:18:43.000000 bencode_c-0.0.7/src/bencode_c/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-21 01:18:43.000000 bencode_c-0.0.7/src/bencode_c/decode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-05-21 01:18:43.000000 bencode_c-0.0.7/src/bencode_c/encode.h
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 01:18:43.000000 bencode_c-0.0.7/src/bencode_c/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:18:50.171282 bencode_c-0.0.7/src/bencode_c.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-21 01:18:50.000000 bencode_c-0.0.7/src/bencode_c.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-21 01:18:50.000000 bencode_c-0.0.7/src/bencode_c.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 01:18:50.000000 bencode_c-0.0.7/src/bencode_c.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-21 01:18:50.000000 bencode_c-0.0.7/src/bencode_c.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 01:18:50.000000 bencode_c-0.0.7/src/bencode_c.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:18:50.171282 bencode_c-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-21 01:18:43.000000 bencode_c-0.0.7/tests/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-21 01:18:43.000000 bencode_c-0.0.7/tests/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 01:18:43.000000 bencode_c-0.0.7/tests/test_torrent.py
```

### Comparing `bencode_c-0.0.6/PKG-INFO` & `bencode_c-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bencode-c
-Version: 0.0.6
+Version: 0.0.7
 Summary: A fast and correct bencode serialize/deserialize library
 Author-email: trim21 <trim21me@gmail.com>
 License: MIT
 Keywords: bencode,bittorrent,bit-torrent,serialize,deserialize,p2p
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bencode_c-0.0.6/pyproject.toml` & `bencode_c-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pyproject.toml
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bencode-c"
-version = "0.0.6"
+version = "0.0.7"
 description = "A fast and correct bencode serialize/deserialize library"
 license = { text = "MIT" }
 requires-python = ">=3.8,<4.0"
 authors = [
     { name = "trim21", email = "trim21me@gmail.com" },
 ]
 readme = 'readme.md'
```

### Comparing `bencode_c-0.0.6/src/bencode_c/bencode.c` & `bencode_c-0.0.7/src/bencode_c/bencode.c`

 * *Files identical despite different names*

### Comparing `bencode_c-0.0.6/src/bencode_c/decode.h` & `bencode_c-0.0.7/src/bencode_c/decode.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,49 @@
 #include "common.h"
 
 static PyObject *BencodeDecodeError;
 
-static PyObject *decode_any(const char *buf, HPy_ssize_t *index, HPy_ssize_t size);
+static inline PyObject *decodeError(const char *fmt, ...);
+static PyObject *decode_any(const char *buf, Py_ssize_t *index, Py_ssize_t size);
+static PyObject *decode_int(const char *buf, Py_ssize_t *index, Py_ssize_t size);
+static PyObject *decode_bytes(const char *buf, Py_ssize_t *index, Py_ssize_t size);
+static PyObject *decode_dict(const char *buf, Py_ssize_t *index, Py_ssize_t size);
+static PyObject *decode_list(const char *buf, Py_ssize_t *index, Py_ssize_t size);
 
-static inline HPy decodeError(const char *fmt, ...) {
+static PyObject *bdecode(PyObject *self, PyObject *b) {
+  if (!PyBytes_Check(b)) {
+    PyErr_SetString(PyExc_TypeError, "can only decode bytes");
+    return NULL;
+  }
+
+  Py_ssize_t size = PyBytes_Size(b);
+  const char *buf = PyBytes_AsString(b);
+
+  Py_ssize_t index = 0;
+
+  PyObject *r = decode_any(buf, &index, size);
+
+  if (index != size) {
+    return decodeError("invalid bencode data, index %d", index);
+  }
+
+  // return Py_BuildValue("");
+  return r;
+  // return Py_None;
+}
+
+static inline PyObject *decodeError(const char *fmt, ...) {
   PyErr_SetObject(BencodeDecodeError, PyUnicode_FromFormat(fmt));
   return NULL;
 }
 
-static HPy decode_int(const char *buf, HPy_ssize_t *index, HPy_ssize_t size) {
-  HPy_ssize_t index_e = 0;
+static PyObject *decode_int(const char *buf, Py_ssize_t *index, Py_ssize_t size) {
+  Py_ssize_t index_e = 0;
 
-  for (HPy_ssize_t i = *index; i < size; i++) {
+  for (Py_ssize_t i = *index; i < size; i++) {
     if (buf[i] == 'e') {
       index_e = i;
       break;
     }
   }
 
   if (index_e == 0) {
@@ -35,47 +62,47 @@
   } else if (buf[*index] == '0') {
     if (*index + 1 != index_e) {
       return decodeError("invalid int, non-zero int should not start with '0'. found at %d", *index);
     }
   }
 
   long long val = 0;
-  for (HPy_ssize_t i = *index; i < index_e; i++) {
+  for (Py_ssize_t i = *index; i < index_e; i++) {
     if (buf[i] > '9' || buf[i] < '0') {
       return decodeError("invalid int, '%c' found at %d", buf[i], i);
     }
     val = val * 10 + (buf[i] - '0');
   }
 
   val = val * sign;
 
   *index = index_e + 1;
   return PyLong_FromLongLong(val);
 }
 
 // // there is no bytes/str in bencode, they only have 1 type for both of them.
-static HPy decode_str(const char *buf, HPy_ssize_t *index, HPy_ssize_t size) {
-  HPy_ssize_t index_sep = 0;
-  for (HPy_ssize_t i = *index; i < size; i++) {
+static PyObject *decode_bytes(const char *buf, Py_ssize_t *index, Py_ssize_t size) {
+  Py_ssize_t index_sep = 0;
+  for (Py_ssize_t i = *index; i < size; i++) {
     if (buf[i] == ':') {
       index_sep = i;
       break;
     }
   }
 
   if (index_sep == 0) {
     return decodeError("invalid string, missing length: index %d", *index);
   }
 
   if (buf[*index] == '0' && *index + 1 != index_sep) {
     return decodeError("invalid bytes length, found at %d", *index);
   }
 
-  HPy_ssize_t len = 0;
-  for (HPy_ssize_t i = *index; i < index_sep; i++) {
+  Py_ssize_t len = 0;
+  for (Py_ssize_t i = *index; i < index_sep; i++) {
     if (buf[i] < '0' || buf[i] > '9') {
       return decodeError("invalid bytes length, found '%c' at %d", buf[i], i);
     }
     len = len * 10 + (buf[i] - '0');
   }
 
   if (index_sep + len >= size) {
@@ -83,26 +110,28 @@
   }
 
   *index = index_sep + len + 1;
 
   return PyBytes_FromStringAndSize(&buf[index_sep + 1], len);
 }
 
-static HPy decode_list(const char *buf, HPy_ssize_t *index, HPy_ssize_t size) {
+static PyObject *decode_list(const char *buf, Py_ssize_t *index, Py_ssize_t size) {
   *index = *index + 1;
 
-  HPy l = PyList_New(0);
+  PyObject *l = PyList_New(0);
 
   while (buf[*index] != 'e') {
-    HPy obj = decode_any(buf, index, size);
+    PyObject *obj = decode_any(buf, index, size);
     if (obj == NULL) {
       return NULL;
     }
 
     PyList_Append(l, obj);
+
+    Py_DecRef(obj);
   }
 
   *index = *index + 1;
 
   return l;
 }
 
@@ -120,80 +149,61 @@
   } else if (len1 > len2) {
     return 1;
   } else {
     return 0;
   }
 }
 
-static HPy decode_dict(const char *buf, HPy_ssize_t *index, HPy_ssize_t size) {
+static PyObject *decode_dict(const char *buf, Py_ssize_t *index, Py_ssize_t size) {
   *index = *index + 1;
-  HPy d = PyDict_New();
+  PyObject *d = PyDict_New();
   const char *lastKey = NULL;
   size_t lastKeyLen = 0;
   const char *currentKey;
   size_t currentKeyLen;
   while (buf[*index] != 'e') {
-    HPy key = decode_str(buf, index, size);
+    PyObject *key = decode_bytes(buf, index, size);
     if (key == NULL) {
       return NULL;
     }
 
-    HPy obj = decode_any(buf, index, size);
+    PyObject *obj = decode_any(buf, index, size);
     if (obj == NULL) {
       return NULL;
     }
     currentKeyLen = PyBytes_Size(key);
     currentKey = PyBytes_AsString(key);
     // skip first key
     if (lastKey != NULL) {
       if (strCompare(currentKey, currentKeyLen, lastKey, lastKeyLen) < 0) {
         return decodeError("invalid dict, key not sorted. index %d", *index);
       }
     }
     lastKey = currentKey;
     lastKeyLen = currentKeyLen;
     PyDict_SetItem(d, key, obj);
+    Py_DecRef(key);
+    Py_DecRef(obj);
   }
   *index = *index + 1;
   return d;
 }
 
-static PyObject *decode_any(const char *buf, HPy_ssize_t *index, HPy_ssize_t size) {
+static PyObject *decode_any(const char *buf, Py_ssize_t *index, Py_ssize_t size) {
   // int
   if (buf[*index] == 'i') {
     return decode_int(buf, index, size);
   }
   if (buf[*index] >= '0' && buf[*index] <= '9') {
-    return decode_str(buf, index, size);
+    return decode_bytes(buf, index, size);
   }
   // // list
   if (buf[*index] == 'l') {
     return decode_list(buf, index, size);
   }
 
   if (buf[*index] == 'd') {
     return decode_dict(buf, index, size);
   }
 
   return decodeError("invalid bencode prefix '%c', index %d", buf[*index], *index);
 }
-
-static PyObject *bdecode(PyObject *self, PyObject *b) {
-  if (!PyBytes_Check(b)) {
-    PyErr_SetString(PyExc_TypeError, "can only decode bytes");
-    return NULL;
-  }
-
-  HPy_ssize_t size = PyBytes_Size(b);
-  const char *buf = PyBytes_AsString(b);
-
-  HPy_ssize_t index = 0;
-
-  PyObject *r = decode_any(buf, &index, size);
-
-  if (index != size) {
-    Py_DecRef(r);
-    return decodeError("invalid bencode data, index %d", index);
-  }
-
-  return r;
-}
```

### Comparing `bencode_c-0.0.6/src/bencode_c/encode.h` & `bencode_c-0.0.7/src/bencode_c/encode.h`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,19 @@
   if (keys == NULL) {
     runtimeError("failed to get dict keys");
     return 1;
   }
 
   *count = PyObject_Length(keys);
 
+  if (*count == 0) {
+    Py_DecRef(keys);
+    return 0;
+  }
+
   *list = PyList_New(0);
 
   for (HPy_ssize_t i = 0; i < *count; i++) {
     HPy key = PySequence_GetItem(keys, i);
     HPy value = PyDict_GetItem(obj, key);
     HPy keyAsBytes = key;
     if (PyUnicode_Check(key)) {
@@ -107,14 +112,16 @@
       runtimeError("can not pack key value pair");
       return 1;
     }
 
     PyList_Append(*list, tu);
   }
 
+  Py_DecRef(keys);
+
   if (PyObject_CallMethod(*list, "sort", NULL) == NULL) {
     return 1;
   }
 
   // check duplicated keys
   const char *currentKey = NULL;
   size_t currentKeylen = 0;
@@ -181,23 +188,29 @@
 
     returnIfError(bufferWrite(buf, "i", 1));
     returnIfError(bufferWriteLong(buf, val));
     return bufferWrite(buf, "e", 1);
   } else if (PyList_Check(obj)) {
     HPy_ssize_t len = PyList_Size(obj);
     returnIfError(bufferWrite(buf, "l", 1));
+    if (len == 0) {
+      return bufferWrite(buf, "e", 1);
+    }
 
     for (HPy_ssize_t i = 0; i < len; i++) {
       HPy o = PyList_GetItem(obj, i);
       returnIfError(encodeAny(buf, o));
     }
     return bufferWrite(buf, "e", 1);
   } else if (PyTuple_Check(obj)) {
     HPy_ssize_t len = PyTuple_Size(obj);
     returnIfError(bufferWrite(buf, "l", 1));
+    if (len == 0) {
+      return bufferWrite(buf, "e", 1);
+    }
 
     for (HPy_ssize_t i = 0; i < len; i++) {
       HPy o = PyTuple_GetItem(obj, i);
       returnIfError(encodeAny(buf, o));
     }
     return bufferWrite(buf, "e", 1);
 
@@ -205,41 +218,48 @@
     returnIfError(bufferWrite(buf, "d", 1));
     HPy list = NULL;
     HPy_ssize_t count = 0;
     if (buildDictKeyList(obj, &list, &count)) {
       return 1;
     }
 
+    if (count == 0) {
+      return bufferWrite(buf, "e", 1);
+    }
+
     for (HPy_ssize_t i = 0; i < count; i++) {
       HPy keyValue = PyList_GetItem(list, i); // tuple[bytes, Any]
+
       if (keyValue == NULL) {
         runtimeError("failed to get key/value tuple from list");
         return 1;
       }
+
       HPy key = PyTuple_GetItem(keyValue, 0);
-      HPy value = PyTuple_GetItem(keyValue, 1);
+      Py_DecRef(keyValue);
       if (key == NULL) {
         runtimeError("can't get key from key,value tuple");
         return 1;
       }
-      if (value == NULL) {
-        runtimeError("can't get value");
+
+      if (encodeBytes(buf, key)) {
+        Py_DecRef(key);
         return 1;
       }
-      if (encodeBytes(buf, key)) {
-        Py_DecRef(list);
+
+      HPy value = PyTuple_GetItem(keyValue, 1);
+      if (value == NULL) {
+        runtimeError("can't get value");
         return 1;
       }
+
       if (encodeAny(buf, value)) {
-        Py_DecRef(list);
+        Py_DecRef(value);
         return 1;
       }
-
-      Py_DecRef(key);
-      Py_DecRef(value);
     }
 
     Py_DecRef(list);
     return bufferWrite(buf, "e", 1);
   }
 
   HPy typ = PyObject_Type(obj);
@@ -249,23 +269,20 @@
   return 1;
 }
 
 static HPy bencode(HPy self, HPy obj) {
   // self is the module object
 
   struct buffer *buf = newBuffer();
-  Py_IncRef(obj);
 
   if (encodeAny(buf, obj)) {
     freeBuffer(buf);
-    Py_DecRef(obj);
     // error when encoding
     return NULL;
   }
 
   HPy res = PyBytes_FromStringAndSize(buf->buf, buf->len);
 
   freeBuffer(buf);
-  Py_DecRef(obj);
 
   return res;
 };
```

### Comparing `bencode_c-0.0.6/src/bencode_c.egg-info/PKG-INFO` & `bencode_c-0.0.7/src/bencode_c.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bencode-c
-Version: 0.0.6
+Version: 0.0.7
 Summary: A fast and correct bencode serialize/deserialize library
 Author-email: trim21 <trim21me@gmail.com>
 License: MIT
 Keywords: bencode,bittorrent,bit-torrent,serialize,deserialize,p2p
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bencode_c-0.0.6/tests/test_decode.py` & `bencode_c-0.0.7/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `bencode_c-0.0.6/tests/test_encode.py` & `bencode_c-0.0.7/tests/test_encode.py`

 * *Files identical despite different names*

