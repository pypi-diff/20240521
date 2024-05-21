# Comparing `tmp/mosaik-3.3.2.tar.gz` & `tmp/mosaik-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaik-3.3.2.tar", last modified: Fri Apr 12 12:40:02 2024, max compression
+gzip compressed data, was "mosaik-3.3.3.tar", max compression
```

## Comparing `mosaik-3.3.2.tar` & `mosaik-3.3.3.tar`

### file list

```diff
@@ -1,47 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:40:02.456640 mosaik-3.3.2/
--rw-rw-rw-   0 root         (0) root         (0)      479 2024-04-08 13:12:09.000000 mosaik-3.3.2/AUTHORS.txt
--rw-rw-rw-   0 root         (0) root         (0)    24436 2024-04-03 06:59:03.000000 mosaik-3.3.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    17285 2024-04-12 12:40:02.456640 mosaik-3.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3536 2024-04-08 13:12:09.000000 mosaik-3.3.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:40:02.452639 mosaik-3.3.2/mosaik/
--rw-rw-rw-   0 root         (0) root         (0)      490 2024-04-08 13:12:09.000000 mosaik-3.3.2/mosaik/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7024 2024-04-08 13:12:09.000000 mosaik-3.3.2/mosaik/_debug.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-08 13:12:09.000000 mosaik-3.3.2/mosaik/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     5837 2024-04-08 13:12:09.000000 mosaik-3.3.2/mosaik/adapters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:40:02.452639 mosaik-3.3.2/mosaik/basic_simulators/
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-04-03 06:59:03.000000 mosaik-3.3.2/mosaik/basic_simulators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3637 2024-04-08 13:12:09.000000 mosaik-3.3.2/mosaik/basic_simulators/input_simulator.py
--rw-rw-rw-   0 root         (0) root         (0)     2265 2024-04-08 13:12:09.000000 mosaik-3.3.2/mosaik/basic_simulators/output_simulator.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2024-04-08 13:12:09.000000 mosaik-3.3.2/mosaik/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4069 2024-04-08 13:12:09.000000 mosaik-3.3.2/mosaik/in_or_out_set.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-08 13:12:09.000000 mosaik-3.3.2/mosaik/internal_util.py
--rw-rw-rw-   0 root         (0) root         (0)     4224 2024-04-08 13:12:09.000000 mosaik-3.3.2/mosaik/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     7745 2024-04-08 13:12:09.000000 mosaik-3.3.2/mosaik/proxies.py
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-03 06:59:03.000000 mosaik-3.3.2/mosaik/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    44209 2024-04-08 13:12:09.000000 mosaik-3.3.2/mosaik/scenario.py
--rw-rw-rw-   0 root         (0) root         (0)    17830 2024-04-08 13:12:09.000000 mosaik-3.3.2/mosaik/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)    27154 2024-04-12 12:29:21.000000 mosaik-3.3.2/mosaik/simmanager.py
--rw-rw-rw-   0 root         (0) root         (0)     3235 2024-04-08 13:12:09.000000 mosaik-3.3.2/mosaik/tiered_time.py
--rw-rw-rw-   0 root         (0) root         (0)    20903 2024-04-08 13:12:09.000000 mosaik-3.3.2/mosaik/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:40:02.456640 mosaik-3.3.2/mosaik.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17285 2024-04-12 12:40:02.000000 mosaik-3.3.2/mosaik.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      931 2024-04-12 12:40:02.000000 mosaik-3.3.2/mosaik.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 12:40:02.000000 mosaik-3.3.2/mosaik.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2024-04-12 12:40:02.000000 mosaik-3.3.2/mosaik.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-12 12:40:02.000000 mosaik-3.3.2/mosaik.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1438 2024-04-12 12:29:21.000000 mosaik-3.3.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-04-12 12:40:02.456640 mosaik-3.3.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1775 2024-04-12 12:29:21.000000 mosaik-3.3.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:40:02.456640 mosaik-3.3.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2255 2024-04-08 13:12:09.000000 mosaik-3.3.2/tests/test_adapters.py
--rw-rw-rw-   0 root         (0) root         (0)     5307 2024-04-08 13:12:09.000000 mosaik-3.3.2/tests/test_attr_specification.py
--rw-rw-rw-   0 root         (0) root         (0)     1540 2024-04-08 13:12:09.000000 mosaik-3.3.2/tests/test_basic_simulators.py
--rw-rw-rw-   0 root         (0) root         (0)      809 2024-04-03 06:59:03.000000 mosaik-3.3.2/tests/test_benchmarks.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2024-04-03 06:59:03.000000 mosaik-3.3.2/tests/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2314 2024-04-08 13:12:09.000000 mosaik-3.3.2/tests/test_mosaik.py
--rw-rw-rw-   0 root         (0) root         (0)    15735 2024-04-08 13:12:09.000000 mosaik-3.3.2/tests/test_scenario.py
--rw-rw-rw-   0 root         (0) root         (0)    16921 2024-04-08 13:12:09.000000 mosaik-3.3.2/tests/test_scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)    20583 2024-04-12 12:29:21.000000 mosaik-3.3.2/tests/test_simmanager.py
--rw-rw-rw-   0 root         (0) root         (0)     2380 2024-04-08 13:12:09.000000 mosaik-3.3.2/tests/test_tiered_time.py
--rw-rw-rw-   0 root         (0) root         (0)      717 2024-04-08 13:12:09.000000 mosaik-3.3.2/tests/test_tutorial.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2024-04-03 06:59:03.000000 mosaik-3.3.2/tests/test_util.py
+-rw-r--r--   0        0        0      479 2024-05-21 08:56:36.149355 mosaik-3.3.3/AUTHORS.rst
+-rw-r--r--   0        0        0    12418 2024-05-21 12:33:07.179197 mosaik-3.3.3/CHANGES.rst
+-rw-r--r--   0        0        0    24436 2024-05-17 09:34:17.456184 mosaik-3.3.3/LICENSE.txt
+-rw-r--r--   0        0        0     3536 2024-05-17 09:34:17.456184 mosaik-3.3.3/README.rst
+-rw-r--r--   0        0        0      494 2024-05-21 09:15:36.016036 mosaik-3.3.3/mosaik/__init__.py
+-rw-r--r--   0        0        0     7024 2024-05-17 09:34:17.772188 mosaik-3.3.3/mosaik/_debug.py
+-rw-r--r--   0        0        0       69 2024-05-21 12:04:39.787438 mosaik-3.3.3/mosaik/_version.py
+-rw-r--r--   0        0        0     5837 2024-05-17 09:34:17.772188 mosaik-3.3.3/mosaik/adapters.py
+-rw-r--r--   0        0        0       89 2024-05-17 09:34:17.776188 mosaik-3.3.3/mosaik/basic_simulators/__init__.py
+-rw-r--r--   0        0        0     3637 2024-05-17 09:34:17.776188 mosaik-3.3.3/mosaik/basic_simulators/input_simulator.py
+-rw-r--r--   0        0        0     2265 2024-05-17 09:34:17.776188 mosaik-3.3.3/mosaik/basic_simulators/output_simulator.py
+-rw-r--r--   0        0        0     1541 2024-05-21 08:56:36.149355 mosaik-3.3.3/mosaik/exceptions.py
+-rw-r--r--   0        0        0     1313 2024-05-21 09:31:35.352775 mosaik-3.3.3/mosaik/greetings_util.py
+-rw-r--r--   0        0        0     4069 2024-05-17 09:34:17.776188 mosaik-3.3.3/mosaik/in_or_out_set.py
+-rw-r--r--   0        0        0     1760 2024-05-21 09:15:36.016036 mosaik-3.3.3/mosaik/internal_util.py
+-rw-r--r--   0        0        0     4224 2024-05-17 09:34:17.776188 mosaik-3.3.3/mosaik/progress.py
+-rw-r--r--   0        0        0     7678 2024-05-21 08:56:36.149355 mosaik-3.3.3/mosaik/proxies.py
+-rw-r--r--   0        0        0        1 2024-05-17 09:34:17.776188 mosaik-3.3.3/mosaik/py.typed
+-rw-r--r--   0        0        0    44797 2024-05-21 12:04:39.787438 mosaik-3.3.3/mosaik/scenario.py
+-rw-r--r--   0        0        0    17750 2024-05-21 08:56:36.153355 mosaik-3.3.3/mosaik/scheduler.py
+-rw-r--r--   0        0        0    27992 2024-05-21 08:56:36.153355 mosaik-3.3.3/mosaik/simmanager.py
+-rw-r--r--   0        0        0     3235 2024-05-17 09:34:17.776188 mosaik-3.3.3/mosaik/tiered_time.py
+-rw-r--r--   0        0        0    20903 2024-05-17 09:34:17.776188 mosaik-3.3.3/mosaik/util.py
+-rw-r--r--   0        0        0     2055 2024-05-21 12:33:07.179197 mosaik-3.3.3/pyproject.toml
+-rw-r--r--   0        0        0    17738 1970-01-01 00:00:00.000000 mosaik-3.3.3/PKG-INFO
```

### Comparing `mosaik-3.3.2/LICENSE.txt` & `mosaik-3.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mosaik-3.3.2/PKG-INFO` & `mosaik-3.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: mosaik
-Version: 3.3.2
-Summary: Mosaik is a flexible Smart-Grid co-simulation framework.
-Home-page: https://mosaik.offis.de
+Version: 3.3.3
+Summary: mosaik is a flexible smart-grid co-simulation framework
+Home-page: https://mosaik.offis.de/
+License: LGPL-2.1-only
 Author: mosaik development team
 Author-email: mosaik@offis.de
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
+Classifier: License :: OSI Approved
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: loguru (>=0.6,<1)
+Requires-Dist: mosaik-api-v3 (>=3.0.10,<4.0.0)
+Requires-Dist: networkx (>=2.5,<3.0)
+Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Requires-Dist: typing-extensions (>=4.5,<5.0)
+Project-URL: Documentation, https://mosaik.readthedocs.io/
+Project-URL: Repository, https://gitlab.com/mosaik/mosaik
 Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-License-File: AUTHORS.txt
-Requires-Dist: networkx>=2.5
-Requires-Dist: mosaik-api-v3>=3.0.7
-Requires-Dist: loguru>=0.6.0
-Requires-Dist: tqdm>=4.64.1
-Requires-Dist: typing-extensions>=4.5.0
 
 Mosaik
 ======
 
 Mosaik is a simulation compositor for Smart Grid simulations.
 
 It lets you re-use existing simulators and couple them to simulate large-scale
@@ -109,18 +110,24 @@
     }
 
 Get in touch, ask questions, discuss 💬
 ---------------------------------------
 You have a question, a feature request or want to generally discuss the amazing 
 possibilities with co-simulation and mosaik? We are curious to hear from you! 
 Join us on `GitHub Discussions <https://github.com/orgs/OFFIS-mosaik/discussions>`_.
-
 Changelog
 =========
 
+3.3.3 - 2024-05-21
+------------------
+
+- [NEW] mosaik greeting with ASCII art and version information, contact links (https://gitlab.com/mosaik/mosaik/-/issues/216)
+- [NEW] Better error messages on remote errors (https://gitlab.com/mosaik/mosaik/-/issues/234)
+- [FIX] Error message for serialization errors assigns blame correctly (https://gitlab.com/mosaik/mosaik/-/issues/232)
+
 3.3.2 - 2024-04-12
 ------------------
 
 - [FIX] Fix versioning issue
 
 3.3.1 - 2024-04-12
 ------------------
@@ -425,20 +432,20 @@
  You can find information about older versions on the `history page`__
 
 __ https://gitlab.com/mosaik/mosaik-hdf5
 __ https://gitlab.com/mosaik/mosaik-api-python
 __ https://gitlab.com/mosaik/mosaik-api-java
 __ https://mosaik.readthedocs.org/en/latest/about/history.html
 
-
 Authors
 =======
 
 The original concepts for mosaik were developed by Steffen Schütte and Stefan
 Scherfke.
 
 The author of mosaik version 2 is Stefan Scherfke.
 
 Current and former members of the mosaik team: Sharaf Alsharif, Tobias Brandt, Reef Eilers, André El-Ama,
 Bengt Lüers, Okko Nannen, Annika Ofenloch, Mostafa Ramezani, Thomas Raub,
 Stefan Scherfke, Florian Schloegl, Eike Schulte, Steffen Schütte, Jan Sören Schwarz,
 Cornelius Steinbrink, Malte Stomberg, Deborah Tolk
+
```

### Comparing `mosaik-3.3.2/README.rst` & `mosaik-3.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `mosaik-3.3.2/mosaik/_debug.py` & `mosaik-3.3.3/mosaik/_debug.py`

 * *Files identical despite different names*

### Comparing `mosaik-3.3.2/mosaik/adapters.py` & `mosaik-3.3.3/mosaik/adapters.py`

 * *Files identical despite different names*

### Comparing `mosaik-3.3.2/mosaik/basic_simulators/input_simulator.py` & `mosaik-3.3.3/mosaik/basic_simulators/input_simulator.py`

 * *Files identical despite different names*

### Comparing `mosaik-3.3.2/mosaik/basic_simulators/output_simulator.py` & `mosaik-3.3.3/mosaik/basic_simulators/output_simulator.py`

 * *Files identical despite different names*

### Comparing `mosaik-3.3.2/mosaik/in_or_out_set.py` & `mosaik-3.3.3/mosaik/in_or_out_set.py`

 * *Files identical despite different names*

### Comparing `mosaik-3.3.2/mosaik/progress.py` & `mosaik-3.3.3/mosaik/progress.py`

 * *Files identical despite different names*

### Comparing `mosaik-3.3.2/mosaik/proxies.py` & `mosaik-3.3.3/mosaik/proxies.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 from mosaik_api_v3.types import Meta, SimId
 from mosaik.exceptions import ScenarioError
 
 
 class Proxy(ABC):
     """A proxy for a mosaik simulator from the view of a mosaik
     scenario.
-    
+
     Generally, this will be a ``BaseProxy`` subclass wrapped in the
     appropriate ``Adapter`` subclasses to bring the interface of the
     connected simulator in line with the most up-to-date API version.
     """
     @abstractmethod
     async def send(self, request: Any) -> Any:
         """Send a request to the connected simulator.
-        
+
         :param request: Generally, this will be a three-tuple consisting
         of a function name, a list of positional arguments and a dict
         of named arguments.
         :return: The return value from the remote simulator (depends on
         the specified function).
         """
         raise NotImplementedError()
@@ -180,29 +180,26 @@
                 "Something went wrong in _handle_remote_requests, "
                 f"exception type {type(e)}")
             await self.stop()
 
     async def init(self, sid: SimId, **kwargs: Any) -> List[int]:
         self._meta = await self.send(["init", (sid,), kwargs])
         return extract_version(self._meta)
-    
+
     @property
     def meta(self) -> Meta:
         return self._meta
-    
+
     async def send(self, request: Any) -> Any:
         return await self._channel.send(request)
 
     async def stop(self) -> None:
         try:
-            await asyncio.wait_for(
-                self._channel.send(["stop", [], {}]),
-                0.1,
-            )
-        except (asyncio.IncompleteReadError, asyncio.TimeoutError):
+            await asyncio.wait_for(self._channel.send(["stop", [], {}]), 0.1)
+        except (asyncio.TimeoutError, asyncio.IncompleteReadError):
             pass
         await self._channel.close()
         await self._reader_task
 
 
 def extract_version(meta: Meta) -> List[int]:
     if "api_version" not in meta:
```

### Comparing `mosaik-3.3.2/mosaik/scenario.py` & `mosaik-3.3.3/mosaik/scenario.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from __future__ import annotations
 
 import asyncio
 from collections import defaultdict
 import contextlib
 from copy import copy
 from dataclasses import dataclass
+from mosaik.greetings_util import print_greetings
 import itertools
 from loguru import logger
 from mosaik_api_v3 import OutputData, OutputRequest
 import networkx
 from tqdm import tqdm
 from typing import (
     TYPE_CHECKING,
@@ -34,14 +35,15 @@
     TypeVar,
     Union,
 )
 import warnings
 from typing_extensions import Literal, TypeAlias, TypedDict
 
 from mosaik_api_v3.types import Attr, CreateResult, EntityId, FullId, ModelDescription, ModelName, SimId
+from mosaik_api_v3.connection import RemoteException
 
 from mosaik import simmanager
 from mosaik.internal_util import doc_link
 from mosaik.proxies import Proxy
 from mosaik.simmanager import SimRunner, MosaikConfigTotal
 from mosaik import scheduler
 from mosaik.exceptions import ScenarioError, SimulationError
@@ -235,15 +237,18 @@
         sim_config: SimConfig,
         mosaik_config: Optional[MosaikConfig] = None,
         time_resolution: float = 1.,
         debug: bool = False,
         cache: bool = True,
         max_loop_iterations: int = 100,
         asyncio_loop: Optional[asyncio.AbstractEventLoop] = None,
+        skip_greetings: bool = False
     ):
+        if not skip_greetings:
+            print_greetings()
         self.sim_config = sim_config
 
         self.config = copy(base_config)
         if mosaik_config:
             self.config.update(mosaik_config)
 
         self.sims = {}
@@ -679,14 +684,23 @@
         try:
             self.loop.run_until_complete(scheduler.run(
                 self, until, rt_factor, rt_strict, lazy_stepping
             ))
             success = True
         except KeyboardInterrupt:
             logger.info('Simulation canceled. Terminating ...')
+        except RemoteException as exc:
+            logger.error(
+                f"Simulator {exc.source} aborted the simulation with error "
+                f"{exc.remote_type}({exc.remote_msg})." + (
+                    " Further information provided:\n" + "\n".join(exc.further_args)
+                    if exc.further_args
+                    else ""
+                )
+            )
         finally:
             for sid, sim in self.sims.items():
                 sim.tqdm.close()
             self.tqdm.close()
             self.shutdown()
             if self._debug:
                 dbg.disable()
```

### Comparing `mosaik-3.3.2/mosaik/scheduler.py` & `mosaik-3.3.3/mosaik/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from loguru import logger
 from math import ceil
 from time import perf_counter
 
 from mosaik_api_v3 import InputData, SimId, Time
 
 from mosaik.exceptions import SimulationError
-from mosaik.internal_util import recursive_merge_all, recursive_merge_existing
+from mosaik.internal_util import merge_all, merge_existing
 from mosaik.simmanager import FULL_ID, SimRunner
 
 from typing import TYPE_CHECKING, Any, Coroutine, Dict, List, Optional
 
 from mosaik.tiered_time import TieredTime
 if TYPE_CHECKING:
     from mosaik.scenario import World
@@ -235,17 +235,17 @@
     assert sim.current_step is not None
     # Input data starts with the data from set_data calls
     input_data = sim.inputs_from_set_data
     sim.inputs_from_set_data = {}
     # Merge the persistent inputs into the input data, adding keys as
     # necessary. mosaik controls three levels deep, all further levels
     # therefore should not be merged.
-    recursive_merge_all(
-        lambda attrs_new, attrs_old: recursive_merge_all(
-            lambda data_new, data_old: recursive_merge_all(
+    merge_all(
+        lambda attrs_new, attrs_old: merge_all(
+            lambda data_new, data_old: merge_all(
                 lambda val_new, val_old: val_new, data_new, data_old
             ),
             attrs_new,
             attrs_old,
         ),
         input_data,
         sim.persistent_inputs,
@@ -270,17 +270,17 @@
                 val = None
             input_vals = input_data.setdefault(dest_eid, {}).setdefault(dest_attr, {})
             input_vals[FULL_ID % (src_sim.sid, src_eid)] = val
 
     # Merge the data back into the persistent inputs. Here, only keys
     # that already exist should be updated, as those are the persistent
     # attributes. (Adding others would make those persistent as well.)
-    recursive_merge_existing(
-        lambda attrs_old, attrs_new: recursive_merge_existing(
-            lambda data_old, data_new: recursive_merge_existing(
+    merge_existing(
+        lambda attrs_old, attrs_new: merge_existing(
+            lambda data_old, data_new: merge_existing(
                 lambda val_old, val_new: val_new, data_old, data_new
             ),
             attrs_old,
             attrs_new,
         ),
         sim.persistent_inputs,
         input_data,
```

### Comparing `mosaik-3.3.2/mosaik/simmanager.py` & `mosaik-3.3.3/mosaik/simmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import importlib
 import itertools
 import os
 import shlex
 import subprocess
 import sys
 import platform
+from json import JSONEncoder
 from loguru import logger
 from typing import (
     Any,
     Callable,
     Coroutine,
     Dict,
     List,
@@ -38,15 +39,15 @@
 )
 import tqdm
 from typing_extensions import Literal, TypeAlias, TypedDict
 
 import mosaik_api_v3
 from mosaik_api_v3.connection import Channel
 from mosaik_api_v3.types import OutputData, OutputRequest, SimId, Time, InputData, Attr, EntityId, FullId
-from mosaik.exceptions import ScenarioError, SimulationError
+from mosaik.exceptions import NonSerializableOutputsError, ScenarioError, SimulationError
 from mosaik.progress import Progress
 from mosaik.proxies import Proxy, LocalProxy, BaseProxy, RemoteProxy
 from mosaik.adapters import init_and_get_adapter
 from mosaik.tiered_time import TieredInterval, TieredTime
 
 if 'Windows' in platform.system():
     from subprocess import CREATE_NEW_CONSOLE  # type: ignore (only Windows)
@@ -216,15 +217,15 @@
     Return a :class:`RemoteProcess` instance.
 
     Raise a :exc:`~mosaik.exceptions.ScenarioError` if the simulator cannot be
     instantiated.
     """
     channel_future: asyncio.Future[Channel] = asyncio.Future()
     async def on_connect(r: asyncio.StreamReader, w: asyncio.StreamWriter):
-        channel_future.set_result(Channel(r, w))
+        channel_future.set_result(Channel(r, w, name=sim_name))
 
     server = await asyncio.start_server(on_connect, *mosaik_config["addr"])
     try:
         actual_addr = server.sockets[0].getsockname()
 
         replacements = {
             "addr": "%s:%s" % actual_addr,
@@ -314,15 +315,15 @@
     try:
         reader, writer = await asyncio.open_connection(host, port)
     except (ConnectionError, OSError):
         raise SimulationError(
             f'Simulator "{sim_name}" could not be started: Could not connect to '
             f'"{sim_config["connect"]}"'
         )
-    return RemoteProxy(Channel(reader, writer), mosaik_remote)
+    return RemoteProxy(Channel(reader, writer, name=sim_name), mosaik_remote)
 
 
 Port: TypeAlias = Tuple[EntityId, Attr]
 """Pair of an entity ID and an attribute of that entity"""
 
 
 class SimRunner:
@@ -480,15 +481,31 @@
         if is_earlier:
             self.newer_step.set()
 
     async def setup_done(self):
         return await self._proxy.send(["setup_done", (), {}])
 
     async def step(self, time: Time, inputs: InputData, max_advance: Time) -> Optional[Time]:
-        return await self._proxy.send(["step", (time, inputs, max_advance), {}])
+        try:
+            return await self._proxy.send(["step", (time, inputs, max_advance), {}])
+        except TypeError:  # from JSON serialization
+            # Find source for more precise error message
+            encoder = JSONEncoder()
+            error = NonSerializableOutputsError(self.sid)
+            for dest_eid, entity_inputs in inputs.items():
+                for dest_attr, attr_inputs in entity_inputs.items():
+                    for src_id, value in attr_inputs.items():
+                        try:
+                            encoder.encode(value)
+                        except TypeError as e:
+                            error.add_error(dest_eid, dest_attr, src_id, e)
+            if error:
+                raise error
+            else:  # no culprits found, raise original exception
+                raise
 
     async def get_data(self, outputs: OutputRequest) -> OutputData:
         return await self._proxy.send(["get_data", (outputs,), {}])
 
     def get_output_for(self, time: Time) -> OutputData:
         assert self.outputs is not None
         for data_time, value in reversed(self.outputs.items()):
```

### Comparing `mosaik-3.3.2/mosaik/tiered_time.py` & `mosaik-3.3.3/mosaik/tiered_time.py`

 * *Files identical despite different names*

### Comparing `mosaik-3.3.2/mosaik/util.py` & `mosaik-3.3.3/mosaik/util.py`

 * *Files identical despite different names*

