# Comparing `tmp/paibox-1.1.0a1.tar.gz` & `tmp/paibox-1.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paibox-1.1.0a1.tar", max compression
+gzip compressed data, was "paibox-1.1.0a2.tar", max compression
```

## Comparing `paibox-1.1.0a1.tar` & `paibox-1.1.0a2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1371 2024-05-19 09:30:00.406718 paibox-1.1.0a1/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-05-19 09:30:00.406718 paibox-1.1.0a1/LICENSE
--rw-r--r--   0        0        0      958 2024-05-19 09:30:00.406718 paibox-1.1.0a1/README.md
--rw-r--r--   0        0        0    37145 2024-05-19 09:30:00.406718 paibox-1.1.0a1/docs/Guide-of-PAIBox.md
--rw-r--r--   0        0        0     2816 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/__init__.py
--rw-r--r--   0        0        0      150 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/__init__.py
--rw-r--r--   0        0        0      394 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/checker.py
--rw-r--r--   0        0        0    16050 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/conf_template.py
--rw-r--r--   0        0        0     2079 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/constrs.py
--rw-r--r--   0        0        0     3030 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/context.py
--rw-r--r--   0        0        0    20470 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/graphs.py
--rw-r--r--   0        0        0     1228 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/graphs_types.py
--rw-r--r--   0        0        0    23907 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/mapper.py
--rw-r--r--   0        0        0    25600 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/placement.py
--rw-r--r--   0        0        0    21588 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/routing.py
--rw-r--r--   0        0        0    12062 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/backend/segment_utils.py
--rw-r--r--   0        0        0    10304 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/base.py
--rw-r--r--   0        0        0     5168 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/collector.py
--rw-r--r--   0        0        0      143 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/components/__init__.py
--rw-r--r--   0        0        0    30230 2024-05-19 09:30:00.410719 paibox-1.1.0a1/paibox/components/functional.py
--rw-r--r--   0        0        0    12086 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/modules.py
--rw-r--r--   0        0        0       25 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/neuron/__init__.py
--rw-r--r--   0        0        0    18488 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/neuron/base.py
--rw-r--r--   0        0        0     5632 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/neuron/neurons.py
--rw-r--r--   0        0        0      775 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/neuron/utils.py
--rw-r--r--   0        0        0     5238 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/projection.py
--rw-r--r--   0        0        0       88 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/synapses/__init__.py
--rw-r--r--   0        0        0    12804 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/synapses/base.py
--rw-r--r--   0        0        0      714 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/synapses/conv_types.py
--rw-r--r--   0        0        0    20753 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/synapses/conv_utils.py
--rw-r--r--   0        0        0     9036 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/synapses/synapses.py
--rw-r--r--   0        0        0    15277 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/components/synapses/transforms.py
--rw-r--r--   0        0        0     1704 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/context.py
--rw-r--r--   0        0        0     1791 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/exceptions.py
--rw-r--r--   0        0        0     7091 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/mixin.py
--rw-r--r--   0        0        0     1567 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/naming.py
--rw-r--r--   0        0        0     5322 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/network.py
--rw-r--r--   0        0        0      417 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/node.py
--rw-r--r--   0        0        0      115 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/simulator/__init__.py
--rw-r--r--   0        0        0     7793 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/simulator/encoder.py
--rw-r--r--   0        0        0     1230 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/simulator/probe.py
--rw-r--r--   0        0        0     6932 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/simulator/simulator.py
--rw-r--r--   0        0        0     1571 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/simulator/utils.py
--rw-r--r--   0        0        0      400 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/tools.py
--rw-r--r--   0        0        0     2227 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/types.py
--rw-r--r--   0        0        0     5531 2024-05-19 09:30:00.414718 paibox-1.1.0a1/paibox/utils.py
--rw-r--r--   0        0        0     2241 2024-05-19 09:30:00.414718 paibox-1.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 paibox-1.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1371 2024-05-21 11:46:16.796567 paibox-1.1.0a2/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-05-21 11:46:16.796567 paibox-1.1.0a2/LICENSE
+-rw-r--r--   0        0        0      958 2024-05-21 11:46:16.796567 paibox-1.1.0a2/README.md
+-rw-r--r--   0        0        0    37145 2024-05-21 11:46:16.800567 paibox-1.1.0a2/docs/Guide-of-PAIBox.md
+-rw-r--r--   0        0        0     2816 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/__init__.py
+-rw-r--r--   0        0        0      150 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/__init__.py
+-rw-r--r--   0        0        0      394 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/checker.py
+-rw-r--r--   0        0        0    16085 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/conf_template.py
+-rw-r--r--   0        0        0     2079 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/constrs.py
+-rw-r--r--   0        0        0     3112 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/context.py
+-rw-r--r--   0        0        0    20470 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/graphs.py
+-rw-r--r--   0        0        0     1228 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/graphs_types.py
+-rw-r--r--   0        0        0    24207 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/mapper.py
+-rw-r--r--   0        0        0    25600 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/placement.py
+-rw-r--r--   0        0        0    21588 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/routing.py
+-rw-r--r--   0        0        0    12062 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/segment_utils.py
+-rw-r--r--   0        0        0    10304 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/base.py
+-rw-r--r--   0        0        0     5168 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/collector.py
+-rw-r--r--   0        0        0      143 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/__init__.py
+-rw-r--r--   0        0        0    30230 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/functional.py
+-rw-r--r--   0        0        0    12086 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/modules.py
+-rw-r--r--   0        0        0       25 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/neuron/__init__.py
+-rw-r--r--   0        0        0    18494 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/neuron/base.py
+-rw-r--r--   0        0        0     5632 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/neuron/neurons.py
+-rw-r--r--   0        0        0      775 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/neuron/utils.py
+-rw-r--r--   0        0        0     5238 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/projection.py
+-rw-r--r--   0        0        0       88 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/synapses/__init__.py
+-rw-r--r--   0        0        0    12804 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/synapses/base.py
+-rw-r--r--   0        0        0      714 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/synapses/conv_types.py
+-rw-r--r--   0        0        0    20753 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/synapses/conv_utils.py
+-rw-r--r--   0        0        0     9036 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/synapses/synapses.py
+-rw-r--r--   0        0        0    15277 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/synapses/transforms.py
+-rw-r--r--   0        0        0     1704 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/context.py
+-rw-r--r--   0        0        0     1791 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/exceptions.py
+-rw-r--r--   0        0        0     7091 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/mixin.py
+-rw-r--r--   0        0        0     1567 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/naming.py
+-rw-r--r--   0        0        0     5322 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/network.py
+-rw-r--r--   0        0        0      417 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/node.py
+-rw-r--r--   0        0        0      115 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/simulator/__init__.py
+-rw-r--r--   0        0        0     7793 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/simulator/encoder.py
+-rw-r--r--   0        0        0     1230 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/simulator/probe.py
+-rw-r--r--   0        0        0     6932 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/simulator/simulator.py
+-rw-r--r--   0        0        0     1571 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/simulator/utils.py
+-rw-r--r--   0        0        0      400 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/tools.py
+-rw-r--r--   0        0        0     2239 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/types.py
+-rw-r--r--   0        0        0     3164 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/utils.py
+-rw-r--r--   0        0        0     2241 2024-05-21 11:46:16.804567 paibox-1.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 paibox-1.1.0a2/PKG-INFO
```

### Comparing `paibox-1.1.0a1/CHANGELOG.md` & `paibox-1.1.0a2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/LICENSE` & `paibox-1.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/README.md` & `paibox-1.1.0a2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIBox/blob/master/pyproject.toml">
         <img src="https://img.shields.io/pypi/pyversions/paibox">
     </a>
-    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.1.0a1">
-        <img src="https://img.shields.io/github/v/release/PAICookers/PAIBox&color=orange">
+    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.1.0a2">
+        <img src="https://img.shields.io/github/v/release/PAICookers/PAIBox?color=orange">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIBox">
       <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIBox/master?color=red">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIBox/master">
 	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIBox/master.svg" alt="pre-commit.ci status">
     </a>
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
                                    # PAIBox
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_p_a_i_b_o_x_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
- _v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_&_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/
+ _v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_?_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/
     _g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
 ð ç¨æ·ä½¿ç¨æåï¼[Guide-of-PAIBox](docs/Guide-of-PAIBox.md)
 é«æç¼åæµè¯é¡¹ç®æåï¼[Guide-of-Test](docs/Guide-of-Test.md)
 [Changelog](./CHANGELOG.md)
```

### Comparing `paibox-1.1.0a1/docs/Guide-of-PAIBox.md` & `paibox-1.1.0a2/docs/Guide-of-PAIBox.md`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/__init__.py` & `paibox-1.1.0a2/paibox/__init__.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/backend/conf_template.py` & `paibox-1.1.0a2/paibox/backend/conf_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
 from pathlib import Path
-from typing import Any, ClassVar, Dict, List, Literal, NamedTuple, TypedDict
+from typing import Any, ClassVar, Dict, List, NamedTuple, TypedDict
 
 import numpy as np
 from numpy.typing import NDArray
 from paicorelib import (
     LCN_EX,
     AxonCoord,
     ChipCoord,
@@ -331,34 +331,35 @@
 
 
 def gen_config_frames_by_coreconf(
     config_dict: CorePlmConf,
     write_to_file: bool,
     fp: Path,
     split_by_coord: bool,
-    format: Literal["txt", "bin", "npy"],
+    formats: List[str],
 ) -> Dict[Coord, FrameArrayType]:
     """Generate configuration frames by given the `CorePlmConfig`.
 
     Args:
         - config_dict: the dictionary of configurations.
         - write_to_file: whether to write frames to file.
         - fp: If `write_to_file` is `True`, specify the path.
         - split_by_coord: whether to split the generated frames file by the core coordinates.
-        - format: `txt`, `bin`, or `npy`.
+        - format: a list of formats to export.
     """
 
     def _write_to_f(name: str, array: FrameArrayType) -> None:
-        _fp = fp / (name + f".{format}")
-        if format == "npy":
-            np2npy(_fp, array)
-        elif format == "bin":
-            np2bin(_fp, array)
-        else:
-            np2txt(_fp, array)
+        for format in formats:
+            _fp = fp / (name + f".{format}")
+            if format == "npy":
+                np2npy(_fp, array)
+            elif format == "bin":
+                np2bin(_fp, array)
+            else:
+                np2txt(_fp, array)
 
     _default_rid = RId(0, 0)
     _debug_dict: Dict[Coord, Dict[str, Any]] = dict()
     frame_arrays_on_core: Dict[Coord, FrameArrayType] = dict()
 
     for chip_coord, conf_in_chip in config_dict.items():
         for core_coord, v in conf_in_chip.items():
@@ -439,18 +440,18 @@
 
     if write_to_file:
         if split_by_coord:
             for core_coord, f in frame_arrays_on_core.items():
                 addr = core_coord.address
                 _write_to_f(f"config_core{addr}", f)
         else:
-            _f = np.concatenate(
+            f = np.concatenate(
                 list(frame_arrays_on_core.values()), dtype=FRAME_DTYPE, casting="no"
             )
-            _write_to_f(f"config_cores_all", _f)
+            _write_to_f(f"config_cores_all", f)
 
     return frame_arrays_on_core
 
 
 def export_core_params_json(core_conf: Dict[Coord, CoreConfig], fp: Path) -> None:
     _valid_conf = {str(k): v.export() for k, v in core_conf.items()}
```

### Comparing `paibox-1.1.0a1/paibox/backend/constrs.py` & `paibox-1.1.0a2/paibox/backend/constrs.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/backend/context.py` & `paibox-1.1.0a2/paibox/backend/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 DEFAULT_OUTPUT_CORE_ADDR_START = Coord(0, 0)
 DEFAULT_CORE_PARAMS_CONF_JSON = "core_params.json"
 DEFAULT_INPUT_CONF_JSON = "input_proj_info.json"
 DEFAULT_OUTPUT_CONF_JSON = "output_dest_info.json"
 
 
 class _BackendContext(_Context):
-    _DefaultContext = {
+    _default = {
         "output_chip_addr": DEFAULT_OUTPUT_CHIP_ADDR,  # RO mostly
         "target_chip_addr": DEFAULT_LOCAL_CHIP_ADDR,  # RO mostly
         "build_directory": Path.cwd(),  # R/W
         "output_core_addr_start": DEFAULT_OUTPUT_CORE_ADDR_START,  # RO
         "core_conf_json": DEFAULT_CORE_PARAMS_CONF_JSON,  # RO mostly
         "input_conf_json": DEFAULT_INPUT_CONF_JSON,  # RO mostly
         "output_conf_json": DEFAULT_OUTPUT_CONF_JSON,  # RO mostly
         "cflags": dict(),  # R/W
     }
 
     def __init__(self) -> None:
         super().__init__()
-        self.update(self._DefaultContext)
+        self.update(self._default)
 
     @property
     def target_chip_addr(self) -> List[ChipCoord]:
         return self["target_chip_addr"]
 
     @target_chip_addr.setter
     def target_chip_addr(self, addr: Union[CoordLike, List[CoordLike]]) -> None:
@@ -83,14 +83,18 @@
         self["build_directory"] = Path(p)
 
     @property
     def cflags(self) -> Dict[str, Any]:
         """Compilation options."""
         return self["cflags"]
 
+    def set_default(self) -> None:
+        self.clear_all()
+        self.update(self._default)
+
 
 _BACKEND_CONTEXT = _BackendContext()
 
 
 def set_cflag(**kwargs) -> None:
     for k, v in kwargs.items():
         _BACKEND_CONTEXT.cflags[k] = v
```

### Comparing `paibox-1.1.0a1/paibox/backend/graphs.py` & `paibox-1.1.0a2/paibox/backend/graphs.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/backend/graphs_types.py` & `paibox-1.1.0a2/paibox/backend/graphs_types.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/backend/mapper.py` & `paibox-1.1.0a2/paibox/backend/mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -498,32 +498,44 @@
         self,
         write_to_file: bool = True,
         *,
         fp: Optional[Union[str, Path]] = None,
         format: Literal["txt", "bin", "npy"] = "bin",
         split_by_coord: bool = False,
         export_core_params: bool = False,
+        use_hw_sim: bool = True,
     ) -> Dict[Coord, Any]:
         """Generate configuration frames & export to file.
 
         Args:
             - write_to_file: whether to write frames into file.
             - fp: If `write_to_file` is `True`, specify the output path.
             - format: `txt`, `bin`, or `npy`. `bin` is recommended.
             - split_by_coord: whether to split the generated frames file by the core coordinates.
             - export_core_params: whether to export the parameters of occupied cores.
+            - use_hw_sim: whether to use hardware simulator. If use, '.txt' will be exported.
 
         Return: a dictionary of configurations.
         """
         if format not in ("bin", "npy", "txt"):
             raise ValueError(f"format {format} is not supported.")
 
+        formats = [format]
+        if use_hw_sim:
+            formats.append("txt")
+
+        formats = list(set(formats))
+
         _fp = _fp_check(fp)
         config_dict = gen_config_frames_by_coreconf(
-            self.graph_info["members"], write_to_file, _fp, split_by_coord, format
+            self.graph_info["members"],
+            write_to_file,
+            _fp,
+            split_by_coord,
+            formats,
         )
 
         if export_core_params:
             # Export the parameters of occupied cores
             export_core_params_json(self.core_params, _fp)
 
         # Export the configurations of input nodes
```

### Comparing `paibox-1.1.0a1/paibox/backend/placement.py` & `paibox-1.1.0a2/paibox/backend/placement.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/backend/routing.py` & `paibox-1.1.0a2/paibox/backend/routing.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/backend/segment_utils.py` & `paibox-1.1.0a2/paibox/backend/segment_utils.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/base.py` & `paibox-1.1.0a2/paibox/base.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/collector.py` & `paibox-1.1.0a2/paibox/collector.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/components/functional.py` & `paibox-1.1.0a2/paibox/components/functional.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/components/modules.py` & `paibox-1.1.0a2/paibox/components/modules.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/components/neuron/base.py` & `paibox-1.1.0a2/paibox/components/neuron/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         synaptic_integration_mode: SIM,
         bit_truncation: int,
         keep_shape: bool = False,
     ) -> None:
         """Stateless attributes. Scalar."""
         # Basic attributes.
         self.keep_shape = keep_shape
-        self._n_neuron = shape2num(shape)
         self._shape = as_shape(shape)
+        self._n_neuron = shape2num(self._shape)
 
         # DO NOT modify the names of the following variables.
         # They will be exported to the parameter verification model.
         self.reset_mode: RM = reset_mode
         self.reset_v: int = reset_v  # Signed 30-bit
         self.leak_comparison: LCM = leak_comparison
         self.threshold_mask_bits: int = threshold_mask_bits
```

### Comparing `paibox-1.1.0a1/paibox/components/neuron/neurons.py` & `paibox-1.1.0a2/paibox/components/neuron/neurons.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/components/neuron/utils.py` & `paibox-1.1.0a2/paibox/components/neuron/utils.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/components/projection.py` & `paibox-1.1.0a2/paibox/components/projection.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/components/synapses/base.py` & `paibox-1.1.0a2/paibox/components/synapses/base.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/components/synapses/conv_types.py` & `paibox-1.1.0a2/paibox/components/synapses/conv_types.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/components/synapses/conv_utils.py` & `paibox-1.1.0a2/paibox/components/synapses/conv_utils.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/components/synapses/synapses.py` & `paibox-1.1.0a2/paibox/components/synapses/synapses.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -187,16 +187,16 @@
 
         super().__init__(
             source,
             dest,
             kernel,
             _single(stride),
             _single(padding),
-            _single(output_padding),
             _single(1),
+            _single(output_padding),
             kernel_order,
             name,
         )
 
 
 class ConvTranspose2d(ConvTranspose2dSyn):
     def __init__(
@@ -237,12 +237,12 @@
 
         super().__init__(
             source,
             dest,
             kernel,
             _pair(stride),
             _pair(padding),
-            _pair(output_padding),
             _pair(1),
+            _pair(output_padding),
             kernel_order,
             name,
         )
```

### Comparing `paibox-1.1.0a1/paibox/components/synapses/transforms.py` & `paibox-1.1.0a2/paibox/components/synapses/transforms.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/context.py` & `paibox-1.1.0a2/paibox/context.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/exceptions.py` & `paibox-1.1.0a2/paibox/exceptions.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/mixin.py` & `paibox-1.1.0a2/paibox/mixin.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/naming.py` & `paibox-1.1.0a2/paibox/naming.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/network.py` & `paibox-1.1.0a2/paibox/network.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/simulator/encoder.py` & `paibox-1.1.0a2/paibox/simulator/encoder.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/simulator/probe.py` & `paibox-1.1.0a2/paibox/simulator/probe.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/simulator/simulator.py` & `paibox-1.1.0a2/paibox/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/simulator/utils.py` & `paibox-1.1.0a2/paibox/simulator/utils.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a1/paibox/types.py` & `paibox-1.1.0a2/paibox/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     Union,
 )
 
 import numpy as np
 from numpy.typing import NDArray
 from typing_extensions import TypeAlias
 
-Shape = TypeVar("Shape", int, Tuple[int, ...], List[int])
+Shape = TypeVar("Shape", int, Tuple[int, ...], List[int], np.ndarray)
 ArrayType = TypeVar("ArrayType", List[int], Tuple[int, ...], np.ndarray)
 Scalar = TypeVar("Scalar", int, float, np.generic)
 IntScalarType = TypeVar("IntScalarType", int, np.bool_, np.integer)
 DataType = TypeVar("DataType", int, np.bool_, np.integer, np.ndarray)
 DataArrayType = TypeVar(
     "DataArrayType", int, np.bool_, np.integer, List[int], Tuple[int, ...], np.ndarray
 )
```

### Comparing `paibox-1.1.0a1/pyproject.toml` & `paibox-1.1.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paibox"
-version = "1.1.0a1"
+version = "1.1.0a2"
 description = "Toolchain of PAICORE 2.0"
 authors = ["Ziru Pan <zrpan@stu.pku.edu.cn>"]
 maintainers = [
     "Hongtu Xia <hongtux@pku.edu.cn>",
     "Siyuan Gao <siyuan-gao@outlook.com>",
     "Zhaoyang Hao <hzyang2218@gmail.com>",
     "Ziru Pan <zrpan@stu.pku.edu.cn>",
@@ -34,15 +34,15 @@
 # Includes the document
 include = ["docs/Guide-of-PAIBox.md", "CHANGELOG.md"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^2.0"
 numpy = "^1.24.0"
-paicorelib = "^1.1.1"
+paicorelib = "^1.1.2"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `paibox-1.1.0a1/PKG-INFO` & `paibox-1.1.0a2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paibox
-Version: 1.1.0a1
+Version: 1.1.0a2
 Summary: Toolchain of PAICORE 2.0
 Home-page: https://github.com/PAICookers/PAIBox
 License: GPL-3.0-or-later
 Keywords: PAICORE 2.0,PAIBox,SNN,Toolchain
 Author: Ziru Pan
 Author-email: zrpan@stu.pku.edu.cn
 Maintainer: Hongtu Xia
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: numpy (>=1.24.0,<2.0.0)
-Requires-Dist: paicorelib (>=1.1.1,<2.0.0)
+Requires-Dist: paicorelib (>=1.1.2,<2.0.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Project-URL: Documentation, https://github.com/PAICookers/PAIBox#readme
 Project-URL: Repository, https://github.com/PAICookers/PAIBox
 Description-Content-Type: text/markdown
 
 <div align="center">
 
@@ -36,16 +36,16 @@
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIBox/blob/master/pyproject.toml">
         <img src="https://img.shields.io/pypi/pyversions/paibox">
     </a>
-    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.1.0a1">
-        <img src="https://img.shields.io/github/v/release/PAICookers/PAIBox&color=orange">
+    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.1.0a2">
+        <img src="https://img.shields.io/github/v/release/PAICookers/PAIBox?color=orange">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIBox">
       <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIBox/master?color=red">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIBox/master">
 	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIBox/master.svg" alt="pre-commit.ci status">
     </a>
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: paibox Version: 1.1.0a1 Summary: Toolchain of
+Metadata-Version: 2.1 Name: paibox Version: 1.1.0a2 Summary: Toolchain of
 PAICORE 2.0 Home-page: https://github.com/PAICookers/PAIBox License: GPL-3.0-
 or-later Keywords: PAICORE 2.0,PAIBox,SNN,Toolchain Author: Ziru Pan Author-
 email: zrpan@stu.pku.edu.cn Maintainer: Hongtu Xia Maintainer-email:
 hongtux@pku.edu.cn Requires-Python: >=3.8,<4.0 Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development :: Build Tools Classifier: Topic :: Software Development ::
 Libraries Requires-Dist: numpy (>=1.24.0,<2.0.0) Requires-Dist: paicorelib
-(>=1.1.1,<2.0.0) Requires-Dist: pydantic (>=2.0,<3.0) Project-URL:
+(>=1.1.2,<2.0.0) Requires-Dist: pydantic (>=2.0,<3.0) Project-URL:
 Documentation, https://github.com/PAICookers/PAIBox#readme Project-URL:
 Repository, https://github.com/PAICookers/PAIBox Description-Content-Type:
 text/markdown
                                    # PAIBox
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_p_a_i_b_o_x_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
- _v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_&_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/
+ _v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_?_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/
     _g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
 ð ç¨æ·ä½¿ç¨æåï¼[Guide-of-PAIBox](docs/Guide-of-PAIBox.md)
 é«æç¼åæµè¯é¡¹ç®æåï¼[Guide-of-Test](docs/Guide-of-Test.md)
 [Changelog](./CHANGELOG.md)
```

