# Comparing `tmp/tailucas_pylib-0.4.0.tar.gz` & `tmp/tailucas_pylib-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailucas_pylib-0.4.0.tar", max compression
+gzip compressed data, was "tailucas_pylib-0.4.1.tar", max compression
```

## Comparing `tailucas_pylib-0.4.0.tar` & `tailucas_pylib-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.4.0/LICENSE
--rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.4.0/README.md
--rw-r--r--   0        0        0      557 2024-05-01 09:18:41.667566 tailucas_pylib-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6313 2024-05-01 09:18:41.667566 tailucas_pylib-0.4.0/tailucas_pylib/__init__.py
--rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.4.0/tailucas_pylib/app.py
--rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.4.0/tailucas_pylib/aws/__init__.py
--rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.4.0/tailucas_pylib/aws/metrics.py
--rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.4.0/tailucas_pylib/aws/swf.py
--rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.4.0/tailucas_pylib/bluetooth.py
--rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.4.0/tailucas_pylib/data.py
--rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.4.0/tailucas_pylib/datetime.py
--rw-r--r--   0        0        0     1503 2024-05-01 06:59:19.767564 tailucas_pylib-0.4.0/tailucas_pylib/device.py
--rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.4.0/tailucas_pylib/handler.py
--rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.4.0/tailucas_pylib/process.py
--rw-r--r--   0        0        0     9984 2024-04-30 08:38:32.802013 tailucas_pylib-0.4.0/tailucas_pylib/rabbit.py
--rw-r--r--   0        0        0     5398 2024-04-28 08:25:39.491596 tailucas_pylib-0.4.0/tailucas_pylib/threads.py
--rw-r--r--   0        0        0     3387 2024-04-30 05:12:18.922012 tailucas_pylib-0.4.0/tailucas_pylib/zmq.py
--rw-r--r--   0        0        0    12330 1970-01-01 00:00:00.000000 tailucas_pylib-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.4.1/LICENSE
+-rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.4.1/README.md
+-rw-r--r--   0        0        0      557 2024-05-21 19:28:12.454654 tailucas_pylib-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6677 2024-05-21 19:09:22.494655 tailucas_pylib-0.4.1/tailucas_pylib/__init__.py
+-rw-r--r--   0        0        0     2269 2024-05-21 19:20:13.224657 tailucas_pylib-0.4.1/tailucas_pylib/app.py
+-rw-r--r--   0        0        0     1371 2024-05-21 19:19:43.864657 tailucas_pylib-0.4.1/tailucas_pylib/aws/__init__.py
+-rw-r--r--   0        0        0     1426 2024-05-21 19:19:55.344657 tailucas_pylib-0.4.1/tailucas_pylib/aws/metrics.py
+-rw-r--r--   0        0        0     9194 2024-05-21 19:20:03.704657 tailucas_pylib-0.4.1/tailucas_pylib/aws/swf.py
+-rw-r--r--   0        0        0     2475 2024-05-21 19:21:17.174659 tailucas_pylib-0.4.1/tailucas_pylib/bluetooth.py
+-rw-r--r--   0        0        0      739 2024-05-21 19:21:37.124660 tailucas_pylib-0.4.1/tailucas_pylib/data.py
+-rw-r--r--   0        0        0     3287 2024-05-21 19:21:43.304660 tailucas_pylib-0.4.1/tailucas_pylib/datetime.py
+-rw-r--r--   0        0        0     1505 2024-05-21 19:10:35.564653 tailucas_pylib-0.4.1/tailucas_pylib/device.py
+-rw-r--r--   0        0        0     3206 2024-05-21 19:21:49.914660 tailucas_pylib-0.4.1/tailucas_pylib/handler.py
+-rw-r--r--   0        0        0     1023 2024-05-21 19:21:53.924660 tailucas_pylib-0.4.1/tailucas_pylib/process.py
+-rw-r--r--   0        0        0    10718 2024-05-21 19:22:00.294660 tailucas_pylib-0.4.1/tailucas_pylib/rabbit.py
+-rw-r--r--   0        0        0     5685 2024-05-21 19:23:47.274660 tailucas_pylib-0.4.1/tailucas_pylib/threads.py
+-rw-r--r--   0        0        0     3525 2024-05-21 19:22:37.504660 tailucas_pylib-0.4.1/tailucas_pylib/zmq.py
+-rw-r--r--   0        0        0    12330 1970-01-01 00:00:00.000000 tailucas_pylib-0.4.1/PKG-INFO
```

### Comparing `tailucas_pylib-0.4.0/LICENSE` & `tailucas_pylib-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.4.0/README.md` & `tailucas_pylib-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.4.0/pyproject.toml` & `tailucas_pylib-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tailucas-pylib"
-version = "0.4.0"
+version = "0.4.1"
 description = "Common Python utility modules"
 authors = ["Tai Lucas <tglucas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `tailucas_pylib-0.4.0/tailucas_pylib/__init__.py` & `tailucas_pylib-0.4.1/tailucas_pylib/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,136 +1,165 @@
 import builtins
 import logging.handlers
 import os.path
 import sys
 
-
-if hasattr(builtins, 'PYTEST'):
+if hasattr(builtins, "PYTEST"):
     pass
 else:
     from app import APP_NAME, WORK_DIR
+
     builtins.APP_NAME = APP_NAME  # type: ignore
     builtins.APP_PATH = WORK_DIR  # type: ignore
 
     log = logging.getLogger(APP_NAME)
 
     # do not propagate to console logging
     log.propagate = False
     # DEBUG logging until startup complete
     log.setLevel(logging.DEBUG)
     # define the log format
-    formatter = logging.Formatter('%(name)s %(threadName)s [%(levelname)s] %(message)s')
+    formatter = logging.Formatter("%(name)s %(threadName)s [%(levelname)s] %(message)s")
     log_handler = None
-    if os.path.exists('/dev/log'):
-        log_handler = logging.handlers.SysLogHandler(address='/dev/log')
+    if os.path.exists("/dev/log"):
+        log_handler = logging.handlers.SysLogHandler(address="/dev/log")
         log_handler.setFormatter(formatter)
         log.addHandler(log_handler)
-    if sys.stdout.isatty() or ('SUPERVISOR_ENABLED' in os.environ and log_handler is None):
-        log.warning("Using console logging because there is a tty or under supervisord.")
+    if sys.stdout.isatty() or (
+        "SUPERVISOR_ENABLED" in os.environ and log_handler is None
+    ):
+        log.warning(
+            "Using console logging because there is a tty or under supervisord."
+        )
         log_handler = logging.StreamHandler(stream=sys.stdout)
         log_handler.setFormatter(formatter)
         log.addHandler(log_handler)
     builtins.log = log  # type: ignore
     builtins.log_handler = log_handler  # type: ignore
 
     # use parent of this module's top-level __init__.py
     from pathlib import Path
+
     app_path = Path(os.path.abspath(os.path.dirname(__file__))).parent
-    log.debug(f'Running from {app_path}, using working directory {WORK_DIR}')
+    log.debug(f"Running from {app_path}, using working directory {WORK_DIR}")
     # assert working directory for assumptions made (such as PyDrive)
     current_work_dir = os.getcwd()
     if current_work_dir != WORK_DIR:
-        log.warning(f'Changing working directory from {current_work_dir} to {WORK_DIR}')
+        log.warning(f"Changing working directory from {current_work_dir} to {WORK_DIR}")
         os.chdir(WORK_DIR)
 
     from configparser import ConfigParser
+
     app_config = ConfigParser()
     app_config.optionxform = str
-    app_config_path = os.path.join(WORK_DIR, f'app.conf')
+    app_config_path = os.path.join(WORK_DIR, "app.conf")
     if os.path.exists(app_config_path):
-        log.info(f'Loading application configuration from {app_config_path}')
+        log.info(f"Loading application configuration from {app_config_path}")
         app_config.read([app_config_path])
-        device_name = app_config.get('app', 'device_name')
+        device_name = app_config.get("app", "device_name")
         builtins.DEVICE_NAME = device_name  # type: ignore
         device_name_base = device_name
-        device_name_parts = device_name.split('-')
+        device_name_parts = device_name.split("-")
         if len(device_name_parts) > 2:
             # throw away any suffixes
-            device_name_base = '-'.join(device_name_parts[0:2])
+            device_name_base = "-".join(device_name_parts[0:2])
         builtins.DEVICE_NAME_BASE = device_name_base  # type: ignore
     else:
-        log.warning(f'Setting builtins DEVICE_NAME and DEVICE_NAME_BASE to "{APP_NAME}" due to missing configuration.')
+        log.warning(
+            f'Setting builtins DEVICE_NAME and DEVICE_NAME_BASE to "{APP_NAME}" due to missing configuration.'
+        )
         builtins.DEVICE_NAME = APP_NAME
         builtins.DEVICE_NAME_BASE = APP_NAME
     builtins.APP_CONFIG = app_config  # type: ignore
 
     # 1Password credentials
     creds = None
     app_creds_config = None
-    op_connect_server_env = 'OP_CONNECT_HOST'
+    op_connect_server_env = "OP_CONNECT_HOST"
     if op_connect_server_env in os.environ:
-        if hasattr(builtins, 'creds_config'):
+        if hasattr(builtins, "creds_config"):
             try:
                 app_creds_config = builtins.creds_config
                 import onepasswordconnectsdk
                 from onepasswordconnectsdk.client import (
                     Client,
-                    new_client_from_environment
+                    new_client_from_environment,
                 )
+
                 creds_client: Client = new_client_from_environment()
                 creds_vaults = creds_client.get_vaults()
-                creds_vault_id = os.environ['OP_VAULT']
+                creds_vault_id = os.environ["OP_VAULT"]
                 op_connect_server = os.environ[op_connect_server_env]
                 vault_found = False
                 if creds_vaults:
                     for vault in creds_vaults:
-                        log.info(f"Credential vault on 1Password server {op_connect_server} {vault.name} ({vault.id}) contains {vault.items} credentials.")
+                        log.info(
+                            f"Credential vault on 1Password server {op_connect_server} {vault.name} ({vault.id}) contains {vault.items} credentials."
+                        )
                         if creds_vault_id == vault.id:
                             vault_found = True
                 if not vault_found:
-                    log.error(f'No vault matching ID {creds_vault_id} found on 1Password server {op_connect_server}. See https://github.com/1Password/connect-sdk-python/')
+                    log.error(
+                        f"No vault matching ID {creds_vault_id} found on 1Password server {op_connect_server}. See https://github.com/1Password/connect-sdk-python/"
+                    )
                     sys.exit(1)
-                creds = onepasswordconnectsdk.load(client=creds_client, config=app_creds_config)
+                creds = onepasswordconnectsdk.load(
+                    client=creds_client, config=app_creds_config
+                )
                 builtins.creds = creds  # type: ignore
-                builtins.creds_vault_id = creds_vault_id # type: ignore
+                builtins.creds_vault_id = creds_vault_id  # type: ignore
             except ModuleNotFoundError:
-                log.error('1Password configuration is set but onepasswordconnectsdk is not available or missing from package configuration.')
+                log.error(
+                    "1Password configuration is set but onepasswordconnectsdk is not available or missing from package configuration."
+                )
         else:
-            log.warning(f'Assign CredsConfig to builtins.creds_config in __main__ to enable 1Password credential services.')
+            log.warning(
+                "Assign CredsConfig to builtins.creds_config in __main__ to enable 1Password credential services."
+            )
     else:
-        log.warning(f'Set environment variable {op_connect_server_env} to enable 1Password credential services.')
+        log.warning(
+            f"Set environment variable {op_connect_server_env} to enable 1Password credential services."
+        )
 
     # Sentry
-    if app_creds_config and hasattr(app_creds_config, 'sentry_dsn'):
+    if app_creds_config and hasattr(app_creds_config, "sentry_dsn"):
         integrations = []
-        if hasattr(builtins, 'SENTRY_EXTRAS'):
+        if hasattr(builtins, "SENTRY_EXTRAS"):
             integrations = builtins.SENTRY_EXTRAS  # type: ignore
         else:
-            log.warning(f'Define a list builtins.SENTRY_EXTRAS in __main__ to enable Sentry.io extras.')
+            log.warning(
+                "Define a list builtins.SENTRY_EXTRAS in __main__ to enable Sentry.io extras."
+            )
         sentry_environment = None
-        if hasattr(builtins, 'SENTRY_ENVIRONMENT'):
+        if hasattr(builtins, "SENTRY_ENVIRONMENT"):
             sentry_environment = builtins.SENTRY_ENVIRONMENT  # type: ignore
         sentry_default_integrations = True
-        if hasattr(builtins, 'SENTRY_DEFAULT_INTEGRATIONS'):
+        if hasattr(builtins, "SENTRY_DEFAULT_INTEGRATIONS"):
             sentry_default_integrations = builtins.SENTRY_DEFAULT_INTEGRATIONS  # type: ignore
         import sentry_sdk
+
         sentry_sdk.init(
             dsn=creds.sentry_dsn,  # type: ignore
             environment=sentry_environment,  # type: ignore
             integrations=integrations,
-            default_integrations=sentry_default_integrations
+            default_integrations=sentry_default_integrations,
         )
     else:
-        log.warning(f'Add sentry_dsn to CredsConfig in __main__ to enable Sentry.io ticketing.')
+        log.warning(
+            "Add sentry_dsn to CredsConfig in __main__ to enable Sentry.io ticketing."
+        )
 
     # Cronitor
-    if app_creds_config and hasattr(app_creds_config, 'cronitor_token'):
+    if app_creds_config and hasattr(app_creds_config, "cronitor_token"):
         import cronitor
+
         cronitor.api_key = creds.cronitor_token  # type: ignore
     else:
-        log.warning(f'Add cronitor_token to CredsConfig in __main__ to enable Cronitor.io monitoring.')
+        log.warning(
+            "Add cronitor_token to CredsConfig in __main__ to enable Cronitor.io monitoring."
+        )
 
     # ZMQ helpers
-    URL_WORKER_APP = 'inproc://app'
+    URL_WORKER_APP = "inproc://app"
     builtins.URL_WORKER_APP = URL_WORKER_APP  # type: ignore
-    URL_WORKER_PUBLISHER = 'inproc://publisher'
-    builtins.URL_WORKER_PUBLISHER = URL_WORKER_PUBLISHER  # type: ignore
+    URL_WORKER_PUBLISHER = "inproc://publisher"
+    builtins.URL_WORKER_PUBLISHER = URL_WORKER_PUBLISHER  # type: ignore
```

### Comparing `tailucas_pylib-0.4.0/tailucas_pylib/app.py` & `tailucas_pylib-0.4.1/tailucas_pylib/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,77 @@
 import logging
-import zmq
-
 from threading import Thread
 from typing import Dict
 
+import zmq
+
 from .data import make_payload
 from .handler import exception_handler
 from .threads import shutting_down, threads_tracked
 from .zmq import Closable
 
-
-log = logging.getLogger(APP_NAME)  # type: ignore
+log = logging.getLogger(APP_NAME)  # type: ignore  # noqa: F821
 
 
 class AppThread(Thread):
-
     def __init__(self, name):
         Thread.__init__(self, name=name)
         self.daemon = True
         threads_tracked.add(self.name)
 
     def untrack(self):
         threads_tracked.remove(self.name)
 
 
 class ZmqRelay(AppThread, Closable):
-
     def __init__(self, name, source_zmq_url, sink_zmq_url):
         AppThread.__init__(self, name=name)
         Closable.__init__(self, connect_url=source_zmq_url)
         self._sink_zmq_url = sink_zmq_url
 
     def process_message(self, sink_socket):
         data = self.socket.recv_pyobj()
         payload = make_payload(data=data)
         # do not info on heartbeats
-        if 'device_info' not in data:
-            log.debug(f'Relaying {len(data)} bytes from {self.socket_url} to {self._sink_zmq_url} ({len(payload)} bytes)')
+        if "device_info" not in data:
+            log.debug(
+                f"Relaying {len(data)} bytes from {self.socket_url} to {self._sink_zmq_url} ({len(payload)} bytes)"
+            )
         sink_socket.send(payload)
 
     def startup(self):
         pass
 
     def run(self):
         self.startup()
         self.get_socket()
-        with exception_handler(connect_url=self._sink_zmq_url, and_raise=False, shutdown_on_error=True) as socket:
+        with exception_handler(
+            connect_url=self._sink_zmq_url, and_raise=False, shutdown_on_error=True
+        ) as socket:
             while not shutting_down:
                 self.process_message(sink_socket=socket)
         self.close()
 
 
 class ZmqWorker(AppThread):
-
     def __init__(self, name: str, worker_zmq_url: str):
         AppThread.__init__(self, name=name)
         self._worker_zmq_url = worker_zmq_url
 
     async def process_message(self, message: Dict) -> Dict:
         raise NotImplementedError()
 
     def startup(self):
         pass
 
     def run(self):
         self.startup()
-        with exception_handler(connect_url=self._worker_zmq_url, socket_type=zmq.REP, and_raise=False, shutdown_on_error=True) as zmq_socket:
+        with exception_handler(
+            connect_url=self._worker_zmq_url,
+            socket_type=zmq.REP,
+            and_raise=False,
+            shutdown_on_error=True,
+        ) as zmq_socket:
             while not shutting_down:
                 message = zmq_socket.recv_pyobj()
                 response = self.process_message(message=message)
                 zmq_socket.send_pyobj(response)
```

### Comparing `tailucas_pylib-0.4.0/tailucas_pylib/aws/__init__.py` & `tailucas_pylib-0.4.1/tailucas_pylib/aws/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import builtins
 import logging
 import os
 
-
-log = logging.getLogger(APP_NAME)  # type: ignore
+log = logging.getLogger(APP_NAME)  # type: ignore  # noqa: F821
 boto3_session = None
 aws_enabled = False
 
 try:
-    os.environ['AWS_ACCESS_KEY_ID']
-    os.environ['AWS_SECRET_ACCESS_KEY']
+    os.environ["AWS_ACCESS_KEY_ID"]
+    os.environ["AWS_SECRET_ACCESS_KEY"]
     aws_enabled = True
 except KeyError:
-    if hasattr(builtins, 'creds_config') and hasattr(creds_config, 'aws_akid'):  # type: ignore
-        log.debug('AWS environment variables unset. Setting in Python from credential provider.')
-        os.environ['AWS_ACCESS_KEY_ID'] = creds_config.aws_akid  # type: ignore
-        os.environ['AWS_SECRET_ACCESS_KEY'] = creds_config.aws_sak  # type: ignore
+    if hasattr(builtins, "creds_config") and hasattr(creds_config, "aws_akid"):  # type: ignore  # noqa: F821
+        log.debug(
+            "AWS environment variables unset. Setting in Python from credential provider."
+        )
+        os.environ["AWS_ACCESS_KEY_ID"] = creds_config.aws_akid  # type: ignore  # noqa: F821
+        os.environ["AWS_SECRET_ACCESS_KEY"] = creds_config.aws_sak  # type: ignore  # noqa: F821
         aws_enabled = True
 
 if aws_enabled:
     from boto3 import Session
     from botocore.session import Session as BotoCoreSession
 
     boto_session = BotoCoreSession()
     boto3_session = Session(
-        aws_access_key_id=creds_config.aws_akid,  # type: ignore
-        aws_secret_access_key=creds_config.aws_sak,  # type: ignore
-        botocore_session=boto_session)
-
-if hasattr(builtins, 'APP_CONFIG') and APP_CONFIG.has_section('botoflow'):  # type: ignore
-    swf_region = APP_CONFIG.get('botoflow', 'region')  # type: ignore
-    swf_domain = APP_CONFIG.get('botoflow', 'domain')  # type: ignore
+        aws_access_key_id=creds_config.aws_akid,  # type: ignore  # noqa: F821
+        aws_secret_access_key=creds_config.aws_sak,  # type: ignore  # noqa: F821
+        botocore_session=boto_session,
+    )
+
+if hasattr(builtins, "APP_CONFIG") and APP_CONFIG.has_section("botoflow"):  # type: ignore  # noqa: F821
+    swf_region = APP_CONFIG.get("botoflow", "region")  # type: ignore  # noqa: F821
+    swf_domain = APP_CONFIG.get("botoflow", "domain")  # type: ignore  # noqa: F821
```

### Comparing `tailucas_pylib-0.4.0/tailucas_pylib/aws/swf.py` & `tailucas_pylib-0.4.1/tailucas_pylib/aws/swf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,230 +1,248 @@
 import logging
-import zmq
-
-from sentry_sdk import capture_exception
 from threading import Thread
 from traceback import StackSummary
-from botoflow import activity, \
-    activities, \
-    execute, \
-    return_, \
-    WorkflowDefinition
-from botoflow.options import activity_options
-from botoflow.constants import SECONDS, MINUTES
-from botocore.exceptions import EndpointConnectionError as bcece
-from botoflow.exceptions import ActivityTaskFailedError, ActivityTaskTimedOutError, \
-    WorkflowFailedError, WorkflowTimedOutError
 
-from .metrics import post_count_metric
+import zmq
+from botocore.exceptions import EndpointConnectionError as bcece
+from botoflow import WorkflowDefinition, activities, activity, execute, return_
+from botoflow.constants import MINUTES, SECONDS
+from botoflow.exceptions import WorkflowFailedError, WorkflowTimedOutError
+from botoflow.options import activity_options
+from sentry_sdk import capture_exception
 
 from .. import threads
 from ..bluetooth import ping_bluetooth_devices
 from ..data import make_payload
 from ..handler import exception_handler
+from .metrics import post_count_metric
 
-
-log = logging.getLogger(APP_NAME)  # type: ignore
+log = logging.getLogger(APP_NAME)  # type: ignore  # noqa: F821
 
 
 class SWFActivityWaiter(Thread):
-
-    def __init__(self, zmq_ipc_url, event_source, output_type, workflow_starter, workflow_instance):
+    def __init__(
+        self,
+        zmq_ipc_url,
+        event_source,
+        output_type,
+        workflow_starter,
+        workflow_instance,
+    ):
         Thread.__init__(self, name=self.__class__.__name__)
         self.daemon = True
         self._event_source = event_source
         self._output_type = output_type
         self._workflow_starter = workflow_starter
         self._workflow_instance = workflow_instance
         self._zmq_url = zmq_ipc_url
 
     def run(self):
         if self._workflow_instance is None:
-            log.warning(f'No workflow instance for {self._output_type} @ {self._event_source}')
+            log.warning(
+                f"No workflow instance for {self._output_type} @ {self._event_source}"
+            )
             return
         execution_result = None
-        with exception_handler(connect_url=self._zmq_url, socket_type=zmq.PUSH, and_raise=False) as zmq_socket:
+        with exception_handler(
+            connect_url=self._zmq_url, socket_type=zmq.PUSH, and_raise=False
+        ) as zmq_socket:
             try:
-                log.info(f"Awaiting {self._output_type} execution result: {self._workflow_instance.workflow_execution}")
-                execution_result = self._workflow_starter.wait_for_completion(self._workflow_instance, 1)
+                log.info(
+                    f"Awaiting {self._output_type} execution result: {self._workflow_instance.workflow_execution}"
+                )
+                execution_result = self._workflow_starter.wait_for_completion(
+                    self._workflow_instance, 1
+                )
             except (WorkflowTimedOutError, WorkflowFailedError):
-                log.warning(f'Workflow {self._workflow_instance.workflow_execution} has failed.', exc_info=True)
+                log.warning(
+                    f"Workflow {self._workflow_instance.workflow_execution} has failed.",
+                    exc_info=True,
+                )
             if execution_result is not None:
                 zmq_socket.send_pyobj({self._event_source: execution_result})
-        message = f'Workflow is done for {self._output_type} with result {execution_result}'
+        message = (
+            f"Workflow is done for {self._output_type} with result {execution_result}"
+        )
         if execution_result:
             log.info(message)
         else:
             log.warning(message)
 
 
 def swf_exception_handler(err: Exception, tb_list: StackSummary):
     try:
         raise err
     except bcece:
-        log.warning(f'SWF', exc_info=True)
+        log.warning("SWF", exc_info=True)
     except Exception:
-        log.exception('SWF')
+        log.exception("SWF")
         capture_exception()
-        post_count_metric('Fatals')
+        post_count_metric("Fatals")
     finally:
         threads.shutting_down = True
         threads.interruptable_sleep.set()
 
 
-@activities(schedule_to_start_timeout=1*MINUTES,
-            start_to_close_timeout=1*MINUTES)
+@activities(schedule_to_start_timeout=1 * MINUTES, start_to_close_timeout=1 * MINUTES)
 class HelloWorldActivities(object):
-
-    @activity(version='1.0', start_to_close_timeout=5*SECONDS)
+    @activity(version="1.0", start_to_close_timeout=5 * SECONDS)
     def get_name(self):
-        return APP_NAME # type: ignore
+        return APP_NAME  # type: ignore  # noqa: F821
 
-    @activity(version='1.1', start_to_close_timeout=5*SECONDS)
+    @activity(version="1.1", start_to_close_timeout=5 * SECONDS)
     def print_greeting(self, greeting, name):
         message = f"{greeting} {name}!"
         log.info(message)
         return message
 
 
 class HelloWorldWorkflow(WorkflowDefinition):
-
-    @execute(version='1.1', execution_start_to_close_timeout=1*MINUTES)
+    @execute(version="1.1", execution_start_to_close_timeout=1 * MINUTES)
     def execute(self, greeting):
         name = yield HelloWorldActivities.get_name()
-        with activity_options(task_list='notifier'):
+        with activity_options(task_list="notifier"):
             yield TTSActivity.say(f"Testing {name}")
         response = yield HelloWorldActivities.print_greeting(greeting, name)
         return_(response)
 
 
-@activities(schedule_to_start_timeout=1*MINUTES,
-            start_to_close_timeout=1*MINUTES)
+@activities(schedule_to_start_timeout=1 * MINUTES, start_to_close_timeout=1 * MINUTES)
 class BluetoothActivity(object):
-
     def __init__(self, device_key, device_type, device_location):
         super().__init__()
         self.device_key = device_key
         self.device_type = device_type
         self.device_location = device_location
 
-    @activity(version='1.0', start_to_close_timeout=20*SECONDS)
+    @activity(version="1.0", start_to_close_timeout=20 * SECONDS)
     def ping_bluetooth(self, owner_device_list):
         ping_responses = ping_bluetooth_devices(owner_device_list)
-        log.info(f'{self.device_type} {owner_device_list!s} in {self.device_location} returns {ping_responses!s}...')
+        log.info(
+            f"{self.device_type} {owner_device_list!s} in {self.device_location} returns {ping_responses!s}..."
+        )
         if ping_responses is None:
             return None
         active_devices = []
         for owner, ping_response in list(ping_responses.items()):
-            device_label = f'{owner} is here.'
-            log.info(f'{self.device_type} {owner} in {self.device_location}: [{ping_response}] => ({device_label})')
-            active_devices.append({
-                    'device_key': self.device_key,
-                    'device_type': self.device_type,
-                    'device_location': self.device_location,
-                    'device_label': device_label})
+            device_label = f"{owner} is here."
+            log.info(
+                f"{self.device_type} {owner} in {self.device_location}: [{ping_response}] => ({device_label})"
+            )
+            active_devices.append(
+                {
+                    "device_key": self.device_key,
+                    "device_type": self.device_type,
+                    "device_location": self.device_location,
+                    "device_label": device_label,
+                }
+            )
         return make_payload(
-            timestamp=None,
-            data={'active_devices': active_devices},
-            msgpack=False)
+            timestamp=None, data={"active_devices": active_devices}, msgpack=False
+        )
 
 
-@activities(schedule_to_start_timeout=1*MINUTES,
-            start_to_close_timeout=1*MINUTES)
+@activities(schedule_to_start_timeout=1 * MINUTES, start_to_close_timeout=1 * MINUTES)
 class IOBoardActivity(object):
-
     def __init__(self, zmq_url):
         self._zmq_url = zmq_url
 
-    @activity(version='1.1', start_to_close_timeout=5*SECONDS)
+    @activity(version="1.1", start_to_close_timeout=5 * SECONDS)
     def trigger_output(self, device_key, duration):
-        with exception_handler(connect_url=self._zmq_url, socket_type=zmq.PUSH, and_raise=False) as zmq_socket:
+        with exception_handler(
+            connect_url=self._zmq_url, socket_type=zmq.PUSH, and_raise=False
+        ) as zmq_socket:
             zmq_socket.send_pyobj((device_key, duration))
 
 
-@activities(schedule_to_start_timeout=1*MINUTES,
-            start_to_close_timeout=1*MINUTES)
+@activities(schedule_to_start_timeout=1 * MINUTES, start_to_close_timeout=1 * MINUTES)
 class TTSActivity(object):
-
     def __init__(self, zmq_url):
         self._zmq_url = zmq_url
 
-    @activity(version='1.0', start_to_close_timeout=30*SECONDS)
+    @activity(version="1.0", start_to_close_timeout=30 * SECONDS)
     def say(self, message):
-        with exception_handler(connect_url=self._zmq_url, socket_type=zmq.PUSH, and_raise=False) as zmq_socket:
+        with exception_handler(
+            connect_url=self._zmq_url, socket_type=zmq.PUSH, and_raise=False
+        ) as zmq_socket:
             zmq_socket.send_pyobj(message)
 
 
-@activities(schedule_to_start_timeout=1*MINUTES,
-            start_to_close_timeout=1*MINUTES)
+@activities(schedule_to_start_timeout=1 * MINUTES, start_to_close_timeout=1 * MINUTES)
 class SnapshotActivity(object):
-
     def __init__(self, zmq_url):
         self._zmq_url = zmq_url
 
-    @activity(version='1.0', start_to_close_timeout=30*SECONDS)
+    @activity(version="1.0", start_to_close_timeout=30 * SECONDS)
     def snapshot_camera(self, device_key, device_label, camera_config):
-        with exception_handler(connect_url=self._zmq_url, socket_type=zmq.PUSH, and_raise=False) as zmq_socket:
+        with exception_handler(
+            connect_url=self._zmq_url, socket_type=zmq.PUSH, and_raise=False
+        ) as zmq_socket:
             zmq_socket.send_pyobj((device_key, device_label, camera_config))
 
 
-@activities(schedule_to_start_timeout=1*MINUTES,
-            start_to_close_timeout=1*MINUTES)
+@activities(schedule_to_start_timeout=1 * MINUTES, start_to_close_timeout=1 * MINUTES)
 class ImageProcessActivity(object):
-
     def __init__(self, zmq_url):
         self._zmq_url = zmq_url
 
-    @activity(version='1.0', start_to_close_timeout=30*SECONDS)
-    def image_process_camera(self, device_key, device_label, camera_config, snapshot_processor_address):
-        with exception_handler(connect_url=self._zmq_url, socket_type=zmq.PUSH, and_raise=False) as zmq_socket:
-            zmq_socket.send_pyobj((device_key, device_label, camera_config, snapshot_processor_address))
+    @activity(version="1.0", start_to_close_timeout=30 * SECONDS)
+    def image_process_camera(
+        self, device_key, device_label, camera_config, snapshot_processor_address
+    ):
+        with exception_handler(
+            connect_url=self._zmq_url, socket_type=zmq.PUSH, and_raise=False
+        ) as zmq_socket:
+            zmq_socket.send_pyobj(
+                (device_key, device_label, camera_config, snapshot_processor_address)
+            )
 
 
 class ImageProcessWorkflow(WorkflowDefinition):
-
-    @execute(version='1.0', execution_start_to_close_timeout=1*MINUTES)
-    def execute(self, app, device_key, device_label, camera_config, snapshot_processor_address):
+    @execute(version="1.0", execution_start_to_close_timeout=1 * MINUTES)
+    def execute(
+        self, app, device_key, device_label, camera_config, snapshot_processor_address
+    ):
         response = None
         with activity_options(task_list=app):
-            response = yield ImageProcessActivity.image_process_camera(device_key, device_label, camera_config, snapshot_processor_address)
+            response = yield ImageProcessActivity.image_process_camera(
+                device_key, device_label, camera_config, snapshot_processor_address
+            )
         return_(response)
 
 
 class SnapshotWorkflow(WorkflowDefinition):
-
-    @execute(version='1.0', execution_start_to_close_timeout=1*MINUTES)
+    @execute(version="1.0", execution_start_to_close_timeout=1 * MINUTES)
     def execute(self, app, device_key, device_label, camera_config):
         response = None
         with activity_options(task_list=app):
-            response = yield SnapshotActivity.snapshot_camera(device_key, device_label, camera_config)
+            response = yield SnapshotActivity.snapshot_camera(
+                device_key, device_label, camera_config
+            )
         return_(response)
 
 
 class TTSWorkflow(WorkflowDefinition):
-
-    @execute(version='1.0', execution_start_to_close_timeout=1*MINUTES)
+    @execute(version="1.0", execution_start_to_close_timeout=1 * MINUTES)
     def execute(self, app, message):
         response = None
         with activity_options(task_list=app):
             response = yield TTSActivity.say(message)
         return_(response)
 
 
 class IOBoardWorkflow(WorkflowDefinition):
-
-    @execute(version='1.0', execution_start_to_close_timeout=1*MINUTES)
+    @execute(version="1.0", execution_start_to_close_timeout=1 * MINUTES)
     def execute(self, app, device_key, duration=None):
         response = None
         with activity_options(task_list=app):
             response = yield IOBoardActivity.trigger_output(device_key, duration)
         return_(response)
 
 
 class BluetoothWorkflow(WorkflowDefinition):
-
-    @execute(version='1.0', execution_start_to_close_timeout=1*MINUTES)
+    @execute(version="1.0", execution_start_to_close_timeout=1 * MINUTES)
     def execute(self, app, owner_device_list):
         response = None
         with activity_options(task_list=app):
             response = yield BluetoothActivity.ping_bluetooth(owner_device_list)
-        return_(response)
+        return_(response)
```

### Comparing `tailucas_pylib-0.4.0/tailucas_pylib/bluetooth.py` & `tailucas_pylib-0.4.1/tailucas_pylib/bluetooth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,72 @@
 import logging
-from .process import exec_cmd
 
 from sentry_sdk import capture_exception
 
+from .process import exec_cmd
 
-log = logging.getLogger(APP_NAME)  # type: ignore
+log = logging.getLogger(APP_NAME)  # type: ignore  # noqa: F821
 
 
 def bluetooth_init():
     # first test for a Bluetooth adaptor and format this type of output
     # Devices:
     # hci0    00:09:DD:50:17:18
-    out, err, rc = exec_cmd(['hcitool', 'dev'])
+    out, err, rc = exec_cmd(["hcitool", "dev"])
     if rc != 0 or out is None:
-        raise RuntimeError(f'Cannot query hcitool to find Bluetooth adaptors: {out} {err}')
-    hcitool = out.decode().rstrip().split('\n')
+        raise RuntimeError(
+            f"Cannot query hcitool to find Bluetooth adaptors: {out} {err}"
+        )
+    hcitool = out.decode().rstrip().split("\n")
     if len(hcitool) < 2:
-        raise RuntimeError('No Bluetooth adaptors found using hcitool.')
+        raise RuntimeError("No Bluetooth adaptors found using hcitool.")
     for line in hcitool[1:]:
-        adapter = ' '.join(line.split())
-        log.info(f'Bluetooth adaptor found: {adapter}')
+        adapter = " ".join(line.split())
+        log.info(f"Bluetooth adaptor found: {adapter}")
 
 
 def l2ping(owner, device):
-    log.debug(f'l2ping {owner} @ {device}...')
-    out, err, rc = exec_cmd(['sudo', '/usr/bin/l2ping', '-t1', '-c1', device])
+    log.debug(f"l2ping {owner} @ {device}...")
+    out, err, rc = exec_cmd(["sudo", "/usr/bin/l2ping", "-t1", "-c1", device])
     l2pingo = None
     if out is not None:
         l2pingo = out.decode()
     else:
-        raise RuntimeError(f'Cannot perform l2ping of {owner} @ {device}: {err}')
+        raise RuntimeError(f"Cannot perform l2ping of {owner} @ {device}: {err}")
     if rc == 0:
-        log.debug(f'l2ping output: {l2pingo}')
+        log.debug(f"l2ping output: {l2pingo}")
         return l2pingo
     else:
-        log.debug(f'Non-zero exit {rc} for l2ping output: {l2pingo} {err}')
+        log.debug(f"Non-zero exit {rc} for l2ping output: {l2pingo} {err}")
     return None
 
 
 def ping_bluetooth_devices(owner_device_list):
     owner_devices = list()
     ping_response = dict()
     try:
         log.debug(owner_device_list)
-        if type(owner_device_list) is str:
-            owner_device_string = owner_device_list.split(',')
+        if isinstance(owner_device_list, str):
+            owner_device_string = owner_device_list.split(",")
             for ods in owner_device_string:
-                od = ods.split(';')
+                od = ods.split(";")
                 owner_devices.append((od[0], od[1]))
-        elif type(owner_device_list) is tuple:
+        elif isinstance(owner_device_list, tuple):
             owner_devices.append(owner_device_list)
-        elif type(owner_device_list) is list:
+        elif isinstance(owner_device_list, list):
             owner_devices = owner_device_list
         else:
             raise f"Unsupported type {type(owner_device_list)} for parameters {owner_device_list}."
-        log.info(f'DEBUG: l2ping using {owner_devices}.')
+        log.info(f"DEBUG: l2ping using {owner_devices}.")
         for owner, device in owner_devices:
             sample_value = l2ping(owner, device)
-            log.debug(f'ping response for {owner} @ {device}: {sample_value}')
+            log.debug(f"ping response for {owner} @ {device}: {sample_value}")
             if sample_value:
                 ping_response[owner] = sample_value
     except Exception:
-        log.exception('ping_bluetooth_devices')
+        log.exception("ping_bluetooth_devices")
         capture_exception()
         raise
 
     if len(ping_response) > 0:
         return ping_response
     return None
```

### Comparing `tailucas_pylib-0.4.0/tailucas_pylib/data.py` & `tailucas_pylib-0.4.1/tailucas_pylib/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
-import simplejson as json
+
 import msgpack
+import simplejson as json
 
 from .datetime import make_timestamp
 
-
-log = logging.getLogger(APP_NAME)  # type: ignore
+log = logging.getLogger(APP_NAME)  # type: ignore  # noqa: F821
 
 
 def make_payload(timestamp=None, data=None, pack=True):
-    payload = {'timestamp': make_timestamp(timestamp=timestamp, make_string=True)}
+    payload = {"timestamp": make_timestamp(timestamp=timestamp, make_string=True)}
     if data is not None and len(data) > 0:
         if isinstance(data, dict):
             payload.update(data)
         else:
-            payload['data'] = data
+            payload["data"] = data
     if log.level == logging.DEBUG:
         try:
             log.debug(json.dumps(payload))
         except (TypeError, UnicodeDecodeError):
-            log.exception('Cannot JSON-encode payload for logging.')
+            log.exception("Cannot JSON-encode payload for logging.")
     if pack:
         return msgpack.packb(payload)
     return payload
```

### Comparing `tailucas_pylib-0.4.0/tailucas_pylib/datetime.py` & `tailucas_pylib-0.4.1/tailucas_pylib/datetime.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,81 +1,91 @@
 import logging
+from datetime import datetime
+
 import dateutil.parser
 import pytz
-
-from datetime import datetime, timedelta
 from dateutil import tz
 
-
-log = logging.getLogger(APP_NAME)  # type: ignore
+log = logging.getLogger(APP_NAME)  # type: ignore  # noqa: F821
 
 
-ISO_DATE_FORMAT = '%Y-%m-%dT%H:%M:%S.%f%z'
+ISO_DATE_FORMAT = "%Y-%m-%dT%H:%M:%S.%f%z"
 
 
 def is_list(value):
     return isinstance(value, list)
 
 
 def make_timestamp(timestamp=None, as_tz=pytz.utc, make_string=False):
     if isinstance(timestamp, float) or isinstance(timestamp, int):
         timestamp = datetime.utcfromtimestamp(timestamp).replace(tzinfo=pytz.utc)
     elif isinstance(timestamp, str):
         try:
-            log.debug(f'Attempting to parse timestamp {timestamp}')
+            log.debug(f"Attempting to parse timestamp {timestamp}")
             timestamp = dateutil.parser.parse(timestamp)
-            log.debug(f'Parsed timestamp is {timestamp}')
+            log.debug(f"Parsed timestamp is {timestamp}")
         except ValueError:
             # try integer representation
             try:
-                timestamp = datetime.utcfromtimestamp(int(timestamp)).replace(tzinfo=pytz.utc)
-                log.debug(f'Parsed integer timestamp is {timestamp}')
+                timestamp = datetime.utcfromtimestamp(int(timestamp)).replace(
+                    tzinfo=pytz.utc
+                )
+                log.debug(f"Parsed integer timestamp is {timestamp}")
             except ValueError:
                 log.exception(f"Unable to parse {timestamp}. Using 'now'.")
                 timestamp = None
     if timestamp is None:
         timestamp = datetime.utcnow().replace(tzinfo=pytz.utc)
     if timestamp.tzinfo is None:
         local_tz = tz.tzlocal()
-        log.debug(f'{timestamp}: fixed to local time {local_tz}')
+        log.debug(f"{timestamp}: fixed to local time {local_tz}")
         # we use the default specific to the physical locality of the devices
         timestamp = timestamp.replace(tzinfo=local_tz)
     if timestamp.tzinfo != as_tz:
         # now adjust to requested TZ
         new_timestamp = timestamp.astimezone(tz=as_tz)
-        log.debug(f'{timestamp} adjusted to {new_timestamp} ({timestamp.tzinfo} to {as_tz})')
+        log.debug(
+            f"{timestamp} adjusted to {new_timestamp} ({timestamp.tzinfo} to {as_tz})"
+        )
         timestamp = new_timestamp
-    log.debug(f'Using timestamp {timestamp}')
+    log.debug(f"Using timestamp {timestamp}")
     if make_string:
         return timestamp.strftime(ISO_DATE_FORMAT)  # type: ignore
     return timestamp
 
 
 def make_unix_timestamp(timestamp=None):
-    return int((make_timestamp(timestamp=timestamp).replace(tzinfo=None) - datetime(1970, 1, 1)).total_seconds())
+    return int(
+        (
+            make_timestamp(timestamp=timestamp).replace(tzinfo=None)
+            - datetime(1970, 1, 1)
+        ).total_seconds()
+    )
 
 
 def parse_datetime(value=None, as_tz=pytz.utc):
     timestamp = datetime.utcnow().replace(tzinfo=as_tz)
     if value is None:
         return timestamp
     if isinstance(value, str):
         try:
             timestamp = dateutil.parser.parse(value)
-            log.debug(f'Parsed timestamp is {timestamp}')
+            log.debug(f"Parsed timestamp is {timestamp}")
         except ValueError:
-            log.exception(f"Cannot parse date-like string {value}. Defaulting to '{timestamp}'.")
+            log.exception(
+                f"Cannot parse date-like string {value}. Defaulting to '{timestamp}'."
+            )
     elif isinstance(value, datetime):
         timestamp = value
     else:
         raise RuntimeError(f"Unknown date/time type: '{value}'")
     # ensure that some timezone information is present
     if timestamp.tzinfo is None:
         local_tz = tz.tzlocal()
-        log.debug(f'{timestamp}: setting to local time {local_tz}')
+        log.debug(f"{timestamp}: setting to local time {local_tz}")
         # we use the default specific to the physical locality of the devices
         timestamp = timestamp.replace(tzinfo=local_tz)
     if timestamp.tzinfo != as_tz:
         # now adjust to requested TZ
-        log.debug(f'{timestamp}: setting to {as_tz} from {timestamp.tzinfo}')
+        log.debug(f"{timestamp}: setting to {as_tz} from {timestamp.tzinfo}")
         timestamp = timestamp.astimezone(tz=as_tz)
     return timestamp
```

### Comparing `tailucas_pylib-0.4.0/tailucas_pylib/device.py` & `tailucas_pylib-0.4.1/tailucas_pylib/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from pydantic import BaseModel, Field
 from typing import Optional
+
+from pydantic import BaseModel, Field
 from typing_extensions import Annotated
 
 
 class Device(BaseModel):
     active: Optional[bool] = None
     device_id: Optional[str] = None
     device_key: str
@@ -25,20 +26,20 @@
     normal_value: Optional[int] = None
     pulse_discards: Optional[int] = None
     register_reading: Optional[int] = None
     sample_value: Optional[int] = None
     storage_path: Optional[str] = None
     storage_url: Optional[str] = None
     timestamp: Optional[int] = None
-    type_: Optional[Annotated[str, Field(alias='type')]] = None
+    type_: Optional[Annotated[str, Field(alias="type")]] = None
     uptime: Optional[int] = None
 
     def __str__(self):
-        str_rep = ''
+        str_rep = ""
         for name, value in vars(self).items():
             if len(str_rep) > 0:
-                str_rep += ','
+                str_rep += ","
             if not isinstance(value, bytes):
-                str_rep += f'{name}={value}'
+                str_rep += f"{name}={value}"
             else:
-                str_rep += f'{name}={len(value)} bytes'
-        return str_rep
+                str_rep += f"{name}={len(value)} bytes"
+        return str_rep
```

### Comparing `tailucas_pylib-0.4.0/tailucas_pylib/handler.py` & `tailucas_pylib-0.4.1/tailucas_pylib/handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 import logging
-import zmq
+from typing import ContextManager, Optional
 
+import zmq
 from sentry_sdk import capture_exception
-from typing import ContextManager, Optional
-from zmq.error import ZMQError, ContextTerminated
+from zmq.error import ContextTerminated
 
 from . import threads
-
 from .threads import die
-from .zmq import zmq_socket, try_close
-
+from .zmq import try_close, zmq_socket
 
-log = logging.getLogger(APP_NAME)  # type: ignore
+log = logging.getLogger(APP_NAME)  # type: ignore  # noqa: F821
 
 
 class exception_handler(ContextManager):
-
     def __init__(
-            self,
-            connect_url: str,
-            socket_type: Optional[int]=zmq.PUSH,
-            and_raise: Optional[bool]=True,
-            close_on_exit: Optional[bool]=True,
-            shutdown_on_error: Optional[bool]=False,
-            is_async: Optional[bool]=False):
+        self,
+        connect_url: str,
+        socket_type: Optional[int] = zmq.PUSH,
+        and_raise: Optional[bool] = True,
+        close_on_exit: Optional[bool] = True,
+        shutdown_on_error: Optional[bool] = False,
+        is_async: Optional[bool] = False,
+    ):
         self._zmq_socket = None
         self._zmq_url = connect_url
         self._socket_type = socket_type
         self._and_raise = and_raise
         self._close_on_exit = close_on_exit
         self._shutdown_on_error = shutdown_on_error
         self._is_async = is_async
 
     def __enter__(self):
-        self._zmq_socket = zmq_socket(socket_type=self._socket_type, is_async=self._is_async)
+        self._zmq_socket = zmq_socket(
+            socket_type=self._socket_type, is_async=self._is_async
+        )
         if self._socket_type in [zmq.PULL, zmq.PUB, zmq.REP]:
-            log.debug(f'Binding {self._socket_type} ({zmq.PUSH=}, {zmq.PULL=}, {zmq.REQ=}, {zmq.REP=}) ZMQ socket to {self._zmq_url}')
+            log.debug(
+                f"Binding {self._socket_type} ({zmq.PUSH=}, {zmq.PULL=}, {zmq.REQ=}, {zmq.REP=}) ZMQ socket to {self._zmq_url}"
+            )
             self._zmq_socket.bind(self._zmq_url)
         else:
-            log.debug(f'Connecting {self._socket_type} ({zmq.PUSH=}, {zmq.PULL=}, {zmq.REQ=}, {zmq.REP=}) ZMQ socket to {self._zmq_url}')
+            log.debug(
+                f"Connecting {self._socket_type} ({zmq.PUSH=}, {zmq.PULL=}, {zmq.REQ=}, {zmq.REP=}) ZMQ socket to {self._zmq_url}"
+            )
             self._zmq_socket.connect(self._zmq_url)
         return self._zmq_socket
 
     def __exit__(self, exc_type, exc_val, tb):
-        if self._close_on_exit or (exc_type and issubclass(exc_type, ContextTerminated)):
+        if self._close_on_exit or (
+            exc_type and issubclass(exc_type, ContextTerminated)
+        ):
             if self._zmq_socket:
                 try_close(self._zmq_socket)
         if exc_type is None:
             return True
-        log.debug(f'Handling {exc_type.__name__} with flags...')
+        log.debug(f"Handling {exc_type.__name__} with flags...")
         if issubclass(exc_type, ContextTerminated):
             log.debug(self.__class__.__name__, exc_info=True)
             # treat as non-critical
             return True
         elif issubclass(exc_type, ResourceWarning):
             # raised to indicate a fatal dependency error that
             # does not fill Sentry with exception regressions
@@ -69,8 +75,8 @@
                 log.exception(self.__class__.__name__)
                 capture_exception(error=(exc_type, exc_val, tb))
                 if self._shutdown_on_error:
                     die(exception=exc_type)
             else:
                 # log the exception as informational if in debug mode
                 log.debug(self.__class__.__name__, exc_info=True)
-        return not self._and_raise
+        return not self._and_raise
```

### Comparing `tailucas_pylib-0.4.0/tailucas_pylib/process.py` & `tailucas_pylib-0.4.1/tailucas_pylib/process.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 import logging
 import signal
 import subprocess
 
 from .threads import die
 
-
-log = logging.getLogger(APP_NAME)  # type: ignore
+log = logging.getLogger(APP_NAME)  # type: ignore  # noqa: F821
 
 
 def exec_cmd(cmd):
     p = subprocess.Popen(cmd, stdout=subprocess.PIPE)
     out, err = p.communicate()
     return out, err, p.returncode
 
 
 def exec_cmd_log(cmd):
-    o,e,c = exec_cmd(cmd)
-    log.info(f'{cmd} (exit {c}): {o}{e}')
+    o, e, c = exec_cmd(cmd)
+    log.info(f"{cmd} (exit {c}): {o}{e}")
 
 
 # noinspection PyUnusedLocal
 class SignalHandler:
-
     def __init__(self):
         self.last_signal = 0
         signal.signal(signal.SIGTERM, self.terminate)
         signal.signal(signal.SIGHUP, self.hup)
 
     def hup(self, signum, frame):
-        log.warning(f'Signal {signum} received.')
+        log.warning(f"Signal {signum} received.")
         self.last_signal = signum
         if log.getEffectiveLevel() == logging.INFO:
             log.setLevel(logging.DEBUG)
         elif log.getEffectiveLevel() == logging.DEBUG:
             log.setLevel(logging.INFO)
 
     def terminate(self, signum, frame):
-        log.warning(f'Signal {signum} received.')
+        log.warning(f"Signal {signum} received.")
         self.last_signal = signum
         die()
```

### Comparing `tailucas_pylib-0.4.0/tailucas_pylib/rabbit.py` & `tailucas_pylib-0.4.1/tailucas_pylib/rabbit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,223 +1,275 @@
 import logging
+
 import msgpack
 import pika
 import zmq
-
 from msgpack.exceptions import UnpackException
-from pika.exceptions import StreamLostError, \
-    ConnectionClosedByBroker, \
-    AMQPChannelError, \
-    AMQPConnectionError
+from pika.exceptions import (
+    AMQPConnectionError,
+    ConnectionClosedByBroker,
+    StreamLostError,
+)
 from sentry_sdk.integrations.logging import ignore_logger
 
 from . import threads
-
 from .app import AppThread
 from .data import make_payload
-from .datetime import make_timestamp, make_unix_timestamp
 from .handler import exception_handler
 
-
 # Reduce Sentry noise from pika loggers
-ignore_logger('pika.adapters.base_connection')
-ignore_logger('pika.adapters.blocking_connection')
-ignore_logger('pika.adapters.utils.connection_workflow')
-ignore_logger('pika.adapters.utils.io_services_utils')
-ignore_logger('pika.callback')
-ignore_logger('pika.channel')
-ignore_logger('pika.connection')
+ignore_logger("pika.adapters.base_connection")
+ignore_logger("pika.adapters.blocking_connection")
+ignore_logger("pika.adapters.utils.connection_workflow")
+ignore_logger("pika.adapters.utils.io_services_utils")
+ignore_logger("pika.callback")
+ignore_logger("pika.channel")
+ignore_logger("pika.connection")
 
 
-log = logging.getLogger(APP_NAME)  # type: ignore
+log = logging.getLogger(APP_NAME)  # type: ignore  # noqa: F821
 
 
 BLOCKED_CONNECTION_TIMEOUT = 5
 PUBLISH_RETRIES = 3
 
 
 class MQConnection(AppThread):
-    def __init__(self, name, mq_server_address, mq_exchange_name, mq_topic_filter='#', mq_exchange_type='topic', mq_arguments=None):
+    def __init__(
+        self,
+        name,
+        mq_server_address,
+        mq_exchange_name,
+        mq_topic_filter="#",
+        mq_exchange_type="topic",
+        mq_arguments=None,
+    ):
         AppThread.__init__(self, name=name)
 
         if isinstance(mq_server_address, str):
             self._mq_server_list = [mq_server_address]
         elif isinstance(mq_server_address, list):
             self._mq_server_list = mq_server_address
         else:
-            raise AssertionError(f'Unsupported argument type: {mq_server_address}')
+            raise AssertionError(f"Unsupported argument type: {mq_server_address}")
 
         pika_parameters = list()
         for source in self._mq_server_list:
-            pika_parameters.append(pika.ConnectionParameters(
-                host=source,
-                blocked_connection_timeout=BLOCKED_CONNECTION_TIMEOUT))
+            pika_parameters.append(
+                pika.ConnectionParameters(
+                    host=source, blocked_connection_timeout=BLOCKED_CONNECTION_TIMEOUT
+                )
+            )
         self._pika_parameters = tuple(pika_parameters)
 
         self._mq_exchange_name = mq_exchange_name
         self._mq_topic_filter = mq_topic_filter
         self._mq_exchange_type = mq_exchange_type
         self._mq_arguments = mq_arguments
 
         self._mq_connection = None
         self._mq_channel = None
         self._mq_queue_name = None
 
-    def _basic_publish(self, routing_key, event_payload, close_channel=False, close_connection=False):
+    def _basic_publish(
+        self, routing_key, event_payload, close_channel=False, close_connection=False
+    ):
         success = False
         tries = 1
         while tries <= PUBLISH_RETRIES:
             try:
                 self._setup_channel()
             except AMQPConnectionError as e:
-                raise ResourceWarning('Problem setting up connection or channel.') from e
+                raise ResourceWarning(
+                    "Problem setting up connection or channel."
+                ) from e
             try:
                 message_body = make_payload(data=event_payload)
-                log.info(f'Sending {len(message_body)} bytes to exchange {self._mq_exchange_name} with routing {routing_key} to queue {self._mq_queue_name}.')
+                log.info(
+                    f"Sending {len(message_body)} bytes to exchange {self._mq_exchange_name} with routing {routing_key} to queue {self._mq_queue_name}."
+                )
                 self._mq_channel.basic_publish(
                     exchange=self._mq_exchange_name,
                     routing_key=routing_key,
-                    body=message_body)
+                    body=message_body,
+                )
                 success = True
                 # exit loop
                 break
             except StreamLostError as e:
                 # try again
                 if tries < PUBLISH_RETRIES:
-                    log.warning(f'Retrying on lost stream during publish: {e!s}')
+                    log.warning(f"Retrying on lost stream during publish: {e!s}")
                 else:
-                    raise RuntimeWarning('Publish failure after retry.') from e
+                    raise RuntimeWarning("Publish failure after retry.") from e
             except ConnectionClosedByBroker as e:
                 raise ResourceWarning() from e
             finally:
                 if close_channel or not success:
-                    log.debug(f'Closing potentially stale channel (successful attempt? {success})...')
+                    log.debug(
+                        f"Closing potentially stale channel (successful attempt? {success})..."
+                    )
                     self._close_channel()
                     if tries > 1:
                         if close_connection or not success:
-                            log.debug(f'Closing potentially stale connection (successful attempt? {success})...')
+                            log.debug(
+                                f"Closing potentially stale connection (successful attempt? {success})..."
+                            )
                             self._close_connection()
                 tries += 1
         if not success:
-            raise AssertionError('No success after publish attempt.')
+            raise AssertionError("No success after publish attempt.")
 
     def _setup_connection(self):
         if self._mq_connection is None or self._mq_connection.is_closed:
             if self._mq_connection:
-                log.info(f'Recreating RabbitMQ connection...')
-            self._mq_connection = pika.BlockingConnection(parameters=self._pika_parameters)
+                log.info("Recreating RabbitMQ connection...")
+            self._mq_connection = pika.BlockingConnection(
+                parameters=self._pika_parameters
+            )
 
     def _setup_channel(self):
         self._setup_connection()
         if self._mq_channel is None or self._mq_channel.is_closed:
             if self._mq_channel:
-                log.info(f'Recreating RabbitMQ channel...')
+                log.info("Recreating RabbitMQ channel...")
             self._mq_channel = self._mq_connection.channel()
-            self._mq_channel.exchange_declare(exchange=self._mq_exchange_name, exchange_type=self._mq_exchange_type, arguments=self._mq_arguments)
-            mq_result = self._mq_channel.queue_declare('', exclusive=True)
+            self._mq_channel.exchange_declare(
+                exchange=self._mq_exchange_name,
+                exchange_type=self._mq_exchange_type,
+                arguments=self._mq_arguments,
+            )
+            mq_result = self._mq_channel.queue_declare("", exclusive=True)
             self._mq_queue_name = mq_result.method.queue
-            log.info(f'Using RabbitMQ server(s) {self._mq_server_list} using {self._mq_exchange_type} exchange {self._mq_exchange_name} and queue {self._mq_queue_name}.')
+            log.info(
+                f"Using RabbitMQ server(s) {self._mq_server_list} using {self._mq_exchange_type} exchange {self._mq_exchange_name} and queue {self._mq_queue_name}."
+            )
 
     def _close_connection(self):
         if self._mq_connection and self._mq_connection.is_open:
-            log.info(f'Closing RabbitMQ connection...')
+            log.info("Closing RabbitMQ connection...")
             try:
                 self._mq_connection.close()
             except Exception:
                 log.debug(self.__class__.__name__, exc_info=True)
 
     def _close_channel(self):
         if self._mq_channel and self._mq_channel.is_open:
-            log.info(f'Closing RabbitMQ channel...')
+            log.info("Closing RabbitMQ channel...")
             try:
                 self._mq_channel.close()
             except Exception:
                 log.debug(self.__class__.__name__, exc_info=True)
 
     def stop(self):
         self._close_channel()
         self._close_connection()
 
 
 class ZMQListener(MQConnection):
-
-    def __init__(self, zmq_url, mq_server_address, mq_exchange_name, mq_topic_filter, mq_exchange_type):
+    def __init__(
+        self,
+        zmq_url,
+        mq_server_address,
+        mq_exchange_name,
+        mq_topic_filter,
+        mq_exchange_type,
+    ):
         MQConnection.__init__(
             self,
-            name=f'{self.__class__.__name__} ({zmq_url})',
+            name=f"{self.__class__.__name__} ({zmq_url})",
             mq_server_address=mq_server_address,
             mq_exchange_name=mq_exchange_name,
             mq_topic_filter=mq_topic_filter,
-            mq_exchange_type=mq_exchange_type)
+            mq_exchange_type=mq_exchange_type,
+        )
         self._zmq_url = zmq_url
 
     def _setup_channel(self):
         MQConnection._setup_channel(self)
         self._mq_channel.queue_bind(
             exchange=self._mq_exchange_name,
             queue=self._mq_queue_name,
-            routing_key=self._mq_topic_filter)
+            routing_key=self._mq_topic_filter,
+        )
         self._mq_channel.basic_consume(
-            queue=self._mq_queue_name,
-            on_message_callback=self.callback,
-            auto_ack=True)
+            queue=self._mq_queue_name, on_message_callback=self.callback, auto_ack=True
+        )
 
     # noinspection PyBroadException
     def run(self):
-        with exception_handler(connect_url=self._zmq_url, and_raise=False, shutdown_on_error=True) as zmq_socket:
+        with exception_handler(
+            connect_url=self._zmq_url, and_raise=False, shutdown_on_error=True
+        ) as zmq_socket:
             self.processor = zmq_socket
             try:
                 self._setup_channel()
-                log.info(f'Ready for RabbitMQ messages.')
+                log.info("Ready for RabbitMQ messages.")
                 self._mq_channel.start_consuming()
-            except (AMQPConnectionError, ConnectionClosedByBroker, StreamLostError) as e:
+            except (
+                AMQPConnectionError,
+                ConnectionClosedByBroker,
+                StreamLostError,
+            ) as e:
                 # handled error due to already shutting down
-                raise ResourceWarning('Consumer interrupted.') from e
+                raise ResourceWarning("Consumer interrupted.") from e
             finally:
-                log.info(f'RabbitMQ listener has finished.')
+                log.info("RabbitMQ listener has finished.")
 
     def callback(self, ch, method, properties, body):
         topic = method.routing_key
-        log.debug(f'[{topic}]: {body}')
-        topic_parts = topic.split('.')
+        log.debug(f"[{topic}]: {body}")
+        topic_parts = topic.split(".")
         if len(topic_parts) < 3:
-            log.warning(f'Ignoring non-routable message from topic [{topic}] due to unsufficient topic parts.')
+            log.warning(
+                f"Ignoring non-routable message from topic [{topic}] due to unsufficient topic parts."
+            )
             return
-        if topic_parts[1] not in ['heartbeat', 'leader']:
-            log.info(f'Device event on topic [{topic}]')
+        if topic_parts[1] not in ["heartbeat", "leader"]:
+            log.info(f"Device event on topic [{topic}]")
         device_event = None
         try:
             device_event = msgpack.unpackb(body)
         except UnpackException:
-            log.exception('Bad message: {}'.format(body))
+            log.exception("Bad message: {}".format(body))
             return
         try:
             self.processor.send_pyobj({topic_parts[2]: device_event})
         except Exception as e:
             log.debug(self.__class__.__name__, exc_info=True)
             if not threads.shutting_down:
                 raise e
 
 
 class RabbitMQRelay(AppThread):
-
-    def __init__(self, zmq_url, mq_server_address, mq_exchange_name, mq_topic_filter, mq_exchange_type):
-        AppThread.__init__(self, name=f'{self.__class__.__name__} ({zmq_url})')
+    def __init__(
+        self,
+        zmq_url,
+        mq_server_address,
+        mq_exchange_name,
+        mq_topic_filter,
+        mq_exchange_type,
+    ):
+        AppThread.__init__(self, name=f"{self.__class__.__name__} ({zmq_url})")
         self._source_zmq_url = zmq_url
         self._source_socket_type = zmq.PULL
 
         self._mq_config_server = mq_server_address
         self._mq_connection = pika.BlockingConnection(
             pika.ConnectionParameters(
                 host=self._mq_config_server,
-                blocked_connection_timeout=BLOCKED_CONNECTION_TIMEOUT))
+                blocked_connection_timeout=BLOCKED_CONNECTION_TIMEOUT,
+            )
+        )
         self._mq_channel = self._mq_connection.channel()
         self._mq_config_exchange = mq_exchange_name
         self._mq_exchange_type = mq_exchange_type
-        self._mq_channel.exchange_declare(exchange=self._mq_config_exchange, exchange_type=self._mq_exchange_type)
+        self._mq_channel.exchange_declare(
+            exchange=self._mq_config_exchange, exchange_type=self._mq_exchange_type
+        )
         self._mq_device_topic = mq_topic_filter
 
     @property
     def device_topic(self):
         return self._mq_device_topic
 
     def close(self):
@@ -225,19 +277,27 @@
 
     def process_message(self, zmq_socket):
         event_topic, event_payload = zmq_socket.recv_pyobj()
         try:
             self._mq_channel.basic_publish(
                 exchange=self._mq_config_exchange,
                 routing_key=event_topic,
-                body=make_payload(data=event_payload))
+                body=make_payload(data=event_payload),
+            )
         except (ConnectionClosedByBroker, StreamLostError) as e:
             raise ResourceWarning() from e
 
     def startup(self):
-        log.info(f'Using RabbitMQ server at {self._mq_config_server} with {self._mq_exchange_type} ({self._mq_device_topic}) exchange {self._mq_config_exchange}.')
+        log.info(
+            f"Using RabbitMQ server at {self._mq_config_server} with {self._mq_exchange_type} ({self._mq_device_topic}) exchange {self._mq_config_exchange}."
+        )
 
     def run(self):
         self.startup()
-        with exception_handler(connect_url=self._source_zmq_url, socket_type=self._source_socket_type, and_raise=False, shutdown_on_error=True) as zmq_socket:
+        with exception_handler(
+            connect_url=self._source_zmq_url,
+            socket_type=self._source_socket_type,
+            and_raise=False,
+            shutdown_on_error=True,
+        ) as zmq_socket:
             while not threads.shutting_down:
                 self.process_message(zmq_socket=zmq_socket)
```

### Comparing `tailucas_pylib-0.4.0/tailucas_pylib/threads.py` & `tailucas_pylib-0.4.1/tailucas_pylib/threads.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-import cronitor
 import logging
 import signal
 import sys
 import threading
 import time
 import traceback
-
 from datetime import datetime
+
+import cronitor
 from sentry_sdk import Hub
 from zmq.error import ZMQError
 
 from .aws.metrics import post_count_metric
 from .zmq import try_close, zmq_sockets
 
-
-log = logging.getLogger(APP_NAME)  # type: ignore
+log = logging.getLogger(APP_NAME)  # type: ignore  # noqa: F821
 
 # threads to interrupt
 interruptable_sleep = threading.Event()
 # threads to nanny
 threads_tracked = set()
 # shutdown flag
 shutting_down = False
@@ -26,116 +25,126 @@
 trigger_exception = None
 
 
 def die(exception=None):
     global shutting_down
     global interruptable_sleep
     global trigger_exception
-    log.debug(f'Shutting down Sentry...')
+    log.debug("Shutting down Sentry...")
     client = Hub.current.client
     if client is not None:
         client.close(timeout=2.0)
-    log.debug(f'Shutting down application...')
+    log.debug("Shutting down application...")
     shutting_down = True
     interruptable_sleep.set()
     # enforce latch so as not to unset later due to __main__ shutdown
     if exception is not None:
         trigger_exception = exception
 
 
 def bye():
     global trigger_exception
     exit_cause = trigger_exception
     exit_code = 0
-    exit_message = f'Shutdown complete.'
+    exit_message = "Shutdown complete."
     if exit_cause is not None:
-        exit_message += f' Exception was {exit_cause!s}.'
+        exit_message += f" Exception was {exit_cause!s}."
         exit_code = 1
-    exit_message += f' Exiting with code {exit_code}.'
+    exit_message += f" Exiting with code {exit_code}."
     log.info(exit_message)
     # flush loggers
     logging.shutdown()
     # exit process
     exit(code=exit_code)
 
 
 # noinspection PyShadowingNames
 def thread_nanny(signal_handler):
     global interruptable_sleep
     global threads_tracked
     global shutting_down
-    shutting_down_grace_secs = APP_CONFIG.getint('app', 'shutting_down_grace_secs', fallback=30)  # type: ignore
+    shutting_down_grace_secs = APP_CONFIG.getint(  # noqa: F821
+        "app", "shutting_down_grace_secs", fallback=30
+    )  # type: ignore
     shutting_down_time = None
     monitor = None
-    if APP_CONFIG.has_option('app', 'cronitor_monitor_key'):  # type: ignore
-        monitor = cronitor.Monitor(APP_CONFIG.get('app', 'cronitor_monitor_key'))  # type: ignore
+    if APP_CONFIG.has_option("app", "cronitor_monitor_key"):  # type: ignore  # noqa: F821
+        monitor = cronitor.Monitor(APP_CONFIG.get("app", "cronitor_monitor_key"))  # type: ignore  # noqa: F821
     while True:
         if signal_handler.last_signal == signal.SIGTERM:
             shutting_down = True
         # take stock of running threads
         threads_alive = set()
         for thread_info in threading.enumerate():
             if thread_info.is_alive():
                 threads_alive.add(thread_info.getName())
                 # print non-daemon threads that linger
                 if shutting_down and not thread_info.daemon:
                     code = []
                     stack = sys._current_frames()[thread_info.ident]
                     for filename, lineno, name, line in traceback.extract_stack(stack):
-                        code.append('File: "%s", line %d, in %s' % (filename, lineno, name))
+                        code.append(
+                            'File: "%s", line %d, in %s' % (filename, lineno, name)
+                        )
                         if line:
                             code.append("  %s" % (line.strip()))
                     for line in code:
                         log.debug(line)
         if not shutting_down:
             thread_deficit = threads_tracked - threads_alive
-            state = 'ok'
+            state = "ok"
             if len(thread_deficit) > 0:
-                error_msg = f'A thread has died. Expected threads are [{threads_tracked}], ' \
-                            f'missing is [{thread_deficit}].'
+                error_msg = (
+                    f"A thread has died. Expected threads are [{threads_tracked}], "
+                    f"missing is [{thread_deficit}]."
+                )
                 log.warning(error_msg)
-                post_count_metric('Fatals')
+                post_count_metric("Fatals")
                 die(exception=ResourceWarning(error_msg))
-                state = 'fail'
+                state = "fail"
             elif datetime.now().minute % 5 == 0:
                 # zero every 5 minutes
-                post_count_metric('Fatals', 0)
+                post_count_metric("Fatals", 0)
             if monitor is not None:
                 try:
                     monitor.ping(
-                        host=DEVICE_NAME, # type: ignore
+                        host=DEVICE_NAME,  # type: ignore  # noqa: F821
                         state=state,
                         metrics={
-                            'count': len(threads_alive),
-                            'error_count': len(thread_deficit)
-                        }
+                            "count": len(threads_alive),
+                            "error_count": len(thread_deficit),
+                        },
                     )
                 except Exception as e:
-                    log.warning(f'Problem sending cronitor ping: {e!s}')
+                    log.warning(f"Problem sending cronitor ping: {e!s}")
             # don't block on the long sleep
             interruptable_sleep.wait(60)
         else:
             # interrupt any other sleepers now
             interruptable_sleep.set()
             now = int(time.time())
             if shutting_down_time is None:
                 shutting_down_time = now
-            if (now - shutting_down_time > shutting_down_grace_secs):
+            if now - shutting_down_time > shutting_down_grace_secs:
                 if log.level != logging.DEBUG:
-                    log.warning(f"Shutting-down duration has exceeded {shutting_down_grace_secs}s. Switching to debug logging...")
+                    log.warning(
+                        f"Shutting-down duration has exceeded {shutting_down_grace_secs}s. Switching to debug logging..."
+                    )
                     log.setLevel(logging.DEBUG)
                 # close zmq sockets that are still alive (and blocking shutdown)
                 try:
-                    for s,l in zmq_sockets.items(): # type: ignore
+                    for s, loc in zmq_sockets.items():  # type: ignore
                         try:
                             if s and not s.closed:
-                                log.warning(f'Closing lingering socket {s!r} created at {l}.')
+                                log.warning(
+                                    f"Closing lingering socket {s!r} created at {loc}."
+                                )
                                 try_close(s)
                         except ZMQError:
-                            log.debug('ZMQ error on closing socket.', exc_info=True)
+                            log.debug("ZMQ error on closing socket.", exc_info=True)
                             # not interesting in this context
                             continue
                 except RuntimeError:
                     # protect against "Set changed size during iteration", try again later
-                    log.debug('Issue on closing lingering sockets.', exc_info=True)
+                    log.debug("Issue on closing lingering sockets.", exc_info=True)
         # never spin
         time.sleep(2)
```

### Comparing `tailucas_pylib-0.4.0/tailucas_pylib/zmq.py` & `tailucas_pylib-0.4.1/tailucas_pylib/zmq.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import inspect
 import logging
-import zmq
-
 from typing import Optional
+from weakref import WeakKeyDictionary
 
-from weakref import WeakKeyDictionary, WeakSet
+import zmq
+from zmq.asyncio import Context as AsyncioContext
 from zmq.error import ZMQError
 
-log = logging.getLogger(APP_NAME)  # type: ignore
+log = logging.getLogger(APP_NAME)  # type: ignore  # noqa: F821
 
 zmq_sockets = WeakKeyDictionary()
 zmq_context = zmq.Context()
 zmq_context.setsockopt(zmq.LINGER, 0)
 # asyncio capabilities
-from zmq.asyncio import Context as AsyncioContext
+
 zmq_async_context = None
 
 
-def zmq_socket(socket_type: int, is_async: Optional[bool]=False):
+def zmq_socket(socket_type: int, is_async: Optional[bool] = False):
     call_stack = inspect.stack()
     locations = []
     for fi in call_stack:
-        locations.append(f'{fi.function} in {fi.filename} @ line {fi.lineno}')
-    location = ', '.join(locations)
-    log.debug(f'Creating {is_async=} {socket_type} ({zmq.PUSH=}, {zmq.PULL=}, {zmq.REQ=}, {zmq.REP=}) socket for location {location}...')
+        locations.append(f"{fi.function} in {fi.filename} @ line {fi.lineno}")
+    location = ", ".join(locations)
+    log.debug(
+        f"Creating {is_async=} {socket_type} ({zmq.PUSH=}, {zmq.PULL=}, {zmq.REQ=}, {zmq.REP=}) socket for location {location}..."
+    )
     if is_async:
         global zmq_async_context
         if zmq_async_context is None:
             # FIXME: https://github.com/zeromq/pyzmq/issues/940
             # FIXME: Exception in callback Socket._init_io_state.<locals>.<lambda>() on Context.term() within asyncio
             zmq_async_context = AsyncioContext.shadow(zmq_context.underlying)
             zmq_async_context.setsockopt(zmq.LINGER, 0)
@@ -35,67 +37,74 @@
     else:
         socket = zmq_context.socket(socket_type)
     zmq_sockets[socket] = location
     return socket
 
 
 def zmq_term():
-    log.info(f'Shutting down ZMQ context...')
+    log.info("Shutting down ZMQ context...")
     zmq_context.term()
     global zmq_async_context
     if zmq_async_context:
-        log.info(f'Shutting down async ZMQ context...')
+        log.info("Shutting down async ZMQ context...")
         try:
             zmq_async_context.term()
         except Exception:
-            log.debug('Error closing async ZMQ context.', exc_info=True)
-    log.info(f'ZMQ shutdown complete.')
+            log.debug("Error closing async ZMQ context.", exc_info=True)
+    log.info("ZMQ shutdown complete.")
 
 
 def try_close(socket):
     if socket is None:
         return
     try:
         try:
             location = zmq_sockets[socket]
             if location:
-                log.debug(f'Closing {socket!r} created at {location}...')
+                log.debug(f"Closing {socket!r} created at {location}...")
         except KeyError:
-            log.debug(f'Closing {socket!r}...')
+            log.debug(f"Closing {socket!r}...")
         socket.close()
     except ZMQError:
-        log.warning(f'Ignoring socket error when closing socket.', exc_info=True)
+        log.warning("Ignoring socket error when closing socket.", exc_info=True)
 
 
 class Closable(object):
-
     @property
     def socket(self):
         return self._socket
 
     @property
     def socket_type(self):
         return self._socket_type
 
     @property
     def socket_url(self):
         return self._socket_url
 
-    def __init__(self, connect_url: str, socket_type=zmq.PULL, is_async: Optional[bool]=False):
+    def __init__(
+        self, connect_url: str, socket_type=zmq.PULL, is_async: Optional[bool] = False
+    ):
         self._socket = None
         self._socket_url: str = connect_url
         self._socket_type: int = socket_type
         self._is_async: Optional[bool] = is_async
 
     def get_socket(self):
         if self._socket is None:
-            self._socket = zmq_socket(socket_type=self._socket_type, is_async=self._is_async)
+            self._socket = zmq_socket(
+                socket_type=self._socket_type, is_async=self._is_async
+            )
             if self._socket_type in [zmq.PULL, zmq.PUB, zmq.REP]:
-                log.debug(f'Binding {self._socket_type} ({zmq.PULL=}, {zmq.PUB=}, {zmq.REP=}) ZMQ socket to {self._socket_url}.')
+                log.debug(
+                    f"Binding {self._socket_type} ({zmq.PULL=}, {zmq.PUB=}, {zmq.REP=}) ZMQ socket to {self._socket_url}."
+                )
                 self._socket.bind(self._socket_url)
             else:
-                log.debug(f'Connecting {self._socket_type} ({zmq.PUSH=}, {zmq.PULL=}, {zmq.REQ=}, {zmq.REP=}) ZMQ socket to {self._socket_url}')
+                log.debug(
+                    f"Connecting {self._socket_type} ({zmq.PUSH=}, {zmq.PULL=}, {zmq.REQ=}, {zmq.REP=}) ZMQ socket to {self._socket_url}"
+                )
                 self._socket.connect(self._socket_url)
         return self._socket
 
     def close(self):
         try_close(self._socket)
```

### Comparing `tailucas_pylib-0.4.0/PKG-INFO` & `tailucas_pylib-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailucas-pylib
-Version: 0.4.0
+Version: 0.4.1
 Summary: Common Python utility modules
 License: MIT
 Author: Tai Lucas
 Author-email: tglucas@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

