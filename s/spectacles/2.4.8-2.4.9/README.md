# Comparing `tmp/spectacles-2.4.8.tar.gz` & `tmp/spectacles-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectacles-2.4.8.tar", max compression
+gzip compressed data, was "spectacles-2.4.9.tar", max compression
```

## Comparing `spectacles-2.4.8.tar` & `spectacles-2.4.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1082 2019-10-02 19:47:43.000000 spectacles-2.4.8/LICENSE
--rw-r--r--   0        0        0     3192 2022-11-21 17:52:41.756936 spectacles-2.4.8/README.md
--rw-r--r--   0        0        0     2379 2024-04-19 14:54:19.766158 spectacles-2.4.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-07 13:53:18.822598 spectacles-2.4.8/spectacles/__init__.py
--rw-r--r--   0        0        0    35199 2024-04-19 14:54:19.766988 spectacles-2.4.8/spectacles/cli.py
--rw-r--r--   0        0        0    39349 2024-04-19 14:54:19.767618 spectacles-2.4.8/spectacles/client.py
--rw-r--r--   0        0        0     5725 2024-02-07 13:53:18.824740 spectacles-2.4.8/spectacles/exceptions.py
--rw-r--r--   0        0        0     3596 2024-02-07 13:53:18.824979 spectacles-2.4.8/spectacles/logger.py
--rw-r--r--   0        0        0    18470 2024-02-07 13:53:18.825222 spectacles-2.4.8/spectacles/lookml.py
--rw-r--r--   0        0        0     3226 2024-02-07 13:53:18.825399 spectacles-2.4.8/spectacles/models.py
--rw-r--r--   0        0        0     5455 2024-02-07 13:53:18.825856 spectacles-2.4.8/spectacles/printer.py
--rw-r--r--   0        0        0     1459 2024-02-07 13:53:18.825964 spectacles-2.4.8/spectacles/project_select.py
--rw-r--r--   0        0        0        0 2022-08-26 11:43:56.097650 spectacles-2.4.8/spectacles/py.typed
--rw-r--r--   0        0        0    24833 2024-04-19 14:54:19.768200 spectacles-2.4.8/spectacles/runner.py
--rw-r--r--   0        0        0     1291 2024-02-07 13:53:18.826609 spectacles-2.4.8/spectacles/tracking.py
--rw-r--r--   0        0        0     3320 2024-02-07 13:53:18.827372 spectacles-2.4.8/spectacles/utils.py
--rw-r--r--   0        0        0      317 2024-02-07 13:53:18.827931 spectacles-2.4.8/spectacles/validators/__init__.py
--rw-r--r--   0        0        0     7269 2024-02-07 13:53:18.828465 spectacles-2.4.8/spectacles/validators/content.py
--rw-r--r--   0        0        0     4922 2024-04-19 14:54:19.769021 spectacles-2.4.8/spectacles/validators/data_test.py
--rw-r--r--   0        0        0     2407 2024-04-19 14:54:19.769506 spectacles-2.4.8/spectacles/validators/lookml.py
--rw-r--r--   0        0        0    22392 2024-02-12 16:45:14.304045 spectacles-2.4.8/spectacles/validators/sql.py
--rw-r--r--   0        0        0     4832 1970-01-01 00:00:00.000000 spectacles-2.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1082 2021-11-18 20:00:49.748916 spectacles-2.4.9/LICENSE
+-rw-r--r--   0        0        0     3192 2022-11-08 19:17:18.791087 spectacles-2.4.9/README.md
+-rw-r--r--   0        0        0     2379 2024-05-21 20:52:37.127730 spectacles-2.4.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-01 19:35:01.756973 spectacles-2.4.9/spectacles/__init__.py
+-rw-r--r--   0        0        0    35199 2024-05-16 19:55:37.199411 spectacles-2.4.9/spectacles/cli.py
+-rw-r--r--   0        0        0    42228 2024-05-21 20:52:37.128450 spectacles-2.4.9/spectacles/client.py
+-rw-r--r--   0        0        0     5725 2024-02-01 19:35:01.759196 spectacles-2.4.9/spectacles/exceptions.py
+-rw-r--r--   0        0        0     3596 2024-02-01 19:35:01.760489 spectacles-2.4.9/spectacles/logger.py
+-rw-r--r--   0        0        0    18470 2024-02-01 19:35:01.761930 spectacles-2.4.9/spectacles/lookml.py
+-rw-r--r--   0        0        0     3226 2024-02-01 19:35:01.763569 spectacles-2.4.9/spectacles/models.py
+-rw-r--r--   0        0        0     5455 2024-02-01 19:35:01.764332 spectacles-2.4.9/spectacles/printer.py
+-rw-r--r--   0        0        0     1459 2024-02-01 19:35:01.764661 spectacles-2.4.9/spectacles/project_select.py
+-rw-r--r--   0        0        0        0 2022-11-08 19:17:18.797644 spectacles-2.4.9/spectacles/py.typed
+-rw-r--r--   0        0        0    24833 2024-05-10 13:59:46.812482 spectacles-2.4.9/spectacles/runner.py
+-rw-r--r--   0        0        0     1291 2024-02-07 14:29:12.583042 spectacles-2.4.9/spectacles/tracking.py
+-rw-r--r--   0        0        0     3320 2024-02-01 19:35:01.773330 spectacles-2.4.9/spectacles/utils.py
+-rw-r--r--   0        0        0      317 2024-02-01 19:35:01.775261 spectacles-2.4.9/spectacles/validators/__init__.py
+-rw-r--r--   0        0        0     7269 2024-02-01 19:35:01.776148 spectacles-2.4.9/spectacles/validators/content.py
+-rw-r--r--   0        0        0     4922 2024-05-10 13:59:46.813148 spectacles-2.4.9/spectacles/validators/data_test.py
+-rw-r--r--   0        0        0     2407 2024-05-10 13:59:46.813705 spectacles-2.4.9/spectacles/validators/lookml.py
+-rw-r--r--   0        0        0    22392 2024-02-19 17:48:48.562889 spectacles-2.4.9/spectacles/validators/sql.py
+-rw-r--r--   0        0        0     4832 1970-01-01 00:00:00.000000 spectacles-2.4.9/PKG-INFO
```

### Comparing `spectacles-2.4.8/LICENSE` & `spectacles-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.8/README.md` & `spectacles-2.4.9/README.md`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.8/pyproject.toml` & `spectacles-2.4.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectacles"
-version = "2.4.8"
+version = "2.4.9"
 description = "A command-line, continuous integration tool for Looker and LookML."
 authors = ["Spectacles <hello@spectacles.dev>"]
 license = "MIT"
 readme = "README.md"
 keywords = [
     "Looker",
     "LookML",
```

### Comparing `spectacles-2.4.8/spectacles/cli.py` & `spectacles-2.4.9/spectacles/cli.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.8/spectacles/client.py` & `spectacles-2.4.9/spectacles/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,56 @@
 import json
 import time
 from dataclasses import dataclass
+from http import HTTPStatus
 from typing import Any, Dict, List, Optional, Tuple
 
 import backoff
 import httpx
 from aiocache import Cache, cached, serializers
-from httpx import ConnectError, HTTPStatusError, RemoteProtocolError, TimeoutException
+from httpx import HTTPStatusError, NetworkError, RemoteProtocolError, TimeoutException
 
 import spectacles.utils as utils
 from spectacles.exceptions import LookerApiError, SpectaclesException
 from spectacles.logger import GLOBAL_LOGGER as logger
 from spectacles.models import JsonDict
 
 DEFAULT_API_VERSION = 4.0
 TIMEOUT_SEC = 300
 LOOKML_VALIDATION_TIMEOUT = 7200
 MAX_ASYNC_CONNECTIONS = 200
-DEFAULT_MAX_TRIES = 3
-BACKOFF_EXCEPTIONS = (
+
+DEFAULT_RETRIES = 3
+DEFAULT_NETWORK_RETRIES = 10
+NETWORK_EXCEPTIONS = (
+    NetworkError,
     TimeoutException,
+    RemoteProtocolError,
+)
+STATUS_EXCEPTIONS = (
     HTTPStatusError,
-    ConnectError,
     LookerApiError,
-    RemoteProtocolError,
 )
+BACKOFF_EXCEPTIONS = NETWORK_EXCEPTIONS + STATUS_EXCEPTIONS
+
+
+def giveup_unless_bad_gateway(exception: Exception) -> bool:
+    """Give up retries if a status error encountered with any code besides 502/504."""
+    if isinstance(exception, LookerApiError):
+        return exception.status not in (
+            HTTPStatus.BAD_GATEWAY,
+            HTTPStatus.GATEWAY_TIMEOUT,
+        )
+    elif isinstance(exception, HTTPStatusError):
+        return exception.response.status_code not in (
+            HTTPStatus.BAD_GATEWAY,
+            HTTPStatus.GATEWAY_TIMEOUT,
+        )
+    else:
+        return False
 
 
 @dataclass(frozen=True)  # Token is immutable
 class AccessToken:
     access_token: str
     token_type: str
     expires_in: int
@@ -166,15 +188,20 @@
 
     async def put(self, url: str, *args: Any, **kwargs: Any) -> httpx.Response:
         return await self.request("PUT", url, *args, **kwargs)
 
     async def delete(self, url: str, *args: Any, **kwargs: Any) -> httpx.Response:
         return await self.request("DELETE", url, *args, **kwargs)
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     def get_looker_release_version(self) -> str:
         """Gets the version number of connected Looker instance.
 
         Returns:
             str: Looker instance release version number (e.g. 6.22.12)
 
         """
@@ -197,15 +224,20 @@
                     "Please try again."
                 ),
                 response=response,
             ) from error
 
         return response.json()["looker_release_version"]  # type: ignore[no-any-return]
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def get_workspace(self) -> str:
         """Gets the session workspace.
 
         Args:
             project: Name of the Looker project to use.
 
         Returns:
@@ -225,15 +257,20 @@
                     "Unable to get the workspace in use by this session. "
                     "Please try again."
                 ),
                 response=response,
             ) from error
         return response.json()["workspace_id"]  # type: ignore[no-any-return]
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def update_workspace(self, workspace: str) -> None:
         """Updates the session workspace.
 
         Args:
             workspace: The workspace to switch to, either 'production' or 'dev'
         """
         logger.debug(f"Updating session to use the {workspace} workspace")
@@ -253,15 +290,20 @@
                     "checked out by the user whose API credentials "
                     "Spectacles is using, please save it and try again."
                 ),
                 response=response,
             ) from error
         self.workspace = workspace
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def get_all_branches(self, project: str) -> List[JsonDict]:
         """Returns a list of git branches in the project repository.
 
         Args:
             project: Name of the Looker project to use.
         """
         logger.debug(f"Getting all Git branches in project '{project}'")
@@ -281,15 +323,20 @@
                     "Please try again."
                 ),
                 response=response,
             ) from error
 
         return response.json()  # type: ignore[no-any-return]
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def checkout_branch(self, project: str, branch: str) -> None:
         """Checks out a new git branch. Only works in dev workspace.
 
         Args:
             project: Name of the Looker project to use.
             branch: Name of the Git branch to check out.
         """
@@ -308,15 +355,20 @@
                     f"Unable to checkout Git branch '{branch}'. "
                     "If you have uncommitted changes on the current branch, "
                     "please commit or revert them, then try again."
                 ),
                 response=response,
             ) from error
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def reset_to_remote(self, project: str) -> None:
         """Reset a project development branch to the revision of the project that is on the remote.
 
         Args:
             project: Name of the Looker project to use.
 
         """
@@ -335,14 +387,20 @@
                 detail=(
                     "Unable to reset local Git branch "
                     "to match remote. Please try again."
                 ),
                 response=response,
             ) from error
 
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def get_manifest(self, project: str) -> JsonDict:
         """Gets all the dependent LookML projects defined in the manifest file.
 
         Args:
             project: Name of the Looker project to use.
 
         Returns:
@@ -367,15 +425,20 @@
                 response=response,
             ) from error
 
         manifest = response.json()
 
         return manifest  # type: ignore[no-any-return]
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def get_active_branch(self, project: str) -> JsonDict:
         """Gets the active branch for the user in the given project.
 
         Args:
             project: Name of the Looker project to use.
 
         Returns:
@@ -401,21 +464,31 @@
             ) from error
 
         branch_name = response.json()["name"]
         logger.debug(f"The active branch is '{branch_name}'")
 
         return response.json()  # type: ignore[no-any-return]
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def get_active_branch_name(self, project: str) -> str:
         """Helper method to return only the branch name."""
         full_response = await self.get_active_branch(project)
         return full_response["name"]  # type: ignore[no-any-return]
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def create_branch(
         self, project: str, branch: str, ref: Optional[str] = None
     ) -> None:
         """Creates a branch in the given project.
 
         Args:
             project: Name of the Looker project to use.
@@ -451,15 +524,20 @@
                 name="unable-to-create-branch",
                 title="Couldn't create new Git branch.",
                 status=response.status_code,
                 detail=detail,
                 response=response,
             ) from error
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def hard_reset_branch(self, project: str, branch: str, ref: str) -> None:
         """Hard resets a branch to the ref prodvided.
 
         DANGER: hard reset will be force pushed to the remote. Unsaved changes and
             commits may be permanently lost.
 
         Args:
@@ -486,15 +564,20 @@
                     f"Unable to update branch '{branch}' "
                     f"in project '{project}' using ref '{ref}'. "
                     "Please try again."
                 ),
                 response=response,
             ) from error
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def delete_branch(self, project: str, branch: str) -> None:
         """Deletes a branch in the given project.
 
         Args:
             project: Name of the Looker project to use.
             branch: Name of the branch to delete.
         """
@@ -515,15 +598,20 @@
                 detail=(
                     f"Unable to delete branch '{branch}' "
                     f"in project '{project}'. Please try again."
                 ),
                 response=response,
             ) from error
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def all_lookml_tests(self, project: str) -> List[JsonDict]:
         """Gets all LookML/data tests for a given project.
 
         Args:
             project: Name of the Looker project to use
 
         Returns:
@@ -548,15 +636,20 @@
                     f"project '{project}'. Please try again."
                 ),
                 response=response,
             ) from error
 
         return response.json()  # type: ignore[no-any-return]
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def run_lookml_test(
         self, project: str, model: Optional[str] = None, test: Optional[str] = None
     ) -> List[JsonDict]:
         """Runs all LookML/data tests for a given project and model (optional)
 
         This command only runs tests in production, as the Looker API doesn't currently
         allow us to run data tests on a specific branch.
@@ -605,15 +698,20 @@
                     f"project '{project}'. Please try again."
                 ),
                 response=response,
             ) from error
 
         return response.json()  # type: ignore[no-any-return]
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def get_lookml_models(
         self, fields: Optional[List[str]] = None
     ) -> List[JsonDict]:
         """Gets all models and explores from the LookmlModel endpoint.
 
         Returns:
             List[JsonDict]: JSON response containing LookML models and explores.
@@ -638,15 +736,20 @@
                 status=response.status_code,
                 detail="Unable to retrieve LookML details. Please try again.",
                 response=response,
             ) from error
 
         return response.json()  # type: ignore[no-any-return]
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def get_lookml_dimensions(
         self, model: str, explore: str
     ) -> List[Dict[str, Any]]:
         """Gets all dimensions for an explore from the LookmlModel endpoint."""
         logger.debug(f"Getting all dimensions from explore {model}/{explore}")
         params = {"fields": ["fields"]}
         url = utils.compose_url(
@@ -668,15 +771,20 @@
                 ),
                 response=response,
             ) from error
 
         return response.json()["fields"]["dimensions"]  # type: ignore[no-any-return]
 
     @cached(cache=Cache.MEMORY, serializer=serializers.PickleSerializer())  # type: ignore
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=5)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def create_query(
         self,
         model: str,
         explore: str,
         dimensions: List[str],
         fields: Optional[List[str]] = None,
     ) -> JsonDict:
@@ -734,15 +842,20 @@
             model,
             explore,
             "*" if len(dimensions) != 1 else dimensions[0],
             query_id,
         )
         return result  # type: ignore[no-any-return]
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=5)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def create_query_task(self, query_id: str) -> str:
         """Runs a previously created query asynchronously and returns the query task ID.
 
         If a ClientError or TimeoutError is received, attempts to retry.
 
         Args:
             session: Existing asychronous HTTP session.
@@ -778,15 +891,20 @@
             ) from error
 
         result = response.json()
         query_task_id = result["id"]
         logger.debug("Query %s is running under query task %s", query_id, query_task_id)
         return query_task_id  # type: ignore[no-any-return]
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def get_query_task_multi_results(
         self, query_task_ids: Tuple[str, ...]
     ) -> JsonDict:
         """Returns query task results.
 
         If a ClientError or TimeoutError is received, attempts to retry.
 
@@ -822,15 +940,20 @@
                 ),
                 response=response,
             ) from error
 
         result = response.json()
         return result  # type: ignore[no-any-return]
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def cancel_query_task(self, query_task_id: str) -> None:
         """Cancels a query task.
 
         Args:
             query_task_id: ID for the query task to cancel.
 
         """
@@ -858,15 +981,21 @@
                 detail=("Failed to run the content validator. Please try again."),
                 response=response,
             ) from error
 
         result = response.json()
         return result  # type: ignore[no-any-return]
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        # Omit retries on timeouts because timeout is already very long
+        STATUS_EXCEPTIONS + (NetworkError,),
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def lookml_validation(
         self, project: str, timeout: int = LOOKML_VALIDATION_TIMEOUT
     ) -> JsonDict:
         logger.debug(
             f"Validating LookML for project '{project}' with timeout {timeout} seconds."
         )
         url = utils.compose_url(self.api_url, path=["projects", project, "validate"])
@@ -882,15 +1011,21 @@
                 detail=("Failed to run the LookML validator. Please try again."),
                 response=response,
             ) from error
 
         result = response.json()
         return result  # type: ignore[no-any-return]
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        # Omit retries on timeouts because timeout is already very long
+        STATUS_EXCEPTIONS + (NetworkError,),
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def cached_lookml_validation(self, project: str) -> Optional[JsonDict]:
         logger.debug(f"Getting cached LookML validation results for '{project}'")
         url = utils.compose_url(self.api_url, path=["projects", project, "validate"])
         response = await self.get(url=url, timeout=1800)
 
         try:
             response.raise_for_status()
@@ -910,15 +1045,20 @@
         if response.status_code == 204:
             return None
 
         result = response.json()
         return result  # type: ignore[no-any-return]
 
     @cached(cache=Cache.MEMORY, serializer=serializers.PickleSerializer())  # type: ignore
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def all_folders(self) -> List[JsonDict]:
         logger.debug("Getting information about all folders")
         url = utils.compose_url(self.api_url, path=["folders"])
         response = await self.get(url=url, timeout=TIMEOUT_SEC)
 
         try:
             response.raise_for_status()
@@ -930,15 +1070,20 @@
                 detail=("Failed to get all folders."),
                 response=response,
             ) from error
 
         result = response.json()
         return result  # type: ignore[no-any-return]
 
-    @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
+    @backoff.on_exception(
+        backoff.expo,
+        BACKOFF_EXCEPTIONS,
+        giveup=giveup_unless_bad_gateway,
+        max_tries=DEFAULT_NETWORK_RETRIES,
+    )
     async def run_query(
         self, query_id: str, explore: str, model: str, dimension: Optional[str] = None
     ) -> str:
         """Returns the compiled SQL for a given query ID.
 
         The corresponding Looker API endpoint allows us to run queries with a variety
         of result formats, however we only use the `sql` result format, which doesn't
```

### Comparing `spectacles-2.4.8/spectacles/exceptions.py` & `spectacles-2.4.9/spectacles/exceptions.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.8/spectacles/logger.py` & `spectacles-2.4.9/spectacles/logger.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.8/spectacles/lookml.py` & `spectacles-2.4.9/spectacles/lookml.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.8/spectacles/models.py` & `spectacles-2.4.9/spectacles/models.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.8/spectacles/printer.py` & `spectacles-2.4.9/spectacles/printer.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.8/spectacles/project_select.py` & `spectacles-2.4.9/spectacles/project_select.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.8/spectacles/runner.py` & `spectacles-2.4.9/spectacles/runner.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.8/spectacles/tracking.py` & `spectacles-2.4.9/spectacles/tracking.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.8/spectacles/utils.py` & `spectacles-2.4.9/spectacles/utils.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.8/spectacles/validators/content.py` & `spectacles-2.4.9/spectacles/validators/content.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.8/spectacles/validators/data_test.py` & `spectacles-2.4.9/spectacles/validators/data_test.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.8/spectacles/validators/lookml.py` & `spectacles-2.4.9/spectacles/validators/lookml.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.8/spectacles/validators/sql.py` & `spectacles-2.4.9/spectacles/validators/sql.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.8/PKG-INFO` & `spectacles-2.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectacles
-Version: 2.4.8
+Version: 2.4.9
 Summary: A command-line, continuous integration tool for Looker and LookML.
 License: MIT
 Keywords: Looker,LookML,CI,continuous integration,testing,validation
 Author: Spectacles
 Author-email: hello@spectacles.dev
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

