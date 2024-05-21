# Comparing `tmp/crab_framework-0.1.0.tar.gz` & `tmp/crab_framework-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crab_framework-0.1.0.tar", max compression
+gzip compressed data, was "crab_framework-0.1.1.tar", max compression
```

## Comparing `crab_framework-0.1.0.tar` & `crab_framework-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1502 2024-05-12 19:29:01.230200 crab_framework-0.1.0/README.md
--rw-r--r--   0        0        0      770 2024-05-12 19:29:01.230200 crab_framework-0.1.0/crab/__init__.py
--rw-r--r--   0        0        0     5844 2024-05-12 19:29:01.230200 crab_framework-0.1.0/crab/actions/android_actions.py
--rw-r--r--   0        0        0     5697 2024-05-12 19:29:01.230200 crab_framework-0.1.0/crab/actions/desktop_actions.py
--rw-r--r--   0        0        0     1232 2024-05-12 19:29:01.230200 crab_framework-0.1.0/crab/actions/system_actions.py
--rw-r--r--   0        0        0     9226 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/actions/visual_prompt_actions.py
--rw-r--r--   0        0        0      708 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/agents/single_agent/__init__.py
--rw-r--r--   0        0        0     3120 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/agents/single_agent/base_agent.py
--rw-r--r--   0        0        0     4800 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/agents/single_agent/openai_agent.py
--rw-r--r--   0        0        0      708 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/benchmarks/__init__.py
--rw-r--r--   0        0        0     2847 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/benchmarks/template.py
--rw-r--r--   0        0        0     3792 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/benchmarks/ubuntu.py
--rw-r--r--   0        0        0      960 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/core/__init__.py
--rw-r--r--   0        0        0    13486 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/core/benchmark.py
--rw-r--r--   0        0        0     1743 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/core/decorators.py
--rw-r--r--   0        0        0     8994 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/core/environment.py
--rw-r--r--   0        0        0      794 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/core/exceptions.py
--rw-r--r--   0        0        0     9139 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/core/graph_evaluator.py
--rw-r--r--   0        0        0     1091 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/core/models/__init__.py
--rw-r--r--   0        0        0    12763 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/core/models/action.py
--rw-r--r--   0        0        0      923 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/core/models/benchmark_interface.py
--rw-r--r--   0        0        0     1359 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/core/models/config.py
--rw-r--r--   0        0        0     2720 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/core/models/evaluator.py
--rw-r--r--   0        0        0     2663 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/core/models/task.py
--rw-r--r--   0        0        0      708 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/environments/__init__.py
--rw-r--r--   0        0        0     1157 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/environments/android.py
--rw-r--r--   0        0        0     1164 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/environments/linux.py
--rw-r--r--   0        0        0     1336 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/environments/template.py
--rw-r--r--   0        0        0      708 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/server/__init__.py
--rw-r--r--   0        0        0     1453 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/server/api.py
--rw-r--r--   0        0        0     1321 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/server/config.py
--rw-r--r--   0        0        0     2663 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/server/exception_handlers.py
--rw-r--r--   0        0        0     2128 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/server/logger.py
--rw-r--r--   0        0        0     2307 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/server/main.py
--rw-r--r--   0        0        0     1764 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/server/middleware.py
--rw-r--r--   0        0        0     1564 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/server/utils.py
--rw-r--r--   0        0        0     3478 2024-05-12 19:29:01.234200 crab_framework-0.1.0/crab/utils/common.py
--rw-r--r--   0        0        0     1864 2024-05-12 19:29:01.238200 crab_framework-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3180 1970-01-01 00:00:00.000000 crab_framework-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1502 2024-05-21 17:44:03.551961 crab_framework-0.1.1/README.md
+-rw-r--r--   0        0        0      770 2024-05-21 17:44:03.551961 crab_framework-0.1.1/crab/__init__.py
+-rw-r--r--   0        0        0     5844 2024-05-21 17:44:03.551961 crab_framework-0.1.1/crab/actions/android_actions.py
+-rw-r--r--   0        0        0     5697 2024-05-21 17:44:03.551961 crab_framework-0.1.1/crab/actions/desktop_actions.py
+-rw-r--r--   0        0        0     1232 2024-05-21 17:44:03.551961 crab_framework-0.1.1/crab/actions/system_actions.py
+-rw-r--r--   0        0        0     9226 2024-05-21 17:44:03.551961 crab_framework-0.1.1/crab/actions/visual_prompt_actions.py
+-rw-r--r--   0        0        0      708 2024-05-21 17:44:03.551961 crab_framework-0.1.1/crab/agents/single_agent/__init__.py
+-rw-r--r--   0        0        0     3120 2024-05-21 17:44:03.551961 crab_framework-0.1.1/crab/agents/single_agent/base_agent.py
+-rw-r--r--   0        0        0     4800 2024-05-21 17:44:03.551961 crab_framework-0.1.1/crab/agents/single_agent/openai_agent.py
+-rw-r--r--   0        0        0      708 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/benchmarks/__init__.py
+-rw-r--r--   0        0        0     2847 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/benchmarks/template.py
+-rw-r--r--   0        0        0     3792 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/benchmarks/ubuntu.py
+-rw-r--r--   0        0        0      960 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/core/__init__.py
+-rw-r--r--   0        0        0    13486 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/core/benchmark.py
+-rw-r--r--   0        0        0     1743 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/core/decorators.py
+-rw-r--r--   0        0        0     8994 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/core/environment.py
+-rw-r--r--   0        0        0      794 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/core/exceptions.py
+-rw-r--r--   0        0        0     9139 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/core/graph_evaluator.py
+-rw-r--r--   0        0        0     1091 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/core/models/__init__.py
+-rw-r--r--   0        0        0    12763 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/core/models/action.py
+-rw-r--r--   0        0        0      923 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/core/models/benchmark_interface.py
+-rw-r--r--   0        0        0     1359 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/core/models/config.py
+-rw-r--r--   0        0        0     2720 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/core/models/evaluator.py
+-rw-r--r--   0        0        0     2663 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/core/models/task.py
+-rw-r--r--   0        0        0      708 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/environments/__init__.py
+-rw-r--r--   0        0        0     1157 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/environments/android.py
+-rw-r--r--   0        0        0     1164 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/environments/linux.py
+-rw-r--r--   0        0        0     1336 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/environments/template.py
+-rw-r--r--   0        0        0      708 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/server/__init__.py
+-rw-r--r--   0        0        0     1453 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/server/api.py
+-rw-r--r--   0        0        0     1321 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/server/config.py
+-rw-r--r--   0        0        0     2663 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/server/exception_handlers.py
+-rw-r--r--   0        0        0     2128 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/server/logger.py
+-rw-r--r--   0        0        0     2307 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/server/main.py
+-rw-r--r--   0        0        0     1764 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/server/middleware.py
+-rw-r--r--   0        0        0     1564 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/server/utils.py
+-rw-r--r--   0        0        0     3478 2024-05-21 17:44:03.555961 crab_framework-0.1.1/crab/utils/common.py
+-rw-r--r--   0        0        0     1863 2024-05-21 17:44:03.559960 crab_framework-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 crab_framework-0.1.1/PKG-INFO
```

### Comparing `crab_framework-0.1.0/README.md` & `crab_framework-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/__init__.py` & `crab_framework-0.1.1/crab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2024 @ CAMEL-AI.org. All Rights Reserved. ===========
 # ruff: noqa: F403
 from .core import *
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

### Comparing `crab_framework-0.1.0/crab/actions/android_actions.py` & `crab_framework-0.1.1/crab/actions/android_actions.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/actions/desktop_actions.py` & `crab_framework-0.1.1/crab/actions/desktop_actions.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/actions/system_actions.py` & `crab_framework-0.1.1/crab/actions/system_actions.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/actions/visual_prompt_actions.py` & `crab_framework-0.1.1/crab/actions/visual_prompt_actions.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/agents/single_agent/__init__.py` & `crab_framework-0.1.1/crab/agents/single_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/agents/single_agent/base_agent.py` & `crab_framework-0.1.1/crab/agents/single_agent/base_agent.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/agents/single_agent/openai_agent.py` & `crab_framework-0.1.1/crab/agents/single_agent/openai_agent.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/benchmarks/__init__.py` & `crab_framework-0.1.1/crab/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/benchmarks/template.py` & `crab_framework-0.1.1/crab/benchmarks/template.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/benchmarks/ubuntu.py` & `crab_framework-0.1.1/crab/benchmarks/ubuntu.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/core/__init__.py` & `crab_framework-0.1.1/crab/core/__init__.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/core/benchmark.py` & `crab_framework-0.1.1/crab/core/benchmark.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/core/decorators.py` & `crab_framework-0.1.1/crab/core/decorators.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/core/environment.py` & `crab_framework-0.1.1/crab/core/environment.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/core/exceptions.py` & `crab_framework-0.1.1/crab/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/core/graph_evaluator.py` & `crab_framework-0.1.1/crab/core/graph_evaluator.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/core/models/__init__.py` & `crab_framework-0.1.1/crab/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/core/models/action.py` & `crab_framework-0.1.1/crab/core/models/action.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/core/models/benchmark_interface.py` & `crab_framework-0.1.1/crab/core/models/benchmark_interface.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/core/models/config.py` & `crab_framework-0.1.1/crab/core/models/config.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/core/models/evaluator.py` & `crab_framework-0.1.1/crab/core/models/evaluator.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/core/models/task.py` & `crab_framework-0.1.1/crab/core/models/task.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/environments/__init__.py` & `crab_framework-0.1.1/crab/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/environments/android.py` & `crab_framework-0.1.1/crab/environments/android.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/environments/linux.py` & `crab_framework-0.1.1/crab/environments/linux.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/environments/template.py` & `crab_framework-0.1.1/crab/environments/template.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/server/__init__.py` & `crab_framework-0.1.1/crab/server/__init__.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/server/api.py` & `crab_framework-0.1.1/crab/server/api.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/server/config.py` & `crab_framework-0.1.1/crab/server/config.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/server/exception_handlers.py` & `crab_framework-0.1.1/crab/server/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/server/logger.py` & `crab_framework-0.1.1/crab/server/logger.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/server/main.py` & `crab_framework-0.1.1/crab/server/main.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/server/middleware.py` & `crab_framework-0.1.1/crab/server/middleware.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/server/utils.py` & `crab_framework-0.1.1/crab/server/utils.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/crab/utils/common.py` & `crab_framework-0.1.1/crab/utils/common.py`

 * *Files identical despite different names*

### Comparing `crab_framework-0.1.0/pyproject.toml` & `crab_framework-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["poetry-core>=1.2.0", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "crab-framework"
-version = "0.1.0"
+version = "0.1.1"
 description = "Cross-platfrom Agent Benchmark Framework for Multimodal Embodied Language Model Agents"
 
 authors = ["CAMEL-AI.org"]
 maintainers = ["Tianqi Xu <tianqi.xu@kaust.edu.sa>"]
 
 packages = [{ include = "crab" }]
 
 readme = "README.md"
 license = "Apache License 2.0"
 repository = "https://github.com/camel-ai/crab"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 
 # core
 docstring-parser = "^0"
 networkx = "^3"
 dill = "^0.3.8"
 pydantic = "^2.6"
```

### Comparing `crab_framework-0.1.0/PKG-INFO` & `crab_framework-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: crab-framework
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cross-platfrom Agent Benchmark Framework for Multimodal Embodied Language Model Agents
 Home-page: https://github.com/camel-ai/crab
 License: Apache-2.0
 Author: CAMEL-AI.org
 Maintainer: Tianqi Xu
 Maintainer-email: tianqi.xu@kaust.edu.sa
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: server
 Provides-Extra: visual-prompt
 Requires-Dist: dill (>=0.3.8,<0.4.0)
 Requires-Dist: docstring-parser (>=0,<1)
```

