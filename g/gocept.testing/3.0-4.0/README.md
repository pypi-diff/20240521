# Comparing `tmp/gocept.testing-3.0.tar.gz` & `tmp/gocept.testing-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gocept.testing-3.0.tar", last modified: Thu Aug 26 06:27:05 2021, max compression
+gzip compressed data, was "gocept.testing-4.0.tar", last modified: Tue May 21 13:02:51 2024, max compression
```

## Comparing `gocept.testing-3.0.tar` & `gocept.testing-4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-08-26 06:27:05.000000 gocept.testing-3.0/
--rw-r--r--   0 mac        (513) staff       (20)      305 2021-08-26 06:27:04.000000 gocept.testing-3.0/.coveragerc
--rw-r--r--   0 mac        (513) staff       (20)     1089 2021-08-26 06:27:04.000000 gocept.testing-3.0/.pre-commit-config.yaml
--rw-r--r--   0 mac        (513) staff       (20)     2814 2021-08-26 06:27:04.000000 gocept.testing-3.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)     1068 2021-08-26 06:27:04.000000 gocept.testing-3.0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      125 2021-08-26 06:27:04.000000 gocept.testing-3.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)    14275 2021-08-26 06:27:05.000000 gocept.testing-3.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     6755 2021-08-26 06:27:04.000000 gocept.testing-3.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)       23 2021-08-26 06:27:04.000000 gocept.testing-3.0/pytest.ini
--rw-r--r--   0 mac        (513) staff       (20)      213 2021-08-26 06:27:05.000000 gocept.testing-3.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     1888 2021-08-26 06:27:04.000000 gocept.testing-3.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-08-26 06:27:05.000000 gocept.testing-3.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-08-26 06:27:05.000000 gocept.testing-3.0/src/gocept/
--rw-r--r--   0 mac        (513) staff       (20)       76 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-08-26 06:27:05.000000 gocept.testing-3.0/src/gocept/testing/
--rw-r--r--   0 mac        (513) staff       (20)       17 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept/testing/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     2680 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept/testing/assertion.py
--rw-r--r--   0 mac        (513) staff       (20)      260 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept/testing/fixture.py
--rw-r--r--   0 mac        (513) staff       (20)     1038 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept/testing/mock.py
--rw-r--r--   0 mac        (513) staff       (20)     1733 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept/testing/mtime.py
--rw-r--r--   0 mac        (513) staff       (20)     1192 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept/testing/patch.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-08-26 06:27:05.000000 gocept.testing-3.0/src/gocept/testing/tests/
--rw-r--r--   0 mac        (513) staff       (20)     4210 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept/testing/tests/test_assertion.py
--rw-r--r--   0 mac        (513) staff       (20)      688 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept/testing/tests/test_fixture.py
--rw-r--r--   0 mac        (513) staff       (20)     4096 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept/testing/tests/test_mock.py
--rw-r--r--   0 mac        (513) staff       (20)     1480 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept/testing/tests/test_mtime.py
--rw-r--r--   0 mac        (513) staff       (20)     2877 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept/testing/tests/test_patch.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-08-26 06:27:05.000000 gocept.testing-3.0/src/gocept.testing.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)    14275 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept.testing.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      820 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept.testing.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept.testing.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        7 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept.testing.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept.testing.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)       11 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept.testing.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        7 2021-08-26 06:27:04.000000 gocept.testing-3.0/src/gocept.testing.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)      356 2021-08-26 06:27:04.000000 gocept.testing-3.0/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 13:02:51.510400 gocept.testing-4.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      255 2024-05-21 13:02:51.000000 gocept.testing-4.0/.coveragerc
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1069 2024-05-21 13:02:51.000000 gocept.testing-4.0/.pre-commit-config.yaml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3030 2024-05-21 13:02:51.000000 gocept.testing-4.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1100 2024-05-21 13:02:51.000000 gocept.testing-4.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      125 2024-05-21 13:02:51.000000 gocept.testing-4.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11346 2024-05-21 13:02:51.510250 gocept.testing-4.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6784 2024-05-21 13:02:51.000000 gocept.testing-4.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       23 2024-05-21 13:02:51.000000 gocept.testing-4.0/pytest.ini
+-rw-r--r--   0 m.howitz   (502) staff       (20)      213 2024-05-21 13:02:51.510652 gocept.testing-4.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1906 2024-05-21 13:02:51.000000 gocept.testing-4.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 13:02:51.505111 gocept.testing-4.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 13:02:51.506908 gocept.testing-4.0/src/gocept/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 13:02:51.508826 gocept.testing-4.0/src/gocept/testing/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       17 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept/testing/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2633 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept/testing/assertion.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      260 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept/testing/fixture.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1038 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept/testing/mock.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1733 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept/testing/mtime.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1192 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept/testing/patch.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 13:02:51.509659 gocept.testing-4.0/src/gocept/testing/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4210 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept/testing/tests/test_assertion.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      688 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept/testing/tests/test_fixture.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4096 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept/testing/tests/test_mock.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1480 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept/testing/tests/test_mtime.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2877 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept/testing/tests/test_patch.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-21 13:02:51.509969 gocept.testing-4.0/src/gocept.testing.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11346 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept.testing.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      820 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept.testing.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept.testing.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        7 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept.testing.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept.testing.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)       11 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept.testing.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        7 2024-05-21 13:02:51.000000 gocept.testing-4.0/src/gocept.testing.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      341 2024-05-21 13:02:51.000000 gocept.testing-4.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gocept.testing-3.0/CHANGES.rst` & `gocept.testing-4.0/CHANGES.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 Changelog
 =========
 
+4.0 (2024-05-21)
+----------------
+
+Backwards incompatible changes
+++++++++++++++++++++++++++++++
+
+- Drop support for Python 3.7, 3.8.
+
+Features
+++++++++
+
+- Add support for Python 3.11, 3.12 and 3.13 (as of beta 1).
+
+
 3.0 (2021-08-26)
 ----------------
 
 Backwards incompatible changes
 ++++++++++++++++++++++++++++++
 
 - Change license form ZPL to MIT.
 
 - Drop support for Python 2, 3.4, 3.5 and 3.6
 
 Features
 ++++++++
 
-- Add support for Python 3.8, 3.9 and 3.10 (as of rc.1).
+- Add support for Python 3.8, 3.9 and 3.10 (as of rc.1).
 
 
 2.0.post1 (2018-11-22)
 ----------------------
 
 - Fix PyPI page rendering.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gocept.testing-3.0/LICENSE.txt` & `gocept.testing-4.0/LICENSE.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 Copyright (c) 2011-2021 gocept gmbh & co. kg
+Copyright (c) 2024 Minddistrict
 Permission is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy, modify, merge,
 publish, distribute, sublicense, and/or sell copies of the Software, and to permit
 persons to whom the Software is furnished to do so, subject to the following
 conditions:
```

### Comparing `gocept.testing-3.0/README.rst` & `gocept.testing-4.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 ==============
 gocept.testing
 ==============
 
-.. image:: https://github.com/gocept/gocept.testing/workflows/tests/badge.svg
-    :target: https://github.com/gocept/gocept.testing/actions?query=workflow%3Atests
+.. image:: https://github.com/minddistrict/gocept.testing/workflows/tests/badge.svg
+    :target: https://github.com/minddistrict/gocept.testing/actions?query=workflow%3Atests
 
-.. image:: https://coveralls.io/repos/github/gocept/gocept.testing/badge.svg
-    :target: https://coveralls.io/github/gocept/gocept.testing
+.. image:: https://coveralls.io/repos/github/minddistrict/gocept.testing/badge.svg
+    :target: https://coveralls.io/github/minddistrict/gocept.testing
 
 
 This package collects various helpers for writing tests.
 
-.. contents:: :depth: 1
+.. contents::
 
 
 assertEllipsis
 ==============
 
 An assertion which is very helpful when using Testbrowser with
-unittest.TestCase (instead of doctests).
+``unittest.TestCase`` (instead of ``doctest``).
 
 Some examples::
 
     class MyTest(unittest.TestCase, gocept.testing.assertion.Ellipsis):
     # [...]
 
 
@@ -71,15 +71,15 @@
 
 
 mock patch context
 ==================
 
 ``gocept.testing.mock.Patches`` collects `mock`_ patches that are valid for the
 whole TestCase, and resets them all in one go in tearDown (this is pending
-incluion upstream as ``mock.patcher()``, see `issue 30`_)::
+inclusion upstream as ``mock.patcher()``, see `issue 30`_)::
 
     class MyTest(unittest.TestCase):
 
         def setUp(self):
             self.patches = gocept.testing.mock.Patches()
 
         def tearDown(self):
@@ -94,15 +94,15 @@
 :add_object: wraps ``mock.patch.object``
 :add_dict: wraps ``mock.patch.dict``
 
 Note that ``gocept.testing`` does not declare a dependency on ``mock`` to be as
 lightweight as possible, so clients need to do that themselves.
 
 If you want to save typing, you can mix ``gocept.testing.mock.PatchHelper``
-into your TestCase, it defines a setUp method that instatiates ``Patches`` and
+into your TestCase, it defines a setUp method that instantiates ``Patches`` and
 a tearDown that calls ``reset()`` on it.
 
 
 .. _`mock`: http://www.voidspace.org.uk/python/mock/
 .. _`issue 30`: http://code.google.com/p/mock/issues/detail?id=30
 
 
@@ -231,8 +231,8 @@
                 'my.package', 'resources/js'))
 
 
 Development
 ===========
 
 The git repository of the source code as well as the issue tracker are
-available at https://github.com/gocept/gocept.testing.
+available at https://github.com/minddistrict/gocept.testing.
```

### Comparing `gocept.testing-3.0/setup.py` & `gocept.testing-4.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
 setup(
     name='gocept.testing',
-    version='3.0',
-    author='gocept <mail at gocept dot com>',
-    author_email='mail@gocept.com',
-    url='https://github.com/gocept/gocept.testing',
+    version='4.0',
+    author='minddistrict <mail at minddistrict dot com>',
+    author_email='mail@minddistrict.com',
+    url='https://github.com/minddistrict/gocept.testing',
     description="""\
 A collection of test helpers, additional assertions, and the like.""",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'Programming Language :: Python :: 3.13',
         'Programming Language :: Python :: Implementation',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Application Frameworks',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Software Development :: Testing',
     ],
-    long_description=(
-        open('README.rst').read()
-        + '\n\n'
-        + open('CHANGES.rst').read()),
+    long_description=(open('README.rst').read() + '\n\n' +
+                      open('CHANGES.rst').read()),
     packages=find_packages('src'),
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
     license='MIT',
     keywords="testing unittest assertions",
     namespace_packages=['gocept'],
-    python_requires='>=3.7',
+    python_requires='>=3.9',
     install_requires=[
         'setuptools',
     ],
 )
```

### Comparing `gocept.testing-3.0/src/gocept/testing/assertion.py` & `gocept.testing-4.0/src/gocept/testing/assertion.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,32 +18,31 @@
     norm_actual = ' '.join(actual.split())
     return doctest._ellipsis_match(norm_expected, norm_actual)
 
 
 class Ellipsis:
     """Assertion helper that provides doctest-style ellipsis matching.
 
-    Inherit from this class in additition to unittest.TestCase.
+    Inherit from this class in addition to unittest.TestCase.
     """
 
     def assertEllipsis(self, expected, actual):
         if ellipsis_match(expected, actual):
             return True
         # report ndiff
         engine = difflib.Differ(charjunk=difflib.IS_CHARACTER_JUNK)
-        diff = list(engine.compare(expected.splitlines(True),
-                                   actual.splitlines(True)))
+        diff = list(
+            engine.compare(expected.splitlines(True), actual.splitlines(True)))
         kind = 'ndiff with -expected +actual'
         diff = [line.rstrip() + '\n' for line in diff]
         self.fail('Differences (%s):\n' % kind + ''.join(diff))
 
     def assertNotEllipsis(self, expected, actual):
         if ellipsis_match(expected, actual):
-            self.fail(
-                'Value unexpectedly matches expression %r.' % expected)
+            self.fail('Value unexpectedly matches expression %r.' % expected)
 
 
 class Exceptions:
 
     def assertNothingRaised(self, callable=None, *args, **kw):
         context = AssertNothingRaisedContext(self)
         if callable is None:
@@ -60,17 +59,16 @@
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, tb):
         if exc_type is None:
             return True
         exc_name = exc_type.__name__
-        message = (
-            'Unexpectedly raised %s, original traceback follows:\n'
-            % exc_name)
+        message = ('Unexpectedly raised %s, original traceback follows:\n' %
+                   exc_name)
         # cut off "Traceback: (most recent call last)" and the original
         #  message, since we're printing that ourselves
         stack = ''.join(
             traceback.format_exception(exc_type, exc_value, tb)[1:-1])
         text = message + stack + f'Unexpected {exc_name}: {exc_value}'
         raise self.failureException(text)
```

### Comparing `gocept.testing-3.0/src/gocept/testing/mock.py` & `gocept.testing-4.0/src/gocept/testing/mock.py`

 * *Files identical despite different names*

### Comparing `gocept.testing-3.0/src/gocept/testing/mtime.py` & `gocept.testing-4.0/src/gocept/testing/mtime.py`

 * *Files identical despite different names*

### Comparing `gocept.testing-3.0/src/gocept/testing/patch.py` & `gocept.testing-4.0/src/gocept/testing/patch.py`

 * *Files identical despite different names*

### Comparing `gocept.testing-3.0/src/gocept/testing/tests/test_assertion.py` & `gocept.testing-4.0/src/gocept/testing/tests/test_assertion.py`

 * *Files identical despite different names*

### Comparing `gocept.testing-3.0/src/gocept/testing/tests/test_fixture.py` & `gocept.testing-4.0/src/gocept/testing/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `gocept.testing-3.0/src/gocept/testing/tests/test_mock.py` & `gocept.testing-4.0/src/gocept/testing/tests/test_mock.py`

 * *Files identical despite different names*

### Comparing `gocept.testing-3.0/src/gocept/testing/tests/test_mtime.py` & `gocept.testing-4.0/src/gocept/testing/tests/test_mtime.py`

 * *Files identical despite different names*

### Comparing `gocept.testing-3.0/src/gocept/testing/tests/test_patch.py` & `gocept.testing-4.0/src/gocept/testing/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `gocept.testing-3.0/src/gocept.testing.egg-info/SOURCES.txt` & `gocept.testing-4.0/src/gocept.testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

