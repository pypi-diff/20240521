# Comparing `tmp/paddleocr_onnx-0.1.0.tar.gz` & `tmp/paddleocr_onnx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddleocr_onnx-0.1.0.tar", max compression
+gzip compressed data, was "paddleocr_onnx-0.2.0.tar", max compression
```

## Comparing `paddleocr_onnx-0.1.0.tar` & `paddleocr_onnx-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       60 2024-05-21 05:01:59.373760 paddleocr_onnx-0.1.0/paddleocr_onnx/__init__.py
--rw-r--r--   0        0        0      188 2024-05-21 05:22:32.817415 paddleocr_onnx-0.1.0/paddleocr_onnx/dict/en_dict.txt
--rw-r--r--   0        0        0     1824 2024-05-21 05:45:51.726720 paddleocr_onnx-0.1.0/paddleocr_onnx/imaug/__init__.py
--rw-r--r--   0        0        0    17508 2024-05-21 05:25:34.583033 paddleocr_onnx-0.1.0/paddleocr_onnx/imaug/operators.py
--rw-r--r--   0        0        0        0 2024-05-20 08:55:13.591571 paddleocr_onnx-0.1.0/paddleocr_onnx/infer/__init__.py
--rw-r--r--   0        0        0    10507 2024-05-20 10:12:57.911563 paddleocr_onnx-0.1.0/paddleocr_onnx/infer/predict_det.py
--rw-r--r--   0        0        0     4617 2024-05-20 08:43:37.271574 paddleocr_onnx-0.1.0/paddleocr_onnx/infer/predict_rec.py
--rw-r--r--   0        0        0     3015 2024-05-21 05:36:53.523954 paddleocr_onnx-0.1.0/paddleocr_onnx/infer/predict_system.py
--rw-r--r--   0        0        0    10499 2024-05-20 09:48:14.101563 paddleocr_onnx-0.1.0/paddleocr_onnx/infer/utility.py
--rw-r--r--   0        0        0     5245 2024-05-20 09:48:45.561566 paddleocr_onnx-0.1.0/paddleocr_onnx/paddle_onnx.py
--rw-r--r--   0        0        0      654 2024-05-21 05:37:12.345129 paddleocr_onnx-0.1.0/paddleocr_onnx/postprocess/__init__.py
--rw-r--r--   0        0        0     8759 2024-05-21 05:36:20.900593 paddleocr_onnx-0.1.0/paddleocr_onnx/postprocess/det.py
--rw-r--r--   0        0        0     7491 2024-05-21 05:37:31.727788 paddleocr_onnx-0.1.0/paddleocr_onnx/postprocess/rec.py
--rw-r--r--   0        0        0     3419 2024-05-20 09:35:49.351569 paddleocr_onnx-0.1.0/paddleocr_onnx/ppstructure/utility.py
--rw-r--r--   0        0        0      795 2024-05-21 05:53:01.561241 paddleocr_onnx-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      600 2024-05-21 05:21:44.654987 paddleocr_onnx-0.1.0/README.md
--rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 paddleocr_onnx-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       60 2024-05-21 05:01:59.373760 paddleocr_onnx-0.2.0/paddleocr_onnx/__init__.py
+-rw-r--r--   0        0        0      188 2024-05-21 05:22:32.817415 paddleocr_onnx-0.2.0/paddleocr_onnx/dict/en_dict.txt
+-rw-r--r--   0        0        0     1824 2024-05-21 05:45:51.726720 paddleocr_onnx-0.2.0/paddleocr_onnx/imaug/__init__.py
+-rw-r--r--   0        0        0    17508 2024-05-21 05:25:34.583033 paddleocr_onnx-0.2.0/paddleocr_onnx/imaug/operators.py
+-rw-r--r--   0        0        0        0 2024-05-20 08:55:13.591571 paddleocr_onnx-0.2.0/paddleocr_onnx/infer/__init__.py
+-rw-r--r--   0        0        0    10507 2024-05-20 10:12:57.911563 paddleocr_onnx-0.2.0/paddleocr_onnx/infer/predict_det.py
+-rw-r--r--   0        0        0     4617 2024-05-20 08:43:37.271574 paddleocr_onnx-0.2.0/paddleocr_onnx/infer/predict_rec.py
+-rw-r--r--   0        0        0     3015 2024-05-21 05:36:53.523954 paddleocr_onnx-0.2.0/paddleocr_onnx/infer/predict_system.py
+-rw-r--r--   0        0        0    10499 2024-05-20 09:48:14.101563 paddleocr_onnx-0.2.0/paddleocr_onnx/infer/utility.py
+-rw-r--r--   0        0        0     5245 2024-05-20 09:48:45.561566 paddleocr_onnx-0.2.0/paddleocr_onnx/paddle_onnx.py
+-rw-r--r--   0        0        0      654 2024-05-21 05:37:12.345129 paddleocr_onnx-0.2.0/paddleocr_onnx/postprocess/__init__.py
+-rw-r--r--   0        0        0     8759 2024-05-21 05:36:20.900593 paddleocr_onnx-0.2.0/paddleocr_onnx/postprocess/det.py
+-rw-r--r--   0        0        0     7491 2024-05-21 05:37:31.727788 paddleocr_onnx-0.2.0/paddleocr_onnx/postprocess/rec.py
+-rw-r--r--   0        0        0     3419 2024-05-20 09:35:49.351569 paddleocr_onnx-0.2.0/paddleocr_onnx/ppstructure/utility.py
+-rw-r--r--   0        0        0      794 2024-05-21 05:58:31.992489 paddleocr_onnx-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      600 2024-05-21 05:21:44.654987 paddleocr_onnx-0.2.0/README.md
+-rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 paddleocr_onnx-0.2.0/PKG-INFO
```

### Comparing `paddleocr_onnx-0.1.0/paddleocr_onnx/imaug/__init__.py` & `paddleocr_onnx-0.2.0/paddleocr_onnx/imaug/__init__.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.1.0/paddleocr_onnx/imaug/operators.py` & `paddleocr_onnx-0.2.0/paddleocr_onnx/imaug/operators.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.1.0/paddleocr_onnx/infer/predict_det.py` & `paddleocr_onnx-0.2.0/paddleocr_onnx/infer/predict_det.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.1.0/paddleocr_onnx/infer/predict_rec.py` & `paddleocr_onnx-0.2.0/paddleocr_onnx/infer/predict_rec.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.1.0/paddleocr_onnx/infer/predict_system.py` & `paddleocr_onnx-0.2.0/paddleocr_onnx/infer/predict_system.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.1.0/paddleocr_onnx/infer/utility.py` & `paddleocr_onnx-0.2.0/paddleocr_onnx/infer/utility.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.1.0/paddleocr_onnx/paddle_onnx.py` & `paddleocr_onnx-0.2.0/paddleocr_onnx/paddle_onnx.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.1.0/paddleocr_onnx/postprocess/__init__.py` & `paddleocr_onnx-0.2.0/paddleocr_onnx/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.1.0/paddleocr_onnx/postprocess/det.py` & `paddleocr_onnx-0.2.0/paddleocr_onnx/postprocess/det.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.1.0/paddleocr_onnx/postprocess/rec.py` & `paddleocr_onnx-0.2.0/paddleocr_onnx/postprocess/rec.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.1.0/paddleocr_onnx/ppstructure/utility.py` & `paddleocr_onnx-0.2.0/paddleocr_onnx/ppstructure/utility.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.1.0/pyproject.toml` & `paddleocr_onnx-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "paddleocr-onnx"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["The Walnut AI <support@thewalnut.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">3.10,<3.13"
+python = ">3.9,<3.13"
 numpy = "^1.26.4"
 pyclipper = "^1.3.0.post5"
 shapely = "^2.0.4"
 opencv-python-headless = "^4.9.0.80"
 onnxruntime = "^1.18.0"
 six = "^1.16.0"
 pillow = "^10.3.0"
```

### Comparing `paddleocr_onnx-0.1.0/README.md` & `paddleocr_onnx-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.1.0/PKG-INFO` & `paddleocr_onnx-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: paddleocr-onnx
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: The Walnut AI
 Author-email: support@thewalnut.ai
-Requires-Python: >3.10,<3.13
+Requires-Python: >3.9,<3.13
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: onnxruntime (>=1.18.0,<2.0.0)
 Requires-Dist: opencv-python-headless (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: pyclipper (>=1.3.0.post5,<2.0.0)
```

