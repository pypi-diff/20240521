# Comparing `tmp/paddleocr_onnx-0.2.0.tar.gz` & `tmp/paddleocr_onnx-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddleocr_onnx-0.2.0.tar", max compression
+gzip compressed data, was "paddleocr_onnx-0.2.1.tar", max compression
```

## Comparing `paddleocr_onnx-0.2.0.tar` & `paddleocr_onnx-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       60 2024-05-21 05:01:59.373760 paddleocr_onnx-0.2.0/paddleocr_onnx/__init__.py
--rw-r--r--   0        0        0      188 2024-05-21 05:22:32.817415 paddleocr_onnx-0.2.0/paddleocr_onnx/dict/en_dict.txt
--rw-r--r--   0        0        0     1824 2024-05-21 05:45:51.726720 paddleocr_onnx-0.2.0/paddleocr_onnx/imaug/__init__.py
--rw-r--r--   0        0        0    17508 2024-05-21 05:25:34.583033 paddleocr_onnx-0.2.0/paddleocr_onnx/imaug/operators.py
--rw-r--r--   0        0        0        0 2024-05-20 08:55:13.591571 paddleocr_onnx-0.2.0/paddleocr_onnx/infer/__init__.py
--rw-r--r--   0        0        0    10507 2024-05-20 10:12:57.911563 paddleocr_onnx-0.2.0/paddleocr_onnx/infer/predict_det.py
--rw-r--r--   0        0        0     4617 2024-05-20 08:43:37.271574 paddleocr_onnx-0.2.0/paddleocr_onnx/infer/predict_rec.py
--rw-r--r--   0        0        0     3015 2024-05-21 05:36:53.523954 paddleocr_onnx-0.2.0/paddleocr_onnx/infer/predict_system.py
--rw-r--r--   0        0        0    10499 2024-05-20 09:48:14.101563 paddleocr_onnx-0.2.0/paddleocr_onnx/infer/utility.py
--rw-r--r--   0        0        0     5245 2024-05-20 09:48:45.561566 paddleocr_onnx-0.2.0/paddleocr_onnx/paddle_onnx.py
--rw-r--r--   0        0        0      654 2024-05-21 05:37:12.345129 paddleocr_onnx-0.2.0/paddleocr_onnx/postprocess/__init__.py
--rw-r--r--   0        0        0     8759 2024-05-21 05:36:20.900593 paddleocr_onnx-0.2.0/paddleocr_onnx/postprocess/det.py
--rw-r--r--   0        0        0     7491 2024-05-21 05:37:31.727788 paddleocr_onnx-0.2.0/paddleocr_onnx/postprocess/rec.py
--rw-r--r--   0        0        0     3419 2024-05-20 09:35:49.351569 paddleocr_onnx-0.2.0/paddleocr_onnx/ppstructure/utility.py
--rw-r--r--   0        0        0      794 2024-05-21 05:58:31.992489 paddleocr_onnx-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      600 2024-05-21 05:21:44.654987 paddleocr_onnx-0.2.0/README.md
--rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 paddleocr_onnx-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       60 2024-05-21 05:01:59.373760 paddleocr_onnx-0.2.1/paddleocr_onnx/__init__.py
+-rw-r--r--   0        0        0      188 2024-05-21 05:22:32.817415 paddleocr_onnx-0.2.1/paddleocr_onnx/dict/en_dict.txt
+-rw-r--r--   0        0        0     1824 2024-05-21 05:45:51.726720 paddleocr_onnx-0.2.1/paddleocr_onnx/imaug/__init__.py
+-rw-r--r--   0        0        0    17508 2024-05-21 05:25:34.583033 paddleocr_onnx-0.2.1/paddleocr_onnx/imaug/operators.py
+-rw-r--r--   0        0        0        0 2024-05-20 08:55:13.591571 paddleocr_onnx-0.2.1/paddleocr_onnx/infer/__init__.py
+-rw-r--r--   0        0        0    10552 2024-05-21 06:09:39.022972 paddleocr_onnx-0.2.1/paddleocr_onnx/infer/predict_det.py
+-rw-r--r--   0        0        0     4647 2024-05-21 06:09:46.444869 paddleocr_onnx-0.2.1/paddleocr_onnx/infer/predict_rec.py
+-rw-r--r--   0        0        0     3060 2024-05-21 06:09:53.272556 paddleocr_onnx-0.2.1/paddleocr_onnx/infer/predict_system.py
+-rw-r--r--   0        0        0    10499 2024-05-20 09:48:14.101563 paddleocr_onnx-0.2.1/paddleocr_onnx/infer/utility.py
+-rw-r--r--   0        0        0     5290 2024-05-21 06:09:14.981370 paddleocr_onnx-0.2.1/paddleocr_onnx/paddle_onnx.py
+-rw-r--r--   0        0        0      654 2024-05-21 05:37:12.345129 paddleocr_onnx-0.2.1/paddleocr_onnx/postprocess/__init__.py
+-rw-r--r--   0        0        0     8759 2024-05-21 05:36:20.900593 paddleocr_onnx-0.2.1/paddleocr_onnx/postprocess/det.py
+-rw-r--r--   0        0        0     7491 2024-05-21 05:37:31.727788 paddleocr_onnx-0.2.1/paddleocr_onnx/postprocess/rec.py
+-rw-r--r--   0        0        0     3419 2024-05-20 09:35:49.351569 paddleocr_onnx-0.2.1/paddleocr_onnx/ppstructure/utility.py
+-rw-r--r--   0        0        0      794 2024-05-21 06:10:46.306440 paddleocr_onnx-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      600 2024-05-21 05:21:44.654987 paddleocr_onnx-0.2.1/README.md
+-rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 paddleocr_onnx-0.2.1/PKG-INFO
```

### Comparing `paddleocr_onnx-0.2.0/paddleocr_onnx/imaug/__init__.py` & `paddleocr_onnx-0.2.1/paddleocr_onnx/imaug/__init__.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.0/paddleocr_onnx/imaug/operators.py` & `paddleocr_onnx-0.2.1/paddleocr_onnx/imaug/operators.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.0/paddleocr_onnx/infer/predict_det.py` & `paddleocr_onnx-0.2.1/paddleocr_onnx/infer/predict_det.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import time
 
 import numpy as np
 
-import infer.utility as utility
-from imaug import create_operators, transform
-from postprocess import build_post_process
+import paddleocr_onnx.infer.utility as utility
+from paddleocr_onnx.imaug import create_operators, transform
+from paddleocr_onnx.postprocess import build_post_process
 
 
 class TextDetector(object):
     def __init__(self, args):
         self.args = args
         self.det_algorithm = args.det_algorithm
         self.use_onnx = args.use_onnx
```

### Comparing `paddleocr_onnx-0.2.0/paddleocr_onnx/infer/predict_rec.py` & `paddleocr_onnx-0.2.1/paddleocr_onnx/infer/predict_rec.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # limitations under the License.
 import math
 import time
 
 import cv2
 import numpy as np
 
-import infer.utility as utility
-from postprocess import build_post_process
+import paddleocr_onnx.infer.utility as utility
+from paddleocr_onnx.postprocess import build_post_process
 
 
 class TextRecognizer(object):
     def __init__(self, args):
         self.rec_image_shape = [int(v) for v in args.rec_image_shape.split(",")]
         self.rec_batch_num = args.rec_batch_num
         self.rec_algorithm = args.rec_algorithm
```

### Comparing `paddleocr_onnx-0.2.0/paddleocr_onnx/infer/predict_system.py` & `paddleocr_onnx-0.2.1/paddleocr_onnx/infer/predict_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 import time
 
-import infer.predict_det as predict_det
-import infer.predict_rec as predict_rec
-from infer.utility import get_rotate_crop_image
+import paddleocr_onnx.infer.predict_det as predict_det
+import paddleocr_onnx.infer.predict_rec as predict_rec
+from paddleocr_onnx.infer.utility import get_rotate_crop_image
 
 
 class TextSystem(object):
     def __init__(self, args):
 
         self.text_detector = predict_det.TextDetector(args)
         self.text_recognizer = predict_rec.TextRecognizer(args)
```

### Comparing `paddleocr_onnx-0.2.0/paddleocr_onnx/infer/utility.py` & `paddleocr_onnx-0.2.1/paddleocr_onnx/infer/utility.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.0/paddleocr_onnx/paddle_onnx.py` & `paddleocr_onnx-0.2.1/paddleocr_onnx/paddle_onnx.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import cv2
 import numpy as np
 
-from infer import predict_system
-from infer.utility import alpha_to_color, binarize_img, str2bool
-from ppstructure.utility import init_args
+from paddleocr_onnx.infer import predict_system
+from paddleocr_onnx.infer.utility import alpha_to_color, binarize_img, str2bool
+from paddleocr_onnx.ppstructure.utility import init_args
 
 
 def parse_args(mMain=True):
     import argparse
 
     parser = init_args()
     parser.add_help = mMain
```

### Comparing `paddleocr_onnx-0.2.0/paddleocr_onnx/postprocess/__init__.py` & `paddleocr_onnx-0.2.1/paddleocr_onnx/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.0/paddleocr_onnx/postprocess/det.py` & `paddleocr_onnx-0.2.1/paddleocr_onnx/postprocess/det.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.0/paddleocr_onnx/postprocess/rec.py` & `paddleocr_onnx-0.2.1/paddleocr_onnx/postprocess/rec.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.0/paddleocr_onnx/ppstructure/utility.py` & `paddleocr_onnx-0.2.1/paddleocr_onnx/ppstructure/utility.py`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.0/pyproject.toml` & `paddleocr_onnx-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paddleocr-onnx"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["The Walnut AI <support@thewalnut.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.9,<3.13"
 numpy = "^1.26.4"
```

### Comparing `paddleocr_onnx-0.2.0/README.md` & `paddleocr_onnx-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `paddleocr_onnx-0.2.0/PKG-INFO` & `paddleocr_onnx-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddleocr-onnx
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: The Walnut AI
 Author-email: support@thewalnut.ai
 Requires-Python: >3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

