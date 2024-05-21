# Comparing `tmp/tair_pulse-1.0.2.tar.gz` & `tmp/tair_pulse-1.1.1.tar.gz`

## Comparing `tair_pulse-1.0.2.tar` & `tair_pulse-1.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tair_pulse-1.0.2/requirements.txt
--rw-r--r--   0        0        0   615372 2020-02-02 00:00:00.000000 tair_pulse-1.0.2/docs/example.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tair_pulse-1.0.2/pulse/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 tair_pulse-1.0.2/pulse/__main__.py
--rw-r--r--   0        0        0   205980 2020-02-02 00:00:00.000000 tair_pulse-1.0.2/pulse/keys.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 tair_pulse-1.0.2/pulse/main.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tair_pulse-1.0.2/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 tair_pulse-1.0.2/LICENSE
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 tair_pulse-1.0.2/README.md
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 tair_pulse-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 tair_pulse-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tair_pulse-1.1.1/requirements-dev.lock
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tair_pulse-1.1.1/requirements.lock
+-rw-r--r--   0        0        0   615372 2020-02-02 00:00:00.000000 tair_pulse-1.1.1/docs/example.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tair_pulse-1.1.1/src/tair_pulse/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tair_pulse-1.1.1/src/tair_pulse/__main__.py
+-rw-r--r--   0        0        0   205980 2020-02-02 00:00:00.000000 tair_pulse-1.1.1/src/tair_pulse/keys.py
+-rw-r--r--   0        0        0     8372 2020-02-02 00:00:00.000000 tair_pulse-1.1.1/src/tair_pulse/main.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tair_pulse-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 tair_pulse-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 tair_pulse-1.1.1/README.md
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 tair_pulse-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 tair_pulse-1.1.1/PKG-INFO
```

### Comparing `tair_pulse-1.0.2/docs/example.png` & `tair_pulse-1.1.1/docs/example.png`

 * *Files identical despite different names*

### Comparing `tair_pulse-1.0.2/pulse/keys.py` & `tair_pulse-1.1.1/src/tair_pulse/keys.py`

 * *Files identical despite different names*

### Comparing `tair_pulse-1.0.2/pulse/main.py` & `tair_pulse-1.1.1/src/tair_pulse/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import argparse
 import datetime
 import gc
+import plotly.graph_objects as go
 import random
+import redis
 import signal
 import time
-from typing import Union
-
-import plotly.graph_objects as go
-import redis
 from plotly_resampler import FigureResampler
+from typing import Union
 
-from pulse.keys import SLOT2KEY
+from tair_pulse.keys import SLOT2KEY
 
 # args
 EXAMPLES = """
 Examples:
 
  Run the TairPulse with the default configuration against 127.0.0.1:6379:
    $ tair-pulse
@@ -247,19 +246,22 @@
     clean_keys()
 
     print(f"Write data to latency.html... {len(datetime_array)}")
     fig = FigureResampler(go.Figure())
     fig.add_trace(go.Scattergl(name='latency', showlegend=False), hf_x=datetime_array, hf_y=latency_array)
 
     max_y = max(latency_array)
+    total_width = 0
     for error_name, error in error_dict.items():
         x = [i[0] for i in error.array]
         y = [max_y for i in error.array]
         width = [(i[1] - i[0]).total_seconds() * 1000 for i in error.array]
-        fig.add_trace(go.Bar(x=x, y=y, width=width, offset=0, name=error_name, opacity=0.7))
+        total_width += sum(width)
+        name = f"{error_name}  --  {len(error.array)} times, {sum(width)/1000:.3f}s"
+        fig.add_trace(go.Bar(x=x, y=y, width=width, offset=0, name=name, opacity=0.7))
     fig.update_layout(
         title=f"TairPulse ({g_args.host}:{g_args.port})",
         yaxis_title="latency(ms)",
         height=500,
         legend=dict(yanchor="top", y=-0.2, xanchor="left", x=0)
     )
     fig.write_html(filename)
```

### Comparing `tair_pulse-1.0.2/LICENSE` & `tair_pulse-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tair_pulse-1.0.2/README.md` & `tair_pulse-1.1.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # TairPulse
 
 TairPulse is a tool for visualizing the latency and availability of Tair/Redis instances.
 
-![example.png](https://s2.loli.net/2023/10/11/b6wDT1i8FmKQx52.png)
+![example.png](./docs/example.png)
 
 ## Installation
 
-TairPulse requires `Python 3.7` or later.
+TairPulse requires `Python 3.8` or later.
 
 Install it using `pip` or your preferred PyPI package manager.
 
 ```bash
 pip install tair-pulse
 ```
```

### Comparing `tair_pulse-1.0.2/pyproject.toml` & `tair_pulse-1.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,42 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
 [project]
 name = "tair-pulse"
-version = "1.0.2"
+version = "1.1.1"
+description = "TairPulse is a tool to visualize the latency and availability of Tair/Redis instances."
 authors = [
     { name = "Tair", email = "tair-opensource@alibabacloud.com" },
     { name = "suxb201", email = "suxb201@gmail.com" },
 ]
-description = "TairPulse is a tool to visualize the latency and availability of Tair/Redis instances."
+dependencies = [
+    "plotly>=5.22.0",
+    "redis>=5.0.4",
+    "plotly-resampler>=0.10.0",
+]
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">= 3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-]
-dependencies = [
-    "plotly >= 5.17.0",
-    "redis >= 5.0.0",
-    "plotly-resampler >= 0.9.1",
+    "Topic :: Database",
 ]
 
 [project.scripts]
-tair-pulse = "pulse.__main__:main"
+"tair-pulse" = "tair_pulse.main:main"
 
 [project.urls]
 "Homepage" = "https://github.com/tair-opensource"
 "Bug Tracker" = "https://github.com/tair-opensource"
 
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[tool.rye]
+managed = true
+dev-dependencies = []
+
+[tool.hatch.metadata]
+allow-direct-references = true
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/tair_pulse"]
```

### Comparing `tair_pulse-1.0.2/PKG-INFO` & `tair_pulse-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tair-pulse
-Version: 1.0.2
+Version: 1.1.1
 Summary: TairPulse is a tool to visualize the latency and availability of Tair/Redis instances.
 Project-URL: Homepage, https://github.com/tair-opensource
 Project-URL: Bug Tracker, https://github.com/tair-opensource
 Author-email: Tair <tair-opensource@alibabacloud.com>, suxb201 <suxb201@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: plotly-resampler>=0.9.1
-Requires-Dist: plotly>=5.17.0
-Requires-Dist: redis>=5.0.0
+Classifier: Topic :: Database
+Requires-Python: >=3.8
+Requires-Dist: plotly-resampler>=0.10.0
+Requires-Dist: plotly>=5.22.0
+Requires-Dist: redis>=5.0.4
 Description-Content-Type: text/markdown
 
 # TairPulse
 
 TairPulse is a tool for visualizing the latency and availability of Tair/Redis instances.
 
-![example.png](https://s2.loli.net/2023/10/11/b6wDT1i8FmKQx52.png)
+![example.png](./docs/example.png)
 
 ## Installation
 
-TairPulse requires `Python 3.7` or later.
+TairPulse requires `Python 3.8` or later.
 
 Install it using `pip` or your preferred PyPI package manager.
 
 ```bash
 pip install tair-pulse
 ```
```

