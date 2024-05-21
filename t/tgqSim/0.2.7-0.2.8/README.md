# Comparing `tmp/tgqSim-0.2.7.tar.gz` & `tmp/tgqSim-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgqSim-0.2.7.tar", last modified: Mon May 20 01:36:04 2024, max compression
+gzip compressed data, was "tgqSim-0.2.8.tar", last modified: Mon May 20 07:09:04 2024, max compression
```

## Comparing `tgqSim-0.2.7.tar` & `tgqSim-0.2.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:36:04.626012 tgqSim-0.2.7/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-20 01:36:02.000000 tgqSim-0.2.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-20 01:36:02.000000 tgqSim-0.2.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      753 2024-05-20 01:36:04.626012 tgqSim-0.2.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-20 01:36:02.000000 tgqSim-0.2.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 01:36:04.626012 tgqSim-0.2.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1185 2024-05-20 01:36:03.000000 tgqSim-0.2.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:36:04.625012 tgqSim-0.2.7/tgqSim/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:36:04.626012 tgqSim-0.2.7/tgqSim/GateSimulation/
--rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-20 01:36:02.000000 tgqSim-0.2.7/tgqSim/GateSimulation/DoubleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     5413 2024-05-20 01:36:02.000000 tgqSim-0.2.7/tgqSim/GateSimulation/SingleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-20 01:36:02.000000 tgqSim-0.2.7/tgqSim/GateSimulation/TripleGate.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-20 01:36:02.000000 tgqSim-0.2.7/tgqSim/GateSimulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22219 2024-05-20 01:36:02.000000 tgqSim-0.2.7/tgqSim/QuantumCircuit.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-20 01:36:03.000000 tgqSim-0.2.7/tgqSim/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18468 2024-05-20 01:36:02.000000 tgqSim-0.2.7/tgqSim/draw_circuit_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:36:04.626012 tgqSim-0.2.7/tgqSim/lib/
--rw-rw-rw-   0 root         (0) root         (0)    66280 2024-05-20 01:36:02.000000 tgqSim-0.2.7/tgqSim/lib/cuda_11-8_tgq_simulator.so
--rw-rw-rw-   0 root         (0) root         (0)    77800 2024-05-20 01:36:02.000000 tgqSim-0.2.7/tgqSim/lib/cuda_12-4_tgq_simulator.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:36:04.626012 tgqSim-0.2.7/tgqSim/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 01:36:03.000000 tgqSim-0.2.7/tgqSim/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      623 2024-05-20 01:36:02.000000 tgqSim-0.2.7/tgqSim/utils/dev_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:36:04.625012 tgqSim-0.2.7/tgqSim.egg-info/
--rw-r--r--   0 root         (0) root         (0)      753 2024-05-20 01:36:04.000000 tgqSim-0.2.7/tgqSim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2024-05-20 01:36:04.000000 tgqSim-0.2.7/tgqSim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 01:36:04.000000 tgqSim-0.2.7/tgqSim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       74 2024-05-20 01:36:04.000000 tgqSim-0.2.7/tgqSim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-20 01:36:04.000000 tgqSim-0.2.7/tgqSim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 07:09:04.910247 tgqSim-0.2.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-20 07:09:03.000000 tgqSim-0.2.8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-20 07:09:03.000000 tgqSim-0.2.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      753 2024-05-20 07:09:04.909247 tgqSim-0.2.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-20 07:09:03.000000 tgqSim-0.2.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 07:09:04.910247 tgqSim-0.2.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2024-05-20 07:09:03.000000 tgqSim-0.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 07:09:04.908247 tgqSim-0.2.8/tgqSim/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 07:09:04.909247 tgqSim-0.2.8/tgqSim/GateSimulation/
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-20 07:09:03.000000 tgqSim-0.2.8/tgqSim/GateSimulation/DoubleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     5413 2024-05-20 07:09:03.000000 tgqSim-0.2.8/tgqSim/GateSimulation/SingleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-20 07:09:03.000000 tgqSim-0.2.8/tgqSim/GateSimulation/TripleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-20 07:09:03.000000 tgqSim-0.2.8/tgqSim/GateSimulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23459 2024-05-20 07:09:03.000000 tgqSim-0.2.8/tgqSim/QuantumCircuit.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-20 07:09:03.000000 tgqSim-0.2.8/tgqSim/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18468 2024-05-20 07:09:03.000000 tgqSim-0.2.8/tgqSim/draw_circuit_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 07:09:04.909247 tgqSim-0.2.8/tgqSim/lib/
+-rw-rw-rw-   0 root         (0) root         (0)    66280 2024-05-20 07:09:03.000000 tgqSim-0.2.8/tgqSim/lib/cuda_11-8_tgq_simulator.so
+-rw-rw-rw-   0 root         (0) root         (0)    77800 2024-05-20 07:09:03.000000 tgqSim-0.2.8/tgqSim/lib/cuda_12-4_tgq_simulator.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 07:09:04.909247 tgqSim-0.2.8/tgqSim/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 07:09:03.000000 tgqSim-0.2.8/tgqSim/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      623 2024-05-20 07:09:03.000000 tgqSim-0.2.8/tgqSim/utils/dev_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 07:09:04.909247 tgqSim-0.2.8/tgqSim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      753 2024-05-20 07:09:04.000000 tgqSim-0.2.8/tgqSim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2024-05-20 07:09:04.000000 tgqSim-0.2.8/tgqSim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 07:09:04.000000 tgqSim-0.2.8/tgqSim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2024-05-20 07:09:04.000000 tgqSim-0.2.8/tgqSim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-20 07:09:04.000000 tgqSim-0.2.8/tgqSim.egg-info/top_level.txt
```

### Comparing `tgqSim-0.2.7/LICENSE` & `tgqSim-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tgqSim-0.2.7/PKG-INFO` & `tgqSim-0.2.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.2.7
+Version: 0.2.8
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,quantum,simulator,noise
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `tgqSim-0.2.7/setup.py` & `tgqSim-0.2.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='tgqSim',
-    version='0.2.7',
+    version='0.2.8',
     description='TGQ量子模拟器',  # 包描述
     long_description="Python for quantum simulation http://www.tiangongqs.com",  # 详细描述
     long_description_content_type='text/markdown',
     author='tiangongqs',  # 作者姓名
     license='MIT',  # 许可证
     package=find_packages(),
     include_package_data=True,
```

### Comparing `tgqSim-0.2.7/tgqSim/GateSimulation/DoubleGate.py` & `tgqSim-0.2.8/tgqSim/GateSimulation/DoubleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.2.7/tgqSim/GateSimulation/SingleGate.py` & `tgqSim-0.2.8/tgqSim/GateSimulation/SingleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.2.7/tgqSim/GateSimulation/TripleGate.py` & `tgqSim-0.2.8/tgqSim/GateSimulation/TripleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.2.7/tgqSim/QuantumCircuit.py` & `tgqSim-0.2.8/tgqSim/QuantumCircuit.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,23 +61,23 @@
     def __init__(self, message):
         self.message = message
         super().__init__(self.message)
 
 
 class QuantumCircuit:
     def __init__(self, qbit_number=None):
-        self.qbit_list = [] if not qbit_number else self.add_qubits(number=qbit_number)
+        self.qbit_list = []
         self.cbit_list = []
         self.gate_list = []
         self.qbit_register = {}
         self.base_single_gate = ['h', 'x', 'y', 'z', 'rx', 'ry', 'rz', 'u3', 's', 'sdg', 't', 'tdg', "damp_I", "pd", "ad"]
         self.base_double_gate = ['cx', 'swap', 'iswap', 'cz', 'cp', 'rxx', 'ryy', 'rzz', 'syc']
         self.base_triple_gate = ['ccx', 'cswap']
         self.noise_mapper = {"bit_flip": "BF", "asymmetric_depolarization": "ADP", "depolarize": "DP", "phase_flip": "PF", "phase_damp": "PD", "amplitude_damp": "AD"}
-        self.width = 0
+        self.width = qbit_number
         self.state = []
         self.circuit_diag = []
         self.isgpu = False
         self.deviceid = []
         self.noise_circuit = []
         self.current_gate_info = ()
         self.prob_result = {}
@@ -102,50 +102,71 @@
     def add_single_gate(self, gate_pos: Union[int, str], *gate_info):
         """
         添加单比特门序列
         :param gate_pos:
         :param gate_info: 门类型，门参数
         :return:
         """
+        tmp_pos = gate_pos
+        if isinstance(gate_pos, list):
+            tmp_pos = gate_pos[0]
+        if tmp_pos < 0 or tmp_pos >= self.width:
+            raise ValueError("添加的位置不能为负数或不能超过线路设置的比特数")
+        if len(gate_info) >= 1:
+            if gate_info[0] not in self.base_single_gate:
+                raise ValueError("添加的门名称在框架支持中，请检查添加门的名称")
         if isinstance(gate_pos, int):
             gatename = gate_info[0].upper()
             self.circuit_diag.append([(gatename, gate_pos)])
         else:
             self.circuit_diag.append([(gatename, int(gate_pos))])
+
         self.current_gate_info = (gate_pos, gate_info)
         self.gate_list.append((gate_pos, gate_info))
         # print("over")
         return self
         # todo 通过比特名称访问
         # if isinstance(gate_pos, str):
         #     return self.gate_list.append((gate_pos, gate_type))
 
-    def add_double_gate(self, gate_pos_0, gate_pos_1, *gate_info):
+    def add_double_gate(self, gate_pos_0:int, gate_pos_1:int, *gate_info):
         """
         添加两比特门序列
         :param gate_pos_0: 控制位
         :param gate_pos_1: 目标位
         :param gate_info: 门类型，门参数
         :return:
         """
+        min_pos, max_pos = min([gate_pos_0, gate_pos_1]), max([gate_pos_0, gate_pos_1])
+        if min_pos < 0 or max_pos >= self.width:
+            raise ValueError("添加的位置不能为负数或不能超过线路设置的比特数")
+        if len(gate_info) >= 1:
+            if gate_info[0] not in self.base_single_gate:
+                raise ValueError("添加的门名称在框架支持中，请检查添加门的名称")
         if gate_info[0] in ["rxx", 'ryy', 'rzz', 'iswap', 'syc']:
             self.circuit_diag.append([(gate_info[0].upper(), (gate_pos_1, gate_pos_0))])
         else:
             self.circuit_diag.append([(gate_info[0].upper(), gate_pos_1, gate_pos_0)])
         self.current_gate_info = ([gate_pos_0, gate_pos_1], gate_info)
         self.gate_list.append(([gate_pos_0, gate_pos_1], gate_info))
         return self
 
-    def add_triple_gate(self, gate_pos, *gate_info):
+    def add_triple_gate(self, gate_pos:list, *gate_info):
         """
         添加三比特门序列
         :param gate_pos:
         :param gate_info:
         :return:
         """
+        min_pos, max_pos = min(gate_pos), max(gate_pos)
+        if min_pos < 0 or max_pos >= self.width:
+            raise ValueError("添加的位置不能为负数或不能超过线路设置的比特数")
+        if len(gate_info) >= 1:
+            if gate_info[0] not in self.base_single_gate:
+                raise ValueError("添加的门名称在框架支持中，请检查添加门的名称")
         self.circuit_diag.append([(gate_info[0].upper(), gate_pos[2], gate_pos[0], gate_pos[1])])
         self.current_gate_info = (gate_pos, gate_info)
         self.gate_list.append((gate_pos, gate_info))
         return self
     
     def setdevice(self, deviceList: Union[int, list]):
         gpus = GPUtil.getGPUs()
```

### Comparing `tgqSim-0.2.7/tgqSim/draw_circuit_tools.py` & `tgqSim-0.2.8/tgqSim/draw_circuit_tools.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.2.7/tgqSim/lib/cuda_11-8_tgq_simulator.so` & `tgqSim-0.2.8/tgqSim/lib/cuda_11-8_tgq_simulator.so`

 * *Files identical despite different names*

### Comparing `tgqSim-0.2.7/tgqSim/lib/cuda_12-4_tgq_simulator.so` & `tgqSim-0.2.8/tgqSim/lib/cuda_12-4_tgq_simulator.so`

 * *Files identical despite different names*

### Comparing `tgqSim-0.2.7/tgqSim/utils/dev_tools.py` & `tgqSim-0.2.8/tgqSim/utils/dev_tools.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.2.7/tgqSim.egg-info/PKG-INFO` & `tgqSim-0.2.8/tgqSim.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.2.7
+Version: 0.2.8
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,quantum,simulator,noise
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `tgqSim-0.2.7/tgqSim.egg-info/SOURCES.txt` & `tgqSim-0.2.8/tgqSim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

