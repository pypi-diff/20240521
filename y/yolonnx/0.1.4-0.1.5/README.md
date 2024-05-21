# Comparing `tmp/yolonnx-0.1.4.tar.gz` & `tmp/yolonnx-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolonnx-0.1.4.tar", last modified: Fri Apr 26 06:32:07 2024, max compression
+gzip compressed data, was "yolonnx-0.1.5.tar", last modified: Tue May 21 10:23:39 2024, max compression
```

## Comparing `yolonnx-0.1.4.tar` & `yolonnx-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1099 2024-04-19 12:11:03.505690 yolonnx-0.1.4/LICENSE
--rw-r--r--   0        0        0     1282 2024-04-22 14:07:07.942295 yolonnx-0.1.4/README.md
--rw-r--r--   0        0        0      738 2024-04-26 06:32:07.143778 yolonnx-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 12:05:13.818667 yolonnx-0.1.4/src/yolonnx/__init__.py
--rw-r--r--   0        0        0      428 2024-04-23 07:40:59.649339 yolonnx-0.1.4/src/yolonnx/model.py
--rw-r--r--   0        0        0     1377 2024-04-22 13:45:27.021530 yolonnx-0.1.4/src/yolonnx/protocols.py
--rw-r--r--   0        0        0      108 2024-04-22 12:06:52.774186 yolonnx-0.1.4/src/yolonnx/services/__init__.py
--rw-r--r--   0        0        0     4106 2024-04-26 06:30:37.837154 yolonnx-0.1.4/src/yolonnx/services/classifier.py
--rw-r--r--   0        0        0     2988 2024-04-23 07:39:11.587139 yolonnx-0.1.4/src/yolonnx/services/detector.py
--rw-r--r--   0        0        0     1364 2024-04-22 13:50:09.339584 yolonnx-0.1.4/src/yolonnx/to_tensor_strategies.py
--rw-r--r--   0        0        0     1569 2024-04-22 12:31:23.751245 yolonnx-0.1.4/src/yolonnx/utils.py
--rw-r--r--   0        0        0        0 2024-04-23 08:14:27.133123 yolonnx-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     1763 1970-01-01 00:00:00.000000 yolonnx-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-04-19 12:11:03.505690 yolonnx-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1282 2024-04-22 14:07:07.942295 yolonnx-0.1.5/README.md
+-rw-r--r--   0        0        0      738 2024-05-21 10:23:39.090707 yolonnx-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-22 12:05:13.818667 yolonnx-0.1.5/src/yolonnx/__init__.py
+-rw-r--r--   0        0        0      428 2024-04-23 07:40:59.649339 yolonnx-0.1.5/src/yolonnx/model.py
+-rw-r--r--   0        0        0     1377 2024-04-22 13:45:27.021530 yolonnx-0.1.5/src/yolonnx/protocols.py
+-rw-r--r--   0        0        0      108 2024-04-22 12:06:52.774186 yolonnx-0.1.5/src/yolonnx/services/__init__.py
+-rw-r--r--   0        0        0     4113 2024-05-21 10:19:38.455509 yolonnx-0.1.5/src/yolonnx/services/classifier.py
+-rw-r--r--   0        0        0     2988 2024-04-23 07:39:11.587139 yolonnx-0.1.5/src/yolonnx/services/detector.py
+-rw-r--r--   0        0        0     1364 2024-04-22 13:50:09.339584 yolonnx-0.1.5/src/yolonnx/to_tensor_strategies.py
+-rw-r--r--   0        0        0     1569 2024-04-22 12:31:23.751245 yolonnx-0.1.5/src/yolonnx/utils.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:14:27.133123 yolonnx-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     1763 1970-01-01 00:00:00.000000 yolonnx-0.1.5/PKG-INFO
```

### Comparing `yolonnx-0.1.4/LICENSE` & `yolonnx-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yolonnx-0.1.4/README.md` & `yolonnx-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `yolonnx-0.1.4/pyproject.toml` & `yolonnx-0.1.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "yolonnx"
-version = "0.1.4"
+version = "0.1.5"
 description = "This package lets you run your YOLOv8 detection and classification models using ONNXRuntime."
 authors = [
     { name = "Kasper Fromm Pedersen", email = "kasperf@cs.aau.dk" },
 ]
 dependencies = [
     "numpy==1.26.*",
     "aau-label==0.2.*",
```

### Comparing `yolonnx-0.1.4/src/yolonnx/protocols.py` & `yolonnx-0.1.5/src/yolonnx/protocols.py`

 * *Files identical despite different names*

### Comparing `yolonnx-0.1.4/src/yolonnx/services/classifier.py` & `yolonnx-0.1.5/src/yolonnx/services/classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         labels_idx = numpy.argwhere(results >= self.threshold)
         scores: NDArray[float32] = results[labels_idx]
 
         rv: list[ClassifierResult] = []
         for i in range(len(labels_idx)):
             id = labels_idx[i][0]
             label_name = self.names[id]
-            rv.append(ClassifierResult(name=label_name, score=scores[i][0]))
+            rv.append(ClassifierResult(name=label_name, score=scores[i][0].item()))
 
         rv.sort(key=lambda x: x.score, reverse=True)
         return rv
 
     def run(self, img: T) -> Sequence[ClassifierResult]:
         """
         Run the classifier on the given image and return a sequence of ClassifierResult objects.
```

### Comparing `yolonnx-0.1.4/src/yolonnx/services/detector.py` & `yolonnx-0.1.5/src/yolonnx/services/detector.py`

 * *Files identical despite different names*

### Comparing `yolonnx-0.1.4/src/yolonnx/to_tensor_strategies.py` & `yolonnx-0.1.5/src/yolonnx/to_tensor_strategies.py`

 * *Files identical despite different names*

### Comparing `yolonnx-0.1.4/src/yolonnx/utils.py` & `yolonnx-0.1.5/src/yolonnx/utils.py`

 * *Files identical despite different names*

### Comparing `yolonnx-0.1.4/PKG-INFO` & `yolonnx-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolonnx
-Version: 0.1.4
+Version: 0.1.5
 Summary: This package lets you run your YOLOv8 detection and classification models using ONNXRuntime.
 Keywords: ONNX,YOLOv8,onnxruntime,vision
 Home-page: https://www.cs.aau.dk/
 Author-Email: Kasper Fromm Pedersen <kasperf@cs.aau.dk>
 License: MIT
 Project-URL: Homepage, https://www.cs.aau.dk/
 Project-URL: Repository, https://github.com/fromm1990/yolonnx
```

