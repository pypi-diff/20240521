# Comparing `tmp/zur_ecu_client-0.0.6.tar.gz` & `tmp/zur_ecu_client-0.0.7.tar.gz`

## Comparing `zur_ecu_client-0.0.6.tar` & `zur_ecu_client-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/requirements.txt
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.github/workflows/black.yml
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.github/workflows/publish-to-test-pypi.yaml
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.idea/.gitignore
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.idea/ECU-Client.iml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.idea/runConfigurations/pytest.xml
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.vscode/settings.json
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/__init__.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/ecu_client.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/messages.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/mock_ecu.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/udp_server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/senml/__init__.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml_msg.py
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml_msg_dv.py
--rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml_msg_ecu.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml_unit.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml_zur_names.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/senml/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/tests/test_messages.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/tests/test_sample.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/README.md
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/__about__.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.github/workflows/black.yml
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.github/workflows/publish-to-test-pypi.yaml
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.idea/.gitignore
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.idea/ECU-Client.iml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.idea/runConfigurations/pytest.xml
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.vscode/settings.json
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/__init__.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/ecu_client.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/messages.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/mock_ecu.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/udp_server.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/senml/__init__.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_msg.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_msg_dv.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_msg_ecu.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_unit.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_zur_names.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/senml/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/tests/test_messages.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/tests/test_sample.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/README.md
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/PKG-INFO
```

### Comparing `zur_ecu_client-0.0.6/.github/workflows/publish-to-test-pypi.yaml` & `zur_ecu_client-0.0.7/.github/workflows/publish-to-test-pypi.yaml`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.6/.github/workflows/python-package.yml` & `zur_ecu_client-0.0.7/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.6/.idea/runConfigurations/pytest.xml` & `zur_ecu_client-0.0.7/.idea/runConfigurations/pytest.xml`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.6/src/zur_ecu_client/ecu_client.py` & `zur_ecu_client-0.0.7/src/zur_ecu_client/ecu_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 import sched
 import time
 from threading import Thread
 
-from src.zur_ecu_client.senml.senml_zur_names import SenmlNames
+from .senml import SenmlNames
 from .udp_server import UdpServer
 
 
 class EcuClient:
 
     def __init__(
         self, listener, ecu_ip: str, ecu_port: int, calls_per_second: int
```

### Comparing `zur_ecu_client-0.0.6/src/zur_ecu_client/messages.py` & `zur_ecu_client-0.0.7/src/zur_ecu_client/messages.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from enum import Enum, IntEnum
 from typing import List
 
-from src.zur_ecu_client.senml.senml import Senml
-from src.zur_ecu_client.senml.senml_zur_names import SenmlNames
-from src.zur_ecu_client.senml.util import value_by_key_prefix
+from .senml import SenmlNames
+from .senml import Senml
+from .senml import value_by_key_prefix
 
 
 class Messages:
     class AmiState(Enum):
         ACCELERATION = "acceleration"
         SKIDPAD = "skidpad"
         TRACKDRIVE = "trackdrive"
```

### Comparing `zur_ecu_client-0.0.6/src/zur_ecu_client/udp_server.py` & `zur_ecu_client-0.0.7/src/zur_ecu_client/udp_server.py`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml.py` & `zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 
-from src.zur_ecu_client.senml.senml_unit import SenmlUnit
-from src.zur_ecu_client.senml.senml_zur_names import SenmlNames
-from src.zur_ecu_client.senml.util import value_by_key_prefix
+from .senml_unit import SenmlUnit
+from .senml_zur_names import SenmlNames
+from .util import value_by_key_prefix
 
 
 class Senml:
     class Type(Enum):
         REQUEST = 1
         DATA = 2
         ACKNOWLEDGMENT = 3
```

### Comparing `zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml_msg.py` & `zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_msg.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 
-from src.zur_ecu_client.senml.senml import Senml
-from src.zur_ecu_client.senml.senml_unit import SenmlUnit
-from src.zur_ecu_client.senml.senml_zur_names import SenmlNames
+from .senml import Senml
+from .senml_unit import SenmlUnit
+from .senml_zur_names import SenmlNames
 
 
 class SenmlMessage:
     def __init__(self, msg_type: SenmlNames, msg_map: List[Senml.Record]) -> None:
         msg_type: List = msg_type.value.split(":")
         self.baseName = msg_type[0]
         self.name = msg_type[1]
```

### Comparing `zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml_msg_dv.py` & `zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_msg_dv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from src.zur_ecu_client.senml.senml import Senml
-from src.zur_ecu_client.senml.senml_msg import SenmlMessage
-from src.zur_ecu_client.senml.senml_unit import SenmlUnit
-from src.zur_ecu_client.senml.senml_zur_names import SenmlNames
+from .senml import Senml
+from .senml_msg import SenmlMessage
+from .senml_unit import SenmlUnit
+from .senml_zur_names import SenmlNames
 
 
 class Dv:
     class Cfg(SenmlMessage):
         def __init__(
             self,
             ass: str = None,
@@ -29,17 +29,17 @@
                     ),
                 ],
             )
 
     class Ctrl(SenmlMessage):
         def __init__(
             self,
-            brake: str = None,
-            steering: str = None,
-            throttle: str = None,
+            brake: int = None,
+            steering: int = None,
+            throttle: int = None,
             status: str = None,
         ) -> None:
             super().__init__(
                 SenmlNames.DV_CTRL,
                 [
                     Senml.Record(
                         SenmlNames.DV_CTRL_BRAKE,
@@ -87,17 +87,17 @@
                     ),
                 ],
             )
 
     class Acc(SenmlMessage):
         def __init__(
             self,
-            x: str = None,
-            y: str = None,
-            z: str = None,
+            x: int = None,
+            y: int = None,
+            z: int = None,
         ) -> None:
             super().__init__(
                 SenmlNames.DV_ACC,
                 [
                     Senml.Record(
                         SenmlNames.DV_ACC_X,
                         SenmlUnit.ACCELERATION,
```

### Comparing `zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml_msg_ecu.py` & `zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_msg_ecu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from src.zur_ecu_client.senml.senml import Senml
-from src.zur_ecu_client.senml.senml_msg import SenmlMessage
-from src.zur_ecu_client.senml.senml_unit import SenmlUnit
-from src.zur_ecu_client.senml.senml_zur_names import SenmlNames
+from .senml import Senml
+from .senml_msg import SenmlMessage
+from .senml_unit import SenmlUnit
+from .senml_zur_names import SenmlNames
 
 
 class Ecu:
     class Hvcb(SenmlMessage):
         def __init__(
             self,
             lv_accu: int = None,
```

### Comparing `zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml_unit.py` & `zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_unit.py`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml_zur_names.py` & `zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_zur_names.py`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.6/tests/test_messages.py` & `zur_ecu_client-0.0.7/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.6/tests/test_sample.py` & `zur_ecu_client-0.0.7/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.6/.gitignore` & `zur_ecu_client-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.6/LICENSE.txt` & `zur_ecu_client-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.6/pyproject.toml` & `zur_ecu_client-0.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "zur_ecu_client" 
-version = "0.0.6"
+dynamic = [
+  "version"
+]
 description = "Internal Python library which provides an interface to the ECU"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]
 authors = [
     {name = "ZUR Driverless", email = "driverless@zurichuasracing.ch" },
@@ -61,7 +63,10 @@
 
 
 [project.scripts]
 sample = "sample:main"
 
 
 [tool.setuptools]
+
+[tool.hatch.version]
+path = "__about__.py"
```

### Comparing `zur_ecu_client-0.0.6/PKG-INFO` & `zur_ecu_client-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: zur_ecu_client
-Version: 0.0.6
+Version: 0.0.7
 Summary: Internal Python library which provides an interface to the ECU
 Project-URL: Homepage, https://zurichuasracing.ch
 Project-URL: Bug Reports, https://github.com/zurich-uas-racing/issues
 Project-URL: Source, https://github.com/zurich-uas-racing/ecu-client
 Author-email: ZUR Driverless <driverless@zurichuasracing.ch>, Finn Scheller <finn.scheller@zurichuasracing.ch>, Cèline Brun <bruncel1@students.zhaw.ch>
 Maintainer-email: ZUR Driverless <driverless@zurichuasracing.ch>
 License: MIT License
```

