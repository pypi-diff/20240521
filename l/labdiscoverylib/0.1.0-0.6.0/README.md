# Comparing `tmp/labdiscoverylib-0.1.0.tar.gz` & `tmp/labdiscoverylib-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labdiscoverylib-0.1.0.tar", last modified: Mon Oct  9 08:35:34 2023, max compression
+gzip compressed data, was "labdiscoverylib-0.6.0.tar", last modified: Mon May 20 23:13:36 2024, max compression
```

## Comparing `labdiscoverylib-0.1.0.tar` & `labdiscoverylib-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 nctrun    (1000) nctrun    (1000)        0 2023-10-09 08:35:34.819495 labdiscoverylib-0.1.0/
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)    34520 2023-10-09 07:56:01.000000 labdiscoverylib-0.1.0/LICENSE
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     5407 2023-10-09 08:35:34.819495 labdiscoverylib-0.1.0/PKG-INFO
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     4135 2023-10-09 08:34:42.000000 labdiscoverylib-0.1.0/README.md
-drwxrwxr-x   0 nctrun    (1000) nctrun    (1000)        0 2023-10-09 08:35:34.819495 labdiscoverylib-0.1.0/labdiscoverylib/
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)    50497 2023-10-09 08:29:28.000000 labdiscoverylib-0.1.0/labdiscoverylib/__init__.py
-drwxrwxr-x   0 nctrun    (1000) nctrun    (1000)        0 2023-10-09 08:35:34.819495 labdiscoverylib-0.1.0/labdiscoverylib/backends/
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)      261 2023-10-09 08:29:07.000000 labdiscoverylib-0.1.0/labdiscoverylib/backends/__init__.py
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)    23257 2023-10-09 08:29:12.000000 labdiscoverylib-0.1.0/labdiscoverylib/backends/redis_manager.py
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     5207 2023-10-09 08:29:17.000000 labdiscoverylib-0.1.0/labdiscoverylib/config.py
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     1106 2023-10-09 08:29:22.000000 labdiscoverylib-0.1.0/labdiscoverylib/exc.py
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     4030 2023-10-09 08:29:33.000000 labdiscoverylib-0.1.0/labdiscoverylib/ops.py
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)    17053 2023-10-09 08:29:36.000000 labdiscoverylib-0.1.0/labdiscoverylib/tasks.py
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)    16332 2023-10-09 08:29:40.000000 labdiscoverylib-0.1.0/labdiscoverylib/users.py
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     1151 2023-10-09 08:29:44.000000 labdiscoverylib-0.1.0/labdiscoverylib/utils.py
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     9359 2023-10-09 08:29:47.000000 labdiscoverylib-0.1.0/labdiscoverylib/views.py
-drwxrwxr-x   0 nctrun    (1000) nctrun    (1000)        0 2023-10-09 08:35:34.819495 labdiscoverylib-0.1.0/labdiscoverylib.egg-info/
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     5407 2023-10-09 08:35:34.000000 labdiscoverylib-0.1.0/labdiscoverylib.egg-info/PKG-INFO
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)      547 2023-10-09 08:35:34.000000 labdiscoverylib-0.1.0/labdiscoverylib.egg-info/SOURCES.txt
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)        1 2023-10-09 08:35:34.000000 labdiscoverylib-0.1.0/labdiscoverylib.egg-info/dependency_links.txt
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)        1 2023-10-09 08:14:21.000000 labdiscoverylib-0.1.0/labdiscoverylib.egg-info/not-zip-safe
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)       25 2023-10-09 08:35:34.000000 labdiscoverylib-0.1.0/labdiscoverylib.egg-info/requires.txt
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)       16 2023-10-09 08:35:34.000000 labdiscoverylib-0.1.0/labdiscoverylib.egg-info/top_level.txt
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)       79 2023-10-09 08:35:34.819495 labdiscoverylib-0.1.0/setup.cfg
--rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     1696 2023-10-09 08:01:30.000000 labdiscoverylib-0.1.0/setup.py
+drwxrwxr-x   0 nctrun    (1000) nctrun    (1000)        0 2024-05-20 23:13:36.513005 labdiscoverylib-0.6.0/
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)    34520 2023-10-09 07:56:01.000000 labdiscoverylib-0.6.0/LICENSE
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     5422 2024-05-20 23:13:36.513005 labdiscoverylib-0.6.0/PKG-INFO
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     4150 2023-12-06 19:21:30.000000 labdiscoverylib-0.6.0/README.md
+drwxrwxr-x   0 nctrun    (1000) nctrun    (1000)        0 2024-05-20 23:13:36.513005 labdiscoverylib-0.6.0/labdiscoverylib/
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)    50565 2023-12-07 01:53:32.000000 labdiscoverylib-0.6.0/labdiscoverylib/__init__.py
+drwxrwxr-x   0 nctrun    (1000) nctrun    (1000)        0 2024-05-20 23:13:36.513005 labdiscoverylib-0.6.0/labdiscoverylib/backends/
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)      261 2023-10-09 08:29:07.000000 labdiscoverylib-0.6.0/labdiscoverylib/backends/__init__.py
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)    23924 2023-12-07 00:49:03.000000 labdiscoverylib-0.6.0/labdiscoverylib/backends/redis_manager.py
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     5207 2023-10-09 08:29:17.000000 labdiscoverylib-0.6.0/labdiscoverylib/config.py
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     1106 2023-10-09 08:29:22.000000 labdiscoverylib-0.6.0/labdiscoverylib/exc.py
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     4030 2023-10-09 08:29:33.000000 labdiscoverylib-0.6.0/labdiscoverylib/ops.py
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)    16953 2023-12-07 01:05:35.000000 labdiscoverylib-0.6.0/labdiscoverylib/tasks.py
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)    16610 2023-12-07 00:52:49.000000 labdiscoverylib-0.6.0/labdiscoverylib/users.py
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     1151 2023-12-07 00:45:36.000000 labdiscoverylib-0.6.0/labdiscoverylib/utils.py
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     9738 2023-12-07 02:16:11.000000 labdiscoverylib-0.6.0/labdiscoverylib/views.py
+drwxrwxr-x   0 nctrun    (1000) nctrun    (1000)        0 2024-05-20 23:13:36.513005 labdiscoverylib-0.6.0/labdiscoverylib.egg-info/
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     5422 2024-05-20 23:13:36.000000 labdiscoverylib-0.6.0/labdiscoverylib.egg-info/PKG-INFO
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)      547 2024-05-20 23:13:36.000000 labdiscoverylib-0.6.0/labdiscoverylib.egg-info/SOURCES.txt
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)        1 2024-05-20 23:13:36.000000 labdiscoverylib-0.6.0/labdiscoverylib.egg-info/dependency_links.txt
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)        1 2023-10-09 08:14:21.000000 labdiscoverylib-0.6.0/labdiscoverylib.egg-info/not-zip-safe
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)       38 2024-05-20 23:13:36.000000 labdiscoverylib-0.6.0/labdiscoverylib.egg-info/requires.txt
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)       16 2024-05-20 23:13:36.000000 labdiscoverylib-0.6.0/labdiscoverylib.egg-info/top_level.txt
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)       79 2024-05-20 23:13:36.513005 labdiscoverylib-0.6.0/setup.cfg
+-rw-rw-r--   0 nctrun    (1000) nctrun    (1000)     1712 2023-12-07 01:04:47.000000 labdiscoverylib-0.6.0/setup.py
```

### Comparing `labdiscoverylib-0.1.0/LICENSE` & `labdiscoverylib-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `labdiscoverylib-0.1.0/PKG-INFO` & `labdiscoverylib-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labdiscoverylib
-Version: 0.1.0
+Version: 0.6.0
 Summary: LabDiscoveryEngine library for creating unmanaged laboratories
 Home-page: https://developers.labsland.com/labdiscoverylib/
 Author: LabsLand
 Author-email: dev@labsland.com
 License: GNU AGPL v3
 Project-URL: Documentation, https://developers.labsland.com/labdiscoverylib/en/stable/
 Project-URL: Code, https://github.com/labsland/labdiscoverylib
@@ -26,25 +26,25 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # labdiscoverylib
 
 [![CircleCI](https://circleci.com/gh/labsland/labdiscoverylib.svg?style=svg)](https://circleci.com/gh/labsland/labdiscoverylib)
-[![documentation](https://raw.githubusercontent.com/labsland/labdiscoverylib/0.5.x/docs/source/_static/docs.svg)](https://developers.labsland.com/labdiscoverylib/)
+[![documentation](https://raw.githubusercontent.com/labsland/labdiscoverylib/main/docs/source/_static/docs.svg)](https://developers.labsland.com/labdiscoverylib/)
 [![Version](https://img.shields.io/pypi/v/labdiscoverylib.svg)](https://pypi.python.org/pypi/labdiscoverylib/)
 [![Python versions](https://img.shields.io/pypi/pyversions/labdiscoverylib.svg)](https://pypi.python.org/pypi/labdiscoverylib/)
 
 **labdiscoverylib** is a library for creating [LabDiscoveryEngine](https://github.com/labsland/labdiscoveryengine/) remote laboratories, based on [weblablib](https://developers.labsland.com/weblablib).
 
 A remote laboratory is a software and hardware system that enables students to access real laboratories through the Internet.
 For example, a student can be learning how to program a robot by writing code in a computer at home and sending it to a remote laboratory, where the student can see how the program behaves in a real environment.
 
 Creating a remote laboratory may imply many layers, such as authentication, authorization, scheduling, etc., so Remote Laboratory Management Systems (RLMS) were created to make the common layers of remote laboatories.
-WebLab-Deusto is an Open Source RLMS, and it has multiple ways ([see the docs](https://weblabdeusto.readthedocs.org)) to create a remote laboratory (in different programming languages, etc.).
+WebLab-Deusto is an Open Source RLMS, and it has multiple ways ([see the docs](https://developers.labsland.com/labdiscoveryengine/en/stable/)) to create a remote laboratory (in different programming languages, etc.).
 
 In the case of Python, with the popular [Flask](http://flask.pocoo.org) microframework, **labdiscoverylib** is the wrapper used to create *unmanaged labs*.
 *Unmanaged labs* is a term used in WebLab-Deusto to refer laboratories where the authors develop the full stack (server, client, deployment), as opposed to *managed labs*.
 
 If you are familiar with Flask and with Web development, and want to be able to customize everything but not need to implement all the layers of authentication, administration, etc., this library would be very useful. Furthermore, this library allows you to develop remote laboratories for many environments (from regular computers with Linux to systems such as Raspberry Pi). And it integrates very well with other Flask components such as [Flask-SocketIO](https://flask-socketio.readthedocs.io/), [Flask-SQLAlchemy](http://flask-sqlalchemy.pocoo.org/) for databases or [Flask-Assets](https://flask-assets.readthedocs.io/).
 
 ## Documentation
@@ -63,15 +63,15 @@
 ```python
 from flask import Flask, url_for
 from labdiscoverylib import WebLab, weblab_user, requires_active
 
 app = Flask(__name__)
 app.config.update({
     'SECRET_KEY': 'secret', # MUST CHANGE
-    'WEBLAB_USERNAME': 'weblabdeusto',
+    'WEBLAB_USERNAME': 'lde',
     'WEBLAB_PASSWORD': 'password',
 })
 
 weblab = WebLab(app)
 
 @weblab.on_start
 def on_start(client_data, server_data):
```

### Comparing `labdiscoverylib-0.1.0/README.md` & `labdiscoverylib-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # labdiscoverylib
 
 [![CircleCI](https://circleci.com/gh/labsland/labdiscoverylib.svg?style=svg)](https://circleci.com/gh/labsland/labdiscoverylib)
-[![documentation](https://raw.githubusercontent.com/labsland/labdiscoverylib/0.5.x/docs/source/_static/docs.svg)](https://developers.labsland.com/labdiscoverylib/)
+[![documentation](https://raw.githubusercontent.com/labsland/labdiscoverylib/main/docs/source/_static/docs.svg)](https://developers.labsland.com/labdiscoverylib/)
 [![Version](https://img.shields.io/pypi/v/labdiscoverylib.svg)](https://pypi.python.org/pypi/labdiscoverylib/)
 [![Python versions](https://img.shields.io/pypi/pyversions/labdiscoverylib.svg)](https://pypi.python.org/pypi/labdiscoverylib/)
 
 **labdiscoverylib** is a library for creating [LabDiscoveryEngine](https://github.com/labsland/labdiscoveryengine/) remote laboratories, based on [weblablib](https://developers.labsland.com/weblablib).
 
 A remote laboratory is a software and hardware system that enables students to access real laboratories through the Internet.
 For example, a student can be learning how to program a robot by writing code in a computer at home and sending it to a remote laboratory, where the student can see how the program behaves in a real environment.
 
 Creating a remote laboratory may imply many layers, such as authentication, authorization, scheduling, etc., so Remote Laboratory Management Systems (RLMS) were created to make the common layers of remote laboatories.
-WebLab-Deusto is an Open Source RLMS, and it has multiple ways ([see the docs](https://weblabdeusto.readthedocs.org)) to create a remote laboratory (in different programming languages, etc.).
+WebLab-Deusto is an Open Source RLMS, and it has multiple ways ([see the docs](https://developers.labsland.com/labdiscoveryengine/en/stable/)) to create a remote laboratory (in different programming languages, etc.).
 
 In the case of Python, with the popular [Flask](http://flask.pocoo.org) microframework, **labdiscoverylib** is the wrapper used to create *unmanaged labs*.
 *Unmanaged labs* is a term used in WebLab-Deusto to refer laboratories where the authors develop the full stack (server, client, deployment), as opposed to *managed labs*.
 
 If you are familiar with Flask and with Web development, and want to be able to customize everything but not need to implement all the layers of authentication, administration, etc., this library would be very useful. Furthermore, this library allows you to develop remote laboratories for many environments (from regular computers with Linux to systems such as Raspberry Pi). And it integrates very well with other Flask components such as [Flask-SocketIO](https://flask-socketio.readthedocs.io/), [Flask-SQLAlchemy](http://flask-sqlalchemy.pocoo.org/) for databases or [Flask-Assets](https://flask-assets.readthedocs.io/).
 
 ## Documentation
@@ -34,15 +34,15 @@
 ```python
 from flask import Flask, url_for
 from labdiscoverylib import WebLab, weblab_user, requires_active
 
 app = Flask(__name__)
 app.config.update({
     'SECRET_KEY': 'secret', # MUST CHANGE
-    'WEBLAB_USERNAME': 'weblabdeusto',
+    'WEBLAB_USERNAME': 'lde',
     'WEBLAB_PASSWORD': 'password',
 })
 
 weblab = WebLab(app)
 
 @weblab.on_start
 def on_start(client_data, server_data):
```

### Comparing `labdiscoverylib-0.1.0/labdiscoverylib/__init__.py` & `labdiscoverylib-0.6.0/labdiscoverylib/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """
 labdiscoverylib
 ~~~~~~~~~~~~~~~
 
-This library is a wrapper for developing unmanaged WebLab-Deusto remote laboratories. You may find
-documentation about WebLab-Deusto at:
+This library is a wrapper for developing unmanaged LabDiscoveryEngine remote laboratories. You may find
+documentation about LabDiscoveryEngine at:
 
-   https://weblabdeusto.readthedocs.org/
+   https://developers.labsland.com/labdiscoveryengine/
 
 And the documentation on labdiscoverylib at:
 
    https://developers.labsland.com/labdiscoverylib/
 
 This library heavily relies on Flask, so if you are new to Flask, you might find very useful to
 learn a bit about it first:
 
    http://flask.pocoo.org/
 
-The library is designed to forget about the integration with WebLab-Deusto and make it easy. It
+The library is designed to forget about the integration with LabDiscoveryEngine and make it easy. It
 provides:
 
  * A WebLab object. You must initialize it with the app. It will include a set of new web methods
-   that WebLab-Deusto uses. It also allows you to define what methods should be call on the
+   that LabDiscoveryEngine uses. It also allows you to define what methods should be call on the
    beginning and end of the user session.
 
  * A set of methods to access information about the current information, such as ``weblab_user``,
    (which can be anonymous or not, active or not), ``requires_login`` (for methods which should
    never be used by anonymous users), ``requires_active`` (for methods which should only be
    used by users who are supposed to be using the laboratory now), ``poll`` (to report WebLab
    that the user is still active) or ``logout`` (to report WebLab that the user left).
@@ -48,15 +48,14 @@
 import warnings
 import threading
 import traceback
 import webbrowser
 
 from functools import wraps
 
-import six
 import redis
 import click
 import requests
 
 from flask import jsonify, request, current_app, redirect, \
      url_for, g, session, after_this_request, render_template, \
      has_request_context, has_app_context
@@ -94,41 +93,41 @@
            'socket_requires_login', 'socket_requires_active',
            'current_task', 'current_task_stopping', 'WebLabTask',
            'WebLabError', 'NoContextError', 'InvalidConfigError',
            'WebLabNotInitializedError', 'TimeoutError',
            'AlreadyRunningError', 'CurrentUser', 'AnonymousUser',
            'ExpiredUser']
 
-__version__ = '0.5.7'
+__version__ = '0.6.0'
 __license__ = 'GNU Affero General Public License v3 http://www.gnu.org/licenses/agpl.html'
 
 
 #############################################################
 #
-# WebLab-Deusto Flask extension:
+# LabDiscoveryEngine Flask extension:
 #
 #
 #
 
 class WebLab(object):
     """
     WebLab is a Flask extension that manages the settings (backend, session, etc.), and
     the registration of certain methods (e.g., on_start, etc.)
 
     Initializes the object. All the parameters are optional.
 
     :param app: the Flask application
 
     :param base_url: the base URL to be used. By default, the WebLab URLs will be
-                     ``/weblab/sessions/<something>``.  If you provide ``base_url = '/foo'``, then
-                     it will be listening in ``/foo/weblab/sessions/<something>``. This is the
+                     ``/ldl/sessions/<something>``.  If you provide ``base_url = '/foo'``, then
+                     it will be listening in ``/foo/ldl/sessions/<something>``. This is the
                      route that will be used in the Flask application (so if your application
                      is deployed in ``/bar``, then it will be
-                     ``/bar/foo/weblab/sessions/<something>``. This URLs do NOT need to be
-                     publicly available (they can be only available to WebLab-Deusto if you
+                     ``/bar/foo/ldl/sessions/<something>``. This URLs do NOT need to be
+                     publicly available (they can be only available to LabDiscoveryEngine if you
                      want, by playing with the firewall or so). You can also configure it with
                      ``WEBLAB_BASE_URL`` in the Flask configuration.
 
     :param callback_url: a URL that WebLab will implement that must be public. For example,
                          ``/mylab/callback/``, this URL must be available to the final user.
                          The user will be redirected there with a token and this code will
                          redirect him to the initial_url. You can also configure it with
@@ -240,19 +239,19 @@
         #
         # Initialize and register the "weblab" blueprint
         #
         if not self._base_url:
             self._base_url = self._app.config.get(ConfigurationKeys.WEBLAB_BASE_URL)
 
         if self._base_url:
-            url = '{}/weblab'.format(self._base_url)
+            url = '{}/ldl'.format(self._base_url)
             if self._base_url.endswith('/'):
                 print("Note: your base_url ({}) ends in '/'. This way, the url will be {} (with //). Are you sure that's what you want?".format(self._base_url, url), file=sys.stderr)
         else:
-            url = '/weblab'
+            url = '/ldl'
 
         self._app.register_blueprint(weblab_blueprint, url_prefix=url)
 
         #
         # Add a callback URL
         #
         if not self._callback_url:
@@ -410,15 +409,15 @@
                 weblab_user.data.store_if_modified()
 
             return response
 
         click.disable_unicode_literals_warning = True
         @app.cli.group('weblab')
         def weblab_cli():
-            """WebLab-Deusto related operations: initialize new sessions for development, run tasks, etc."""
+            """LabDiscoveryEngine related operations: initialize new sessions for development, run tasks, etc."""
             pass
 
         @weblab_cli.command('clean-expired-users')
         def clean_expired_users():
             """
             Clean expired users.
 
@@ -443,31 +442,35 @@
         def loop(threads, reload): # pylint: disable=redefined-builtin
             """
             Run planned tasks and clean expired users, permanently.
             """
             if reload is None:
                 reload = current_app.debug
 
+            if reload:
+                print("reload temporaily not supported")
+                reload = False
+
             def run_loop():
                 if reload:
                     print("Running with reloader. Don't use this in production mode.")
                 self.loop(int(threads), reload)
 
             if reload:
-                from werkzeug.serving import run_with_reloader
-                run_with_reloader(run_loop)
+                # run_with_reloader(run_loop)
+                run_loop()
             else:
                 run_loop()
 
         @weblab_cli.group()
         def fake():
             """Fake user management.
 
-            With this interface, you can test your laboratory without WebLab-Deusto. It implements the same
-            methods used by WebLab-Deusto (create new user, check status, kick out user), from a command
+            With this interface, you can test your laboratory without LabDiscoveryEngine. It implements the same
+            methods used by LabDiscoveryEngine (create new user, check status, kick out user), from a command
             line interface. The "new" command has several parameters for changing language, user name, etc.
             """
             pass
 
         def _weblab_api_request(url_name, json_data, session_id=None):
             if session_id:
                 url = url_for(url_name, session_id=session_id, _external=True)
@@ -488,48 +491,53 @@
         @click.option('--experiment-name', default='mylab', help="Experiment name")
         @click.option('--category-name', default='Lab Experiments', help="Category name (of the experiment)")
         @click.option('--dont-open-browser', is_flag=True, help="Do not open the fake user in a web browser")
         @click.option('--client-initial-data', default='{}', help="Client initial data")
         @click.option('--client-initial-data-file', default=None, help="Client initial data (JSON file)")
         def fake_user(name, username, username_unique, assigned_time, back, locale, experiment_name, category_name, dont_open_browser, client_initial_data, client_initial_data_file):
             """
-            Create a fake WebLab-Deusto user session.
+            Create a fake LabDiscoveryEngine user session.
 
             This command creates a new user session and stores the session in disk, so you
             can use other commands to check its status or delete it.
             """
             assigned_time = float(assigned_time)
-
-            start_time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S") + '.0'
-            start_time_timestamp = time.time()
+            start_time = datetime.datetime.now(datetime.timezone.utc)
             
             try:
                 client_initial_data_data = json.loads(client_initial_data)
             except Exception as json_err:
                 print("Error reading {}: {}".format(client_initial_data, json_err))
                 client_initial_data_data = {}
 
             if client_initial_data_file:
                 try:
                     client_initial_data_data = json.load(open(client_initial_data_file))
                 except Exception as err:
                     print("Error reading {}: {}".format(client_initial_data_file, err))
 
             request_data = {
-                'client_initial_data': client_initial_data_data,
-                'server_initial_data': {
-                    'priority.queue.slot.start': start_time,
-                    'priority.queue.slot.start.timestamp': start_time_timestamp,
-                    'priority.queue.slot.length': assigned_time,
-                    'request.username': username,
-                    'request.full_name': name,
-                    'request.username.unique': username_unique,
-                    'request.locale': locale,
-                    'request.experiment_id.experiment_name': experiment_name,
-                    'request.experiment_id.category_name': category_name,
+                'request': {
+                    'locale': locale,
+                    'user': client_initial_data_data,
+                    'server': {},
+                    'backUrl': back
+                },
+                'laboratory': {
+                    'name': experiment_name,
+                    'category': category_name,
+                },
+                'user': {
+                    'username': username,
+                    'fullName': name,
+                    'unique': username_unique,
+                },
+                'schedule': {
+                    'start': start_time.isoformat(),
+                    'length': assigned_time,
                 },
                 'back': back,
             }
 
             initial_time = time.time()
             result = _weblab_api_request('weblab._start_session', request_data)
             final_time = time.time()
@@ -538,15 +546,15 @@
                 print()
                 print("Congratulations! The session is started [in {:.2f} seconds]".format(final_time - initial_time))
                 print()
                 print("Open: {}".format(result['url']))
                 print()
                 print("Session identifier: {}\n".format(result['session_id']))
                 open(".fake_weblab_user_session_id", 'w').write(result['session_id'])
-                print("Now you can make calls as if you were WebLab-Deusto (no argument needed):")
+                print("Now you can make calls as if you were LabDiscoveryEngine (no argument needed):")
                 print(" - flask weblab fake status")
                 print(" - flask weblab fake dispose")
                 print()
                 if not dont_open_browser:
                     webbrowser.open(result['url'])
             else:
                 print()
@@ -555,15 +563,15 @@
 
         @fake.command('status')
         def fake_status():
             """
             Check status of a fake user.
 
             Once you create a user with flask "weblab fake new", you can use this command to
-            simulate the status method of WebLab-Deusto and see what it would return.
+            simulate the status method of LabDiscoveryEngine and see what it would return.
             """
             if not os.path.exists('.fake_weblab_user_session_id'):
                 print("Session not found. Did you call 'flask weblab fake new' first?")
                 return
             session_id = open('.fake_weblab_user_session_id').read()
             current_status_time = status_time(session_id)
             print(self._backend.get_user(session_id))
@@ -571,15 +579,15 @@
 
         @fake.command('dispose')
         def fake_dispose():
             """
             End a session of a fake user.
 
             Once you create a user with 'flask weblab fake new', you can use this command to
-            simulate the dispose method of WebLab-Deusto to kill the current session.
+            simulate the dispose method of LabDiscoveryEngine to kill the current session.
             """
             if not os.path.exists('.fake_weblab_user_session_id'):
                 print("Session not found. Did you call 'flask weblab fake new' first?")
                 return
             session_id = open('.fake_weblab_user_session_id').read()
             print(self._backend.get_user(session_id))
 
@@ -617,15 +625,15 @@
             if self._app.config.get('WEBLAB_AUTOCLEAN_THREAD', True):
                 self._cleaner_thread = _CleanerThread.create(self, self._app)
                 if self._cleaner_thread is not None:
                     self._cleaner_thread.start()
 
             threads_per_process = self._app.config.get('WEBLAB_TASK_THREADS_PROCESS', 3)
             if threads_per_process > 0: # If set to 0, no thread is running
-                for number in six.moves.range(threads_per_process):
+                for number in range(threads_per_process):
                     task_thread = _TaskRunner(number, self, self._app)
                     self._task_threads.append(task_thread)
                     task_thread.start()
 
         for task_wrapper in self._task_functions.values():
             # XXX This is cleaning locks when restarted. Is this a good thing?
             # A current user in production might be in problem if done this way.
@@ -687,16 +695,16 @@
             def start(client_data, server_data):
                 initialize_my_resources() # Example code
 
         :param func: The function that will be used on start.
 
         This function has two parameters:
 
-        :param client_data: Data provided by the WebLab-Deusto client. It is a dictionary with different parameters.
-        :param server_data: Data provided by the WebLab-Deusto server (username, etc., generally wrapped in the ``weblab_user`` method)
+        :param client_data: Data provided by the LabDiscoveryEngine client. It is a dictionary with different parameters.
+        :param server_data: Data provided by the LabDiscoveryEngine server (username, etc., generally wrapped in the ``weblab_user`` method)
         """
         if self._on_start is not None:
             raise ValueError("on_start has already been defined")
 
         self._on_start = func
         return func
 
@@ -712,15 +720,15 @@
             raise ValueError("on_dispose has already been defined")
 
         self._on_dispose = func
         return func
 
     def clean_expired_users(self):
         """
-        Typically, users are deleted by WebLab-Deusto calling the dispose method.
+        Typically, users are deleted by LabDiscoveryEngine calling the dispose method.
         However, in some conditions (e.g., restarting WebLab), the dispose method
         might not be called, and the laboratory can end in a wrong state. So as to
         avoid this, labdiscoverylib provides three systems:
 
          1. A command flask clean_expired_users.
          2. A thread that by default is running which calls this method every few seconds.
          3. This API method, available as ``weblab.clean_expired_users()``
@@ -1214,19 +1222,19 @@
             socketio_disconnect()
         return func(*args, **kwargs)
 
     return wrapper
 
 def logout():
     """
-    Notify WebLab-Deusto that the user left the laboratory, so next user can enter.
+    Notify LabDiscoveryEngine that the user left the laboratory, so next user can enter.
 
-    This process is not real time. What it happens is that WebLab-Deusto periodically is requesting
+    This process is not real time. What it happens is that LabDiscoveryEngine periodically is requesting
     whether the user is still alive or not. If you call logout, labdiscoverylib will reply the next time
-    that the user left. So it may take some seconds for WebLab-Deusto to realize of that. You can
+    that the user left. So it may take some seconds for LabDiscoveryEngine to realize of that. You can
     regulate this time with ``WEBLAB_POLL_INTERVAL`` setting (defaults to 5).
     """
     session_id = _current_session_id()
     if session_id:
         _current_backend().force_exit(session_id)
```

### Comparing `labdiscoverylib-0.1.0/labdiscoverylib/backends/redis_manager.py` & `labdiscoverylib-0.6.0/labdiscoverylib/backends/redis_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # Copyright 2023 onwards LabsLand Experimentia S.L.U.
 # This software is licensed under the GNU AGPL v3:
 # GNU Affero General Public License version 3 (see the file LICENSE)
 # Read in the documentation about the license
 
 import json
 import time
+import datetime
 
 import redis
 from flask import current_app
 
 from labdiscoverylib.config import ConfigurationKeys
-from labdiscoverylib.utils import create_token, _current_timestamp
+from labdiscoverylib.utils import create_token
 from labdiscoverylib.users import AnonymousUser, CurrentUser, ExpiredUser
 
 
-class RedisManager(object):
+class RedisManager:
     """
     To manage users, sessions and tasks.
 
     USER-RELATED STRUCTURES:
     - <prefix>:weblab:sessions:<session_id> : These keys contain the session ids, storing their creation time. They are
     set to expire when created, so they might need to be refreshed. These keys are used to check if a session has been
     deleted, or to request that a session be deleted.
@@ -35,39 +36,39 @@
     def __init__(self, redis_url, key_base, task_expires, weblab):
         self.client = redis.StrictRedis.from_url(redis_url, decode_responses=True)
         self.weblab = weblab
         self.key_base = key_base  # Redis base prefix to use. It is *not* user or session specific.
 
         self.task_expires = task_expires
 
-    def add_user(self, session_id, user, expiration):
+    def add_user(self, session_id: str, user, expiration):
         """
         Adds a new user.
         This will:
           - Store all user fields into a <prefix>:weblab:active:<sessionid> hashset.
           - Schedule this hashset to expire in a while.
           - Store the sessionid with the current time in the key <prefix>:weblab:sessions:<sessionid>
           - Schedule this last key to expire in a while.
         """
         key = '{}:weblab:active:{}'.format(self.key_base, session_id)
 
         pipeline = self.client.pipeline()
-        pipeline.hset(key, 'max_date', user.max_date)
-        pipeline.hset(key, 'last_poll', user.last_poll)
+        pipeline.hset(key, 'max_date', None if not user.max_date else user.max_date.isoformat())
+        pipeline.hset(key, 'last_poll', None if not user.last_poll else user.last_poll.isoformat())
         pipeline.hset(key, 'username', user.username)
         pipeline.hset(key, 'username-unique', user.username_unique)
         pipeline.hset(key, 'data', json.dumps(user.data))
         pipeline.hset(key, 'back', user.back)
         pipeline.hset(key, 'exited', json.dumps(user.exited))
         pipeline.hset(key, 'locale', json.dumps(user.locale))
         pipeline.hset(key, 'full_name', json.dumps(user.full_name))
         pipeline.hset(key, 'experiment_name', json.dumps(user.experiment_name))
         pipeline.hset(key, 'category_name', json.dumps(user.category_name))
         pipeline.hset(key, 'experiment_id', json.dumps(user.experiment_id))
-        pipeline.hset(key, 'start_date', user.start_date)
+        pipeline.hset(key, 'start_date', None if not user.start_date else user.start_date.isoformat())
         pipeline.hset(key, 'request_client_data', json.dumps(user.request_client_data))
         pipeline.hset(key, 'request_server_data', json.dumps(user.request_server_data))
         pipeline.expire(key, expiration)
         pipeline.set('{}:weblab:sessions:{}'.format(self.key_base, session_id), time.time())
         pipeline.expire('{}:weblab:sessions:{}'.format(self.key_base, session_id), expiration + 300)
         pipeline.execute()
 
@@ -105,24 +106,24 @@
 
         (back, last_poll, max_date, username,
          username_unique, data, exited, locale, full_name,
          experiment_name, category_name, experiment_id,
          request_client_data, request_server_data, start_date) = pipeline.execute()
 
         if max_date is not None:
-            return CurrentUser(session_id=session_id, back=back, last_poll=float(last_poll),
-                               max_date=float(max_date), username=username,
+            return CurrentUser(session_id=session_id, back=back, last_poll=datetime.datetime.fromisoformat(last_poll),
+                               max_date=datetime.datetime.fromisoformat(max_date), username=username,
                                username_unique=username_unique,
                                data=json.loads(data), exited=json.loads(exited),
                                locale=json.loads(locale), full_name=json.loads(full_name),
                                experiment_name=json.loads(experiment_name),
                                category_name=json.loads(category_name),
                                request_client_data=json.loads(request_client_data),
                                request_server_data=json.loads(request_server_data),
-                               start_date=float(start_date),
+                               start_date=datetime.datetime.fromisoformat(start_date),
                                experiment_id=json.loads(experiment_id))
 
         return self.get_expired_user(session_id)
 
     def get_expired_user(self, session_id):
         pipeline = self.client.pipeline()
         key = '{}:weblab:inactive:{}'.format(self.key_base, session_id)
@@ -132,25 +133,28 @@
             pipeline.hget(key, name)
 
         (back, max_date, username, username_unique, data, locale,
          full_name, experiment_name, category_name, experiment_id, exited, last_poll,
          request_client_data, request_server_data, start_date, disposing_resources) = pipeline.execute()
 
         if max_date is not None:
-            return ExpiredUser(session_id=session_id, last_poll=last_poll, back=back, max_date=float(max_date), exited=exited,
+            return ExpiredUser(session_id=session_id, 
+                               last_poll=datetime.datetime.fromisoformat(last_poll) if last_poll else None, 
+                               back=back, 
+                               max_date=datetime.datetime.fromisoformat(max_date), exited=exited,
                                username=username, username_unique=username_unique,
                                data=json.loads(data),
                                locale=json.loads(locale),
                                full_name=json.loads(full_name),
                                experiment_name=json.loads(experiment_name),
                                category_name=json.loads(category_name),
                                experiment_id=json.loads(experiment_id),
                                request_client_data=json.loads(request_client_data),
                                request_server_data=json.loads(request_server_data),
-                               start_date=float(start_date),
+                               start_date=datetime.datetime.fromisoformat(start_date),
                                disposing_resources=json.loads(disposing_resources))
 
         return AnonymousUser()
 
     def _tests_delete_user(self, session_id):
         "Only for testing"
         self.client.delete('{}:weblab:active:{}'.format(self.key_base, session_id))
@@ -166,26 +170,26 @@
         #
         pipeline = self.client.pipeline()
         pipeline.delete("{}:weblab:active:{}".format(self.key_base, session_id))
 
         key = '{}:weblab:inactive:{}'.format(self.key_base, session_id)
 
         pipeline.hset(key, "back", expired_user.back)
-        pipeline.hset(key, "max_date", expired_user.max_date)
+        pipeline.hset(key, "max_date", None if not expired_user.max_date else expired_user.max_date.isoformat())
         pipeline.hset(key, "username", expired_user.username)
         pipeline.hset(key, "username-unique", expired_user.username_unique)
         pipeline.hset(key, "data", json.dumps(expired_user.data))
         pipeline.hset(key, "locale", json.dumps(expired_user.locale))
         pipeline.hset(key, "full_name", json.dumps(expired_user.full_name))
         pipeline.hset(key, "experiment_name", json.dumps(expired_user.experiment_name))
         pipeline.hset(key, "category_name", json.dumps(expired_user.category_name))
         pipeline.hset(key, "experiment_id", json.dumps(expired_user.experiment_id))
         pipeline.hset(key, "request_client_data", json.dumps(expired_user.request_client_data))
         pipeline.hset(key, "request_server_data", json.dumps(expired_user.request_server_data))
-        pipeline.hset(key, "start_date", expired_user.start_date)
+        pipeline.hset(key, "start_date", None if not expired_user.start_date else expired_user.start_date.isoformat())
         pipeline.hset(key, "disposing_resources", json.dumps(True))
 
         # During half an hour after being created, the user is redirected to
         # the original URL. After that, every record of the user has been deleted
         pipeline.expire("{}:weblab:inactive:{}".format(self.key_base, session_id), current_app.config.get(ConfigurationKeys.WEBLAB_EXPIRED_USERS_TIMEOUT, 3600))
         results = pipeline.execute()
 
@@ -223,17 +227,17 @@
             pipeline.hget(session_id_key, 'exited')
 
             max_date, last_poll, exited = pipeline.execute()
 
             if max_date is not None and last_poll is not None: 
                 # Double check: he might be deleted in the meanwhile
                 # We don't use 'active', since active takes into account 'exited'
-
-                time_left = float(max_date) - _current_timestamp()
-                time_without_polling = _current_timestamp() - float(last_poll)
+                now = datetime.datetime.now(datetime.timezone.utc)
+                time_left = (datetime.datetime.fromisoformat(max_date) - now).total_seconds()
+                time_without_polling = (now - datetime.datetime.fromisoformat(last_poll)).total_seconds()
                 user_exited = exited in ('true', '1', 'True', 'TRUE')
 
                 if time_left <= 0:
                     expired_sessions.append(session_id)
 
                 elif time_without_polling >= self.weblab.timeout:
                     expired_sessions.append(session_id)
@@ -246,18 +250,18 @@
     def session_exists(self, session_id):
         user = self.get_user(session_id)
         return not user.is_anonymous
 
     def poll(self, session_id):
         key = '{}:weblab:active:{}'.format(self.key_base, session_id)
 
-        last_poll = _current_timestamp()
+        last_poll = datetime.datetime.now(datetime.timezone.utc)
         pipeline = self.client.pipeline()
         pipeline.hget(key, "max_date")
-        pipeline.hset(key, "last_poll", last_poll)
+        pipeline.hset(key, "last_poll", last_poll.isoformat())
         max_date, _ = pipeline.execute()
 
         if max_date is None:
             # If the user was deleted in between, revert the last_poll
             self.client.delete(key)
 
     #
```

### Comparing `labdiscoverylib-0.1.0/labdiscoverylib/config.py` & `labdiscoverylib-0.6.0/labdiscoverylib/config.py`

 * *Files identical despite different names*

### Comparing `labdiscoverylib-0.1.0/labdiscoverylib/exc.py` & `labdiscoverylib-0.6.0/labdiscoverylib/exc.py`

 * *Files identical despite different names*

### Comparing `labdiscoverylib-0.1.0/labdiscoverylib/ops.py` & `labdiscoverylib-0.6.0/labdiscoverylib/ops.py`

 * *Files identical despite different names*

### Comparing `labdiscoverylib-0.1.0/labdiscoverylib/tasks.py` & `labdiscoverylib-0.6.0/labdiscoverylib/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # Read in the documentation about the license
 
 import sys
 import time
 import threading
 import traceback
 
-import six
 import redis
 
 from werkzeug.local import LocalProxy
 from werkzeug.datastructures import ImmutableDict
 
 from flask import g
 
@@ -392,16 +391,14 @@
            }
         """
         return self._task_data['error']
 
     def __repr__(self):
         """Represent a WebLab task"""
         representation = '<WebLab Task {}>'.format(self._task_id)
-        if six.PY2:
-            representation = representation.encode('utf8')
         return representation
 
     def __lt__(self, other):
         """Compare, for Python 3"""
         if isinstance(other, WebLabTask):
             return self._task_id < other._task_id
 
@@ -453,15 +450,15 @@
                 # and Redis died before, or a Redis upgrade or so.
                 traceback.print_exc()
                 time.sleep(5)
             except Exception:
                 traceback.print_exc()
                 continue
 
-            for _ in six.moves.range(_TaskRunner._STEPS_WAITING):
+            for _ in range(_TaskRunner._STEPS_WAITING):
                 time.sleep(0.05)
                 if self._stopping:
                     break
 
 
 def _current_task():
     task_id = getattr(g, '_weblab_task_id', None)
```

### Comparing `labdiscoverylib-0.1.0/labdiscoverylib/users.py` & `labdiscoverylib-0.6.0/labdiscoverylib/users.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 # This software is licensed under the GNU AGPL v3:
 # GNU Affero General Public License version 3 (see the file LICENSE)
 # Read in the documentation about the license
 
 import abc
 import json
 import zlib
+import datetime
 import warnings
 
-import six
+from typing import Optional
 
 from werkzeug.datastructures import ImmutableDict
 from werkzeug.local import LocalProxy
 from flask import g, current_app
 
 from labdiscoverylib.utils import create_token, _current_backend, _current_timestamp, \
      _current_weblab, _current_session_id
@@ -67,62 +68,61 @@
      * :class:`CurrentUser`
      * :class:`ExpiredUser`
 
     """
     __metaclass__ = abc.ABCMeta
 
     @abc.abstractproperty
-    def active(self):
+    def active(self) -> bool:
         """Is the user active right now or not?"""
 
     @abc.abstractproperty
-    def is_anonymous(self):
+    def is_anonymous(self) -> bool:
         """Was the user a valid user recently?"""
 
     @abc.abstractmethod
-    def __str__(self):
+    def __str__(self) -> str:
         """str representation"""
 
 class AnonymousDataImmutableDict(dict):
     def _method(self, *args, **kwargs): # pylint: disable=unused-argument, no-self-use
         raise TypeError("Anonymous user contains no valid data")
 
     __setitem__ = __getitem__ = __delitem__ = __iter__ = __len__ = _method
 
     keys = values = get = setdefault = items = iteritems = _method
 
     pop = popitem = copy = update = clear = _method
 
-@six.python_2_unicode_compatible
 class AnonymousUser(WebLabUser):
     """
     Implementation of :class:`WebLabUser` representing anonymous users.
     """
 
     @property
-    def active(self):
+    def active(self) -> bool:
         """Is active? Always ``False``"""
         return False
 
     @property
-    def is_anonymous(self):
+    def is_anonymous(self) -> bool:
         """Is anonymous? Always ``True``"""
         return True
 
     @property
-    def locale(self):
-        """Language requested by WebLab-Deusto? Always ``None``"""
+    def locale(self) -> Optional[str]:
+        """Language requested by LabDiscoveryEngine? Always ``None``"""
         return None
 
     @property
-    def data(self):
+    def data(self) -> dict:
         """An object that raises error if accessed as a dict"""
         return AnonymousDataImmutableDict()
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "Anonymous user"
 
 _OBJECT = object()
 
 class _CurrentOrExpiredUser(WebLabUser): # pylint: disable=abstract-method
     def __init__(self, session_id, back, last_poll, max_date, username, username_unique,
                  exited, data, locale, full_name, experiment_name, category_name, experiment_id,
@@ -141,103 +141,103 @@
         self._experiment_name = experiment_name
         self._category_name = category_name
         self._experiment_id = experiment_id
         self._request_client_data = request_client_data
         self._request_server_data = request_server_data
 
     @property
-    def experiment_name(self):
-        """Experiment name (as in WebLab-Deusto)"""
+    def experiment_name(self) -> str:
+        """Experiment name (as in LabDiscoveryEngine)"""
         return self._experiment_name
 
     @property
-    def category_name(self):
-        """Experiment category name (as in WebLab-Deusto)"""
+    def category_name(self) -> Optional[str]:
+        """Experiment category name (as in LabDiscoveryEngine)"""
         return self._category_name
 
     @property
-    def experiment_id(self):
-        """Experiment id (as in WebLab-Deusto)"""
+    def experiment_id(self) -> str:
+        """Experiment id (as in LabDiscoveryEngine)"""
         return self._experiment_id
 
     @property
-    def full_name(self):
+    def full_name(self) -> Optional[str]:
         """User full name"""
         return self._full_name
 
     @property
-    def locale(self):
+    def locale(self) -> Optional[str]:
         """Language requested by the system (e.g., was the user using Moodle in Spanish?). 'es'"""
         return self._locale
 
     @property
-    def back(self):
+    def back(self) -> str:
         """URL of the previous website. When the user has finished, redirect him there"""
         return self._back
 
     @property
-    def last_poll(self):
+    def last_poll(self) -> datetime.datetime:
         """Last time the user called poll() (can be done by an automated process)"""
         return self._last_poll
 
     @property
-    def session_id(self):
+    def session_id(self) -> str:
         """Session identifying the current user"""
         return self._session_id
 
     @property
-    def max_date(self):
+    def max_date(self) -> datetime.datetime:
         """When should the user finish"""
         return self._max_date
 
     @property
-    def username(self):
+    def username(self) -> str:
         """
         Username of the user. Note: this is short, but not unique across institutions.
         There could be a ``john`` in ``institutionA`` and another ``john`` in ``institutionB``
         """
         return self._username
 
     @property
-    def username_unique(self):
+    def username_unique(self) -> str:
         """
         Unique username across institutions. It's ``john@institutionA`` (which is
         different to ``john@institutionB``)
         """
         return self._username_unique
 
     @property
-    def exited(self):
+    def exited(self) -> bool:
         """
         Did the user call :func:`logout`?
         """
         return self._exited
 
     @property
-    def request_client_data(self):
+    def request_client_data(self) -> ImmutableDict:
         """
         Information provided in the beginning of the interaction (on_start): client_data
         """
         return ImmutableDict(self._request_client_data or {})
 
     @property
-    def request_server_data(self):
+    def request_server_data(self) -> ImmutableDict:
         """
         Information provided in the beginning of the interaction (on_start): server_data
         """
         return ImmutableDict(self._request_server_data or {})
 
     @property
-    def start_date(self):
+    def start_date(self) -> datetime.datetime:
         """
         Information provided in the beginning of the interaction (on_start): client_data
         """
         return self._start_date
 
-    def add_action(self, session_id, action):
+    def add_action(self, session_id: str, action):
         """
         Adds a new raw action to a session_id, returning the action_id
         """
         action_id = create_token()
         self.store_action(session_id, action_id, action)
         return action_id
 
@@ -251,28 +251,29 @@
     def clean_actions(self, session_id): # pylint: disable=no-self-use
         """
         Remove all actions of a session_id
         """
         backend = _current_backend()
         backend.clean_actions(session_id)
 
+def utcnow():
+    return datetime.datetime.now(datetime.timezone.utc)
+
 class DataHolder(dict):
     def __init__(self, user, data, previous_hash=None):
         super(DataHolder, self).__init__(data)
         self._user = user
         self._initial_hash = previous_hash or self._get_hash(data)
 
     @property
-    def initial_hash(self):
+    def initial_hash(self) -> str:
         return self._initial_hash
 
     def _get_hash(self, data):
         data_str = json.dumps(data)
-        if six.PY2:
-            data_str = data_str.decode('utf8')
         return zlib.crc32(data_str.encode('utf8'))
 
     def store(self):
         backend = _current_backend()
         data = self.copy()
         backend.update_data(self._user._session_id, data)
         self._initial_hash = self._get_hash(data)
@@ -291,15 +292,14 @@
         user = backend.get_user(self._user._session_id)
         if isinstance(user.data, DataHolder):
             self.update(user.data)
             for key in list(self):
                 if key not in user.data:
                     self.pop(key, None)
 
-@six.python_2_unicode_compatible
 class CurrentUser(_CurrentOrExpiredUser):
     """
     This class is a :class:`WebLabUser` representing a user which is still actively using a
     laboratory. If the session expires, it will become a :class:`ExpiredUser`.
     """
 
     def __init__(self, *args, **kwargs):
@@ -312,15 +312,15 @@
         User data. By default an empty dictionary.
         You can access to it and modify it across processes.
         See also :meth:`CurrentUser.update_data`.
         """
         return self._data
 
     @data.setter
-    def data(self, data):
+    def data(self, data: dict):
         self._data = DataHolder(self, data, previous_hash=self._data.initial_hash)
 
     def update_data(self, new_data=_OBJECT):
         """
         .. deprecated:: 0.5.0
 
         Use weblab_user.data.store() or don't use anything if inside a view or on_start.
@@ -332,26 +332,26 @@
 
         if new_data != _OBJECT:
             new_data = self._data
 
         self.data = self._data
 
     @property
-    def time_without_polling(self):
+    def time_without_polling(self) -> float:
         """
         Seconds without polling
         """
-        return _current_timestamp() - self.last_poll
+        return (utcnow() - self.last_poll).total_seconds()
 
     @property
     def time_left(self):
         """
         Seconds left (0 if time passed)
         """
-        return max(0, self.max_date - _current_timestamp())
+        return max(0, (self.max_date - utcnow()).total_seconds())
 
     def to_expired_user(self):
         """
         Create a ExpiredUser based on the data of the user
         """
         return ExpiredUser(session_id=self._session_id, back=self._back, max_date=self._max_date,
                            last_poll=self._last_poll, exited=self._exited,
@@ -431,17 +431,16 @@
 
     @property
     def is_anonymous(self):
         """Is the user anonymous? ``False``"""
         return False
 
     def __str__(self):
-        return 'Current user (id: {!r}): {!r} ({!r}), last poll: {:.2f} seconds ago. Max date in {:.2f} seconds. Redirecting to {!r}'.format(self._session_id, self._username, self._username_unique, self.time_without_polling, self._max_date - _current_timestamp(), self._back)
+        return 'Current user (id: {!r}): {!r} ({!r}), last poll: {:.2f} seconds ago. Max date in {:.2f} seconds. Redirecting to {!r}'.format(self._session_id, self._username, self._username_unique, self.time_without_polling, (self._max_date - utcnow()).total_seconds(), self._back)
 
-@six.python_2_unicode_compatible
 class ExpiredUser(_CurrentOrExpiredUser):
     """
     This class is a :class:`WebLabUser` representing a user which has been kicked out already.
     Typically this ExpiredUser is kept in the backend for around an hour (it depends on
     ``WEBLAB_EXPIRED_USERS_TIMEOUT`` setting).
 
     Most of the fields are same as in :class:`CurrentUser`.
@@ -487,8 +486,8 @@
     def is_anonymous(self):
         """
         Is it an anonymous user? (``False``)
         """
         return False
 
     def __str__(self):
-        return 'Expired user (id: {!r}): {!r} ({!r}), max date in {:.2f} seconds. Redirecting to {!r}'.format(self._session_id, self._username, self._username_unique, self._max_date - _current_timestamp(), self._back)
+        return 'Expired user (id: {!r}): {!r} ({!r}), max date in {:.2f} seconds. Redirecting to {!r}'.format(self._session_id, self._username, self._username_unique, (self._max_date - utcnow()).total_seconds(), self._back)
```

### Comparing `labdiscoverylib-0.1.0/labdiscoverylib/utils.py` & `labdiscoverylib-0.6.0/labdiscoverylib/utils.py`

 * *Files identical despite different names*

### Comparing `labdiscoverylib-0.1.0/labdiscoverylib/views.py` & `labdiscoverylib-0.6.0/labdiscoverylib/views.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import datetime
 import traceback
 
 from flask import Blueprint, Response, current_app, jsonify, request, url_for
 
 from labdiscoverylib.exc import NotFoundError
 from labdiscoverylib.config import ConfigurationKeys
-from labdiscoverylib.utils import create_token, _to_timestamp, _current_backend, _current_weblab, _current_timestamp
+from labdiscoverylib.utils import create_token, _to_timestamp, _current_backend, _current_weblab
 from labdiscoverylib.users import CurrentUser, _set_weblab_user_cache
 from labdiscoverylib.ops import status_time, update_weblab_user_data, dispose_user
 
 weblab_blueprint = Blueprint("weblab", __name__) # pylint: disable=invalid-name
 
 @weblab_blueprint.before_request
 def _require_http_credentials():
@@ -79,57 +79,88 @@
     """
     Create a new session: WebLab-Deusto is telling us that a new user is coming. We register the user in the backend system.
     """
     request_data = request.get_json(force=True)
     return jsonify(**_process_start_request(request_data))
 
 def _process_start_request(request_data):
-    """ Auxiliar method, called also from the Flask CLI to fake_user """
-    client_initial_data = request_data['client_initial_data']
-    server_initial_data = request_data['server_initial_data']
+    """ 
+    Auxiliar method, called also from the Flask CLI to fake_user.
 
-    # Parse the initial date + assigned time to know the maximum time
-    start_date_timestamp = server_initial_data.get('priority.queue.slot.start.timestamp')
-    if start_date_timestamp: # if the time is available in timestamp, use it
-        start_date = datetime.datetime.fromtimestamp(float(start_date_timestamp))
-    else:
-        # Otherwise, to keep backwards compatibility, assume that it's in the same timezone
-        # as we are
-        start_date_str = server_initial_data['priority.queue.slot.start']
-        start_date_str, microseconds = start_date_str.split('.')
-        difference = datetime.timedelta(microseconds=int(microseconds))
-        start_date = datetime.datetime.strptime(start_date_str, "%Y-%m-%d %H:%M:%S") + difference
+    The expected request_data looks like this:
+
+    {
+        'request': {
+            'locale': 'en',
+            'ldeReservationId': 'Zyv24cnaOqWXnZVO2v3hdQdrIxBC66BM9VM1EUFCBqM',
+            'user': {
+                # User data
+            },
+            'server': {
+                # Server data
+            },
+            'backUrl': "http://...", # wherever we have to redirect the user after
+        },
+        'laboratory': {
+            'name': "My lab",
+            'category': "My category", # Optional
+        },
+        'user': {
+            'username': "john", # Not guaranteed to be unique
+            'unique': "john@labsland",
+            'fullName': "John Smith", # Optional
+        },
+        'schedule': {
+            'start': "2023-12-06T23:13:58.076302+00:00",
+            'length': 298, # seconds left after that start
+        }
+    }
+
+    """
+    client_initial_data = request_data['request'].get('user')
+    server_initial_data = request_data['request'].get('server')
 
-    slot_length = float(server_initial_data['priority.queue.slot.length'])
+    # Parse the initial date + assigned time to know the maximum time
+    start_date = datetime.datetime.fromisoformat(request_data['schedule']['start'])
+    slot_length = float(request_data['schedule']['length'])
     max_date = start_date + datetime.timedelta(seconds=slot_length)
-    locale = server_initial_data.get('request.locale')
-    full_name = server_initial_data['request.full_name']
+    locale = request_data['request'].get('locale', 'en')
+    full_name = request_data['user'].get('fullName')
+    username = request_data['user']['username']
+    username_unique = request_data['user']['unique']
+
+    experiment_name = request_data['laboratory']['name']
+    category_name = request_data['laboratory'].get('category')
+    if category_name:
+        experiment_id = '{}@{}'.format(experiment_name, category_name)
+    else:
+        experiment_id = experiment_name
 
-    experiment_name = server_initial_data['request.experiment_id.experiment_name']
-    category_name = server_initial_data['request.experiment_id.category_name']
-    experiment_id = '{}@{}'.format(experiment_name, category_name)
+    back_url = request_data['request']['backUrl']
 
     # Create a global session
     session_id = create_token()
 
+
     # Prepare adding this to backend
-    user = CurrentUser(session_id=session_id, back=request_data['back'],
-                       last_poll=_current_timestamp(), max_date=float(_to_timestamp(max_date)),
-                       username=server_initial_data['request.username'],
-                       username_unique=server_initial_data['request.username.unique'],
+    user = CurrentUser(session_id=session_id, back=back_url,
+                       last_poll=datetime.datetime.now(datetime.timezone.utc),
+                       max_date=max_date,
+                       username=username,
+                       username_unique=username_unique,
                        exited=False, data={}, locale=locale,
                        full_name=full_name, experiment_name=experiment_name,
                        experiment_id=experiment_id, category_name=category_name,
                        request_client_data=client_initial_data,
                        request_server_data=server_initial_data,
-                       start_date=float(_to_timestamp(start_date)))
+                       start_date=start_date)
 
     backend = _current_backend()
 
-    backend.add_user(session_id, user, expiration=30 + int(float(server_initial_data['priority.queue.slot.length'])))
+    backend.add_user(session_id, user, expiration=30 + int(float(slot_length)))
 
 
     kwargs = {}
     scheme = current_app.config.get(ConfigurationKeys.WEBLAB_SCHEME)
     if scheme:
         kwargs['_scheme'] = scheme
 
@@ -201,27 +232,28 @@
         if future_timeout is not None and time.time() > future_timeout:
             # Do not process more requests, timeout happened
             break
 
     return jsonify(status=status)
 
 
-@weblab_blueprint.route('/sessions/<session_id>', methods=['POST'])
+@weblab_blueprint.route('/sessions/<session_id>', methods=['POST', 'DELETE'])
 def _dispose_experiment(session_id):
     """
     This method is called to kick one user out. This may happen
     when an administrator defines so, or when the assigned time
     is over.
     """
-    request_data = request.get_json(force=True)
-    if 'action' not in request_data:
-        return jsonify(message="Unknown op")
+    if request.method == 'POST':
+        request_data = request.get_json(force=True)
+        if 'action' not in request_data:
+            return jsonify(message="Unknown op")
 
-    if request_data['action'] != 'delete':
-        return jsonify(message="Unknown op")
+        if request_data['action'] != 'delete':
+            return jsonify(message="Unknown op")
 
     try:
         dispose_user(session_id, waiting=True)
     except NotFoundError:
         return jsonify(message="Not found")
 
     return jsonify(message="Deleted")
```

### Comparing `labdiscoverylib-0.1.0/labdiscoverylib.egg-info/PKG-INFO` & `labdiscoverylib-0.6.0/labdiscoverylib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labdiscoverylib
-Version: 0.1.0
+Version: 0.6.0
 Summary: LabDiscoveryEngine library for creating unmanaged laboratories
 Home-page: https://developers.labsland.com/labdiscoverylib/
 Author: LabsLand
 Author-email: dev@labsland.com
 License: GNU AGPL v3
 Project-URL: Documentation, https://developers.labsland.com/labdiscoverylib/en/stable/
 Project-URL: Code, https://github.com/labsland/labdiscoverylib
@@ -26,25 +26,25 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # labdiscoverylib
 
 [![CircleCI](https://circleci.com/gh/labsland/labdiscoverylib.svg?style=svg)](https://circleci.com/gh/labsland/labdiscoverylib)
-[![documentation](https://raw.githubusercontent.com/labsland/labdiscoverylib/0.5.x/docs/source/_static/docs.svg)](https://developers.labsland.com/labdiscoverylib/)
+[![documentation](https://raw.githubusercontent.com/labsland/labdiscoverylib/main/docs/source/_static/docs.svg)](https://developers.labsland.com/labdiscoverylib/)
 [![Version](https://img.shields.io/pypi/v/labdiscoverylib.svg)](https://pypi.python.org/pypi/labdiscoverylib/)
 [![Python versions](https://img.shields.io/pypi/pyversions/labdiscoverylib.svg)](https://pypi.python.org/pypi/labdiscoverylib/)
 
 **labdiscoverylib** is a library for creating [LabDiscoveryEngine](https://github.com/labsland/labdiscoveryengine/) remote laboratories, based on [weblablib](https://developers.labsland.com/weblablib).
 
 A remote laboratory is a software and hardware system that enables students to access real laboratories through the Internet.
 For example, a student can be learning how to program a robot by writing code in a computer at home and sending it to a remote laboratory, where the student can see how the program behaves in a real environment.
 
 Creating a remote laboratory may imply many layers, such as authentication, authorization, scheduling, etc., so Remote Laboratory Management Systems (RLMS) were created to make the common layers of remote laboatories.
-WebLab-Deusto is an Open Source RLMS, and it has multiple ways ([see the docs](https://weblabdeusto.readthedocs.org)) to create a remote laboratory (in different programming languages, etc.).
+WebLab-Deusto is an Open Source RLMS, and it has multiple ways ([see the docs](https://developers.labsland.com/labdiscoveryengine/en/stable/)) to create a remote laboratory (in different programming languages, etc.).
 
 In the case of Python, with the popular [Flask](http://flask.pocoo.org) microframework, **labdiscoverylib** is the wrapper used to create *unmanaged labs*.
 *Unmanaged labs* is a term used in WebLab-Deusto to refer laboratories where the authors develop the full stack (server, client, deployment), as opposed to *managed labs*.
 
 If you are familiar with Flask and with Web development, and want to be able to customize everything but not need to implement all the layers of authentication, administration, etc., this library would be very useful. Furthermore, this library allows you to develop remote laboratories for many environments (from regular computers with Linux to systems such as Raspberry Pi). And it integrates very well with other Flask components such as [Flask-SocketIO](https://flask-socketio.readthedocs.io/), [Flask-SQLAlchemy](http://flask-sqlalchemy.pocoo.org/) for databases or [Flask-Assets](https://flask-assets.readthedocs.io/).
 
 ## Documentation
@@ -63,15 +63,15 @@
 ```python
 from flask import Flask, url_for
 from labdiscoverylib import WebLab, weblab_user, requires_active
 
 app = Flask(__name__)
 app.config.update({
     'SECRET_KEY': 'secret', # MUST CHANGE
-    'WEBLAB_USERNAME': 'weblabdeusto',
+    'WEBLAB_USERNAME': 'lde',
     'WEBLAB_PASSWORD': 'password',
 })
 
 weblab = WebLab(app)
 
 @weblab.on_start
 def on_start(client_data, server_data):
```

### Comparing `labdiscoverylib-0.1.0/labdiscoverylib.egg-info/SOURCES.txt` & `labdiscoverylib-0.6.0/labdiscoverylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labdiscoverylib-0.1.0/setup.py` & `labdiscoverylib-0.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 cp_license="GNU AGPL v3"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='labdiscoverylib',
-      version='0.1.0',
+      version='0.6.0',
       description="LabDiscoveryEngine library for creating unmanaged laboratories",
       long_description=long_description,
       long_description_content_type="text/markdown",
       project_urls=OrderedDict((
             ('Documentation', 'https://developers.labsland.com/labdiscoverylib/en/stable/'),
             ('Code', 'https://github.com/labsland/labdiscoverylib'),
             ('Issue tracker', 'https://github.com/labsland/labdiscoverylib/issues'),
@@ -37,9 +37,9 @@
       classifiers=classifiers,
       zip_safe=False,
       author='LabsLand',
       author_email='dev@labsland.com',
       url='https://developers.labsland.com/labdiscoverylib/',
       license=cp_license,
       packages=['labdiscoverylib', 'labdiscoverylib.backends'],
-      install_requires=['redis', 'flask', 'six', 'requests'],
+      install_requires=['redis', 'flask<3', 'werkzeug<3', 'six', 'requests'],
      )
```

