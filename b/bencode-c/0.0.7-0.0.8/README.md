# Comparing `tmp/bencode_c-0.0.7.tar.gz` & `tmp/bencode_c-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bencode_c-0.0.7.tar", last modified: Tue May 21 01:18:50 2024, max compression
+gzip compressed data, was "bencode_c-0.0.8.tar", last modified: Tue May 21 14:10:07 2024, max compression
```

## Comparing `bencode_c-0.0.7.tar` & `bencode_c-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:18:50.175282 bencode_c-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-21 01:18:50.175282 bencode_c-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-21 01:18:43.000000 bencode_c-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 01:18:43.000000 bencode_c-0.0.7/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 01:18:50.175282 bencode_c-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-21 01:18:43.000000 bencode_c-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:18:50.171282 bencode_c-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:18:50.171282 bencode_c-0.0.7/src/bencode_c/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-21 01:18:43.000000 bencode_c-0.0.7/src/bencode_c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-21 01:18:43.000000 bencode_c-0.0.7/src/bencode_c/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-21 01:18:43.000000 bencode_c-0.0.7/src/bencode_c/bencode.c
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-21 01:18:43.000000 bencode_c-0.0.7/src/bencode_c/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-21 01:18:43.000000 bencode_c-0.0.7/src/bencode_c/decode.h
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-05-21 01:18:43.000000 bencode_c-0.0.7/src/bencode_c/encode.h
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 01:18:43.000000 bencode_c-0.0.7/src/bencode_c/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:18:50.171282 bencode_c-0.0.7/src/bencode_c.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-21 01:18:50.000000 bencode_c-0.0.7/src/bencode_c.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-21 01:18:50.000000 bencode_c-0.0.7/src/bencode_c.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 01:18:50.000000 bencode_c-0.0.7/src/bencode_c.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-21 01:18:50.000000 bencode_c-0.0.7/src/bencode_c.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 01:18:50.000000 bencode_c-0.0.7/src/bencode_c.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:18:50.171282 bencode_c-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-21 01:18:43.000000 bencode_c-0.0.7/tests/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-21 01:18:43.000000 bencode_c-0.0.7/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 01:18:43.000000 bencode_c-0.0.7/tests/test_torrent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:10:07.365729 bencode_c-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-21 14:10:07.365729 bencode_c-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-21 14:10:04.000000 bencode_c-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-21 14:10:04.000000 bencode_c-0.0.8/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 14:10:07.365729 bencode_c-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-21 14:10:04.000000 bencode_c-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:10:07.361729 bencode_c-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:10:07.361729 bencode_c-0.0.8/src/bencode_c/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-21 14:10:04.000000 bencode_c-0.0.8/src/bencode_c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-21 14:10:04.000000 bencode_c-0.0.8/src/bencode_c/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-21 14:10:04.000000 bencode_c-0.0.8/src/bencode_c/bencode.c
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-21 14:10:04.000000 bencode_c-0.0.8/src/bencode_c/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-05-21 14:10:04.000000 bencode_c-0.0.8/src/bencode_c/decode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-21 14:10:04.000000 bencode_c-0.0.8/src/bencode_c/encode.h
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 14:10:04.000000 bencode_c-0.0.8/src/bencode_c/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:10:07.365729 bencode_c-0.0.8/src/bencode_c.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-21 14:10:07.000000 bencode_c-0.0.8/src/bencode_c.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-21 14:10:07.000000 bencode_c-0.0.8/src/bencode_c.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 14:10:07.000000 bencode_c-0.0.8/src/bencode_c.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-21 14:10:07.000000 bencode_c-0.0.8/src/bencode_c.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 14:10:07.000000 bencode_c-0.0.8/src/bencode_c.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:10:07.365729 bencode_c-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-21 14:10:04.000000 bencode_c-0.0.8/tests/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-21 14:10:04.000000 bencode_c-0.0.8/tests/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 14:10:04.000000 bencode_c-0.0.8/tests/test_torrent.py
```

### Comparing `bencode_c-0.0.7/PKG-INFO` & `bencode_c-0.0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bencode-c
-Version: 0.0.7
+Version: 0.0.8
 Summary: A fast and correct bencode serialize/deserialize library
 Author-email: trim21 <trim21me@gmail.com>
 License: MIT
 Keywords: bencode,bittorrent,bit-torrent,serialize,deserialize,p2p
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,7 +14,19 @@
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Requires-Dist: pytest==8.2.0; extra == "testing"
 Requires-Dist: pytest-github-actions-annotate-failures==0.2.0; extra == "testing"
 
 bencode serialize/deserialize written in native c extension.
+
+```shell
+pip install bencode-c
+```
+
+```python
+import bencode_c
+
+assert bencode_c.bdecode(b'...') == ...
+
+assert bencode_c.bencode(...) == b'...'
+```
```

### Comparing `bencode_c-0.0.7/pyproject.toml` & `bencode_c-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pyproject.toml
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bencode-c"
-version = "0.0.7"
+version = "0.0.8"
 description = "A fast and correct bencode serialize/deserialize library"
 license = { text = "MIT" }
 requires-python = ">=3.8,<4.0"
 authors = [
     { name = "trim21", email = "trim21me@gmail.com" },
 ]
 readme = 'readme.md'
```

### Comparing `bencode_c-0.0.7/src/bencode_c/bencode.c` & `bencode_c-0.0.8/src/bencode_c/bencode.c`

 * *Files 11% similar despite different names*

```diff
@@ -15,24 +15,30 @@
 };
 
 PyMODINIT_FUNC PyInit__bencode(void) {
   PyObject *m = PyModule_Create(&moduleDef);
   if (m == NULL)
     return NULL;
 
-  BencodeDecodeError = PyErr_NewException("_bencode.BencodeDecodeError", NULL, NULL);
+  errTypeMessage = PyUnicode_FromString(NON_SUPPORTED_TYPE_MESSAGE);
+  if(errTypeMessage == NULL) {
+    Py_DECREF(m);
+    return NULL;
+  }
+
+  BencodeDecodeError = PyErr_NewException("bencode_c.BencodeDecodeError", NULL, NULL);
   Py_XINCREF(BencodeDecodeError);
   if (PyModule_AddObject(m, "BencodeDecodeError", BencodeDecodeError) < 0) {
     Py_XDECREF(BencodeDecodeError);
     Py_CLEAR(BencodeDecodeError);
     Py_DECREF(m);
     return NULL;
   }
 
-  BencodeEncodeError = PyErr_NewException("_bencode.BencodeEncodeError", NULL, NULL);
+  BencodeEncodeError = PyErr_NewException("bencode_c.BencodeEncodeError", NULL, NULL);
   Py_XINCREF(BencodeEncodeError);
   if (PyModule_AddObject(m, "BencodeEncodeError", BencodeEncodeError) < 0) {
     Py_XDECREF(BencodeEncodeError);
     Py_CLEAR(BencodeEncodeError);
     Py_DECREF(m);
     return NULL;
   }
```

### Comparing `bencode_c-0.0.7/src/bencode_c/decode.h` & `bencode_c-0.0.8/src/bencode_c/decode.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,131 +1,132 @@
 #include "common.h"
+#include "object.h"
 
 static PyObject *BencodeDecodeError;
 
-static inline PyObject *decodeError(const char *fmt, ...);
-static PyObject *decode_any(const char *buf, Py_ssize_t *index, Py_ssize_t size);
-static PyObject *decode_int(const char *buf, Py_ssize_t *index, Py_ssize_t size);
-static PyObject *decode_bytes(const char *buf, Py_ssize_t *index, Py_ssize_t size);
-static PyObject *decode_dict(const char *buf, Py_ssize_t *index, Py_ssize_t size);
-static PyObject *decode_list(const char *buf, Py_ssize_t *index, Py_ssize_t size);
+static inline PyObject *decodingError(const char *fmt, ...);
+
+static PyObject *decodeAny(const char *buf, Py_ssize_t *index, Py_ssize_t size);
+static PyObject *decodeInt(const char *buf, Py_ssize_t *index, Py_ssize_t size);
+static PyObject *decodeBytes(const char *buf, Py_ssize_t *index, Py_ssize_t size);
+static PyObject *decodeDict(const char *buf, Py_ssize_t *index, Py_ssize_t size, PyObject *dict);
+static PyObject *decodeList(const char *buf, Py_ssize_t *index, Py_ssize_t size);
 
 static PyObject *bdecode(PyObject *self, PyObject *b) {
   if (!PyBytes_Check(b)) {
     PyErr_SetString(PyExc_TypeError, "can only decode bytes");
     return NULL;
   }
 
   Py_ssize_t size = PyBytes_Size(b);
   const char *buf = PyBytes_AsString(b);
 
   Py_ssize_t index = 0;
 
-  PyObject *r = decode_any(buf, &index, size);
+  PyObject *r = decodeAny(buf, &index, size);
 
   if (index != size) {
-    return decodeError("invalid bencode data, index %d", index);
+    return decodingError("invalid bencode data, index %d", index);
   }
 
-  // return Py_BuildValue("");
   return r;
-  // return Py_None;
 }
 
-static inline PyObject *decodeError(const char *fmt, ...) {
+static inline PyObject *decodingError(const char *fmt, ...) {
   PyErr_SetObject(BencodeDecodeError, PyUnicode_FromFormat(fmt));
   return NULL;
 }
 
-static PyObject *decode_int(const char *buf, Py_ssize_t *index, Py_ssize_t size) {
+static PyObject *decodeInt(const char *buf, Py_ssize_t *index, Py_ssize_t size) {
   Py_ssize_t index_e = 0;
 
   for (Py_ssize_t i = *index; i < size; i++) {
     if (buf[i] == 'e') {
       index_e = i;
       break;
     }
   }
 
   if (index_e == 0) {
-    return decodeError("invalid int, missing 'e': %d", *index);
+    return decodingError("invalid int, missing 'e': %d", *index);
   }
 
   long long sign = 1;
   *index = *index + 1;
   if (buf[*index] == '-') {
     if (buf[*index + 1] == '0') {
-      return decodeError("invalid int, '-0' found at %d", *index);
+      return decodingError("invalid int, '-0' found at %d", *index);
     }
 
     sign = -1;
     *index = *index + 1;
   } else if (buf[*index] == '0') {
     if (*index + 1 != index_e) {
-      return decodeError("invalid int, non-zero int should not start with '0'. found at %d", *index);
+      return decodingError("invalid int, non-zero int should not start with '0'. found at %d", *index);
     }
   }
 
   long long val = 0;
   for (Py_ssize_t i = *index; i < index_e; i++) {
     if (buf[i] > '9' || buf[i] < '0') {
-      return decodeError("invalid int, '%c' found at %d", buf[i], i);
+      return decodingError("invalid int, '%c' found at %d", buf[i], i);
     }
     val = val * 10 + (buf[i] - '0');
   }
 
   val = val * sign;
 
   *index = index_e + 1;
   return PyLong_FromLongLong(val);
 }
 
 // // there is no bytes/str in bencode, they only have 1 type for both of them.
-static PyObject *decode_bytes(const char *buf, Py_ssize_t *index, Py_ssize_t size) {
+static PyObject *decodeBytes(const char *buf, Py_ssize_t *index, Py_ssize_t size) {
   Py_ssize_t index_sep = 0;
   for (Py_ssize_t i = *index; i < size; i++) {
     if (buf[i] == ':') {
       index_sep = i;
       break;
     }
   }
 
   if (index_sep == 0) {
-    return decodeError("invalid string, missing length: index %d", *index);
+    return decodingError("invalid string, missing length: index %d", *index);
   }
 
   if (buf[*index] == '0' && *index + 1 != index_sep) {
-    return decodeError("invalid bytes length, found at %d", *index);
+    return decodingError("invalid bytes length, found at %d", *index);
   }
 
   Py_ssize_t len = 0;
   for (Py_ssize_t i = *index; i < index_sep; i++) {
     if (buf[i] < '0' || buf[i] > '9') {
-      return decodeError("invalid bytes length, found '%c' at %d", buf[i], i);
+      return decodingError("invalid bytes length, found '%c' at %d", buf[i], i);
     }
     len = len * 10 + (buf[i] - '0');
   }
 
   if (index_sep + len >= size) {
-    return decodeError("bytes length overflow, index %d", *index);
+    return decodingError("bytes length overflow, index %d", *index);
   }
 
   *index = index_sep + len + 1;
 
   return PyBytes_FromStringAndSize(&buf[index_sep + 1], len);
 }
 
-static PyObject *decode_list(const char *buf, Py_ssize_t *index, Py_ssize_t size) {
+static PyObject *decodeList(const char *buf, Py_ssize_t *index, Py_ssize_t size) {
   *index = *index + 1;
 
   PyObject *l = PyList_New(0);
 
   while (buf[*index] != 'e') {
-    PyObject *obj = decode_any(buf, index, size);
+    PyObject *obj = decodeAny(buf, index, size);
     if (obj == NULL) {
+      Py_DecRef(l);
       return NULL;
     }
 
     PyList_Append(l, obj);
 
     Py_DecRef(obj);
   }
@@ -149,61 +150,71 @@
   } else if (len1 > len2) {
     return 1;
   } else {
     return 0;
   }
 }
 
-static PyObject *decode_dict(const char *buf, Py_ssize_t *index, Py_ssize_t size) {
+static PyObject *decodeDict(const char *buf, Py_ssize_t *index, Py_ssize_t size, PyObject *d) {
   *index = *index + 1;
-  PyObject *d = PyDict_New();
   const char *lastKey = NULL;
   size_t lastKeyLen = 0;
   const char *currentKey;
   size_t currentKeyLen;
   while (buf[*index] != 'e') {
-    PyObject *key = decode_bytes(buf, index, size);
+    PyObject *key = decodeBytes(buf, index, size);
     if (key == NULL) {
       return NULL;
     }
 
-    PyObject *obj = decode_any(buf, index, size);
+    PyObject *obj = decodeAny(buf, index, size);
     if (obj == NULL) {
+      Py_DecRef(key);
       return NULL;
     }
     currentKeyLen = PyBytes_Size(key);
     currentKey = PyBytes_AsString(key);
     // skip first key
     if (lastKey != NULL) {
-      if (strCompare(currentKey, currentKeyLen, lastKey, lastKeyLen) < 0) {
-        return decodeError("invalid dict, key not sorted. index %d", *index);
+      int keyCmp = strCompare(currentKey, currentKeyLen, lastKey, lastKeyLen);
+      if (keyCmp < 0) {
+        return decodingError("invalid dict, key not sorted. index %d", *index);
+      }
+      if (keyCmp == 0) {
+        return decodingError("invalid dict, find duplicated keys %.*s. index %d", currentKeyLen, currentKey, *index);
       }
     }
     lastKey = currentKey;
     lastKeyLen = currentKeyLen;
     PyDict_SetItem(d, key, obj);
-    Py_DecRef(key);
-    Py_DecRef(obj);
   }
   *index = *index + 1;
   return d;
 }
 
-static PyObject *decode_any(const char *buf, Py_ssize_t *index, Py_ssize_t size) {
+static PyObject *decodeAny(const char *buf, Py_ssize_t *index, Py_ssize_t size) {
   // int
   if (buf[*index] == 'i') {
-    return decode_int(buf, index, size);
+    return decodeInt(buf, index, size);
   }
   if (buf[*index] >= '0' && buf[*index] <= '9') {
-    return decode_bytes(buf, index, size);
+    return decodeBytes(buf, index, size);
   }
   // // list
   if (buf[*index] == 'l') {
-    return decode_list(buf, index, size);
+    return decodeList(buf, index, size);
   }
 
   if (buf[*index] == 'd') {
-    return decode_dict(buf, index, size);
+    PyObject *dict = PyDict_New();
+
+    PyObject *r = decodeDict(buf, index, size, dict);
+    if (r == NULL) {
+      Py_DecRef(dict);
+      return NULL;
+    }
+
+    return r;
   }
 
-  return decodeError("invalid bencode prefix '%c', index %d", buf[*index], *index);
+  return decodingError("invalid bencode prefix '%c', index %d", buf[*index], *index);
 }
```

### Comparing `bencode_c-0.0.7/src/bencode_c/encode.h` & `bencode_c-0.0.8/src/bencode_c/encode.h`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 #define HPyLong_Check(obj) Py_TypeCheck(obj, PyLong_Type)
 #define returnIfError(o)                                                                                               \
   if (o) {                                                                                                             \
     return o;                                                                                                          \
   }
 
+static HPy errTypeMessage;
+
 static inline void runtimeError(const char *data) { PyErr_SetString(PyExc_RuntimeError, data); }
 
 static inline void typeError(const char *data) { PyErr_SetString(PyExc_TypeError, data); }
 
 static inline HPy bencodeError(const char *data) {
   PyErr_SetString(BencodeEncodeError, data);
   return NULL;
@@ -73,51 +75,67 @@
 }
 
 static void freeBuffer(struct buffer *buf) {
   free(buf->buf);
   free(buf);
 }
 
+static int encodeAny(struct buffer *buf, HPy obj);
+
 // obj must be a python dict object.
 // TODO: use c native struct and sorting
 static int buildDictKeyList(HPy obj, HPy *list, HPy_ssize_t *count) {
+  *count = PyObject_Length(obj);
+
+  if (*count == 0) {
+    return 0;
+  }
+
   HPy keys = PyDict_Keys(obj);
   if (keys == NULL) {
     runtimeError("failed to get dict keys");
     return 1;
   }
 
-  *count = PyObject_Length(keys);
-
-  if (*count == 0) {
-    Py_DecRef(keys);
-    return 0;
-  }
-
   *list = PyList_New(0);
 
   for (HPy_ssize_t i = 0; i < *count; i++) {
     HPy key = PySequence_GetItem(keys, i);
-    HPy value = PyDict_GetItem(obj, key);
+    if (key == NULL) {
+      Py_DecRef(keys);
+      runtimeError("failed to get key from dict");
+      return 1;
+    }
+
     HPy keyAsBytes = key;
     if (PyUnicode_Check(key)) {
       keyAsBytes = PyUnicode_AsUTF8String(key);
     } else if (!PyBytes_Check(key)) {
       bencodeError("dict key must be str or bytes");
+      Py_DecRef(keys);
+      Py_DecRef(key);
+      return 1;
+    }
+
+    HPy value = PyDict_GetItem(obj, key);
+    if (value == NULL) {
       Py_DecRef(key);
+      Py_DecRef(keys);
+      runtimeError("failed to get value from dict");
       return 1;
     }
 
     HPy tu = PyTuple_Pack(2, keyAsBytes, value);
     if (tu == NULL) {
       runtimeError("can not pack key value pair");
       return 1;
     }
 
     PyList_Append(*list, tu);
+    Py_DecRef(tu);
   }
 
   Py_DecRef(keys);
 
   if (PyObject_CallMethod(*list, "sort", NULL) == NULL) {
     return 1;
   }
@@ -132,56 +150,119 @@
     HPy keyValue = PyList_GetItem(*list, i);
     HPy key = PyTuple_GetItem(keyValue, 0);
     currentKeylen = PyBytes_Size(key);
     currentKey = PyBytes_AsString(key);
     if (lastKey != NULL) {
       if (lastKeylen == currentKeylen) {
         if (strncmp(lastKey, currentKey, lastKeylen) == 0) {
+          // Py_DecRef(keyValue);
+          // Py_DecRef(key);
           bencodeError("find duplicated keys with str and bytes in dict");
           return 1;
         }
       }
     }
 
     lastKey = currentKey;
     lastKeylen = currentKeylen;
+
+    // Py_DecRef(keyValue);
+    // Py_DecRef(key);
   }
 
   return 0;
 }
+
+// TODO: use PyUnicode_AsUTF8AndSize after 3.10
+static int encodeStr(struct buffer *buf, HPy obj) {
+  HPy b = PyUnicode_AsUTF8String(obj);
+
+  HPy_ssize_t size = PyBytes_Size(b);
+
+  const char *data = PyBytes_AsString(b);
+
+  int err = bufferWriteLong(buf, size);
+  err |= bufferWrite(buf, ":", 1);
+  err |= bufferWrite(buf, data, size);
+
+  Py_DecRef(b);
+
+  return err;
+}
+
 static int encodeBytes(struct buffer *buf, HPy obj) {
   HPy_ssize_t size = PyBytes_Size(obj);
   const char *data = PyBytes_AsString(obj);
 
   returnIfError(bufferWriteLong(buf, size));
   returnIfError(bufferWrite(buf, ":", 1));
   return bufferWrite(buf, data, size);
 }
 
+static int encodeDict(struct buffer *buf, HPy obj) {
+  returnIfError(bufferWrite(buf, "d", 1));
+  HPy list = NULL;
+  HPy_ssize_t count = 0;
+  if (buildDictKeyList(obj, &list, &count)) {
+    if (list != NULL) {
+      Py_DecRef(list);
+    }
+    return 1;
+  }
+
+  if (count == 0) {
+    return bufferWrite(buf, "e", 1);
+  }
+
+  for (HPy_ssize_t i = 0; i < count; i++) {
+    HPy keyValue = PyList_GetItem(list, i); // tuple[bytes, Any]
+    if (keyValue == NULL) {
+      Py_DecRef(list);
+      runtimeError("failed to get key/value tuple from list");
+      return 1;
+    }
+
+    HPy key = PyTuple_GetItem(keyValue, 0);
+    if (key == NULL) {
+      Py_DecRef(list);
+      runtimeError("can't get key from key,value tuple");
+      return 1;
+    }
+
+    if (encodeBytes(buf, key)) {
+      Py_DecRef(list);
+      return 1;
+    }
+
+    HPy value = PyTuple_GetItem(keyValue, 1);
+    if (value == NULL) {
+      Py_DecRef(list);
+      runtimeError("can't get value");
+      return 1;
+    }
+
+    if (encodeAny(buf, value)) {
+      Py_DecRef(list);
+      return 1;
+    }
+  }
+
+  Py_DecRef(list);
+  return bufferWrite(buf, "e", 1);
+}
+
 static int encodeAny(struct buffer *buf, HPy obj) {
   if (Py_True == obj) {
     return bufferWrite(buf, "i1e", 3);
   } else if (Py_False == obj) {
     return bufferWrite(buf, "i0e", 3);
   } else if (PyBytes_Check(obj)) {
     return encodeBytes(buf, obj);
   } else if (PyUnicode_Check(obj)) {
-
-#if PY_VERSION_HEX >= 0x03100000
-    HPy_ssize_t size;
-    const char *data = PyUnicode_AsUTF8AndSize(obj, &size);
-#else
-    HPy b = PyUnicode_AsUTF8String(obj);
-    HPy_ssize_t size = PyBytes_Size(b);
-    const char *data = PyBytes_AsString(b);
-#endif
-
-    returnIfError(bufferWriteLong(buf, size));
-    returnIfError(bufferWrite(buf, ":", 1));
-    return bufferWrite(buf, data, size);
+    return encodeStr(buf, obj);
   } else if (PyLong_Check(obj)) {
     long long val = PyLong_AsLongLong(obj);
 
     // python int may overflow c long long
     if (PyErr_Occurred()) {
       return 1;
     }
@@ -211,64 +292,35 @@
     for (HPy_ssize_t i = 0; i < len; i++) {
       HPy o = PyTuple_GetItem(obj, i);
       returnIfError(encodeAny(buf, o));
     }
     return bufferWrite(buf, "e", 1);
 
   } else if (PyDict_Check(obj)) {
-    returnIfError(bufferWrite(buf, "d", 1));
-    HPy list = NULL;
-    HPy_ssize_t count = 0;
-    if (buildDictKeyList(obj, &list, &count)) {
-      return 1;
-    }
-
-    if (count == 0) {
-      return bufferWrite(buf, "e", 1);
-    }
-
-    for (HPy_ssize_t i = 0; i < count; i++) {
-      HPy keyValue = PyList_GetItem(list, i); // tuple[bytes, Any]
-
-      if (keyValue == NULL) {
-        runtimeError("failed to get key/value tuple from list");
-        return 1;
-      }
-
-      HPy key = PyTuple_GetItem(keyValue, 0);
-      Py_DecRef(keyValue);
-      if (key == NULL) {
-        runtimeError("can't get key from key,value tuple");
-        return 1;
-      }
-
-      if (encodeBytes(buf, key)) {
-        Py_DecRef(key);
-        return 1;
-      }
+    return encodeDict(buf, obj);
+  }
 
-      HPy value = PyTuple_GetItem(keyValue, 1);
-      if (value == NULL) {
-        runtimeError("can't get value");
-        return 1;
-      }
+  HPy typ = PyObject_Type(obj);
 
-      if (encodeAny(buf, value)) {
-        Py_DecRef(value);
-        return 1;
-      }
-    }
+  if (typ == NULL) {
+    runtimeError("failed to get type of object");
+    return 1;
+  }
 
-    Py_DecRef(list);
-    return bufferWrite(buf, "e", 1);
+  HPy ss = PyUnicode_Format(errTypeMessage, typ);
+  if (ss == NULL) {
+    Py_DecRef(typ);
+    runtimeError("failed to get type of object");
+    return 1;
   }
 
-  HPy typ = PyObject_Type(obj);
+  PyErr_SetObject(PyExc_TypeError, ss);
 
-  PyErr_SetObject(BencodeEncodeError, PyUnicode_Format(PyUnicode_FromString(NON_SUPPORTED_TYPE_MESSAGE), typ));
+  Py_DecRef(ss);
+  Py_DecRef(typ);
 
   return 1;
 }
 
 static HPy bencode(HPy self, HPy obj) {
   // self is the module object
```

### Comparing `bencode_c-0.0.7/src/bencode_c.egg-info/PKG-INFO` & `bencode_c-0.0.8/src/bencode_c.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bencode-c
-Version: 0.0.7
+Version: 0.0.8
 Summary: A fast and correct bencode serialize/deserialize library
 Author-email: trim21 <trim21me@gmail.com>
 License: MIT
 Keywords: bencode,bittorrent,bit-torrent,serialize,deserialize,p2p
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,7 +14,19 @@
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Requires-Dist: pytest==8.2.0; extra == "testing"
 Requires-Dist: pytest-github-actions-annotate-failures==0.2.0; extra == "testing"
 
 bencode serialize/deserialize written in native c extension.
+
+```shell
+pip install bencode-c
+```
+
+```python
+import bencode_c
+
+assert bencode_c.bdecode(b'...') == ...
+
+assert bencode_c.bencode(...) == b'...'
+```
```

### Comparing `bencode_c-0.0.7/tests/test_decode.py` & `bencode_c-0.0.8/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `bencode_c-0.0.7/tests/test_encode.py` & `bencode_c-0.0.8/tests/test_encode.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pytest
 
 from bencode_c import BencodeEncodeError, bencode
 
 
 def test_exception_when_strict():
     invalid_obj = None
-    with pytest.raises(BencodeEncodeError):
+    with pytest.raises(TypeError):
         bencode(invalid_obj)
 
 
 def test_encode_str():
     coded = bencode("ThisIsAString")
     assert coded == b"13:ThisIsAString", "Failed to encode string from str."
```

