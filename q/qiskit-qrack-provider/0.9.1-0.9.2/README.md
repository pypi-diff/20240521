# Comparing `tmp/qiskit-qrack-provider-0.9.1.tar.gz` & `tmp/qiskit-qrack-provider-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-qrack-provider-0.9.1.tar", last modified: Sun Dec  3 15:06:09 2023, max compression
+gzip compressed data, was "qiskit-qrack-provider-0.9.2.tar", last modified: Mon Feb 19 16:07:17 2024, max compression
```

## Comparing `qiskit-qrack-provider-0.9.1.tar` & `qiskit-qrack-provider-0.9.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-12-03 15:06:09.084512 qiskit-qrack-provider-0.9.1/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    11357 2023-12-03 12:05:47.000000 qiskit-qrack-provider-0.9.1/LICENSE
--rw-r--r--   0 iamu      (1000) iamu      (1000)     2852 2023-12-03 15:06:09.080512 qiskit-qrack-provider-0.9.1/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1671 2023-12-03 12:05:47.000000 qiskit-qrack-provider-0.9.1/README.md
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-12-03 15:06:09.080512 qiskit-qrack-provider-0.9.1/qiskit/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-12-03 15:06:09.080512 qiskit-qrack-provider-0.9.1/qiskit/providers/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-12-03 15:06:09.080512 qiskit-qrack-provider-0.9.1/qiskit/providers/qrack/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1164 2023-12-03 12:09:45.000000 qiskit-qrack-provider-0.9.1/qiskit/providers/qrack/__init__.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-12-03 15:06:09.080512 qiskit-qrack-provider-0.9.1/qiskit/providers/qrack/backends/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      548 2023-12-03 12:05:47.000000 qiskit-qrack-provider-0.9.1/qiskit/providers/qrack/backends/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    38196 2023-12-03 14:58:57.000000 qiskit-qrack-provider-0.9.1/qiskit/providers/qrack/backends/qasm_simulator.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      914 2023-12-03 12:05:47.000000 qiskit-qrack-provider-0.9.1/qiskit/providers/qrack/qrackerror.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1903 2023-12-03 12:05:47.000000 qiskit-qrack-provider-0.9.1/qiskit/providers/qrack/qrackjob.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1449 2023-12-03 12:05:47.000000 qiskit-qrack-provider-0.9.1/qiskit/providers/qrack/qrackprovider.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     8929 2023-12-03 12:06:45.000000 qiskit-qrack-provider-0.9.1/qiskit/providers/qrack/sampler.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      506 2023-12-03 15:04:07.000000 qiskit-qrack-provider-0.9.1/qiskit/providers/qrack/version.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-12-03 15:06:09.080512 qiskit-qrack-provider-0.9.1/qiskit_qrack_provider.egg-info/
--rw-r--r--   0 iamu      (1000) iamu      (1000)     2852 2023-12-03 15:06:09.000000 qiskit-qrack-provider-0.9.1/qiskit_qrack_provider.egg-info/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      559 2023-12-03 15:06:09.000000 qiskit-qrack-provider-0.9.1/qiskit_qrack_provider.egg-info/SOURCES.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-12-03 15:06:09.000000 qiskit-qrack-provider-0.9.1/qiskit_qrack_provider.egg-info/dependency_links.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       30 2023-12-03 15:06:09.000000 qiskit-qrack-provider-0.9.1/qiskit_qrack_provider.egg-info/requires.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        7 2023-12-03 15:06:09.000000 qiskit-qrack-provider-0.9.1/qiskit_qrack_provider.egg-info/top_level.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-12-03 15:06:09.084512 qiskit-qrack-provider-0.9.1/setup.cfg
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1742 2023-12-03 15:03:52.000000 qiskit-qrack-provider-0.9.1/setup.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-02-19 16:07:17.169690 qiskit-qrack-provider-0.9.2/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    11357 2023-12-03 12:05:47.000000 qiskit-qrack-provider-0.9.2/LICENSE
+-rw-r--r--   0 iamu      (1000) iamu      (1000)     2852 2024-02-19 16:07:17.169690 qiskit-qrack-provider-0.9.2/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1671 2023-12-03 12:05:47.000000 qiskit-qrack-provider-0.9.2/README.md
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-02-19 16:07:17.169690 qiskit-qrack-provider-0.9.2/qiskit/
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-02-19 16:07:17.169690 qiskit-qrack-provider-0.9.2/qiskit/providers/
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-02-19 16:07:17.169690 qiskit-qrack-provider-0.9.2/qiskit/providers/qrack/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1164 2023-12-03 12:09:45.000000 qiskit-qrack-provider-0.9.2/qiskit/providers/qrack/__init__.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-02-19 16:07:17.169690 qiskit-qrack-provider-0.9.2/qiskit/providers/qrack/backends/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      548 2023-12-03 12:05:47.000000 qiskit-qrack-provider-0.9.2/qiskit/providers/qrack/backends/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    38197 2024-02-19 16:05:56.000000 qiskit-qrack-provider-0.9.2/qiskit/providers/qrack/backends/qasm_simulator.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      914 2023-12-03 12:05:47.000000 qiskit-qrack-provider-0.9.2/qiskit/providers/qrack/qrackerror.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1903 2023-12-03 12:05:47.000000 qiskit-qrack-provider-0.9.2/qiskit/providers/qrack/qrackjob.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1449 2023-12-03 12:05:47.000000 qiskit-qrack-provider-0.9.2/qiskit/providers/qrack/qrackprovider.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     8929 2023-12-03 12:06:45.000000 qiskit-qrack-provider-0.9.2/qiskit/providers/qrack/sampler.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      506 2023-12-03 15:04:07.000000 qiskit-qrack-provider-0.9.2/qiskit/providers/qrack/version.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-02-19 16:07:17.169690 qiskit-qrack-provider-0.9.2/qiskit_qrack_provider.egg-info/
+-rw-r--r--   0 iamu      (1000) iamu      (1000)     2852 2024-02-19 16:07:17.000000 qiskit-qrack-provider-0.9.2/qiskit_qrack_provider.egg-info/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      559 2024-02-19 16:07:17.000000 qiskit-qrack-provider-0.9.2/qiskit_qrack_provider.egg-info/SOURCES.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2024-02-19 16:07:17.000000 qiskit-qrack-provider-0.9.2/qiskit_qrack_provider.egg-info/dependency_links.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       30 2024-02-19 16:07:17.000000 qiskit-qrack-provider-0.9.2/qiskit_qrack_provider.egg-info/requires.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        7 2024-02-19 16:07:17.000000 qiskit-qrack-provider-0.9.2/qiskit_qrack_provider.egg-info/top_level.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2024-02-19 16:07:17.169690 qiskit-qrack-provider-0.9.2/setup.cfg
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1742 2024-02-19 16:06:14.000000 qiskit-qrack-provider-0.9.2/setup.py
```

### Comparing `qiskit-qrack-provider-0.9.1/LICENSE` & `qiskit-qrack-provider-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.9.1/PKG-INFO` & `qiskit-qrack-provider-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-qrack-provider
-Version: 0.9.1
+Version: 0.9.2
 Summary: Qiskit Qrack Provider - Qrack High-Performance GPU simulation for Qiskit
 Home-page: https://github.com/vm6502q/qiskit-qrack-provider
 Author: Daniel Strano
 Author-email: dan@unitary.fund
 License: Apache 2.0
 Keywords: qiskit qrack pyqrack simulator quantum addon backend
 Classifier: Environment :: Console
```

### Comparing `qiskit-qrack-provider-0.9.1/README.md` & `qiskit-qrack-provider-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.9.1/qiskit/providers/qrack/__init__.py` & `qiskit-qrack-provider-0.9.2/qiskit/providers/qrack/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.9.1/qiskit/providers/qrack/backends/__init__.py` & `qiskit-qrack-provider-0.9.2/qiskit/providers/qrack/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.9.1/qiskit/providers/qrack/backends/qasm_simulator.py` & `qiskit-qrack-provider-0.9.2/qiskit/providers/qrack/backends/qasm_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         'is_schmidt_decompose': True,
         'is_stabilizer_hybrid': True,
         'is_binary_decision_tree': False,
         'is_paged': True,
         'is_cpu_gpu_hybrid': True,
         'is_host_pointer': False,
         'is_t_injected': True,
-        'is_reactively_separated': True
+        'is_reactively_separated': False
     }
 
     DEFAULT_CONFIGURATION = {
         'backend_name': 'statevector_simulator',
         'backend_version': __version__,
         'n_qubits': 64,
         'conditional': True,
```

### Comparing `qiskit-qrack-provider-0.9.1/qiskit/providers/qrack/qrackerror.py` & `qiskit-qrack-provider-0.9.2/qiskit/providers/qrack/qrackerror.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.9.1/qiskit/providers/qrack/qrackjob.py` & `qiskit-qrack-provider-0.9.2/qiskit/providers/qrack/qrackjob.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.9.1/qiskit/providers/qrack/qrackprovider.py` & `qiskit-qrack-provider-0.9.2/qiskit/providers/qrack/qrackprovider.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.9.1/qiskit/providers/qrack/sampler.py` & `qiskit-qrack-provider-0.9.2/qiskit/providers/qrack/sampler.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.9.1/qiskit_qrack_provider.egg-info/PKG-INFO` & `qiskit-qrack-provider-0.9.2/qiskit_qrack_provider.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-qrack-provider
-Version: 0.9.1
+Version: 0.9.2
 Summary: Qiskit Qrack Provider - Qrack High-Performance GPU simulation for Qiskit
 Home-page: https://github.com/vm6502q/qiskit-qrack-provider
 Author: Daniel Strano
 Author-email: dan@unitary.fund
 License: Apache 2.0
 Keywords: qiskit qrack pyqrack simulator quantum addon backend
 Classifier: Environment :: Console
```

### Comparing `qiskit-qrack-provider-0.9.1/qiskit_qrack_provider.egg-info/SOURCES.txt` & `qiskit-qrack-provider-0.9.2/qiskit_qrack_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.9.1/setup.py` & `qiskit-qrack-provider-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 requirements = [
     'numpy>=1.16.3',
     'pyqrack>=1.21.0'
 ]
 
 # Handle version.
-VERSION = "0.9.1"
+VERSION = "0.9.2"
 
 # Read long description from README.
 README_PATH = os.path.join(os.path.abspath(os.path.dirname(__file__)),
                            'README.md')
 with open(README_PATH) as readme_file:
     README = readme_file.read()
```

