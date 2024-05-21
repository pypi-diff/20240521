# Comparing `tmp/limited_aiogram-0.1.2.tar.gz` & `tmp/limited_aiogram-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limited_aiogram-0.1.2.tar", last modified: Thu Jan 18 16:07:00 2024, max compression
+gzip compressed data, was "limited_aiogram-1.0.tar", last modified: Tue May 21 18:32:05 2024, max compression
```

## Comparing `limited_aiogram-0.1.2.tar` & `limited_aiogram-1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-01-18 16:07:00.734670 limited_aiogram-0.1.2/
--rw-rw-rw-   0        0        0     1102 2024-01-14 15:54:12.000000 limited_aiogram-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1272 2024-01-18 16:07:00.735667 limited_aiogram-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      754 2024-01-18 16:03:14.000000 limited_aiogram-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-01-18 16:07:00.723699 limited_aiogram-0.1.2/limited_aiogram/
--rw-rw-rw-   0        0        0       84 2024-01-14 15:17:48.000000 limited_aiogram-0.1.2/limited_aiogram/__init__.py
--rw-rw-rw-   0        0        0     2432 2024-01-18 15:56:21.000000 limited_aiogram-0.1.2/limited_aiogram/limit_caller.py
--rw-rw-rw-   0        0        0      953 2024-01-18 15:55:42.000000 limited_aiogram-0.1.2/limited_aiogram/limited_bot.py
-drwxrwxrwx   0        0        0        0 2024-01-18 16:07:00.733672 limited_aiogram-0.1.2/limited_aiogram.egg-info/
--rw-rw-rw-   0        0        0     1272 2024-01-18 16:07:00.000000 limited_aiogram-0.1.2/limited_aiogram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2024-01-18 16:07:00.000000 limited_aiogram-0.1.2/limited_aiogram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-18 16:07:00.000000 limited_aiogram-0.1.2/limited_aiogram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-01-18 16:07:00.000000 limited_aiogram-0.1.2/limited_aiogram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-01-18 16:07:00.000000 limited_aiogram-0.1.2/limited_aiogram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-18 16:07:00.736665 limited_aiogram-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      803 2024-01-18 16:00:11.000000 limited_aiogram-0.1.2/setup.py
+drwxrwxr-x   0 artyom    (1000) artyom    (1000)        0 2024-05-21 18:32:05.207322 limited_aiogram-1.0/
+-rw-rw-r--   0 artyom    (1000) artyom    (1000)     1083 2024-05-21 17:42:11.000000 limited_aiogram-1.0/LICENSE
+-rw-r--r--   0 artyom    (1000) artyom    (1000)     1350 2024-05-21 18:32:05.207322 limited_aiogram-1.0/PKG-INFO
+-rw-rw-r--   0 artyom    (1000) artyom    (1000)      724 2024-05-21 17:42:11.000000 limited_aiogram-1.0/README.md
+drwxrwxr-x   0 artyom    (1000) artyom    (1000)        0 2024-05-21 18:32:05.203322 limited_aiogram-1.0/limited_aiogram/
+-rw-rw-r--   0 artyom    (1000) artyom    (1000)       83 2024-05-21 17:42:11.000000 limited_aiogram-1.0/limited_aiogram/__init__.py
+-rw-rw-r--   0 artyom    (1000) artyom    (1000)     1569 2024-05-21 18:22:55.000000 limited_aiogram-1.0/limited_aiogram/limit_caller.py
+-rw-rw-r--   0 artyom    (1000) artyom    (1000)     1101 2024-05-21 18:23:12.000000 limited_aiogram-1.0/limited_aiogram/limited_bot.py
+drwxrwxr-x   0 artyom    (1000) artyom    (1000)        0 2024-05-21 18:32:05.207322 limited_aiogram-1.0/limited_aiogram.egg-info/
+-rw-r--r--   0 artyom    (1000) artyom    (1000)     1350 2024-05-21 18:32:05.000000 limited_aiogram-1.0/limited_aiogram.egg-info/PKG-INFO
+-rw-rw-r--   0 artyom    (1000) artyom    (1000)      311 2024-05-21 18:32:05.000000 limited_aiogram-1.0/limited_aiogram.egg-info/SOURCES.txt
+-rw-rw-r--   0 artyom    (1000) artyom    (1000)        1 2024-05-21 18:32:05.000000 limited_aiogram-1.0/limited_aiogram.egg-info/dependency_links.txt
+-rw-rw-r--   0 artyom    (1000) artyom    (1000)       65 2024-05-21 18:32:05.000000 limited_aiogram-1.0/limited_aiogram.egg-info/requires.txt
+-rw-rw-r--   0 artyom    (1000) artyom    (1000)       16 2024-05-21 18:32:05.000000 limited_aiogram-1.0/limited_aiogram.egg-info/top_level.txt
+-rw-rw-r--   0 artyom    (1000) artyom    (1000)       38 2024-05-21 18:32:05.207322 limited_aiogram-1.0/setup.cfg
+-rw-rw-r--   0 artyom    (1000) artyom    (1000)      884 2024-05-21 18:25:29.000000 limited_aiogram-1.0/setup.py
```

### Comparing `limited_aiogram-0.1.2/LICENSE` & `limited_aiogram-1.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-The MIT License (MIT)
-
-Copyright (c) 2020 Fernando C. Souza
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+The MIT License (MIT)
+
+Copyright (c) 2020 Fernando C. Souza
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `limited_aiogram-0.1.2/PKG-INFO` & `limited_aiogram-1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,48 @@
-Metadata-Version: 2.1
-Name: limited_aiogram
-Version: 0.1.2
-Summary: Limit your api calls to avoid  "Flood control exceeded"
-Author: chazovtema
-Author-email: chazovtema@mail.ru
-Project-URL: github, https://github.com/chazovtema/limited_aiogram
-Keywords: aiogram,limit
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# What is it?
-
-Limited aiogram is an add-on for the original aiogram Bot. This package allows you to limit how often your bot sends messages
-
-# Telegram api limits
-
-Telegram has a number of restrictions for sending messages:
-
-- 30 messages per second to multiple users
-- 20 requests/sec to group
-- 1 message per second to individual chat
-
-# Usage
-
-The code below patches the original Bot class from aiogram, these changes are not reversible!
-```python
-import limit_aiogram
-limit_aiogram.path_bot()
-```
-It is also possible to use a separate class `LimitedBot``, without changing the original class
-
-```python
-import limit_aiogram
-bot = limit_aiogram.LimitedBot('your token')
-```
-
-# Installation
-
-`pip install limited_aiogram`
+Metadata-Version: 2.1
+Name: limited_aiogram
+Version: 1.0
+Summary: Limit your api calls to avoid  "Flood control exceeded"
+Author: chazovtema
+Author-email: chazovtema@mail.ru
+Project-URL: github, https://github.com/chazovtema/limited_aiogram
+Keywords: aiogram,limit
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.25.1
+Requires-Dist: aiogram>=3.0.0
+Requires-Dist: limiter>=0.3.1
+Requires-Dist: cachetools>=5.3.2
+
+# What is it?
+
+Limited aiogram is an add-on for the original aiogram Bot. This package allows you to limit how often your bot sends messages
+
+# Telegram api limits
+
+Telegram has a number of restrictions for sending messages:
+
+- 30 messages per second to multiple users
+- 20 requests/sec to group
+- 1 message per second to individual chat
+
+# Usage
+
+The code below patches the original Bot class from aiogram, these changes are not reversible!
+```python
+import limit_aiogram
+limit_aiogram.path_bot()
+```
+It is also possible to use a separate class `LimitedBot`, without changing the original class
+
+```python
+import limit_aiogram
+bot = limit_aiogram.LimitedBot('your token')
+```
+
+# Installation
+
+`pip install limited_aiogram`
```

### Comparing `limited_aiogram-0.1.2/limited_aiogram/limited_bot.py` & `limited_aiogram-1.0/limited_aiogram/limited_bot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,38 @@
-from typing import Optional, TypeVar
-from aiogram.client.session.base import BaseSession
-
-from aiogram.methods import TelegramMethod, GetChat
-from aiogram import Bot
-
-from .limit_caller import LimitCaller
-
-T = TypeVar("T")
-
-class LimitedBot(Bot):
-    
-    async def __call__(self, method: TelegramMethod[T], request_timeout: Optional[int] = None):
-        
-        coro = self.session(self, method, timeout=request_timeout)
-        if hasattr(method, 'chat_id') and not isinstance(method, GetChat):
-            caller = self.__dict__.get('caller')
-            if not caller:
-                caller = LimitCaller()
-                self.caller = caller
-            chat = await self.get_chat(method.chat_id)
-            return await caller.call(chat, coro)
-        else:
-            return await coro
-
-def path_bot():
-    
-    """Patches the bot, these changes are not reversible"""
-    
-    Bot.__call__ = LimitedBot.__call__
+from typing import Optional, TypeVar
+
+from aiogram.methods import TelegramMethod, GetChat
+from aiogram import Bot
+
+from .limit_caller import LimitCaller
+
+T = TypeVar("T")
+
+class LimitedBot(Bot):
+
+    async def _call(
+        self, method: TelegramMethod[T], request_timeout: Optional[int] = None
+    ):
+        """
+        Just to not modify __init__ method
+        """
+        coro = self.session(self, method, timeout=request_timeout)
+        if hasattr(method, "chat_id") and not isinstance(method, GetChat):
+            return await self.caller.call(method.chat_id, coro)
+        else:
+            return await coro
+
+    async def __call__(
+        self, method: TelegramMethod[T], request_timeout: Optional[int] = None
+    ):
+        caller = getattr(self, "caller", None)
+        if not caller:
+            caller = LimitCaller()
+            self.caller = caller
+            self.__call__ = LimitedBot._call
+        return await LimitedBot._call(self, method, request_timeout)
+
+
+def path_bot():
+    """Patches the bot, these changes are not reversible"""
+
+    Bot.__call__ = LimitedBot.__call__
```

### Comparing `limited_aiogram-0.1.2/limited_aiogram.egg-info/PKG-INFO` & `limited_aiogram-1.0/limited_aiogram.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,48 @@
-Metadata-Version: 2.1
-Name: limited-aiogram
-Version: 0.1.2
-Summary: Limit your api calls to avoid  "Flood control exceeded"
-Author: chazovtema
-Author-email: chazovtema@mail.ru
-Project-URL: github, https://github.com/chazovtema/limited_aiogram
-Keywords: aiogram,limit
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# What is it?
-
-Limited aiogram is an add-on for the original aiogram Bot. This package allows you to limit how often your bot sends messages
-
-# Telegram api limits
-
-Telegram has a number of restrictions for sending messages:
-
-- 30 messages per second to multiple users
-- 20 requests/sec to group
-- 1 message per second to individual chat
-
-# Usage
-
-The code below patches the original Bot class from aiogram, these changes are not reversible!
-```python
-import limit_aiogram
-limit_aiogram.path_bot()
-```
-It is also possible to use a separate class `LimitedBot``, without changing the original class
-
-```python
-import limit_aiogram
-bot = limit_aiogram.LimitedBot('your token')
-```
-
-# Installation
-
-`pip install limited_aiogram`
+Metadata-Version: 2.1
+Name: limited_aiogram
+Version: 1.0
+Summary: Limit your api calls to avoid  "Flood control exceeded"
+Author: chazovtema
+Author-email: chazovtema@mail.ru
+Project-URL: github, https://github.com/chazovtema/limited_aiogram
+Keywords: aiogram,limit
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.25.1
+Requires-Dist: aiogram>=3.0.0
+Requires-Dist: limiter>=0.3.1
+Requires-Dist: cachetools>=5.3.2
+
+# What is it?
+
+Limited aiogram is an add-on for the original aiogram Bot. This package allows you to limit how often your bot sends messages
+
+# Telegram api limits
+
+Telegram has a number of restrictions for sending messages:
+
+- 30 messages per second to multiple users
+- 20 requests/sec to group
+- 1 message per second to individual chat
+
+# Usage
+
+The code below patches the original Bot class from aiogram, these changes are not reversible!
+```python
+import limit_aiogram
+limit_aiogram.path_bot()
+```
+It is also possible to use a separate class `LimitedBot`, without changing the original class
+
+```python
+import limit_aiogram
+bot = limit_aiogram.LimitedBot('your token')
+```
+
+# Installation
+
+`pip install limited_aiogram`
```

