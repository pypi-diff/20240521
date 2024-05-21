# Comparing `tmp/testcontainers-iris-1.1.1b1.tar.gz` & `tmp/testcontainers_iris-1.1.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testcontainers-iris-1.1.1b1.tar", last modified: Thu Dec 14 13:37:17 2023, max compression
+gzip compressed data, was "testcontainers_iris-1.1.1b2.tar", last modified: Tue May 21 01:19:48 2024, max compression
```

## Comparing `testcontainers-iris-1.1.1b1.tar` & `testcontainers_iris-1.1.1b2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:37:17.462778 testcontainers-iris-1.1.1b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-12-14 13:36:21.000000 testcontainers-iris-1.1.1b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-12-14 13:37:17.462778 testcontainers-iris-1.1.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2023-12-14 13:36:21.000000 testcontainers-iris-1.1.1b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-12-14 13:37:17.462778 testcontainers-iris-1.1.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-12-14 13:36:21.000000 testcontainers-iris-1.1.1b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:37:17.458778 testcontainers-iris-1.1.1b1/testcontainers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:37:17.462778 testcontainers-iris-1.1.1b1/testcontainers/iris/
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2023-12-14 13:36:21.000000 testcontainers-iris-1.1.1b1/testcontainers/iris/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:37:17.462778 testcontainers-iris-1.1.1b1/testcontainers_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-12-14 13:37:17.000000 testcontainers-iris-1.1.1b1/testcontainers_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-14 13:37:17.000000 testcontainers-iris-1.1.1b1/testcontainers_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 13:37:17.000000 testcontainers-iris-1.1.1b1/testcontainers_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-14 13:37:17.000000 testcontainers-iris-1.1.1b1/testcontainers_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-14 13:37:17.000000 testcontainers-iris-1.1.1b1/testcontainers_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:37:17.462778 testcontainers-iris-1.1.1b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-12-14 13:36:21.000000 testcontainers-iris-1.1.1b1/tests/test_iris.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:19:48.876158 testcontainers_iris-1.1.1b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-21 01:18:55.000000 testcontainers_iris-1.1.1b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-21 01:19:48.876158 testcontainers_iris-1.1.1b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-21 01:18:55.000000 testcontainers_iris-1.1.1b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-21 01:19:48.876158 testcontainers_iris-1.1.1b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-21 01:18:55.000000 testcontainers_iris-1.1.1b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:19:48.876158 testcontainers_iris-1.1.1b2/testcontainers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:19:48.876158 testcontainers_iris-1.1.1b2/testcontainers/iris/
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-21 01:18:55.000000 testcontainers_iris-1.1.1b2/testcontainers/iris/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:19:48.876158 testcontainers_iris-1.1.1b2/testcontainers_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-21 01:19:48.000000 testcontainers_iris-1.1.1b2/testcontainers_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-21 01:19:48.000000 testcontainers_iris-1.1.1b2/testcontainers_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 01:19:48.000000 testcontainers_iris-1.1.1b2/testcontainers_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 01:19:48.000000 testcontainers_iris-1.1.1b2/testcontainers_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 01:19:48.000000 testcontainers_iris-1.1.1b2/testcontainers_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:19:48.876158 testcontainers_iris-1.1.1b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-21 01:18:55.000000 testcontainers_iris-1.1.1b2/tests/test_iris.py
```

### Comparing `testcontainers-iris-1.1.1b1/LICENSE` & `testcontainers_iris-1.1.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `testcontainers-iris-1.1.1b1/PKG-INFO` & `testcontainers_iris-1.1.1b2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: testcontainers-iris
-Version: 1.1.1b1
+Version: 1.1.1b2
 Summary: InterSystems IRIS component of testcontainers-python.
 Home-page: https://github.com/caretdev/testcontainers-iris-python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: testcontainers-core
 Requires-Dist: sqlalchemy
 Requires-Dist: sqlalchemy-iris
+Requires-Dist: requests<2.32.0
 
 # Testcontainers-python for InterSystems IRIS
 
 [testcontainers-python](https://testcontainers-python.readthedocs.io/en/latest/README.html) facilitates the use of Docker containers for functional and integration testing.
 
 ## Other implementations
 
@@ -47,8 +48,10 @@
     namespace="TEST",
 )
 
 ```
 
 `username`, `password`, `namespace` will be created during start of the container with required values, user will get %All role
 
+[Demo](iris.ipynb) with Jupiter Notebook 
+
 More extensive documentation can be found at [Read The Docs](https://testcontainers-python.readthedocs.io/).
```

### Comparing `testcontainers-iris-1.1.1b1/README.md` & `testcontainers_iris-1.1.1b2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -35,8 +35,10 @@
     namespace="TEST",
 )
 
 ```
 
 `username`, `password`, `namespace` will be created during start of the container with required values, user will get %All role
 
+[Demo](iris.ipynb) with Jupiter Notebook 
+
 More extensive documentation can be found at [Read The Docs](https://testcontainers-python.readthedocs.io/).
```

### Comparing `testcontainers-iris-1.1.1b1/testcontainers/iris/__init__.py` & `testcontainers_iris-1.1.1b2/testcontainers/iris/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-iris-1.1.1b1/testcontainers_iris.egg-info/PKG-INFO` & `testcontainers_iris-1.1.1b2/testcontainers_iris.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: testcontainers-iris
-Version: 1.1.1b1
+Version: 1.1.1b2
 Summary: InterSystems IRIS component of testcontainers-python.
 Home-page: https://github.com/caretdev/testcontainers-iris-python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: testcontainers-core
 Requires-Dist: sqlalchemy
 Requires-Dist: sqlalchemy-iris
+Requires-Dist: requests<2.32.0
 
 # Testcontainers-python for InterSystems IRIS
 
 [testcontainers-python](https://testcontainers-python.readthedocs.io/en/latest/README.html) facilitates the use of Docker containers for functional and integration testing.
 
 ## Other implementations
 
@@ -47,8 +48,10 @@
     namespace="TEST",
 )
 
 ```
 
 `username`, `password`, `namespace` will be created during start of the container with required values, user will get %All role
 
+[Demo](iris.ipynb) with Jupiter Notebook 
+
 More extensive documentation can be found at [Read The Docs](https://testcontainers-python.readthedocs.io/).
```

### Comparing `testcontainers-iris-1.1.1b1/tests/test_iris.py` & `testcontainers_iris-1.1.1b2/tests/test_iris.py`

 * *Files identical despite different names*

