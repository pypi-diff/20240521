# Comparing `tmp/pytest_django_docker_pg-0.0.2.tar.gz` & `tmp/pytest_django_docker_pg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_django_docker_pg-0.0.2.tar", last modified: Tue Jan 30 14:46:14 2024, max compression
+gzip compressed data, was "pytest_django_docker_pg-0.0.3.tar", last modified: Tue May 21 09:29:57 2024, max compression
```

## Comparing `pytest_django_docker_pg-0.0.2.tar` & `pytest_django_docker_pg-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:46:14.636087 pytest_django_docker_pg-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-30 14:46:02.000000 pytest_django_docker_pg-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-01-30 14:46:14.636087 pytest_django_docker_pg-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-01-30 14:46:02.000000 pytest_django_docker_pg-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-01-30 14:46:02.000000 pytest_django_docker_pg-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:46:14.636087 pytest_django_docker_pg-0.0.2/pytest_django_docker_pg/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-30 14:46:02.000000 pytest_django_docker_pg-0.0.2/pytest_django_docker_pg/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 14:46:02.000000 pytest_django_docker_pg-0.0.2/pytest_django_docker_pg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-01-30 14:46:02.000000 pytest_django_docker_pg-0.0.2/pytest_django_docker_pg/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:46:14.636087 pytest_django_docker_pg-0.0.2/pytest_django_docker_pg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-01-30 14:46:14.000000 pytest_django_docker_pg-0.0.2/pytest_django_docker_pg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-30 14:46:14.000000 pytest_django_docker_pg-0.0.2/pytest_django_docker_pg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 14:46:14.000000 pytest_django_docker_pg-0.0.2/pytest_django_docker_pg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-30 14:46:14.000000 pytest_django_docker_pg-0.0.2/pytest_django_docker_pg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-30 14:46:14.000000 pytest_django_docker_pg-0.0.2/pytest_django_docker_pg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-30 14:46:14.000000 pytest_django_docker_pg-0.0.2/pytest_django_docker_pg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 14:46:14.636087 pytest_django_docker_pg-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 14:46:14.636087 pytest_django_docker_pg-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-01-30 14:46:02.000000 pytest_django_docker_pg-0.0.2/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:29:57.386236 pytest_django_docker_pg-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-21 09:29:49.000000 pytest_django_docker_pg-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-21 09:29:57.386236 pytest_django_docker_pg-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-21 09:29:49.000000 pytest_django_docker_pg-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-21 09:29:49.000000 pytest_django_docker_pg-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:29:57.386236 pytest_django_docker_pg-0.0.3/pytest_django_docker_pg/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 09:29:49.000000 pytest_django_docker_pg-0.0.3/pytest_django_docker_pg/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:29:49.000000 pytest_django_docker_pg-0.0.3/pytest_django_docker_pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-21 09:29:49.000000 pytest_django_docker_pg-0.0.3/pytest_django_docker_pg/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:29:57.386236 pytest_django_docker_pg-0.0.3/pytest_django_docker_pg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-21 09:29:57.000000 pytest_django_docker_pg-0.0.3/pytest_django_docker_pg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-21 09:29:57.000000 pytest_django_docker_pg-0.0.3/pytest_django_docker_pg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:29:57.000000 pytest_django_docker_pg-0.0.3/pytest_django_docker_pg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-21 09:29:57.000000 pytest_django_docker_pg-0.0.3/pytest_django_docker_pg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-21 09:29:57.000000 pytest_django_docker_pg-0.0.3/pytest_django_docker_pg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 09:29:57.000000 pytest_django_docker_pg-0.0.3/pytest_django_docker_pg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:29:57.386236 pytest_django_docker_pg-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:29:57.386236 pytest_django_docker_pg-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-21 09:29:49.000000 pytest_django_docker_pg-0.0.3/tests/test_plugin.py
```

### Comparing `pytest_django_docker_pg-0.0.2/LICENSE` & `pytest_django_docker_pg-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_django_docker_pg-0.0.2/PKG-INFO` & `pytest_django_docker_pg-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_django_docker_pg
-Version: 0.0.2
+Version: 0.0.3
 License: MIT License
         
         Copyright (c) 2024 Belegnar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -34,16 +34,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pytest<8.0.0,>=7.0.0
+Requires-Dist: pytest<9.0.0,>=7.0.0
 Requires-Dist: docker>=6.1.0
+Requires-Dist: requests<2.32.0
 
 # pytest-django-docker-pg
 
 Starts a dockerized postgresql instance in pytest hook allowing `pytest_django` tests, for example, to be run against it.
 
 ## How to use
```

### Comparing `pytest_django_docker_pg-0.0.2/README.md` & `pytest_django_docker_pg-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pytest_django_docker_pg-0.0.2/pyproject.toml` & `pytest_django_docker_pg-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytest_django_docker_pg"
 dynamic = ["version"]
 requires-python = ">=3.10"
 dependencies = [
-    "pytest>=7.0.0,<8.0.0",
+    "pytest>=7.0.0,<9.0.0",
     "docker>=6.1.0",
+    "requests<2.32.0",
 ]
 classifiers = [
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.10",
```

### Comparing `pytest_django_docker_pg-0.0.2/pytest_django_docker_pg/plugin.py` & `pytest_django_docker_pg-0.0.3/pytest_django_docker_pg/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_django_docker_pg-0.0.2/pytest_django_docker_pg.egg-info/PKG-INFO` & `pytest_django_docker_pg-0.0.3/pytest_django_docker_pg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_django_docker_pg
-Version: 0.0.2
+Version: 0.0.3
 License: MIT License
         
         Copyright (c) 2024 Belegnar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -34,16 +34,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pytest<8.0.0,>=7.0.0
+Requires-Dist: pytest<9.0.0,>=7.0.0
 Requires-Dist: docker>=6.1.0
+Requires-Dist: requests<2.32.0
 
 # pytest-django-docker-pg
 
 Starts a dockerized postgresql instance in pytest hook allowing `pytest_django` tests, for example, to be run against it.
 
 ## How to use
```

