# Comparing `tmp/asyncpause-0.1.0.tar.gz` & `tmp/asyncpause-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpause-0.1.0.tar", last modified: Mon May 20 00:20:07 2024, max compression
+gzip compressed data, was "asyncpause-0.1.1.tar", last modified: Tue May 21 17:43:01 2024, max compression
```

## Comparing `asyncpause-0.1.0.tar` & `asyncpause-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1211 2024-05-20 00:09:38.154909 asyncpause-0.1.0/LICENSE
--rw-r--r--   0        0        0     2989 2024-05-20 00:19:53.527545 asyncpause-0.1.0/README.md
--rw-r--r--   0        0        0      513 2024-05-20 00:20:07.837752 asyncpause-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       75 2024-05-20 00:16:42.078802 asyncpause-0.1.0/src/asyncpause/__init__.py
--rw-r--r--   0        0        0     3970 2024-05-20 00:15:32.140570 asyncpause-0.1.0/src/asyncpause/ap.py
--rw-r--r--   0        0        0        0 2024-05-20 00:17:54.038118 asyncpause-0.1.0/src/asyncpause/py.typed
--rw-r--r--   0        0        0        0 2024-05-20 00:14:31.285595 asyncpause-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3349 1970-01-01 00:00:00.000000 asyncpause-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-21 17:42:58.186208 asyncpause-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3551 2024-05-21 17:42:58.186208 asyncpause-0.1.1/README.md
+-rw-r--r--   0        0        0      513 2024-05-21 17:43:01.594199 asyncpause-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       75 2024-05-21 17:42:58.186208 asyncpause-0.1.1/src/asyncpause/__init__.py
+-rw-r--r--   0        0        0     3970 2024-05-21 17:42:58.186208 asyncpause-0.1.1/src/asyncpause/ap.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:42:58.186208 asyncpause-0.1.1/src/asyncpause/py.typed
+-rw-r--r--   0        0        0     3911 1970-01-01 00:00:00.000000 asyncpause-0.1.1/PKG-INFO
```

### Comparing `asyncpause-0.1.0/LICENSE` & `asyncpause-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncpause-0.1.0/README.md` & `asyncpause-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -40,14 +40,34 @@
     await asyncio.sleep(6)
 
 asyncio.run(main())
 ```
 
 In this example, the `aprint` function its just an example. Just run this script, and watch your console get filled with timely greetings.
 
+If you want to decouple the function call from background processes initialiation, you can use the `start_background` method:
+
+```python
+import asyncio
+from datetime import datetime, timedelta
+from asyncpause import AsyncPause
+
+async def aprint(*args, **kwargs):
+    print(*args, **kwargs)
+
+D = AsyncPause(aprint, filepath="aprint.scheduled.calls")
+
+async def main():
+    d = await D.start_background()
+    d.set(datetime.now(), "Hello, world!")
+    d.set(timedelta(seconds=1), "Hello, world after a second!")
+    await asyncio.sleep(3)
+asyncio.run(main())
+```
+
 ## How It Works
 
 1. **Initialization**: Create an `AsyncPause` object with your target function.
 2. **Scheduling**: Use the `set` method to schedule your function calls. You can specify a delay in seconds, a `timedelta`, or a specific `datetime`.
 3. **Persistence**: The library saves the scheduled calls to a file (or keeps them in memory if you prefer).
 4. **Execution**: It runs the scheduled calls at the right time, even after restarts.
```

### Comparing `asyncpause-0.1.0/pyproject.toml` & `asyncpause-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "asyncpause"
-version = "0.1.0"
+version = "0.1.1"
 description = "a Python library to schedule and persist async function calls, ensuring they run exactly when you need them, even after restarts."
 authors = [
     { name = "Grigory Bakunov", email = "bobuk@rubedo.cloud" },
 ]
 dependencies = [
-    "aiofiles>=23.2.1",
+    "aiofiles>=23.0.0",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "Unlicense"
```

### Comparing `asyncpause-0.1.0/src/asyncpause/ap.py` & `asyncpause-0.1.1/src/asyncpause/ap.py`

 * *Files identical despite different names*

### Comparing `asyncpause-0.1.0/PKG-INFO` & `asyncpause-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: asyncpause
-Version: 0.1.0
+Version: 0.1.1
 Summary: a Python library to schedule and persist async function calls, ensuring they run exactly when you need them, even after restarts.
 Author-Email: Grigory Bakunov <bobuk@rubedo.cloud>
 License: Unlicense
 Requires-Python: >=3.10
-Requires-Dist: aiofiles>=23.2.1
+Requires-Dist: aiofiles>=23.0.0
 Description-Content-Type: text/markdown
 
 # asyncpause
 
 Welcome to `asyncpause`! This nifty little Python library is here to make sure your async functions get called exactly when you want them to, even if your program decides to take a little nap in between. With `asyncpause`, you can schedule async function calls to run at specific times or after certain delays, and it will ensure they are executed even after a restart. Say goodbye to missed calls and hello to punctuality!
 
 ## Features
@@ -50,14 +50,34 @@
     await asyncio.sleep(6)
 
 asyncio.run(main())
 ```
 
 In this example, the `aprint` function its just an example. Just run this script, and watch your console get filled with timely greetings.
 
+If you want to decouple the function call from background processes initialiation, you can use the `start_background` method:
+
+```python
+import asyncio
+from datetime import datetime, timedelta
+from asyncpause import AsyncPause
+
+async def aprint(*args, **kwargs):
+    print(*args, **kwargs)
+
+D = AsyncPause(aprint, filepath="aprint.scheduled.calls")
+
+async def main():
+    d = await D.start_background()
+    d.set(datetime.now(), "Hello, world!")
+    d.set(timedelta(seconds=1), "Hello, world after a second!")
+    await asyncio.sleep(3)
+asyncio.run(main())
+```
+
 ## How It Works
 
 1. **Initialization**: Create an `AsyncPause` object with your target function.
 2. **Scheduling**: Use the `set` method to schedule your function calls. You can specify a delay in seconds, a `timedelta`, or a specific `datetime`.
 3. **Persistence**: The library saves the scheduled calls to a file (or keeps them in memory if you prefer).
 4. **Execution**: It runs the scheduled calls at the right time, even after restarts.
```

