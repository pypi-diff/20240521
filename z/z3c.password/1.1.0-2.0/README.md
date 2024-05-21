# Comparing `tmp/z3c.password-1.1.0.tar.gz` & `tmp/z3c.password-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z3c.password-1.1.0.tar", last modified: Tue Dec 14 12:28:19 2021, max compression
+gzip compressed data, was "z3c.password-2.0.tar", last modified: Tue May 21 09:59:48 2024, max compression
```

## Comparing `z3c.password-1.1.0.tar` & `z3c.password-2.0.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-14 12:28:19.910580 z3c.password-1.1.0/
--rw-r--r--   0 mac        (513) staff       (20)     4801 2021-12-14 12:28:19.000000 z3c.password-1.1.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)       32 2021-12-14 12:28:19.000000 z3c.password-1.1.0/COPYRIGHT.rst
--rw-r--r--   0 mac        (513) staff       (20)     2070 2021-12-14 12:28:19.000000 z3c.password-1.1.0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      295 2021-12-14 12:28:19.000000 z3c.password-1.1.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     7106 2021-12-14 12:28:19.910700 z3c.password-1.1.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      915 2021-12-14 12:28:19.000000 z3c.password-1.1.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      221 2021-12-14 12:28:19.911169 z3c.password-1.1.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     2963 2021-12-14 12:28:19.000000 z3c.password-1.1.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-14 12:28:19.900556 z3c.password-1.1.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-14 12:28:19.903855 z3c.password-1.1.0/src/z3c/
--rw-r--r--   0 mac        (513) staff       (20)      207 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-14 12:28:19.909288 z3c.password-1.1.0/src/z3c/password/
--rw-r--r--   0 mac        (513) staff       (20)       24 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/password/DEPENDENCIES.txt
--rw-r--r--   0 mac        (513) staff       (20)    13043 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/password/README.txt
--rw-r--r--   0 mac        (513) staff       (20)      112 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/password/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      869 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/password/_compat.py
--rw-r--r--   0 mac        (513) staff       (20)      203 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/password/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     2270 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/password/field.py
--rw-r--r--   0 mac        (513) staff       (20)    17611 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/password/interfaces.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-14 12:28:19.909546 z3c.password-1.1.0/src/z3c/password/locales/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-14 12:28:19.901102 z3c.password-1.1.0/src/z3c/password/locales/de/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-14 12:28:19.909811 z3c.password-1.1.0/src/z3c/password/locales/de/LC_MESSAGES/
--rw-r--r--   0 mac        (513) staff       (20)    11166 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/password/locales/de/LC_MESSAGES/z3c.password.po
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-14 12:28:19.901345 z3c.password-1.1.0/src/z3c/password/locales/nl/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-14 12:28:19.910078 z3c.password-1.1.0/src/z3c/password/locales/nl/LC_MESSAGES/
--rw-r--r--   0 mac        (513) staff       (20)    10917 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/password/locales/nl/LC_MESSAGES/z3c.password.po
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-14 12:28:19.901587 z3c.password-1.1.0/src/z3c/password/locales/ru/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-14 12:28:19.910346 z3c.password-1.1.0/src/z3c/password/locales/ru/LC_MESSAGES/
--rw-r--r--   0 mac        (513) staff       (20)    10925 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/password/locales/ru/LC_MESSAGES/z3c.password.po
--rw-r--r--   0 mac        (513) staff       (20)     7929 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/password/locales/z3c.password.pot
--rw-r--r--   0 mac        (513) staff       (20)     9398 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/password/password.py
--rw-r--r--   0 mac        (513) staff       (20)     9712 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/password/principal.py
--rw-r--r--   0 mac        (513) staff       (20)    27216 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/password/principal.txt
--rw-r--r--   0 mac        (513) staff       (20)     1374 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/password/testing.py
--rw-r--r--   0 mac        (513) staff       (20)     1711 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/password/tests.py
--rw-r--r--   0 mac        (513) staff       (20)       35 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c/password/z3c.password-configure.zcml
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-14 12:28:19.905723 z3c.password-1.1.0/src/z3c.password.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     7106 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c.password.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1001 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c.password.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c.password.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        4 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c.password.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c.password.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      179 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c.password.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        4 2021-12-14 12:28:19.000000 z3c.password-1.1.0/src/z3c.password.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1241 2021-12-14 12:28:19.000000 z3c.password-1.1.0/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 09:59:48.325837 z3c.password-2.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5006 2024-05-21 09:59:47.000000 z3c.password-2.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2024-05-21 09:59:47.000000 z3c.password-2.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2024-05-21 09:59:47.000000 z3c.password-2.0/COPYRIGHT.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2024-05-21 09:59:47.000000 z3c.password-2.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      335 2024-05-21 09:59:47.000000 z3c.password-2.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7634 2024-05-21 09:59:48.325755 z3c.password-2.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      915 2024-05-21 09:59:47.000000 z3c.password-2.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      452 2024-05-21 09:59:48.326089 z3c.password-2.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2924 2024-05-21 09:59:47.000000 z3c.password-2.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 09:59:48.318617 z3c.password-2.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 09:59:48.320747 z3c.password-2.0/src/z3c/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       77 2024-05-21 09:59:47.000000 z3c.password-2.0/src/z3c/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 09:59:48.323783 z3c.password-2.0/src/z3c/password/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       24 2024-05-21 09:59:47.000000 z3c.password-2.0/src/z3c/password/DEPENDENCIES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12957 2024-05-21 09:59:47.000000 z3c.password-2.0/src/z3c/password/README.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      114 2024-05-21 09:59:47.000000 z3c.password-2.0/src/z3c/password/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      203 2024-05-21 09:59:47.000000 z3c.password-2.0/src/z3c/password/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2188 2024-05-21 09:59:47.000000 z3c.password-2.0/src/z3c/password/field.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    17196 2024-05-21 09:59:47.000000 z3c.password-2.0/src/z3c/password/interfaces.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 09:59:48.323954 z3c.password-2.0/src/z3c/password/locales/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 09:59:48.318989 z3c.password-2.0/src/z3c/password/locales/de/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 09:59:48.324320 z3c.password-2.0/src/z3c/password/locales/de/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6145 2024-05-21 09:59:48.000000 z3c.password-2.0/src/z3c/password/locales/de/LC_MESSAGES/z3c.password.mo
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11166 2024-05-21 09:59:47.000000 z3c.password-2.0/src/z3c/password/locales/de/LC_MESSAGES/z3c.password.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 09:59:48.319152 z3c.password-2.0/src/z3c/password/locales/nl/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 09:59:48.324698 z3c.password-2.0/src/z3c/password/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6276 2024-05-21 09:59:48.000000 z3c.password-2.0/src/z3c/password/locales/nl/LC_MESSAGES/z3c.password.mo
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10917 2024-05-21 09:59:47.000000 z3c.password-2.0/src/z3c/password/locales/nl/LC_MESSAGES/z3c.password.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 09:59:48.319313 z3c.password-2.0/src/z3c/password/locales/ru/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 09:59:48.325057 z3c.password-2.0/src/z3c/password/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2243 2024-05-21 09:59:48.000000 z3c.password-2.0/src/z3c/password/locales/ru/LC_MESSAGES/z3c.password.mo
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10925 2024-05-21 09:59:47.000000 z3c.password-2.0/src/z3c/password/locales/ru/LC_MESSAGES/z3c.password.po
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7929 2024-05-21 09:59:47.000000 z3c.password-2.0/src/z3c/password/locales/z3c.password.pot
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9370 2024-05-21 09:59:47.000000 z3c.password-2.0/src/z3c/password/password.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9645 2024-05-21 09:59:47.000000 z3c.password-2.0/src/z3c/password/principal.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    27216 2024-05-21 09:59:47.000000 z3c.password-2.0/src/z3c/password/principal.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1374 2024-05-21 09:59:47.000000 z3c.password-2.0/src/z3c/password/testing.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1216 2024-05-21 09:59:47.000000 z3c.password-2.0/src/z3c/password/tests.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       35 2024-05-21 09:59:47.000000 z3c.password-2.0/src/z3c/password/z3c.password-configure.zcml
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 09:59:48.325331 z3c.password-2.0/src/z3c.password.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7634 2024-05-21 09:59:48.000000 z3c.password-2.0/src/z3c.password.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1157 2024-05-21 09:59:48.000000 z3c.password-2.0/src/z3c.password.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-05-21 09:59:48.000000 z3c.password-2.0/src/z3c.password.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        4 2024-05-21 09:59:48.000000 z3c.password-2.0/src/z3c.password.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-05-21 09:59:48.000000 z3c.password-2.0/src/z3c.password.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      179 2024-05-21 09:59:48.000000 z3c.password-2.0/src/z3c.password.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        4 2024-05-21 09:59:48.000000 z3c.password-2.0/src/z3c.password.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1880 2024-05-21 09:59:47.000000 z3c.password-2.0/tox.ini
```

### Comparing `z3c.password-1.1.0/CHANGES.rst` & `z3c.password-2.0/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 =======
 CHANGES
 =======
 
+2.0 (2024-05-21)
+----------------
+
+- Add support for Python 3.11, 3.12.
+
+- Compile ``*.mo`` files at release time instead of including them in the
+  repository.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 1.1.0 (2021-12-14)
 ------------------
 
 - Add support for Python 3.8, 3.9 and 3.10.
 
 - Drop support for Python 3.4.
```

### Comparing `z3c.password-1.1.0/LICENSE.txt` & `z3c.password-2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `z3c.password-1.1.0/PKG-INFO` & `z3c.password-2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 Metadata-Version: 2.1
 Name: z3c.password
-Version: 1.1.0
+Version: 2.0
 Summary: Password generation and verification utility for Zope3
 Home-page: http://pypi.org/project/z3c.password
 Author: Stephan Richter, Roger Ineichen and the Zope Community
-Author-email: zope3-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: zope3 z3c password verification
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
-Provides-Extra: test
+Requires-Python: >=3.7
 License-File: LICENSE.txt
+Requires-Dist: setuptools
+Requires-Dist: zope.component
+Requires-Dist: zope.exceptions
+Requires-Dist: zope.i18nmessageid
+Requires-Dist: zope.i18n
+Requires-Dist: zope.interface
+Requires-Dist: zope.schema
+Requires-Dist: zope.security
+Provides-Extra: test
+Requires-Dist: z3c.coverage; extra == "test"
+Requires-Dist: zope.password; extra == "test"
+Requires-Dist: zope.pluggableauth; extra == "test"
+Requires-Dist: zope.testing; extra == "test"
 
 ============
 z3c.password
 ============
 
 
 .. image:: https://github.com/zopefoundation/z3c.password/actions/workflows/tests.yml/badge.svg
@@ -54,14 +64,25 @@
 offers a field and a property for those fields.
 
 
 =======
 CHANGES
 =======
 
+2.0 (2024-05-21)
+----------------
+
+- Add support for Python 3.11, 3.12.
+
+- Compile ``*.mo`` files at release time instead of including them in the
+  repository.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 1.1.0 (2021-12-14)
 ------------------
 
 - Add support for Python 3.8, 3.9 and 3.10.
 
 - Drop support for Python 3.4.
 
@@ -228,9 +249,7 @@
   to change it's password. This should not happen if the user did not enter a
   valid password.
 
 0.5.0 (2008-10-21)
 ------------------
 
 - Initial Release
-
-
```

### Comparing `z3c.password-1.1.0/README.rst` & `z3c.password-2.0/README.rst`

 * *Files identical despite different names*

### Comparing `z3c.password-1.1.0/setup.py` & `z3c.password-2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,60 +10,62 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Setup
 """
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 setup(
     name='z3c.password',
-    version='1.1.0',
+    version='2.0',
     author="Stephan Richter, Roger Ineichen and the Zope Community",
-    author_email="zope3-dev@zope.org",
+    author_email="zope-dev@zope.dev",
     description="Password generation and verification utility for Zope3",
     long_description=(
         read('README.rst')
         + '\n\n' +
         read('CHANGES.rst')
     ),
     license="ZPL 2.1",
     keywords="zope3 z3c password verification",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython',
-        "Programming Language :: Python :: Implementation :: PyPy",
+        'Programming Language :: Python :: Implementation :: PyPy',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Topic :: Internet :: WWW/HTTP',
-        'Framework :: Zope :: 3'],
+        'Framework :: Zope :: 3',
+    ],
     url='http://pypi.org/project/z3c.password',
     packages=find_packages('src'),
     include_package_data=True,
     package_dir={'': 'src'},
     namespace_packages=['z3c'],
+    python_requires='>=3.7',
     extras_require=dict(
         test=[
             'z3c.coverage',
             'zope.password',
             'zope.pluggableauth',
             'zope.testing',
         ],
```

### Comparing `z3c.password-1.1.0/src/z3c/password/README.txt` & `z3c.password-2.0/src/z3c/password/README.txt`

 * *Files 2% similar despite different names*

```diff
@@ -130,16 +130,15 @@
   TooManyGroupCharacters: Password contains too many characters of one group (should have at most 6).
 
   >>> pwd.verify('........')
   Traceback (most recent call last):
   ...
   TooManyGroupCharacters: Password contains too many characters of one group (should have at most 6).
 
-  >>> from z3c.password._compat import unichr
-  >>> pwd.verify(unichr(0x0e1)*8)
+  >>> pwd.verify(chr(0x0e1)*8)
   Traceback (most recent call last):
   ...
   TooManyGroupCharacters: Password contains too many characters of one group (should have at most 6).
 
 Let's now verify a list of password that were provided by a bank:
 
   >>> for new in ('K7PzX2JZ', 'DznMLIww', 'ks59Ursq', 'YUcsuIrQ', 'bPEUFGSa',
@@ -252,25 +251,25 @@
   True
 
 We want to have at least 5 others in the password:
 
   >>> pwd = password.HighSecurityPasswordUtility(seed=8)
   >>> pwd.minOthers = 5
 
-  >>> pwd.verify('foobar'+unichr(0x0c3)+unichr(0x0c4))
+  >>> pwd.verify('foobar'+chr(0x0c3)+chr(0x0c4))
   Traceback (most recent call last):
   ...
   TooFewGroupCharactersOthers: Password does not contain enough characters of other characters (should have at least 5).
 
-  >>> pwd.verify('foobar'+unichr(0x0c3)+unichr(0x0c4)+unichr(0x0e1))
+  >>> pwd.verify('foobar'+chr(0x0c3)+chr(0x0c4)+chr(0x0e1))
   Traceback (most recent call last):
   ...
   TooFewGroupCharactersOthers: Password does not contain enough characters of other characters (should have at least 5).
 
-  >>> pwd.verify('fOO'+unichr(0x0e1)*5)
+  >>> pwd.verify('fOO'+chr(0x0e1)*5)
 
 
 Generating passwords with others not yet supported
 
   #>>> pwd.generate()
   #'?d{*~2q|P'
   #
@@ -335,21 +334,21 @@
   >>> from zope.password.password import PlainTextPasswordManager
   >>> from z3c.password import field
 
   >>> pwd = password.HighSecurityPasswordUtility(seed=8)
 
   >>> pwdField = field.Password(
   ...     __name__='password',
-  ...     title=u'Password',
+  ...     title='Password',
   ...     checker=pwd)
 
 Let's validate a value:
 
-  >>> pwdField.validate(u'fooBar12')
-  >>> pwdField.validate(u'fooBar')
+  >>> pwdField.validate('fooBar12')
+  >>> pwdField.validate('fooBar')
   Traceback (most recent call last):
   ...
   TooShortPassword: Password is too short (minimum length: 8).
 
 Validation must work on bound fields too:
 
 Let's now create a principal:
@@ -357,95 +356,95 @@
   >>> from zope.pluggableauth.plugins import principalfolder
   >>> from z3c.password import principal
 
   >>> class MyPrincipal(principal.PrincipalMixIn,
   ...                   principalfolder.InternalPrincipal):
   ...     pass
 
-  >>> user = MyPrincipal('srichter', '123123', u'Stephan Richter')
+  >>> user = MyPrincipal('srichter', '123123', 'Stephan Richter')
 
 Bind the field:
 
   >>> bound = pwdField.bind(user)
 
-  >>> bound.validate(u'fooBar12')
-  >>> bound.validate(u'fooBar')
+  >>> bound.validate('fooBar12')
+  >>> bound.validate('fooBar')
   Traceback (most recent call last):
   ...
   TooShortPassword: Password is too short (minimum length: 8).
 
 Let's create a principal without the PrincipalMixIn:
 
   >>> user = principalfolder.InternalPrincipal('srichter', '123123',
-  ...     u'Stephan Richter')
+  ...     'Stephan Richter')
 
 Bind the field:
 
   >>> bound = pwdField.bind(user)
 
-  >>> bound.validate(u'fooBar12')
-  >>> bound.validate(u'fooBar')
+  >>> bound.validate('fooBar12')
+  >>> bound.validate('fooBar')
   Traceback (most recent call last):
   ...
   TooShortPassword: Password is too short (minimum length: 8).
 
 
 Other common usecase is to do a utility and specify it's name as checker.
 
   >>> import zope.component
   >>> zope.component.provideUtility(pwd, name='my password checker')
 
 Recreate the field:
 
   >>> pwdField = field.Password(
   ...     __name__='password',
-  ...     title=u'Password',
+  ...     title='Password',
   ...     checker='my password checker')
 
 Let's validate a value:
 
-  >>> pwdField.validate(u'fooBar12')
-  >>> pwdField.validate(u'fooBar')
+  >>> pwdField.validate('fooBar12')
+  >>> pwdField.validate('fooBar')
   Traceback (most recent call last):
   ...
   TooShortPassword: Password is too short (minimum length: 8).
 
 
 Edge cases.
 
 No checker specified.
 
   >>> pwdField = field.Password(
   ...     __name__='password',
-  ...     title=u'Password')
+  ...     title='Password')
 
 Validation silently succeeds with a checker:
 
-  >>> pwdField.validate(u'fooBar12')
-  >>> pwdField.validate(u'fooBar')
+  >>> pwdField.validate('fooBar12')
+  >>> pwdField.validate('fooBar')
 
 Bad utility name.
 
   >>> pwdField = field.Password(
   ...     __name__='password',
-  ...     title=u'Password',
+  ...     title='Password',
   ...     checker='foobar password checker')
 
 Burps on the utility lookup as expected:
 
-  >>> pwdField.validate(u'fooBar12')
+  >>> pwdField.validate('fooBar12')
   Traceback (most recent call last):
   ...
   ComponentLookupError:...
 
 Bound object does not have the property:
 
   >>> pwdField = field.Password(
   ...     __name__='foobar',
-  ...     title=u'Password',
+  ...     title='Password',
   ...     checker=pwd)
 
   >>> bound = pwdField.bind(user)
 
 Validation silently succeeds:
 
-  >>> bound.validate(u'fooBar12')
+  >>> bound.validate('fooBar12')
```

### Comparing `z3c.password-1.1.0/src/z3c/password/field.py` & `z3c.password-2.0/src/z3c/password/field.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,42 +11,42 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Password Field Implementation
 """
 import zope.component
 import zope.schema
+
 from z3c.password import interfaces
-from z3c.password._compat import string_types
 
 
 class Password(zope.schema.Password):
 
     def __init__(self, checker=None, ignoreEmpty=False, **kw):
         self._checker = checker
         self._ignoreEmpty = ignoreEmpty
-        super(Password, self).__init__(**kw)
+        super().__init__(**kw)
 
     @property
     def checker(self):
         if self._checker is None:
             return None
-        if not isinstance(self._checker, string_types):
+        if not isinstance(self._checker, str):
             return self._checker
         return zope.component.getUtility(
             interfaces.IPasswordUtility, self._checker)
 
     def validate(self, value):
         if not value and self._ignoreEmpty:
             # leaving a password empty worked fine with formlib,
             # but seems not to work with z3c.form, value get always validated
             # but we would want to leave the old password in place
             return
 
-        super(Password, self).validate(value)
+        super().validate(value)
         old = None
         if self.context is not None:
             try:
                 old = self.get(self.context)
             except AttributeError:
                 pass
         checker = self.checker
```

### Comparing `z3c.password-1.1.0/src/z3c/password/interfaces.py` & `z3c.password-2.0/src/z3c/password/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """Invalid Password"""
 
     i18n_message = None
 
     def __str__(self):
         if self.i18n_message:
             return translate(self.i18n_message)
-        return super(InvalidPassword, self).__str__()
+        return super().__str__()
 
     def doc(self):
         if self.i18n_message:
             return self.i18n_message
         return self.__class__.__doc__
 
 
@@ -40,39 +40,39 @@
     __doc__ = _('''No new password specified.''')
 
 
 class TooShortPassword(InvalidPassword):
     __doc__ = _('''Password is too short.''')
 
     def __init__(self, minLength=None):
-        super(TooShortPassword, self).__init__()
+        super().__init__()
         self.minLength = minLength
         if minLength is not None:
             self.i18n_message = _(
                 'Password is too short (minimum length: ${minLength}).',
                 mapping=dict(minLength=minLength))
 
 
 class TooLongPassword(InvalidPassword):
     __doc__ = _('''Password is too long.''')
 
     def __init__(self, maxLength=None):
-        super(TooLongPassword, self).__init__()
+        super().__init__()
         self.maxLength = maxLength
         if maxLength is not None:
             self.i18n_message = _(
                 'Password is too long (maximum length: ${maxLength}).',
                 mapping=dict(maxLength=maxLength))
 
 
 class TooSimilarPassword(InvalidPassword):
     __doc__ = _('''Password is too similar to old one.''')
 
     def __init__(self, similarity=None, maxSimilarity=None):
-        super(TooSimilarPassword, self).__init__()
+        super().__init__()
         self.similarity = similarity
         self.maxSimilarity = maxSimilarity
         if similarity is not None and maxSimilarity is not None:
             self.i18n_message = _(
                 'Password is too similar to old one'
                 ' (similarity ${similarity}%, should be at most'
                 ' ${maxSimilarity}%).',
@@ -80,15 +80,15 @@
                              maxSimilarity=int(maxSimilarity * 100)))
 
 
 class TooManyGroupCharacters(InvalidPassword):
     __doc__ = _('''Password contains too many characters of one group.''')
 
     def __init__(self, groupMax=None):
-        super(TooManyGroupCharacters, self).__init__()
+        super().__init__()
         self.groupMax = groupMax
         if groupMax is not None:
             self.i18n_message = _(
                 'Password contains too many characters of one group'
                 ' (should have at most ${groupMax}).',
                 mapping=dict(groupMax=groupMax))
 
@@ -99,96 +99,96 @@
 
 
 class TooFewGroupCharactersLowerLetter(TooFewGroupCharacters):
     __doc__ = _(
         'Password does not contain enough characters of lowercase letters.')
 
     def __init__(self, minLowerLetter=None):
-        super(TooFewGroupCharactersLowerLetter, self).__init__()
+        super().__init__()
         self.minLowerLetter = minLowerLetter
         if minLowerLetter is not None:
             self.i18n_message = _(
                 'Password does not contain enough characters of lowercase'
                 ' letters (should have at least ${minLowerLetter}).',
                 mapping=dict(minLowerLetter=minLowerLetter))
 
 
 class TooFewGroupCharactersUpperLetter(TooFewGroupCharacters):
     __doc__ = _(
         'Password does not contain enough characters of uppercase letters.')
 
     def __init__(self, minUpperLetter=None):
-        super(TooFewGroupCharactersUpperLetter, self).__init__()
+        super().__init__()
         self.minUpperLetter = minUpperLetter
         if minUpperLetter is not None:
             self.i18n_message = _(
                 'Password does not contain enough characters of uppercase'
                 ' letters (should have at least ${minUpperLetter}).',
                 mapping=dict(minUpperLetter=minUpperLetter))
 
 
 class TooFewGroupCharactersDigits(TooFewGroupCharacters):
     __doc__ = _('''Password does not contain enough characters of digits.''')
 
     def __init__(self, minDigits=None):
-        super(TooFewGroupCharactersDigits, self).__init__()
+        super().__init__()
         self.minDigits = minDigits
         if minDigits is not None:
             self.i18n_message = _(
                 'Password does not contain enough characters of digits'
                 ' (should have at least ${minDigits}).',
                 mapping=dict(minDigits=minDigits))
 
 
 class TooFewGroupCharactersSpecials(TooFewGroupCharacters):
     __doc__ = _(
         'Password does not contain enough characters of special characters.')
 
     def __init__(self, minSpecials=None):
-        super(TooFewGroupCharactersSpecials, self).__init__()
+        super().__init__()
         self.minSpecials = minSpecials
         if minSpecials is not None:
             self.i18n_message = _(
                 'Password does not contain enough characters of special'
                 ' characters (should have at least ${minSpecials}).',
                 mapping=dict(minSpecials=minSpecials))
 
 
 class TooFewGroupCharactersOthers(TooFewGroupCharacters):
     __doc__ = _(
         '''Password does not contain enough characters of other characters.''')
 
     def __init__(self, minOthers=None):
-        super(TooFewGroupCharactersOthers, self).__init__()
+        super().__init__()
         self.minOthers = minOthers
         if minOthers is not None:
             self.i18n_message = _(
                 'Password does not contain enough characters of other'
                 ' characters (should have at least ${minOthers}).',
                 mapping=dict(minOthers=minOthers))
 
 
 class TooFewUniqueCharacters(InvalidPassword):
     __doc__ = _('''Password does not contain enough unique characters.''')
 
     def __init__(self, minUniqueCharacters=None):
-        super(TooFewUniqueCharacters, self).__init__()
+        super().__init__()
         self.minUniqueCharacters = minUniqueCharacters
         if minUniqueCharacters is not None:
             self.i18n_message = _(
                 'Password does not contain enough unique characters'
                 ' (should have at least ${minUniqueCharacters}).',
                 mapping=dict(minUniqueCharacters=minUniqueCharacters))
 
 
 class TooFewUniqueLetters(InvalidPassword):
     __doc__ = _('''Password does not contain enough unique letters.''')
 
     def __init__(self, minUniqueLetters=None):
-        super(TooFewUniqueLetters, self).__init__()
+        super().__init__()
         self.minUniqueLetters = minUniqueLetters
         if minUniqueLetters is not None:
             self.i18n_message = _(
                 'Password does not contain enough unique letters'
                 ' (should have at least ${minUniqueLetters}).',
                 mapping=dict(minUniqueLetters=minUniqueLetters))
 
@@ -236,16 +236,16 @@
 
     The purpose of this utility is to make common password-related tasks, such
     as verification and creation simple. However, only the collection of those
     utilites provide an overall net worth.
     """
 
     description = zope.schema.Text(
-        title=_(u'Description'),
-        description=_(u'A description of the password utility.'),
+        title=_('Description'),
+        description=_('A description of the password utility.'),
         required=False)
 
     def verify(new, ref=None):
         """Check whether the new password is valid.
 
         When a passward is good, the method simply returns, otherwise an
         ``InvalidPassword`` exception is raised.
@@ -267,207 +267,207 @@
         """
 
 
 class IHighSecurityPasswordUtility(IPasswordUtility):
     """A password utility for very secure passwords."""
 
     minLength = zope.schema.Int(
-        title=_(u'Minimum Length'),
-        description=_(u'The minimum length of the password.'),
+        title=_('Minimum Length'),
+        description=_('The minimum length of the password.'),
         required=False,
         default=None)
 
     maxLength = zope.schema.Int(
-        title=_(u'Maximum Length'),
-        description=_(u'The maximum length of the password.'),
+        title=_('Maximum Length'),
+        description=_('The maximum length of the password.'),
         required=False,
         default=None)
 
     @zope.interface.invariant
     def minMaxLength(task):
         if task.minLength is not None and task.maxLength is not None:
             if task.minLength > task.maxLength:
                 raise zope.interface.Invalid(
-                    u"Minimum length must not be greater than the maximum"
-                    u" length.")
+                    "Minimum length must not be greater than the maximum"
+                    " length.")
 
     groupMax = zope.schema.Int(
-        title=_(u'Maximum Characters of Group'),
-        description=_(u'The maximum amount of characters that a password can '
-                      u'have from one group. The groups are: digits, letters, '
-                      u'punctuation.'),
+        title=_('Maximum Characters of Group'),
+        description=_('The maximum amount of characters that a password can '
+                      'have from one group. The groups are: digits, letters, '
+                      'punctuation.'),
         required=False,
         default=None)
 
     maxSimilarity = zope.schema.Float(
-        title=_(u'Old/New Similarity'),
+        title=_('Old/New Similarity'),
         description=(
-            u'The similarity ratio between the new and old password.'),
+            'The similarity ratio between the new and old password.'),
         required=False,
         default=None)
 
     minLowerLetter = zope.schema.Int(
-        title=_(u'Minimum Number of Lowercase letters'),
-        description=_(u'The minimum amount of lowercase letters that a '
-                      u'password must have.'),
+        title=_('Minimum Number of Lowercase letters'),
+        description=_('The minimum amount of lowercase letters that a '
+                      'password must have.'),
         required=False,
         default=None)
 
     minUpperLetter = zope.schema.Int(
-        title=_(u'Minimum Number of Uppercase letters'),
-        description=_(u'The minimum amount of uppercase letters that a '
-                      u'password must have.'),
+        title=_('Minimum Number of Uppercase letters'),
+        description=_('The minimum amount of uppercase letters that a '
+                      'password must have.'),
         required=False,
         default=None)
 
     minDigits = zope.schema.Int(
-        title=_(u'Minimum Number of Numeric digits'),
-        description=_(u'The minimum amount of numeric digits that a '
-                      u'password must have.'),
+        title=_('Minimum Number of Numeric digits'),
+        description=_('The minimum amount of numeric digits that a '
+                      'password must have.'),
         required=False,
         default=None)
 
     minSpecials = zope.schema.Int(
-        title=_(u'Minimum Number of Special characters'),
-        description=_(u'The minimum amount of special characters that a '
-                      u'password must have.'),
+        title=_('Minimum Number of Special characters'),
+        description=_('The minimum amount of special characters that a '
+                      'password must have.'),
         required=False,
         default=None)
 
     # WARNING! generating a password with Others is not yet supported
     minOthers = zope.schema.Int(
-        title=_(u'Minimum Number of Other characters'),
-        description=_(u'The minimum amount of other characters that a '
-                      u'password must have.'),
+        title=_('Minimum Number of Other characters'),
+        description=_('The minimum amount of other characters that a '
+                      'password must have.'),
         required=False,
         default=None)
 
     @zope.interface.invariant
     def saneMinimums(task):
         minl = 0
         if task.minLowerLetter:
             if task.minLowerLetter > task.groupMax:
                 raise zope.interface.Invalid(
-                    u"Any group minimum length must NOT be greater than "
-                    u"the maximum group length.")
+                    "Any group minimum length must NOT be greater than "
+                    "the maximum group length.")
 
             minl += task.minLowerLetter
         if task.minUpperLetter:
             if task.minUpperLetter > task.groupMax:
                 raise zope.interface.Invalid(
-                    u"Any group minimum length must NOT be greater than "
-                    u"the maximum group length.")
+                    "Any group minimum length must NOT be greater than "
+                    "the maximum group length.")
 
             minl += task.minUpperLetter
         if task.minDigits:
             if task.minDigits > task.groupMax:
                 raise zope.interface.Invalid(
-                    u"Any group minimum length must NOT be greater than "
-                    u"the maximum group length.")
+                    "Any group minimum length must NOT be greater than "
+                    "the maximum group length.")
 
             minl += task.minDigits
         if task.minSpecials:
             if task.minSpecials > task.groupMax:
                 raise zope.interface.Invalid(
-                    u"Any group minimum length must NOT be greater than "
-                    u"the maximum group length.")
+                    "Any group minimum length must NOT be greater than "
+                    "the maximum group length.")
 
             minl += task.minSpecials
         if task.minOthers:
             if task.minOthers > task.groupMax:
                 raise zope.interface.Invalid(
-                    u"Any group minimum length must NOT be greater than "
-                    u"the maximum group length.")
+                    "Any group minimum length must NOT be greater than "
+                    "the maximum group length.")
 
             minl += task.minOthers
 
         if task.maxLength is not None:
             if minl > task.maxLength:
                 raise zope.interface.Invalid(
-                    u"Sum of group minimum lengths must NOT be greater than "
-                    u"the maximum password length.")
+                    "Sum of group minimum lengths must NOT be greater than "
+                    "the maximum password length.")
 
     minUniqueLetters = zope.schema.Int(
-        title=_(u'Minimum Number of Unique letters'),
-        description=_(u'The minimum amount of unique letters that a '
-                      u'password must have. This is against passwords '
-                      u'like `aAaA0000`. All characters taken lowercase.'),
+        title=_('Minimum Number of Unique letters'),
+        description=_('The minimum amount of unique letters that a '
+                      'password must have. This is against passwords '
+                      'like `aAaA0000`. All characters taken lowercase.'),
         required=False,
         default=None)
 
     @zope.interface.invariant
     def minUniqueLettersLength(task):
         if (task.minUniqueLetters is not None
                 and task.minUniqueLetters is not None):
             if task.minUniqueLetters > task.maxLength:
                 raise zope.interface.Invalid(
-                    u"Minimum unique letters number must not be greater than "
-                    u"the maximum length.")
+                    "Minimum unique letters number must not be greater than "
+                    "the maximum length.")
 
     minUniqueCharacters = zope.schema.Int(
-        title=_(u'Minimum Number of Unique characters'),
-        description=_(u'The minimum amount of unique characters that a '
-                      u'password must have. This is against passwords '
-                      u'like `aAaA0000`. All characters taken lowercase.'),
+        title=_('Minimum Number of Unique characters'),
+        description=_('The minimum amount of unique characters that a '
+                      'password must have. This is against passwords '
+                      'like `aAaA0000`. All characters taken lowercase.'),
         required=False,
         default=None)
 
     @zope.interface.invariant
     def minUniqueCharactersLength(task):
         if (task.minUniqueCharacters is not None
                 and task.minUniqueCharacters is not None):
             if task.minUniqueCharacters > task.maxLength:
                 raise zope.interface.Invalid(
-                    u"Minimum unique characters length must not be greater"
-                    u" than the maximum length.")
+                    "Minimum unique characters length must not be greater"
+                    " than the maximum length.")
 
 
 class IPasswordOptionsUtility(zope.interface.Interface):
     """Different general security options.
 
     The purpose of this utility is to make common password-related options
     available
     """
 
     changePasswordOnNextLogin = zope.schema.Bool(
-        title=_(u'Password must be changed on next login'),
-        description=_(u'Password must be changed on next login'),
+        title=_('Password must be changed on next login'),
+        description=_('Password must be changed on next login'),
         required=False,
         default=False)
 
     passwordExpiresAfter = zope.schema.Int(
-        title=_(u'Password expires after (days)'),
-        description=_(u'Password expires after (days)'),
+        title=_('Password expires after (days)'),
+        description=_('Password expires after (days)'),
         required=False,
         default=None)
 
     lockOutPeriod = zope.schema.Int(
-        title=_(u'Lockout period (minutes)'),
+        title=_('Lockout period (minutes)'),
         description=_(
-            u'Lockout the user after too many failed password entries'
-            u'for this many minutes. The user can try again after.'),
+            'Lockout the user after too many failed password entries'
+            'for this many minutes. The user can try again after.'),
         required=False,
         default=None)
 
     maxFailedAttempts = zope.schema.Int(
-        title=_(u'Max. number of failed password entries before account is'
-                u' locked'),
+        title=_('Max. number of failed password entries before account is'
+                ' locked'),
         description=_(
-            u'Specifies the amount of failed attempts allowed to check '
-            u'the password before the password is locked and no new '
-            u'password can be provided.'),
+            'Specifies the amount of failed attempts allowed to check '
+            'the password before the password is locked and no new '
+            'password can be provided.'),
         required=False,
         default=None)
 
     failedAttemptCheck = zope.schema.Choice(
-        title=_(u'Failed password check method'),
-        description=_(u'Failed password check method. '
+        title=_('Failed password check method'),
+        description=_('Failed password check method. '
                       'All requests, non-reqource requests, POST requests.'),
         required=False,
         values=[TML_CHECK_ALL, TML_CHECK_NONRESOURCE, TML_CHECK_POSTONLY],
         default=TML_CHECK_ALL)
 
     disallowPasswordReuse = zope.schema.Bool(
-        title=_(u'Disallow Password Reuse'),
-        description=_(u'Do not allow to set a previously set password again.'),
+        title=_('Disallow Password Reuse'),
+        description=_('Do not allow to set a previously set password again.'),
         required=False,
         default=False)
```

### Comparing `z3c.password-1.1.0/src/z3c/password/locales/de/LC_MESSAGES/z3c.password.po` & `z3c.password-2.0/src/z3c/password/locales/de/LC_MESSAGES/z3c.password.po`

 * *Files identical despite different names*

### Comparing `z3c.password-1.1.0/src/z3c/password/locales/nl/LC_MESSAGES/z3c.password.po` & `z3c.password-2.0/src/z3c/password/locales/nl/LC_MESSAGES/z3c.password.po`

 * *Files identical despite different names*

### Comparing `z3c.password-1.1.0/src/z3c/password/locales/ru/LC_MESSAGES/z3c.password.po` & `z3c.password-2.0/src/z3c/password/locales/ru/LC_MESSAGES/z3c.password.po`

 * *Files identical despite different names*

### Comparing `z3c.password-1.1.0/src/z3c/password/locales/z3c.password.pot` & `z3c.password-2.0/src/z3c/password/locales/z3c.password.pot`

 * *Files identical despite different names*

### Comparing `z3c.password-1.1.0/src/z3c/password/password.py` & `z3c.password-2.0/src/z3c/password/password.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,38 +13,39 @@
 ##############################################################################
 """Password Utility Implementation
 """
 import difflib
 import random
 import string
 import time
+
 import zope.interface
 from zope.schema.fieldproperty import FieldProperty
 
 from z3c.password import interfaces
 
 
 @zope.interface.implementer(interfaces.IPasswordUtility)
-class TrivialPasswordUtility(object):
+class TrivialPasswordUtility:
     """A trivial password utility."""
 
-    description = (u'All passwords are accepted and always the "trivial" '
-                   u'password is generated.')
+    description = ('All passwords are accepted and always the "trivial" '
+                   'password is generated.')
 
     def verify(self, new, ref=None):
         '''See interfaces.IPasswordUtility'''
         return
 
     def generate(self, ref=None):
         '''See interfaces.IPasswordUtility'''
         return 'trivial'
 
 
 @zope.interface.implementer(interfaces.IHighSecurityPasswordUtility)
-class HighSecurityPasswordUtility(object):
+class HighSecurityPasswordUtility:
     """An implementation of the high-security password API."""
 
     minLength = FieldProperty(
         interfaces.IHighSecurityPasswordUtility['minLength'])
     maxLength = FieldProperty(
         interfaces.IHighSecurityPasswordUtility['maxLength'])
     groupMax = FieldProperty(
@@ -67,17 +68,17 @@
         interfaces.IHighSecurityPasswordUtility['minUniqueLetters'])
 
     LOWERLETTERS = string.ascii_letters[:26]
     UPPERLETTERS = string.ascii_letters[26:]
     DIGITS = string.digits
     SPECIALS = string.punctuation
 
-    description = (u'Passwords generated and verified by this utility conform '
-                   u'strictly to the specified parameters. See the interface '
-                   u'for more details.')
+    description = ('Passwords generated and verified by this utility conform '
+                   'strictly to the specified parameters. See the interface '
+                   'for more details.')
 
     def __init__(self, minLength=8, maxLength=12, groupMax=6,
                  maxSimilarity=0.6, seed=None,
                  minLowerLetter=None, minUpperLetter=None, minDigits=None,
                  minSpecials=None, minOthers=None,
                  minUniqueCharacters=None, minUniqueLetters=None):
         self.minLength = minLength
@@ -202,15 +203,15 @@
                 verified = False
             else:
                 verified = True
         return new
 
 
 @zope.interface.implementer(interfaces.IPasswordOptionsUtility)
-class PasswordOptionsUtility(object):
+class PasswordOptionsUtility:
     """An implementation of the security options."""
 
     changePasswordOnNextLogin = FieldProperty(
         interfaces.IPasswordOptionsUtility['changePasswordOnNextLogin'])
     passwordExpiresAfter = FieldProperty(
         interfaces.IPasswordOptionsUtility['passwordExpiresAfter'])
     lockOutPeriod = FieldProperty(
```

### Comparing `z3c.password-1.1.0/src/z3c/password/principal.py` & `z3c.password-2.0/src/z3c/password/principal.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Principal MixIn for Advanced Password Management
 """
 import datetime
+
 import persistent.list
 import zope.component
 from zope.security.management import getInteraction
 
 from z3c.password import interfaces
 
 
-class PrincipalMixIn(object):
+class PrincipalMixIn:
     """A Principal Mixin class for ``zope.app.principalfolder``'s internal
     principal."""
 
     passwordExpiresAfter = None
     passwordSetOn = None
     # force PasswordExpired, e.g. for changePasswordOnNextLogin
     passwordExpired = False
@@ -49,20 +50,20 @@
                 passwordManager = self._getPasswordManager()
 
                 for pwd in self.previousPasswords:
                     if passwordManager.checkPassword(pwd, password):
                         raise interfaces.PreviousPasswordNotAllowed(self)
 
     def getPassword(self):
-        return super(PrincipalMixIn, self).getPassword()
+        return super().getPassword()
 
     def setPassword(self, password, passwordManagerName=None):
         self._checkDisallowedPreviousPassword(password)
 
-        super(PrincipalMixIn, self).setPassword(password, passwordManagerName)
+        super().setPassword(password, passwordManagerName)
 
         if self._disallowPasswordReuse():
             if self.previousPasswords is None:
                 self.previousPasswords = persistent.list.PersistentList()
 
             if self.password is not None:
                 # storm/custom property does not like a simple append
@@ -106,15 +107,15 @@
             return False
 
     def checkPassword(self, pwd, ignoreExpiration=False, ignoreFailures=False):
         # keep this as fast as possible, because it will be called (usually)
         # for EACH request
 
         # Check the password
-        same = super(PrincipalMixIn, self).checkPassword(pwd)
+        same = super().checkPassword(pwd)
 
         # Do not try to record failed attempts or raise account locked
         # errors for requests that are irrelevant in this regard.
         if not self._isRelevantRequest():
             return same
 
         if not ignoreFailures and self.lastFailedAttempt is not None:
```

### Comparing `z3c.password-1.1.0/src/z3c/password/principal.txt` & `z3c.password-2.0/src/z3c/password/principal.txt`

 * *Files identical despite different names*

### Comparing `z3c.password-1.1.0/src/z3c/password/testing.py` & `z3c.password-2.0/src/z3c/password/testing.py`

 * *Files identical despite different names*

### Comparing `z3c.password-1.1.0/src/z3c/password/tests.py` & `z3c.password-2.0/src/z3c/password/tests.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,42 +10,25 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Test Setup
 """
 import doctest
-import re
 import unittest
 from doctest import DocFileSuite
-from zope.testing import renormalizing
 
 from z3c.password import testing
 
-checker = renormalizing.RENormalizing([
-    # Python 3 bytes add a "b".
-    (re.compile("b('.*?')"),
-     r"\1"),
-    (re.compile('b(".*?")'),
-     r"\1"),
-    # Python 3 adds module name to exceptions.
-    (re.compile("z3c.password.interfaces.NoPassword"),
-     r"NoPassword"),
-    (re.compile("zope.security.interfaces.NoInteraction"),
-     r"NoInteraction"),
-])
-
 
 def test_suite():
     flags = doctest.NORMALIZE_WHITESPACE |\
         doctest.ELLIPSIS |\
         doctest.IGNORE_EXCEPTION_DETAIL
     return unittest.TestSuite((
         DocFileSuite('README.txt',
                      setUp=testing.setUp, tearDown=testing.tearDown,
-                     optionflags=flags, checker=checker,
-                     ),
+                     optionflags=flags),
         DocFileSuite('principal.txt',
                      setUp=testing.setUp, tearDown=testing.tearDown,
-                     optionflags=flags, checker=checker,
-                     ),
+                     optionflags=flags),
     ))
```

### Comparing `z3c.password-1.1.0/src/z3c.password.egg-info/PKG-INFO` & `z3c.password-2.0/src/z3c.password.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 Metadata-Version: 2.1
 Name: z3c.password
-Version: 1.1.0
+Version: 2.0
 Summary: Password generation and verification utility for Zope3
 Home-page: http://pypi.org/project/z3c.password
 Author: Stephan Richter, Roger Ineichen and the Zope Community
-Author-email: zope3-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: zope3 z3c password verification
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
-Provides-Extra: test
+Requires-Python: >=3.7
 License-File: LICENSE.txt
+Requires-Dist: setuptools
+Requires-Dist: zope.component
+Requires-Dist: zope.exceptions
+Requires-Dist: zope.i18nmessageid
+Requires-Dist: zope.i18n
+Requires-Dist: zope.interface
+Requires-Dist: zope.schema
+Requires-Dist: zope.security
+Provides-Extra: test
+Requires-Dist: z3c.coverage; extra == "test"
+Requires-Dist: zope.password; extra == "test"
+Requires-Dist: zope.pluggableauth; extra == "test"
+Requires-Dist: zope.testing; extra == "test"
 
 ============
 z3c.password
 ============
 
 
 .. image:: https://github.com/zopefoundation/z3c.password/actions/workflows/tests.yml/badge.svg
@@ -54,14 +64,25 @@
 offers a field and a property for those fields.
 
 
 =======
 CHANGES
 =======
 
+2.0 (2024-05-21)
+----------------
+
+- Add support for Python 3.11, 3.12.
+
+- Compile ``*.mo`` files at release time instead of including them in the
+  repository.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 1.1.0 (2021-12-14)
 ------------------
 
 - Add support for Python 3.8, 3.9 and 3.10.
 
 - Drop support for Python 3.4.
 
@@ -228,9 +249,7 @@
   to change it's password. This should not happen if the user did not enter a
   valid password.
 
 0.5.0 (2008-10-21)
 ------------------
 
 - Initial Release
-
-
```

### Comparing `z3c.password-1.1.0/src/z3c.password.egg-info/SOURCES.txt` & `z3c.password-2.0/src/z3c.password.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 tox.ini
@@ -13,21 +14,23 @@
 src/z3c.password.egg-info/namespace_packages.txt
 src/z3c.password.egg-info/not-zip-safe
 src/z3c.password.egg-info/requires.txt
 src/z3c.password.egg-info/top_level.txt
 src/z3c/password/DEPENDENCIES.txt
 src/z3c/password/README.txt
 src/z3c/password/__init__.py
-src/z3c/password/_compat.py
 src/z3c/password/configure.zcml
 src/z3c/password/field.py
 src/z3c/password/interfaces.py
 src/z3c/password/password.py
 src/z3c/password/principal.py
 src/z3c/password/principal.txt
 src/z3c/password/testing.py
 src/z3c/password/tests.py
 src/z3c/password/z3c.password-configure.zcml
 src/z3c/password/locales/z3c.password.pot
+src/z3c/password/locales/de/LC_MESSAGES/z3c.password.mo
 src/z3c/password/locales/de/LC_MESSAGES/z3c.password.po
+src/z3c/password/locales/nl/LC_MESSAGES/z3c.password.mo
 src/z3c/password/locales/nl/LC_MESSAGES/z3c.password.po
+src/z3c/password/locales/ru/LC_MESSAGES/z3c.password.mo
 src/z3c/password/locales/ru/LC_MESSAGES/z3c.password.po
```

### Comparing `z3c.password-1.1.0/tox.ini` & `z3c.password-2.0/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,92 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
+    release-check
     lint
-    py27
-    py35
-    py36
     py37
     py38
     py39
     py310
-    pypy
+    py311
+    py312
     pypy3
     coverage
 
 [testenv]
 usedevelop = true
+package = wheel
+wheel_build_env = .pkg
 deps =
     zope.testrunner
+setenv =
+    py312: VIRTUALENV_PIP=23.1.2
+    py312: PIP_REQUIRE_VIRTUALENV=0
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
 extras =
     test
+[testenv:release-check]
+description = ensure that the distribution is ready to release
+basepython = python3
+skip_install = true
+deps =
+    twine
+    build
+    check-manifest
+    check-python-versions >= 0.20.0
+    wheel
+commands_pre =
+commands =
+    check-manifest
+    check-python-versions --only setup.py,tox.ini,.github/workflows/tests.yml
+    python -m build --sdist --no-isolation
+    twine check dist/*
 
 [testenv:lint]
 basepython = python3
 skip_install = true
 deps =
+    isort
     flake8
-    check-manifest
-    check-python-versions >= 0.19.1
-    wheel
 commands =
+    isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
     flake8 src setup.py
-    check-manifest
-    check-python-versions
+
+[testenv:isort-apply]
+basepython = python3
+skip_install = true
+commands_pre =
+deps =
+    isort
+commands =
+    isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
     zope.testrunner
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
-    coverage html
-    coverage report -m --fail-under=86
+    coverage html --ignore-errors
+    coverage report --show-missing --fail-under=86
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = z3c.password
 
 [coverage:report]
 precision = 2
+ignore_errors = True
 exclude_lines =
     pragma: no cover
     pragma: nocover
     except ImportError:
     raise NotImplementedError
     if __name__ == '__main__':
     self.fail
```

