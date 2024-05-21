# Comparing `tmp/disunity-0.1.7.tar.gz` & `tmp/disunity-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disunity-0.1.7.tar", last modified: Thu Jan  4 11:18:16 2024, max compression
+gzip compressed data, was "disunity-0.1.8.tar", last modified: Tue May 21 18:51:24 2024, max compression
```

## Comparing `disunity-0.1.7.tar` & `disunity-0.1.8.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 tadeo      (501) staff       (20)        0 2024-01-04 11:18:16.569146 disunity-0.1.7/
--rw-r--r--   0 tadeo      (501) staff       (20)     1062 2024-01-04 10:36:50.000000 disunity-0.1.7/LICENSE
--rw-r--r--   0 tadeo      (501) staff       (20)     1992 2024-01-04 11:18:16.568787 disunity-0.1.7/PKG-INFO
--rw-r--r--   0 tadeo      (501) staff       (20)     1473 2024-01-04 10:36:50.000000 disunity-0.1.7/README.md
--rw-r--r--   0 tadeo      (501) staff       (20)      703 2024-01-04 11:17:06.000000 disunity-0.1.7/pyproject.toml
--rw-r--r--   0 tadeo      (501) staff       (20)       38 2024-01-04 11:18:16.569205 disunity-0.1.7/setup.cfg
-drwxr-xr-x   0 tadeo      (501) staff       (20)        0 2024-01-04 11:18:16.562031 disunity-0.1.7/src/
-drwxr-xr-x   0 tadeo      (501) staff       (20)        0 2024-01-04 11:18:16.565430 disunity-0.1.7/src/disunity/
--rw-r--r--   0 tadeo      (501) staff       (20)      172 2024-01-04 10:36:50.000000 disunity-0.1.7/src/disunity/__init__.py
--rw-r--r--   0 tadeo      (501) staff       (20)     1362 2024-01-04 10:36:50.000000 disunity-0.1.7/src/disunity/cache.py
--rw-r--r--   0 tadeo      (501) staff       (20)     3672 2024-01-04 10:36:50.000000 disunity-0.1.7/src/disunity/embed.py
--rw-r--r--   0 tadeo      (501) staff       (20)      801 2024-01-04 10:36:50.000000 disunity-0.1.7/src/disunity/errors.py
--rw-r--r--   0 tadeo      (501) staff       (20)     5465 2024-01-04 10:36:50.000000 disunity-0.1.7/src/disunity/identifiers.py
-drwxr-xr-x   0 tadeo      (501) staff       (20)        0 2024-01-04 11:18:16.568144 disunity-0.1.7/src/disunity/models/
--rw-r--r--   0 tadeo      (501) staff       (20)      286 2024-01-04 10:36:50.000000 disunity-0.1.7/src/disunity/models/__init__.py
--rw-r--r--   0 tadeo      (501) staff       (20)     6301 2024-01-04 11:17:51.000000 disunity-0.1.7/src/disunity/models/components.py
--rw-r--r--   0 tadeo      (501) staff       (20)     4107 2024-01-04 10:36:50.000000 disunity-0.1.7/src/disunity/models/context.py
--rw-r--r--   0 tadeo      (501) staff       (20)     2464 2024-01-04 10:36:50.000000 disunity-0.1.7/src/disunity/models/interaction.py
--rw-r--r--   0 tadeo      (501) staff       (20)      812 2024-01-04 10:36:50.000000 disunity-0.1.7/src/disunity/models/member.py
--rw-r--r--   0 tadeo      (501) staff       (20)     4377 2024-01-04 10:36:50.000000 disunity-0.1.7/src/disunity/models/message.py
--rw-r--r--   0 tadeo      (501) staff       (20)      758 2024-01-04 10:36:50.000000 disunity-0.1.7/src/disunity/models/user.py
--rw-r--r--   0 tadeo      (501) staff       (20)     5967 2024-01-04 10:36:50.000000 disunity-0.1.7/src/disunity/package.py
--rw-r--r--   0 tadeo      (501) staff       (20)    10612 2024-01-04 10:36:50.000000 disunity-0.1.7/src/disunity/server.py
--rw-r--r--   0 tadeo      (501) staff       (20)      989 2024-01-04 10:36:50.000000 disunity-0.1.7/src/disunity/utils.py
-drwxr-xr-x   0 tadeo      (501) staff       (20)        0 2024-01-04 11:18:16.568451 disunity-0.1.7/src/disunity.egg-info/
--rw-r--r--   0 tadeo      (501) staff       (20)     1992 2024-01-04 11:18:16.000000 disunity-0.1.7/src/disunity.egg-info/PKG-INFO
--rw-r--r--   0 tadeo      (501) staff       (20)      586 2024-01-04 11:18:16.000000 disunity-0.1.7/src/disunity.egg-info/SOURCES.txt
--rw-r--r--   0 tadeo      (501) staff       (20)        1 2024-01-04 11:18:16.000000 disunity-0.1.7/src/disunity.egg-info/dependency_links.txt
--rw-r--r--   0 tadeo      (501) staff       (20)        9 2024-01-04 11:18:16.000000 disunity-0.1.7/src/disunity.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 18:51:24.550630 disunity-0.1.8/
+-rw-rw-rw-   0        0        0     1083 2024-05-21 18:48:45.000000 disunity-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     2066 2024-05-21 18:51:24.549491 disunity-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1533 2024-05-21 18:48:45.000000 disunity-0.1.8/README.md
+-rw-rw-rw-   0        0        0      731 2024-05-21 18:48:45.000000 disunity-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 18:51:24.550630 disunity-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 18:51:24.507318 disunity-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 18:51:24.519681 disunity-0.1.8/src/disunity/
+-rw-rw-rw-   0        0        0      190 2024-05-21 18:48:45.000000 disunity-0.1.8/src/disunity/__init__.py
+-rw-rw-rw-   0        0        0     1403 2024-05-21 18:48:45.000000 disunity-0.1.8/src/disunity/cache.py
+-rw-rw-rw-   0        0        0     3634 2024-05-21 18:48:45.000000 disunity-0.1.8/src/disunity/embed.py
+-rw-rw-rw-   0        0        0      828 2024-05-21 18:48:45.000000 disunity-0.1.8/src/disunity/errors.py
+-rw-rw-rw-   0        0        0     5643 2024-05-21 18:48:45.000000 disunity-0.1.8/src/disunity/identifiers.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:51:24.545803 disunity-0.1.8/src/disunity/models/
+-rw-rw-rw-   0        0        0      337 2024-05-21 18:48:45.000000 disunity-0.1.8/src/disunity/models/__init__.py
+-rw-rw-rw-   0        0        0      956 2024-05-21 18:48:45.000000 disunity-0.1.8/src/disunity/models/attachment.py
+-rw-rw-rw-   0        0        0     6543 2024-05-21 18:48:45.000000 disunity-0.1.8/src/disunity/models/components.py
+-rw-rw-rw-   0        0        0     5053 2024-05-21 18:48:45.000000 disunity-0.1.8/src/disunity/models/context.py
+-rw-rw-rw-   0        0        0     2527 2024-05-21 18:48:45.000000 disunity-0.1.8/src/disunity/models/interaction.py
+-rw-rw-rw-   0        0        0      834 2024-05-21 18:48:45.000000 disunity-0.1.8/src/disunity/models/member.py
+-rw-rw-rw-   0        0        0     4584 2024-05-21 18:48:45.000000 disunity-0.1.8/src/disunity/models/message.py
+-rw-rw-rw-   0        0        0      782 2024-05-21 18:48:45.000000 disunity-0.1.8/src/disunity/models/user.py
+-rw-rw-rw-   0        0        0     6172 2024-05-21 18:48:45.000000 disunity-0.1.8/src/disunity/package.py
+-rw-rw-rw-   0        0        0    11848 2024-05-21 18:48:45.000000 disunity-0.1.8/src/disunity/server.py
+-rw-rw-rw-   0        0        0     1031 2024-05-21 18:48:45.000000 disunity-0.1.8/src/disunity/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:51:24.548002 disunity-0.1.8/src/disunity.egg-info/
+-rw-rw-rw-   0        0        0     2066 2024-05-21 18:51:24.000000 disunity-0.1.8/src/disunity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      620 2024-05-21 18:51:24.000000 disunity-0.1.8/src/disunity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 18:51:24.000000 disunity-0.1.8/src/disunity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-21 18:51:24.000000 disunity-0.1.8/src/disunity.egg-info/top_level.txt
```

### Comparing `disunity-0.1.7/LICENSE` & `disunity-0.1.8/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Duxle
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Duxle
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `disunity-0.1.7/PKG-INFO` & `disunity-0.1.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-Metadata-Version: 2.1
-Name: disunity
-Version: 0.1.7
-Summary: Python framework for Discord interactions using a web server
-Author: Tadeo Murillo, 
-Project-URL: Homepoge, https://github.com/murillotadeo/disunity
-Project-URL: Bug Tracker, https://github.com/murillotadeo/disunity/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# disunity
-
-Python framework for Discord interactions using a web server
-
-# Installation
-`pip install disunity`
-
-# Introduction to Disunity
-```python
-import disunity
-
-server = disunity.DisunityServer()
-
-if __name__ == '__main__':
-    server.run()
-```
-
-Using packages
-```python
-import disunity
-import pathlib
-
-server = disunity.DisunityServer()
-
-@server.before_serving
-def load_packages():
-    for package in [f"{f.parent}.{f.stem}" for f in pathlib.Path("packages").glob("*.py")]:
-        server.load_package(package)
-
-if __name__ == '__main__':
-    server.run()
-
-```
-
-# Setting up a package
-
-```python
-from disunity import package, utils
-
-class FirstPackage(package.Package):
-    def __init__(self, app):
-        self.app = app
-
-    @package.Package.command('ping')
-    async def ping(self, ctx):
-        return await ctx.callback("Pong!")
-
-def setup(app):
-    app.register_package(FirstPackage(app))
-
-```
-
-# Disclaimer
-
-This will require that you already have hosting service for the server to run on as well as a domain to host the server on. If you have neither of these, an alternative would be to host on Heroku using a web application with Gunicorn. 
-
-# Side note
-
-The server will receive interactions to the `/interactions` endpoint of your server. It will look like this: `https://example.com/interactions`. Once you run the server, put the url with the added interactions endpoint into the `interactions` URL on your app located in the Discord developer portal.
-
+Metadata-Version: 2.1
+Name: disunity
+Version: 0.1.8
+Summary: Python framework for Discord interactions using a web server
+Author: Tadeo Murillo, 
+Project-URL: Homepoge, https://github.com/murillotadeo/disunity
+Project-URL: Bug Tracker, https://github.com/murillotadeo/disunity/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# disunity
+
+Python framework for Discord interactions using a web server
+
+# Installation
+`pip install disunity`
+
+# Introduction to Disunity
+```python
+import disunity
+
+server = disunity.DisunityServer()
+
+if __name__ == '__main__':
+    server.run()
+```
+
+Using packages
+```python
+import disunity
+import pathlib
+
+server = disunity.DisunityServer()
+
+@server.before_serving
+def load_packages():
+    for package in [f"{f.parent}.{f.stem}" for f in pathlib.Path("packages").glob("*.py")]:
+        server.load_package(package)
+
+if __name__ == '__main__':
+    server.run()
+
+```
+
+# Setting up a package
+
+```python
+from disunity import package, utils
+
+class FirstPackage(package.Package):
+    def __init__(self, app):
+        self.app = app
+
+    @package.Package.command('ping')
+    async def ping(self, ctx):
+        return await ctx.callback("Pong!")
+
+def setup(app):
+    app.register_package(FirstPackage(app))
+
+```
+
+# Disclaimer
+
+This will require that you already have hosting service for the server to run on as well as a domain to host the server on. If you have neither of these, an alternative would be to host on Heroku using a web application with Gunicorn. 
+
+# Side note
+
+The server will receive interactions to the `/interactions` endpoint of your server. It will look like this: `https://example.com/interactions`. Once you run the server, put the url with the added interactions endpoint into the `interactions` URL on your app located in the Discord developer portal.
+
```

### Comparing `disunity-0.1.7/README.md` & `disunity-0.1.8/README.md`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-# disunity
-
-Python framework for Discord interactions using a web server
-
-# Installation
-`pip install disunity`
-
-# Introduction to Disunity
-```python
-import disunity
-
-server = disunity.DisunityServer()
-
-if __name__ == '__main__':
-    server.run()
-```
-
-Using packages
-```python
-import disunity
-import pathlib
-
-server = disunity.DisunityServer()
-
-@server.before_serving
-def load_packages():
-    for package in [f"{f.parent}.{f.stem}" for f in pathlib.Path("packages").glob("*.py")]:
-        server.load_package(package)
-
-if __name__ == '__main__':
-    server.run()
-
-```
-
-# Setting up a package
-
-```python
-from disunity import package, utils
-
-class FirstPackage(package.Package):
-    def __init__(self, app):
-        self.app = app
-
-    @package.Package.command('ping')
-    async def ping(self, ctx):
-        return await ctx.callback("Pong!")
-
-def setup(app):
-    app.register_package(FirstPackage(app))
-
-```
-
-# Disclaimer
-
-This will require that you already have hosting service for the server to run on as well as a domain to host the server on. If you have neither of these, an alternative would be to host on Heroku using a web application with Gunicorn. 
-
-# Side note
-
-The server will receive interactions to the `/interactions` endpoint of your server. It will look like this: `https://example.com/interactions`. Once you run the server, put the url with the added interactions endpoint into the `interactions` URL on your app located in the Discord developer portal.
-
+# disunity
+
+Python framework for Discord interactions using a web server
+
+# Installation
+`pip install disunity`
+
+# Introduction to Disunity
+```python
+import disunity
+
+server = disunity.DisunityServer()
+
+if __name__ == '__main__':
+    server.run()
+```
+
+Using packages
+```python
+import disunity
+import pathlib
+
+server = disunity.DisunityServer()
+
+@server.before_serving
+def load_packages():
+    for package in [f"{f.parent}.{f.stem}" for f in pathlib.Path("packages").glob("*.py")]:
+        server.load_package(package)
+
+if __name__ == '__main__':
+    server.run()
+
+```
+
+# Setting up a package
+
+```python
+from disunity import package, utils
+
+class FirstPackage(package.Package):
+    def __init__(self, app):
+        self.app = app
+
+    @package.Package.command('ping')
+    async def ping(self, ctx):
+        return await ctx.callback("Pong!")
+
+def setup(app):
+    app.register_package(FirstPackage(app))
+
+```
+
+# Disclaimer
+
+This will require that you already have hosting service for the server to run on as well as a domain to host the server on. If you have neither of these, an alternative would be to host on Heroku using a web application with Gunicorn. 
+
+# Side note
+
+The server will receive interactions to the `/interactions` endpoint of your server. It will look like this: `https://example.com/interactions`. Once you run the server, put the url with the added interactions endpoint into the `interactions` URL on your app located in the Discord developer portal.
+
```

### Comparing `disunity-0.1.7/src/disunity/cache.py` & `disunity-0.1.8/src/disunity/cache.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from .identifiers import (
-    Autocomplete,
-    CacheableSubCommand,
-    Command,
-    Component,
-    TopLevelSubCommand,
-)
-
-
-class ApplicationCache:
-    def __init__(self):
-        self.commands = dict()
-        self.components = dict()
-        self.autocompletes = dict()
-
-    def add_item(
-        self, incoming: TopLevelSubCommand | Command | Component | Autocomplete
-    ):
-        if isinstance(incoming, TopLevelSubCommand):
-            if "2" not in self.commands:
-                self.commands["2"] = {}  # Sub commands will always by type 2
-
-            if incoming.name in self.commands["2"]:
-                self.commands["2"][str(incoming.name)].add(incoming)
-            else:
-                cacheable = CacheableSubCommand(str(incoming.name)).add(incoming)
-                self.commands["2"][str(incoming.name)] = cacheable
-
-        elif isinstance(incoming, Command):
-            if str(incoming.command_type) not in self.commands:
-                self.commands[str(incoming.command_type)] = {}
-            self.commands[str(incoming.command_type)][incoming.name] = incoming
-
-        elif isinstance(incoming, Component):
-            self.components[str(incoming.name)] = incoming
-
-        elif isinstance(incoming, Autocomplete):
-            self.autocompletes[str(incoming.command_name)] = incoming
-
-        else:
-            raise TypeError
+from .identifiers import (
+    Autocomplete,
+    CacheableSubCommand,
+    Command,
+    Component,
+    TopLevelSubCommand,
+)
+
+
+class ApplicationCache:
+    def __init__(self):
+        self.commands = dict()
+        self.components = dict()
+        self.autocompletes = dict()
+
+    def add_item(
+        self, incoming: TopLevelSubCommand | Command | Component | Autocomplete
+    ):
+        if isinstance(incoming, TopLevelSubCommand):
+            if "2" not in self.commands:
+                self.commands["2"] = {}  # Sub commands will always by type 2
+
+            if incoming.name in self.commands["2"]:
+                self.commands["2"][str(incoming.name)].add(incoming)
+            else:
+                cacheable = CacheableSubCommand(str(incoming.name)).add(incoming)
+                self.commands["2"][str(incoming.name)] = cacheable
+
+        elif isinstance(incoming, Command):
+            if str(incoming.command_type) not in self.commands:
+                self.commands[str(incoming.command_type)] = {}
+            self.commands[str(incoming.command_type)][incoming.name] = incoming
+
+        elif isinstance(incoming, Component):
+            self.components[str(incoming.name)] = incoming
+
+        elif isinstance(incoming, Autocomplete):
+            self.autocompletes[str(incoming.command_name)] = incoming
+
+        else:
+            raise TypeError
```

### Comparing `disunity-0.1.7/src/disunity/embed.py` & `disunity-0.1.8/src/disunity/embed.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,131 +1,127 @@
-from __future__ import annotations
-
-
-class EmptyEmbedError(Exception):
-    def __init__(self, message):
-        super().__init__(message)
-
-
-class Embed:
-    def __init__(
-        self,
-        title: None | str = None,
-        description: None | str = None,
-        color: None | int = None,
-    ):
-        self.__json: dict = {"type": "rich", "color": color}
-
-        self._title: None | str = title
-        self._description: None | str = description
-        self._color: None | int = color
-
-        if self._title is not None:
-            self._title = str(self.title)
-            self.__json["title"] = self.title
-
-        if self._description is not None:
-            self.__json["description"] = str(self._description)
-
-    @property
-    def description(self) -> None | str:
-        return self._description
-
-    @description.setter
-    def description(self, value: None | str) -> None:
-        if value is not None:
-            value = str(value)
-        self._description = value
-        self.__json["description"] = value
-
-    @property
-    def color(self) -> None | int:
-        return self._color
-
-    @color.setter
-    def color(self, value: None | int) -> None:
-        self._color = value
-        self.__json["color"] = value
-
-    @property
-    def title(self) -> None | str:
-        return self._title
-
-    @title.setter
-    def title(self, value: None | str) -> None:
-        if value is not None:
-            value = str(value)
-        self._title = value
-        self.__json["title"] = value
-
-    @property
-    def fields(self) -> None | list[dict]:
-        return self.__json.get("fields", None)
-
-    def add_field(self, name: str, value: str, inline: bool = False) -> Embed:
-        if not bool(name) or not bool(value):
-            raise EmptyEmbedError("Embed field cannot contain an empty value")
-
-        if "fields" not in self.__json:
-            self.__json["fields"] = []
-
-        self.__json["fields"].append({"name": name, "value": value, "inline": inline})
-        return self
-
-    @property
-    def footer(self) -> None | dict:
-        return self.__json.get("footer", None)
-
-    def set_footer(self, text: None | str = None, icon_url: None | str = None) -> Embed:
-        if "footer" not in self.__json:
-            self.__json["footer"] = {}
-
-        if text is not None:
-            self.__json["footer"]["text"] = str(text)
-
-        if icon_url is not None:
-            self.__json["footer"]["icon_url"] = str(icon_url)
-
-        return self
-
-    @property
-    def image(self) -> None | dict:
-        return self.__json.get("url", None)
-
-    def set_image(self, image_url: str) -> Embed:
-        if "image" not in self.__json:
-            self.__json["image"] = {}
-
-        self.__json["image"]["url"] = str(image_url)
-        return self
-
-    @property
-    def thumbnail(self) -> None | dict:
-        return self.__json.get("thumbnail", None)
-
-    def set_thumbnail(self, thumbnail_url: str) -> Embed:
-        if "thumbnail" not in self.__json:
-            self.__json["thumbnail"] = {}
-
-        self.__json["thumbnail"]["url"] = str(thumbnail_url)
-        return self
-
-    @property
-    def author(self) -> None | dict:
-        return self.__json.get("author", None)
-
-    def set_author(
-        self, name: str, url: None | str = None, icon_url: None | str = None
-    ) -> Embed:
-        if "author" not in self.__json:
-            self.__json["author"] = {"name": str(name)}
-
-        if url is not None:
-            self.__json["author"]["url"] = str(url)
-
-        if icon_url is not None:
-            self.__json["author"]["icon_url"] = str(icon_url)
-
-        return self
-
-    def as_dict(self) -> dict:
-        return self.__json
+from __future__ import annotations
+
+
+class EmptyEmbedError(Exception):
+    def __init__(self, message):
+        super().__init__(message)
+
+
+class Embed:
+    def __init__(
+        self,
+        title: None | str = None,
+        description: None | str = None,
+        color: None | int = None,
+    ):
+        self.__json: dict = {"type": "rich", "color": color}
+
+        self._title: None | str = title
+        self._description: None | str = description
+        self._color: None | int = color
+
+        self.title = title
+        self.description = description
+
+    @property
+    def description(self) -> None | str:
+        return self._description
+
+    @description.setter
+    def description(self, value: None | str) -> None:
+        if value is not None:
+            value = str(value)
+        self._description = value
+        self.__json["description"] = value
+
+    @property
+    def color(self) -> None | int:
+        return self._color
+
+    @color.setter
+    def color(self, value: None | int) -> None:
+        self._color = value
+        self.__json["color"] = value
+
+    @property
+    def title(self) -> None | str:
+        return self._title
+
+    @title.setter
+    def title(self, value: None | str) -> None:
+        if value is not None:
+            value = str(value)
+        self._title = value
+        self.__json["title"] = value
+
+    @property
+    def fields(self) -> None | list[dict]:
+        return self.__json.get("fields", None)
+
+    def add_field(self, name: str, value: str, inline: bool = False) -> Embed:
+        if not bool(name) or not bool(value):
+            raise EmptyEmbedError("Embed field cannot contain an empty value")
+
+        if "fields" not in self.__json:
+            self.__json["fields"] = []
+
+        self.__json["fields"].append({"name": name, "value": value, "inline": inline})
+        return self
+
+    @property
+    def footer(self) -> None | dict:
+        return self.__json.get("footer", None)
+
+    def set_footer(self, text: None | str = None, icon_url: None | str = None) -> Embed:
+        if "footer" not in self.__json:
+            self.__json["footer"] = {}
+
+        if text is not None:
+            self.__json["footer"]["text"] = str(text)
+
+        if icon_url is not None:
+            self.__json["footer"]["icon_url"] = str(icon_url)
+
+        return self
+
+    @property
+    def image(self) -> None | dict:
+        return self.__json.get("url", None)
+
+    def set_image(self, image_url: str) -> Embed:
+        if "image" not in self.__json:
+            self.__json["image"] = {}
+
+        self.__json["image"]["url"] = str(image_url)
+        return self
+
+    @property
+    def thumbnail(self) -> None | dict:
+        return self.__json.get("thumbnail", None)
+
+    def set_thumbnail(self, thumbnail_url: str) -> Embed:
+        if "thumbnail" not in self.__json:
+            self.__json["thumbnail"] = {}
+
+        self.__json["thumbnail"]["url"] = str(thumbnail_url)
+        return self
+
+    @property
+    def author(self) -> None | dict:
+        return self.__json.get("author", None)
+
+    def set_author(
+        self, name: str, url: None | str = None, icon_url: None | str = None
+    ) -> Embed:
+        if "author" not in self.__json:
+            self.__json["author"] = {"name": str(name)}
+
+        if url is not None:
+            self.__json["author"]["url"] = str(url)
+
+        if icon_url is not None:
+            self.__json["author"]["icon_url"] = str(icon_url)
+
+        return self
+
+    def as_dict(self) -> dict:
+        return self.__json
```

### Comparing `disunity-0.1.7/src/disunity/identifiers.py` & `disunity-0.1.8/src/disunity/identifiers.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,178 +1,178 @@
-from datetime import datetime, timezone
-from typing import Callable
-
-
-class SubOption:
-    """
-    Represents a sub command option
-
-    Parameters
-    ----------
-    name : str
-        The name of the sub command
-    requires_ack : bool
-        Does the command need to be acked (response using followup). Default
-        to False
-    requires_ephemeral : bool
-        Only required if requires_ack is true. Sets the initial ack message
-        to show ephemerally so following responses can be ephemeral.
-    """
-
-    def __init__(
-        self, name: str, requires_ack: bool = False, requires_ephemeral: bool = False
-    ):
-        self.name: str = name
-        self.ack: bool = requires_ack
-        self.ephemeral: bool = requires_ephemeral
-
-
-class SubCommand(SubOption):
-    def __init__(
-        self,
-        name: str,
-        coroutine: Callable,
-        requires_ack: bool = False,
-        requires_ephemeral: bool = False,
-    ):
-        super().__init__(name, requires_ack, requires_ephemeral)
-        self.name: str = name
-        self.coroutine: Callable = coroutine
-
-    async def __call__(self, context):
-        try:
-            response = await self.coroutine(context)
-            if isinstance(response, dict):
-                return response
-        except Exception as e:
-            context._app.error_handler(e)
-
-
-class TopLevelSubCommand:
-    def __init__(
-        self,
-        name: str,
-        coroutine: Callable,
-        sub_commands: list[str] | list[SubCommand] | SubCommand | str = [],
-        group: str | None = None,
-    ):
-        self.name: str = name
-        self.coroutine: Callable = coroutine
-        self.sub_commands = []
-        self.group = group
-
-        if isinstance(sub_commands, str):
-            self.sub_commands.append(
-                SubCommand(sub_commands, self.coroutine, False, False)
-            )
-        elif isinstance(sub_commands, list):
-            for sub in sub_commands:
-                if isinstance(sub, str):
-                    self.sub_commands.append(
-                        SubCommand(sub, self.coroutine, False, False)
-                    )
-                elif isinstance(sub, SubOption):
-                    self.sub_commands.append(
-                        SubCommand(sub.name, self.coroutine, sub.ack, sub.ephemeral)
-                    )
-        elif isinstance(sub_commands, SubOption):
-            self.sub_commands.append(
-                SubCommand(
-                    sub_commands.name,
-                    self.coroutine,
-                    sub_commands.ack,
-                    sub_commands.ephemeral,
-                )
-            )
-
-
-class CacheableSubCommand:
-    def __init__(self, name: str):
-        self.name: str = name
-        self.map = {"sub_commands": {}}
-
-    def add(self, incoming: TopLevelSubCommand):
-        if incoming.group is not None:
-            self.map[str(incoming.group)] = {}
-            for sub in incoming.sub_commands:
-                self.map[str(incoming.group)][str(sub.name)] = sub
-        else:
-            for sub in incoming.sub_commands:
-                self.map["sub_commands"][str(sub.name)] = sub
-
-        return self
-
-
-class Component:
-    def __init__(
-        self,
-        name: str,
-        coroutine: Callable,
-        requires_ack: bool = False,
-        requires_ephemeral: bool = False,
-        timeout: float = 0.0,
-    ):
-        self.name: str = name
-        self.coroutine: Callable = coroutine
-        self.ack: bool = requires_ack
-        self.ephemeral: bool = requires_ephemeral
-        self.timeout: float | None = None if timeout <= 0.0 else timeout
-
-    async def __call__(self, context):
-        if isinstance(self.timeout, float):
-            if (
-                datetime.now(timezone.utc)
-                - datetime.fromisoformat(context.raw["message"]["timestamp"])
-            ).total_seconds() > self.timeout:
-                if not self.ack:
-                    return {
-                        "type": 4,
-                        "data": {
-                            "content": "This component has timed out.",
-                            "flags": 64,
-                        },
-                    }
-
-        try:
-            response = await self.coroutine(context)
-            if isinstance(response, dict):
-                return response
-        except Exception as e:
-            context._app.error_handler(e)
-
-
-class Command:
-    def __init__(
-        self,
-        name: str,
-        coroutine: Callable,
-        requires_ack: bool = False,
-        requires_ephemeral: bool = False,
-    ):
-        self.name: str = name
-        self.command_type: int = 2
-        self.coroutine: Callable = coroutine
-        self.ack: bool = requires_ack
-        self.ephemeral: bool = requires_ephemeral
-
-    async def __call__(self, context):
-        try:
-            response = await self.coroutine(context)
-            if isinstance(response, dict):
-                return response
-        except Exception as e:
-            context._app.error_handler(e)
-
-
-class Autocomplete:
-    def __init__(self, command_name: str, coroutine: Callable):
-        self.command_name: str = command_name
-        self.coroutine: Callable = coroutine
-
-    async def __call__(self, context):
-        try:
-            response = await self.coroutine(context)
-            if isinstance(response, list):
-                return response
-            return []
-        except Exception as e:
-            context._app.error_handler(e)
+from datetime import datetime, timezone
+from typing import Callable
+
+
+class SubOption:
+    """
+    Represents a sub command option
+
+    Parameters
+    ----------
+    name : str
+        The name of the sub command
+    requires_ack : bool
+        Does the command need to be acked (response using followup). Default
+        to False
+    requires_ephemeral : bool
+        Only required if requires_ack is true. Sets the initial ack message
+        to show ephemerally so following responses can be ephemeral.
+    """
+
+    def __init__(
+        self, name: str, requires_ack: bool = False, requires_ephemeral: bool = False
+    ):
+        self.name: str = name
+        self.ack: bool = requires_ack
+        self.ephemeral: bool = requires_ephemeral
+
+
+class SubCommand(SubOption):
+    def __init__(
+        self,
+        name: str,
+        coroutine: Callable,
+        requires_ack: bool = False,
+        requires_ephemeral: bool = False,
+    ):
+        super().__init__(name, requires_ack, requires_ephemeral)
+        self.name: str = name
+        self.coroutine: Callable = coroutine
+
+    async def __call__(self, context):
+        try:
+            response = await self.coroutine(context)
+            if isinstance(response, dict):
+                return response
+        except Exception as e:
+            context._app.error_handler(e)
+
+
+class TopLevelSubCommand:
+    def __init__(
+        self,
+        name: str,
+        coroutine: Callable,
+        sub_commands: list[str] | list[SubCommand] | SubCommand | str = [],
+        group: str | None = None,
+    ):
+        self.name: str = name
+        self.coroutine: Callable = coroutine
+        self.sub_commands = []
+        self.group = group
+
+        if isinstance(sub_commands, str):
+            self.sub_commands.append(
+                SubCommand(sub_commands, self.coroutine, False, False)
+            )
+        elif isinstance(sub_commands, list):
+            for sub in sub_commands:
+                if isinstance(sub, str):
+                    self.sub_commands.append(
+                        SubCommand(sub, self.coroutine, False, False)
+                    )
+                elif isinstance(sub, SubOption):
+                    self.sub_commands.append(
+                        SubCommand(sub.name, self.coroutine, sub.ack, sub.ephemeral)
+                    )
+        elif isinstance(sub_commands, SubOption):
+            self.sub_commands.append(
+                SubCommand(
+                    sub_commands.name,
+                    self.coroutine,
+                    sub_commands.ack,
+                    sub_commands.ephemeral,
+                )
+            )
+
+
+class CacheableSubCommand:
+    def __init__(self, name: str):
+        self.name: str = name
+        self.map = {"sub_commands": {}}
+
+    def add(self, incoming: TopLevelSubCommand):
+        if incoming.group is not None:
+            self.map[str(incoming.group)] = {}
+            for sub in incoming.sub_commands:
+                self.map[str(incoming.group)][str(sub.name)] = sub
+        else:
+            for sub in incoming.sub_commands:
+                self.map["sub_commands"][str(sub.name)] = sub
+
+        return self
+
+
+class Component:
+    def __init__(
+        self,
+        name: str,
+        coroutine: Callable,
+        requires_ack: bool = False,
+        requires_ephemeral: bool = False,
+        timeout: float = 0.0,
+    ):
+        self.name: str = name
+        self.coroutine: Callable = coroutine
+        self.ack: bool = requires_ack
+        self.ephemeral: bool = requires_ephemeral
+        self.timeout: float | None = None if timeout <= 0.0 else timeout
+
+    async def __call__(self, context):
+        if isinstance(self.timeout, float):
+            if (
+                datetime.now(timezone.utc)
+                - datetime.fromisoformat(context.raw["message"]["timestamp"])
+            ).total_seconds() > self.timeout:
+                if not self.ack:
+                    return {
+                        "type": 4,
+                        "data": {
+                            "content": "This component has timed out.",
+                            "flags": 64,
+                        },
+                    }
+
+        try:
+            response = await self.coroutine(context)
+            if isinstance(response, dict):
+                return response
+        except Exception as e:
+            context._app.error_handler(e)
+
+
+class Command:
+    def __init__(
+        self,
+        name: str,
+        coroutine: Callable,
+        requires_ack: bool = False,
+        requires_ephemeral: bool = False,
+    ):
+        self.name: str = name
+        self.command_type: int = 2
+        self.coroutine: Callable = coroutine
+        self.ack: bool = requires_ack
+        self.ephemeral: bool = requires_ephemeral
+
+    async def __call__(self, context):
+        try:
+            response = await self.coroutine(context)
+            if isinstance(response, dict):
+                return response
+        except Exception as e:
+            context._app.error_handler(e)
+
+
+class Autocomplete:
+    def __init__(self, command_name: str, coroutine: Callable):
+        self.command_name: str = command_name
+        self.coroutine: Callable = coroutine
+
+    async def __call__(self, context):
+        try:
+            response = await self.coroutine(context)
+            if isinstance(response, list):
+                return response
+            return []
+        except Exception as e:
+            context._app.error_handler(e)
```

### Comparing `disunity-0.1.7/src/disunity/models/context.py` & `disunity-0.1.8/src/disunity/models/context.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,127 +1,147 @@
-from .. import embed, errors, utils
-from .components import ActionRow, Modal
-from .interaction import Interaction
-from .message import Message
-
-
-class Context(Interaction):
-    def __init__(self, app, received: dict):
-        super().__init__(received)
-        self._app = app
-        self.acked: bool = False
-        self.options = {}
-
-        if "data" in received:
-            for option in received["data"].get("injected", []):
-                self.options[option["name"]] = option["value"]
-
-    async def callback(
-        self,
-        content: None | str = None,
-        embeds: list[embed.Embed] | embed.Embed = [],
-        components: list[ActionRow] | ActionRow = [],
-        ephemeral: bool = False,
-        response_type: int = utils.InteractionCallbackTypes.CHANNEL_MESSAGE_WITH_SOURCE,
-    ) -> dict:
-        """
-        Creates the first interation response.
-
-        Parameters
-        ----------
-        content: str
-            The content of the message
-        embeds: List[disunity.Embed] | disunity.Embed
-            List of embeds to send, will all be shown at once
-        components: List[ActionRow] | ActionRow:
-            List of components to send.
-        allowed_mentions: list
-            Allowed mentions of the message
-        ephemeral: bool
-            Will the message show publically or privately
-        response_type: int
-            Callback interaction type
-        """
-
-        if isinstance(embeds, embed.Embed):
-            embeds = [embeds]
-        if isinstance(components, ActionRow):
-            components = [components]
-
-        message_body = {
-            "type": response_type,
-            "data": {
-                "content": str(content) if content is not None else "",
-                "embeds": [e.as_dict() for e in embeds if isinstance(e, embed.Embed)],
-                "components": [
-                    row.to_dict() for row in components if isinstance(row, ActionRow)
-                ],
-            },
-        }
-
-        if ephemeral:
-            message_body["data"]["flags"] = 64
-
-        self.acked = True
-        return message_body
-
-    async def followup(
-        self,
-        content: None | str = None,
-        embeds: list[embed.Embed] | embed.Embed = [],
-        components: list[ActionRow] | ActionRow = [],
-        ephemeral: bool = False,
-    ) -> Message:
-        """
-        Used to create a follow up response to an already acked interaction.
-        Parameters
-        ----------
-        content: str
-            The content of the message
-        embeds: List[disunity.Embed] | disunity.Embed
-            List of embeds to send, will all be shown at once
-        components: List[ActionRow] | ActionRow:
-            List of components to send with the message
-        ephemeral: bool
-            Will the message show publically or privately
-        """
-
-        if not self.acked:
-            raise errors.InvalidMethodUse(
-                "Cannot followup an interaction that hasn't been acked"
-            )
-
-        if isinstance(embeds, embed.Embed):
-            embeds = [embeds]
-        if isinstance(components, ActionRow):
-            components = [components]
-
-        message_body = {
-            "content": str(content) if content is not None else "",
-            "embeds": [e.as_dict() for e in embeds if isinstance(e, embed.Embed)],
-            "components": [
-                row.to_dict() for row in components if isinstance(row, ActionRow)
-            ],
-        }
-
-        if ephemeral:
-            message_body["flags"] = 64
-
-        maybe_message = await self._app.make_https_request(
-            "POST",
-            f"webhooks/{self._app.config['CLIENT_ID']}/{self.token}",
-            payload=message_body,
-        )
-
-        return Message(maybe_message, self._app, self.token)
-
-    async def modal_response(self, modal: Modal):
-        """
-        Responds to the interaction with a modal.
-
-        Parameters
-        ----------
-        modal : components.Modal
-            The modal to respond with.
-        """
-
-        return {"type": utils.InteractionCallbackTypes.MODAL, "data": modal.to_dict()}
+from .. import embed, errors, utils
+from .components import ActionRow, Modal
+from .interaction import Interaction
+from .message import Message
+from .attachment import Attachment
+
+
+class Context(Interaction):
+    def __init__(self, app, received: dict):
+        super().__init__(received)
+        self._app = app
+        self.acked: bool = False
+        self.options = {}
+
+        if "data" in received:
+            for option in received["data"].get("injected", []):
+                self.options[option["name"]] = option["value"]
+
+    async def callback(
+        self,
+        content: None | str = None,
+        embeds: list[embed.Embed] | embed.Embed = [],
+        components: list[ActionRow] | ActionRow = [],
+        ephemeral: bool = False,
+        response_type: int = utils.InteractionCallbackTypes.CHANNEL_MESSAGE_WITH_SOURCE,
+    ) -> dict:
+        """
+        Creates the first interation response.
+
+        Parameters
+        ----------
+        content: str
+            The content of the message
+        embeds: List[disunity.Embed] | disunity.Embed
+            List of embeds to send, will all be shown at once
+        components: List[ActionRow] | ActionRow:
+            List of components to send.
+        allowed_mentions: list
+            Allowed mentions of the message
+        ephemeral: bool
+            Will the message show publically or privately
+        response_type: int
+            Callback interaction type
+        """
+
+        if isinstance(embeds, embed.Embed):
+            embeds = [embeds]
+        if isinstance(components, ActionRow):
+            components = [components]
+
+        message_body = {
+            "type": response_type,
+            "data": {
+                "content": str(content) if content is not None else "",
+                "embeds": [e.as_dict() for e in embeds if isinstance(e, embed.Embed)],
+                "components": [
+                    row.to_dict() for row in components if isinstance(row, ActionRow)
+                ],
+            },
+        }
+
+        if ephemeral:
+            message_body["data"]["flags"] = 64
+
+        self.acked = True
+        return message_body
+
+    async def followup(
+        self,
+        content: None | str = None,
+        embeds: list[embed.Embed] | embed.Embed = [],
+        components: list[ActionRow] | ActionRow = [],
+        attachments: list[Attachment] | Attachment = [],
+        ephemeral: bool = False,
+    ) -> Message:
+        """
+        Used to create a follow up response to an already acked interaction.
+        Parameters
+        ----------
+        content: str
+            The content of the message
+        embeds: List[disunity.Embed] | disunity.Embed
+            List of embeds to send, will all be shown at once
+        components: List[ActionRow] | ActionRow:
+            List of components to send with the message
+        attachments: List[Attachment] | Attachment
+            List of attachments to send with the message
+        ephemeral: bool
+            Will the message show publically or privately
+        """
+
+        if not self.acked:
+            raise errors.InvalidMethodUse(
+                "Cannot followup an interaction that hasn't been acked"
+            )
+
+        if isinstance(embeds, embed.Embed):
+            embeds = [embeds]
+        if isinstance(components, ActionRow):
+            components = [components]
+        if isinstance(attachments, Attachment):
+            attachments = [attachments]
+
+        message_body = {
+            "content": str(content) if content is not None else "",
+            "embeds": [e.as_dict() for e in embeds if isinstance(e, embed.Embed)],
+            "components": [
+                row.to_dict() for row in components if isinstance(row, ActionRow)
+            ],
+            "attachments": [
+                {"id": i, "filename": att.filename, "description": att.description}
+                for i, att in enumerate(attachments)
+                if isinstance(att, Attachment)
+            ],
+        }
+
+        if ephemeral:
+            message_body["flags"] = 64
+
+        files = None
+        if attachments:
+            files = [
+                {"id": i, "filename": att.filename, "content": att.content}
+                for i, att in enumerate(attachments)
+                if isinstance(att, Attachment)
+            ]
+
+        maybe_message = await self._app.make_https_request(
+            "POST",
+            f"webhooks/{self._app.config['CLIENT_ID']}/{self.token}",
+            payload=message_body,
+            files=files,
+        )
+
+        return Message(maybe_message, self._app, self.token)
+
+    async def modal_response(self, modal: Modal):
+        """
+        Responds to the interaction with a modal.
+
+        Parameters
+        ----------
+        modal : components.Modal
+            The modal to respond with.
+        """
+
+        return {"type": utils.InteractionCallbackTypes.MODAL, "data": modal.to_dict()}
```

### Comparing `disunity-0.1.7/src/disunity/models/interaction.py` & `disunity-0.1.8/src/disunity/models/interaction.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from .. import utils
-from ..errors import InvalidMethodUse
-from .member import Member
-from .user import User
-
-
-class Interaction:
-    def __init__(self, received):
-        self.raw: dict = received
-        self.app_permissions: int = int(received.get("app_permissions", 0))
-
-        self.channel_id: int = int(received["channel_id"])
-        self.id: int = int(received["id"])
-        self.locale: str = received["locale"]
-        self.token: str = received["token"]
-        self.interaction_type: int = int(received["type"])
-        self.data: dict = received["data"]
-        self.resolved: None | dict = self.data.get("resolved", None)
-        self.component_type: None | int = self.data.get("component_type", None)
-        self.custom_id: None | str = self.data.get("custom_id", None)
-        self.values: list = self.data.get("values", [])
-        self.member: None | Member = None
-        self.used_by: None | User = None
-        self.command_name: str = self.data.get("name", None)
-        self.modal_values: None | list[dict] = None
-
-        if "member" in received:  # Not a DM command
-            self.invoked_by: User = User(received["member"]["user"])
-            self.member = Member(received["member"])
-        else:
-            self.invoked_by: User = User(received["user"])
-
-        if (
-            self.interaction_type == utils.InteractionTypes.MESSAGE_COMPONENT
-        ):  # Component
-            if "interaction" in received["message"]:
-                self.invoked_by: User = User(received["message"]["interaction"]["user"])
-            else:
-                self.invoked_by: User = None
-            if "member" in received:
-                self.used_by: None | User = User(received["member"]["user"])
-            else:
-                self.used_by: None | User = User(received["user"])
-
-        elif (
-            self.interaction_type == utils.InteractionTypes.MODAL_SUBMIT
-        ):  # modal submit
-            self.modal_values: None | list[dict] = self.data["components"][0][
-                "components"
-            ]
-
-    def check_user(self) -> bool:
-        """
-        For components, checks if the component user and
-        the interaction author are the same.
-        """
-
-        if self.interaction_type != utils.InteractionTypes.MESSAGE_COMPONENT:
-            raise InvalidMethodUse("Interaction is not a component interaction")
-
-        if self.invoked_by.id == self.used_by.id:
-            return True
-        return False
+from .. import utils
+from ..errors import InvalidMethodUse
+from .member import Member
+from .user import User
+
+
+class Interaction:
+    def __init__(self, received):
+        self.raw: dict = received
+        self.app_permissions: int = int(received.get("app_permissions", 0))
+
+        self.channel_id: int = int(received["channel_id"])
+        self.id: int = int(received["id"])
+        self.locale: str = received["locale"]
+        self.token: str = received["token"]
+        self.interaction_type: int = int(received["type"])
+        self.data: dict = received["data"]
+        self.resolved: None | dict = self.data.get("resolved", None)
+        self.component_type: None | int = self.data.get("component_type", None)
+        self.custom_id: None | str = self.data.get("custom_id", None)
+        self.values: list = self.data.get("values", [])
+        self.member: None | Member = None
+        self.used_by: None | User = None
+        self.command_name: str = self.data.get("name", None)
+        self.modal_values: None | list[dict] = None
+
+        if "member" in received:  # Not a DM command
+            self.invoked_by: User = User(received["member"]["user"])
+            self.member = Member(received["member"])
+        else:
+            self.invoked_by: User = User(received["user"])
+
+        if (
+            self.interaction_type == utils.InteractionTypes.MESSAGE_COMPONENT
+        ):  # Component
+            if "interaction" in received["message"]:
+                self.invoked_by: User = User(received["message"]["interaction"]["user"])
+            else:
+                self.invoked_by: User = None
+            if "member" in received:
+                self.used_by: None | User = User(received["member"]["user"])
+            else:
+                self.used_by: None | User = User(received["user"])
+
+        elif (
+            self.interaction_type == utils.InteractionTypes.MODAL_SUBMIT
+        ):  # modal submit
+            self.modal_values: None | list[dict] = self.data["components"][0][
+                "components"
+            ]
+
+    def check_user(self) -> bool:
+        """
+        For components, checks if the component user and
+        the interaction author are the same.
+        """
+
+        if self.interaction_type != utils.InteractionTypes.MESSAGE_COMPONENT:
+            raise InvalidMethodUse("Interaction is not a component interaction")
+
+        if self.invoked_by.id == self.used_by.id:
+            return True
+        return False
```

### Comparing `disunity-0.1.7/src/disunity/models/member.py` & `disunity-0.1.8/src/disunity/models/member.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from .. import utils
-from .user import User
-
-
-class Member:
-    def __init__(self, received: dict):
-        self.raw: dict = received
-        self.deaf: bool = received["deaf"]
-        self.pending: bool = received.get("pending", False)
-        self.joined_at = received["joined_at"]
-        self.mute: bool = received["mute"]
-        self.nick: str = received["nick"]
-        self.permissions: int = int(received.get("permissions", 0))
-        self.roles: list[int] = [int(role) for role in received["roles"]]
-        self.user: User = User(received["user"])
-        self.flags: int = int(received["flags"])
-
-    @property
-    def server_avatar_url(self) -> None | str:
-        if self.raw["avatar"] != "None":
-            return utils.return_avatar_as_cdn(self.raw["avatar"], self.user.id)
-        return None
+from .. import utils
+from .user import User
+
+
+class Member:
+    def __init__(self, received: dict):
+        self.raw: dict = received
+        self.deaf: bool = received["deaf"]
+        self.pending: bool = received.get("pending", False)
+        self.joined_at = received["joined_at"]
+        self.mute: bool = received["mute"]
+        self.nick: str = received["nick"]
+        self.permissions: int = int(received.get("permissions", 0))
+        self.roles: list[int] = [int(role) for role in received["roles"]]
+        self.user: User = User(received["user"])
+        self.flags: int = int(received["flags"])
+
+    @property
+    def server_avatar_url(self) -> None | str:
+        if self.raw["avatar"] != "None":
+            return utils.return_avatar_as_cdn(self.raw["avatar"], self.user.id)
+        return None
```

### Comparing `disunity-0.1.7/src/disunity/models/message.py` & `disunity-0.1.8/src/disunity/models/message.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,128 +1,129 @@
-from __future__ import annotations
-
-from ..embed import Embed
-from .components import ActionRow
-from .user import User
-
-
-class MissingTokenError(Exception):
-    def __init__(self, func_name):
-        super().__init__(f"A bot token is required to use the {func_name} method")
-
-
-class ExpiredInteractionError(Exception):
-    def __init__(self):
-        super().__init__(
-            "The token belonging to this interaction has expired or leads to an unkown webhook"
-        )
-
-
-class Message:
-    def __init__(self, raw_message, server, token=None):
-        self.server = server
-        self.raw: dict = raw_message
-        self.id: int = int(raw_message["id"])
-        self.author: User | dict = raw_message.get("author", None)
-        if self.author is not None:
-            self.author: User | dict = User(self.author)
-
-        self.channel_id: int = raw_message["channel_id"]
-        self.components: list[dict] | list = raw_message["components"]
-        self.embeds: list | list[dict] = raw_message["embeds"]
-        self.content: str = raw_message["content"]
-        self.interaction_token: str | None = token
-
-    def remake(self, new_raw):
-        self.raw = new_raw
-        self.content = self.raw["content"]
-        self.embeds = self.raw["embeds"]
-        self.components = self.raw["components"]
-
-    async def edit_as_webhook(
-        self,
-        content: None | str = None,
-        embeds: None | list[Embed] | Embed = None,
-        components: None | list[ActionRow] | ActionRow = None,
-    ) -> Message:
-        if isinstance(embeds, Embed):
-            embeds = [embeds]
-        if isinstance(components, ActionRow):
-            components = [components]
-
-        message_body = self.raw
-        message_body["content"] = str(content) if content is not None else self.content
-        message_body["embeds"] = (
-            [emb.as_dict() for emb in embeds if isinstance(emb, Embed)]
-            if embeds is not None
-            else self.embeds
-        )
-        message_body["components"] = (
-            [row.to_dict() for row in components if isinstance(row, ActionRow)]
-            if components is not None
-            else self.components
-        )
-
-        attempt = await self.server.make_https_request(
-            "PATCH",
-            f"webhooks/{self.server.config['CLIENT_ID']}/{self.interaction_token}/messages/{self.id}",
-            payload=message_body,
-            override_checks=True,
-        )
-
-        if not str(attempt.status).startswith("20"):
-            recv = await attempt.json()
-            if recv["code"] in [10015, 50027]:
-                raise ExpiredInteractionError
-
-        self.remake(message_body)
-        return self
-
-    async def edit_as_bot(
-        self,
-        content: None | str = None,
-        embeds: None | list[Embed] | Embed = None,
-        components: None | list[ActionRow] | ActionRow = None,
-    ) -> Message:
-        if self.server.config["BOT_TOKEN"] is None:
-            raise MissingTokenError("Message.edit_as_bot")
-
-        if isinstance(embeds, Embed):
-            embeds = [embeds]
-        if isinstance(components, ActionRow):
-            components = [components]
-
-        message_body = self.raw
-        message_body["content"] = str(content) if content is not None else self.content
-        message_body["embeds"] = (
-            [emb.as_dict() for emb in embeds if isinstance(emb, Embed)]
-            if embeds is not None
-            else self.embeds
-        )
-        message_body["components"] = (
-            [row.to_dict() for row in components if isinstance(row, ActionRow)]
-            if components is not None
-            else self.components
-        )
-
-        await self.server.make_https_request(
-            "PATCH",
-            f"channels/{self.channel_id}/messages/{self.id}",
-            payload=message_body,
-        )
-
-        self.remake(message_body)
-        return self
-
-    async def delete_as_webhook(self):
-        await self.server.make_https_request(
-            "DELETE",
-            f"webhooks/{self.server.config['CLIENT_ID']}/{self.interaction_token}/messages/{self.id}",
-        )
-
-    async def delete_as_bot(self):
-        if self.server.config["BOT_TOKEN"] is None:
-            raise MissingTokenError("Message.delete_as_bot")
-
-        await self.server.make_https_request(
-            "DELETE", f"channels/{self.channel_id}/messages/{self.id}"
-        )
+from __future__ import annotations
+
+from ..embed import Embed
+from .components import ActionRow
+from .user import User
+
+
+class MissingTokenError(Exception):
+    def __init__(self, func_name):
+        super().__init__(f"A bot token is required to use the {func_name} method")
+
+
+class ExpiredInteractionError(Exception):
+    def __init__(self):
+        super().__init__(
+            "The token belonging to this interaction has expired or leads to an unkown webhook"
+        )
+
+
+class Message:
+    def __init__(self, raw_message, server, token=None):
+        self.server = server
+        self.raw: dict = raw_message
+        self.id: int = int(raw_message["id"])
+        self.author: User | dict = raw_message.get("author", None)
+        if self.author is not None:
+            self.author: User | dict = User(self.author)
+
+        self.channel_id: int = raw_message["channel_id"]
+        self.components: list[dict] | list = raw_message["components"]
+        self.embeds: list | list[dict] = raw_message["embeds"]
+        self.attachments: list | list[dict] = raw_message.get("attachements")
+        self.content: str = raw_message["content"]
+        self.interaction_token: str | None = token
+
+    def remake(self, new_raw):
+        self.raw = new_raw
+        self.content = self.raw["content"]
+        self.embeds = self.raw["embeds"]
+        self.components = self.raw["components"]
+
+    async def edit_as_webhook(
+        self,
+        content: None | str = None,
+        embeds: None | list[Embed] | Embed = None,
+        components: None | list[ActionRow] | ActionRow = None,
+    ) -> Message:
+        if isinstance(embeds, Embed):
+            embeds = [embeds]
+        if isinstance(components, ActionRow):
+            components = [components]
+
+        message_body = self.raw
+        message_body["content"] = str(content) if content is not None else self.content
+        message_body["embeds"] = (
+            [emb.as_dict() for emb in embeds if isinstance(emb, Embed)]
+            if embeds is not None
+            else self.embeds
+        )
+        message_body["components"] = (
+            [row.to_dict() for row in components if isinstance(row, ActionRow)]
+            if components is not None
+            else self.components
+        )
+
+        attempt = await self.server.make_https_request(
+            "PATCH",
+            f"webhooks/{self.server.config['CLIENT_ID']}/{self.interaction_token}/messages/{self.id}",
+            payload=message_body,
+            override_checks=True,
+        )
+
+        if not str(attempt.status).startswith("20"):
+            recv = await attempt.json()
+            if recv["code"] in [10015, 50027]:
+                raise ExpiredInteractionError
+
+        self.remake(message_body)
+        return self
+
+    async def edit_as_bot(
+        self,
+        content: None | str = None,
+        embeds: None | list[Embed] | Embed = None,
+        components: None | list[ActionRow] | ActionRow = None,
+    ) -> Message:
+        if self.server.config["BOT_TOKEN"] is None:
+            raise MissingTokenError("Message.edit_as_bot")
+
+        if isinstance(embeds, Embed):
+            embeds = [embeds]
+        if isinstance(components, ActionRow):
+            components = [components]
+
+        message_body = self.raw
+        message_body["content"] = str(content) if content is not None else self.content
+        message_body["embeds"] = (
+            [emb.as_dict() for emb in embeds if isinstance(emb, Embed)]
+            if embeds is not None
+            else self.embeds
+        )
+        message_body["components"] = (
+            [row.to_dict() for row in components if isinstance(row, ActionRow)]
+            if components is not None
+            else self.components
+        )
+
+        await self.server.make_https_request(
+            "PATCH",
+            f"channels/{self.channel_id}/messages/{self.id}",
+            payload=message_body,
+        )
+
+        self.remake(message_body)
+        return self
+
+    async def delete_as_webhook(self):
+        await self.server.make_https_request(
+            "DELETE",
+            f"webhooks/{self.server.config['CLIENT_ID']}/{self.interaction_token}/messages/{self.id}",
+        )
+
+    async def delete_as_bot(self):
+        if self.server.config["BOT_TOKEN"] is None:
+            raise MissingTokenError("Message.delete_as_bot")
+
+        await self.server.make_https_request(
+            "DELETE", f"channels/{self.channel_id}/messages/{self.id}"
+        )
```

### Comparing `disunity-0.1.7/src/disunity/package.py` & `disunity-0.1.8/src/disunity/package.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-from __future__ import annotations
-
-import inspect
-
-from .identifiers import Autocomplete, Command, Component, SubOption, TopLevelSubCommand
-
-
-class Package:
-    def __init__(self):
-        self.commands = []
-        self.components = []
-
-    @classmethod
-    def command(
-        cls, name: str, requires_ack: bool = False, requires_ephemeral: bool = False
-    ):
-        """
-        Declare a command within the application.
-
-        Parameters
-        ----------
-        name : str
-            The command name
-        requires_ack : bool
-            Does the command need to be acked before the first response.
-            Defaulted to False.
-        requires_ephemeral : bool
-            Only applicable if requires_ack is True. Acks the command
-            using an ephemeral response. Default to False.
-        """
-
-        def decorator(coroutine):
-            actual = coroutine
-
-            if isinstance(actual, staticmethod):
-                actual = actual.__func__
-
-            if not inspect.iscoroutinefunction(actual):
-                raise TypeError("Command methods must be coroutine")
-
-            actual.__command__ = True
-            actual.__component__ = False
-            actual.__subcommand__ = False
-            actual.__autocomplete__ = False
-            actual.__data__ = (name, requires_ack, requires_ephemeral)
-
-            return actual
-
-        return decorator
-
-    @classmethod
-    def component(
-        cls,
-        name: str,
-        requires_ack: bool = False,
-        requires_ephemeral: bool = False,
-        timeout: float = 0.0,
-    ):
-        """ "
-        Declares a component object within the application
-
-        Parameters
-        ----------
-        name : str
-            The name of the component. Will be gathered in the format
-            component_name-<unique tag for this component, preferably
-            the interaction id>.
-        requires_ack : bool
-            Does the interaction need to be acked before the first response
-            Default to False.
-        requires_ephemeral : bool
-            Only applicable if requires_ack is True. Acks the interaction
-            using an ephemeral response.
-        timeout : float
-            The component timeout. Default to 0.0.
-        """
-
-        def decorator(coroutine):
-            actual = coroutine
-
-            if isinstance(actual, staticmethod):
-                actual = actual.__func__
-
-            if not inspect.iscoroutinefunction(actual):
-                raise TypeError("Component methods must be coroutine")
-
-            actual.__command__ = False
-            actual.__component__ = True
-            actual.__subcommand__ = False
-            actual.__autocomplete__ = False
-            actual.__data__ = (name, requires_ack, requires_ephemeral, timeout)
-
-            return actual
-
-        return decorator
-
-    @classmethod
-    def sub(
-        cls,
-        name: str,
-        sub_commands: list[str | SubOption] | str | SubOption,
-        group: None | str = None,
-    ):
-        """
-        Declares a sub command within the application
-
-        Parameters
-        ----------
-        name : str
-            The name of the command base.
-        sub_commands : list[str | SubOption] | str | SubOption
-            The sub command options that this command has.
-        group : str | None
-            The group that the sub commands belong to. Defaults to None.
-        """
-
-        def decorator(coroutine):
-            actual = coroutine
-            if isinstance(actual, staticmethod):
-                actual = actual.__func__
-
-            if not inspect.iscoroutinefunction(actual):
-                raise TypeError("Sub command methods must be coroutine")
-
-            actual.__command__ = False
-            actual.__component__ = False
-            actual.__subcommand__ = True
-            actual.__autocomplete__ = False
-            actual.__data__ = (name, sub_commands, group)
-
-            return actual
-
-        return decorator
-
-    @classmethod
-    def autocomplete(cls, command_name: str):
-        """
-        Declares a autocomplete function for a command
-
-        Should return a list of option choices
-
-        Parameters
-        ----------
-        command_name : str
-            Name of the command this autocomplete belongs to
-
-        Example
-        -------
-        @Package.autocomplete("command")
-
-        async def command_autocomplete(self, ctx: Context):
-            return [
-                {
-                    "name": "Blue",
-                    "value": "blue"
-                }
-            ]
-        """
-
-        def decorator(coroutine):
-            actual = coroutine
-
-            if isinstance(actual, staticmethod):
-                actual = actual.__func__
-
-            if not inspect.iscoroutinefunction(actual):
-                raise TypeError("Autocomplete methods must be coroutine")
-
-            actual.__command__ = False
-            actual.__component__ = False
-            actual.__subcommand__ = False
-            actual.__autocomplete__ = True
-            actual.__data__ = (command_name,)
-
-            return actual
-
-        return decorator
-
-    def unpack(self):
-        to_return = []
-
-        for meth in [
-            attr[1]
-            for attr in inspect.getmembers(self, inspect.iscoroutinefunction)
-            if not attr[0].startswith("__") and not attr[0].endswith("__")
-        ]:
-            try:
-                d = meth.__data__
-
-                if meth.__command__:
-                    to_return.append(Command(d[0], meth, d[1], d[2]))
-
-                elif meth.__component__:
-                    to_return.append(Component(d[0], meth, d[1], d[2], d[3]))
-
-                elif meth.__subcommand__:
-                    to_return.append(TopLevelSubCommand(d[0], meth, d[1], d[2]))
-
-                elif meth.__autocomplete__:
-                    to_return.append(Autocomplete(d[0], meth))
-
-            except AttributeError:
-                continue
-
-        return to_return
+from __future__ import annotations
+
+import inspect
+
+from .identifiers import Autocomplete, Command, Component, SubOption, TopLevelSubCommand
+
+
+class Package:
+    def __init__(self):
+        self.commands = []
+        self.components = []
+
+    @classmethod
+    def command(
+        cls, name: str, requires_ack: bool = False, requires_ephemeral: bool = False
+    ):
+        """
+        Declare a command within the application.
+
+        Parameters
+        ----------
+        name : str
+            The command name
+        requires_ack : bool
+            Does the command need to be acked before the first response.
+            Defaulted to False.
+        requires_ephemeral : bool
+            Only applicable if requires_ack is True. Acks the command
+            using an ephemeral response. Default to False.
+        """
+
+        def decorator(coroutine):
+            actual = coroutine
+
+            if isinstance(actual, staticmethod):
+                actual = actual.__func__
+
+            if not inspect.iscoroutinefunction(actual):
+                raise TypeError("Command methods must be coroutine")
+
+            actual.__command__ = True
+            actual.__component__ = False
+            actual.__subcommand__ = False
+            actual.__autocomplete__ = False
+            actual.__data__ = (name, requires_ack, requires_ephemeral)
+
+            return actual
+
+        return decorator
+
+    @classmethod
+    def component(
+        cls,
+        name: str,
+        requires_ack: bool = False,
+        requires_ephemeral: bool = False,
+        timeout: float = 0.0,
+    ):
+        """ "
+        Declares a component object within the application
+
+        Parameters
+        ----------
+        name : str
+            The name of the component. Will be gathered in the format
+            component_name-<unique tag for this component, preferably
+            the interaction id>.
+        requires_ack : bool
+            Does the interaction need to be acked before the first response
+            Default to False.
+        requires_ephemeral : bool
+            Only applicable if requires_ack is True. Acks the interaction
+            using an ephemeral response.
+        timeout : float
+            The component timeout. Default to 0.0.
+        """
+
+        def decorator(coroutine):
+            actual = coroutine
+
+            if isinstance(actual, staticmethod):
+                actual = actual.__func__
+
+            if not inspect.iscoroutinefunction(actual):
+                raise TypeError("Component methods must be coroutine")
+
+            actual.__command__ = False
+            actual.__component__ = True
+            actual.__subcommand__ = False
+            actual.__autocomplete__ = False
+            actual.__data__ = (name, requires_ack, requires_ephemeral, timeout)
+
+            return actual
+
+        return decorator
+
+    @classmethod
+    def sub(
+        cls,
+        name: str,
+        sub_commands: list[str | SubOption] | str | SubOption,
+        group: None | str = None,
+    ):
+        """
+        Declares a sub command within the application
+
+        Parameters
+        ----------
+        name : str
+            The name of the command base.
+        sub_commands : list[str | SubOption] | str | SubOption
+            The sub command options that this command has.
+        group : str | None
+            The group that the sub commands belong to. Defaults to None.
+        """
+
+        def decorator(coroutine):
+            actual = coroutine
+            if isinstance(actual, staticmethod):
+                actual = actual.__func__
+
+            if not inspect.iscoroutinefunction(actual):
+                raise TypeError("Sub command methods must be coroutine")
+
+            actual.__command__ = False
+            actual.__component__ = False
+            actual.__subcommand__ = True
+            actual.__autocomplete__ = False
+            actual.__data__ = (name, sub_commands, group)
+
+            return actual
+
+        return decorator
+
+    @classmethod
+    def autocomplete(cls, command_name: str):
+        """
+        Declares a autocomplete function for a command
+
+        Should return a list of option choices
+
+        Parameters
+        ----------
+        command_name : str
+            Name of the command this autocomplete belongs to
+
+        Example
+        -------
+        @Package.autocomplete("command")
+
+        async def command_autocomplete(self, ctx: Context):
+            return [
+                {
+                    "name": "Blue",
+                    "value": "blue"
+                }
+            ]
+        """
+
+        def decorator(coroutine):
+            actual = coroutine
+
+            if isinstance(actual, staticmethod):
+                actual = actual.__func__
+
+            if not inspect.iscoroutinefunction(actual):
+                raise TypeError("Autocomplete methods must be coroutine")
+
+            actual.__command__ = False
+            actual.__component__ = False
+            actual.__subcommand__ = False
+            actual.__autocomplete__ = True
+            actual.__data__ = (command_name,)
+
+            return actual
+
+        return decorator
+
+    def unpack(self):
+        to_return = []
+
+        for meth in [
+            attr[1]
+            for attr in inspect.getmembers(self, inspect.iscoroutinefunction)
+            if not attr[0].startswith("__") and not attr[0].endswith("__")
+        ]:
+            try:
+                d = meth.__data__
+
+                if meth.__command__:
+                    to_return.append(Command(d[0], meth, d[1], d[2]))
+
+                elif meth.__component__:
+                    to_return.append(Component(d[0], meth, d[1], d[2], d[3]))
+
+                elif meth.__subcommand__:
+                    to_return.append(TopLevelSubCommand(d[0], meth, d[1], d[2]))
+
+                elif meth.__autocomplete__:
+                    to_return.append(Autocomplete(d[0], meth))
+
+            except AttributeError:
+                continue
+
+        return to_return
```

### Comparing `disunity-0.1.7/src/disunity/utils.py` & `disunity-0.1.8/src/disunity/utils.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from enum import Enum, IntEnum
-
-__version__ = "0.1.3"
-
-
-class InteractionTypes(IntEnum):
-    PING = 1
-    APPLICATION_COMMAND = 2
-    MESSAGE_COMPONENT = 3
-    APPLICATION_COMMAND_AUTOCOMPLETE = 4
-    MODAL_SUBMIT = 5
-
-
-class InteractionCallbackTypes(IntEnum):
-    PONG = 1
-    CHANNEL_MESSAGE_WITH_SOURCE = 4
-    DEFERRED_CHANNEL_MESSAGE_WITH_SOURCE = 5
-    DEFERRED_UPDATE_MESSAGE = 6
-    UPDATE_MESSAGE = 7
-    APPLICATION_COMMAND_AUTOCOMPLETE_RESULT = 8
-    MODAL = 9
-    PREMIUM_REQUIRED = 10
-
-
-class DefaultAvatars(Enum):
-    blurple = 0
-    grey = 1
-    gray = 1
-    green = 2
-    orange = 3
-    red = 4
-
-    def __str__(self):
-        return self.name
-
-
-def return_avatar_as_cdn(avatar, uid):
-    if avatar is not None:
-        animated = avatar.startswith("a_")
-        suffix = "gif" if animated else "png"
-        return f"https://cdn.discordapp.com/avatars/{uid}/{avatar}.{suffix}?size=1024"
-    return f"https://cdn.discordapp.com/embed/avatars/{uid%len(DefaultAvatars)}.png"
+from enum import Enum, IntEnum
+
+__version__ = "0.1.3"
+
+
+class InteractionTypes(IntEnum):
+    PING = 1
+    APPLICATION_COMMAND = 2
+    MESSAGE_COMPONENT = 3
+    APPLICATION_COMMAND_AUTOCOMPLETE = 4
+    MODAL_SUBMIT = 5
+
+
+class InteractionCallbackTypes(IntEnum):
+    PONG = 1
+    CHANNEL_MESSAGE_WITH_SOURCE = 4
+    DEFERRED_CHANNEL_MESSAGE_WITH_SOURCE = 5
+    DEFERRED_UPDATE_MESSAGE = 6
+    UPDATE_MESSAGE = 7
+    APPLICATION_COMMAND_AUTOCOMPLETE_RESULT = 8
+    MODAL = 9
+    PREMIUM_REQUIRED = 10
+
+
+class DefaultAvatars(Enum):
+    blurple = 0
+    grey = 1
+    gray = 1
+    green = 2
+    orange = 3
+    red = 4
+
+    def __str__(self):
+        return self.name
+
+
+def return_avatar_as_cdn(avatar, uid):
+    if avatar is not None:
+        animated = avatar.startswith("a_")
+        suffix = "gif" if animated else "png"
+        return f"https://cdn.discordapp.com/avatars/{uid}/{avatar}.{suffix}?size=1024"
+    return f"https://cdn.discordapp.com/embed/avatars/{uid%len(DefaultAvatars)}.png"
```

### Comparing `disunity-0.1.7/src/disunity.egg-info/PKG-INFO` & `disunity-0.1.8/src/disunity.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-Metadata-Version: 2.1
-Name: disunity
-Version: 0.1.7
-Summary: Python framework for Discord interactions using a web server
-Author: Tadeo Murillo, 
-Project-URL: Homepoge, https://github.com/murillotadeo/disunity
-Project-URL: Bug Tracker, https://github.com/murillotadeo/disunity/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# disunity
-
-Python framework for Discord interactions using a web server
-
-# Installation
-`pip install disunity`
-
-# Introduction to Disunity
-```python
-import disunity
-
-server = disunity.DisunityServer()
-
-if __name__ == '__main__':
-    server.run()
-```
-
-Using packages
-```python
-import disunity
-import pathlib
-
-server = disunity.DisunityServer()
-
-@server.before_serving
-def load_packages():
-    for package in [f"{f.parent}.{f.stem}" for f in pathlib.Path("packages").glob("*.py")]:
-        server.load_package(package)
-
-if __name__ == '__main__':
-    server.run()
-
-```
-
-# Setting up a package
-
-```python
-from disunity import package, utils
-
-class FirstPackage(package.Package):
-    def __init__(self, app):
-        self.app = app
-
-    @package.Package.command('ping')
-    async def ping(self, ctx):
-        return await ctx.callback("Pong!")
-
-def setup(app):
-    app.register_package(FirstPackage(app))
-
-```
-
-# Disclaimer
-
-This will require that you already have hosting service for the server to run on as well as a domain to host the server on. If you have neither of these, an alternative would be to host on Heroku using a web application with Gunicorn. 
-
-# Side note
-
-The server will receive interactions to the `/interactions` endpoint of your server. It will look like this: `https://example.com/interactions`. Once you run the server, put the url with the added interactions endpoint into the `interactions` URL on your app located in the Discord developer portal.
-
+Metadata-Version: 2.1
+Name: disunity
+Version: 0.1.8
+Summary: Python framework for Discord interactions using a web server
+Author: Tadeo Murillo, 
+Project-URL: Homepoge, https://github.com/murillotadeo/disunity
+Project-URL: Bug Tracker, https://github.com/murillotadeo/disunity/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# disunity
+
+Python framework for Discord interactions using a web server
+
+# Installation
+`pip install disunity`
+
+# Introduction to Disunity
+```python
+import disunity
+
+server = disunity.DisunityServer()
+
+if __name__ == '__main__':
+    server.run()
+```
+
+Using packages
+```python
+import disunity
+import pathlib
+
+server = disunity.DisunityServer()
+
+@server.before_serving
+def load_packages():
+    for package in [f"{f.parent}.{f.stem}" for f in pathlib.Path("packages").glob("*.py")]:
+        server.load_package(package)
+
+if __name__ == '__main__':
+    server.run()
+
+```
+
+# Setting up a package
+
+```python
+from disunity import package, utils
+
+class FirstPackage(package.Package):
+    def __init__(self, app):
+        self.app = app
+
+    @package.Package.command('ping')
+    async def ping(self, ctx):
+        return await ctx.callback("Pong!")
+
+def setup(app):
+    app.register_package(FirstPackage(app))
+
+```
+
+# Disclaimer
+
+This will require that you already have hosting service for the server to run on as well as a domain to host the server on. If you have neither of these, an alternative would be to host on Heroku using a web application with Gunicorn. 
+
+# Side note
+
+The server will receive interactions to the `/interactions` endpoint of your server. It will look like this: `https://example.com/interactions`. Once you run the server, put the url with the added interactions endpoint into the `interactions` URL on your app located in the Discord developer portal.
+
```

### Comparing `disunity-0.1.7/src/disunity.egg-info/SOURCES.txt` & `disunity-0.1.8/src/disunity.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,13 +10,14 @@
 src/disunity/server.py
 src/disunity/utils.py
 src/disunity.egg-info/PKG-INFO
 src/disunity.egg-info/SOURCES.txt
 src/disunity.egg-info/dependency_links.txt
 src/disunity.egg-info/top_level.txt
 src/disunity/models/__init__.py
+src/disunity/models/attachment.py
 src/disunity/models/components.py
 src/disunity/models/context.py
 src/disunity/models/interaction.py
 src/disunity/models/member.py
 src/disunity/models/message.py
 src/disunity/models/user.py
```

