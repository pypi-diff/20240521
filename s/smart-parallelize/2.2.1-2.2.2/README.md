# Comparing `tmp/smart_parallelize-2.2.1.tar.gz` & `tmp/smart_parallelize-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_parallelize-2.2.1.tar", max compression
+gzip compressed data, was "smart_parallelize-2.2.2.tar", max compression
```

## Comparing `smart_parallelize-2.2.1.tar` & `smart_parallelize-2.2.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      554 2024-05-13 01:37:00.192639 smart_parallelize-2.2.1/README.md
--rw-r--r--   0        0        0      317 2024-05-21 19:46:43.572298 smart_parallelize-2.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.2.1/smart_parallelize/__init__.py
--rw-r--r--   0        0        0     4202 2024-05-21 19:46:31.474437 smart_parallelize-2.2.1/smart_parallelize/parallelize.py
--rw-r--r--   0        0        0     4328 2024-05-21 19:46:36.544808 smart_parallelize-2.2.1/smart_parallelize/parallelize_DEP.py
--rw-r--r--   0        0        0     1824 2024-05-21 19:46:08.870023 smart_parallelize-2.2.1/smart_parallelize/parallelize_native.py
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 smart_parallelize-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0      554 2024-05-13 01:37:00.192639 smart_parallelize-2.2.2/README.md
+-rw-r--r--   0        0        0      317 2024-05-21 20:50:37.878510 smart_parallelize-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.2.2/smart_parallelize/__init__.py
+-rw-r--r--   0        0        0     4202 2024-05-21 19:46:31.474437 smart_parallelize-2.2.2/smart_parallelize/parallelize.py
+-rw-r--r--   0        0        0     4328 2024-05-21 19:46:36.544808 smart_parallelize-2.2.2/smart_parallelize/parallelize_DEP.py
+-rw-r--r--   0        0        0     2232 2024-05-21 20:49:46.010609 smart_parallelize-2.2.2/smart_parallelize/parallelize_native.py
+-rw-r--r--   0        0        0     1089 2024-05-21 20:37:44.902899 smart_parallelize-2.2.2/smart_parallelize/test.py
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 smart_parallelize-2.2.2/PKG-INFO
```

### Comparing `smart_parallelize-2.2.1/README.md` & `smart_parallelize-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `smart_parallelize-2.2.1/smart_parallelize/parallelize.py` & `smart_parallelize-2.2.2/smart_parallelize/parallelize.py`

 * *Files identical despite different names*

### Comparing `smart_parallelize-2.2.1/smart_parallelize/parallelize_DEP.py` & `smart_parallelize-2.2.2/smart_parallelize/parallelize_DEP.py`

 * *Files identical despite different names*

### Comparing `smart_parallelize-2.2.1/smart_parallelize/parallelize_native.py` & `smart_parallelize-2.2.2/smart_parallelize/parallelize_native.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,33 @@
 
 
 # print('testing')
 # sleep(1)
 
 def smart_parallelize(func, args2parallelize, *args):
     args2par = list(args[:args2parallelize])
-    argsnotpar = [list(args[args2parallelize:])*len(args2par[0])]
+    args2par2 = []
+    for i,a in enumerate(args2par[0]):
+        c = []
+        for i in range(args2parallelize):
+            c.append(a)
+        args2par2.append(tuple(c))
+    args2par = args2par2
+    argsnotpar = list(([args[args2parallelize:]]))*len(args2par)
+
     if len(argsnotpar[0]) != 0:
-        inputs = zip(*args2par, *argsnotpar)
+        inputs = [a+argsnotpar[i] for i, a in enumerate(args2par)]
     else:
-        inputs = zip(*args2par)
+        inputs = args2par
+
+    # argsnotpar = [list(args[args2parallelize:])]*len(args2par)
+    # if len(argsnotpar[0]) != 0:
+    #     inputs = zip(*args2par, *argsnotpar)
+    # else:
+    #     inputs = zip(*args2par)
     with Pool() as p:
         out = p.starmap(func, inputs)
     
     if isinstance(out[0], list) or isinstance(out[0], np.ndarray):
         num_outs = 1
         out = np.array(out)
         return out
```

### Comparing `smart_parallelize-2.2.1/PKG-INFO` & `smart_parallelize-2.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-parallelize
-Version: 2.2.1
+Version: 2.2.2
 Summary: 
 Author: Truman DeWalch
 Author-email: trumandewalch@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

