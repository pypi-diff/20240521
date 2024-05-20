# Comparing `tmp/codeflash-0.6.2.tar.gz` & `tmp/codeflash-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflash-0.6.2.tar", max compression
+gzip compressed data, was "codeflash-0.6.3.tar", max compression
```

## Comparing `codeflash-0.6.2.tar` & `codeflash-0.6.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0       11 2024-01-05 04:36:50.272525 codeflash-0.6.2/README.md
--rw-r--r--   0        0        0     4405 2024-05-14 02:15:39.711762 codeflash-0.6.2/codeflash/LICENSE
--rw-r--r--   0        0        0        0 2024-02-13 02:11:11.085505 codeflash-0.6.2/codeflash/__init__.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274581 codeflash-0.6.2/codeflash/api/__init__.py
--rw-r--r--   0        0        0     9081 2024-05-15 20:35:59.691603 codeflash-0.6.2/codeflash/api/aiservice.py
--rw-r--r--   0        0        0     4699 2024-05-11 03:50:31.229426 codeflash-0.6.2/codeflash/api/cfapi.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274847 codeflash-0.6.2/codeflash/cli_cmds/__init__.py
--rw-r--r--   0        0        0     8319 2024-05-11 03:50:31.229647 codeflash-0.6.2/codeflash/cli_cmds/cli.py
--rw-r--r--   0        0        0    22865 2024-04-18 20:02:37.017426 codeflash-0.6.2/codeflash/cli_cmds/cmd_init.py
--rw-r--r--   0        0        0      440 2024-04-16 22:27:44.247326 codeflash-0.6.2/codeflash/cli_cmds/logging_config.py
--rw-r--r--   0        0        0     1827 2024-03-24 21:57:44.196107 codeflash-0.6.2/codeflash/cli_cmds/workflows/codeflash-optimize.yaml
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.275400 codeflash-0.6.2/codeflash/code_utils/__init__.py
--rw-r--r--   0        0        0     9536 2024-05-13 05:06:56.603708 codeflash-0.6.2/codeflash/code_utils/code_extractor.py
--rw-r--r--   0        0        0     8556 2024-05-13 05:06:56.603994 codeflash-0.6.2/codeflash/code_utils/code_replacer.py
--rw-r--r--   0        0        0     2956 2024-05-11 03:50:31.230947 codeflash-0.6.2/codeflash/code_utils/code_utils.py
--rw-r--r--   0        0        0      273 2024-04-15 22:14:14.315668 codeflash-0.6.2/codeflash/code_utils/compat.py
--rw-r--r--   0        0        0      224 2024-02-10 04:17:44.568348 codeflash-0.6.2/codeflash/code_utils/config_consts.py
--rw-r--r--   0        0        0     3908 2024-04-18 23:42:01.686181 codeflash-0.6.2/codeflash/code_utils/config_parser.py
--rw-r--r--   0        0        0     2880 2024-04-18 22:25:22.392531 codeflash-0.6.2/codeflash/code_utils/env_utils.py
--rw-r--r--   0        0        0     2056 2024-05-11 03:50:31.232101 codeflash-0.6.2/codeflash/code_utils/formatter.py
--rw-r--r--   0        0        0     3329 2024-05-13 05:06:56.604437 codeflash-0.6.2/codeflash/code_utils/git_utils.py
--rw-r--r--   0        0        0    23837 2024-05-15 20:35:59.692389 codeflash-0.6.2/codeflash/code_utils/instrument_existing_tests.py
--rw-r--r--   0        0        0     3497 2024-04-18 23:24:18.257591 codeflash-0.6.2/codeflash/code_utils/shell_utils.py
--rw-r--r--   0        0        0     1007 2024-01-05 04:36:50.277228 codeflash-0.6.2/codeflash/code_utils/sqlalchemy_utils.py
--rw-r--r--   0        0        0     1898 2024-05-13 05:06:56.605285 codeflash-0.6.2/codeflash/code_utils/time_utils.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277391 codeflash-0.6.2/codeflash/discovery/__init__.py
--rw-r--r--   0        0        0    18567 2024-05-11 03:50:31.233149 codeflash-0.6.2/codeflash/discovery/discover_unit_tests.py
--rw-r--r--   0        0        0    20032 2024-05-14 17:53:59.915027 codeflash-0.6.2/codeflash/discovery/functions_to_optimize.py
--rw-r--r--   0        0        0     1230 2024-04-18 03:01:28.780898 codeflash-0.6.2/codeflash/github/PrComment.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277833 codeflash-0.6.2/codeflash/github/__init__.py
--rw-r--r--   0        0        0      725 2024-05-07 21:23:45.633992 codeflash-0.6.2/codeflash/main.py
--rw-r--r--   0        0        0      133 2024-05-11 03:50:31.233935 codeflash-0.6.2/codeflash/models/ExperimentMetadata.py
--rw-r--r--   0        0        0        0 2024-05-11 03:50:31.233961 codeflash-0.6.2/codeflash/models/__init__.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.278392 codeflash-0.6.2/codeflash/optimization/__init__.py
--rw-r--r--   0        0        0    11557 2024-05-06 18:43:33.547955 codeflash-0.6.2/codeflash/optimization/function_context.py
--rw-r--r--   0        0        0    54500 2024-05-14 17:53:59.915560 codeflash-0.6.2/codeflash/optimization/optimizer.py
--rw-r--r--   0        0        0        0 2024-01-29 22:33:50.970495 codeflash-0.6.2/codeflash/result/__init__.py
--rw-r--r--   0        0        0     4539 2024-05-13 05:06:56.606567 codeflash-0.6.2/codeflash/result/create_pr.py
--rw-r--r--   0        0        0     1992 2024-05-13 05:06:56.607228 codeflash-0.6.2/codeflash/result/explanation.py
--rw-r--r--   0        0        0        0 2024-03-19 02:04:16.181069 codeflash-0.6.2/codeflash/telemetry/__init__.py
--rw-r--r--   0        0        0     1247 2024-04-19 00:07:03.195469 codeflash-0.6.2/codeflash/telemetry/posthog.py
--rw-r--r--   0        0        0      579 2024-03-19 02:04:16.181306 codeflash-0.6.2/codeflash/telemetry/sentry.py
--rw-r--r--   0        0        0    20467 2024-05-11 03:50:31.235086 codeflash-0.6.2/codeflash/tracer.py
--rw-r--r--   0        0        0        1 2024-05-11 03:50:31.235685 codeflash-0.6.2/codeflash/tracing/__init__.py
--rw-r--r--   0        0        0     2644 2024-05-11 03:50:31.235798 codeflash-0.6.2/codeflash/tracing/profile_stats.py
--rw-r--r--   0        0        0     5942 2024-05-11 03:50:31.235999 codeflash-0.6.2/codeflash/tracing/replay_test.py
--rw-r--r--   0        0        0      210 2024-05-09 02:05:53.366617 codeflash-0.6.2/codeflash/tracing/tracing_utils.py
--rw-r--r--   0        0        0     1905 2024-04-18 03:01:28.781529 codeflash-0.6.2/codeflash/update_license_version.py
--rw-r--r--   0        0        0        0 2024-01-20 20:41:44.799451 codeflash-0.6.2/codeflash/verification/__init__.py
--rw-r--r--   0        0        0     4977 2024-05-11 03:50:31.236508 codeflash-0.6.2/codeflash/verification/comparator.py
--rw-r--r--   0        0        0     1241 2024-05-14 17:53:59.915887 codeflash-0.6.2/codeflash/verification/equivalence.py
--rw-r--r--   0        0        0    14621 2024-05-11 03:50:31.236755 codeflash-0.6.2/codeflash/verification/parse_test_output.py
--rw-r--r--   0        0        0     6776 2024-05-11 03:50:31.237209 codeflash-0.6.2/codeflash/verification/test_results.py
--rw-r--r--   0        0        0     1852 2024-05-11 03:50:31.237506 codeflash-0.6.2/codeflash/verification/test_runner.py
--rw-r--r--   0        0        0     2338 2024-05-09 02:05:53.368797 codeflash-0.6.2/codeflash/verification/verification_utils.py
--rw-r--r--   0        0        0     4200 2024-05-11 03:50:31.238025 codeflash-0.6.2/codeflash/verification/verifier.py
--rw-r--r--   0        0        0      150 2024-05-15 20:37:08.800953 codeflash-0.6.2/codeflash/version.py
--rw-r--r--   0        0        0     2963 2024-05-15 20:37:08.800212 codeflash-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     1447 1970-01-01 00:00:00.000000 codeflash-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-01-05 04:36:50.272525 codeflash-0.6.3/README.md
+-rw-r--r--   0        0        0     4405 2024-05-15 20:37:10.891716 codeflash-0.6.3/codeflash/LICENSE
+-rw-r--r--   0        0        0        0 2024-02-13 02:11:11.085505 codeflash-0.6.3/codeflash/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274581 codeflash-0.6.3/codeflash/api/__init__.py
+-rw-r--r--   0        0        0     8992 2024-05-20 22:02:25.658457 codeflash-0.6.3/codeflash/api/aiservice.py
+-rw-r--r--   0        0        0     4699 2024-05-11 03:50:31.229426 codeflash-0.6.3/codeflash/api/cfapi.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274847 codeflash-0.6.3/codeflash/cli_cmds/__init__.py
+-rw-r--r--   0        0        0     8319 2024-05-11 03:50:31.229647 codeflash-0.6.3/codeflash/cli_cmds/cli.py
+-rw-r--r--   0        0        0    22865 2024-04-18 20:02:37.017426 codeflash-0.6.3/codeflash/cli_cmds/cmd_init.py
+-rw-r--r--   0        0        0      440 2024-04-16 22:27:44.247326 codeflash-0.6.3/codeflash/cli_cmds/logging_config.py
+-rw-r--r--   0        0        0     1827 2024-03-24 21:57:44.196107 codeflash-0.6.3/codeflash/cli_cmds/workflows/codeflash-optimize.yaml
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.275400 codeflash-0.6.3/codeflash/code_utils/__init__.py
+-rw-r--r--   0        0        0     9536 2024-05-13 05:06:56.603708 codeflash-0.6.3/codeflash/code_utils/code_extractor.py
+-rw-r--r--   0        0        0     8556 2024-05-13 05:06:56.603994 codeflash-0.6.3/codeflash/code_utils/code_replacer.py
+-rw-r--r--   0        0        0     2956 2024-05-11 03:50:31.230947 codeflash-0.6.3/codeflash/code_utils/code_utils.py
+-rw-r--r--   0        0        0      273 2024-04-15 22:14:14.315668 codeflash-0.6.3/codeflash/code_utils/compat.py
+-rw-r--r--   0        0        0      224 2024-02-10 04:17:44.568348 codeflash-0.6.3/codeflash/code_utils/config_consts.py
+-rw-r--r--   0        0        0     3908 2024-04-18 23:42:01.686181 codeflash-0.6.3/codeflash/code_utils/config_parser.py
+-rw-r--r--   0        0        0     2880 2024-04-18 22:25:22.392531 codeflash-0.6.3/codeflash/code_utils/env_utils.py
+-rw-r--r--   0        0        0     2056 2024-05-11 03:50:31.232101 codeflash-0.6.3/codeflash/code_utils/formatter.py
+-rw-r--r--   0        0        0     3345 2024-05-19 03:53:17.610537 codeflash-0.6.3/codeflash/code_utils/git_utils.py
+-rw-r--r--   0        0        0    23837 2024-05-19 03:53:17.611076 codeflash-0.6.3/codeflash/code_utils/instrument_existing_tests.py
+-rw-r--r--   0        0        0     3497 2024-04-18 23:24:18.257591 codeflash-0.6.3/codeflash/code_utils/shell_utils.py
+-rw-r--r--   0        0        0     1007 2024-01-05 04:36:50.277228 codeflash-0.6.3/codeflash/code_utils/sqlalchemy_utils.py
+-rw-r--r--   0        0        0     1898 2024-05-13 05:06:56.605285 codeflash-0.6.3/codeflash/code_utils/time_utils.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277391 codeflash-0.6.3/codeflash/discovery/__init__.py
+-rw-r--r--   0        0        0    18567 2024-05-11 03:50:31.233149 codeflash-0.6.3/codeflash/discovery/discover_unit_tests.py
+-rw-r--r--   0        0        0    20032 2024-05-14 17:53:59.915027 codeflash-0.6.3/codeflash/discovery/functions_to_optimize.py
+-rw-r--r--   0        0        0     1291 2024-05-20 22:02:25.659212 codeflash-0.6.3/codeflash/github/PrComment.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277833 codeflash-0.6.3/codeflash/github/__init__.py
+-rw-r--r--   0        0        0      725 2024-05-07 21:23:45.633992 codeflash-0.6.3/codeflash/main.py
+-rw-r--r--   0        0        0      133 2024-05-11 03:50:31.233935 codeflash-0.6.3/codeflash/models/ExperimentMetadata.py
+-rw-r--r--   0        0        0        0 2024-05-11 03:50:31.233961 codeflash-0.6.3/codeflash/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.278392 codeflash-0.6.3/codeflash/optimization/__init__.py
+-rw-r--r--   0        0        0    11999 2024-05-20 22:02:25.659613 codeflash-0.6.3/codeflash/optimization/function_context.py
+-rw-r--r--   0        0        0    54363 2024-05-20 22:02:25.660170 codeflash-0.6.3/codeflash/optimization/optimizer.py
+-rw-r--r--   0        0        0        0 2024-01-29 22:33:50.970495 codeflash-0.6.3/codeflash/result/__init__.py
+-rw-r--r--   0        0        0     4539 2024-05-13 05:06:56.606567 codeflash-0.6.3/codeflash/result/create_pr.py
+-rw-r--r--   0        0        0     1992 2024-05-13 05:06:56.607228 codeflash-0.6.3/codeflash/result/explanation.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:04:16.181069 codeflash-0.6.3/codeflash/telemetry/__init__.py
+-rw-r--r--   0        0        0     1247 2024-04-19 00:07:03.195469 codeflash-0.6.3/codeflash/telemetry/posthog.py
+-rw-r--r--   0        0        0      579 2024-03-19 02:04:16.181306 codeflash-0.6.3/codeflash/telemetry/sentry.py
+-rw-r--r--   0        0        0    20467 2024-05-11 03:50:31.235086 codeflash-0.6.3/codeflash/tracer.py
+-rw-r--r--   0        0        0        1 2024-05-11 03:50:31.235685 codeflash-0.6.3/codeflash/tracing/__init__.py
+-rw-r--r--   0        0        0     2644 2024-05-11 03:50:31.235798 codeflash-0.6.3/codeflash/tracing/profile_stats.py
+-rw-r--r--   0        0        0     5942 2024-05-11 03:50:31.235999 codeflash-0.6.3/codeflash/tracing/replay_test.py
+-rw-r--r--   0        0        0      210 2024-05-09 02:05:53.366617 codeflash-0.6.3/codeflash/tracing/tracing_utils.py
+-rw-r--r--   0        0        0     1905 2024-04-18 03:01:28.781529 codeflash-0.6.3/codeflash/update_license_version.py
+-rw-r--r--   0        0        0        0 2024-01-20 20:41:44.799451 codeflash-0.6.3/codeflash/verification/__init__.py
+-rw-r--r--   0        0        0     4977 2024-05-11 03:50:31.236508 codeflash-0.6.3/codeflash/verification/comparator.py
+-rw-r--r--   0        0        0     1241 2024-05-14 17:53:59.915887 codeflash-0.6.3/codeflash/verification/equivalence.py
+-rw-r--r--   0        0        0    14621 2024-05-11 03:50:31.236755 codeflash-0.6.3/codeflash/verification/parse_test_output.py
+-rw-r--r--   0        0        0     6839 2024-05-19 03:53:17.612310 codeflash-0.6.3/codeflash/verification/test_results.py
+-rw-r--r--   0        0        0     1852 2024-05-11 03:50:31.237506 codeflash-0.6.3/codeflash/verification/test_runner.py
+-rw-r--r--   0        0        0     2338 2024-05-09 02:05:53.368797 codeflash-0.6.3/codeflash/verification/verification_utils.py
+-rw-r--r--   0        0        0     4191 2024-05-20 22:02:25.660439 codeflash-0.6.3/codeflash/verification/verifier.py
+-rw-r--r--   0        0        0      150 2024-05-20 22:09:46.506693 codeflash-0.6.3/codeflash/version.py
+-rw-r--r--   0        0        0     2963 2024-05-20 22:09:46.505324 codeflash-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     1447 1970-01-01 00:00:00.000000 codeflash-0.6.3/PKG-INFO
```

### Comparing `codeflash-0.6.2/codeflash/LICENSE` & `codeflash-0.6.3/codeflash/LICENSE`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/api/aiservice.py` & `codeflash-0.6.3/codeflash/api/aiservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,28 +152,28 @@
         except requests.exceptions.RequestException as e:
             logging.exception(f"Error logging features: {e}")
 
     def generate_regression_tests(
         self,
         source_code_being_tested: str,
         function_to_optimize: FunctionToOptimize,
-        dependent_function_names: list[str],
+        helper_function_names: list[str],
         module_path: str,
         test_module_path: str,
         test_framework: str,
         test_timeout: int,
         trace_id: str,
     ) -> Optional[Tuple[str, str]]:
         """Generate regression tests for the given function by making a request to the Django endpoint.
 
         Parameters
         ----------
         - source_code_being_tested (str): The source code of the function being tested.
         - function_to_optimize (FunctionToOptimize): The function to optimize.
-        - dependent_function_names (list[Source]): List of dependent function names.
+        - helper_function_names (list[Source]): List of helper function names.
         - module_path (str): The module path where the function is located.
         - test_module_path (str): The module path for the test code.
         - test_framework (str): The test framework to use, e.g., "pytest".
         - test_timeout (int): The timeout for each test in seconds.
 
         Returns
         -------
@@ -183,15 +183,15 @@
         assert test_framework in [
             "pytest",
             "unittest",
         ], f"Invalid test framework, got {test_framework} but expected 'pytest' or 'unittest'"
         payload = {
             "source_code_being_tested": source_code_being_tested,
             "function_to_optimize": function_to_optimize,
-            "dependent_function_names": dependent_function_names,
+            "helper_function_names": helper_function_names,
             "module_path": module_path,
             "test_module_path": test_module_path,
             "test_framework": test_framework,
             "test_timeout": test_timeout,
             "trace_id": trace_id,
             "python_version": platform.python_version(),
         }
@@ -204,28 +204,27 @@
 
         # the timeout should be the same as the timeout for the AI service backend
 
         if response.status_code == 200:
             response_json = response.json()
             logging.info(f"Generated tests for function {function_to_optimize.function_name}")
             return response_json["generated_tests"], response_json["instrumented_tests"]
-        else:
-            try:
-                error = response.json()["error"]
-                logging.error(f"Error generating tests: {response.status_code} - {error}")
-                ph(
-                    "cli-testgen-error-response",
-                    {"response_status_code": response.status_code, "error": error},
-                )
-                return None
-            except Exception:
-                logging.exception(f"Error generating tests: {response.status_code} - {response.text}")
-                ph(
-                    "cli-testgen-error-response",
-                    {"response_status_code": response.status_code, "error": response.text},
-                )
-                return None
+        try:
+            error = response.json()["error"]
+            logging.error(f"Error generating tests: {response.status_code} - {error}")
+            ph(
+                "cli-testgen-error-response",
+                {"response_status_code": response.status_code, "error": error},
+            )
+            return None
+        except Exception:
+            logging.exception(f"Error generating tests: {response.status_code} - {response.text}")
+            ph(
+                "cli-testgen-error-response",
+                {"response_status_code": response.status_code, "error": response.text},
+            )
+            return None
 
 
 class LocalAiServiceClient(AiServiceClient):
     def get_aiservice_base_url(self) -> str:
         return "http://localhost:8000"
```

### Comparing `codeflash-0.6.2/codeflash/api/cfapi.py` & `codeflash-0.6.3/codeflash/api/cfapi.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/cli_cmds/cli.py` & `codeflash-0.6.3/codeflash/cli_cmds/cli.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/cli_cmds/cmd_init.py` & `codeflash-0.6.3/codeflash/cli_cmds/cmd_init.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/cli_cmds/workflows/codeflash-optimize.yaml` & `codeflash-0.6.3/codeflash/cli_cmds/workflows/codeflash-optimize.yaml`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/code_utils/code_extractor.py` & `codeflash-0.6.3/codeflash/code_utils/code_extractor.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/code_utils/code_replacer.py` & `codeflash-0.6.3/codeflash/code_utils/code_replacer.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/code_utils/code_utils.py` & `codeflash-0.6.3/codeflash/code_utils/code_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/code_utils/config_parser.py` & `codeflash-0.6.3/codeflash/code_utils/config_parser.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/code_utils/env_utils.py` & `codeflash-0.6.3/codeflash/code_utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/code_utils/formatter.py` & `codeflash-0.6.3/codeflash/code_utils/formatter.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/code_utils/git_utils.py` & `codeflash-0.6.3/codeflash/code_utils/git_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 def get_remote_url(repo: Optional[Repo] = None) -> str:
     repository: Repo = repo if repo else git.Repo(search_parent_directories=True)
     return repository.remote().url
 
 
 def get_repo_owner_and_name(repo: Optional[Repo] = None) -> tuple[str, str]:
     remote_url = get_remote_url(repo)  # call only once
-    remote_url = remote_url.rstrip(".git") if remote_url.endswith(".git") else remote_url
+    remote_url = get_remote_url(repo).removesuffix(".git") if remote_url.endswith(".git") else remote_url
     split_url = remote_url.split("/")
     repo_owner_with_github, repo_name = split_url[-2], split_url[-1]
     repo_owner = (
         repo_owner_with_github.split(":")[1] if ":" in repo_owner_with_github else repo_owner_with_github
     )
     return repo_owner, repo_name
```

### Comparing `codeflash-0.6.2/codeflash/code_utils/instrument_existing_tests.py` & `codeflash-0.6.3/codeflash/code_utils/instrument_existing_tests.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/code_utils/shell_utils.py` & `codeflash-0.6.3/codeflash/code_utils/shell_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/code_utils/sqlalchemy_utils.py` & `codeflash-0.6.3/codeflash/code_utils/sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/code_utils/time_utils.py` & `codeflash-0.6.3/codeflash/code_utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/discovery/discover_unit_tests.py` & `codeflash-0.6.3/codeflash/discovery/discover_unit_tests.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/discovery/functions_to_optimize.py` & `codeflash-0.6.3/codeflash/discovery/functions_to_optimize.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/github/PrComment.py` & `codeflash-0.6.3/codeflash/github/PrComment.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Union
 
 from pydantic import BaseModel
 from pydantic.dataclasses import dataclass
 
+from codeflash.code_utils.time_utils import humanize_runtime
 from codeflash.verification.test_results import TestResults
 
 
 @dataclass(frozen=True, config={"arbitrary_types_allowed": True})
 class PrComment:
     optimization_explanation: str
     best_runtime: int
@@ -16,16 +17,16 @@
     speedup_x: str
     speedup_pct: str
     winning_test_results: TestResults
 
     def to_json(self) -> dict[str, Union[str, dict[str, dict[str, int]]]]:
         return {
             "optimization_explanation": self.optimization_explanation,
-            "best_runtime": f"{(self.best_runtime / 1000):.2f}",
-            "original_runtime": f"{(self.original_runtime / 1000):.2f}",
+            "best_runtime": humanize_runtime(self.best_runtime),
+            "original_runtime": humanize_runtime(self.original_runtime),
             "function_name": self.function_name,
             "file_path": self.relative_file_path,
             "speedup_x": self.speedup_x,
             "speedup_pct": self.speedup_pct,
             "report_table": {
                 test_type.to_name(): result
                 for test_type, result in self.winning_test_results.get_test_pass_fail_report_by_type().items()
```

### Comparing `codeflash-0.6.2/codeflash/main.py` & `codeflash-0.6.3/codeflash/main.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/optimization/function_context.py` & `codeflash-0.6.3/codeflash/optimization/function_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,82 +50,116 @@
         module: ast.Module = ast.parse(file_contents)
     except SyntaxError as e:
         logging.exception(f"get_type_annotation_context - Syntax error in code: {e}")
         return []
     sources: list[tuple[Source, str, str]] = []
     ast_parents: list[FunctionParent] = []
 
+    def get_annotation_source(
+        jedi_script: jedi.Script,
+        name: str,
+        node_parents,
+        line_no: int,
+        col_no: str,
+    ) -> str:
+        try:
+            definition: list[Name] = jedi_script.goto(
+                line=line_no,
+                column=col_no,
+                follow_imports=True,
+                follow_builtin_imports=False,
+            )
+        except Exception as ex:
+            if hasattr(name, "full_name"):
+                logging.exception(
+                    f"Error while getting definition for {name.full_name}: {ex}",
+                )
+            else:
+                logging.exception(f"Error while getting definition: {ex}")
+            definition = []
+        if definition:  # TODO can be multiple definitions
+            definition_path = str(definition[0].module_path)
+            # The definition is part of this project and not defined within the original function
+            if (
+                definition_path.startswith(project_root_path + os.sep)
+                and definition[0].full_name
+                and not path_belongs_to_site_packages(definition_path)
+                and not belongs_to_function(definition[0], function_name)
+            ):
+                source_code = get_code(
+                    [
+                        FunctionToOptimize(
+                            definition[0].name,
+                            definition_path,
+                            node_parents[:-1],
+                        ),
+                    ],
+                )[0]
+                if source_code:
+                    sources.append(
+                        (
+                            Source(
+                                definition[0].name,
+                                definition[0],
+                                source_code,
+                            ),
+                            definition_path,
+                            definition[0].full_name.removeprefix(
+                                definition[0].module_name + ".",
+                            ),
+                        ),
+                    )
+
     def visit_children(
         node: Union[ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef, ast.Module],
         node_parents: list[FunctionParent],
     ) -> None:
         child: Union[ast.AST, ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef, ast.Module]
         for child in ast.iter_child_nodes(node):
             visit(child, node_parents)
 
+    def visit_all_annotation_children(
+        node: Union[ast.Subscript, ast.Name, ast.BinOp],
+        node_parents: list[FunctionParent],
+    ) -> None:
+        if isinstance(node, ast.BinOp) and isinstance(node.op, ast.BitOr):
+            visit_all_annotation_children(node.left, node_parents)
+            visit_all_annotation_children(node.right, node_parents)
+        if isinstance(node, ast.Name) and hasattr(node, "id"):
+            name: str = node.id
+            line_no: int = node.lineno
+            col_no: int = node.col_offset
+            get_annotation_source(jedi_script, name, node_parents, line_no, col_no)
+        if isinstance(node, ast.Subscript):
+            if hasattr(node, "slice"):
+                if isinstance(node.slice, ast.Subscript):
+                    visit_all_annotation_children(node.slice, node_parents)
+                elif isinstance(node.slice, ast.Tuple):
+                    for elt in node.slice.elts:
+                        if isinstance(elt, (ast.Name, ast.Subscript)):
+                            visit_all_annotation_children(elt, node_parents)
+                elif isinstance(node.slice, ast.Name):
+                    visit_all_annotation_children(node.slice, node_parents)
+            if hasattr(node, "value"):
+                visit_all_annotation_children(node.value, node_parents)
+
     def visit(
         node: Union[ast.AST, ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef, ast.Module],
         node_parents: list[FunctionParent],
     ) -> None:
         if isinstance(node, (ast.Module, ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef)):
             if isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef)):
                 if node.name == function_name and node_parents == function.parents:
                     arg: ast.arg
                     for arg in node.args.args:
-                        if arg.annotation and hasattr(arg.annotation, "id"):
-                            name: str = arg.annotation.id
-                            line_no: int = arg.annotation.lineno
-                            col_no: int = arg.annotation.col_offset
-                            try:
-                                definition: list[Name] = jedi_script.goto(
-                                    line=line_no,
-                                    column=col_no,
-                                    follow_imports=True,
-                                    follow_builtin_imports=False,
-                                )
-                            except Exception as ex:
-                                if hasattr(name, "full_name"):
-                                    logging.exception(
-                                        f"Error while getting definition for {name.full_name}: {ex}",
-                                    )
-                                else:
-                                    logging.exception(f"Error while getting definition: {ex}")
-                                definition = []
-                            if definition:  # TODO can be multiple definitions
-                                definition_path = str(definition[0].module_path)
-                                # The definition is part of this project and not defined within the original function
-                                if (
-                                    definition_path.startswith(project_root_path + os.sep)
-                                    and definition[0].full_name
-                                    and not path_belongs_to_site_packages(definition_path)
-                                    and not belongs_to_function(definition[0], function_name)
-                                ):
-                                    source_code = get_code(
-                                        [
-                                            FunctionToOptimize(
-                                                definition[0].name,
-                                                definition_path,
-                                                node_parents[:-1],
-                                            ),
-                                        ],
-                                    )[0]
-                                    if source_code:
-                                        sources.append(
-                                            (
-                                                Source(
-                                                    definition[0].name,
-                                                    definition[0],
-                                                    source_code,
-                                                ),
-                                                definition_path,
-                                                definition[0].full_name.removeprefix(
-                                                    definition[0].module_name + ".",
-                                                ),
-                                            ),
-                                        )
+                        if arg.annotation:
+                            visit_all_annotation_children(arg.annotation, node_parents)
+                    if node.returns:
+                        visit_all_annotation_children(node.returns, node_parents)
+
             if not isinstance(node, ast.Module):
                 node_parents.append(FunctionParent(node.name, type(node).__name__))
             visit_children(node, node_parents)
             if not isinstance(node, ast.Module):
                 node_parents.pop()
 
     visit(module, ast_parents)
@@ -155,44 +189,43 @@
                 ) and belongs_to_function(ref, function_name):
                     names.append(ref)
             elif belongs_to_function(ref, function_name):
                 names.append(ref)
 
     for name in names:
         try:
-            definitions: list[Name] = script.goto(
-                line=name.line,
-                column=name.column,
+            definitions: list[Name] = name.goto(
                 follow_imports=True,
                 follow_builtin_imports=False,
             )
         except Exception as e:
             try:
                 logging.exception(f"Error while getting definition for {name.full_name}: {e}")
             except Exception as e:
                 # name.full_name can also throw exceptions sometimes
                 logging.exception(f"Error while getting definition: {e}")
             definitions = []
         if definitions:
             # TODO: there can be multiple definitions, see how to handle such cases
-            definition_path = str(definitions[0].module_path)
+            definition = definitions[0]
+            definition_path = str(definition.module_path)
             # The definition is part of this project and not defined within the original function
             if (
                 definition_path.startswith(project_root_path + os.sep)
                 and not path_belongs_to_site_packages(definition_path)
-                and definitions[0].full_name
-                and not belongs_to_function(definitions[0], function_name)
+                and definition.full_name
+                and not belongs_to_function(definition, function_name)
             ):
                 source_code = get_code_no_skeleton(definition_path, definitions[0].name)
                 if source_code:
                     sources.append(
                         (
-                            Source(name.full_name, definitions[0], source_code),
+                            Source(definition.full_name, definition, source_code),
                             definition_path,
-                            name.full_name.removeprefix(name.module_name + "."),
+                            definition.full_name.removeprefix(name.module_name + "."),
                         ),
                     )
     annotation_sources = get_type_annotation_context(
         function_to_optimize,
         script,
         project_root_path,
     )
@@ -205,48 +238,45 @@
             existing_full_names.add(source[0].full_name)
     return deduped_sources
 
 
 MAX_PROMPT_TOKENS = 4096  # 128000  # gpt-4-128k
 
 
-def get_constrained_function_context_and_dependent_functions(
+def get_constrained_function_context_and_helper_functions(
     function_to_optimize: FunctionToOptimize,
     project_root_path: str,
     code_to_optimize: str,
     max_tokens: int = MAX_PROMPT_TOKENS,
 ) -> tuple[str, list[tuple[Source, str, str]]]:
     # TODO: Not just do static analysis, but also find the datatypes of function arguments by running the existing
     #  unittests and inspecting the arguments to resolve the real definitions and dependencies.
-    dependent_functions: list[tuple[Source, str, str]] = get_function_variables_definitions(
+    helper_functions: list[tuple[Source, str, str]] = get_function_variables_definitions(
         function_to_optimize,
         project_root_path,
     )
     tokenizer = tiktoken.encoding_for_model("gpt-3.5-turbo")
     code_to_optimize_tokens = tokenizer.encode(code_to_optimize)
 
     if not function_to_optimize.parents:
-        dependent_functions_sources = [function[0].source_code for function in dependent_functions]
+        helper_functions_sources = [function[0].source_code for function in helper_functions]
     else:
-        dependent_functions_sources = [
+        helper_functions_sources = [
             function[0].source_code
-            for function in dependent_functions
-            if not function[2].count(".")
-            or function[2].split(".")[0] != function_to_optimize.parents[0].name
+            for function in helper_functions
+            if not function[2].count(".") or function[2].split(".")[0] != function_to_optimize.parents[0].name
         ]
-    dependent_functions_tokens = [
-        len(tokenizer.encode(function)) for function in dependent_functions_sources
-    ]
+    helper_functions_tokens = [len(tokenizer.encode(function)) for function in helper_functions_sources]
 
     context_list = []
     context_len = len(code_to_optimize_tokens)
     logging.debug(f"ORIGINAL CODE TOKENS LENGTH: {context_len}")
-    logging.debug(f"ALL DEPENDENCIES TOKENS LENGTH: {sum(dependent_functions_tokens)}")
-    for function_source, source_len in zip(dependent_functions_sources, dependent_functions_tokens):
+    logging.debug(f"ALL DEPENDENCIES TOKENS LENGTH: {sum(helper_functions_tokens)}")
+    for function_source, source_len in zip(helper_functions_sources, helper_functions_tokens):
         if context_len + source_len <= max_tokens:
             context_list.append(function_source)
             context_len += source_len
         else:
             break
     logging.debug("FINAL OPTIMIZATION CONTEXT TOKENS LENGTH:", context_len)
-    dependent_code: str = "\n".join(context_list)
-    return dependent_code, dependent_functions
+    helper_code: str = "\n".join(context_list)
+    return helper_code, helper_functions
```

### Comparing `codeflash-0.6.2/codeflash/optimization/optimizer.py` & `codeflash-0.6.3/codeflash/optimization/optimizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     FunctionParent,
     FunctionToOptimize,
     get_functions_to_optimize,
 )
 from codeflash.models.ExperimentMetadata import ExperimentMetadata
 from codeflash.optimization.function_context import (
     Source,
-    get_constrained_function_context_and_dependent_functions,
+    get_constrained_function_context_and_helper_functions,
 )
 from codeflash.result.create_pr import check_create_pr, existing_tests_source_for
 from codeflash.result.explanation import Explanation
 from codeflash.telemetry import posthog
 from codeflash.telemetry.posthog import ph
 from codeflash.telemetry.sentry import init_sentry
 from codeflash.verification.equivalence import compare_test_results
@@ -67,46 +67,46 @@
 from codeflash.verification.test_runner import run_tests
 from codeflash.verification.verification_utils import TestConfig, get_test_file_path
 from codeflash.verification.verifier import generate_tests
 
 
 class OptimizationSet(BaseModel):
     control: list[OptimizedCandidate]
-    experiment: list[OptimizedCandidate] | None
+    experiment: Optional[list[OptimizedCandidate]]
 
 
 class OptimizedCandidateResult(BaseModel):
     times_run: int
     best_test_runtime: int
     best_test_results: TestResults
 
 
 class OriginalCodeBaseline(BaseModel):
     generated_test_results: TestResults
     existing_test_results: TestResults
-    overall_test_results: TestResults | None
+    overall_test_results: Optional[TestResults]
     runtime: int
 
 
 class GeneratedTests(BaseModel):
     generated_original_test_source: str
     instrumented_test_source: str
 
 
 class BestOptimization(BaseModel):
     candidate: OptimizedCandidate
-    dependent_functions: list[tuple[Source, str, str]]
+    helper_functions: list[tuple[Source, str, str]]
     runtime: int
     winning_test_results: TestResults
 
 
 class CodeOptimizationContext(BaseModel):
-    code_to_optimize_with_dependents: str
+    code_to_optimize_with_helpers: str
     contextual_dunder_methods: set[tuple[str, str]]
-    dependent_functions: list[tuple[Source, str, str]]
+    helper_functions: list[tuple[Source, str, str]]
     preexisting_functions: list[str]
 
 
 class Optimizer:
     def __init__(self, args: Namespace) -> None:
         self.args = args
         init_sentry(not args.disable_telemetry)
@@ -228,44 +228,44 @@
             function_to_optimize,
             self.args.project_root,
             original_code,
         )
         if not is_successful(ctx_result):
             return Failure(ctx_result.failure())
         code_context: CodeOptimizationContext = ctx_result.unwrap()
-        dependent_functions_by_module_abspath = defaultdict(set)
-        for _, module_abspath, qualified_name in code_context.dependent_functions:
-            dependent_functions_by_module_abspath[module_abspath].add(qualified_name)
-        original_dependent_code = {}
-        for module_abspath in dependent_functions_by_module_abspath:
+        helper_functions_by_module_abspath = defaultdict(set)
+        for _, module_abspath, qualified_name in code_context.helper_functions:
+            helper_functions_by_module_abspath[module_abspath].add(qualified_name)
+        original_helper_code = {}
+        for module_abspath in helper_functions_by_module_abspath:
             with pathlib.Path(module_abspath).open(encoding="utf8") as f:
-                dependent_code = f.read()
-                original_dependent_code[module_abspath] = dependent_code
-        logging.info(f"Code to be optimized:\n{code_context.code_to_optimize_with_dependents}")
+                helper_code = f.read()
+                original_helper_code[module_abspath] = helper_code
+        logging.info(f"Code to be optimized:\n{code_context.code_to_optimize_with_helpers}")
         module_path = module_name_from_file_path(function_to_optimize.file_path, self.args.project_root)
 
-        for module_abspath in original_dependent_code:
-            code_context.code_to_optimize_with_dependents = add_needed_imports_from_module(
-                original_dependent_code[module_abspath],
-                code_context.code_to_optimize_with_dependents,
+        for module_abspath in original_helper_code:
+            code_context.code_to_optimize_with_helpers = add_needed_imports_from_module(
+                original_helper_code[module_abspath],
+                code_context.code_to_optimize_with_helpers,
                 module_abspath,
                 function_to_optimize.file_path,
                 self.args.project_root,
             )
 
         instrumented_unittests_created_for_function = self.instrument_existing_tests(
             function_to_optimize=function_to_optimize,
             function_to_tests=function_to_tests,
         )
         self.instrumented_unittests_created.update(instrumented_unittests_created_for_function)
 
         generated_results = self.generate_tests_and_optimizations(
-            code_context.code_to_optimize_with_dependents,
+            code_context.code_to_optimize_with_helpers,
             function_to_optimize,
-            code_context.dependent_functions,
+            code_context.helper_functions,
             module_path,
             function_trace_id,
             run_experiment=should_run_experiment,
         )
         if not is_successful(generated_results):
             return Failure(generated_results.failure())
         tests_and_opts: tuple[GeneratedTests, OptimizationSet] = generated_results.unwrap()
@@ -273,14 +273,15 @@
         generated_tests_path = get_test_file_path(
             self.args.tests_root,
             function_to_optimize.function_name,
             0,
         )
         with pathlib.Path(generated_tests_path).open("w", encoding="utf8") as file:
             file.write(generated_tests.instrumented_test_source)
+        logging.info(f"Generated tests:\n{generated_tests.generated_original_test_source}")
         self.test_files_created.add(generated_tests_path)
         baseline_result = self.establish_original_code_baseline(
             function_to_optimize.qualified_name,
             instrumented_unittests_created_for_function,
             generated_tests_path,
             function_to_tests.get(module_path + "." + function_to_optimize.qualified_name, []),
         )
@@ -303,21 +304,21 @@
                 function_to_optimize.qualified_name_with_modules_from_root(self.args.project_root),
                 [],
             )
 
             best_optimization = self.determine_best_candidate(
                 candidates,
                 code_context,
-                dependent_functions_by_module_abspath,
+                helper_functions_by_module_abspath,
                 function_to_optimize,
                 generated_tests_path,
                 instrumented_unittests_created_for_function,
                 original_code,
                 original_code_baseline,
-                original_dependent_code,
+                original_helper_code,
                 function_trace_id[:-4] + f"EXP{u}" if should_run_experiment else function_trace_id,
                 tests_in_file,
             )
             ph("cli-optimize-function-finished", {"function_trace_id": function_trace_id})
 
             if best_optimization:
                 logging.info(
@@ -336,76 +337,76 @@
                 self.log_successful_optimization(
                     explanation,
                     function_to_optimize,
                     function_trace_id,
                     generated_tests,
                 )
 
-                self.replace_function_and_dependents_with_optimized_code(
+                self.replace_function_and_helpers_with_optimized_code(
                     code_context,
-                    dependent_functions_by_module_abspath,
+                    helper_functions_by_module_abspath,
                     explanation,
                     best_optimization.candidate.source_code,
                     function_to_optimize.qualified_name,
                 )
 
-                new_code, new_dependent_code = self.reformat_code_and_dependents(
-                    dependent_functions_by_module_abspath,
+                new_code, new_helper_code = self.reformat_code_and_helpers(
+                    helper_functions_by_module_abspath,
                     explanation.file_path,
                     original_code,
                 )
 
                 existing_tests = existing_tests_source_for(
                     function_to_optimize.qualified_name_with_modules_from_root(self.args.project_root),
                     function_to_tests,
                     tests_root=self.test_cfg.tests_root,
                 )
 
-                original_code_combined = original_dependent_code.copy()
+                original_code_combined = original_helper_code.copy()
                 original_code_combined[explanation.file_path] = original_code
-                new_code_combined = new_dependent_code.copy()
+                new_code_combined = new_helper_code.copy()
                 new_code_combined[explanation.file_path] = new_code
                 if not self.args.no_pr:
                     check_create_pr(
                         original_code=original_code_combined,
                         new_code=new_code_combined,
                         explanation=explanation,
                         existing_tests_source=existing_tests,
                         generated_original_test_source=generated_tests.generated_original_test_source,
                     )
                     if self.args.all or env_utils.get_pr_number():
                         # Reverting to original code, because optimizing functions in a sequence can lead to
                         #  a) Error propagation, where error in one function can cause the next optimization to fail
                         #  b) Performance estimates become unstable, as the runtime of an optimization might be
                         #     dependent on the runtime of the previous optimization
-                        self.write_code_and_dependents(
+                        self.write_code_and_helpers(
                             original_code,
-                            original_dependent_code,
+                            original_helper_code,
                             function_to_optimize.file_path,
-                            dependent_functions_by_module_abspath,
+                            helper_functions_by_module_abspath,
                         )
         # Delete all the generated tests to not cause any clutter.
         pathlib.Path(generated_tests_path).unlink(missing_ok=True)
         for test_paths in instrumented_unittests_created_for_function:
             pathlib.Path(test_paths).unlink(missing_ok=True)
         if not best_optimization:
             return Failure(f"No best optimizations found for function {function_to_optimize.qualified_name}")
         return Success(best_optimization)
 
     def determine_best_candidate(
         self,
         candidates: list[OptimizedCandidate],
         code_context: CodeOptimizationContext,
-        dependent_functions_by_module_abspath: dict[str, set[str]],
+        helper_functions_by_module_abspath: dict[str, set[str]],
         function_to_optimize: FunctionToOptimize,
         generated_tests_path: str,
         instrumented_unittests_created_for_function: set[str],
         original_code: str,
         original_code_baseline: OriginalCodeBaseline,
-        original_dependent_code: dict[str, str],
+        original_helper_code: dict[str, str],
         function_trace_id: str,
         only_run_this_test_function: list[TestsInFile] | None = None,
     ) -> BestOptimization | None:
         best_optimization: BestOptimization | None = None
         best_runtime_until_now = original_code_baseline.runtime  # The fastest code runtime until now
 
         speedup_ratios: dict[str, float | None] = {}
@@ -437,15 +438,15 @@
                     preexisting_functions=code_context.preexisting_functions,
                     contextual_functions=code_context.contextual_dunder_methods,
                     project_root_path=self.args.project_root,
                 )
                 for (
                     module_abspath,
                     qualified_names,
-                ) in dependent_functions_by_module_abspath.items():
+                ) in helper_functions_by_module_abspath.items():
                     replace_function_definitions_in_module(
                         function_names=list(qualified_names),
                         optimized_code=candidate.source_code,
                         file_path_of_module_with_function_to_optimize=function_to_optimize.file_path,
                         module_abspath=module_abspath,
                         preexisting_functions=[],
                         contextual_functions=code_context.contextual_dunder_methods,
@@ -454,19 +455,19 @@
             except (
                 ValueError,
                 SyntaxError,
                 cst.ParserSyntaxError,
                 AttributeError,
             ) as e:
                 logging.error(e)  # noqa: TRY400
-                self.write_code_and_dependents(
+                self.write_code_and_helpers(
                     original_code,
-                    original_dependent_code,
+                    original_helper_code,
                     function_to_optimize.file_path,
-                    dependent_functions_by_module_abspath,
+                    helper_functions_by_module_abspath,
                 )
                 continue
 
             # Run generated tests if at least one of them passed
             run_generated_tests = False
             if original_code_baseline.generated_test_results:
                 for test_result in original_code_baseline.generated_test_results.test_results:
@@ -514,24 +515,24 @@
                     logging.info(
                         f"Original runtime: {humanize_runtime(original_code_baseline.runtime)} Best test runtime: "
                         f"{humanize_runtime(best_test_runtime)}, ratio = "
                         f"{((original_code_baseline.runtime - best_test_runtime) / best_test_runtime)}",
                     )
                     best_optimization = BestOptimization(
                         candidate=candidate,
-                        dependent_functions=code_context.dependent_functions,
+                        helper_functions=code_context.helper_functions,
                         runtime=best_test_runtime,
                         winning_test_results=candidate_result.best_test_results,
                     )
                     best_runtime_until_now = best_test_runtime
-            self.write_code_and_dependents(
+            self.write_code_and_helpers(
                 original_code,
-                original_dependent_code,
+                original_helper_code,
                 function_to_optimize.file_path,
-                dependent_functions_by_module_abspath,
+                helper_functions_by_module_abspath,
             )
             logging.info("----------------")
         self.aiservice_client.log_results(
             function_trace_id=function_trace_id,
             speedup_ratio=speedup_ratios,
             original_runtime=original_code_baseline.runtime,
             optimized_runtime=optimized_runtimes,
@@ -566,58 +567,58 @@
                 "winning_test_results": {
                     tt.to_name(): v
                     for tt, v in explanation.winning_test_results.get_test_pass_fail_report_by_type().items()
                 },
             },
         )
 
-    def write_code_and_dependents(
+    def write_code_and_helpers(
         self,
         original_code: str,
-        original_dependent_code: dict[str, str],
+        original_helper_code: dict[str, str],
         path: str,
-        dependent_functions_by_module_abspath: dict[str, set[str]],
+        helper_functions_by_module_abspath: dict[str, set[str]],
     ) -> None:
         with pathlib.Path(path).open("w", encoding="utf8") as f:
             f.write(original_code)
-        for module_abspath in dependent_functions_by_module_abspath:
+        for module_abspath in helper_functions_by_module_abspath:
             with pathlib.Path(module_abspath).open("w", encoding="utf8") as f:
-                f.write(original_dependent_code[module_abspath])
+                f.write(original_helper_code[module_abspath])
 
-    def reformat_code_and_dependents(
+    def reformat_code_and_helpers(
         self,
-        dependent_functions_by_module_abspath: dict[str, set[str]],
+        helper_functions_by_module_abspath: dict[str, set[str]],
         path: str,
         original_code: str,
     ) -> tuple[str, dict[str, str]]:
         should_sort_imports = True
         if isort.code(original_code) != original_code:
             should_sort_imports = False
 
         new_code = format_code(
             self.args.formatter_cmd,
             self.args.imports_sort_cmd,
             should_sort_imports,
             path,
         )
-        new_dependent_code: dict[str, str] = {
+        new_helper_code: dict[str, str] = {
             module_abspath: format_code(
                 self.args.formatter_cmd,
                 self.args.imports_sort_cmd,
                 should_sort_imports,
                 module_abspath,
             )
-            for module_abspath in dependent_functions_by_module_abspath
+            for module_abspath in helper_functions_by_module_abspath
         }
-        return new_code, new_dependent_code
+        return new_code, new_helper_code
 
-    def replace_function_and_dependents_with_optimized_code(
+    def replace_function_and_helpers_with_optimized_code(
         self,
         code_context: CodeOptimizationContext,
-        dependent_functions_by_module_abspath: dict[str, set[str]],
+        helper_functions_by_module_abspath: dict[str, set[str]],
         explanation: Explanation,
         optimized_code: str,
         qualified_function_name: str,
     ) -> None:
         replace_function_definitions_in_module(
             function_names=[qualified_function_name],
             optimized_code=optimized_code,
@@ -626,15 +627,15 @@
             preexisting_functions=code_context.preexisting_functions,
             contextual_functions=code_context.contextual_dunder_methods,
             project_root_path=self.args.project_root,
         )
         for (
             module_abspath,
             qualified_names,
-        ) in dependent_functions_by_module_abspath.items():
+        ) in helper_functions_by_module_abspath.items():
             replace_function_definitions_in_module(
                 function_names=list(qualified_names),
                 optimized_code=optimized_code,
                 file_path_of_module_with_function_to_optimize=explanation.file_path,
                 module_abspath=module_abspath,
                 preexisting_functions=[],
                 contextual_functions=code_context.contextual_dunder_methods,
@@ -652,61 +653,61 @@
         )
         if code_to_optimize is None:
             return Failure("Could not find function to optimize.")
         success, preexisting_functions = get_all_function_names(code_to_optimize)
         if not success:
             return Failure("Error in parsing the code, skipping optimization.")
         (
-            dependent_code,
-            dependent_functions,
-        ) = get_constrained_function_context_and_dependent_functions(
+            helper_code,
+            helper_functions,
+        ) = get_constrained_function_context_and_helper_functions(
             function_to_optimize,
             self.args.project_root,
             code_to_optimize,
         )
         if function_to_optimize.parents:
             function_class = function_to_optimize.parents[0].name
-            dependent_methods = [
+            helper_methods = [
                 df
-                for df in dependent_functions
+                for df in helper_functions
                 if df[2].count(".") > 0 and df[2].split(".")[0] == function_class
             ]
             optimizable_methods = [function_to_optimize] + [
                 FunctionToOptimize(
-                    df[2].split(".")[0],
+                    df[2].split(".")[-1],
                     "",
                     [FunctionParent(df[2].split(".")[0], "ClassDef")],
                     None,
                     None,
                 )
-                for df in dependent_methods
+                for df in helper_methods
             ]
             if len(optimizable_methods) > 1:
                 code_to_optimize, contextual_dunder_methods = extract_code(
                     optimizable_methods,
                 )
                 if code_to_optimize is None:
                     return Failure("Could not find function to optimize.")
-        code_to_optimize_with_dependents = dependent_code + "\n" + code_to_optimize
+        code_to_optimize_with_helpers = helper_code + "\n" + code_to_optimize
 
-        code_to_optimize_with_dependents_and_imports = add_needed_imports_from_module(
+        code_to_optimize_with_helpers_and_imports = add_needed_imports_from_module(
             original_source_code,
-            code_to_optimize_with_dependents,
+            code_to_optimize_with_helpers,
             function_to_optimize.file_path,
             function_to_optimize.file_path,
             project_root,
         )
         preexisting_functions.extend(
-            [fn[0].full_name.split(".")[-1] for fn in dependent_functions],
+            [fn[0].full_name.split(".")[-1] for fn in helper_functions],
         )
         return Success(
             CodeOptimizationContext(
-                code_to_optimize_with_dependents=code_to_optimize_with_dependents_and_imports,
+                code_to_optimize_with_helpers=code_to_optimize_with_helpers_and_imports,
                 contextual_dunder_methods=contextual_dunder_methods,
-                dependent_functions=dependent_functions,
+                helper_functions=helper_functions,
                 preexisting_functions=preexisting_functions,
             ),
         )
 
     def cleanup_leftover_test_return_values(self) -> None:
         # remove leftovers from previous run
         pathlib.Path(get_run_tmp_file("test_return_values_0.bin")).unlink(
@@ -753,44 +754,44 @@
                 f"Discovered {relevant_test_files_count} existing unit test file"
                 f"{'s' if relevant_test_files_count != 1 else ''} for {func_qualname}",
             )
         return unique_instrumented_test_files
 
     def generate_tests_and_optimizations(
         self,
-        code_to_optimize_with_dependents: str,
+        code_to_optimize_with_helpers: str,
         function_to_optimize: FunctionToOptimize,
-        dependent_functions: list[tuple[Source, str, str]],
+        helper_functions: list[tuple[Source, str, str]],
         module_path: str,
         function_trace_id: str,
         run_experiment: bool = False,
     ) -> Result[tuple[GeneratedTests, OptimizationSet], str]:
         generated_original_test_source = None
         instrumented_test_source = None
         max_workers = 2 if not run_experiment else 3
         with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
             future_tests = executor.submit(
                 self.generate_and_instrument_tests,
-                code_to_optimize_with_dependents,
+                code_to_optimize_with_helpers,
                 function_to_optimize,
-                [definition[0].full_name for definition in dependent_functions],
+                [definition[0].full_name for definition in helper_functions],
                 module_path,
                 function_trace_id[:-4] + "EXP0" if run_experiment else function_trace_id,
             )
             future_optimization_candidates = executor.submit(
                 self.aiservice_client.optimize_python_code,
-                code_to_optimize_with_dependents,
+                code_to_optimize_with_helpers,
                 function_trace_id[:-4] + "EXP0" if run_experiment else function_trace_id,
                 N_CANDIDATES,
                 ExperimentMetadata(id=self.experiment_id, group="control") if run_experiment else None,
             )
             if run_experiment:
                 future_candidates_exp = executor.submit(
                     self.local_aiservice_client.optimize_python_code,
-                    code_to_optimize_with_dependents,
+                    code_to_optimize_with_helpers,
                     function_trace_id[:-4] + "EXP1",
                     N_CANDIDATES,
                     ExperimentMetadata(id=self.experiment_id, group="experiment"),
                 )
 
             future_tests_result = future_tests.result()
             candidates: list[OptimizedCandidate] = future_optimization_candidates.result()
@@ -848,15 +849,15 @@
         else:
             test_env["PYTHONPATH"] += os.pathsep + self.args.project_root
         cumulative_test_runtime = 0
         cumulative_test_runs = 0
         first_run = True
         do_break = False
         logging.info(
-            f"Running {len(instrumented_unittests_created_for_function)} tests for {function_name} ..."
+            f"Running {len(instrumented_unittests_created_for_function)} tests for {function_name} ...",
         )
         while (
             cumulative_test_runtime < MAX_CUMULATIVE_TEST_RUNTIME_NANOSECONDS
             and cumulative_test_runs < MAX_TEST_FUNCTION_RUNS
         ):
             for i in range(MAX_TEST_RUN_ITERATIONS):
                 if generated_tests_elapsed_time > MAX_FUNCTION_TEST_SECONDS:
@@ -1176,23 +1177,23 @@
         )
         return unittest_results
 
     def generate_and_instrument_tests(
         self,
         source_code_being_tested: str,
         function_to_optimize: FunctionToOptimize,
-        dependent_function_names: list[str],
+        helper_function_names: list[str],
         module_path: str,
         function_trace_id: str,
     ) -> Union[Tuple[str, str], None]:
         tests = generate_tests(
             self.aiservice_client,
             source_code_being_tested=source_code_being_tested,
             function_to_optimize=function_to_optimize,
-            dependent_function_names=dependent_function_names,
+            helper_function_names=helper_function_names,
             module_path=module_path,
             test_cfg=self.test_cfg,
             test_timeout=INDIVIDUAL_TEST_TIMEOUT,
             use_cached_tests=self.args.use_cached_tests,
             function_trace_id=function_trace_id,
         )
         if tests is None:
```

### Comparing `codeflash-0.6.2/codeflash/result/create_pr.py` & `codeflash-0.6.3/codeflash/result/create_pr.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/result/explanation.py` & `codeflash-0.6.3/codeflash/result/explanation.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/telemetry/posthog.py` & `codeflash-0.6.3/codeflash/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/telemetry/sentry.py` & `codeflash-0.6.3/codeflash/telemetry/sentry.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/tracer.py` & `codeflash-0.6.3/codeflash/tracer.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/tracing/profile_stats.py` & `codeflash-0.6.3/codeflash/tracing/profile_stats.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/tracing/replay_test.py` & `codeflash-0.6.3/codeflash/tracing/replay_test.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/update_license_version.py` & `codeflash-0.6.3/codeflash/update_license_version.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/verification/comparator.py` & `codeflash-0.6.3/codeflash/verification/comparator.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/verification/equivalence.py` & `codeflash-0.6.3/codeflash/verification/equivalence.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/verification/parse_test_output.py` & `codeflash-0.6.3/codeflash/verification/parse_test_output.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/verification/test_results.py` & `codeflash-0.6.3/codeflash/verification/test_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     def get_test_pass_fail_report(self) -> str:
         passed = 0
         failed = 0
         for test_result in self.test_results:
             if test_result.did_pass:
                 passed += 1
             else:
+                logging.info(f"Failed test: {test_result.id}")
                 failed += 1
         return f"Passed: {passed}, Failed: {failed}"
 
     def get_test_pass_fail_report_by_type(self) -> dict[TestType, dict[str, int]]:
         report = {}
         for test_type in TestType:
             report[test_type] = {"passed": 0, "failed": 0}
```

### Comparing `codeflash-0.6.2/codeflash/verification/test_runner.py` & `codeflash-0.6.3/codeflash/verification/test_runner.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/verification/verification_utils.py` & `codeflash-0.6.3/codeflash/verification/verification_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.2/codeflash/verification/verifier.py` & `codeflash-0.6.3/codeflash/verification/verifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 )
 
 
 def generate_tests(
     aiservice_client: AiServiceClient,
     source_code_being_tested: str,
     function_to_optimize: FunctionToOptimize,
-    dependent_function_names: list[str],
+    helper_function_names: list[str],
     module_path: str,
     test_cfg: TestConfig,
     test_timeout: int,
     use_cached_tests: bool,
     function_trace_id: str,
 ) -> Optional[Tuple[str, str]]:
     # TODO: Sometimes this recreates the original Class definition. This overrides and messes up the original
@@ -43,15 +43,15 @@
         test_module_path = module_name_from_file_path(
             get_test_file_path(test_cfg.tests_root, function_to_optimize.function_name, 0),
             test_cfg.project_root_path,
         )
         response = aiservice_client.generate_regression_tests(
             source_code_being_tested=source_code_being_tested,
             function_to_optimize=function_to_optimize,
-            dependent_function_names=dependent_function_names,
+            helper_function_names=helper_function_names,
             module_path=module_path,
             test_module_path=test_module_path,
             test_framework=test_cfg.test_framework,
             test_timeout=test_timeout,
             trace_id=function_trace_id,
         )
         if response and isinstance(response, tuple) and len(response) == 2:
```

### Comparing `codeflash-0.6.2/pyproject.toml` & `codeflash-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "codeflash"
-version = "0.6.2" # Determined by poetry-dynamic-versioning during `poetry build`
+version = "0.6.3" # Determined by poetry-dynamic-versioning during `poetry build`
 description = "Client for codeflash.ai - automatic code performance optimization, powered by AI"
 license = "BSL-1.1"
 authors = ["CodeFlash Inc. <contact@codeflash.ai>"]
 homepage = "https://codeflash.ai"
 readme = "README.md"
 packages = [
     { include = "codeflash" },
```

### Comparing `codeflash-0.6.2/PKG-INFO` & `codeflash-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeflash
-Version: 0.6.2
+Version: 0.6.3
 Summary: Client for codeflash.ai - automatic code performance optimization, powered by AI
 Home-page: https://codeflash.ai
 License: BSL-1.1
 Keywords: codeflash,performance,optimization,ai,code,machine learning,LLM
 Author: CodeFlash Inc.
 Author-email: contact@codeflash.ai
 Requires-Python: >=3.9,<4.0
```

