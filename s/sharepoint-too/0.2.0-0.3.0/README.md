# Comparing `tmp/sharepoint-too-0.2.0.tar.gz` & `tmp/sharepoint_too-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharepoint-too-0.2.0.tar", last modified: Thu Sep 23 15:37:47 2021, max compression
+gzip compressed data, was "sharepoint_too-0.3.0.tar", last modified: Tue May 21 17:24:54 2024, max compression
```

## Comparing `sharepoint-too-0.2.0.tar` & `sharepoint_too-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2021-09-23 15:37:47.762258 sharepoint-too-0.2.0/
--rw-r--r--   0 tsantor    (501) staff       (20)      599 2021-09-23 15:31:58.000000 sharepoint-too-0.2.0/HISTORY.md
--rw-r--r--   0 tsantor    (501) staff       (20)     1079 2021-09-01 14:39:58.000000 sharepoint-too-0.2.0/LICENSE
--rw-r--r--   0 tsantor    (501) staff       (20)      135 2021-09-01 14:40:49.000000 sharepoint-too-0.2.0/MANIFEST.in
--rw-r--r--   0 tsantor    (501) staff       (20)     5506 2021-09-23 15:37:47.762385 sharepoint-too-0.2.0/PKG-INFO
--rw-r--r--   0 tsantor    (501) staff       (20)     3176 2020-04-28 23:36:03.000000 sharepoint-too-0.2.0/README.md
--rw-r--r--   0 tsantor    (501) staff       (20)      189 2021-09-23 15:37:47.762777 sharepoint-too-0.2.0/setup.cfg
--rwxr-xr-x   0 tsantor    (501) staff       (20)     1925 2021-09-23 15:35:50.000000 sharepoint-too-0.2.0/setup.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2021-09-23 15:37:47.760818 sharepoint-too-0.2.0/sharepoint_too/
--rwxr-xr-x   0 tsantor    (501) staff       (20)       70 2021-09-23 15:32:13.000000 sharepoint-too-0.2.0/sharepoint_too/__init__.py
--rw-r--r--   0 tsantor    (501) staff       (20)    11543 2021-09-23 15:30:27.000000 sharepoint-too-0.2.0/sharepoint_too/session.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2021-09-23 15:37:47.762016 sharepoint-too-0.2.0/sharepoint_too.egg-info/
--rw-r--r--   0 tsantor    (501) staff       (20)     5506 2021-09-23 15:37:47.000000 sharepoint-too-0.2.0/sharepoint_too.egg-info/PKG-INFO
--rw-r--r--   0 tsantor    (501) staff       (20)      338 2021-09-23 15:37:47.000000 sharepoint-too-0.2.0/sharepoint_too.egg-info/SOURCES.txt
--rw-r--r--   0 tsantor    (501) staff       (20)        1 2021-09-23 15:37:47.000000 sharepoint-too-0.2.0/sharepoint_too.egg-info/dependency_links.txt
--rw-r--r--   0 tsantor    (501) staff       (20)        1 2021-09-23 15:37:36.000000 sharepoint-too-0.2.0/sharepoint_too.egg-info/not-zip-safe
--rw-r--r--   0 tsantor    (501) staff       (20)       38 2021-09-23 15:37:47.000000 sharepoint-too-0.2.0/sharepoint_too.egg-info/requires.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       15 2021-09-23 15:37:47.000000 sharepoint-too-0.2.0/sharepoint_too.egg-info/top_level.txt
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-21 17:24:54.261039 sharepoint_too-0.3.0/
+-rw-r--r--   0 tsantor    (501) staff       (20)      200 2024-05-10 21:13:48.000000 sharepoint_too-0.3.0/AUTHORS.md
+-rw-r--r--   0 tsantor    (501) staff       (20)      703 2024-05-10 21:13:48.000000 sharepoint_too-0.3.0/HISTORY.md
+-rw-r--r--   0 tsantor    (501) staff       (20)     1085 2024-05-10 19:48:08.000000 sharepoint_too-0.3.0/LICENSE
+-rw-r--r--   0 tsantor    (501) staff       (20)       72 2024-05-10 20:02:53.000000 sharepoint_too-0.3.0/MANIFEST.in
+-rw-r--r--   0 tsantor    (501) staff       (20)     4796 2024-05-21 17:24:54.260823 sharepoint_too-0.3.0/PKG-INFO
+-rw-r--r--   0 tsantor    (501) staff       (20)     2864 2024-05-10 21:13:48.000000 sharepoint_too-0.3.0/README.md
+-rw-r--r--   0 tsantor    (501) staff       (20)     4817 2024-05-10 19:54:07.000000 sharepoint_too-0.3.0/pyproject.toml
+-rw-r--r--   0 tsantor    (501) staff       (20)       38 2024-05-21 17:24:54.261083 sharepoint_too-0.3.0/setup.cfg
+-rw-r--r--   0 tsantor    (501) staff       (20)       69 2024-05-10 21:14:08.000000 sharepoint_too-0.3.0/setup.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-21 17:24:54.257434 sharepoint_too-0.3.0/src/
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-21 17:24:54.259166 sharepoint_too-0.3.0/src/sharepoint_too/
+-rwxr-xr-x   0 tsantor    (501) staff       (20)       70 2024-05-10 19:53:32.000000 sharepoint_too-0.3.0/src/sharepoint_too/__init__.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     9602 2024-05-14 21:10:58.000000 sharepoint_too-0.3.0/src/sharepoint_too/session.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-21 17:24:54.260584 sharepoint_too-0.3.0/src/sharepoint_too.egg-info/
+-rw-r--r--   0 tsantor    (501) staff       (20)     4796 2024-05-21 17:24:54.000000 sharepoint_too-0.3.0/src/sharepoint_too.egg-info/PKG-INFO
+-rw-r--r--   0 tsantor    (501) staff       (20)      374 2024-05-21 17:24:54.000000 sharepoint_too-0.3.0/src/sharepoint_too.egg-info/SOURCES.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)        1 2024-05-21 17:24:54.000000 sharepoint_too-0.3.0/src/sharepoint_too.egg-info/dependency_links.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       30 2024-05-21 17:24:54.000000 sharepoint_too-0.3.0/src/sharepoint_too.egg-info/requires.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       15 2024-05-21 17:24:54.000000 sharepoint_too-0.3.0/src/sharepoint_too.egg-info/top_level.txt
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-05-21 17:24:54.260250 sharepoint_too-0.3.0/tests/
+-rw-r--r--   0 tsantor    (501) staff       (20)     5683 2024-05-10 22:06:44.000000 sharepoint_too-0.3.0/tests/test_sharepoint_too.py
```

### Comparing `sharepoint-too-0.2.0/HISTORY.md` & `sharepoint_too-0.3.0/HISTORY.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 # History
+
 All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).
 
-## 0.1.0 (2020-04-27)
-* First release on PyPI.
+## 0.3.0 (2024-05-10)
 
-## 0.1.1 (2020-04-27)
-* Updated license and installaton instructions due to typo.
+- **Changed**: Use modern Python tooling. Update to work with Python 3.9.x.
+
+## 0.2.0 (2021-09-23)
+
+- **Changed**: Now you must pass on open file as content along with desired filename. We can't assume the file is local, it may be local or in the cloud. Such as with Django storages.
 
 ## 0.1.2 (2020-06-08)
-* When uploading a file to SharePoint we use just the filename and not the full file path.
 
+- When uploading a file to SharePoint we use just the filename and not the full file path.
 
-## 0.2.0 (2021-09-23)
-* **Changed**: Now you must pass on open file as content along with desired filename. We can't assume the file is local, it may be local or in the cloud. Such as with Django storages.
+## 0.1.1 (2020-04-27)
+
+- Updated license and installaton instructions due to typo.
+
+## 0.1.0 (2020-04-27)
+
+- First release on PyPI.
```

### Comparing `sharepoint-too-0.2.0/LICENSE` & `sharepoint_too-0.3.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # The MIT License (MIT)
 
-Copyright (c) 2020 Tim Santor
+Copyright (c) 2020-2024, Tim Santor
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to use,
+copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
+Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `sharepoint-too-0.2.0/PKG-INFO` & `sharepoint_too-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,113 +1,131 @@
 Metadata-Version: 2.1
 Name: sharepoint-too
-Version: 0.2.0
+Version: 0.3.0
 Summary: This module will handle authentication for your SharePoint Online/O365 site, allowing you to make straightforward HTTP requests from Python. It extends the commonly used Requests module, meaning that returned objects are familliar, easy to work with and well documented.
-Home-page: https://github.com/tsantor/sharepoint-too
-Author: Tim Santor
-Author-email: tsantor@xstudios.com
-License: MIT
-Description: # SharePoint Too
-        Author:Tim Santor <tsantor@xstudios.agency>
-        
-        ## Overview
-        This module will handle authentication for your SharePoint Online/O365 site, allowing you to make straightforward HTTP requests from Python. It extends the commonly used Requests module, meaning that returned objects are familliar, easy to work with and well documented. Leverages [requests_ntlm](https://github.com/requests/requests-ntlm) for authentication.
-        
-        Inspired by [Sharepy](https://github.com/JonathanHolvey/sharepy) which seems to no longer be maintained.
-        
-        **NOTE:** Currently handles dealing with SharePoint Lists via handy shortcut methods, but you can currently also call `sp.get(url, *args, **kwargs)` and `sp.post(url, *args, **kwargs)` with manually assembled SharePoint REST URLs and it will work.
-        
-        ## Installation
-        SharePoint Too can be installed from the Python Package Index, PyPI.
-        
-            pip install sharepoint-too
-        
-        ## Initiate a SharePoint session
-        
-            from sharepoint_too import SharePointSession
-            sp = SharePointSession("example.sharepoint.com")
-        
-        ## Make an API call
-        
-            r = sp.get_lists()
-        
-        This will return a Requests `response` object. See the [requests documentation](http://docs.python-requests.org/en/master/) for details. By default, the headers `accept: application/json;odata=verbose` and` content-type: application/json;odata=verbose` are sent with all requests, so API responses will be formatted as JSON where available.
-        
-        Headers can be added or overridden by supplying a dictionary to the relevant method:
-        
-            r = sp.get_lists(headers={"Accept": "application/atom+xml"})
-        
-        Currently the `post()` method will send a `x-requestdigest` header, allowing modifications to be made to SharePoint objects.
-        
-        ## Other available methods
-        
-            sp.get_list_metadata(weblist_url, list_guid=None, list_title=None)
-            sp.get_list_entity_type(weblist_url, list_guid=None, list_title=None)
-            sp.get_list_items(weblist_url, list_guid=None, list_title=None)
-            sp.get_list_item(weblist_url, item_id, list_guid=None, list_title=None)
-            sp.add_list_item(weblist_url, payload, list_guid=None, list_title=None)
-            sp.update_list_item(weblist_url, item_id, data, list_guid=None, list_title=None)
-            sp.upload(weblist_url, item_id, filename, list_guid=None, list_title=None)
-            sp.delete_list_item(weblist_url, item_id, list_guid=None, list_title=None)
-        
-        **NOTE:** Only `list_guid` or `list_title` need to be supplied, not both.
-        
-        ## Tests
-        Since the tests require a SharePoint account you'll need to supply private values in order to run the tests:
-        
-        Create a file called `~/sharepoint_too/config.cfg`:
-        
-            [default]
-            domain=
-            user=
-            pwd=
-            site_url=https://example.sharepoint.com
-            weblist_url=https://example.sharepoint.com/_api/web/lists
-            list_title=
-            list_guid=
-            list_item_type=
-        
-        
-        Now you can run:
-        
-            python -m pytest tests/test_sharepoint_too.py
-        
-        ## Documentation
-        Documentation is available at TODO
-        
-        ## Requirements
-        
-        - [requests](https://github.com/psf/requests)
-        - [requests_ntlm](https://github.com/requests/requests-ntlm)
-        
-        # Issues
-        If you experience any issues, please create an [issue](https://bitbucket.org/tsantor/sharepoint-too/issues) on Bitbucket.
-        
-        
-        # History
-        All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).
-        
-        ## 0.1.0 (2020-04-27)
-        * First release on PyPI.
-        
-        ## 0.1.1 (2020-04-27)
-        * Updated license and installaton instructions due to typo.
-        
-        ## 0.1.2 (2020-06-08)
-        * When uploading a file to SharePoint we use just the filename and not the full file path.
-        
-        
-        ## 0.2.0 (2021-09-23)
-        * **Changed**: Now you must pass on open file as content along with desired filename. We can't assume the file is local, it may be local or in the cloud. Such as with Django storages.
-        
-Keywords: sharepoint-too
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Author-email: Tim Santor <tsantor@xstudios.com>
+Project-URL: Repository, https://github.com/tsantor/sharepoint-too.git
+Project-URL: Issues, https://github.com/tsantor/sharepoint-too/issues
+Project-URL: Changelog, https://github.com/tsantor/sharepoint-too/blob/master/HISTORY.md
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+Requires-Dist: requests_ntlm
+Requires-Dist: requests
+Provides-Extra: dev
+
+# SharePoint Too
+
+![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen)
+
+## Overview
+
+This module will handle authentication for your SharePoint Online/O365 site, allowing you to make straightforward HTTP requests from Python. It extends the commonly used Requests module, meaning that returned objects are familliar, easy to work with and well documented. Leverages [requests_ntlm](https://github.com/requests/requests-ntlm) for authentication.
+
+Inspired by [Sharepy](https://github.com/JonathanHolvey/sharepy) which seems to no longer be maintained.
+
+**NOTE:** Currently handles dealing with SharePoint Lists via handy shortcut methods, but you can currently also call `sp.get(url, *args, **kwargs)` and `sp.post(url, *args, **kwargs)` with manually assembled SharePoint REST URLs and it will work.
+
+## Installation
+
+```bash
+python3 -m pip install sharepoint-too
+```
+
+## Usage
+
+### Initiate a SharePoint session
+
+```python
+from sharepoint_too import SharePointSession
+sp = SharePointSession("example.sharepoint.com")
+```
+
+### Make an API call
+
+```python
+r = sp.get_lists()
+```
+
+This will return a Requests `response` object. See the [requests documentation](http://docs.python-requests.org/en/master/) for details. By default, the headers `accept: application/json;odata=verbose` and` content-type: application/json;odata=verbose` are sent with all requests, so API responses will be formatted as JSON where available.
+
+Headers can be added or overridden by supplying a dictionary to the relevant method:
+
+```python
+r = sp.get_lists(headers={"Accept": "application/atom+xml"})
+```
+
+Currently the `post()` method will send a `x-requestdigest` header, allowing modifications to be made to SharePoint objects.
+
+### Other available methods
+
+```python
+sp.get_list_metadata(weblist_url, list_guid=None, list_title=None)
+sp.get_list_entity_type(weblist_url, list_guid=None, list_title=None)
+sp.get_list_items(weblist_url, list_guid=None, list_title=None)
+sp.get_list_item(weblist_url, item_id, list_guid=None, list_title=None)
+sp.add_list_item(weblist_url, payload, list_guid=None, list_title=None)
+sp.update_list_item(weblist_url, item_id, data, list_guid=None, list_title=None)
+sp.upload(weblist_url, item_id, filename, list_guid=None, list_title=None)
+sp.delete_list_item(weblist_url, item_id, list_guid=None, list_title=None)
+```
+
+**NOTE:** Only `list_guid` or `list_title` need to be supplied, not both.
+
+<!-- ## Documentation
+Visit the docs [here](https://github.io/tsantor/sharepoint-too/docs/) -->
+
+## Development
+
+To get a list of all commands with descriptions simply run `make`.
+
+```bash
+make env
+make pip_install
+make pip_install_editable
+```
+
+## Testing
+
+```bash
+make pytest
+make coverage
+make open_coverage
+```
+
+## Issues
+
+If you experience any issues, please create an [issue](https://github.com/tsantor/sharepoint-too/issues) on GitHub.
+
+# History
+
+All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).
+
+## 0.3.0 (2024-05-10)
+
+- **Changed**: Use modern Python tooling. Update to work with Python 3.9.x.
+
+## 0.2.0 (2021-09-23)
+
+- **Changed**: Now you must pass on open file as content along with desired filename. We can't assume the file is local, it may be local or in the cloud. Such as with Django storages.
+
+## 0.1.2 (2020-06-08)
+
+- When uploading a file to SharePoint we use just the filename and not the full file path.
+
+## 0.1.1 (2020-04-27)
+
+- Updated license and installaton instructions due to typo.
+
+## 0.1.0 (2020-04-27)
+
+- First release on PyPI.
```

### Comparing `sharepoint-too-0.2.0/README.md` & `sharepoint_too-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,82 @@
 # SharePoint Too
-Author:Tim Santor <tsantor@xstudios.agency>
+
+![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen)
 
 ## Overview
+
 This module will handle authentication for your SharePoint Online/O365 site, allowing you to make straightforward HTTP requests from Python. It extends the commonly used Requests module, meaning that returned objects are familliar, easy to work with and well documented. Leverages [requests_ntlm](https://github.com/requests/requests-ntlm) for authentication.
 
 Inspired by [Sharepy](https://github.com/JonathanHolvey/sharepy) which seems to no longer be maintained.
 
 **NOTE:** Currently handles dealing with SharePoint Lists via handy shortcut methods, but you can currently also call `sp.get(url, *args, **kwargs)` and `sp.post(url, *args, **kwargs)` with manually assembled SharePoint REST URLs and it will work.
 
 ## Installation
-SharePoint Too can be installed from the Python Package Index, PyPI.
 
-    pip install sharepoint-too
+```bash
+python3 -m pip install sharepoint-too
+```
+
+## Usage
 
-## Initiate a SharePoint session
+### Initiate a SharePoint session
 
-    from sharepoint_too import SharePointSession
-    sp = SharePointSession("example.sharepoint.com")
+```python
+from sharepoint_too import SharePointSession
+sp = SharePointSession("example.sharepoint.com")
+```
 
-## Make an API call
+### Make an API call
 
-    r = sp.get_lists()
+```python
+r = sp.get_lists()
+```
 
 This will return a Requests `response` object. See the [requests documentation](http://docs.python-requests.org/en/master/) for details. By default, the headers `accept: application/json;odata=verbose` and` content-type: application/json;odata=verbose` are sent with all requests, so API responses will be formatted as JSON where available.
 
 Headers can be added or overridden by supplying a dictionary to the relevant method:
 
-    r = sp.get_lists(headers={"Accept": "application/atom+xml"})
+```python
+r = sp.get_lists(headers={"Accept": "application/atom+xml"})
+```
 
 Currently the `post()` method will send a `x-requestdigest` header, allowing modifications to be made to SharePoint objects.
 
-## Other available methods
+### Other available methods
 
-    sp.get_list_metadata(weblist_url, list_guid=None, list_title=None)
-    sp.get_list_entity_type(weblist_url, list_guid=None, list_title=None)
-    sp.get_list_items(weblist_url, list_guid=None, list_title=None)
-    sp.get_list_item(weblist_url, item_id, list_guid=None, list_title=None)
-    sp.add_list_item(weblist_url, payload, list_guid=None, list_title=None)
-    sp.update_list_item(weblist_url, item_id, data, list_guid=None, list_title=None)
-    sp.upload(weblist_url, item_id, filename, list_guid=None, list_title=None)
-    sp.delete_list_item(weblist_url, item_id, list_guid=None, list_title=None)
+```python
+sp.get_list_metadata(weblist_url, list_guid=None, list_title=None)
+sp.get_list_entity_type(weblist_url, list_guid=None, list_title=None)
+sp.get_list_items(weblist_url, list_guid=None, list_title=None)
+sp.get_list_item(weblist_url, item_id, list_guid=None, list_title=None)
+sp.add_list_item(weblist_url, payload, list_guid=None, list_title=None)
+sp.update_list_item(weblist_url, item_id, data, list_guid=None, list_title=None)
+sp.upload(weblist_url, item_id, filename, list_guid=None, list_title=None)
+sp.delete_list_item(weblist_url, item_id, list_guid=None, list_title=None)
+```
 
 **NOTE:** Only `list_guid` or `list_title` need to be supplied, not both.
 
-## Tests
-Since the tests require a SharePoint account you'll need to supply private values in order to run the tests:
-
-Create a file called `~/sharepoint_too/config.cfg`:
-
-    [default]
-    domain=
-    user=
-    pwd=
-    site_url=https://example.sharepoint.com
-    weblist_url=https://example.sharepoint.com/_api/web/lists
-    list_title=
-    list_guid=
-    list_item_type=
+<!-- ## Documentation
+Visit the docs [here](https://github.io/tsantor/sharepoint-too/docs/) -->
 
+## Development
 
-Now you can run:
+To get a list of all commands with descriptions simply run `make`.
 
-    python -m pytest tests/test_sharepoint_too.py
+```bash
+make env
+make pip_install
+make pip_install_editable
+```
 
-## Documentation
-Documentation is available at TODO
+## Testing
 
-## Requirements
+```bash
+make pytest
+make coverage
+make open_coverage
+```
 
-- [requests](https://github.com/psf/requests)
-- [requests_ntlm](https://github.com/requests/requests-ntlm)
+## Issues
 
-# Issues
-If you experience any issues, please create an [issue](https://bitbucket.org/tsantor/sharepoint-too/issues) on Bitbucket.
+If you experience any issues, please create an [issue](https://github.com/tsantor/sharepoint-too/issues) on GitHub.
```

### Comparing `sharepoint-too-0.2.0/sharepoint_too.egg-info/PKG-INFO` & `sharepoint_too-0.3.0/src/sharepoint_too.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,113 +1,131 @@
 Metadata-Version: 2.1
 Name: sharepoint-too
-Version: 0.2.0
+Version: 0.3.0
 Summary: This module will handle authentication for your SharePoint Online/O365 site, allowing you to make straightforward HTTP requests from Python. It extends the commonly used Requests module, meaning that returned objects are familliar, easy to work with and well documented.
-Home-page: https://github.com/tsantor/sharepoint-too
-Author: Tim Santor
-Author-email: tsantor@xstudios.com
-License: MIT
-Description: # SharePoint Too
-        Author:Tim Santor <tsantor@xstudios.agency>
-        
-        ## Overview
-        This module will handle authentication for your SharePoint Online/O365 site, allowing you to make straightforward HTTP requests from Python. It extends the commonly used Requests module, meaning that returned objects are familliar, easy to work with and well documented. Leverages [requests_ntlm](https://github.com/requests/requests-ntlm) for authentication.
-        
-        Inspired by [Sharepy](https://github.com/JonathanHolvey/sharepy) which seems to no longer be maintained.
-        
-        **NOTE:** Currently handles dealing with SharePoint Lists via handy shortcut methods, but you can currently also call `sp.get(url, *args, **kwargs)` and `sp.post(url, *args, **kwargs)` with manually assembled SharePoint REST URLs and it will work.
-        
-        ## Installation
-        SharePoint Too can be installed from the Python Package Index, PyPI.
-        
-            pip install sharepoint-too
-        
-        ## Initiate a SharePoint session
-        
-            from sharepoint_too import SharePointSession
-            sp = SharePointSession("example.sharepoint.com")
-        
-        ## Make an API call
-        
-            r = sp.get_lists()
-        
-        This will return a Requests `response` object. See the [requests documentation](http://docs.python-requests.org/en/master/) for details. By default, the headers `accept: application/json;odata=verbose` and` content-type: application/json;odata=verbose` are sent with all requests, so API responses will be formatted as JSON where available.
-        
-        Headers can be added or overridden by supplying a dictionary to the relevant method:
-        
-            r = sp.get_lists(headers={"Accept": "application/atom+xml"})
-        
-        Currently the `post()` method will send a `x-requestdigest` header, allowing modifications to be made to SharePoint objects.
-        
-        ## Other available methods
-        
-            sp.get_list_metadata(weblist_url, list_guid=None, list_title=None)
-            sp.get_list_entity_type(weblist_url, list_guid=None, list_title=None)
-            sp.get_list_items(weblist_url, list_guid=None, list_title=None)
-            sp.get_list_item(weblist_url, item_id, list_guid=None, list_title=None)
-            sp.add_list_item(weblist_url, payload, list_guid=None, list_title=None)
-            sp.update_list_item(weblist_url, item_id, data, list_guid=None, list_title=None)
-            sp.upload(weblist_url, item_id, filename, list_guid=None, list_title=None)
-            sp.delete_list_item(weblist_url, item_id, list_guid=None, list_title=None)
-        
-        **NOTE:** Only `list_guid` or `list_title` need to be supplied, not both.
-        
-        ## Tests
-        Since the tests require a SharePoint account you'll need to supply private values in order to run the tests:
-        
-        Create a file called `~/sharepoint_too/config.cfg`:
-        
-            [default]
-            domain=
-            user=
-            pwd=
-            site_url=https://example.sharepoint.com
-            weblist_url=https://example.sharepoint.com/_api/web/lists
-            list_title=
-            list_guid=
-            list_item_type=
-        
-        
-        Now you can run:
-        
-            python -m pytest tests/test_sharepoint_too.py
-        
-        ## Documentation
-        Documentation is available at TODO
-        
-        ## Requirements
-        
-        - [requests](https://github.com/psf/requests)
-        - [requests_ntlm](https://github.com/requests/requests-ntlm)
-        
-        # Issues
-        If you experience any issues, please create an [issue](https://bitbucket.org/tsantor/sharepoint-too/issues) on Bitbucket.
-        
-        
-        # History
-        All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).
-        
-        ## 0.1.0 (2020-04-27)
-        * First release on PyPI.
-        
-        ## 0.1.1 (2020-04-27)
-        * Updated license and installaton instructions due to typo.
-        
-        ## 0.1.2 (2020-06-08)
-        * When uploading a file to SharePoint we use just the filename and not the full file path.
-        
-        
-        ## 0.2.0 (2021-09-23)
-        * **Changed**: Now you must pass on open file as content along with desired filename. We can't assume the file is local, it may be local or in the cloud. Such as with Django storages.
-        
-Keywords: sharepoint-too
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Author-email: Tim Santor <tsantor@xstudios.com>
+Project-URL: Repository, https://github.com/tsantor/sharepoint-too.git
+Project-URL: Issues, https://github.com/tsantor/sharepoint-too/issues
+Project-URL: Changelog, https://github.com/tsantor/sharepoint-too/blob/master/HISTORY.md
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+Requires-Dist: requests_ntlm
+Requires-Dist: requests
+Provides-Extra: dev
+
+# SharePoint Too
+
+![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen)
+
+## Overview
+
+This module will handle authentication for your SharePoint Online/O365 site, allowing you to make straightforward HTTP requests from Python. It extends the commonly used Requests module, meaning that returned objects are familliar, easy to work with and well documented. Leverages [requests_ntlm](https://github.com/requests/requests-ntlm) for authentication.
+
+Inspired by [Sharepy](https://github.com/JonathanHolvey/sharepy) which seems to no longer be maintained.
+
+**NOTE:** Currently handles dealing with SharePoint Lists via handy shortcut methods, but you can currently also call `sp.get(url, *args, **kwargs)` and `sp.post(url, *args, **kwargs)` with manually assembled SharePoint REST URLs and it will work.
+
+## Installation
+
+```bash
+python3 -m pip install sharepoint-too
+```
+
+## Usage
+
+### Initiate a SharePoint session
+
+```python
+from sharepoint_too import SharePointSession
+sp = SharePointSession("example.sharepoint.com")
+```
+
+### Make an API call
+
+```python
+r = sp.get_lists()
+```
+
+This will return a Requests `response` object. See the [requests documentation](http://docs.python-requests.org/en/master/) for details. By default, the headers `accept: application/json;odata=verbose` and` content-type: application/json;odata=verbose` are sent with all requests, so API responses will be formatted as JSON where available.
+
+Headers can be added or overridden by supplying a dictionary to the relevant method:
+
+```python
+r = sp.get_lists(headers={"Accept": "application/atom+xml"})
+```
+
+Currently the `post()` method will send a `x-requestdigest` header, allowing modifications to be made to SharePoint objects.
+
+### Other available methods
+
+```python
+sp.get_list_metadata(weblist_url, list_guid=None, list_title=None)
+sp.get_list_entity_type(weblist_url, list_guid=None, list_title=None)
+sp.get_list_items(weblist_url, list_guid=None, list_title=None)
+sp.get_list_item(weblist_url, item_id, list_guid=None, list_title=None)
+sp.add_list_item(weblist_url, payload, list_guid=None, list_title=None)
+sp.update_list_item(weblist_url, item_id, data, list_guid=None, list_title=None)
+sp.upload(weblist_url, item_id, filename, list_guid=None, list_title=None)
+sp.delete_list_item(weblist_url, item_id, list_guid=None, list_title=None)
+```
+
+**NOTE:** Only `list_guid` or `list_title` need to be supplied, not both.
+
+<!-- ## Documentation
+Visit the docs [here](https://github.io/tsantor/sharepoint-too/docs/) -->
+
+## Development
+
+To get a list of all commands with descriptions simply run `make`.
+
+```bash
+make env
+make pip_install
+make pip_install_editable
+```
+
+## Testing
+
+```bash
+make pytest
+make coverage
+make open_coverage
+```
+
+## Issues
+
+If you experience any issues, please create an [issue](https://github.com/tsantor/sharepoint-too/issues) on GitHub.
+
+# History
+
+All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).
+
+## 0.3.0 (2024-05-10)
+
+- **Changed**: Use modern Python tooling. Update to work with Python 3.9.x.
+
+## 0.2.0 (2021-09-23)
+
+- **Changed**: Now you must pass on open file as content along with desired filename. We can't assume the file is local, it may be local or in the cloud. Such as with Django storages.
+
+## 0.1.2 (2020-06-08)
+
+- When uploading a file to SharePoint we use just the filename and not the full file path.
+
+## 0.1.1 (2020-04-27)
+
+- Updated license and installaton instructions due to typo.
+
+## 0.1.0 (2020-04-27)
+
+- First release on PyPI.
```

