# Comparing `tmp/arize_phoenix_evals-0.9.0.tar.gz` & `tmp/arize_phoenix_evals-0.9.1.tar.gz`

## Comparing `arize_phoenix_evals-0.9.0.tar` & `arize_phoenix_evals-0.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/__init__.py
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/classify.py
--rw-r--r--   0        0        0    30282 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/default_templates.py
--rw-r--r--   0        0        0    15651 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/evaluators.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/exceptions.py
--rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/executors.py
--rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/generate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/py.typed
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/retrievals.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/templates.py
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/utils.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/__init__.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/anthropic.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/base.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/bedrock.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/litellm.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/mistralai.py
--rw-r--r--   0        0        0    15311 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/openai.py
--rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/rate_limiters.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/vertex.py
--rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/vertexai.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/.gitignore
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/IP_NOTICE
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/LICENSE
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/README.md
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/__init__.py
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/classify.py
+-rw-r--r--   0        0        0    30282 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/default_templates.py
+-rw-r--r--   0        0        0    15651 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/evaluators.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/exceptions.py
+-rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/executors.py
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/generate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/py.typed
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/retrievals.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/templates.py
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/utils.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/__init__.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/anthropic.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/base.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/bedrock.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/litellm.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/mistralai.py
+-rw-r--r--   0        0        0    15585 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/openai.py
+-rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/rate_limiters.py
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/vertex.py
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/vertexai.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/.gitignore
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/IP_NOTICE
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/README.md
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/PKG-INFO
```

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/__init__.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/__init__.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/classify.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/classify.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/default_templates.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/default_templates.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/evaluators.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/evaluators.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/executors.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/executors.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/generate.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/generate.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/retrievals.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/retrievals.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/templates.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/templates.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/utils.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/utils.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/anthropic.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/base.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/base.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/bedrock.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/litellm.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/litellm.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/mistralai.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/mistralai.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/openai.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,19 @@
         self._is_azure = bool(self.azure_endpoint)
 
         self._model_uses_legacy_completion_api = self.model.startswith(LEGACY_COMPLETION_API_MODELS)
         if self.api_key is None:
             api_key = os.getenv(OPENAI_API_KEY_ENVVAR_NAME)
             if api_key is None:
                 # TODO: Create custom AuthenticationError
+                if self._is_azure:
+                    raise RuntimeError(
+                        "Azure API key not provided. Pass it as an argument to 'api_key' "
+                        "or set it in your environment: 'export OPENAI_API_KEY=****'"
+                    )
                 raise RuntimeError(
                     "OpenAI's API key not provided. Pass it as an argument to 'api_key' "
                     "or set it in your environment: 'export OPENAI_API_KEY=sk-****'"
                 )
             self.api_key = api_key
 
         # Set the version, organization, and base_url - default to openAI
```

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/rate_limiters.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/rate_limiters.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/vertex.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/vertex.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/vertexai.py` & `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/vertexai.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/LICENSE` & `arize_phoenix_evals-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/README.md` & `arize_phoenix_evals-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.0/pyproject.toml` & `arize_phoenix_evals-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
-version = "0.9.0"
+version = "0.9.1"
 dependencies = [
   "pandas",
   "tqdm",
   "typing-extensions>=4.5, <5",
 ]
 
 [project.optional-dependencies]
```

### Comparing `arize_phoenix_evals-0.9.0/PKG-INFO` & `arize_phoenix_evals-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arize-phoenix-evals
-Version: 0.9.0
+Version: 0.9.1
 Summary: LLM Evaluations
 Project-URL: Documentation, https://docs.arize.com/phoenix/
 Project-URL: Issues, https://github.com/Arize-ai/phoenix/issues
 Project-URL: Source, https://github.com/Arize-ai/phoenix
 Author-email: Arize AI <phoenix-devs@arize.com>
 License: Elastic-2.0
 License-File: IP_NOTICE
```

