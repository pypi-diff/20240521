# Comparing `tmp/timer-0.2.2.tar.gz` & `tmp/timer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timer-0.2.2.tar", last modified: Mon Aug 30 15:26:55 2021, max compression
+gzip compressed data, was "timer-0.2.3.tar", last modified: Tue May 21 02:41:40 2024, max compression
```

## Comparing `timer-0.2.2.tar` & `timer-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 15:26:55.521801 timer-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-08-30 15:26:47.000000 timer-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3556 2021-08-30 15:26:55.521801 timer-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2292 2021-08-30 15:26:47.000000 timer-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-30 15:26:55.521801 timer-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      641 2021-08-30 15:26:47.000000 timer-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 15:26:55.521801 timer-0.2.2/timer/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-08-30 15:26:47.000000 timer-0.2.2/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      406 2021-08-30 15:26:47.000000 timer-0.2.2/timer/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3709 2021-08-30 15:26:47.000000 timer-0.2.2/timer/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 15:26:55.521801 timer-0.2.2/timer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3556 2021-08-30 15:26:55.000000 timer-0.2.2/timer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      196 2021-08-30 15:26:55.000000 timer-0.2.2/timer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-30 15:26:55.000000 timer-0.2.2/timer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-08-30 15:26:55.000000 timer-0.2.2/timer.egg-info/top_level.txt
+drwxr-xr-x   0 lucienshui   (501) staff       (20)        0 2024-05-21 02:41:40.339724 timer-0.2.3/
+-rw-r--r--   0 lucienshui   (501) staff       (20)    11357 2024-05-20 17:03:55.000000 timer-0.2.3/LICENSE
+-rw-r--r--   0 lucienshui   (501) staff       (20)     2530 2024-05-21 02:41:40.339560 timer-0.2.3/PKG-INFO
+-rw-r--r--   0 lucienshui   (501) staff       (20)     2292 2024-05-20 17:03:55.000000 timer-0.2.3/README.md
+-rw-r--r--   0 lucienshui   (501) staff       (20)       38 2024-05-21 02:41:40.339779 timer-0.2.3/setup.cfg
+-rw-r--r--   0 lucienshui   (501) staff       (20)      641 2024-05-20 17:03:55.000000 timer-0.2.3/setup.py
+drwxr-xr-x   0 lucienshui   (501) staff       (20)        0 2024-05-21 02:41:40.338872 timer-0.2.3/timer/
+-rw-r--r--   0 lucienshui   (501) staff       (20)      140 2024-05-20 17:27:56.000000 timer-0.2.3/timer/__init__.py
+-rw-r--r--   0 lucienshui   (501) staff       (20)      406 2024-05-20 17:30:44.000000 timer-0.2.3/timer/__version__.py
+-rw-r--r--   0 lucienshui   (501) staff       (20)     4331 2024-05-20 17:27:08.000000 timer-0.2.3/timer/timer.py
+drwxr-xr-x   0 lucienshui   (501) staff       (20)        0 2024-05-21 02:41:40.339387 timer-0.2.3/timer.egg-info/
+-rw-r--r--   0 lucienshui   (501) staff       (20)     2530 2024-05-21 02:41:40.000000 timer-0.2.3/timer.egg-info/PKG-INFO
+-rw-r--r--   0 lucienshui   (501) staff       (20)      196 2024-05-21 02:41:40.000000 timer-0.2.3/timer.egg-info/SOURCES.txt
+-rw-r--r--   0 lucienshui   (501) staff       (20)        1 2024-05-21 02:41:40.000000 timer-0.2.3/timer.egg-info/dependency_links.txt
+-rw-r--r--   0 lucienshui   (501) staff       (20)        6 2024-05-21 02:41:40.000000 timer-0.2.3/timer.egg-info/top_level.txt
```

### Comparing `timer-0.2.2/LICENSE` & `timer-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `timer-0.2.2/PKG-INFO` & `timer-0.2.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,136 +1,125 @@
-Metadata-Version: 2.1
-Name: timer
-Version: 0.2.2
-Summary: Python Code Timer
-Home-page: https://github.com/LucienShui/timer
-Author: Lucien Shui
-Author-email: lucien@lucien.ink
-License: UNKNOWN
-Description: # Timer
-        
-        Python code timer, support block wise and function wise
-        
-        ## Installation
-        
-        ```shell
-        pip install timer
-        ```
-        
-        ## Usage
-        
-        1. import
-            ```py
-            from timer import timer
-            ```
-        
-        2. decorate without brackets
-            ```py
-            @timer
-            def func(): ...
-            ```
-        
-        3. decorate with brackets
-            ```py
-            @timer()
-            def func(): ...
-            ```
-        
-        4. decorate with name and time unit
-            ```py
-            @timer('function name', 's')
-            def func(): ...
-            ```
-        
-        5. decorate with key word arguments
-            ```py
-            @timer(name='function name', unit='s')
-            def func(): ...
-            ```
-           
-        6. block wise without object
-        
-            ```py
-            with timer():
-                ...
-            ```
-           
-        7. block wise with object
-           
-            ```py
-            with timer() as t:
-                ...
-                print(t.elapse)
-            ```
-        
-        ## Sample Code
-        
-        ```python
-        import logging
-        import time
-        
-        from timer import timer, get_timer
-        
-        # default timer's logging level is logging.DEBUG
-        # so timer would print nothing if logging level is logging.INFO or higher
-        logging.basicConfig(level=logging.DEBUG)
-        
-        # or you can change default timer's logging level
-        timer.set_level(logging.DEBUG)
-        
-        # also you can get a timer with custom logging level with get_timer(level)
-        warning_timer = get_timer(logging.WARNING)
-        
-        
-        # explicit the timer's name and it's time unit
-        @timer('function:add', unit='s')
-        def add(a, b):
-            time.sleep(.1)
-            return a + b
-        
-        
-        # function name is timer's name for default
-        @timer
-        def sub(a, b):
-            time.sleep(.1)
-            return a - b
-        
-        
-        if __name__ == '__main__':
-            # 'timer' would be timer's name by default
-            with timer('time.sleep(2)') as t:
-                print(3)
-                time.sleep(1)
-                print(f'after time.sleep(1) once, t.elapse = {t.elapse}')
-                time.sleep(1)
-                print(f'after time.sleep(1) twice, t.elapse = {t.elapse}')
-            print(f'after with, t.elapse = {t.elapse}')
-            
-            with warning_timer('test'):
-               pass
-        
-            print(add(1, 1))
-            print(sub(2, 1))
-        ```
-        
-        ### Outputs
-        
-        ```plain
-        3
-        after time.sleep(1) once, t.elapse = 1.003798776
-        after time.sleep(1) twice, t.elapse = 2.0052743459999998
-        DEBUG:timer.time.sleep(2): 2.006 s
-        after with, t.elapse = 2.005628447
-        WARNING:timer.test:start
-        WARNING:timer.test:cost 0 ms
-        DEBUG:timer.function:add: 0.105 s
-        2
-        DEBUG:timer.sub: 102 ms
-        1
-        ```
-        
-        ## Special Thanks
-        
-        [@Krzysztof S](https://github.com/papierukartka)
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# Timer
+
+Python code timer, support block wise and function wise
+
+## Installation
+
+```shell
+pip install timer
+```
+
+## Usage
+
+1. import
+    ```py
+    from timer import timer
+    ```
+
+2. decorate without brackets
+    ```py
+    @timer
+    def func(): ...
+    ```
+
+3. decorate with brackets
+    ```py
+    @timer()
+    def func(): ...
+    ```
+
+4. decorate with name and time unit
+    ```py
+    @timer('function name', 's')
+    def func(): ...
+    ```
+
+5. decorate with key word arguments
+    ```py
+    @timer(name='function name', unit='s')
+    def func(): ...
+    ```
+   
+6. block wise without object
+
+    ```py
+    with timer():
+        ...
+    ```
+   
+7. block wise with object
+   
+    ```py
+    with timer() as t:
+        ...
+        print(t.elapse)
+    ```
+
+## Sample Code
+
+```python
+import logging
+import time
+
+from timer import timer, get_timer
+
+# default timer's logging level is logging.DEBUG
+# so timer would print nothing if logging level is logging.INFO or higher
+logging.basicConfig(level=logging.DEBUG)
+
+# or you can change default timer's logging level
+timer.set_level(logging.DEBUG)
+
+# also you can get a timer with custom logging level with get_timer(level)
+warning_timer = get_timer(logging.WARNING)
+
+
+# explicit the timer's name and it's time unit
+@timer('function:add', unit='s')
+def add(a, b):
+    time.sleep(.1)
+    return a + b
+
+
+# function name is timer's name for default
+@timer
+def sub(a, b):
+    time.sleep(.1)
+    return a - b
+
+
+if __name__ == '__main__':
+    # 'timer' would be timer's name by default
+    with timer('time.sleep(2)') as t:
+        print(3)
+        time.sleep(1)
+        print(f'after time.sleep(1) once, t.elapse = {t.elapse}')
+        time.sleep(1)
+        print(f'after time.sleep(1) twice, t.elapse = {t.elapse}')
+    print(f'after with, t.elapse = {t.elapse}')
+    
+    with warning_timer('test'):
+       pass
+
+    print(add(1, 1))
+    print(sub(2, 1))
+```
+
+### Outputs
+
+```plain
+3
+after time.sleep(1) once, t.elapse = 1.003798776
+after time.sleep(1) twice, t.elapse = 2.0052743459999998
+DEBUG:timer.time.sleep(2): 2.006 s
+after with, t.elapse = 2.005628447
+WARNING:timer.test:start
+WARNING:timer.test:cost 0 ms
+DEBUG:timer.function:add: 0.105 s
+2
+DEBUG:timer.sub: 102 ms
+1
+```
+
+## Special Thanks
+
+[@Krzysztof S](https://github.com/papierukartka)
```

### Comparing `timer-0.2.2/README.md` & `timer-0.2.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: timer
+Version: 0.2.3
+Summary: Python Code Timer
+Home-page: https://github.com/LucienShui/timer
+Author: Lucien Shui
+Author-email: lucien@lucien.ink
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Timer
 
 Python code timer, support block wise and function wise
 
 ## Installation
 
 ```shell
```

### Comparing `timer-0.2.2/setup.py` & `timer-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `timer-0.2.2/timer/timer.py` & `timer-0.2.3/timer/timer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
+from typing import Any, Callable
 import types
-import typing
 from inspect import isfunction
 from time import perf_counter
 
 
 def _log(logger: logging.Logger, level: int, message: str):
     if level == logging.DEBUG:
         logger.debug(message)
@@ -16,20 +16,35 @@
         logger.error(message)
     elif level == logging.CRITICAL:
         logger.critical(message)
     else:
         raise AssertionError('wrong level')
 
 
-def get_timer(level: int = logging.DEBUG):
+def _get_logger_print_fn(logger: logging.Logger, level: int) -> Callable[[str], None]:
+    if level == logging.DEBUG:
+        return logger.debug
+    if level == logging.INFO:
+        return logger.info
+    if level == logging.WARNING:
+        return logger.warning
+    if level == logging.ERROR:
+        return logger.error
+    if level == logging.CRITICAL:
+        return logger.critical
+    raise AssertionError('wrong level')
+
+
+def get_timer(level: int = None, print_fn: Callable[[str], None] = None):
     class Timer(object):
 
         _level = level
+        _print_fn = print_fn
 
-        def __init__(self, name_or_func: typing.Any = None, unit: str = 'auto'):
+        def __init__(self, name_or_func: Any = None, unit: str = 'auto'):
             """
             :param name_or_func: name of function, or function itself, user should not care about this parameter
             :param unit: time's unit, should be one of 's', 'ms' or 'auto'
             """
             if unit not in ['s', 'ms', 'auto']:
                 raise AssertionError(f"field unit should be one of 's', 'ms', 'auto', got {unit}")
 
@@ -42,37 +57,40 @@
 
             self._unit: str = unit
 
             self._logger: logging.Logger = logging.getLogger('timer')
 
             self._begin: float = ...
             self._end: float = ...
-            self._elapse: float = ...
+
+        def _log(self, message: str, name: str = None) -> None:
+            if self._print_fn is not None:
+                pass
+            if self._level is not None:
+                if name is not None:
+                    _log(self._logger.getChild(name), self._level, message)
 
         @property
-        def elapse(self) -> float:
-            if self._elapse is ...:
-                return perf_counter() - self._begin
-            return self._elapse
+        def elapse(self) -> int:
+            if self._end is ...:
+                end = perf_counter()
+            else:
+                end = self._end
+            return round((end - self._begin) * 1000)
 
         def _start(self, name: str) -> None:
-            logger = self._logger.getChild(name)
-            _log(logger, self._level, 'start')
+            self._log('start', name=name)
             self._begin = perf_counter()
 
         def _stop(self, name: str) -> None:
             self._end = perf_counter()
-            self._elapse: float = self._end - self._begin
-
-            logger = self._logger.getChild(name)
-
-            if self._unit == 'ms' or (self._unit == 'auto' and self._elapse < 1):
-                _log(logger, self._level, f'cost {self._elapse * 1000:.0f} ms')
+            if self._unit == 'ms' or (self._unit == 'auto' and self.elapse < 1000):
+                self._log(f'cost {self.elapse} ms', name=name)
             else:
-                _log(logger, self._level, f'cost {self._elapse:.3f} s')
+                self._log(f'cost {self.elapse / 1000:.3f} s', name=name)
 
         def __enter__(self):
             self._start(self._name or 'timer')
             return self
 
         def __exit__(self, exc_type, exc_val, exc_tb):
             self._stop(self._name or 'timer')
```

