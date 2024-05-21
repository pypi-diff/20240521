# Comparing `tmp/paddleocr_onnx-0.4.2.tar.gz` & `tmp/paddleocr_onnx-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddleocr_onnx-0.4.2.tar", max compression
+gzip compressed data, was "paddleocr_onnx-0.5.0.tar", max compression
```

## Comparing `paddleocr_onnx-0.4.2.tar` & `paddleocr_onnx-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       60 2024-05-21 05:01:59.373760 paddleocr_onnx-0.4.2/paddleocr_onnx/__init__.py
--rw-r--r--   0        0        0      284 2024-05-21 06:47:21.579416 paddleocr_onnx-0.4.2/paddleocr_onnx/dict/en_dict.txt
--rw-r--r--   0        0        0     1824 2024-05-21 05:45:51.726720 paddleocr_onnx-0.4.2/paddleocr_onnx/imaug/__init__.py
--rw-r--r--   0        0        0    17508 2024-05-21 05:25:34.583033 paddleocr_onnx-0.4.2/paddleocr_onnx/imaug/operators.py
--rw-r--r--   0        0        0        0 2024-05-20 08:55:13.591571 paddleocr_onnx-0.4.2/paddleocr_onnx/infer/__init__.py
--rw-r--r--   0        0        0    10552 2024-05-21 06:09:39.022972 paddleocr_onnx-0.4.2/paddleocr_onnx/infer/predict_det.py
--rw-r--r--   0        0        0     4647 2024-05-21 06:09:46.444869 paddleocr_onnx-0.4.2/paddleocr_onnx/infer/predict_rec.py
--rw-r--r--   0        0        0     3060 2024-05-21 06:09:53.272556 paddleocr_onnx-0.4.2/paddleocr_onnx/infer/predict_system.py
--rw-r--r--   0        0        0    10498 2024-05-21 06:22:28.006395 paddleocr_onnx-0.4.2/paddleocr_onnx/infer/utility.py
--rw-r--r--   0        0        0  2434538 2024-05-20 10:51:56.581559 paddleocr_onnx-0.4.2/paddleocr_onnx/models/en_PP-OCRv3_det_infer.onnx
--rw-r--r--   0        0        0  7992123 2024-05-20 10:52:05.601559 paddleocr_onnx-0.4.2/paddleocr_onnx/models/en_PP-OCRv4_rec_infer.onnx
--rw-r--r--   0        0        0     5506 2024-05-21 06:30:10.633223 paddleocr_onnx-0.4.2/paddleocr_onnx/paddle_onnx.py
--rw-r--r--   0        0        0      654 2024-05-21 05:37:12.345129 paddleocr_onnx-0.4.2/paddleocr_onnx/postprocess/__init__.py
--rw-r--r--   0        0        0     8759 2024-05-21 05:36:20.900593 paddleocr_onnx-0.4.2/paddleocr_onnx/postprocess/det.py
--rw-r--r--   0        0        0     7491 2024-05-21 06:41:36.562411 paddleocr_onnx-0.4.2/paddleocr_onnx/postprocess/rec.py
--rw-r--r--   0        0        0     3449 2024-05-21 06:11:50.858223 paddleocr_onnx-0.4.2/paddleocr_onnx/ppstructure/utility.py
--rw-r--r--   0        0        0      794 2024-05-21 06:48:08.189811 paddleocr_onnx-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      600 2024-05-21 05:21:44.654987 paddleocr_onnx-0.4.2/README.md
--rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 paddleocr_onnx-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0       60 2024-05-21 05:01:59.373760 paddleocr_onnx-0.5.0/paddleocr_onnx/__init__.py
+-rw-r--r--   0        0        0      284 2024-05-21 06:47:21.579416 paddleocr_onnx-0.5.0/paddleocr_onnx/dict/en_dict.txt
+-rw-r--r--   0        0        0     1824 2024-05-21 05:45:51.726720 paddleocr_onnx-0.5.0/paddleocr_onnx/imaug/__init__.py
+-rw-r--r--   0        0        0    17508 2024-05-21 05:25:34.583033 paddleocr_onnx-0.5.0/paddleocr_onnx/imaug/operators.py
+-rw-r--r--   0        0        0        0 2024-05-20 08:55:13.591571 paddleocr_onnx-0.5.0/paddleocr_onnx/infer/__init__.py
+-rw-r--r--   0        0        0    10552 2024-05-21 06:09:39.022972 paddleocr_onnx-0.5.0/paddleocr_onnx/infer/predict_det.py
+-rw-r--r--   0        0        0     4647 2024-05-21 06:09:46.444869 paddleocr_onnx-0.5.0/paddleocr_onnx/infer/predict_rec.py
+-rw-r--r--   0        0        0     3060 2024-05-21 06:09:53.272556 paddleocr_onnx-0.5.0/paddleocr_onnx/infer/predict_system.py
+-rw-r--r--   0        0        0    10498 2024-05-21 06:22:28.006395 paddleocr_onnx-0.5.0/paddleocr_onnx/infer/utility.py
+-rw-r--r--   0        0        0  2434538 2024-05-20 10:51:56.581559 paddleocr_onnx-0.5.0/paddleocr_onnx/models/en_PP-OCRv3_det_infer.onnx
+-rw-r--r--   0        0        0  7992123 2024-05-20 10:52:05.601559 paddleocr_onnx-0.5.0/paddleocr_onnx/models/en_PP-OCRv4_rec_infer.onnx
+-rw-r--r--   0        0        0     5506 2024-05-21 06:30:10.633223 paddleocr_onnx-0.5.0/paddleocr_onnx/paddle_onnx.py
+-rw-r--r--   0        0        0      654 2024-05-21 05:37:12.345129 paddleocr_onnx-0.5.0/paddleocr_onnx/postprocess/__init__.py
+-rw-r--r--   0        0        0     8759 2024-05-21 05:36:20.900593 paddleocr_onnx-0.5.0/paddleocr_onnx/postprocess/det.py
+-rw-r--r--   0        0        0     7491 2024-05-21 06:41:36.562411 paddleocr_onnx-0.5.0/paddleocr_onnx/postprocess/rec.py
+-rw-r--r--   0        0        0     3449 2024-05-21 06:11:50.858223 paddleocr_onnx-0.5.0/paddleocr_onnx/ppstructure/utility.py
+-rw-r--r--   0        0        0      769 2024-05-21 07:13:41.260159 paddleocr_onnx-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      600 2024-05-21 05:21:44.654987 paddleocr_onnx-0.5.0/README.md
+-rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 paddleocr_onnx-0.5.0/PKG-INFO
```

### Comparing `paddleocr_onnx-0.4.2/paddleocr_onnx/imaug/__init__.py` & `paddleocr_onnx-0.5.0/paddleocr_onnx/imaug/__init__.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.4.2/paddleocr_onnx/imaug/operators.py` & `paddleocr_onnx-0.5.0/paddleocr_onnx/imaug/operators.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.4.2/paddleocr_onnx/infer/predict_det.py` & `paddleocr_onnx-0.5.0/paddleocr_onnx/infer/predict_det.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.4.2/paddleocr_onnx/infer/predict_rec.py` & `paddleocr_onnx-0.5.0/paddleocr_onnx/infer/predict_rec.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.4.2/paddleocr_onnx/infer/predict_system.py` & `paddleocr_onnx-0.5.0/paddleocr_onnx/infer/predict_system.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.4.2/paddleocr_onnx/infer/utility.py` & `paddleocr_onnx-0.5.0/paddleocr_onnx/infer/utility.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.4.2/paddleocr_onnx/models/en_PP-OCRv3_det_infer.onnx` & `paddleocr_onnx-0.5.0/paddleocr_onnx/models/en_PP-OCRv3_det_infer.onnx`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.4.2/paddleocr_onnx/models/en_PP-OCRv4_rec_infer.onnx` & `paddleocr_onnx-0.5.0/paddleocr_onnx/models/en_PP-OCRv4_rec_infer.onnx`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.4.2/paddleocr_onnx/paddle_onnx.py` & `paddleocr_onnx-0.5.0/paddleocr_onnx/paddle_onnx.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.4.2/paddleocr_onnx/postprocess/__init__.py` & `paddleocr_onnx-0.5.0/paddleocr_onnx/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.4.2/paddleocr_onnx/postprocess/det.py` & `paddleocr_onnx-0.5.0/paddleocr_onnx/postprocess/det.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.4.2/paddleocr_onnx/postprocess/rec.py` & `paddleocr_onnx-0.5.0/paddleocr_onnx/postprocess/rec.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.4.2/paddleocr_onnx/ppstructure/utility.py` & `paddleocr_onnx-0.5.0/paddleocr_onnx/ppstructure/utility.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.4.2/pyproject.toml` & `paddleocr_onnx-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "paddleocr-onnx"
-version = "0.4.2"
+version = "0.5.0"
 description = ""
 authors = ["The Walnut AI <support@thewalnut.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.9,<3.13"
 numpy = "^1.26.4"
 pyclipper = "^1.3.0.post5"
 shapely = "^2.0.4"
 opencv-python-headless = "^4.9.0.80"
-onnxruntime = "^1.18.0"
 six = "^1.16.0"
 pillow = "^10.3.0"
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
 black = "^24.4.2"
```

### Comparing `paddleocr_onnx-0.4.2/README.md` & `paddleocr_onnx-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.4.2/PKG-INFO` & `paddleocr_onnx-0.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: paddleocr-onnx
-Version: 0.4.2
+Version: 0.5.0
 Summary: 
 Author: The Walnut AI
 Author-email: support@thewalnut.ai
 Requires-Python: >3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: onnxruntime (>=1.18.0,<2.0.0)
 Requires-Dist: opencv-python-headless (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: pyclipper (>=1.3.0.post5,<2.0.0)
 Requires-Dist: shapely (>=2.0.4,<3.0.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Description-Content-Type: text/markdown
```

