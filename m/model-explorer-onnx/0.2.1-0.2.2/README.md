# Comparing `tmp/model_explorer_onnx-0.2.1.tar.gz` & `tmp/model_explorer_onnx-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_explorer_onnx-0.2.1.tar", last modified: Mon May 20 19:00:56 2024, max compression
+gzip compressed data, was "model_explorer_onnx-0.2.2.tar", last modified: Mon May 20 19:06:08 2024, max compression
```

## Comparing `model_explorer_onnx-0.2.1.tar` & `model_explorer_onnx-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:56.080603 model_explorer_onnx-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-20 19:00:52.000000 model_explorer_onnx-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-20 19:00:56.080603 model_explorer_onnx-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-20 19:00:52.000000 model_explorer_onnx-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-20 19:00:52.000000 model_explorer_onnx-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:00:56.080603 model_explorer_onnx-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:56.076603 model_explorer_onnx-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:56.076603 model_explorer_onnx-0.2.1/src/model_explorer_onnx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:56.080603 model_explorer_onnx-0.2.1/src/model_explorer_onnx/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:52.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-20 19:00:52.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx/bin/onnxvis.py
--rw-r--r--   0 runner    (1001) docker     (127)    21334 2024-05-20 19:00:52.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:56.080603 model_explorer_onnx-0.2.1/src/model_explorer_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-20 19:00:56.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-20 19:00:56.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:00:56.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 19:00:56.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-20 19:00:56.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-20 19:00:56.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:06:08.827177 model_explorer_onnx-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-20 19:06:03.000000 model_explorer_onnx-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-20 19:06:08.827177 model_explorer_onnx-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-20 19:06:03.000000 model_explorer_onnx-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-20 19:06:03.000000 model_explorer_onnx-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:06:08.827177 model_explorer_onnx-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:06:08.823177 model_explorer_onnx-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:06:08.823177 model_explorer_onnx-0.2.2/src/model_explorer_onnx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:06:08.823177 model_explorer_onnx-0.2.2/src/model_explorer_onnx/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:06:03.000000 model_explorer_onnx-0.2.2/src/model_explorer_onnx/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-20 19:06:03.000000 model_explorer_onnx-0.2.2/src/model_explorer_onnx/bin/onnxvis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21335 2024-05-20 19:06:03.000000 model_explorer_onnx-0.2.2/src/model_explorer_onnx/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:06:08.823177 model_explorer_onnx-0.2.2/src/model_explorer_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-20 19:06:08.000000 model_explorer_onnx-0.2.2/src/model_explorer_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-20 19:06:08.000000 model_explorer_onnx-0.2.2/src/model_explorer_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:06:08.000000 model_explorer_onnx-0.2.2/src/model_explorer_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 19:06:08.000000 model_explorer_onnx-0.2.2/src/model_explorer_onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-20 19:06:08.000000 model_explorer_onnx-0.2.2/src/model_explorer_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-20 19:06:08.000000 model_explorer_onnx-0.2.2/src/model_explorer_onnx.egg-info/top_level.txt
```

### Comparing `model_explorer_onnx-0.2.1/LICENSE` & `model_explorer_onnx-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `model_explorer_onnx-0.2.1/PKG-INFO` & `model_explorer_onnx-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.2.1
+Version: 0.2.2
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
 Project-URL: Repository, https://github.com/justinchuby/model-explorer-onnx
 Keywords: onnx,model-explorer,visualization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `model_explorer_onnx-0.2.1/README.md` & `model_explorer_onnx-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `model_explorer_onnx-0.2.1/pyproject.toml` & `model_explorer_onnx-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-explorer-onnx"
-version = "0.2.1"
+version = "0.2.2"
 description = "Adapter for ai-edge-model-explorer to support ONNX models"
 authors = [{ name = "Justin Chu", email = "justinchu@microsoft.com" }]
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 keywords = ["onnx", "model-explorer", "visualization"]
 classifiers = [
```

### Comparing `model_explorer_onnx-0.2.1/src/model_explorer_onnx/main.py` & `model_explorer_onnx-0.2.2/src/model_explorer_onnx/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     return True
 
 
 def display_tensor_json(tensor: ir.TensorProtocol | None, settings: Settings) -> str:
     try:
         array = _tensor_to_numpy(tensor)
         size_limit = settings.const_element_count_limit
-        if size_limit < 0 or size_limit > array.size:
+        if size_limit < 0 or size_limit >= array.size:
             # Use separators=(',', ':') to remove spaces
             return json.dumps(array.tolist(), separators=(",", ":"))
         # Show the first `size_limit` elements if the tensor is too large
         return json.dumps(
             (array.flatten())[:size_limit].tolist(), separators=(",", ":")
         )
     except Exception as e:
```

### Comparing `model_explorer_onnx-0.2.1/src/model_explorer_onnx.egg-info/PKG-INFO` & `model_explorer_onnx-0.2.2/src/model_explorer_onnx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.2.1
+Version: 0.2.2
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
 Project-URL: Repository, https://github.com/justinchuby/model-explorer-onnx
 Keywords: onnx,model-explorer,visualization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

