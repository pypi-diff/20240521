# Comparing `tmp/widget_periodictable-4.1.0.tar.gz` & `tmp/widget_periodictable-4.1.1.tar.gz`

## Comparing `widget_periodictable-4.1.0.tar` & `widget_periodictable-4.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 widget_periodictable-4.1.0/src/widget_periodictable/__init__.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 widget_periodictable-4.1.0/src/widget_periodictable/utils.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 widget_periodictable-4.1.0/src/widget_periodictable/static/widget.css
--rw-r--r--   0        0        0   113467 2020-02-02 00:00:00.000000 widget_periodictable-4.1.0/src/widget_periodictable/static/widget.js
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 widget_periodictable-4.1.0/.gitignore
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 widget_periodictable-4.1.0/README.md
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 widget_periodictable-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 widget_periodictable-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/src/widget_periodictable/__init__.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/src/widget_periodictable/utils.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/src/widget_periodictable/static/widget.css
+-rw-r--r--   0        0        0   113467 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/src/widget_periodictable/static/widget.js
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/.gitignore
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/README.md
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/PKG-INFO
```

### Comparing `widget_periodictable-4.1.0/src/widget_periodictable/__init__.py` & `widget_periodictable-4.1.1/src/widget_periodictable/__init__.py`

 * *Files identical despite different names*

### Comparing `widget_periodictable-4.1.0/src/widget_periodictable/utils.py` & `widget_periodictable-4.1.1/src/widget_periodictable/utils.py`

 * *Files identical despite different names*

### Comparing `widget_periodictable-4.1.0/src/widget_periodictable/static/widget.css` & `widget_periodictable-4.1.1/src/widget_periodictable/static/widget.css`

 * *Files identical despite different names*

### Comparing `widget_periodictable-4.1.0/src/widget_periodictable/static/widget.js` & `widget_periodictable-4.1.1/src/widget_periodictable/static/widget.js`

 * *Files identical despite different names*

### Comparing `widget_periodictable-4.1.0/PKG-INFO` & `widget_periodictable-4.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,11 @@
-Metadata-Version: 2.3
-Name: widget-periodictable
-Version: 4.1.0
-Keywords: anywidget,jupyter,jupyterlab,mendeleev,osscar,widget
-Requires-Dist: anywidget>=0.9.10
-Provides-Extra: dev
-Requires-Dist: bumpver>=2023; extra == 'dev'
-Requires-Dist: jupyterlab; extra == 'dev'
-Requires-Dist: watchfiles; extra == 'dev'
-Description-Content-Type: text/markdown
-
 # Jupyter widget: Interactive periodic table
 
 [![PyPI version](https://badge.fury.io/py/widget-periodictable.svg)](https://badge.fury.io/py/widget-periodictable)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/osscar-org/widget-periodictable/main?urlpath=%2Fvoila%2Frender%2Fexamples%2Fintroduction.ipynb)
 
 ## Installation & usage
 
 ```sh
 pip install widget-periodictable
 ```
 
@@ -34,12 +24,25 @@
 ```sh
 npm install
 npm run dev
 ```
 
 Open the example notebook in JupyterLab, VS Code, or your favorite editor to start developing. Changes made in `js/` will be reflected in the notebook.
 
+### Releasing and publishing a new version
+
+In order to make a new release of the library and publish to PYPI, run
+
+```bash
+bumpver update --major/--minor/--patch
+```
+
+This will
+
+- update version numbers, make a corresponding `git commit` and a `git tag`;
+- push this commit and tag to Github, which triggers the Github Action that makes a new Github Release and publishes the package to PYPI.
+
 ## Acknowledgements
 
 We acknowledge support from the EPFL Open Science Fund via the [OSSCAR](http://www.osscar.org) project.
 
-<img src='https://www.osscar.org/_images/logos.png' width='700'>
+<img src='https://www.osscar.org/_images/logos.png' width='700'>
```

