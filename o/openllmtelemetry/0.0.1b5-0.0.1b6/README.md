# Comparing `tmp/openllmtelemetry-0.0.1b5.tar.gz` & `tmp/openllmtelemetry-0.0.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openllmtelemetry-0.0.1b5.tar", max compression
+gzip compressed data, was "openllmtelemetry-0.0.1b6.tar", max compression
```

## Comparing `openllmtelemetry-0.0.1b5.tar` & `openllmtelemetry-0.0.1b6.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0    11357 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b5/LICENSE
--rw-r--r--   0        0        0     4317 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b5/README.md
--rw-r--r--   0        0        0       99 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/__init__.py
--rw-r--r--   0        0        0     8376 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/config.py
--rw-r--r--   0        0        0     2629 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrument.py
--rw-r--r--   0        0        0    11339 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/LICENSE
--rw-r--r--   0        0        0        0 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/__init__.py
--rw-r--r--   0        0        0    12023 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/bedrock/__init__.py
--rw-r--r--   0        0        0     2344 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py
--rw-r--r--   0        0        0     1715 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     4678 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/shared/__init__.py
--rw-r--r--   0        0        0     8374 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py
--rw-r--r--   0        0        0     5411 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py
--rw-r--r--   0        0        0     3509 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py
--rw-r--r--   0        0        0     1231 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/utils.py
--rw-r--r--   0        0        0     2397 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/v0/__init__.py
--rw-r--r--   0        0        0     2904 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/v1/__init__.py
--rw-r--r--   0        0        0       28 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/version.py
--rw-r--r--   0        0        0     1403 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b5/openllmtelemetry/intrument_openai.py
--rw-r--r--   0        0        0     3150 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b5/openllmtelemetry/secure.py
--rw-r--r--   0        0        0     2457 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b5/openllmtelemetry/semantic_conventions/gen_ai/__init__.py
--rw-r--r--   0        0        0      809 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b5/openllmtelemetry/span_exporter.py
--rw-r--r--   0        0        0      477 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b5/openllmtelemetry/version.py
--rw-r--r--   0        0        0     1653 2024-05-15 14:56:39.985842 openllmtelemetry-0.0.1b5/pyproject.toml
--rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 openllmtelemetry-0.0.1b5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-22 23:27:14.459880 openllmtelemetry-0.0.1b6/LICENSE
+-rw-r--r--   0        0        0     4317 2024-04-24 17:37:18.405975 openllmtelemetry-0.0.1b6/README.md
+-rw-r--r--   0        0        0       75 2024-05-21 15:45:54.138472 openllmtelemetry-0.0.1b6/openllmtelemetry/__init__.py
+-rw-r--r--   0        0        0     8435 2024-05-21 15:52:52.542394 openllmtelemetry-0.0.1b6/openllmtelemetry/config.py
+-rw-r--r--   0        0        0       61 2024-05-21 15:52:52.019303 openllmtelemetry-0.0.1b6/openllmtelemetry/guardrails/__init__.py
+-rw-r--r--   0        0        0     4054 2024-05-21 15:52:52.674562 openllmtelemetry-0.0.1b6/openllmtelemetry/guardrails/client.py
+-rw-r--r--   0        0        0     7180 2024-05-21 15:52:52.674867 openllmtelemetry-0.0.1b6/openllmtelemetry/guardrails/handlers.py
+-rw-r--r--   0        0        0     1971 2024-05-21 15:52:52.675317 openllmtelemetry-0.0.1b6/openllmtelemetry/instrument.py
+-rw-r--r--   0        0        0    11339 2024-04-24 17:37:18.407381 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-24 17:37:18.407435 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/__init__.py
+-rw-r--r--   0        0        0    14053 2024-05-21 15:52:52.543647 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/bedrock/__init__.py
+-rw-r--r--   0        0        0     2344 2024-04-30 16:55:16.794654 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py
+-rw-r--r--   0        0        0     1719 2024-05-21 15:52:52.019985 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     4769 2024-05-21 15:52:52.675543 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/shared/__init__.py
+-rw-r--r--   0        0        0     9995 2024-05-21 15:52:52.675741 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py
+-rw-r--r--   0        0        0     6306 2024-05-21 15:52:52.675965 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py
+-rw-r--r--   0        0        0     3509 2024-05-21 15:52:52.020983 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py
+-rw-r--r--   0        0        0     1231 2024-04-30 16:55:16.796566 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/utils.py
+-rw-r--r--   0        0        0     2401 2024-05-21 15:52:52.021214 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/v0/__init__.py
+-rw-r--r--   0        0        0     2908 2024-05-21 15:52:52.021419 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/v1/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-24 17:37:18.409700 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/version.py
+-rw-r--r--   0        0        0     1407 2024-05-21 15:52:52.021650 openllmtelemetry-0.0.1b6/openllmtelemetry/intrument_openai.py
+-rw-r--r--   0        0        0     2493 2024-05-21 15:52:52.676238 openllmtelemetry-0.0.1b6/openllmtelemetry/semantic_conventions/gen_ai/__init__.py
+-rw-r--r--   0        0        0      809 2024-05-20 22:42:13.975873 openllmtelemetry-0.0.1b6/openllmtelemetry/span_exporter.py
+-rw-r--r--   0        0        0      477 2024-04-24 17:37:18.410285 openllmtelemetry-0.0.1b6/openllmtelemetry/version.py
+-rw-r--r--   0        0        0     1653 2024-05-21 16:19:11.435989 openllmtelemetry-0.0.1b6/pyproject.toml
+-rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 openllmtelemetry-0.0.1b6/PKG-INFO
```

### Comparing `openllmtelemetry-0.0.1b5/LICENSE` & `openllmtelemetry-0.0.1b6/LICENSE`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b5/README.md` & `openllmtelemetry-0.0.1b6/README.md`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b5/openllmtelemetry/config.py` & `openllmtelemetry-0.0.1b6/openllmtelemetry/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import configparser
 import logging
 import os
 from dataclasses import dataclass, fields
+from getpass import getpass
 from pathlib import Path
 from typing import Optional
 
 from opentelemetry.exporter.otlp.proto.http.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor, SimpleSpanProcessor
 
-from openllmtelemetry.secure import GuardrailsApi
+from openllmtelemetry.guardrails import GuardrailsApi
 from openllmtelemetry.span_exporter import DebugOTLSpanExporter
 
 CFG_API_KEY = "api_key"
 
 CFG_ENDPOINT_KEY = "endpoint"
 
 CFG_WHYLABS_SECTION = "whylabs"
@@ -51,32 +52,33 @@
         )
 
     @property
     def whylabs_traces_endpoint(self) -> str:
         assert self.whylabs_endpoint is not None, "WhyLabs endpoint is not set."
         return f"{self.whylabs_endpoint.rstrip('/')}/v1/traces"
 
-    def guardrail_client(self, default_dataset_id: Optional[str]) -> Optional[GuardrailsApi]:
+    def guardrail_client(self, default_dataset_id: str) -> Optional[GuardrailsApi]:
         if self.guardrails_endpoint and self.guardrails_api_key:
             return GuardrailsApi(
                 guardrails_endpoint=self.guardrails_endpoint,
                 guardrails_api_key=self.guardrails_api_key,
                 dataset_id=default_dataset_id,
             )
         LOGGER.warning("GuardRails endpoint is not set.")
         return None
 
     def config_tracer_provider(
         self,
         tracer_provider: TracerProvider,
         dataset_id: str,
         disable_batching: bool = False,
+        debug: bool = False,
     ):
         if self.whylabs_traces_endpoint and self.whylabs_api_key:
-            debug_enabled = os.environ.get("WHYLABS_DEBUG_TRACE")
+            debug_enabled = os.environ.get("WHYLABS_DEBUG_TRACE") or debug
             whylabs_api_key_header = {"X-API-Key": self.whylabs_api_key, "X-WHYLABS-RESOURCE": dataset_id}
             # TODO: support other kinds of exporters
             if debug_enabled:
                 otlp_exporter = DebugOTLSpanExporter(
                     endpoint=self.whylabs_traces_endpoint,
                     headers=whylabs_api_key_header,  # noqa: F821
                 )
@@ -106,15 +108,15 @@
             }
         with open(config_path, "w") as configfile:
             config.write(configfile)
 
     def __repr__(self):
         # hide the api_key from output
         field_strs = [
-            f"{field.name}='***key***'" if 'key' in field.name else f"{field.name}={getattr(self, field.name)}" for field in fields(self)
+            f"{field.name}='***key***'" if "key" in field.name else f"{field.name}={getattr(self, field.name)}" for field in fields(self)
         ]
         return f"{self.__class__.__name__}({', '.join(field_strs)})"
 
     @classmethod
     def read(cls, config_path: str) -> "GuardrailConfig":
         config = configparser.ConfigParser()
         ok_files = config.read(config_path)
@@ -125,15 +127,15 @@
         whylabs_api_key = config.get(CFG_WHYLABS_SECTION, CFG_API_KEY)
         guardrails_endpoint = config.get(CFG_GUARDRAILS_SECTION, CFG_ENDPOINT_KEY, fallback=None)
         guardrails_api_key = config.get(CFG_GUARDRAILS_SECTION, CFG_API_KEY, fallback=None)
 
         return GuardrailConfig(whylabs_endpoint, whylabs_api_key, guardrails_endpoint, guardrails_api_key)
 
 
-def load_config() -> GuardrailConfig:
+def load_config() -> Optional[GuardrailConfig]:
     config_path = os.environ.get("WHYLABS_GUARDRAILS_CONFIG")
     if config_path is None:
         config_path = _DEFAULT_CONFIG_FILE
     config = GuardrailConfig(None, None, None, None)
     try:
         config = GuardrailConfig.read(config_path)
     except:  # noqa
@@ -142,15 +144,15 @@
         config = _load_config_from_env(config)
     if config.is_partial and _in_ipython_session:
         config = _interactive_config(config)
 
     return config
 
 
-def load_dataset_id(dataset_id: Optional[str]) -> Optional[str]:
+def load_dataset_id(dataset_id: str) -> Optional[str]:
     effective_dataset_id = os.environ.get("WHYLABS_DEFAULT_DATASET_ID", dataset_id)
     if effective_dataset_id is None:
         if _in_ipython_session:
             effective_dataset_id = input("Set the default dataset ID: ").strip()
             if len(effective_dataset_id) > 0:
                 print("Using dataset ID: ", effective_dataset_id)
             else:
@@ -172,24 +174,24 @@
 
 def _interactive_config(config: GuardrailConfig) -> GuardrailConfig:
     whylabs_endpoint = config.whylabs_endpoint or _DEFAULT_ENDPOINT
     whylabs_api_key = config.whylabs_api_key
     guardrails_endpoint = config.guardrails_endpoint
     guardrails_api_key = config.guardrails_api_key
     if whylabs_api_key is None:
-        whylabs_api_key = input("Set WhyLabs API Key: ").strip()
+        whylabs_api_key = getpass("Set WhyLabs API Key: ").strip()
         print("Using WhyLabs API key with ID: ", whylabs_api_key[:10])
     if guardrails_endpoint is None:
         guardrails_endpoint = input("Set GuardRails endpoint (leave blank to skip guardrail): ").strip()
         if len(guardrails_endpoint) == 0:
             guardrails_endpoint = None
         if guardrails_endpoint is None:
             print("GuardRails endpoint is not set. Only tracing is enabled.")
     if guardrails_endpoint is not None and guardrails_api_key is None:
-        guardrails_api_key = input("Set GuardRails API Key: ").strip()
+        guardrails_api_key = getpass("Set GuardRails API Key: ").strip()
         if len(guardrails_api_key) > 15:
             print("Using GuardRails API key with prefix: ", guardrails_api_key[:6])
 
     guardrail_config = GuardrailConfig(
         whylabs_endpoint=whylabs_endpoint,
         whylabs_api_key=whylabs_api_key,
         guardrails_endpoint=guardrails_endpoint,
@@ -198,13 +200,13 @@
 
     save_config = input("Do you want to save these settings to a configuration file? [y/n]: ").strip().lower()
     if save_config == "y" or save_config == "yes":
         try:
             os.makedirs(_CONFIG_DIR, exist_ok=True)
             guardrail_config.write(_DEFAULT_CONFIG_FILE)
         except Exception as e:  # noqa
-            LOGGER.exception(f"Failed to write the configuration file: {e}")
+            LOGGER.exception("Failed to write the configuration file.")
 
             print("Failed to write the configuration file.")
 
     print(f"Set config: {guardrail_config}")
     return guardrail_config
```

### Comparing `openllmtelemetry-0.0.1b5/openllmtelemetry/instrument.py` & `openllmtelemetry-0.0.1b6/openllmtelemetry/instrument.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,33 @@
 import os
 from logging import getLogger
-from typing import Dict, Optional, Tuple
+from typing import Optional
 
 from opentelemetry import trace
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.trace import Tracer
 
 from openllmtelemetry.config import load_config, load_dataset_id
 from openllmtelemetry.intrument_openai import init_instrumentors
 from openllmtelemetry.version import __version__
 
 LOGGER = getLogger(__name__)
 
-_tracer_cache: Dict[str, trace.Tracer] = {}
-_last_added_tracer: Optional[Tuple[str, trace.Tracer]] = None
-
 
 def instrument(
     application_name: Optional[str] = None,
     dataset_id: Optional[str] = None,
     tracer_name: Optional[str] = None,
     service_name: Optional[str] = None,
     disable_batching: bool = False,
+    debug: bool = False,
 ) -> Tracer:
-    global _tracer_cache, _last_added_tracer
-
     config = load_config()
     dataset_id = load_dataset_id(dataset_id)
-    if dataset_id is None:
-        raise ValueError(
-            "dataset_id must be specified in a parameter or in env var: e.g. "
-            "os.environ[\"WHYLABS_DEFAULT_DATASET_ID\"] = \"model-1\""
-        )
     guardrails_api = config.guardrail_client(default_dataset_id=dataset_id)
 
     if application_name is None:
         otel_service_name = os.environ.get("OTEL_SERVICE_NAME")
         if otel_service_name:
             application_name = otel_service_name
         else:
@@ -51,25 +42,14 @@
             "application.name": application_name,
             "version": __version__,
             "resource.id": dataset_id or "",  # TODO: resource id probably should be at the span level
         }
     )
 
     tracer_provider = TracerProvider(resource=resource)
-    config.config_tracer_provider(tracer_provider, dataset_id=dataset_id, disable_batching=disable_batching)
+    config.config_tracer_provider(tracer_provider, dataset_id=dataset_id, disable_batching=disable_batching, debug=debug)
 
     tracer = trace.get_tracer(tracer_name)
     trace.set_tracer_provider(tracer_provider)
-    _tracer_cache[tracer_name] = tracer
-    _last_added_tracer = (tracer_name, tracer)
 
     init_instrumentors(tracer, guardrails_api)
     return tracer
-
-
-def get_tracer(name: Optional[str] = None) -> Optional[Tracer]:
-    if _last_added_tracer is None:
-        return None
-    elif name is None:
-        return _last_added_tracer[1]
-    else:
-        return _tracer_cache.get(name)
```

### Comparing `openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/LICENSE` & `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/LICENSE`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/bedrock/__init__.py` & `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/bedrock/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 """
 Copyright 2024 traceloop
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
@@ -29,16 +28,16 @@
 from opentelemetry.instrumentation.utils import (
     _SUPPRESS_INSTRUMENTATION_KEY,
     unwrap,
 )
 from opentelemetry.trace import SpanKind, get_tracer
 from wrapt import wrap_function_wrapper
 
+from openllmtelemetry.guardrails import GuardrailsApi  # noqa: E402
 from openllmtelemetry.instrumentation.bedrock.reusable_streaming_body import ReusableStreamingBody
-from openllmtelemetry.secure import GuardrailsApi  # noqa: E402
 from openllmtelemetry.semantic_conventions.gen_ai import LLMRequestTypeValues, SpanAttributes
 from openllmtelemetry.version import __version__
 
 LOGGER = logging.getLogger(__name__)
 
 _instruments = ("boto3 >= 1.28.57",)
 
@@ -55,33 +54,34 @@
             span.set_attribute(name, value)
     return
 
 
 def _with_tracer_wrapper(func):
     """Helper for providing tracer for wrapper functions."""
 
-    def _with_tracer(tracer, secure_api: GuardrailsApi, to_wrap):
+    def _with_tracer(tracer, guardrails_api: GuardrailsApi, to_wrap):
         def wrapper(wrapped, instance, args, kwargs):
-            return func(tracer, secure_api, to_wrap, wrapped, instance, args, kwargs)
+            return func(tracer, guardrails_api, to_wrap, wrapped, instance, args, kwargs)
 
         return wrapper
 
     return _with_tracer
 
-def _handle_request(secure_api: Optional[GuardrailsApi], prompt: str, span):
+
+def _handle_request(guardrails_api: Optional[GuardrailsApi], prompt: str, span):
     prompt_metrics = None
     if prompt is not None:
-        prompt_metrics = secure_api.eval_prompt(prompt) if secure_api is not None else None
+        prompt_metrics = guardrails_api.eval_prompt(prompt) if guardrails_api is not None else None
     if prompt_metrics and span is not None:
-            LOGGER.debug(prompt_metrics)
-            metrics = prompt_metrics.metrics[0]
-            for k in metrics.additional_keys:
-                if metrics.additional_properties[k] is not None:
-                    metric_value = metrics.additional_properties[k]
-                    span.set_attribute(f"langkit.metrics.{k}", metric_value)
+        LOGGER.debug(prompt_metrics)
+        metrics = prompt_metrics.metrics[0]
+        for k in metrics.additional_keys:
+            if metrics.additional_properties[k] is not None:
+                metric_value = metrics.additional_properties[k]
+                span.set_attribute(f"langkit.metrics.{k}", metric_value)
     return prompt
 
 
 def _handle_response(secure_api: Optional[GuardrailsApi], prompt, response, span):
     response_text: Optional[str] = None
     response_metrics = None
     results = response.get("results")
@@ -139,14 +139,60 @@
                 prompt = request_body.get("prompt")
             elif vendor == "amazon":
                 if is_titan_text:
                     prompt = request_body["inputText"]
                 else:
                     LOGGER.debug("LLM not suppported yet")
             LOGGER.debug(f"extracted prompt: {prompt}")
+
+            def prompt_provider():
+                prompt = None
+                if vendor == "cohere":
+                    prompt = request_body.get("prompt")
+                elif vendor == "anthropic":
+                    prompt = request_body.get("inputText")
+                elif vendor == "ai21":
+                    prompt = request_body.get("prompt")
+                elif vendor == "meta":
+                    prompt = request_body.get("prompt")
+                elif vendor == "amazon":
+                    if is_titan_text:
+                        prompt = request_body["inputText"]
+                    else:
+                        LOGGER.debug("LLM not suppported yet")
+                LOGGER.debug(f"extracted prompt: {prompt}")
+                return prompt
+
+            def call_llm(span):
+                response = fn(*args, **kwargs)
+                response["body"] = ReusableStreamingBody(response["body"]._raw_stream, response["body"]._content_length)
+                return response
+
+            def prompt_attributes_setter(span):
+                _set_span_attribute(span, SpanAttributes.LLM_VENDOR, vendor)
+                _set_span_attribute(span, SpanAttributes.LLM_REQUEST_MODEL, model)
+
+                if vendor == "cohere":
+                    _set_cohere_span_attributes(span, request_body, {})
+                elif vendor == "anthropic":
+                    _set_anthropic_span_attributes(span, request_body, {})
+                elif vendor == "ai21":
+                    _set_ai21_span_attributes(span, request_body, {})
+                elif vendor == "meta":
+                    _set_llama_span_attributes(span, request_body, {})
+                elif vendor == "amazon":
+                    _set_amazon_titan_span_attributes(span, request_body, {})
+
+            def response_extractor(r):
+                if is_openai_v1():
+                    response_dict = model_as_dict(r)
+                else:
+                    response_dict = r
+                return response_dict["choices"][0]["text"]
+
             # TODO: check for input text first
             prompt = _handle_request(secure_api, prompt, span)
             response = fn(*args, **kwargs)
 
             response["body"] = ReusableStreamingBody(response["body"]._raw_stream, response["body"]._content_length)
             response_body = json.loads(response.get("body").read())
             response_body = _handle_response(secure_api, prompt, response_body, span)
```

### Comparing `openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py` & `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/__init__.py` & `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 Original source: openllmetry: https://github.com/traceloop/openllmetry
 """
 import logging
 from typing import Collection, Optional
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 
-from openllmtelemetry.secure import GuardrailsApi
+from openllmtelemetry.guardrails import GuardrailsApi
 
 from .utils import is_openai_v1
 from .v0 import OpenAIV0Instrumentor
 from .v1 import OpenAIV1Instrumentor
 
 _instruments = ("openai>=0.27.0",)
```

### Comparing `openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/shared/__init__.py` & `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/shared/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,19 +84,20 @@
         _set_span_attribute(span, SpanAttributes.LLM_REQUEST_MAX_TOKENS, kwargs.get("max_tokens"))
         _set_span_attribute(span, SpanAttributes.LLM_TEMPERATURE, kwargs.get("temperature"))
         _set_span_attribute(span, SpanAttributes.LLM_TOP_P, kwargs.get("top_p"))
         _set_span_attribute(span, SpanAttributes.LLM_FREQUENCY_PENALTY, kwargs.get("frequency_penalty"))
         _set_span_attribute(span, SpanAttributes.LLM_PRESENCE_PENALTY, kwargs.get("presence_penalty"))
         _set_span_attribute(span, SpanAttributes.LLM_USER, kwargs.get("user"))
         _set_span_attribute(span, SpanAttributes.LLM_HEADERS, str(kwargs.get("headers")))
+        _set_span_attribute(span, SpanAttributes.LLM_STREAMING, str(kwargs.get("stream")))
     except Exception as ex:  # pylint: disable=broad-except
         logger.warning("Failed to set input attributes for openai span, error: %s", str(ex))
 
 
-def _set_response_attributes(span, response):
+def _set_response_attributes(response, span):
     if not span.is_recording():
         return
 
     try:
         _set_span_attribute(span, SpanAttributes.LLM_RESPONSE_MODEL, response.get("model"))
 
         usage = response.get("usage")
```

### Comparing `openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py` & `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,81 +18,115 @@
 Original source: openllmetry: https://github.com/traceloop/openllmetry
 """
 import logging
 from typing import Optional
 
 from opentelemetry import context as context_api
 from opentelemetry.instrumentation.utils import _SUPPRESS_INSTRUMENTATION_KEY
-from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
+from openllmtelemetry.guardrails import GuardrailsApi
+from openllmtelemetry.guardrails.handlers import async_wrapper, sync_wrapper
 from openllmtelemetry.instrumentation.openai.shared import (
     _set_functions_attributes,
     _set_request_attributes,
     _set_response_attributes,
     _set_span_attribute,
     is_streaming_response,
     model_as_dict,
     should_send_prompts,
 )
 from openllmtelemetry.instrumentation.openai.utils import (
     _with_tracer_wrapper,
     is_openai_v1,
-    start_as_current_span_async,
 )
-from openllmtelemetry.secure import GuardrailsApi
 from openllmtelemetry.semantic_conventions.gen_ai import LLMRequestTypeValues, SpanAttributes
 
 SPAN_NAME = "openai.completion"
 LLM_REQUEST_TYPE = LLMRequestTypeValues.COMPLETION
 
 logger = logging.getLogger(__name__)
 
 
+def create_prompt_provider(kwargs):
+    def prompt_provider():
+        return kwargs.get("prompt")
+
+    return prompt_provider
+
+
 @_with_tracer_wrapper
-def completion_wrapper(tracer, secure_api: Optional[GuardrailsApi], wrapped, instance, args, kwargs):
+def completion_wrapper(tracer, guardrails_api: Optional[GuardrailsApi], wrapped, instance, args, kwargs):
     if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
         return wrapped(*args, **kwargs)
 
-    # span needs to be opened and closed manually because the response is a generator
-    span = tracer.start_span(
-        SPAN_NAME,
-        kind=SpanKind.CLIENT,
-        attributes={SpanAttributes.LLM_REQUEST_TYPE: LLM_REQUEST_TYPE.value},
-    )
+    prompt_provider = create_prompt_provider(kwargs)
 
-    _handle_request(span, kwargs)
-    response = wrapped(*args, **kwargs)
+    def call_llm(span):
+        r = wrapped(*args, **kwargs)
+        if not kwargs.get("stream"):
+            _handle_response(r, span)
+            if is_openai_v1():
+                response_dict = model_as_dict(r)
+            else:
+                response_dict = r
 
-    if is_streaming_response(response):
-        # span will be closed after the generator is done
-        return _build_from_streaming_response(span, response)
-    else:
-        _handle_response(response, span)
+            _set_response_attributes(response_dict, span)
+        return r
 
-    span.end()
-    return response
+    def prompt_attributes_setter(span):
+        _set_request_attributes(span, kwargs)
+
+    def response_extractor(r):
+        if is_openai_v1():
+            response_dict = model_as_dict(r)
+        else:
+            response_dict = r
+        return response_dict["choices"][0]["text"]
+
+    return sync_wrapper(
+        tracer, guardrails_api, prompt_provider, call_llm, response_extractor, prompt_attributes_setter, LLMRequestTypeValues.COMPLETION
+    )
 
 
 @_with_tracer_wrapper
-async def acompletion_wrapper(tracer, guard: Optional[GuardrailsApi], wrapped, instance, args, kwargs):
+async def acompletion_wrapper(tracer, guardrails_api: Optional[GuardrailsApi], wrapped, instance, args, kwargs):
     if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
         return wrapped(*args, **kwargs)
 
-    async with start_as_current_span_async(
-        tracer=tracer,
-        name=SPAN_NAME,
-        kind=SpanKind.CLIENT,
-        attributes={SpanAttributes.LLM_REQUEST_TYPE: LLM_REQUEST_TYPE.value},
-    ) as span:
-        _handle_request(span, kwargs)
-        response = await wrapped(*args, **kwargs)
-        _handle_response(response, span)
+    prompt_provider = create_prompt_provider(kwargs)
+
+    async def call_llm(span):
+        r = await wrapped(*args, **kwargs)
+        if not kwargs.get("stream"):
+            _handle_response(r, span)
+        return r
 
-        return response
+    def prompt_attributes_setter(span):
+        _set_request_attributes(span, kwargs)
+
+    def response_extractor(r):
+        if is_openai_v1():
+            response_dict = model_as_dict(r)
+        else:
+            response_dict = r
+        return response_dict["choices"][0]["text"]
+
+    return async_wrapper(
+        tracer,
+        guardrails_api,  # guardrails_client,
+        prompt_provider,
+        call_llm,
+        response_extractor,
+        kwargs,
+        prompt_attributes_setter,
+        _build_from_streaming_response,
+        is_streaming_response,
+        LLMRequestTypeValues.COMPLETION,
+    )
 
 
 def _handle_request(span, kwargs):
     _set_request_attributes(span, kwargs)
     if should_send_prompts():
         _set_prompts(span, kwargs.get("prompt"))
         _set_functions_attributes(span, kwargs.get("functions"))
@@ -100,15 +134,15 @@
 
 def _handle_response(response, span):
     if is_openai_v1():
         response_dict = model_as_dict(response)
     else:
         response_dict = response
 
-    _set_response_attributes(span, response_dict)
+    _set_response_attributes(response_dict, span)
 
     if should_send_prompts():
         _set_completions(span, response_dict.get("choices"))
 
 
 def _set_prompts(span, prompt):
     if not span.is_recording() or not prompt:
@@ -153,14 +187,14 @@
             if choice.get("finish_reason"):
                 complete_choice["finish_reason"] = choice.get("finish_reason")
 
             complete_choice["text"] += choice.get("text")
 
         yield item_to_yield
 
-    _set_response_attributes(span, complete_response)
+    _set_response_attributes(complete_response, span)
 
     if should_send_prompts():
         _set_completions(span, complete_response.get("choices"))
 
     span.set_status(Status(StatusCode.OK))
     span.end()
```

### Comparing `openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py` & `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
 def _handle_response(response, span):
     if is_openai_v1():
         response_dict = model_as_dict(response)
     else:
         response_dict = response
 
-    _set_response_attributes(span, response_dict)
+    _set_response_attributes(response_dict, span)
 
 
 def _set_prompts(span, prompt):
     if not span.is_recording() or not prompt:
         return
 
     try:
```

### Comparing `openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/utils.py` & `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/utils.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/v0/__init__.py` & `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/v0/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,28 +19,28 @@
 """
 from typing import Collection, Optional
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
+from openllmtelemetry.guardrails import GuardrailsApi
 from openllmtelemetry.instrumentation.openai.shared.chat_wrappers import (
     achat_wrapper,
     chat_wrapper,
 )
 from openllmtelemetry.instrumentation.openai.shared.completion_wrappers import (
     acompletion_wrapper,
     completion_wrapper,
 )
 from openllmtelemetry.instrumentation.openai.shared.embeddings_wrappers import (
     aembeddings_wrapper,
     embeddings_wrapper,
 )
 from openllmtelemetry.instrumentation.openai.version import __version__
-from openllmtelemetry.secure import GuardrailsApi
 
 _instruments = ("openai >= 0.27.0", "openai < 1.0.0")
 
 
 class OpenAIV0Instrumentor(BaseInstrumentor):
     def __init__(self, guard: Optional[GuardrailsApi]):
         self._guard = guard
```

### Comparing `openllmtelemetry-0.0.1b5/openllmtelemetry/instrumentation/openai/v1/__init__.py` & `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/v1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,28 +19,28 @@
 """
 from typing import Collection
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
+from openllmtelemetry.guardrails import GuardrailsApi
 from openllmtelemetry.instrumentation.openai.shared.chat_wrappers import (
     achat_wrapper,
     chat_wrapper,
 )
 from openllmtelemetry.instrumentation.openai.shared.completion_wrappers import (
     acompletion_wrapper,
     completion_wrapper,
 )
 from openllmtelemetry.instrumentation.openai.shared.embeddings_wrappers import (
     aembeddings_wrapper,
     embeddings_wrapper,
 )
 from openllmtelemetry.instrumentation.openai.version import __version__
-from openllmtelemetry.secure import GuardrailsApi
 
 _instruments = ("openai >= 1.0.0",)
 
 
 class OpenAIV1Instrumentor(BaseInstrumentor):
     def __init__(self, guard: GuardrailsApi):
         self._secure_api = guard
```

### Comparing `openllmtelemetry-0.0.1b5/openllmtelemetry/intrument_openai.py` & `openllmtelemetry-0.0.1b6/openllmtelemetry/intrument_openai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import importlib
 import logging
 from typing import Optional
 
 from opentelemetry.trace import Tracer
 
-from openllmtelemetry.secure import GuardrailsApi
+from openllmtelemetry.guardrails import GuardrailsApi
 
 LOGGER = logging.getLogger(__name__)
 
 
 def init_instrumentors(trace_provider: Tracer, secure_api: Optional[GuardrailsApi]):
     for instrumentor in [init_openai_instrumentor, init_bedrock_instrumentor]:
         instrumentor(trace_provider=trace_provider, secure_api=secure_api)
```

### Comparing `openllmtelemetry-0.0.1b5/openllmtelemetry/semantic_conventions/gen_ai/__init__.py` & `openllmtelemetry-0.0.1b6/openllmtelemetry/semantic_conventions/gen_ai/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     LLM_TOP_K = "llm.top_k"
     LLM_FREQUENCY_PENALTY = "llm.frequency_penalty"
     LLM_PRESENCE_PENALTY = "llm.presence_penalty"
     LLM_PROMPTS = "llm.prompts"
     LLM_COMPLETIONS = "llm.completions"
     LLM_CHAT_STOP_SEQUENCES = "llm.chat.stop_sequences"
     LLM_REQUEST_FUNCTIONS = "llm.request.functions"
+    LLM_STREAMING = "llm.streaming"
 
     # Vector DB
     VECTOR_DB_VENDOR = "vector_db.vendor"
     VECTOR_DB_QUERY_TOP_K = "vector_db.query.top_k"
 
 
 class Events(Enum):
```

### Comparing `openllmtelemetry-0.0.1b5/openllmtelemetry/span_exporter.py` & `openllmtelemetry-0.0.1b6/openllmtelemetry/span_exporter.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b5/pyproject.toml` & `openllmtelemetry-0.0.1b6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "OpenLLMTelemetry"
-version = "0.0.1.b5"
+version = "0.0.1.b6"
 description = "End-to-end observability with built-in security guardrails."
 authors = ["WhyLabs.ai <support@whylabs.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `openllmtelemetry-0.0.1b5/PKG-INFO` & `openllmtelemetry-0.0.1b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: OpenLLMTelemetry
-Version: 0.0.1b5
+Name: openllmtelemetry
+Version: 0.0.1b6
 Summary: End-to-end observability with built-in security guardrails.
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: support@whylabs.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

