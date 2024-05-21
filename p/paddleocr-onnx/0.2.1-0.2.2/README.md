# Comparing `tmp/paddleocr_onnx-0.2.1.tar.gz` & `tmp/paddleocr_onnx-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddleocr_onnx-0.2.1.tar", max compression
+gzip compressed data, was "paddleocr_onnx-0.2.2.tar", max compression
```

## Comparing `paddleocr_onnx-0.2.1.tar` & `paddleocr_onnx-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       60 2024-05-21 05:01:59.373760 paddleocr_onnx-0.2.1/paddleocr_onnx/__init__.py
--rw-r--r--   0        0        0      188 2024-05-21 05:22:32.817415 paddleocr_onnx-0.2.1/paddleocr_onnx/dict/en_dict.txt
--rw-r--r--   0        0        0     1824 2024-05-21 05:45:51.726720 paddleocr_onnx-0.2.1/paddleocr_onnx/imaug/__init__.py
--rw-r--r--   0        0        0    17508 2024-05-21 05:25:34.583033 paddleocr_onnx-0.2.1/paddleocr_onnx/imaug/operators.py
--rw-r--r--   0        0        0        0 2024-05-20 08:55:13.591571 paddleocr_onnx-0.2.1/paddleocr_onnx/infer/__init__.py
--rw-r--r--   0        0        0    10552 2024-05-21 06:09:39.022972 paddleocr_onnx-0.2.1/paddleocr_onnx/infer/predict_det.py
--rw-r--r--   0        0        0     4647 2024-05-21 06:09:46.444869 paddleocr_onnx-0.2.1/paddleocr_onnx/infer/predict_rec.py
--rw-r--r--   0        0        0     3060 2024-05-21 06:09:53.272556 paddleocr_onnx-0.2.1/paddleocr_onnx/infer/predict_system.py
--rw-r--r--   0        0        0    10499 2024-05-20 09:48:14.101563 paddleocr_onnx-0.2.1/paddleocr_onnx/infer/utility.py
--rw-r--r--   0        0        0     5290 2024-05-21 06:09:14.981370 paddleocr_onnx-0.2.1/paddleocr_onnx/paddle_onnx.py
--rw-r--r--   0        0        0      654 2024-05-21 05:37:12.345129 paddleocr_onnx-0.2.1/paddleocr_onnx/postprocess/__init__.py
--rw-r--r--   0        0        0     8759 2024-05-21 05:36:20.900593 paddleocr_onnx-0.2.1/paddleocr_onnx/postprocess/det.py
--rw-r--r--   0        0        0     7491 2024-05-21 05:37:31.727788 paddleocr_onnx-0.2.1/paddleocr_onnx/postprocess/rec.py
--rw-r--r--   0        0        0     3419 2024-05-20 09:35:49.351569 paddleocr_onnx-0.2.1/paddleocr_onnx/ppstructure/utility.py
--rw-r--r--   0        0        0      794 2024-05-21 06:10:46.306440 paddleocr_onnx-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      600 2024-05-21 05:21:44.654987 paddleocr_onnx-0.2.1/README.md
--rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 paddleocr_onnx-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       60 2024-05-21 05:01:59.373760 paddleocr_onnx-0.2.2/paddleocr_onnx/__init__.py
+-rw-r--r--   0        0        0      188 2024-05-21 05:22:32.817415 paddleocr_onnx-0.2.2/paddleocr_onnx/dict/en_dict.txt
+-rw-r--r--   0        0        0     1824 2024-05-21 05:45:51.726720 paddleocr_onnx-0.2.2/paddleocr_onnx/imaug/__init__.py
+-rw-r--r--   0        0        0    17508 2024-05-21 05:25:34.583033 paddleocr_onnx-0.2.2/paddleocr_onnx/imaug/operators.py
+-rw-r--r--   0        0        0        0 2024-05-20 08:55:13.591571 paddleocr_onnx-0.2.2/paddleocr_onnx/infer/__init__.py
+-rw-r--r--   0        0        0    10552 2024-05-21 06:09:39.022972 paddleocr_onnx-0.2.2/paddleocr_onnx/infer/predict_det.py
+-rw-r--r--   0        0        0     4647 2024-05-21 06:09:46.444869 paddleocr_onnx-0.2.2/paddleocr_onnx/infer/predict_rec.py
+-rw-r--r--   0        0        0     3060 2024-05-21 06:09:53.272556 paddleocr_onnx-0.2.2/paddleocr_onnx/infer/predict_system.py
+-rw-r--r--   0        0        0    10499 2024-05-20 09:48:14.101563 paddleocr_onnx-0.2.2/paddleocr_onnx/infer/utility.py
+-rw-r--r--   0        0        0     5290 2024-05-21 06:09:14.981370 paddleocr_onnx-0.2.2/paddleocr_onnx/paddle_onnx.py
+-rw-r--r--   0        0        0      654 2024-05-21 05:37:12.345129 paddleocr_onnx-0.2.2/paddleocr_onnx/postprocess/__init__.py
+-rw-r--r--   0        0        0     8759 2024-05-21 05:36:20.900593 paddleocr_onnx-0.2.2/paddleocr_onnx/postprocess/det.py
+-rw-r--r--   0        0        0     7491 2024-05-21 05:37:31.727788 paddleocr_onnx-0.2.2/paddleocr_onnx/postprocess/rec.py
+-rw-r--r--   0        0        0     3449 2024-05-21 06:11:50.858223 paddleocr_onnx-0.2.2/paddleocr_onnx/ppstructure/utility.py
+-rw-r--r--   0        0        0      794 2024-05-21 06:12:16.042600 paddleocr_onnx-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      600 2024-05-21 05:21:44.654987 paddleocr_onnx-0.2.2/README.md
+-rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 paddleocr_onnx-0.2.2/PKG-INFO
```

### Comparing `paddleocr_onnx-0.2.1/paddleocr_onnx/imaug/__init__.py` & `paddleocr_onnx-0.2.2/paddleocr_onnx/imaug/__init__.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.1/paddleocr_onnx/imaug/operators.py` & `paddleocr_onnx-0.2.2/paddleocr_onnx/imaug/operators.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.1/paddleocr_onnx/infer/predict_det.py` & `paddleocr_onnx-0.2.2/paddleocr_onnx/infer/predict_det.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.1/paddleocr_onnx/infer/predict_rec.py` & `paddleocr_onnx-0.2.2/paddleocr_onnx/infer/predict_rec.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.1/paddleocr_onnx/infer/predict_system.py` & `paddleocr_onnx-0.2.2/paddleocr_onnx/infer/predict_system.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.1/paddleocr_onnx/infer/utility.py` & `paddleocr_onnx-0.2.2/paddleocr_onnx/infer/utility.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.1/paddleocr_onnx/paddle_onnx.py` & `paddleocr_onnx-0.2.2/paddleocr_onnx/paddle_onnx.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.1/paddleocr_onnx/postprocess/__init__.py` & `paddleocr_onnx-0.2.2/paddleocr_onnx/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.1/paddleocr_onnx/postprocess/det.py` & `paddleocr_onnx-0.2.2/paddleocr_onnx/postprocess/det.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.1/paddleocr_onnx/postprocess/rec.py` & `paddleocr_onnx-0.2.2/paddleocr_onnx/postprocess/rec.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.1/paddleocr_onnx/ppstructure/utility.py` & `paddleocr_onnx-0.2.2/paddleocr_onnx/ppstructure/utility.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from infer.utility import init_args as infer_args
-from infer.utility import str2bool, str2int_tuple
+from paddleocr_onnx.infer.utility import init_args as infer_args
+from paddleocr_onnx.infer.utility import str2bool, str2int_tuple
 
 
 def init_args():
     parser = infer_args()
 
     # params for output
     parser.add_argument("--output", type=str, default="./output")
```

### Comparing `paddleocr_onnx-0.2.1/pyproject.toml` & `paddleocr_onnx-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paddleocr-onnx"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["The Walnut AI <support@thewalnut.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.9,<3.13"
 numpy = "^1.26.4"
```

### Comparing `paddleocr_onnx-0.2.1/README.md` & `paddleocr_onnx-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.1/PKG-INFO` & `paddleocr_onnx-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddleocr-onnx
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: The Walnut AI
 Author-email: support@thewalnut.ai
 Requires-Python: >3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

