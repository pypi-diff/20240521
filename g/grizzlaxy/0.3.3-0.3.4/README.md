# Comparing `tmp/grizzlaxy-0.3.3.tar.gz` & `tmp/grizzlaxy-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grizzlaxy-0.3.3.tar", max compression
+gzip compressed data, was "grizzlaxy-0.3.4.tar", max compression
```

## Comparing `grizzlaxy-0.3.3.tar` & `grizzlaxy-0.3.4.tar`

### file list

```diff
@@ -1,15 +1,20 @@
--rw-r--r--   0        0        0     1061 2023-06-22 00:33:43.206354 grizzlaxy-0.3.3/LICENSE
--rw-r--r--   0        0        0      151 2023-06-26 19:43:56.507337 grizzlaxy-0.3.3/README.md
--rw-r--r--   0        0        0      173 2024-04-04 18:13:23.644673 grizzlaxy-0.3.3/grizzlaxy/__init__.py
--rw-r--r--   0        0        0     4502 2024-01-31 22:21:34.053999 grizzlaxy-0.3.3/grizzlaxy/auth.py
--rw-r--r--   0        0        0     9556 2024-03-22 19:31:59.186558 grizzlaxy-0.3.3/grizzlaxy/cli.py
--rw-r--r--   0        0        0        0 2024-03-22 19:57:27.525049 grizzlaxy-0.3.3/grizzlaxy/components/__init__.py
--rw-r--r--   0        0        0     2442 2024-04-04 18:12:51.851820 grizzlaxy-0.3.3/grizzlaxy/find.py
--rw-r--r--   0        0        0      367 2023-09-26 04:06:50.584404 grizzlaxy-0.3.3/grizzlaxy/index-style.css
--rw-r--r--   0        0        0      256 2024-01-30 01:40:07.085191 grizzlaxy-0.3.3/grizzlaxy/index-template.html
--rw-r--r--   0        0        0     1684 2023-12-09 00:51:54.291186 grizzlaxy-0.3.3/grizzlaxy/index.py
--rw-r--r--   0        0        0     4099 2024-01-31 22:33:51.017006 grizzlaxy-0.3.3/grizzlaxy/reload.py
--rw-r--r--   0        0        0     4219 2024-04-04 18:50:31.118862 grizzlaxy-0.3.3/grizzlaxy/utils.py
--rw-r--r--   0        0        0       18 2024-04-04 18:52:36.365225 grizzlaxy-0.3.3/grizzlaxy/version.py
--rw-r--r--   0        0        0      856 2024-04-04 18:52:36.343436 grizzlaxy-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 grizzlaxy-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-22 00:33:43.206354 grizzlaxy-0.3.4/LICENSE
+-rw-r--r--   0        0        0      151 2023-06-26 19:43:56.507337 grizzlaxy-0.3.4/README.md
+-rw-r--r--   0        0        0      173 2024-04-04 18:13:23.644673 grizzlaxy-0.3.4/grizzlaxy/__init__.py
+-rw-r--r--   0        0        0     4502 2024-01-31 22:21:34.053999 grizzlaxy-0.3.4/grizzlaxy/auth.py
+-rw-r--r--   0        0        0     8242 2024-05-07 04:51:08.087921 grizzlaxy-0.3.4/grizzlaxy/cli.py
+-rw-r--r--   0        0        0       49 2024-05-18 22:22:59.215967 grizzlaxy-0.3.4/grizzlaxy/components/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 22:21:58.304934 grizzlaxy-0.3.4/grizzlaxy/components/editor.css
+-rw-r--r--   0        0        0     2664 2024-05-18 22:32:04.934491 grizzlaxy-0.3.4/grizzlaxy/components/editor.js
+-rw-r--r--   0        0        0     2410 2024-05-18 22:18:56.098591 grizzlaxy-0.3.4/grizzlaxy/components/editor.py
+-rw-r--r--   0        0        0     1589 2024-05-07 04:51:08.088187 grizzlaxy-0.3.4/grizzlaxy/config.py
+-rw-r--r--   0        0        0     2442 2024-04-04 18:12:51.851820 grizzlaxy-0.3.4/grizzlaxy/find.py
+-rw-r--r--   0        0        0      367 2023-09-26 04:06:50.584404 grizzlaxy-0.3.4/grizzlaxy/index-style.css
+-rw-r--r--   0        0        0      256 2024-01-30 01:40:07.085191 grizzlaxy-0.3.4/grizzlaxy/index-template.html
+-rw-r--r--   0        0        0     1684 2023-12-09 00:51:54.291186 grizzlaxy-0.3.4/grizzlaxy/index.py
+-rw-r--r--   0        0        0     4099 2024-01-31 22:33:51.017006 grizzlaxy-0.3.4/grizzlaxy/reload.py
+-rw-r--r--   0        0        0     2732 2024-04-17 05:39:52.714802 grizzlaxy-0.3.4/grizzlaxy/serialization.py
+-rw-r--r--   0        0        0     4219 2024-04-04 18:50:31.118862 grizzlaxy-0.3.4/grizzlaxy/utils.py
+-rw-r--r--   0        0        0       18 2024-05-21 18:03:16.174974 grizzlaxy-0.3.4/grizzlaxy/version.py
+-rw-r--r--   0        0        0      853 2024-05-21 18:03:16.150618 grizzlaxy-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 grizzlaxy-0.3.4/PKG-INFO
```

### Comparing `grizzlaxy-0.3.3/LICENSE` & `grizzlaxy-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `grizzlaxy-0.3.3/grizzlaxy/auth.py` & `grizzlaxy-0.3.4/grizzlaxy/auth.py`

 * *Files identical despite different names*

### Comparing `grizzlaxy-0.3.3/grizzlaxy/cli.py` & `grizzlaxy-0.3.4/grizzlaxy/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import argparse
 import importlib
 import json
 import sys
-from dataclasses import dataclass, field
 from pathlib import Path
 from textwrap import dedent
 from types import SimpleNamespace
 from uuid import uuid4
 
 import gifnoc
 import uvicorn
@@ -16,77 +15,20 @@
 from starbear.serve import debug_mode, dev_injections
 from starlette.applications import Starlette
 from starlette.config import Config
 from starlette.middleware.httpsredirect import HTTPSRedirectMiddleware
 from starlette.middleware.sessions import SessionMiddleware
 
 from .auth import OAuthMiddleware, PermissionDict, PermissionFile
+from .config import config as gzconfig
 from .find import collect_routes, collect_routes_from_module, compile_routes
 from .reload import FullReloader, InertReloader, JuriggedReloader
 from .utils import UsageError
 
 
-@dataclass
-class GrizzlaxySSLConfig:
-    # Whether SSL is enabled
-    enabled: bool = False
-    # SSL key file
-    keyfile: Path = None
-    # SSL certificate file
-    certfile: Path = None
-
-
-@dataclass
-class GrizzlaxyOAuthConfig:
-    # Whether OAuth is enabled
-    enabled: bool = False
-    # Permissions file
-    permissions: Path = None
-    default_permissions: dict = None
-    name: str = None
-    server_metadata_url: str = None
-    client_kwargs: dict = field(default_factory=dict)
-    environ: dict = field(default_factory=dict)
-
-
-@dataclass
-class GrizzlaxySentryConfig:
-    # Whether Sentry is enabled
-    enabled: bool = False
-    dsn: str = None
-    traces_sample_rate: float = None
-    environment: str = None
-    log_level: str = None
-    event_log_level: str = None
-
-
-@dataclass
-class GrizzlaxyConfig:
-    # Directory or script
-    root: str = None
-    # Name of the module to run
-    module: str = None
-    # Port to serve from
-    port: int = 8000
-    # Hostname to serve from
-    host: str = "127.0.0.1"
-    # Path to watch for changes with jurigged
-    watch: str | bool = None
-    # Run in development mode
-    dev: bool = False
-    # Reloading methodology
-    reload_mode: str = "jurigged"
-    ssl: GrizzlaxySSLConfig = field(default_factory=GrizzlaxySSLConfig)
-    oauth: GrizzlaxyOAuthConfig = field(default_factory=GrizzlaxyOAuthConfig)
-    sentry: GrizzlaxySentryConfig = field(default_factory=GrizzlaxySentryConfig)
-
-
-gzconfig = gifnoc.define(field="grizzlaxy", model=GrizzlaxyConfig)
-
-
 class Grizzlaxy:
     def __init__(self, config):
         root = config.root
         module = config.module
         port = config.port
         host = config.host
         ssl = config.ssl
@@ -224,16 +166,16 @@
 
             sentry_sdk.init(
                 dsn=self.sentry.dsn,
                 traces_sample_rate=self.sentry.traces_sample_rate,
                 environment=self.sentry.environment,
                 integrations=[
                     LoggingIntegration(
-                        level=_get_level(self.sentry.log_level or ""),
-                        event_level=_get_level(self.sentry.event_log_level or ""),
+                        level=_get_level(self.sentry.log_level or "ERROR"),
+                        event_level=_get_level(self.sentry.event_log_level or "ERROR"),
                     )
                 ],
             )
 
         app.grizzlaxy = SimpleNamespace(
             permissions=permissions,
         )
@@ -244,18 +186,23 @@
     def set_routes(self):
         if self.root:
             collected = collect_routes(self.root)
         elif self.module:
             collected = collect_routes_from_module(self.module)
 
         routes = compile_routes("/", collected)
-
         self.reloader.inject_routes(routes)
 
-        self.app.router.routes = routes
+        for route in routes:
+            route._grizzlaxy_managed = True
+
+        remainder = [
+            r for r in self.app.router.routes if not getattr(r, "_grizzlaxy_managed", False)
+        ]
+        self.app.router.routes = routes + remainder
         self.app.map = collected
 
     def run(self):
         token = debug_mode.set(self.dev)
         try:
             uvicorn.run(
                 self.app,
@@ -274,17 +221,15 @@
         config = GrizzlaxyConfig(**kwargs)
     gz = Grizzlaxy(config)
     gz.run()
 
 
 def main(argv=None):
     with gifnoc.cli(
-        argparser=argparse.ArgumentParser(
-            description="Start a grizzlaxy of starbears."
-        ),
+        argparser=argparse.ArgumentParser(description="Start a grizzlaxy of starbears."),
         options=Command(
             mount="grizzlaxy",
             options={
                 ".root": "--root",
                 ".module": Option(aliases=["-m"]),
                 ".port": Option(aliases=["-p"]),
                 ".host": "--host",
```

### Comparing `grizzlaxy-0.3.3/grizzlaxy/find.py` & `grizzlaxy-0.3.4/grizzlaxy/find.py`

 * *Files identical despite different names*

### Comparing `grizzlaxy-0.3.3/grizzlaxy/index.py` & `grizzlaxy-0.3.4/grizzlaxy/index.py`

 * *Files identical despite different names*

### Comparing `grizzlaxy-0.3.3/grizzlaxy/reload.py` & `grizzlaxy-0.3.4/grizzlaxy/reload.py`

 * *Files identical despite different names*

### Comparing `grizzlaxy-0.3.3/grizzlaxy/utils.py` & `grizzlaxy-0.3.4/grizzlaxy/utils.py`

 * *Files identical despite different names*

### Comparing `grizzlaxy-0.3.3/pyproject.toml` & `grizzlaxy-0.3.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grizzlaxy"
-version = "0.3.3"
+version = "0.3.4"
 description = "Create an app from a galaxy of starbears"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -16,24 +16,25 @@
 jurigged = "^0.5.5"
 pyyaml = {version = "^6.0.1", optional = true}
 sentry-sdk = {extras = ["starlette"], version = "^1.35.0", optional = true}
 sse-starlette = "^1.8.2"
 gifnoc = "^0.3.0"
 
 [tool.poetry.group.dev.dependencies]
-black = ">=23.3.0"
-ruff = "^0.0.274"
+ruff = "^0.3.7"
 
 [tool.poetry.extras]
 yaml = ["pyyaml"]
 sentry = ["sentry-sdk"]
 
 [tool.poetry.scripts]
 grizzlaxy = "grizzlaxy.cli:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 99
+
+[tool.ruff.lint]
 extend-select = ["I"]
```

### Comparing `grizzlaxy-0.3.3/PKG-INFO` & `grizzlaxy-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzlaxy
-Version: 0.3.3
+Version: 0.3.4
 Summary: Create an app from a galaxy of starbears
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

