# Comparing `tmp/exponent_run-0.0.3.tar.gz` & `tmp/exponent_run-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exponent_run-0.0.3.tar", max compression
+gzip compressed data, was "exponent_run-0.0.4.tar", max compression
```

## Comparing `exponent_run-0.0.3.tar` & `exponent_run-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,18 @@
--rw-r--r--   0        0        0       57 2024-05-03 23:47:20.021413 exponent_run-0.0.3/exponent/__init__.py
--rw-r--r--   0        0        0     5040 2024-05-09 19:22:41.007830 exponent_run-0.0.3/exponent/cli.py
--rw-r--r--   0        0        0     1403 2024-05-07 07:10:08.943140 exponent_run-0.0.3/exponent/core/config.py
--rw-r--r--   0        0        0     7194 2024-05-09 03:32:46.489461 exponent_run-0.0.3/exponent/core/remote_execution/client.py
--rw-r--r--   0        0        0     1994 2024-05-09 00:30:27.349939 exponent_run-0.0.3/exponent/core/remote_execution/kernel.py
--rw-r--r--   0        0        0     5414 2024-05-09 00:30:27.350382 exponent_run-0.0.3/exponent/core/remote_execution/types.py
--rw-r--r--   0        0        0        0 2024-05-03 23:47:19.960349 exponent_run-0.0.3/exponent/tests/__init__.py
--rw-r--r--   0        0        0     1309 2024-05-09 03:32:46.489873 exponent_run-0.0.3/exponent/tests/conftest.py
--rw-r--r--   0        0        0     7764 2024-05-09 03:32:46.490229 exponent_run-0.0.3/exponent/tests/test_cli.py
--rw-r--r--   0        0        0     1518 2024-05-09 19:22:57.019385 exponent_run-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 exponent_run-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       57 2024-05-03 23:47:20.021413 exponent_run-0.0.4/exponent/__init__.py
+-rw-r--r--   0        0        0     7325 2024-05-18 22:21:15.560183 exponent_run-0.0.4/exponent/cli.py
+-rw-r--r--   0        0        0     1727 2024-05-14 23:30:22.001306 exponent_run-0.0.4/exponent/core/config.py
+-rw-r--r--   0        0        0     5548 2024-05-19 02:03:41.245790 exponent_run-0.0.4/exponent/core/remote_execution/client.py
+-rw-r--r--   0        0        0     1508 2024-05-19 02:03:41.246067 exponent_run-0.0.4/exponent/core/remote_execution/code_execution.py
+-rw-r--r--   0        0        0     3440 2024-05-17 09:30:56.979279 exponent_run-0.0.4/exponent/core/remote_execution/files.py
+-rw-r--r--   0        0        0     1254 2024-05-17 07:50:43.085085 exponent_run-0.0.4/exponent/core/remote_execution/languages/diff.py
+-rw-r--r--   0        0        0     4428 2024-05-15 21:47:37.236001 exponent_run-0.0.4/exponent/core/remote_execution/languages/python.py
+-rw-r--r--   0        0        0      555 2024-05-18 00:30:25.944494 exponent_run-0.0.4/exponent/core/remote_execution/languages/shell.py
+-rw-r--r--   0        0        0      578 2024-05-15 21:47:37.236935 exponent_run-0.0.4/exponent/core/remote_execution/session.py
+-rw-r--r--   0        0        0      952 2024-05-15 21:47:37.238191 exponent_run-0.0.4/exponent/core/remote_execution/system_context.py
+-rw-r--r--   0        0        0     4574 2024-05-19 02:03:41.246350 exponent_run-0.0.4/exponent/core/remote_execution/types.py
+-rw-r--r--   0        0        0     8685 2024-05-19 02:03:41.246483 exponent_run-0.0.4/exponent/core/remote_execution/utils.py
+-rw-r--r--   0        0        0        0 2024-05-03 23:47:19.960349 exponent_run-0.0.4/exponent/tests/__init__.py
+-rw-r--r--   0        0        0     1719 2024-05-14 18:25:03.436018 exponent_run-0.0.4/exponent/tests/conftest.py
+-rw-r--r--   0        0        0    11284 2024-05-17 09:35:45.870376 exponent_run-0.0.4/exponent/tests/test_cli.py
+-rw-r--r--   0        0        0     1563 2024-05-20 23:52:54.688326 exponent_run-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 exponent_run-0.0.4/PKG-INFO
```

### Comparing `exponent_run-0.0.3/exponent/core/config.py` & `exponent_run-0.0.4/exponent/core/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 import json
+import logging
 import os
 from functools import lru_cache
-from importlib.metadata import Distribution
+from importlib.metadata import Distribution, PackageNotFoundError
 
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
+logger = logging.getLogger(__name__)
+
 # If the package is editable, we want to use:
 # base_url = localhost:3000
 # base_api_url = localhost:8000
 
 
 def is_editable_install() -> bool:
     if os.getenv("ENVIRONMENT") == "test":
         # We should explicitly set these variables
         # in test when needed
         return False
 
     try:
-        direct_url = Distribution.from_name("exponent-run").read_text("direct_url.json")
-        if not direct_url:
-            return False
-        pkg_is_editable = (
-            json.loads(direct_url).get("dir_info", {}).get("editable", False)
-        )
-        return bool(pkg_is_editable)
-    except Exception as e:
-        print(e)
+        dist = Distribution.from_name("exponent-run")
+    except PackageNotFoundError:
+        logger.info("No distribution info found for exponent-run")
+        return False
+
+    direct_url = dist.read_text("direct_url.json")
+    if not direct_url:
         return False
 
+    try:
+        direct_url_json = json.loads(direct_url)
+    except json.JSONDecodeError:
+        logger.warning("Failed to decode distribution info for exponent-run")
+        return False
+
+    pkg_is_editable = direct_url_json.get("dir_info", {}).get("editable", False)
+    return bool(pkg_is_editable)
+
 
 class Settings(BaseSettings):
     base_url: str = "https://exponent.run"
     base_api_url: str = "https://api.exponent.run"
     api_key: str | None = None
+    log_level: str = "WARNING"
 
     model_config = SettingsConfigDict(
         env_prefix="EXPONENT_",
         env_file=os.path.expanduser("~/.exponent"),
         case_sensitive=False,
     )
```

### Comparing `exponent_run-0.0.3/exponent/tests/conftest.py` & `exponent_run-0.0.4/exponent/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import os
 import tempfile
 from collections.abc import Generator
+from unittest.mock import patch
 
 import pytest
 from click.testing import CliRunner
 
 
 @pytest.fixture(scope="session")
 def event_loop() -> Generator[asyncio.AbstractEventLoop, None, None]:
@@ -38,8 +39,21 @@
 def default_temporary_directory(temporary_directory: str) -> Generator[str, None, None]:
     with open(os.path.join(temporary_directory, "test1.py"), "w") as f:
         f.write("print('Hello, world!')")
 
     with open(os.path.join(temporary_directory, "test2.py"), "w") as f:
         f.write("print('Hello, world!')")
 
+    with open(os.path.join(temporary_directory, "exponent.txt"), "w") as f:
+        f.write("Hello, world!")
+
     yield temporary_directory
+
+
+@pytest.fixture(scope="function", autouse=True)
+def mock_cli_heartbeat() -> Generator[None, None, None]:
+    patcher = patch(
+        "exponent.core.remote_execution.client.RemoteExecutionClient.send_heartbeat"
+    )
+    patcher.start()
+    yield
+    patcher.stop()
```

### Comparing `exponent_run-0.0.3/pyproject.toml` & `exponent_run-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 authors = ["Sashank Thupukari <sashank@exponent.run>"]
 description = "Exponent is an AI Pair Programmer"
 name = "exponent-run"
-version = "0.0.3"
+version = "0.0.4"
 packages = [{ include = "exponent" }]
 
 [tool.poetry.scripts]
 exponent = "exponent.cli:cli"
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.11,<3.13"
+
 
 pydantic = { extras = ["dotenv", "email"], version = "^2.6.4" }
 pydantic-settings = "^2.2.1"
 pytest-env = "^1.1.3"
 click = "^8.1.7"
 httpx = "^0.27.0"
 rapidfuzz = "^3.9.0"
@@ -39,17 +40,17 @@
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.ruff]
 target-version = "py312"
 
 [tool.ruff.lint]
-# pycodestyle, pyflakes, isort, pylint, pyupgrade
+# pycodestyle, pyflakes, isort, pylint, pyupgrade, ruff, blind-exceptions
 ignore = ["E501"]
-select = ["E", "F", "I", "PL", "UP", "W"]
+select = ["E", "F", "I", "PL", "UP", "W", "RUF", "BLE"]
 
 [tool.ruff.lint.isort]
 # Combine multiple `from foo import bar as baz` statements with the same source
 # (`foo`) into a single statement.
 combine-as-imports = true
 # Imports of the form `from foo import bar as baz` show one `import bar as baz`
 # per line. Useful for __init__.py files that just re-export symbols.
```

### Comparing `exponent_run-0.0.3/PKG-INFO` & `exponent_run-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: exponent-run
-Version: 0.0.3
+Version: 0.0.4
 Summary: Exponent is an AI Pair Programmer
 Author: Sashank Thupukari
 Author-email: sashank@exponent.run
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.11,<3.13
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: gitignore-parser (>=0.1.11,<0.2.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: ipykernel (>=6.29.4,<7.0.0)
 Requires-Dist: jupyter-client (>=8.6.1,<9.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
```

