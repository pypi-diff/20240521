# Comparing `tmp/asfquart-0.1.3.tar.gz` & `tmp/asfquart-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asfquart-0.1.3.tar", last modified: Sun Mar  3 14:34:06 2024, max compression
+gzip compressed data, was "asfquart-0.1.4.tar", last modified: Tue May 21 16:45:26 2024, max compression
```

## Comparing `asfquart-0.1.3.tar` & `asfquart-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-03-03 14:34:06.983815 asfquart-0.1.3/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    11357 2023-11-01 17:18:26.000000 asfquart-0.1.3/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)    14540 2024-03-03 14:34:06.983815 asfquart-0.1.3/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      960 2024-01-29 16:01:37.000000 asfquart-0.1.3/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      664 2024-03-03 14:33:39.000000 asfquart-0.1.3/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      274 2024-03-03 14:34:06.983815 asfquart-0.1.3/setup.cfg
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-03-03 14:34:06.979815 asfquart-0.1.3/src/
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-03-03 14:34:06.983815 asfquart-0.1.3/src/asfquart/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      251 2024-02-19 10:45:29.000000 asfquart-0.1.3/src/asfquart/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6636 2024-02-20 15:04:27.000000 asfquart-0.1.3/src/asfquart/auth.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3449 2024-02-20 15:01:25.000000 asfquart-0.1.3/src/asfquart/base.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1869 2023-11-04 15:54:54.000000 asfquart-0.1.3/src/asfquart/config.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5516 2024-02-19 10:46:03.000000 asfquart-0.1.3/src/asfquart/generics.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3010 2024-02-14 12:51:29.000000 asfquart-0.1.3/src/asfquart/ldap.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4682 2024-02-19 09:59:02.000000 asfquart-0.1.3/src/asfquart/session.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2002 2024-02-21 15:41:31.000000 asfquart-0.1.3/src/asfquart/utils.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-03-03 14:34:06.983815 asfquart-0.1.3/src/asfquart.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    14540 2024-03-03 14:34:06.000000 asfquart-0.1.3/src/asfquart.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      403 2024-03-03 14:34:06.000000 asfquart-0.1.3/src/asfquart.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-03-03 14:34:06.000000 asfquart-0.1.3/src/asfquart.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      141 2024-03-03 14:34:06.000000 asfquart-0.1.3/src/asfquart.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        9 2024-03-03 14:34:06.000000 asfquart-0.1.3/src/asfquart.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-21 16:45:26.186886 asfquart-0.1.4/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    11357 2023-11-01 17:18:26.000000 asfquart-0.1.4/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    14558 2024-05-21 16:45:26.186886 asfquart-0.1.4/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      932 2024-04-26 18:08:31.000000 asfquart-0.1.4/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      695 2024-05-02 15:33:26.000000 asfquart-0.1.4/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      274 2024-05-21 16:45:26.186886 asfquart-0.1.4/setup.cfg
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-21 16:45:26.184886 asfquart-0.1.4/src/
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-21 16:45:26.185886 asfquart-0.1.4/src/asfquart/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      251 2024-02-19 10:45:29.000000 asfquart-0.1.4/src/asfquart/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6636 2024-02-20 15:04:27.000000 asfquart-0.1.4/src/asfquart/auth.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    12184 2024-05-21 16:44:36.000000 asfquart-0.1.4/src/asfquart/base.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1043 2024-05-21 16:44:36.000000 asfquart-0.1.4/src/asfquart/config.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5619 2024-05-01 20:57:17.000000 asfquart-0.1.4/src/asfquart/generics.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3075 2024-05-21 16:44:36.000000 asfquart-0.1.4/src/asfquart/ldap.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4854 2024-05-01 20:57:17.000000 asfquart-0.1.4/src/asfquart/session.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4063 2024-05-21 16:44:36.000000 asfquart-0.1.4/src/asfquart/utils.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-21 16:45:26.186886 asfquart-0.1.4/src/asfquart.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    14558 2024-05-21 16:45:26.000000 asfquart-0.1.4/src/asfquart.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      403 2024-05-21 16:45:26.000000 asfquart-0.1.4/src/asfquart.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-05-21 16:45:26.000000 asfquart-0.1.4/src/asfquart.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      158 2024-05-21 16:45:26.000000 asfquart-0.1.4/src/asfquart.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        9 2024-05-21 16:45:26.000000 asfquart-0.1.4/src/asfquart.egg-info/top_level.txt
```

### Comparing `asfquart-0.1.3/LICENSE` & `asfquart-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asfquart-0.1.3/PKG-INFO` & `asfquart-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asfquart
-Version: 0.1.3
+Version: 0.1.4
 Summary: ASF Quart Framework
 Author-email: ASF Infrastructure <users@infra.apache.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -212,35 +212,36 @@
 Requires-Dist: aiohttp>=3.9.2
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: pytest==7.2.0
 Requires-Dist: pytest-cov>=4.0.0
 Requires-Dist: pytest-asyncio>=0.20.3
 Requires-Dist: pytest-mock>=3.10.0
 Requires-Dist: quart>=0.19.4
+Requires-Dist: ezt
+Requires-Dist: asyncinotify
 Provides-Extra: ldap
 Requires-Dist: asfpy[aioldap]; extra == "ldap"
 
   # asfquart - a Quart framework for the ASF
   ![Unit Tests](https://github.com/apache/infrastructure-asfquart/actions/workflows/unit-tests.yml/badge.svg)
   
   This repository will house the future [Quart](https://github.com/pallets/quart/) framework for use 
   within ASF web applications. Nothing much to see here yet...
 
+  For more detailed documentation, see the [documentation page](docs/readme.md).
   
 ## Primer
 
 ~~~python
 import asfquart
 import asfquart.auth
-import asfquart.generics
 
 def my_app():
+    # Construct the quart service. By default, the oauth gateway is enabled at /oauth.
     asfquart.construct("my_app_service")
-    asfquart.generics.setup_oauth()   # Sets up /auth for OAuth handling
-    asfquart.generics.enforce_login() # If not logged in, redirect to the above default login flow
 
     @asfquart.APP.route("/")
     async def homepage():
         return "Hello!"
 
     @asfquart.APP.route("/secret")
     @asfquart.auth.require(asfquart.auth.Requirements.committer)
```

### Comparing `asfquart-0.1.3/README.md` & `asfquart-0.1.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,24 @@
   # asfquart - a Quart framework for the ASF
   ![Unit Tests](https://github.com/apache/infrastructure-asfquart/actions/workflows/unit-tests.yml/badge.svg)
   
   This repository will house the future [Quart](https://github.com/pallets/quart/) framework for use 
   within ASF web applications. Nothing much to see here yet...
 
+  For more detailed documentation, see the [documentation page](docs/readme.md).
   
 ## Primer
 
 ~~~python
 import asfquart
 import asfquart.auth
-import asfquart.generics
 
 def my_app():
+    # Construct the quart service. By default, the oauth gateway is enabled at /oauth.
     asfquart.construct("my_app_service")
-    asfquart.generics.setup_oauth()   # Sets up /auth for OAuth handling
-    asfquart.generics.enforce_login() # If not logged in, redirect to the above default login flow
 
     @asfquart.APP.route("/")
     async def homepage():
         return "Hello!"
 
     @asfquart.APP.route("/secret")
     @asfquart.auth.require(asfquart.auth.Requirements.committer)
@@ -28,8 +27,8 @@
     
     asfquart.APP.run(port=8000)
 
 
 if __name__ == "__main__":
     my_app()
 
-~~~
+~~~
```

### Comparing `asfquart-0.1.3/pyproject.toml` & `asfquart-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asfquart"
-version = "0.1.3"
+version = "0.1.4"
 authors = [ 
   {name = "ASF Infrastructure", email = "users@infra.apache.org"}
 ]
 dependencies = [
     "aiohttp>=3.9.2",
     "PyYAML>=6.0.1",
     "pytest==7.2.0",
     "pytest-cov>=4.0.0",
     "pytest-asyncio>=0.20.3",
     "pytest-mock>=3.10.0",
     "quart>=0.19.4",
+    "ezt",
+    "asyncinotify",
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3"
 ]
```

### Comparing `asfquart-0.1.3/src/asfquart/auth.py` & `asfquart-0.1.4/src/asfquart/auth.py`

 * *Files identical despite different names*

### Comparing `asfquart-0.1.3/src/asfquart/config.py` & `asfquart-0.1.4/src/asfquart/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #!/usr/bin/env python3
+
 """ASFQuart - Configuration readers"""
-import signal
-import asyncio
+
 import yaml
 import functools
 import inspect
-import os
-
-from . import base
 
 DEFAULT_CONFIG_FILENAME = "config.yaml"
 
 
 async def _read_config(callback, config_filename):
     """Reads a YAML configuration and passes it to the callback"""
-    config_as_dict = yaml.safe_load(open(config_filename))
+    with open(config_filename, encoding='utf-8') as r:
+        config_as_dict = yaml.safe_load(r)
     # Some configuration routines may require os to block while the configuration is applied, so
     # we will accept both sync and async callbacks.
     # If the callback is async, await it...
     if inspect.iscoroutinefunction(callback):
         await callback(config_as_dict)
     # Otherwise, just run it in blocking mode
     else:
@@ -29,27 +27,7 @@
     """Standard wrapper for a configuration parser. Reads config.yaml and passes it to the callback as a dict"""
 
     @functools.wraps(func)
     async def config_wrapper(config_filename=DEFAULT_CONFIG_FILENAME):
         await _read_config(func, config_filename)
 
     return config_wrapper
-
-
-def dynamic(func):
-    """Reloadable configuration parser. On startup, or when SIGUSR2 is intercepted, the configuration is reloaded and
-    passed to the configuration callback function."""
-    # If running test suite, the event loop needs to be reset
-    if "PYTEST_CURRENT_TEST" in os.environ and base.loop.is_closed():
-        base.loop = asyncio.get_event_loop()
-
-    @functools.wraps(func)
-    async def config_wrapper_dynamic(config_filename=DEFAULT_CONFIG_FILENAME):
-        def new_task():
-            return asyncio.create_task(_read_config(func, config_filename))
-
-        # Add a signal handler for SIGUSR2
-        base.loop.add_signal_handler(signal.SIGUSR2, new_task)
-        # Read the config on first run
-        await _read_config(func, config_filename)
-
-    return config_wrapper_dynamic
```

### Comparing `asfquart-0.1.3/src/asfquart/generics.py` & `asfquart-0.1.4/src/asfquart/generics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 #!/usr/bin/env python3
 """Generic endpoints for ASFQuart"""
 
-import quart
 import secrets
 import urllib
-import aiohttp
 import time
 
+import quart
+import aiohttp
+
+import asfquart  # implies .session
+
 
 # These are the ASF OAuth URLs for init and verification. Used for setup_oauth()
 OAUTH_URL_INIT = "https://oauth.apache.org/auth-oidc?state=%s&redirect_uri=%s"
 OAUTH_URL_CALLBACK = "https://oauth.apache.org/token-oidc?code=%s"
+DEFAULT_OAUTH_URI = "/auth"
 
-
-def setup_oauth(uri="/auth", workflow_timeout: int = 900):
-    """ "Sets up a generic ASF OAuth endpoint. The default URI is /auth, and the
+def setup_oauth(app, uri=DEFAULT_OAUTH_URI, workflow_timeout: int = 900):
+    """Sets up a generic ASF OAuth endpoint for the given app. The default URI is /auth, and the
     default workflow timeout is 900 seconds (15 min), within which the OAuth login must
     be completed. The OAuth endpoint handles everything related to logging in and out via OAuth,
     and has the following actions:
 
     - /auth?login  - Initializes an OAuth login
     - /auth?login=/foo - Same as above, but redirects to /foo on successful login
     - /auth?logout - Clears a user session, logging them out
     - /auth  - Shows the user's credentials if logged in, 404 otherwise.
 
     This generic route expects the Host: header of the request to be accurate, which means setting
     "ProxyPreserveHost On" in your httpd config if proxying.
     """
 
     pending_states = {}  # keeps track of pending states and their expiry
-    import asfquart  # We import at this point to grab the APP pointer
 
-    @asfquart.APP.route(uri)
+    @app.route(uri)
     async def oauth_endpoint():
         # Init oauth login
         login_uri = quart.request.args.get("login")
         logout_uri = quart.request.args.get("logout")
         if login_uri or quart.request.query_string == b"login":
             state = secrets.token_hex(16)
             # Save the time we initialized this state and the optional login redirect URI
@@ -90,22 +92,25 @@
                     return client_session
                 return quart.Response(
                     status=404,
                     response=f"No active session found.\n",
                 )
 
 
-def enforce_login(redirect_uri="/auth"):
+def enforce_login(app, redirect_uri=DEFAULT_OAUTH_URI):
     """Enforces redirect to the auth provider (if enabled) when a client tries to access a restricted page
     without being logged in. Only redirects if there is no active user session. On success, the client
     is redirected back to the origin page that was restricted. If it is still restricted, the client
     will instead see an error message."""
-    import asfquart
     import asfquart.auth
-    import asfquart.session
-    @asfquart.APP.errorhandler(asfquart.auth.AuthenticationFailed)
+
+    @app.errorhandler(asfquart.auth.AuthenticationFailed)
     async def auth_redirect(error):
-        # If we have no client session, redirect to auth flow
-        if not quart.request.authorization and not await asfquart.session.read():
+        # If we have no client session (and X-No-Redirect is not set), redirect to auth flow
+        if (
+            "x-no-redirect" not in quart.request.headers
+            and not quart.request.authorization
+            and not await asfquart.session.read()
+        ):
             return quart.redirect(f"{redirect_uri}?login={quart.request.full_path}")
         # If we have a session, but still no access, just say so in plain text.
         return quart.Response(status=error.errorcode, response=error.message)
```

### Comparing `asfquart-0.1.3/src/asfquart/ldap.py` & `asfquart-0.1.4/src/asfquart/ldap.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 try:
     import asfpy.aioldap
     import bonsai.errors
     LDAP_SUPPORTED = True
 except ModuleNotFoundError:
     LDAP_SUPPORTED = False
 
-LDAP_CACHE = {}  # Temporary one-hour cache to speed up lookups.
+LDAP_CACHE: dict[str, list] = {}  # Temporary one-hour cache to speed up lookups.
 
 
 class LDAPClient:
     def __init__(self, username: str, password: str):
         self.userid = username
         self.dn = DEFAULT_LDAP_BASE % username
         self.client = asfpy.aioldap.LDAPClient(DEFAULT_LDAP_URI, self.dn, password)
@@ -42,26 +42,26 @@
                 async with self.client.connect():
                     pass
             else:
                 ldap_groups = {attr: [] for attr in attrs}
                 async with self.client.connect() as conn:
                     rv = await conn.search(all_projects, attrs)
                     if not rv:
-                        raise Exception("Empty result set returned by LDAP")
+                        raise Exception("Empty result set returned by LDAP")  # pylint: disable=broad-exception-raised
                     for project in rv:
                         if "dn" in project and any(xattr in project for xattr in attrs):
                             dn_match = GROUP_RE.match(str(project["dn"]))
                             if dn_match:
                                 project_name = dn_match.group(1)
                                 for xattr in attrs:
                                     if self.dn in project.get(xattr, []):
                                         ldap_groups[xattr].append(project_name)
                     LDAP_CACHE[self.userid] = (time.time(), ldap_groups)
             return LDAP_CACHE[self.userid][1]
 
         except bonsai.errors.AuthenticationError as e:
-            raise base.ASFQuartException("Invalid credentials provided", errorcode=403)
+            raise base.ASFQuartException(f"Invalid credentials provided: {e}", errorcode=403)
         except Exception as e:
             print(f"Base exception during LDAP lookup: {e}")
             raise base.ASFQuartException(
                 "Could not perform LDAP authorization check, please try again later.", errorcode=500
             )
```

### Comparing `asfquart-0.1.3/src/asfquart/session.py` & `asfquart-0.1.4/src/asfquart/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python3
 """ASFQuart - User session methods and decorators"""
 import typing
 
 from . import base, ldap
-import quart.sessions
 import time
 import binascii
 
+import quart.sessions
+import asfquart
+
 
 class ClientSession(dict):
     def __init__(self, raw_data: dict):
         """Initializes a client session from a raw dict. ClientSession is a subclassed dict, so that
         we can send it to quart in a format it can render."""
         super().__init__()
         self.uid = raw_data.get("uid")
@@ -23,20 +25,24 @@
         self.committees = raw_data.get("pmcs", [])
         self.projects = raw_data.get("projects", [])
         self.mfa = raw_data.get("mfa", False)
         # Update the external dict representation with internal values
         self.update(self.__dict__.items())
 
 
-async def read(expiry_time=86400*7) -> typing.Optional[ClientSession]:
+async def read(expiry_time=86400*7, app=None) -> typing.Optional[ClientSession]:
     """Fetches a cookie-based session if found (and valid), and updates the last access timestamp
     for the session."""
-    # We store the session cookie using the base.APP.app_id identifier, to distinguish between
+
+    if app is None:
+        app = asfquart.APP
+
+    # We store the session cookie using the app.app_id identifier, to distinguish between
     # two asfquart apps running on the same hostname.
-    cookie_id = base.APP.app_id
+    cookie_id = app.app_id
     if cookie_id in quart.session:
         now = time.time()
         cookie_expiry_deadline = now - expiry_time
         session_dict = quart.session[cookie_id]
         if isinstance(session_dict, dict):
             session_update_timestamp = session_dict.get("uts", 0)
             # If a session cookie has expired (not updated/used for seven days), we delete it instead of returning it
@@ -72,18 +78,26 @@
                             # binascii/ValueError == bad base64 auth string
                             # KeyError = missing username or password
                             raise base.ASFQuartException("Invalid Authorization header provided", errorcode=400)
                 case default:
                     raise base.ASFQuartException("Not implemented yet", errorcode=501)
 
 
-def write(session_data: dict):
+def write(session_data: dict, app=None):
     """Sets a cookie-based user session for this app"""
-    cookie_id = base.APP.app_id
+
+    if app is None:
+        app = asfquart.APP
+
+    cookie_id = app.app_id
     dict_copy = session_data.copy()  # Copy dict so we don't mess with the original data
     dict_copy["uts"] = time.time()   # Set last access timestamp for expiry checks later
     quart.session[cookie_id] = dict_copy
 
 
-def clear():
+def clear(app=None):
     """Clears a session"""
-    quart.session.pop(base.APP.app_id, None)  # Safely pop the session if it's there.
+
+    if app is None:
+        app = asfquart.APP
+
+    quart.session.pop(app.app_id, None)  # Safely pop the session if it's there.
```

### Comparing `asfquart-0.1.3/src/asfquart.egg-info/PKG-INFO` & `asfquart-0.1.4/src/asfquart.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asfquart
-Version: 0.1.3
+Version: 0.1.4
 Summary: ASF Quart Framework
 Author-email: ASF Infrastructure <users@infra.apache.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -212,35 +212,36 @@
 Requires-Dist: aiohttp>=3.9.2
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: pytest==7.2.0
 Requires-Dist: pytest-cov>=4.0.0
 Requires-Dist: pytest-asyncio>=0.20.3
 Requires-Dist: pytest-mock>=3.10.0
 Requires-Dist: quart>=0.19.4
+Requires-Dist: ezt
+Requires-Dist: asyncinotify
 Provides-Extra: ldap
 Requires-Dist: asfpy[aioldap]; extra == "ldap"
 
   # asfquart - a Quart framework for the ASF
   ![Unit Tests](https://github.com/apache/infrastructure-asfquart/actions/workflows/unit-tests.yml/badge.svg)
   
   This repository will house the future [Quart](https://github.com/pallets/quart/) framework for use 
   within ASF web applications. Nothing much to see here yet...
 
+  For more detailed documentation, see the [documentation page](docs/readme.md).
   
 ## Primer
 
 ~~~python
 import asfquart
 import asfquart.auth
-import asfquart.generics
 
 def my_app():
+    # Construct the quart service. By default, the oauth gateway is enabled at /oauth.
     asfquart.construct("my_app_service")
-    asfquart.generics.setup_oauth()   # Sets up /auth for OAuth handling
-    asfquart.generics.enforce_login() # If not logged in, redirect to the above default login flow
 
     @asfquart.APP.route("/")
     async def homepage():
         return "Hello!"
 
     @asfquart.APP.route("/secret")
     @asfquart.auth.require(asfquart.auth.Requirements.committer)
```

