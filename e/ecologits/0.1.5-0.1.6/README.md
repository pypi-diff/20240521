# Comparing `tmp/ecologits-0.1.5.tar.gz` & `tmp/ecologits-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecologits-0.1.5.tar", max compression
+gzip compressed data, was "ecologits-0.1.6.tar", max compression
```

## Comparing `ecologits-0.1.5.tar` & `ecologits-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    16725 2024-05-02 12:03:16.645735 ecologits-0.1.5/LICENSE
--rw-r--r--   0        0        0     2367 2024-05-02 12:03:16.645735 ecologits-0.1.5/README.md
--rw-r--r--   0        0        0       80 2024-05-02 12:03:16.645735 ecologits-0.1.5/ecologits/__init__.py
--rw-r--r--   0        0        0    11901 2024-05-02 12:03:16.649735 ecologits-0.1.5/ecologits/data/models.csv
--rw-r--r--   0        0        0     2798 2024-05-02 12:03:16.649735 ecologits-0.1.5/ecologits/ecologits.py
--rw-r--r--   0        0        0      140 2024-05-02 12:03:16.649735 ecologits-0.1.5/ecologits/exceptions.py
--rw-r--r--   0        0        0      121 2024-05-02 12:03:16.649735 ecologits-0.1.5/ecologits/impacts/__init__.py
--rw-r--r--   0        0        0     1468 2024-05-02 12:03:16.649735 ecologits-0.1.5/ecologits/impacts/dag.py
--rw-r--r--   0        0        0    14965 2024-05-02 12:03:16.649735 ecologits-0.1.5/ecologits/impacts/llm.py
--rw-r--r--   0        0        0     4066 2024-05-02 12:03:16.649735 ecologits-0.1.5/ecologits/impacts/models.py
--rw-r--r--   0        0        0     2992 2024-05-02 12:03:16.649735 ecologits-0.1.5/ecologits/model_repository.py
--rw-r--r--   0        0        0        0 2024-05-02 12:03:16.649735 ecologits-0.1.5/ecologits/tracers/__init__.py
--rw-r--r--   0        0        0     7848 2024-05-02 12:03:16.649735 ecologits-0.1.5/ecologits/tracers/anthropic_tracer.py
--rw-r--r--   0        0        0     5094 2024-05-02 12:03:16.649735 ecologits-0.1.5/ecologits/tracers/cohere_tracer.py
--rw-r--r--   0        0        0     5554 2024-05-02 12:03:16.649735 ecologits-0.1.5/ecologits/tracers/huggingface_tracer.py
--rw-r--r--   0        0        0     5065 2024-05-02 12:03:16.649735 ecologits-0.1.5/ecologits/tracers/mistralai_tracer.py
--rw-r--r--   0        0        0     5313 2024-05-02 12:03:16.649735 ecologits-0.1.5/ecologits/tracers/openai_tracer.py
--rw-r--r--   0        0        0     1496 2024-05-02 12:03:16.649735 ecologits-0.1.5/ecologits/tracers/utils.py
--rw-r--r--   0        0        0     3664 2024-05-02 12:03:16.649735 ecologits-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4580 1970-01-01 00:00:00.000000 ecologits-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-05-21 17:50:01.081300 ecologits-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2367 2024-05-21 17:50:01.081300 ecologits-0.1.6/README.md
+-rw-r--r--   0        0        0       80 2024-05-21 17:50:01.081300 ecologits-0.1.6/ecologits/__init__.py
+-rw-r--r--   0        0        0    11901 2024-05-21 17:50:01.081300 ecologits-0.1.6/ecologits/data/models.csv
+-rw-r--r--   0        0        0     2798 2024-05-21 17:50:01.081300 ecologits-0.1.6/ecologits/ecologits.py
+-rw-r--r--   0        0        0      140 2024-05-21 17:50:01.081300 ecologits-0.1.6/ecologits/exceptions.py
+-rw-r--r--   0        0        0      121 2024-05-21 17:50:01.081300 ecologits-0.1.6/ecologits/impacts/__init__.py
+-rw-r--r--   0        0        0     1468 2024-05-21 17:50:01.081300 ecologits-0.1.6/ecologits/impacts/dag.py
+-rw-r--r--   0        0        0    14965 2024-05-21 17:50:01.081300 ecologits-0.1.6/ecologits/impacts/llm.py
+-rw-r--r--   0        0        0     4066 2024-05-21 17:50:01.081300 ecologits-0.1.6/ecologits/impacts/models.py
+-rw-r--r--   0        0        0     2992 2024-05-21 17:50:01.081300 ecologits-0.1.6/ecologits/model_repository.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:50:01.081300 ecologits-0.1.6/ecologits/tracers/__init__.py
+-rw-r--r--   0        0        0     7848 2024-05-21 17:50:01.081300 ecologits-0.1.6/ecologits/tracers/anthropic_tracer.py
+-rw-r--r--   0        0        0     5094 2024-05-21 17:50:01.081300 ecologits-0.1.6/ecologits/tracers/cohere_tracer.py
+-rw-r--r--   0        0        0     5554 2024-05-21 17:50:01.081300 ecologits-0.1.6/ecologits/tracers/huggingface_tracer.py
+-rw-r--r--   0        0        0     5065 2024-05-21 17:50:01.081300 ecologits-0.1.6/ecologits/tracers/mistralai_tracer.py
+-rw-r--r--   0        0        0     5313 2024-05-21 17:50:01.081300 ecologits-0.1.6/ecologits/tracers/openai_tracer.py
+-rw-r--r--   0        0        0     1496 2024-05-21 17:50:01.081300 ecologits-0.1.6/ecologits/tracers/utils.py
+-rw-r--r--   0        0        0     3709 2024-05-21 17:50:01.081300 ecologits-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4580 1970-01-01 00:00:00.000000 ecologits-0.1.6/PKG-INFO
```

### Comparing `ecologits-0.1.5/LICENSE` & `ecologits-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.5/README.md` & `ecologits-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.5/ecologits/data/models.csv` & `ecologits-0.1.6/ecologits/data/models.csv`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.5/ecologits/ecologits.py` & `ecologits-0.1.6/ecologits/ecologits.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.5/ecologits/impacts/dag.py` & `ecologits-0.1.6/ecologits/impacts/dag.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.5/ecologits/impacts/llm.py` & `ecologits-0.1.6/ecologits/impacts/llm.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.5/ecologits/impacts/models.py` & `ecologits-0.1.6/ecologits/impacts/models.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.5/ecologits/model_repository.py` & `ecologits-0.1.6/ecologits/model_repository.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.5/ecologits/tracers/anthropic_tracer.py` & `ecologits-0.1.6/ecologits/tracers/anthropic_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.5/ecologits/tracers/cohere_tracer.py` & `ecologits-0.1.6/ecologits/tracers/cohere_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.5/ecologits/tracers/huggingface_tracer.py` & `ecologits-0.1.6/ecologits/tracers/huggingface_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.5/ecologits/tracers/mistralai_tracer.py` & `ecologits-0.1.6/ecologits/tracers/mistralai_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.5/ecologits/tracers/openai_tracer.py` & `ecologits-0.1.6/ecologits/tracers/openai_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.5/ecologits/tracers/utils.py` & `ecologits-0.1.6/ecologits/tracers/utils.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.5/pyproject.toml` & `ecologits-0.1.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ecologits"
-version = "0.1.5"
+version = "0.1.6"
 description = "EcoLogits tracks and estimates the energy consumption and environmental impacts of using generative AI models through APIs."
 authors = [
     "GenAI Impact",
     "Data For Good"
 ]
 maintainers = [
     "GenAI Impact"
@@ -34,15 +34,15 @@
     "Operating System :: POSIX :: Linux"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 wrapt = "^1.14.1"
 pydantic = ">=2,<3"
-packaging = "^24.0"
+packaging = ">=23.2,<25.0"
 openai = { version = "^1.12.0", optional = true }
 mistralai = { version = "^0.1.3", optional = true }
 anthropic = { version = "^0.18.1", optional = true }
 cohere = {version = "^5.2.5", optional = true}
 huggingface-hub = { version = "^0.22.2",  optional = true }
 tiktoken = { version = "^0.6.0", optional = true }
 aiohttp = { version = "^3.9.3", optional = true }
@@ -69,16 +69,16 @@
 
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
-mkdocs-material = "^9.5.12"
-mkdocstrings = {version = "^0.25.0", extras = ["python"]}
+mkdocs-material = { version = "^9.5.12", extras = ["imaging"] }
+mkdocstrings = { version = "^0.25.0", extras = ["python"] }
 mkdocs-gen-files = "^0.5.0"
 mkdocs-autorefs = "^1.0.1"
 mkdocs-literate-nav = "^0.6.1"
 
 
 [pytest]
 env_files = [".env"]
```

### Comparing `ecologits-0.1.5/PKG-INFO` & `ecologits-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecologits
-Version: 0.1.5
+Version: 0.1.6
 Summary: EcoLogits tracks and estimates the energy consumption and environmental impacts of using generative AI models through APIs.
 Home-page: https://ecologits.ai
 License: MPL-2.0
 Author: GenAI Impact
 Maintainer: GenAI Impact
 Requires-Python: >=3.9,<4
 Classifier: Intended Audience :: Developers
@@ -34,15 +34,15 @@
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0) ; extra == "huggingface-hub"
 Requires-Dist: anthropic (>=0.18.1,<0.19.0) ; extra == "anthropic"
 Requires-Dist: cohere (>=5.2.5,<6.0.0) ; extra == "cohere"
 Requires-Dist: huggingface-hub (>=0.22.2,<0.23.0) ; extra == "huggingface-hub"
 Requires-Dist: minijinja (>=1.0.16,<2.0.0) ; extra == "huggingface-hub"
 Requires-Dist: mistralai (>=0.1.3,<0.2.0) ; extra == "mistralai"
 Requires-Dist: openai (>=1.12.0,<2.0.0) ; extra == "openai"
-Requires-Dist: packaging (>=24.0,<25.0)
+Requires-Dist: packaging (>=23.2,<25.0)
 Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0) ; extra == "huggingface-hub"
 Requires-Dist: wrapt (>=1.14.1,<2.0.0)
 Project-URL: Documentation, https://ecologits.ai
 Project-URL: Repository, https://github.com/genai-impact/ecologits
 Description-Content-Type: text/markdown
```

