# Comparing `tmp/openai_priority_loadbalancer-1.0.7.tar.gz` & `tmp/openai_priority_loadbalancer-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_priority_loadbalancer-1.0.7.tar", last modified: Fri May 17 23:45:20 2024, max compression
+gzip compressed data, was "openai_priority_loadbalancer-1.0.8.tar", last modified: Tue May 21 16:17:33 2024, max compression
```

## Comparing `openai_priority_loadbalancer-1.0.7.tar` & `openai_priority_loadbalancer-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 23:45:20.849080 openai_priority_loadbalancer-1.0.7/
--rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-1.0.7/LICENSE
--rw-rw-rw-   0        0        0    13852 2024-05-17 10:36:38.000000 openai_priority_loadbalancer-1.0.7/PACKAGE_README.md
--rw-rw-rw-   0        0        0    14716 2024-05-17 23:45:20.846751 openai_priority_loadbalancer-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    12246 2024-05-17 10:37:02.000000 openai_priority_loadbalancer-1.0.7/README.md
--rw-rw-rw-   0        0        0      701 2024-05-17 23:43:58.000000 openai_priority_loadbalancer-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 23:45:20.850087 openai_priority_loadbalancer-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 23:45:20.769762 openai_priority_loadbalancer-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 23:45:20.785619 openai_priority_loadbalancer-1.0.7/src/openai_priority_loadbalancer/
--rw-rw-rw-   0        0        0       45 2024-05-14 20:10:13.000000 openai_priority_loadbalancer-1.0.7/src/openai_priority_loadbalancer/__init__.py
--rw-rw-rw-   0        0        0    13757 2024-05-17 23:43:26.000000 openai_priority_loadbalancer-1.0.7/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py
-drwxrwxrwx   0        0        0        0 2024-05-17 23:45:20.843738 openai_priority_loadbalancer-1.0.7/src/openai_priority_loadbalancer.egg-info/
--rw-rw-rw-   0        0        0    14716 2024-05-17 23:45:20.000000 openai_priority_loadbalancer-1.0.7/src/openai_priority_loadbalancer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2024-05-17 23:45:20.000000 openai_priority_loadbalancer-1.0.7/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 23:45:20.000000 openai_priority_loadbalancer-1.0.7/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-17 23:45:20.000000 openai_priority_loadbalancer-1.0.7/src/openai_priority_loadbalancer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-05-17 23:45:20.000000 openai_priority_loadbalancer-1.0.7/src/openai_priority_loadbalancer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 16:17:33.406986 openai_priority_loadbalancer-1.0.8/
+-rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0    13852 2024-05-17 10:36:38.000000 openai_priority_loadbalancer-1.0.8/PACKAGE_README.md
+-rw-rw-rw-   0        0        0    14716 2024-05-21 16:17:33.400874 openai_priority_loadbalancer-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    12849 2024-05-21 16:03:56.000000 openai_priority_loadbalancer-1.0.8/README.md
+-rw-rw-rw-   0        0        0      724 2024-05-21 16:08:10.000000 openai_priority_loadbalancer-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 16:17:33.407849 openai_priority_loadbalancer-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 16:17:33.287318 openai_priority_loadbalancer-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 16:17:33.315135 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer/
+-rw-rw-rw-   0        0        0       45 2024-05-14 20:10:13.000000 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer/__init__.py
+-rw-rw-rw-   0        0        0    13344 2024-05-21 15:51:47.000000 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:17:33.397151 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer.egg-info/
+-rw-rw-rw-   0        0        0    14716 2024-05-21 16:17:33.000000 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2024-05-21 16:17:33.000000 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 16:17:33.000000 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-21 16:17:33.000000 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-21 16:17:33.000000 openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer.egg-info/top_level.txt
```

### Comparing `openai_priority_loadbalancer-1.0.7/LICENSE` & `openai_priority_loadbalancer-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_priority_loadbalancer-1.0.7/PACKAGE_README.md` & `openai_priority_loadbalancer-1.0.8/PACKAGE_README.md`

 * *Files identical despite different names*

### Comparing `openai_priority_loadbalancer-1.0.7/PKG-INFO` & `openai_priority_loadbalancer-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 1.0.7
+Version: 1.0.8
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai_priority_loadbalancer-1.0.7/README.md` & `openai_priority_loadbalancer-1.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,24 @@
     *Missing this step may result in HTTP 400 errors for a tenant mismatch.*
 
 ## Execution
 
 1. Initially, [python-aoai.ps1](./python-aoai.ps1) once to ensure it executes correctly.
 1. Run [python-aoai.ps1](./python-aoai.ps1) concurrently in multiple terminals to simulate parallel requests from multiple python workers.
 
+## Testing
+
+OpenAI Priority Load Balancer uses `pytest` and `coverage`. The test files can be found in the `tests\lib` directory. Executing `pytest -v` from the root will show test results. Note that these are rudimentary tests still and in the process of being built out further.
+
+To obtain coverage, execute `coverage run -m pytest -v` from the root. This generates a *.coverage* file. Then run `coverage report -m` or, for a nicer presentation, `coverage html`.
+
+Details on `coverage` can be found [here](https://coverage.readthedocs.io/).
+
+Pull requests for improvements are very much appreciated!
+
 ## Distribution of Requests
 
 ### Across Different Priorities
 
 Requests are made to the highest priority backend that is available. For example:
 
 - Priority 1, when available, will always supersede priority 2.
```

### Comparing `openai_priority_loadbalancer-1.0.7/pyproject.toml` & `openai_priority_loadbalancer-1.0.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-[project]
-name = "openai_priority_loadbalancer"
-version = "1.0.7"
-authors = [
-  { name="Simon Kurtz", email="simonkurtz@gmail.com" },
-]
-description = "A multi-backend, prioritization load balancer for OpenAI"
-readme = "PACKAGE_README.md"
-requires-python = ">=3.8"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-    "httpx"
-]
-[project.urls]
-Homepage = "https://github.com/simonkurtz-MSFT/python-openai-loadbalancer"
-Issues = "https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues"
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+[project]
+name = "openai_priority_loadbalancer"
+version = "1.0.8"
+authors = [
+  { name="Simon Kurtz", email="simonkurtz@gmail.com" },
+]
+description = "A multi-backend, prioritization load balancer for OpenAI"
+readme = "PACKAGE_README.md"
+requires-python = ">=3.8"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+    "httpx"
+]
+[project.urls]
+Homepage = "https://github.com/simonkurtz-MSFT/python-openai-loadbalancer"
+Issues = "https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
```

### Comparing `openai_priority_loadbalancer-1.0.7/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py` & `openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,268 +1,256 @@
-"""Module providing a prioritized load-balancing for Azure OpenAI."""
-
-import logging
-import random
-import traceback
-from typing import List
-from datetime import datetime, MAXYEAR, MINYEAR, timedelta, timezone
-import httpx    # import the entirety of the httpx module to avoid potential conflicts with AsyncClient in the openai package by using httpx. notation
-
-class Backend:
-    """Class representing a backend object used with Azure OpenAI, etc."""
-
-    # Constructor
-    def __init__(self, host: str, priority: int):
-        # Public instance variables
-        self.host = host
-        self.is_throttling = False
-        self.priority = priority
-        self.retry_after = datetime.min
-        self.successful_call_count = 0
-
-# Reference design at https://github.com/encode/httpx/blob/master/httpx/_transports/base.py
-# BaseLoadBalancer providing functionality to both synchronous and asynchronous load balancers
-class BaseLoadBalancer():
-    """Logically abstracts the BaseLoadBalancer class which should be inherited by the synchronous and asynchronous load balancer classes."""
-
-    # Constructor
-    def __init__(self, transport, backends: List[Backend]):
-        # Public instance variables
-        self.backends = backends
-
-        # "Private" instance variables
-        self._backend_index = -1
-        self._log = logging.getLogger("openai-priority-loadbalancer")     # https://www.loggly.com/ultimate-guide/python-logging-basics/
-        self._available_backends = 1
-        self._transport = transport
-
-    # "Protected" Methods
-    def _check_throttling(self):
-        """Check if any backend is throttling and reset if necessary."""
-
-        min_datetime = datetime(MINYEAR, 1, 1, tzinfo = timezone.utc)
-
-        for backend in self.backends:
-            if backend.is_throttling and datetime.now(timezone.utc) >= backend.retry_after:
-                backend.is_throttling = False
-                backend.retry_after = min_datetime
-                self._log.info("Backend %s is no longer throttling.", backend.host)
-
-    def _get_backend_index(self):
-        """Return a backend list index of a highest-priority available backend to be used. If no backend is available, -1 will be returned."""
-
-        selected_priority = float('inf')
-        available_backends = []
-
-        # 1) Evaluate all defined backends for availability and priority, leaving only the highest-priority available backends from which to select an index.
-        for i, backend in enumerate(self.backends):
-            if not backend.is_throttling:
-                backend_priority = backend.priority
-
-                # If a backend has a (logically) higher priority (1 would be logically higher than 2, etc.), we select that priority, clear the available backends list
-                # which contains lower-priority backends, then add the higher-priority backend(s) to the list.
-                if backend_priority < selected_priority:
-                    selected_priority = backend_priority
-                    available_backends.clear()
-                    available_backends.append(i)
-                elif backend_priority == selected_priority:
-                    available_backends.append(i)
-
-        # 2) Select an available backend index. If there is only one available backend, it will be selected. If there are multiple available backends, one will be randomly selected. If there are none, we return -1.
-        if len(available_backends) == 1:
-            return available_backends[0]
-
-        if len(available_backends) > 0:
-            # Since this code is very likely being called from multiple python instances with multiple workers in parallel executions, there's no way to distribute requests
-            # uniformly across all Azure OpenAI instances.
-            # Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would also imply a locking mechanism for updates, which would
-            # immediately inhibit the performance benefits of the load balancer. This is why this is more of a pseudo load-balancer. Therefore, we'll just randomize across the available backends.
-            return random.choice(available_backends)
-
-        # If there are no available backends, -1 will be returned to indicate that nothing is available (and that we consequently need to bail by returning an HTTP 429).
-        return -1
-
-    def _get_available_backends(self):
-        """Return the backends that are not actively throttled. This subset is the set of available backends."""
-
-        self._available_backends = 0
-
-        for backend in self.backends:
-            if not backend.is_throttling:
-                self._available_backends += 1
-
-        self._log.info("Available backends: %s/%s", self._available_backends, len(self.backends))
-
-        return self._available_backends
-
-    def _get_soonest_retry_after(self):
-        """Return the soonest retry-after time in seconds among all throttling backends. This provides for the quickest retry time to be returned with the HTTP 429."""
-
-        soonest_retry_after = datetime(MAXYEAR, 1, 1, tzinfo = timezone.utc)
-
-        for backend in self.backends:
-            if backend.is_throttling and backend.retry_after < soonest_retry_after:
-                soonest_retry_after = backend.retry_after
-                soonest_backend = backend.host
-
-        # As the `int` cast truncates the decimal, we need to add 1 to the result to ensure that the delay is at least the number of seconds needed.
-        delay = int((soonest_retry_after - datetime.now(timezone.utc)).total_seconds()) + 1
-        self._log.info("The soonest retry to an available backend would be to %s after %s %s.", soonest_backend, delay, "second" if delay == 1 else "seconds")
-
-        return delay
-
-    def _handle_200_399_response(self, request, response, backend_index):
-        """Handle a successful response from the backend."""
-
-        self._log.info("Request sent to server: %s, Status code: %s", request.url, response.status_code)
-        self.backends[backend_index].successful_call_count += 1
-
-        return response
-
-    def _handle_429_5xx_response(self, request, response, backend_index):
-        """Handle a 429 or 5xx response from the backend by identifying the retry-after interval, if available, and updating the available backends."""
-
-        self._log.info("Request sent to server: %s, Status code: %s - FAIL", request.url, response.status_code)
-
-        # 1) Determine the retry-after interval, if possible; otherwise, assign -1 to indicate that no delay is needed.
-        retry_after = int(response.headers.get('Retry-After', '-1'))
-
-        if retry_after == -1:
-            retry_after = int(response.headers.get('x-ratelimit-reset-requests', '-1'))
-
-        if retry_after == -1:
-            retry_after = int(response.headers.get('x-ratelimit-reset-requests', '10'))
-
-        self._log.info("Backend %s is throttling. Retry after %s %s.", self.backends[backend_index].host, retry_after, "second" if retry_after == 1 else "seconds")
-
-        # 2) Regardless of whether the response indicates a 429 or 5xx error, we mark the backend as throttling to temporarily take it out of the available backend pool.
-        backend = self.backends[backend_index]
-        backend.is_throttling = True
-        backend.retry_after = datetime.now(timezone.utc) + timedelta(seconds = retry_after)
-
-        # 3) Update the available backends.
-        self._get_available_backends()
-
-    def _handle_4xx_response(self, request, response):
-        """Handle a 4xx response other than 429 from the backend."""
-
-        self._log.warning("Request sent to server: %s, Status code: %s - FAIL", request.url, response.status_code)
-
-        return response
-
-    def _modify_request(self, request, backend_index):
-        """Modifies the URL and Host header with the desired backend target. This ensures that the request is sent to the chosen backend server."""
-
-        # Modify the request. Note that only the URL and Host header are being modified on the original request object. We make the smallest incision possible to avoid side effects.
-        # Update URL and host header as both must match the backend server.
-        request.url = request.url.copy_with(host = self.backends[backend_index].host)
-        request.headers = request.headers.copy()    # We need to create a mutable copy of the headers before we modify and assign them back to the request object.
-        request.headers['host'] = self.backends[backend_index].host
-
-    def _return_429(self):
-        """Return an HTTP 429 response with a Retry-After header value. This is returned to the caller of this load balancer when no backends are available."""
-
-        self._log.warning("No backend available!")
-        retry_after = str(self._get_soonest_retry_after())
-        self._log.info("Returning HTTP 429 with Retry-After header value of %s %s.", retry_after, "second" if retry_after == "1" else "seconds")
-
-        return httpx.Response(429, content = '', headers={'Retry-After': retry_after})
-
-class AsyncLoadBalancer(BaseLoadBalancer):
-    """Asynchronous Load Balancer class based on BaseLoadBalancer"""
-
-    # Constructor
-    def __init__(self, backends: List[Backend]):
-        super().__init__(httpx.AsyncClient(), backends)
-
-    # Public Methods
-    async def handle_async_request(self, request):
-        """Handles an asynchronous request by issuing an asynchronous request to an available backed."""
-
-        self._log.info("Intercepted and now handling an asynchronous request.")
-
-        # Identify whether any backend is throttling and reset if necessary, then update the remaning available backends prior to any request handling.
-        self._check_throttling()
-        self._get_available_backends()
-        response = None
-
-        while self._available_backends > 0:
-            # 1) Determine the appropriate backend to use
-            backend_index = self._get_backend_index()
-
-            if backend_index == -1:
-                return self._return_429()
-
-            # 2) Modify the intercepted request
-            self._modify_request(request, backend_index)
-
-            # 3) Send the request to the selected backend (via async)
-            try:
-                response = await self._transport.send(request)
-            except Exception:
-                self._log.error(traceback.print_exc())
-
-            # 4) Evaluate the response from the backend:
-            #    If 429 or a 5xx error, we continue the loop and retry with another backend, if available.
-            #    If 200-399, we return the successful response.
-            #    If any other 4xx error, we break the loop and return the response as we don't explicitly handle these client errors.
-            if response is not None and (response.status_code == 429 or response.status_code >= 500):
-                self._handle_429_5xx_response(request, response, backend_index)
-                continue
-
-            if response is not None and (response.status_code >= 200 and response.status_code <= 399):
-                return self._handle_200_399_response(request, response, backend_index)
-
-            return self._handle_4xx_response(request, response)
-
-        # Since no backends are available, we must return a 429.
-        return self._return_429()
-
-class LoadBalancer(BaseLoadBalancer):
-    """Synchronous Load Balancer class based on BaseLoadBalancer"""
-
-    # Constructor
-    def __init__(self, backends: List[Backend]):
-        super().__init__(httpx.Client(), backends)
-
-    # Public Methods
-    def handle_request(self, request):
-        """Handles a synchronous request by issuing a request to an available backed."""
-
-        self._log.info("Intercepted and now handling a synchronous request.")
-
-        # Identify whether any backend is throttling and reset if necessary, then update the remaning available backends prior to any request handling.
-        self._check_throttling()
-        self._get_available_backends()
-        response = None
-
-        while self._available_backends > 0:
-            # 1) Determine the appropriate backend to use
-            backend_index = self._get_backend_index()
-
-            if backend_index == -1:
-                return self._return_429()
-
-            # 2) Modify the intercepted request
-            self._modify_request(request, backend_index)
-
-            # 3) Send the request to the selected backend
-            try:
-                response = self._transport.send(request)
-            except Exception:
-                self._log.error(traceback.print_exc())
-
-            # 4) Evaluate the response from the backend:
-            #    If 429 or a 5xx error, we continue the loop and retry with another backend, if available.
-            #    If 200-399, we return the successful response.
-            #    If any other 4xx error, we break the loop and return the response as we don't explicitly handle these client errors.
-            if response is not None and (response.status_code == 429 or response.status_code >= 500):
-                self._handle_429_5xx_response(request, response, backend_index)
-                continue
-
-            if response is not None and (response.status_code >= 200 and response.status_code <= 399):
-                return self._handle_200_399_response(request, response, backend_index)
-
-            return self._handle_4xx_response(request, response)
-
-        # Since no backends are available, we must return a 429.
-        return self._return_429()
+"""Module providing a prioritized load-balancing for Azure OpenAI."""
+
+# Python Standard Library
+import logging
+import random
+from typing import List
+from datetime import datetime, MAXYEAR, MINYEAR, timedelta, timezone
+
+# Third-Party Libraries
+import httpx    # import the entirety of the httpx module to avoid potential conflicts with AsyncClient in the openai package by using httpx. notation
+
+class Backend:
+    """Class representing a backend object used with Azure OpenAI, etc."""
+
+    # Constructor
+    def __init__(self, host: str, priority: int):
+        # Public instance variables
+        self.host = host
+        self.is_throttling = False
+        self.priority = priority
+        self.retry_after = datetime.min
+        self.successful_call_count = 0
+
+# Reference design at https://github.com/encode/httpx/blob/master/httpx/_transports/base.py
+# BaseLoadBalancer providing functionality to both synchronous and asynchronous load balancers
+class BaseLoadBalancer():
+    """Logically abstracts the BaseLoadBalancer class which should be inherited by the synchronous and asynchronous load balancer classes."""
+
+    # Constructor
+    def __init__(self, transport, backends: List[Backend]):
+        # Public instance variables
+        self.backends = backends
+
+        # "Private" instance variables
+        self._backend_index = -1
+        self._log = logging.getLogger("openai-priority-loadbalancer")     # https://www.loggly.com/ultimate-guide/python-logging-basics/
+        self._available_backends = 1
+        self._transport = transport
+
+    # "Protected" Methods
+    def _check_throttling(self) -> None:
+        """Check if any backend is throttling and reset if necessary."""
+
+        min_datetime = datetime(MINYEAR, 1, 1, tzinfo = timezone.utc)
+
+        for backend in self.backends:
+            if backend.is_throttling and datetime.now(timezone.utc) >= backend.retry_after:
+                backend.is_throttling = False
+                backend.retry_after = min_datetime
+                self._log.info("Backend %s is no longer throttling.", backend.host)
+
+    def _get_backend_index(self) -> int:
+        """Return a backend list index of a highest-priority available backend to be used. If no backend is available, -1 will be returned."""
+
+        selected_priority = float('inf')
+        available_backends: List[int] = []      # This is a list of indices of available backends
+        index = -1
+
+        # 1) Evaluate all defined backends for availability and priority, leaving only the highest-priority available backends from which to select an index.
+        for i, backend in enumerate(self.backends):
+            if not backend.is_throttling:
+                backend_priority = backend.priority
+
+                # If a backend has a (logically) higher priority (1 would be logically higher than 2, etc.), we select that priority, clear the available
+                # backends index list which contains lower-priority backend indices thus far, then add the higher-priority backend(s) index to the list.
+                if backend_priority < selected_priority:
+                    selected_priority = backend_priority
+                    available_backends.clear()
+                    available_backends.append(i)
+                elif backend_priority == selected_priority:
+                    available_backends.append(i)
+
+        # 2) Out of the available backends indices, select a random index to use.
+        if len(available_backends) > 0:
+            # Since this code is very likely being called from multiple python instances with multiple workers in parallel executions, there's no way to distribute requests
+            # uniformly across all Azure OpenAI instances. Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would
+            # also imply a locking mechanism for updates, which would immediately inhibit the performance benefits of the load balancer. This is why this is more of a
+            # pseudo load-balancer. Therefore, we'll just randomize across the available backends.
+            index = random.choice(available_backends)
+
+        # If there are no available backends, None will be returned to indicate that nothing is available (and that we consequently need to bail by returning an HTTP 429).
+        return index
+
+    def _get_available_backends(self) -> int:
+        """Return the count of backends that are not actively throttled."""
+
+        self._available_backends = 0
+
+        for backend in self.backends:
+            if not backend.is_throttling:
+                self._available_backends += 1
+
+        self._log.info("Available backends: %s/%s", self._available_backends, len(self.backends))
+
+        return self._available_backends
+
+    def _get_soonest_retry_after(self) -> int:
+        """Return the soonest retry-after time in seconds among all throttling backends. This provides for the quickest retry time to be returned with the HTTP 429."""
+
+        soonest_retry_after = datetime(MAXYEAR, 1, 1, tzinfo = timezone.utc)
+
+        for backend in self.backends:
+            if backend.is_throttling and backend.retry_after < soonest_retry_after:
+                soonest_retry_after = backend.retry_after
+                soonest_backend = backend.host
+
+        # As the `int` cast truncates the decimal, we need to add 1 to the result to ensure that the delay is at least the number of seconds needed.
+        delay = int((soonest_retry_after - datetime.now(timezone.utc)).total_seconds()) + 1
+        self._log.info("The soonest retry to an available backend would be to %s after %s %s.", soonest_backend, delay, "second" if delay == 1 else "seconds")
+
+        return delay
+
+    def _handle_200_399_response(self, request, response, backend_index) -> httpx.Response:
+        """Handle a successful response from the backend."""
+
+        self._log.info("Request sent to server: %s, Status code: %s", request.url, response.status_code)
+        self.backends[backend_index].successful_call_count += 1
+
+        return response
+
+    def _handle_429_5xx_response(self, request, response, backend_index) -> None:
+        """Handle a 429 or 5xx response from the backend by identifying the retry-after interval, if available, and updating the available backends."""
+
+        self._log.info("Request sent to server: %s, Status code: %s - FAIL", request.url, response.status_code)
+
+        # 1) Determine the retry-after interval, if possible; otherwise, assign -1 to indicate that no delay is needed.
+        retry_after = int(response.headers.get('Retry-After', '-1'))
+
+        if retry_after == -1:
+            retry_after = int(response.headers.get('x-ratelimit-reset-requests', '-1'))
+
+        if retry_after == -1:
+            retry_after = int(response.headers.get('x-ratelimit-reset-requests', '10'))
+
+        self._log.info("Backend %s is throttling. Retry after %s %s.", self.backends[backend_index].host, retry_after, "second" if retry_after == 1 else "seconds")
+
+        # 2) Regardless of whether the response indicates a 429 or 5xx error, we mark the backend as throttling to temporarily take it out of the available backend pool.
+        backend = self.backends[backend_index]
+        backend.is_throttling = True
+        backend.retry_after = datetime.now(timezone.utc) + timedelta(seconds = retry_after)
+
+        # 3) Update the available backends.
+        self._get_available_backends()
+
+    def _handle_4xx_response(self, request, response) -> httpx.Response:
+        """Handle a 4xx response other than 429 from the backend."""
+
+        self._log.warning("Request sent to server: %s, Status code: %s - FAIL", request.url, response.status_code)
+
+        return response
+
+    def _modify_request(self, request, backend_index) -> None:
+        """Modifies the URL and Host header with the desired backend target. This ensures that the request is sent to the chosen backend server."""
+
+        # Modify the request. Note that only the URL and Host header are being modified on the original request object. We make the smallest incision possible to avoid side effects.
+        # Update URL and host header as both must match the backend server.
+        request.url = request.url.copy_with(host = self.backends[backend_index].host)
+        request.headers = request.headers.copy()    # We need to create a mutable copy of the headers before we modify and assign them back to the request object.
+        request.headers['host'] = self.backends[backend_index].host
+
+    def _return_429(self) -> httpx.Response:
+        """Return an HTTP 429 response with a Retry-After header value. This is returned to the caller of this load balancer when no backends are available."""
+
+        self._log.warning("No backend available!")
+        retry_after = str(self._get_soonest_retry_after())
+        self._log.info("Returning HTTP 429 with Retry-After header value of %s %s.", retry_after, "second" if retry_after == "1" else "seconds")
+
+        return httpx.Response(429, content = '', headers={'Retry-After': retry_after})
+
+class AsyncLoadBalancer(BaseLoadBalancer):
+    """Asynchronous Load Balancer class based on BaseLoadBalancer"""
+
+    # Constructor
+    def __init__(self, backends: List[Backend]):
+        super().__init__(httpx.AsyncClient(), backends)
+
+    # Public Methods
+    async def handle_async_request(self, request) -> httpx.Response:
+        """Handles an asynchronous request by issuing an asynchronous request to an available backed."""
+
+        self._log.info("Intercepted and now handling an asynchronous request.")
+
+        # Identify whether any backend is throttling and reset if necessary, then update the remaning available backends prior to any request handling.
+        self._check_throttling()
+        self._get_available_backends()
+        response = None
+
+        while self._available_backends > 0:
+            # 1) Since we have available backends determine the appropriate backend to use.
+            backend_index = self._get_backend_index()
+
+            # 2) Modify the intercepted request.
+            self._modify_request(request, backend_index)
+
+            # 3) Send the request to the selected backend (via async). If an error occurs, it will just bubble up, which is fine.
+            response = await self._transport.send(request)
+
+            # 4) Evaluate the response from the backend:
+            #    If 429 or a 5xx error, we continue the loop and retry with another backend, if available.
+            #    If 200-399, we return the successful response.
+            #    If any other 4xx error, we break the loop and return the response as we don't explicitly handle these client errors.
+            if response is not None and (response.status_code == 429 or response.status_code >= 500):
+                self._handle_429_5xx_response(request, response, backend_index)
+                continue
+
+            if response is not None and (response.status_code >= 200 and response.status_code <= 399):
+                return self._handle_200_399_response(request, response, backend_index)
+
+            return self._handle_4xx_response(request, response)
+
+        # Since no backends are available, we must return a 429.
+        return self._return_429()
+
+class LoadBalancer(BaseLoadBalancer):
+    """Synchronous Load Balancer class based on BaseLoadBalancer"""
+
+    # Constructor
+    def __init__(self, backends: List[Backend]):
+        super().__init__(httpx.Client(), backends)
+
+    # Public Methods
+    def handle_request(self, request) -> httpx.Response:
+        """Handles a synchronous request by issuing a request to an available backed."""
+
+        self._log.info("Intercepted and now handling a synchronous request.")
+
+        # Identify whether any backend is throttling and reset if necessary, then update the remaning available backends prior to any request handling.
+        self._check_throttling()
+        self._get_available_backends()
+        response = None
+
+        while self._available_backends > 0:
+            # 1) Since we have available backends determine the appropriate backend to use.
+            backend_index = self._get_backend_index()
+
+            # 2) Modify the intercepted request.
+            self._modify_request(request, backend_index)
+
+            # 3) Send the request to the selected backend. If an error occurs, it will just bubble up, which is fine.
+            response = self._transport.send(request)
+
+            # 4) Evaluate the response from the backend:
+            #    If 429 or a 5xx error, we continue the loop and retry with another backend, if available.
+            #    If 200-399, we return the successful response.
+            #    If any other 4xx error, we break the loop and return the response as we don't explicitly handle these client errors.
+            if response is not None and (response.status_code == 429 or response.status_code >= 500):
+                self._handle_429_5xx_response(request, response, backend_index)
+                continue
+
+            if response is not None and (response.status_code >= 200 and response.status_code <= 399):
+                return self._handle_200_399_response(request, response, backend_index)
+
+            return self._handle_4xx_response(request, response)
+
+        # Since no backends are available, we must return a 429.
+        return self._return_429()
```

### Comparing `openai_priority_loadbalancer-1.0.7/src/openai_priority_loadbalancer.egg-info/PKG-INFO` & `openai_priority_loadbalancer-1.0.8/src/openai_priority_loadbalancer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 1.0.7
+Version: 1.0.8
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

