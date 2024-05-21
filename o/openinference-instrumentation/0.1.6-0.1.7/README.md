# Comparing `tmp/openinference_instrumentation-0.1.6.tar.gz` & `tmp/openinference_instrumentation-0.1.7.tar.gz`

## Comparing `openinference_instrumentation-0.1.6.tar` & `openinference_instrumentation-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.6/src/openinference/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.6/src/openinference/instrumentation/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.6/src/openinference/instrumentation/version.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.6/.gitignore
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.6/LICENSE
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.6/README.md
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11173 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.7/src/openinference/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.7/src/openinference/instrumentation/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.7/src/openinference/instrumentation/version.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.7/.gitignore
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.7/LICENSE
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.7/README.md
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.7/PKG-INFO
```

### Comparing `openinference_instrumentation-0.1.6/src/openinference/instrumentation/__init__.py` & `openinference_instrumentation-0.1.7/src/openinference/instrumentation/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,27 +79,27 @@
     def attach_context(self) -> None:
         ctx = get_current()
         if self._session_id:
             ctx = set_value(SpanAttributes.SESSION_ID, self._session_id, ctx)
         if self._user_id:
             ctx = set_value(SpanAttributes.USER_ID, self._user_id, ctx)
         if self._metadata:
-            ctx = set_value(SpanAttributes.METADATA, json.dumps(self._metadata, default=str), ctx)
+            ctx = set_value(SpanAttributes.METADATA, safe_json_dumps(self._metadata), ctx)
         if self._tags:
             ctx = set_value(SpanAttributes.TAG_TAGS, self._tags, ctx)
         if self._prompt_template:
             ctx = set_value(SpanAttributes.LLM_PROMPT_TEMPLATE, self._prompt_template, ctx)
         if self._prompt_template_version:
             ctx = set_value(
                 SpanAttributes.LLM_PROMPT_TEMPLATE_VERSION, self._prompt_template_version, ctx
             )
         if self._prompt_template_variables:
             ctx = set_value(
                 SpanAttributes.LLM_PROMPT_TEMPLATE_VARIABLES,
-                json.dumps(self._prompt_template_variables, default=str),
+                safe_json_dumps(self._prompt_template_variables),
                 ctx,
             )
         self._token = attach(ctx)
 
     def __enter__(self) -> Self:
         self.attach_context()
         return self
@@ -316,7 +316,16 @@
         )
 
 
 def get_attributes_from_context() -> Iterator[Tuple[str, AttributeValue]]:
     for ctx_attr in CONTEXT_ATTRIBUTES:
         if (val := get_value(ctx_attr)) is not None:
             yield ctx_attr, val
+
+
+def safe_json_dumps(obj: Any, **kwargs: Any) -> str:
+    """
+    A convenience wrapper around `json.dumps` that ensures that any object can
+    be safely encoded without a `TypeError` and that non-ASCII Unicode
+    characters are not escaped.
+    """
+    return json.dumps(obj, default=str, ensure_ascii=False, **kwargs)
```

### Comparing `openinference_instrumentation-0.1.6/LICENSE` & `openinference_instrumentation-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation-0.1.6/pyproject.toml` & `openinference_instrumentation-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation-0.1.6/PKG-INFO` & `openinference_instrumentation-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openinference-instrumentation
-Version: 0.1.6
+Version: 0.1.7
 Summary: OpenInference instrumentation utilities
 Project-URL: Homepage, https://github.com/Arize-ai/openinference/tree/main/python/openinference-instrumentation
 Author-email: OpenInference Authors <oss@arize.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

