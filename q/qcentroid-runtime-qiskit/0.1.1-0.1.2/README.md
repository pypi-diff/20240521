# Comparing `tmp/qcentroid_runtime_qiskit-0.1.1.tar.gz` & `tmp/qcentroid_runtime_qiskit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcentroid_runtime_qiskit-0.1.1.tar", max compression
+gzip compressed data, was "qcentroid_runtime_qiskit-0.1.2.tar", max compression
```

## Comparing `qcentroid_runtime_qiskit-0.1.1.tar` & `qcentroid_runtime_qiskit-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,12 @@
--rw-r--r--   0        0        0     1298 2024-05-13 18:01:40.271283 qcentroid_runtime_qiskit-0.1.1/LICENSE
--rw-r--r--   0        0        0      970 2024-05-13 18:01:40.271283 qcentroid_runtime_qiskit-0.1.1/README.md
--rw-r--r--   0        0        0     1020 2024-05-13 18:01:40.271283 qcentroid_runtime_qiskit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1010 2024-05-13 18:01:40.271283 qcentroid_runtime_qiskit-0.1.1/qcentroid_runtime_qiskit/__init__.py
--rw-r--r--   0        0        0     1950 1970-01-01 00:00:00.000000 qcentroid_runtime_qiskit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1298 2024-05-21 09:38:16.429004 qcentroid_runtime_qiskit-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1182 2024-05-21 09:38:16.429004 qcentroid_runtime_qiskit-0.1.2/README.md
+-rw-r--r--   0        0        0     1020 2024-05-21 09:38:16.429004 qcentroid_runtime_qiskit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1647 2024-05-21 09:38:16.429004 qcentroid_runtime_qiskit-0.1.2/qcentroid_runtime_qiskit/__init__.py
+-rw-r--r--   0        0        0      832 2024-05-21 09:38:16.429004 qcentroid_runtime_qiskit-0.1.2/qcentroid_runtime_qiskit/providers/IBMCloud.py
+-rw-r--r--   0        0        0      848 2024-05-21 09:38:16.429004 qcentroid_runtime_qiskit-0.1.2/qcentroid_runtime_qiskit/providers/IBMQuantum.py
+-rw-r--r--   0        0        0     1333 2024-05-21 09:38:16.429004 qcentroid_runtime_qiskit-0.1.2/qcentroid_runtime_qiskit/providers/IonQ.py
+-rw-r--r--   0        0        0      865 2024-05-21 09:38:16.429004 qcentroid_runtime_qiskit-0.1.2/qcentroid_runtime_qiskit/providers/QCtrlEmbedded.py
+-rw-r--r--   0        0        0      569 2024-05-21 09:38:16.429004 qcentroid_runtime_qiskit-0.1.2/qcentroid_runtime_qiskit/providers/QiskitAbstractProvider.py
+-rw-r--r--   0        0        0     2570 2024-05-21 09:38:16.429004 qcentroid_runtime_qiskit-0.1.2/qcentroid_runtime_qiskit/providers/QiskitRuntimeAbstractProvider.py
+-rw-r--r--   0        0        0      261 2024-05-21 09:38:16.429004 qcentroid_runtime_qiskit-0.1.2/qcentroid_runtime_qiskit/providers/__init__.py
+-rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 qcentroid_runtime_qiskit-0.1.2/PKG-INFO
```

### Comparing `qcentroid_runtime_qiskit-0.1.1/LICENSE` & `qcentroid_runtime_qiskit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qcentroid_runtime_qiskit-0.1.1/README.md` & `qcentroid_runtime_qiskit-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # qcentroid-runtime-qiskit
 
 ![deploy to pypi](https://github.com/QCentroid/qcentroid-runtime-qiskit/actions/workflows/publish.yml/badge.svg)
 [![Python](https://img.shields.io/pypi/pyversions/qcentroid-runtime-qiskit.svg)](https://badge.fury.io/py/qcentroid-runtime-qiskit)
 [![PyPI](https://badge.fury.io/py/qcentroid-runtime-qiskit.svg)](https://badge.fury.io/py/qcentroid-runtime-qiskit)
+ [![CodeFactor](https://www.codefactor.io/repository/github/qcentroid/qcentroid-runtime-qiskit/badge)](https://www.codefactor.io/repository/github/qcentroid/qcentroid-runtime-qiskit)
+
  
 QCentroid library to interact with Qiskit
 
 
 
 
 ## Install
@@ -22,22 +24,23 @@
 
 As easy as this:
 
 ```python
 from qcentroid_runtime_qiskit import QCentroidRuntimeQiskit
 import logging
 
-logging.basicConfig(level=logging.DEBUG)
+logger = logging.getLogger(__name__)
 
 def main():
     
     # Get the solver details
-    qcentroid_qiskit = QCentroidRuntimeQiskit.get_instance() # with optional params
+    QCentroidRuntimeQiskit.get_instance() # with optional params
 
-    print(f"currentVersion:{QCentroidRuntimeQiskit.getVersion()}")
+    logger.info(f"currentVersion:{QCentroidRuntimeQiskit.getVersion()}")
     QCentroidRuntimeQiskit.execute(circuit)
     
     
 if __name__ == "__main__":
+    logging.basicConfig(level=logging.DEBUG)
     main() 
 ```
```

### Comparing `qcentroid_runtime_qiskit-0.1.1/pyproject.toml` & `qcentroid_runtime_qiskit-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2271 6365 6e74 726f 6964  ame = "qcentroid
 00000020: 2d72 756e 7469 6d65 2d71 6973 6b69 7422  -runtime-qiskit"
 00000030: 0d0a 7665 7273 696f 6e20 3d20 2230 2e31  ..version = "0.1
-00000040: 2e31 220d 0a64 6573 6372 6970 7469 6f6e  .1"..description
+00000040: 2e32 220d 0a64 6573 6372 6970 7469 6f6e  .2"..description
 00000050: 203d 2022 4c69 6272 6172 7920 746f 2069   = "Library to i
 00000060: 6e74 6572 6163 7420 7769 7468 2071 6365  nteract with qce
 00000070: 6e74 726f 6964 2071 6973 6b69 7420 7275  ntroid qiskit ru
 00000080: 6e74 696d 6522 0d0a 6175 7468 6f72 7320  ntime"..authors 
 00000090: 3d20 5b0d 0a20 2022 5143 656e 7472 6f69  = [..  "QCentroi
 000000a0: 6420 3c69 6e66 6f40 7163 656e 7472 6f69  d <info@qcentroi
 000000b0: 642e 7879 7a3e 2220 5d0d 0a63 6c61 7373  d.xyz>" ]..class
```

### Comparing `qcentroid_runtime_qiskit-0.1.1/PKG-INFO` & `qcentroid_runtime_qiskit-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcentroid-runtime-qiskit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library to interact with qcentroid qiskit runtime
 Home-page: https://www.qcentroid.xyz
 License: MIT
 Author: QCentroid
 Author-email: info@qcentroid.xyz
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -23,14 +23,16 @@
 Description-Content-Type: text/markdown
 
 # qcentroid-runtime-qiskit
 
 ![deploy to pypi](https://github.com/QCentroid/qcentroid-runtime-qiskit/actions/workflows/publish.yml/badge.svg)
 [![Python](https://img.shields.io/pypi/pyversions/qcentroid-runtime-qiskit.svg)](https://badge.fury.io/py/qcentroid-runtime-qiskit)
 [![PyPI](https://badge.fury.io/py/qcentroid-runtime-qiskit.svg)](https://badge.fury.io/py/qcentroid-runtime-qiskit)
+ [![CodeFactor](https://www.codefactor.io/repository/github/qcentroid/qcentroid-runtime-qiskit/badge)](https://www.codefactor.io/repository/github/qcentroid/qcentroid-runtime-qiskit)
+
  
 QCentroid library to interact with Qiskit
 
 
 
 
 ## Install
@@ -46,23 +48,24 @@
 
 As easy as this:
 
 ```python
 from qcentroid_runtime_qiskit import QCentroidRuntimeQiskit
 import logging
 
-logging.basicConfig(level=logging.DEBUG)
+logger = logging.getLogger(__name__)
 
 def main():
     
     # Get the solver details
-    qcentroid_qiskit = QCentroidRuntimeQiskit.get_instance() # with optional params
+    QCentroidRuntimeQiskit.get_instance() # with optional params
 
-    print(f"currentVersion:{QCentroidRuntimeQiskit.getVersion()}")
+    logger.info(f"currentVersion:{QCentroidRuntimeQiskit.getVersion()}")
     QCentroidRuntimeQiskit.execute(circuit)
     
     
 if __name__ == "__main__":
+    logging.basicConfig(level=logging.DEBUG)
     main() 
 ```
```

