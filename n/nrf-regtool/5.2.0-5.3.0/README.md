# Comparing `tmp/nrf_regtool-5.2.0.tar.gz` & `tmp/nrf_regtool-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrf_regtool-5.2.0.tar", last modified: Thu Apr 25 14:51:38 2024, max compression
+gzip compressed data, was "nrf_regtool-5.3.0.tar", last modified: Tue May 21 17:48:37 2024, max compression
```

## Comparing `nrf_regtool-5.2.0.tar` & `nrf_regtool-5.3.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 local-joni  (1000) local-joni  (1000)        0 2024-04-25 14:51:38.461704 nrf_regtool-5.2.0/
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)    11358 2024-04-25 14:47:07.000000 nrf_regtool-5.2.0/LICENSE
--rw-r--r--   0 local-joni  (1000) local-joni  (1000)    13630 2024-04-25 14:51:38.461704 nrf_regtool-5.2.0/PKG-INFO
-drwxrwxr-x   0 local-joni  (1000) local-joni  (1000)        0 2024-04-25 14:51:38.461704 nrf_regtool-5.2.0/nrf_regtool.egg-info/
--rw-r--r--   0 local-joni  (1000) local-joni  (1000)    13630 2024-04-25 14:51:38.000000 nrf_regtool-5.2.0/nrf_regtool.egg-info/PKG-INFO
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)      520 2024-04-25 14:51:38.000000 nrf_regtool-5.2.0/nrf_regtool.egg-info/SOURCES.txt
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)        1 2024-04-25 14:51:38.000000 nrf_regtool-5.2.0/nrf_regtool.egg-info/dependency_links.txt
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)       65 2024-04-25 14:51:38.000000 nrf_regtool-5.2.0/nrf_regtool.egg-info/entry_points.txt
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)       74 2024-04-25 14:51:38.000000 nrf_regtool-5.2.0/nrf_regtool.egg-info/requires.txt
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)       11 2024-04-25 14:51:38.000000 nrf_regtool-5.2.0/nrf_regtool.egg-info/top_level.txt
-drwxrwxr-x   0 local-joni  (1000) local-joni  (1000)        0 2024-04-25 14:51:38.461704 nrf_regtool-5.2.0/nrfregtool/
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)     1565 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/nrfregtool/__init__.py
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)      626 2024-04-25 14:47:07.000000 nrf_regtool-5.2.0/nrfregtool/__main__.py
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)    17162 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/nrfregtool/bicr.py
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)    18606 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/nrfregtool/cli.py
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)     9370 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/nrfregtool/common.py
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)    25372 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/nrfregtool/core.py
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)      906 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/nrfregtool/main.py
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)    15737 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/nrfregtool/parsed_dt.py
-drwxrwxr-x   0 local-joni  (1000) local-joni  (1000)        0 2024-04-25 14:51:38.461704 nrf_regtool-5.2.0/nrfregtool/resources/
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)        0 2024-04-25 14:47:07.000000 nrf_regtool-5.2.0/nrfregtool/resources/__init__.py
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)    24086 2024-04-25 14:47:07.000000 nrf_regtool-5.2.0/nrfregtool/resources/uicrextended.svd
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)    72635 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/nrfregtool/uicr.py
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)      987 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/pyproject.toml
-drwxrwxr-x   0 local-joni  (1000) local-joni  (1000)        0 2024-04-25 14:51:38.461704 nrf_regtool-5.2.0/scripts/
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)       74 2024-04-25 14:47:07.000000 nrf_regtool-5.2.0/scripts/requirements-base.txt
--rw-rw-r--   0 local-joni  (1000) local-joni  (1000)       38 2024-04-25 14:51:38.461704 nrf_regtool-5.2.0/setup.cfg
+drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-05-21 17:48:37.559389 nrf_regtool-5.3.0/
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    11358 2022-12-07 09:09:13.000000 nrf_regtool-5.3.0/LICENSE
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    13630 2024-05-21 17:48:37.559389 nrf_regtool-5.3.0/PKG-INFO
+drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-05-21 17:48:37.559389 nrf_regtool-5.3.0/nrf_regtool.egg-info/
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    13630 2024-05-21 17:48:37.000000 nrf_regtool-5.3.0/nrf_regtool.egg-info/PKG-INFO
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)      542 2024-05-21 17:48:37.000000 nrf_regtool-5.3.0/nrf_regtool.egg-info/SOURCES.txt
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)        1 2024-05-21 17:48:37.000000 nrf_regtool-5.3.0/nrf_regtool.egg-info/dependency_links.txt
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)       65 2024-05-21 17:48:37.000000 nrf_regtool-5.3.0/nrf_regtool.egg-info/entry_points.txt
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)       74 2024-05-21 17:48:37.000000 nrf_regtool-5.3.0/nrf_regtool.egg-info/requires.txt
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)       11 2024-05-21 17:48:37.000000 nrf_regtool-5.3.0/nrf_regtool.egg-info/top_level.txt
+drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-05-21 17:48:37.559389 nrf_regtool-5.3.0/nrfregtool/
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)     1565 2024-05-21 12:29:39.000000 nrf_regtool-5.3.0/nrfregtool/__init__.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)      626 2023-06-15 07:04:14.000000 nrf_regtool-5.3.0/nrfregtool/__main__.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    17162 2024-05-21 12:29:39.000000 nrf_regtool-5.3.0/nrfregtool/bicr.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    18606 2024-05-21 12:29:39.000000 nrf_regtool-5.3.0/nrfregtool/cli.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    10576 2024-05-21 17:45:26.000000 nrf_regtool-5.3.0/nrfregtool/common.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    25372 2024-05-21 12:29:39.000000 nrf_regtool-5.3.0/nrfregtool/core.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    11195 2024-05-21 17:45:26.000000 nrf_regtool-5.3.0/nrfregtool/ctrlsel.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)      906 2024-05-21 12:29:39.000000 nrf_regtool-5.3.0/nrfregtool/main.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    15737 2024-05-21 12:29:39.000000 nrf_regtool-5.3.0/nrfregtool/parsed_dt.py
+drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-05-21 17:48:37.559389 nrf_regtool-5.3.0/nrfregtool/resources/
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)        0 2024-04-28 12:59:50.000000 nrf_regtool-5.3.0/nrfregtool/resources/__init__.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    24086 2023-06-14 07:15:13.000000 nrf_regtool-5.3.0/nrfregtool/resources/uicrextended.svd
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)    73290 2024-05-21 17:45:26.000000 nrf_regtool-5.3.0/nrfregtool/uicr.py
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)      987 2024-05-21 12:29:39.000000 nrf_regtool-5.3.0/pyproject.toml
+drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-05-21 17:48:37.559389 nrf_regtool-5.3.0/scripts/
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)       74 2024-04-28 12:59:50.000000 nrf_regtool-5.3.0/scripts/requirements-base.txt
+-rw-r--r--   0 joni-l    (1000) joni-l    (1000)       38 2024-05-21 17:48:37.559389 nrf_regtool-5.3.0/setup.cfg
```

### Comparing `nrf_regtool-5.2.0/LICENSE` & `nrf_regtool-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.2.0/PKG-INFO` & `nrf_regtool-5.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrf-regtool
-Version: 5.2.0
+Version: 5.3.0
 Summary: Generate files of register content for memory-mapped peripherals.
 Author: Nordic Semiconductor ASA
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `nrf_regtool-5.2.0/nrf_regtool.egg-info/PKG-INFO` & `nrf_regtool-5.3.0/nrf_regtool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrf-regtool
-Version: 5.2.0
+Version: 5.3.0
 Summary: Generate files of register content for memory-mapped peripherals.
 Author: Nordic Semiconductor ASA
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `nrf_regtool-5.2.0/nrf_regtool.egg-info/SOURCES.txt` & `nrf_regtool-5.3.0/nrf_regtool.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,13 +8,14 @@
 nrf_regtool.egg-info/top_level.txt
 nrfregtool/__init__.py
 nrfregtool/__main__.py
 nrfregtool/bicr.py
 nrfregtool/cli.py
 nrfregtool/common.py
 nrfregtool/core.py
+nrfregtool/ctrlsel.py
 nrfregtool/main.py
 nrfregtool/parsed_dt.py
 nrfregtool/uicr.py
 nrfregtool/resources/__init__.py
 nrfregtool/resources/uicrextended.svd
 scripts/requirements-base.txt
```

### Comparing `nrf_regtool-5.2.0/nrfregtool/__init__.py` & `nrf_regtool-5.3.0/nrfregtool/__init__.py`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.2.0/nrfregtool/__main__.py` & `nrf_regtool-5.3.0/nrfregtool/__main__.py`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.2.0/nrfregtool/bicr.py` & `nrf_regtool-5.3.0/nrfregtool/bicr.py`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.2.0/nrfregtool/cli.py` & `nrf_regtool-5.3.0/nrfregtool/cli.py`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.2.0/nrfregtool/common.py` & `nrf_regtool-5.3.0/nrfregtool/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright (c) 2022 Nordic Semiconductor ASA
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
 from __future__ import annotations
 
+import dataclasses as dc
 import enum
 from collections.abc import Mapping
 from typing import Any, Dict, Sequence, Union
 
 import click
 
 _LOG_VERBOSITY = 0
@@ -203,14 +204,53 @@
             if any(substring in label for label in labels)
         }
         if len(processors) == 1:
             return processors.pop()
         return None
 
 
+# Bit position of the function bits in the pinctrl pin value encoded from NRF_PSEL()
+NRF_PSEL_FUN_POS = 17
+# Mask for the function bits in the pinctrl pin value encoded from NRF_PSEL()
+NRF_PSEL_FUN_MASK = 0x7FFF << NRF_PSEL_FUN_POS
+# Pull this from DT
+GPIO_PIN_COUNT = 32
+
+
+@dc.dataclass(frozen=True)
+class NrfPsel:
+    """Decoded NRF_PSEL values."""
+
+    fun: int
+    port: int
+    pin: int
+
+
+def nrf_psel_decode(psel_value: int) -> NrfPsel:
+    """
+    Decode an NRF_PSEL encoded GPIO pin value to its individual parts.
+
+    :param psel_value: GPIO pin value encoded with NRF_PSEL()
+    :return: A decoded tuple of GPIO (port, pin)
+    """
+    port, pin = gpio_port_pin_decode(psel_value & (~NRF_PSEL_FUN_MASK))
+    fun = (psel_value & NRF_PSEL_FUN_MASK) >> NRF_PSEL_FUN_POS
+    return NrfPsel(fun=fun, port=port, pin=pin)
+
+
+def gpio_port_pin_decode(port_pin_val: int) -> Tuple[int, int]:
+    """
+    Decode a GPIO pin value to a tuple consisting of (port, pin)
+
+    :param port_pin_val: GPIO pin value containing an encoded port and pin number
+    :return: A decoded tuple of GPIO (port, pin)
+    """
+    return (port_pin_val // GPIO_PIN_COUNT, port_pin_val % GPIO_PIN_COUNT)
+
+
 class Record(Dict[str, Dict[str, Union[str, int]]]):
     """
     A transcript of the contents of any number of registers and their fields.
     A basic Record is one that is not complete with register instance information, while a complete
     Record is one that also carries instance information.
 
     Basic example: "mem_config"
```

### Comparing `nrf_regtool-5.2.0/nrfregtool/core.py` & `nrf_regtool-5.3.0/nrfregtool/core.py`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.2.0/nrfregtool/main.py` & `nrf_regtool-5.3.0/nrfregtool/main.py`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.2.0/nrfregtool/parsed_dt.py` & `nrf_regtool-5.3.0/nrfregtool/parsed_dt.py`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.2.0/nrfregtool/resources/uicrextended.svd` & `nrf_regtool-5.3.0/nrfregtool/resources/uicrextended.svd`

 * *Files identical despite different names*

### Comparing `nrf_regtool-5.2.0/nrfregtool/uicr.py` & `nrf_regtool-5.3.0/nrfregtool/uicr.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,27 +21,30 @@
 from .common import (
     AddressRegion,
     DomainID,
     OwnerID,
     ProcessorID,
     Record,
     else_none,
+    gpio_port_pin_decode,
     log_dbg,
     log_dev,
     log_vrb,
+    nrf_psel_decode,
     verbose_logs,
 )
+from .ctrlsel import CTRLSEL_DEFAULT, dt_lookup_ctrlsel
 from .parsed_dt import (
+    PARTITION_COMPAT_REGEX,
     ExtractedConfig,
     IndexedBy,
     IndexedByInstance,
     IndexedByPosition,
     InterpretedPeripheral,
     NodeChannels,
-    PARTITION_COMPAT_REGEX,
     ParsedDTNode,
     PeripheralResult,
     ProcessorInfo,
     dt_processor_info,
     sort_configs_by_type,
 )
 
@@ -80,21 +83,16 @@
     ),
 ]
 
 
 # Regex for memory region compatibles that should be allocated via UICR
 MEM_COMPAT_REGEX = re.compile(r"^nordic,owned-(memory|partitions)$")
 
-
-# Pull this from DT
-GPIO_PIN_COUNT = 32
-
-
-# Mask for the function bits in the pinctrl pin value encoded from NRF_PSEL()
-NRF_PSEL_FUN_MASK = 0xFFFF << 16
+# Dimension of the UICR.GPIO[].PIN[] register
+GPIO_PIN_CTRLSEL_PER_PORT = 14
 
 # Collection of logs from extract functions
 UICR_LOGS = defaultdict(list)
 
 
 class DppiLogInfo(NamedTuple):
     """Helper tuple for DPPI logging information."""
@@ -216,14 +214,15 @@
 @dataclass(frozen=True, order=True)
 class GpioConfig(ExtractedConfig):
     """General purpose I/O (GPIO) configuration."""
 
     instance: ParsedDTNode
     owned_pins: List[int] = dc.field(default_factory=list)
     nonsecure_pins: List[int] = dc.field(default_factory=list)
+    pin_ctrlsels: Dict[int, int] = dc.field(default_factory=dict)
 
     def __post_init__(self):
         self.owned_pins.sort()
         self.nonsecure_pins.sort()
 
     @property
     def indexed_by(self) -> IndexedBy:
@@ -236,14 +235,19 @@
             record[f"gpio_own_{index}"] = make_pin_fields(self.owned_pins, SvdEnum.OWN)
 
         if self.nonsecure_pins:
             record[f"gpio_secure_{index}"] = make_pin_fields(
                 self.nonsecure_pins, SvdEnum.NONSECURE
             )
 
+        if self.pin_ctrlsels:
+            for pin, ctrlsel in self.pin_ctrlsels.items():
+                flat_index = index * GPIO_PIN_CTRLSEL_PER_PORT + pin
+                record[f"gpio_pin_ctrlsel_{flat_index}"] = {"CTRLSEL": ctrlsel}
+
         return record
 
 
 @dataclass(frozen=True, order=True)
 class MemoryConfig(ExtractedConfig):
     """Memory configuration."""
 
@@ -632,14 +636,15 @@
     """
     Helper tuple for pin-related information.
     """
 
     port: int
     pin: int
     secure: bool
+    ctrlsel: Optional[int]
 
 
 @enum.unique
 class SourceMapIndex(enum.IntEnum):
     """
     Enumeration of indices in the IPCT array property that defines channel/domain info for when the
     owning domain is a source.
@@ -708,15 +713,15 @@
 
         :param devicetree: edtlib Devicetree object
         """
         super().__init__(devicetree=devicetree, name="UICR")
 
         self._processor: ProcessorInfo = dt_processor_info(devicetree)
         self._resource_nodes = defaultdict(list)
-        self._gpios: List[edtlib.ControllerAndData] = []
+        self._gpios: List[edtlib.Property] = []
         self._pinctrls: List[edtlib.PinCtrl] = []
         self._gpio_pins: List[edtlib.Property] = []
         self._uicr_node: Optional[ParsedDTNode] = None
 
         has_relevant_status = lambda n: (n.enabled or n.reserved)
         has_relevant_address = lambda n: (
             n.domain == DomainID.GLOBAL
@@ -768,20 +773,21 @@
             elif has_relevant_status(node) and (
                 node.compatibles_contain(ResourceCompatible.MAILBOX_ICMSG.value)
                 or node.compatibles_contain(ResourceCompatible.MAILBOX_RPMSG.value)
             ):
                 self._resource_nodes[NodeType.MAILBOX].append(node)
 
             if has_relevant_status(node) or "status" not in node.properties:
-                gpios_props = filter(_is_gpios_prop, node.properties.values())
-                gpios = filter(
-                    _has_nordic_gpio_controller,
-                    chain.from_iterable(prop.val for prop in gpios_props),
+                gpios_props = (
+                    prop
+                    for prop in node.properties.values()
+                    if _is_gpios_prop(prop)
+                    and any((_has_nordic_gpio_controller(v) for v in prop.val))
                 )
-                self._gpios.extend(gpios)
+                self._gpios.extend(gpios_props)
             if has_relevant_status(node) and node.compatibles_contain("nordic"):
                 self._pinctrls.extend(node.pinctrls)
 
                 gpio_pin_props = [
                     p for p in node.properties.values() if p.name.endswith("-pin")
                 ]
                 if gpio_pin_props:
@@ -945,15 +951,15 @@
     def gpio_pin_props(self) -> List[edtlib.Property]:
         """
         GPIO pin properties that are relevant for UICR.
         """
         return self._gpio_pins
 
     @property
-    def gpios(self) -> List[edtlib.ControllerAndData]:
+    def gpios(self) -> List[edtlib.Property]:
         """
         'gpios' property entries referencing GPIO pins that are relevant for UICR.
         """
         return self._gpios
 
     @property
     def pinctrls(self) -> List[edtlib.PinCtrl]:
@@ -1328,42 +1334,22 @@
 
 
 def _has_nordic_gpio_controller(gpios_entry: edtlib.ControllerAndData) -> bool:
     """Returns True if gpios_entry refers to a nordic GPIO node"""
     return ResourceCompatible.GPIO.value in gpios_entry.controller.compats
 
 
-def _gpio_port_pin_decode(port_pin_val: int) -> Tuple[int, int]:
-    """
-    Decode a GPIO pin value to a tuple consisting of (port, pin)
-
-    :param port_pin_val: GPIO pin value containing an encoded port and pin number
-    :return: A decoded tuple of GPIO (port, pin)
-    """
-    return (port_pin_val // GPIO_PIN_COUNT, port_pin_val % GPIO_PIN_COUNT)
-
-
-def _nrf_psel_decode(psel_value: int) -> Tuple[int, int]:
-    """
-    Decode an NRF_PSEL encoded GPIO pin value to a tuple consisting of (port, pin)
-
-    :param psel_value: GPIO pin value encoded with NRF_PSEL()
-    :return: A decoded tuple of GPIO (port, pin)
-    """
-    port_pin = psel_value & (~NRF_PSEL_FUN_MASK)
-    return _gpio_port_pin_decode(port_pin)
-
-
 def _gpio_pin_security_from_node(node: edtlib.Node) -> bool:
     """Get the security level of GPIO pin based on the security of the node using it"""
     node_secure = ParsedDTNode(node).secure
     return node_secure if node_secure is not None else True
 
 
 def _extract_gpios_prop_pin(
+    gpios_prop: edtlib.Property,
     gpios_entry: edtlib.ControllerAndData,
 ) -> GpioPin:
     """
     Get the set of GPIO pins present in the given *-gpios property.
 
     :param gpios_entry: an entry in a 'gpios' property
     :return: A (port, pin) tuple representing the GPIO pin used in the property
@@ -1373,15 +1359,16 @@
         "controller": {"port": gpios_entry.controller.props["port"].val},
         "data": dict(gpios_entry.data),
     }
 
     port: int = cell_data["controller"]["port"]
     pin: int = cell_data["data"]["pin"]
     secure = _gpio_pin_security_from_node(gpios_entry.node)
-    gpio_pin = GpioPin(port=port, pin=pin, secure=secure)
+    ctrlsel = dt_lookup_ctrlsel(gpios_prop, (port, pin))
+    gpio_pin = GpioPin(port=port, pin=pin, secure=secure, ctrlsel=ctrlsel)
 
     _append_log_config(
         ConfigTypeEnum.GPIO, GpiosLogInfo(gpio_pin, gpios_entry, cell_data)
     )
 
     return gpio_pin
 
@@ -1397,28 +1384,31 @@
     pins: Set[GpioPin] = set()
 
     secure = _gpio_pin_security_from_node(pinctrl.node)
 
     for config_node in pinctrl.conf_nodes:
         for group_node in config_node.children.values():
             for psel_val in group_node.props["psels"].val:
-                port, pin = _nrf_psel_decode(psel_val)
-                gpio_pin = GpioPin(port=port, pin=pin, secure=secure)
+                psel = nrf_psel_decode(psel_val)
+                ctrlsel = dt_lookup_ctrlsel(pinctrl, psel)
+                gpio_pin = GpioPin(
+                    port=psel.port, pin=psel.pin, secure=secure, ctrlsel=ctrlsel
+                )
                 pins.add(gpio_pin)
 
                 _append_log_config(
                     ConfigTypeEnum.GPIO,
                     PinctrlLogInfo(gpio_pin, config_node, group_node),
                 )
 
     return pins
 
 
 def _gpio_pins_from_props(
-    gpios: List[edtlib.ControllerAndData],
+    gpios: List[edtlib.Property],
     pinctrls: List[edtlib.PinCtrl],
     gpio_pin_props: List[edtlib.Property],
 ) -> Set[GpioPin]:
     """
     Extract a list of GPIO pins from devicetree objects containing GPIO pin usage information.
 
     :param gpios: 'gpios' property entries
@@ -1426,35 +1416,42 @@
     :param gpio_pin_props: List of GPIO pin properties
 
     :return: List of GPIO pins used by the given devicetree objects
     """
 
     pins: Set[GpioPin] = set()
 
-    gpios_pins = (_extract_gpios_prop_pin(gpio) for gpio in gpios)
-    pins.update(gpios_pins)
+    for gpios_prop in gpios:
+        for gpios_entry in gpios_prop.val:
+            if _has_nordic_gpio_controller(gpios_entry):
+                gpio_pin = _extract_gpios_prop_pin(gpios_prop, gpios_entry)
+                pins.add(gpio_pin)
+            else:
+                print(f"Mismatch on controller of: {gpios_entry}: {gpios_entry.controller.compats}")
 
     for pinctrl in pinctrls:
         pinctrl_pins = _extract_pinctrl_prop_pins(pinctrl)
         pins.update(pinctrl_pins)
 
     for prop in gpio_pin_props:
-        prop_port, prop_pin = _gpio_port_pin_decode(prop.val)
+        prop_port, prop_pin = gpio_port_pin_decode(prop.val)
         secure = _gpio_pin_security_from_node(prop.node)
-        gpio_pin = GpioPin(port=prop_port, pin=prop_pin, secure=secure)
+        gpio_pin = GpioPin(
+            port=prop_port, pin=prop_pin, secure=secure, ctrlsel=None
+        )
         pins.add(gpio_pin)
 
         _append_log_config(ConfigTypeEnum.GPIO, PinPropLogInfo(gpio_pin, prop))
 
     return pins
 
 
 def extract_gpio_configs(
     nodes: List[ParsedDTNode],
-    gpios: List[edtlib.ControllerAndData],
+    gpios: List[edtlib.Property],
     pinctrls: List[edtlib.PinCtrl],
     gpio_pin_props: List[edtlib.Property] = [],
 ) -> List[GpioConfig]:
     """
     Extract GPIO record information from parsed devicetree properties.
 
     :param nodes: Parsed devicetree nodes
@@ -1482,22 +1479,28 @@
         except KeyError:
             raise RuntimeError(
                 f"GPIO port {port=} is not in supported ports ({port_to_instance.keys()})"
             )
 
         owned_pins: List[int] = []
         ns_pins: List[int] = []
+        pin_ctrlsels: Dict[int, int] = {}
 
         for pin in sorted(gpio_pins, key=lambda p: p.pin):
             owned_pins.append(pin.pin)
+            if pin.ctrlsel is not None:
+                pin_ctrlsels[pin.pin] = pin.ctrlsel
             if not pin.secure:
                 ns_pins.append(pin.pin)
 
         config = GpioConfig(
-            instance=instance, owned_pins=owned_pins, nonsecure_pins=ns_pins
+            instance=instance,
+            owned_pins=owned_pins,
+            nonsecure_pins=ns_pins,
+            pin_ctrlsels=pin_ctrlsels,
         )
 
         configs.append(config)
 
     return configs
 
 
@@ -2123,23 +2126,26 @@
     """Log GPIO configurations extracted from UICR."""
 
     pinctrl_nodes = defaultdict(list)
 
     for info in gpio_log_info:
         port = info.gpio.port
         pin = info.gpio.pin
+        ctrlsel = info.gpio.ctrlsel
         secure = info.gpio.secure
 
         if isinstance(info, PinctrlLogInfo):
             # Group them by nodes to avoid duplicate pin outputs, since pinctrl can have multiple
             # nodelabel alternatives reference the same pin info.
             pinctrl_nodes[f"P{port}.{pin}"].append(info)
 
         elif isinstance(info, GpiosLogInfo):
             log_vrb(f"P{port}.{pin}")
+            if ctrlsel is not None:
+                log_vrb(f"\tCTRLSEL: {ctrlsel}")
             log_vrb(f"\tSecure: {bool(secure)}")
             log_vrb(f"\tNode: {info.ctrldata.node.name}")
             log_dbg(f"\tSource: {info.ctrldata.node.path}")
 
             if info.ctrldata.controller.labels:
                 log_dbg(
                     f"\tgpios: <&{info.ctrldata.controller.labels[0]} {pin} {info.cell_data['data']['flags']}>"
@@ -2148,25 +2154,29 @@
                 log_dbg(
                     f"\tController: {info.ctrldata.controller.name}@{info.ctrldata.controller.path}"
                 )
                 log_dbg(f"\tProperties: <{info.cell_data}>")
 
         else:
             log_vrb(f"P{port}.{pin}")
+            if ctrlsel != CTRLSEL_DEFAULT:
+                log_vrb(f"\tCTRLSEL: {ctrlsel}")
             log_vrb(f"\tSecure: {bool(secure)}")
             node_name = (
                 f"{info.prop.node.labels[0]}"
                 if info.prop.node.labels
                 else f"{info.prop.node.name}"
             )
             log_vrb(f"\tSource: {node_name}@{info.prop.node.path}")
             log_dbg(f"Property: {info.prop}")
 
     for pinset, nodes in pinctrl_nodes.items():
         log_vrb(pinset)
+        if nodes[-1].gpio.ctrlsel is not None:
+            log_vrb(f"\tCTRLSEL: {nodes[-1].gpio.ctrlsel}")
         log_vrb(f"\tSecure: {bool(secure)}")
         log_vrb(f"\tPinctrl:")
         for node in nodes:
             log_vrb(f"\t\tNode: {node.config_node.name}")
             log_dbg(f"\t\tSource: {node.group_node.path}")
             log_dbg(f"\t\tProperty: {node.group_node.props['psels']}")
```

### Comparing `nrf_regtool-5.2.0/pyproject.toml` & `nrf_regtool-5.3.0/pyproject.toml`

 * *Files identical despite different names*

