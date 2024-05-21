# Comparing `tmp/lacuscore-1.9.3.tar.gz` & `tmp/lacuscore-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.9.3.tar", max compression
+gzip compressed data, was "lacuscore-1.9.4.tar", max compression
```

## Comparing `lacuscore-1.9.3.tar` & `lacuscore-1.9.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1516 2024-05-02 15:14:18.541012 lacuscore-1.9.3/LICENSE
--rw-r--r--   0        0        0      941 2024-05-02 15:14:18.541012 lacuscore-1.9.3/README.md
--rw-r--r--   0        0        0      341 2024-05-02 15:14:18.541012 lacuscore-1.9.3/lacuscore/__init__.py
--rw-r--r--   0        0        0     2711 2024-05-02 15:14:18.541012 lacuscore-1.9.3/lacuscore/helpers.py
--rw-r--r--   0        0        0     2775 2024-05-02 15:14:18.541012 lacuscore-1.9.3/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    42305 2024-05-02 15:14:18.541012 lacuscore-1.9.3/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2024-05-02 15:14:18.541012 lacuscore-1.9.3/lacuscore/py.typed
--rw-r--r--   0        0        0     1916 2024-05-02 15:14:18.541012 lacuscore-1.9.3/lacuscore/task_logger.py
--rw-r--r--   0        0        0     1874 2024-05-02 15:14:18.541012 lacuscore-1.9.3/pyproject.toml
--rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 lacuscore-1.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1516 2024-05-21 12:41:53.107729 lacuscore-1.9.4/LICENSE
+-rw-r--r--   0        0        0      941 2024-05-21 12:41:53.107729 lacuscore-1.9.4/README.md
+-rw-r--r--   0        0        0      341 2024-05-21 12:41:53.107729 lacuscore-1.9.4/lacuscore/__init__.py
+-rw-r--r--   0        0        0     2711 2024-05-21 12:41:53.107729 lacuscore-1.9.4/lacuscore/helpers.py
+-rw-r--r--   0        0        0     2775 2024-05-21 12:41:53.107729 lacuscore-1.9.4/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    43030 2024-05-21 12:41:53.107729 lacuscore-1.9.4/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:41:53.107729 lacuscore-1.9.4/lacuscore/py.typed
+-rw-r--r--   0        0        0     1916 2024-05-21 12:41:53.107729 lacuscore-1.9.4/lacuscore/task_logger.py
+-rw-r--r--   0        0        0     1875 2024-05-21 12:41:53.111729 lacuscore-1.9.4/pyproject.toml
+-rw-r--r--   0        0        0     2629 1970-01-01 00:00:00.000000 lacuscore-1.9.4/PKG-INFO
```

### Comparing `lacuscore-1.9.3/LICENSE` & `lacuscore-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.9.3/README.md` & `lacuscore-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.9.3/lacuscore/helpers.py` & `lacuscore-1.9.4/lacuscore/helpers.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.9.3/lacuscore/lacus_monitoring.py` & `lacuscore-1.9.4/lacuscore/lacus_monitoring.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.9.3/lacuscore/lacuscore.py` & `lacuscore-1.9.4/lacuscore/lacuscore.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,27 @@
 from . import task_logger
 from .helpers import (
     LacusCoreLogAdapter, CaptureError, RetryCapture, CaptureSettingsError,
     CaptureStatus, CaptureResponse, CaptureResponseJson, CaptureSettings)
 
 if sys.version_info < (3, 11):
     from async_timeout import timeout
+
+    def timeout_expired(timeout_cm, logger, error_message: str) -> None:  # type: ignore[no-untyped-def]
+        if timeout_cm.expired:
+            logger.warning(f'Timeout expired: {error_message}')
+
 else:
     from asyncio import timeout
 
+    def timeout_expired(timeout_cm, logger, error_message: str) -> None:  # type: ignore[no-untyped-def]
+        if timeout_cm.expired():
+            logger.warning(f'Timeout expired: {error_message}')
+
+
 BROWSER = Literal['chromium', 'firefox', 'webkit']
 
 
 def _secure_filename(filename: str) -> str:
     """Copy of secure_filename in werkzeug, to avoid the dependency.
     Source: https://github.com/pallets/werkzeug/blob/d36aaf12b5d12634844e4c7f5dab4a8282688e12/src/werkzeug/utils.py#L197
     """
@@ -519,16 +529,14 @@
                     browser_engine = 'chromium'
                 elif browser_family.startswith('firefox'):
                     browser_engine = 'firefox'
                 else:
                     browser_engine = 'webkit'
             try:
                 logger.debug(f'Capturing {url}')
-                # NOTE: starting with python 3.11, we can use asyncio.timeout
-                # async with asyncio.timeout(self.max_capture_time):
                 general_timeout = to_capture.get('general_timeout_in_sec')
                 stats_pipeline.sadd(f'stats:{today}:captures', url)
                 async with Capture(
                         browser=browser_engine,
                         device_name=to_capture.get('device_name'),
                         proxy=proxy,
                         general_timeout_in_sec=general_timeout,
@@ -541,20 +549,27 @@
                     capture.user_agent = to_capture.get('user_agent')  # type: ignore[assignment]
                     capture.http_credentials = to_capture.get('http_credentials')  # type: ignore[assignment]
                     capture.geolocation = to_capture.get('geolocation')  # type: ignore[assignment]
                     capture.timezone_id = to_capture.get('timezone_id')  # type: ignore[assignment]
                     capture.locale = to_capture.get('locale')  # type: ignore[assignment]
                     capture.color_scheme = to_capture.get('color_scheme')  # type: ignore[assignment]
                     try:
-                        async with timeout(general_timeout):
+                        # make sure the initialization doesn't take too long
+                        if general_timeout is None:
+                            general_timeout = 5
+                        init_timeout = max(general_timeout / 2, 5)
+                        async with timeout(init_timeout) as initialize_timeout:
                             await capture.initialize_context()
+
                     except (TimeoutError, asyncio.exceptions.TimeoutError):
+                        timeout_expired(initialize_timeout, logger, 'Initializing took too long.')
                         logger.warning(f'Initializing the context for {url} took longer than the allowed general timeout ({general_timeout}s)')
                         raise RetryCapture(f'Initializing the context for {url} took longer than the allowed general timeout ({general_timeout}s)')
-                    async with timeout(self.max_capture_time):
+
+                    async with timeout(self.max_capture_time) as capture_timeout:
                         playwright_result = await capture.capture_page(
                             url, referer=to_capture.get('referer'),
                             depth=to_capture.get('depth', 0),
                             rendered_hostname_only=to_capture.get('rendered_hostname_only', True),
                             with_favicon=to_capture.get('with_favicon', False),
                             allow_tracking=to_capture.get('allow_tracking', False),
                             max_depth_capture_time=self.max_capture_time)
@@ -572,14 +587,15 @@
             except asyncio.CancelledError:
                 logger.warning(f'The capture of {url} has been cancelled.')
                 result = {'error': f'The capture of {url} has been cancelled.'}
                 # The capture can be canceled if it has been running for way too long.
                 # We can give it another short.
                 raise RetryCapture(f'The capture of {url} has been cancelled.')
             except (TimeoutError, asyncio.exceptions.TimeoutError):
+                timeout_expired(capture_timeout, logger, 'Capture took too long.')
                 logger.warning(f'The capture of {url} took longer than the allowed max capture time ({self.max_capture_time}s)')
                 result = {'error': f'The capture of {url} took longer than the allowed max capture time ({self.max_capture_time}s)'}
                 raise CaptureError(f'The capture of {url} took longer than the allowed max capture time ({self.max_capture_time}s)')
             except Exception as e:
                 logger.exception(f'Something went poorly {url} - {e}')
                 result = {'error': f'Something went poorly {url} - {e}'}
                 raise CaptureError(f'Something went poorly {url} - {e}')
```

### Comparing `lacuscore-1.9.3/lacuscore/task_logger.py` & `lacuscore-1.9.4/lacuscore/task_logger.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.9.3/pyproject.toml` & `lacuscore-1.9.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.9.3"
+version = "1.9.4"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -25,37 +25,37 @@
     'Programming Language :: Python :: 3.12',
     'Topic :: Security',
     'Topic :: Internet',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = "^2.31.0"
+requests = "^2.32.1"
 Sphinx = [
    {version = "<7.2", python = "<3.9", optional = true},
    {version = "^7.2", python = ">=3.9", optional = true}
 ]
-playwrightcapture = {extras = ["recaptcha"], version = "^1.24.6"}
+playwrightcapture = {extras = ["recaptcha"], version = "^1.24.10"}
 defang = "^0.5.3"
 ua-parser = "^0.18.0"
 redis = {version = "^5.0.4", extras = ["hiredis"]}
 dnspython = "^2.6.1"
 async-timeout = {version = "^4.0.3", python = "<3.11"}
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
 [tool.poetry.group.dev.dependencies]
 types-redis = {version = "^4.6.0.20240425"}
 mypy = "^1.10.0"
-types-requests = "^2.31.0.20240406"
-types-beautifulsoup4 = "^4.12.0.20240229"
+types-requests = "^2.32.0.20240521"
+types-beautifulsoup4 = "^4.12.0.20240511"
 ipython = [
     {version = "<8.13.0", python = "<3.9"},
     {version = "^8.18.0", python = ">=3.9"},
     {version = "^8.19.0", python = ">=3.10"}
 ]
-pytest = "^8.2.0"
+pytest = "^8.2.1"
 
 [build-system]
 requires = ["poetry_core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lacuscore-1.9.3/PKG-INFO` & `lacuscore-1.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.9.3
+Version: 1.9.4
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,17 +24,17 @@
 Classifier: Topic :: Security
 Provides-Extra: docs
 Requires-Dist: Sphinx (<7.2) ; (python_version < "3.9") and (extra == "docs")
 Requires-Dist: Sphinx (>=7.2,<8.0) ; (python_version >= "3.9") and (extra == "docs")
 Requires-Dist: async-timeout (>=4.0.3,<5.0.0) ; python_version < "3.11"
 Requires-Dist: defang (>=0.5.3,<0.6.0)
 Requires-Dist: dnspython (>=2.6.1,<3.0.0)
-Requires-Dist: playwrightcapture[recaptcha] (>=1.24.6,<2.0.0)
+Requires-Dist: playwrightcapture[recaptcha] (>=1.24.10,<2.0.0)
 Requires-Dist: redis[hiredis] (>=5.0.4,<6.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2.32.1,<3.0.0)
 Requires-Dist: ua-parser (>=0.18.0,<0.19.0)
 Project-URL: Documentation, https://lacuscore.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/ail-project/LacusCore
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/lacuscore/badge/?version=latest)](https://lacuscore.readthedocs.io/en/latest/?badge=latest)
```

