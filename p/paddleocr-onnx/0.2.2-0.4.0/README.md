# Comparing `tmp/paddleocr_onnx-0.2.2.tar.gz` & `tmp/paddleocr_onnx-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddleocr_onnx-0.2.2.tar", max compression
+gzip compressed data, was "paddleocr_onnx-0.4.0.tar", max compression
```

## Comparing `paddleocr_onnx-0.2.2.tar` & `paddleocr_onnx-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0       60 2024-05-21 05:01:59.373760 paddleocr_onnx-0.2.2/paddleocr_onnx/__init__.py
--rw-r--r--   0        0        0      188 2024-05-21 05:22:32.817415 paddleocr_onnx-0.2.2/paddleocr_onnx/dict/en_dict.txt
--rw-r--r--   0        0        0     1824 2024-05-21 05:45:51.726720 paddleocr_onnx-0.2.2/paddleocr_onnx/imaug/__init__.py
--rw-r--r--   0        0        0    17508 2024-05-21 05:25:34.583033 paddleocr_onnx-0.2.2/paddleocr_onnx/imaug/operators.py
--rw-r--r--   0        0        0        0 2024-05-20 08:55:13.591571 paddleocr_onnx-0.2.2/paddleocr_onnx/infer/__init__.py
--rw-r--r--   0        0        0    10552 2024-05-21 06:09:39.022972 paddleocr_onnx-0.2.2/paddleocr_onnx/infer/predict_det.py
--rw-r--r--   0        0        0     4647 2024-05-21 06:09:46.444869 paddleocr_onnx-0.2.2/paddleocr_onnx/infer/predict_rec.py
--rw-r--r--   0        0        0     3060 2024-05-21 06:09:53.272556 paddleocr_onnx-0.2.2/paddleocr_onnx/infer/predict_system.py
--rw-r--r--   0        0        0    10499 2024-05-20 09:48:14.101563 paddleocr_onnx-0.2.2/paddleocr_onnx/infer/utility.py
--rw-r--r--   0        0        0     5290 2024-05-21 06:09:14.981370 paddleocr_onnx-0.2.2/paddleocr_onnx/paddle_onnx.py
--rw-r--r--   0        0        0      654 2024-05-21 05:37:12.345129 paddleocr_onnx-0.2.2/paddleocr_onnx/postprocess/__init__.py
--rw-r--r--   0        0        0     8759 2024-05-21 05:36:20.900593 paddleocr_onnx-0.2.2/paddleocr_onnx/postprocess/det.py
--rw-r--r--   0        0        0     7491 2024-05-21 05:37:31.727788 paddleocr_onnx-0.2.2/paddleocr_onnx/postprocess/rec.py
--rw-r--r--   0        0        0     3449 2024-05-21 06:11:50.858223 paddleocr_onnx-0.2.2/paddleocr_onnx/ppstructure/utility.py
--rw-r--r--   0        0        0      794 2024-05-21 06:12:16.042600 paddleocr_onnx-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      600 2024-05-21 05:21:44.654987 paddleocr_onnx-0.2.2/README.md
--rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 paddleocr_onnx-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       60 2024-05-21 05:01:59.373760 paddleocr_onnx-0.4.0/paddleocr_onnx/__init__.py
+-rw-r--r--   0        0        0      188 2024-05-21 05:22:32.817415 paddleocr_onnx-0.4.0/paddleocr_onnx/dict/en_dict.txt
+-rw-r--r--   0        0        0     1824 2024-05-21 05:45:51.726720 paddleocr_onnx-0.4.0/paddleocr_onnx/imaug/__init__.py
+-rw-r--r--   0        0        0    17508 2024-05-21 05:25:34.583033 paddleocr_onnx-0.4.0/paddleocr_onnx/imaug/operators.py
+-rw-r--r--   0        0        0        0 2024-05-20 08:55:13.591571 paddleocr_onnx-0.4.0/paddleocr_onnx/infer/__init__.py
+-rw-r--r--   0        0        0    10552 2024-05-21 06:09:39.022972 paddleocr_onnx-0.4.0/paddleocr_onnx/infer/predict_det.py
+-rw-r--r--   0        0        0     4647 2024-05-21 06:09:46.444869 paddleocr_onnx-0.4.0/paddleocr_onnx/infer/predict_rec.py
+-rw-r--r--   0        0        0     3060 2024-05-21 06:09:53.272556 paddleocr_onnx-0.4.0/paddleocr_onnx/infer/predict_system.py
+-rw-r--r--   0        0        0    10498 2024-05-21 06:22:28.006395 paddleocr_onnx-0.4.0/paddleocr_onnx/infer/utility.py
+-rw-r--r--   0        0        0  2434538 2024-05-20 10:51:56.581559 paddleocr_onnx-0.4.0/paddleocr_onnx/models/en_PP-OCRv3_det_infer.onnx
+-rw-r--r--   0        0        0  7992123 2024-05-20 10:52:05.601559 paddleocr_onnx-0.4.0/paddleocr_onnx/models/en_PP-OCRv4_rec_infer.onnx
+-rw-r--r--   0        0        0     5498 2024-05-21 06:24:49.773089 paddleocr_onnx-0.4.0/paddleocr_onnx/paddle_onnx.py
+-rw-r--r--   0        0        0      654 2024-05-21 05:37:12.345129 paddleocr_onnx-0.4.0/paddleocr_onnx/postprocess/__init__.py
+-rw-r--r--   0        0        0     8759 2024-05-21 05:36:20.900593 paddleocr_onnx-0.4.0/paddleocr_onnx/postprocess/det.py
+-rw-r--r--   0        0        0     7491 2024-05-21 05:37:31.727788 paddleocr_onnx-0.4.0/paddleocr_onnx/postprocess/rec.py
+-rw-r--r--   0        0        0     3449 2024-05-21 06:11:50.858223 paddleocr_onnx-0.4.0/paddleocr_onnx/ppstructure/utility.py
+-rw-r--r--   0        0        0      794 2024-05-21 06:26:02.662850 paddleocr_onnx-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      600 2024-05-21 05:21:44.654987 paddleocr_onnx-0.4.0/README.md
+-rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 paddleocr_onnx-0.4.0/PKG-INFO
```

### Comparing `paddleocr_onnx-0.2.2/paddleocr_onnx/imaug/__init__.py` & `paddleocr_onnx-0.4.0/paddleocr_onnx/imaug/__init__.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.2/paddleocr_onnx/imaug/operators.py` & `paddleocr_onnx-0.4.0/paddleocr_onnx/imaug/operators.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.2/paddleocr_onnx/infer/predict_det.py` & `paddleocr_onnx-0.4.0/paddleocr_onnx/infer/predict_det.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.2/paddleocr_onnx/infer/predict_rec.py` & `paddleocr_onnx-0.4.0/paddleocr_onnx/infer/predict_rec.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.2/paddleocr_onnx/infer/predict_system.py` & `paddleocr_onnx-0.4.0/paddleocr_onnx/infer/predict_system.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.2/paddleocr_onnx/infer/utility.py` & `paddleocr_onnx-0.4.0/paddleocr_onnx/infer/utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     parser.add_argument("--total_process_num", type=int, default=1)
     parser.add_argument("--process_id", type=int, default=0)
 
     parser.add_argument("--benchmark", type=str2bool, default=False)
     parser.add_argument("--save_log_path", type=str, default="./log_output/")
 
     parser.add_argument("--show_log", type=str2bool, default=True)
-    parser.add_argument("--use_onnx", type=str2bool, default=False)
+    parser.add_argument("--use_onnx", type=str2bool, default=True)
 
     # extended function
     parser.add_argument(
         "--return_word_box",
         type=str2bool,
         default=False,
         help="Whether return the bbox of each word (split by space) or chinese character. Only used in ppstructure for layout recovery",
```

### Comparing `paddleocr_onnx-0.2.2/paddleocr_onnx/paddle_onnx.py` & `paddleocr_onnx-0.4.0/paddleocr_onnx/paddle_onnx.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+from pathlib import Path
+
 import cv2
 import numpy as np
 
 from paddleocr_onnx.infer import predict_system
 from paddleocr_onnx.infer.utility import alpha_to_color, binarize_img, str2bool
 from paddleocr_onnx.ppstructure.utility import init_args
 
 
 def parse_args(mMain=True):
     import argparse
 
     parser = init_args()
     parser.add_help = mMain
-    parser.add_argument("--lang", type=str, default="ch")
+    parser.add_argument("--lang", type=str, default="en")
     parser.add_argument("--det", type=str2bool, default=True)
     parser.add_argument("--rec", type=str2bool, default=True)
     parser.add_argument("--type", type=str, default="ocr")
     parser.add_argument("--savefile", type=str2bool, default=False)
     parser.add_argument(
         "--ocr_version",
         type=str,
@@ -76,23 +78,28 @@
         paddleocr package
         args:
             **kwargs: other params show in paddleocr --help
         """
         params = parse_args(mMain=False)
         params.__dict__.update(**kwargs)
 
+        root_dir = Path(__file__).resolve().parent
+
         self.use_angle_cls = params.use_angle_cls
 
-        if params.ocr_version in ["PP-OCRv3", "PP-OCRv4"]:
-            params.rec_image_shape = "3, 48, 320"
-        else:
-            params.rec_image_shape = "3, 32, 320"
+        if params.det_model_dir is None:
+            params.det_model_dir = root_dir / "models/en_PP-OCRv3_det_infer.onnx"
+
+        if params.rec_model_dir is None:
+            params.rec_model_dir = root_dir / "models/en_PP-OCRv4_rec_infer.onnx"
+
+        params.rec_image_shape = "3, 48, 320"
 
         if params.rec_char_dict_path is None:
-            params.rec_char_dict_path = "./dict/en_dict.txt"
+            params.rec_char_dict_path = root_dir / "dict/en_dict.txt"
 
         # init det_model and rec_model
         super().__init__(params)
         self.page_num = params.page_num
 
     def ocr(
         self,
```

### Comparing `paddleocr_onnx-0.2.2/paddleocr_onnx/postprocess/__init__.py` & `paddleocr_onnx-0.4.0/paddleocr_onnx/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.2/paddleocr_onnx/postprocess/det.py` & `paddleocr_onnx-0.4.0/paddleocr_onnx/postprocess/det.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.2/paddleocr_onnx/postprocess/rec.py` & `paddleocr_onnx-0.4.0/paddleocr_onnx/postprocess/rec.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.2/paddleocr_onnx/ppstructure/utility.py` & `paddleocr_onnx-0.4.0/paddleocr_onnx/ppstructure/utility.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.2/pyproject.toml` & `paddleocr_onnx-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paddleocr-onnx"
-version = "0.2.2"
+version = "0.4.0"
 description = ""
 authors = ["The Walnut AI <support@thewalnut.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.9,<3.13"
 numpy = "^1.26.4"
```

### Comparing `paddleocr_onnx-0.2.2/README.md` & `paddleocr_onnx-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.2/PKG-INFO` & `paddleocr_onnx-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddleocr-onnx
-Version: 0.2.2
+Version: 0.4.0
 Summary: 
 Author: The Walnut AI
 Author-email: support@thewalnut.ai
 Requires-Python: >3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

