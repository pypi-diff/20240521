# Comparing `tmp/pysonrpc-1.0.6.tar.gz` & `tmp/pysonrpc-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysonrpc-1.0.6.tar", last modified: Thu Mar  7 00:17:31 2024, max compression
+gzip compressed data, was "pysonrpc-1.0.7.tar", last modified: Tue May 21 16:04:45 2024, max compression
```

## Comparing `pysonrpc-1.0.6.tar` & `pysonrpc-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:17:31.296659 pysonrpc-1.0.6/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-03-07 00:16:29.000000 pysonrpc-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-03-07 00:17:31.296659 pysonrpc-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-03-07 00:16:29.000000 pysonrpc-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-03-07 00:16:29.000000 pysonrpc-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 00:17:31.296659 pysonrpc-1.0.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-03-07 00:16:29.000000 pysonrpc-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:17:31.292659 pysonrpc-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:17:31.292659 pysonrpc-1.0.6/src/pysonrpc/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-07 00:16:29.000000 pysonrpc-1.0.6/src/pysonrpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-03-07 00:16:29.000000 pysonrpc-1.0.6/src/pysonrpc/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10944 2024-03-07 00:16:29.000000 pysonrpc-1.0.6/src/pysonrpc/jsonrpc.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-07 00:16:29.000000 pysonrpc-1.0.6/src/pysonrpc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:17:31.296659 pysonrpc-1.0.6/src/pysonrpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-03-07 00:17:31.000000 pysonrpc-1.0.6/src/pysonrpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-07 00:17:31.000000 pysonrpc-1.0.6/src/pysonrpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 00:17:31.000000 pysonrpc-1.0.6/src/pysonrpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-07 00:17:31.000000 pysonrpc-1.0.6/src/pysonrpc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-07 00:17:31.000000 pysonrpc-1.0.6/src/pysonrpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-07 00:17:31.000000 pysonrpc-1.0.6/src/pysonrpc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:17:31.292659 pysonrpc-1.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-03-07 00:16:29.000000 pysonrpc-1.0.6/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9575 2024-03-07 00:16:29.000000 pysonrpc-1.0.6/test/test_jsonrpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:04:45.610931 pysonrpc-1.0.7/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-05-21 16:03:48.000000 pysonrpc-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-21 16:04:45.610931 pysonrpc-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-21 16:03:48.000000 pysonrpc-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-21 16:03:48.000000 pysonrpc-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 16:04:45.614930 pysonrpc-1.0.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-05-21 16:03:48.000000 pysonrpc-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:04:45.606931 pysonrpc-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:04:45.610931 pysonrpc-1.0.7/src/pysonrpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-21 16:03:48.000000 pysonrpc-1.0.7/src/pysonrpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-21 16:03:48.000000 pysonrpc-1.0.7/src/pysonrpc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10944 2024-05-21 16:03:48.000000 pysonrpc-1.0.7/src/pysonrpc/jsonrpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 16:03:48.000000 pysonrpc-1.0.7/src/pysonrpc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:04:45.610931 pysonrpc-1.0.7/src/pysonrpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-21 16:04:45.000000 pysonrpc-1.0.7/src/pysonrpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-21 16:04:45.000000 pysonrpc-1.0.7/src/pysonrpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 16:04:45.000000 pysonrpc-1.0.7/src/pysonrpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 16:04:45.000000 pysonrpc-1.0.7/src/pysonrpc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-21 16:04:45.000000 pysonrpc-1.0.7/src/pysonrpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 16:04:45.000000 pysonrpc-1.0.7/src/pysonrpc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:04:45.610931 pysonrpc-1.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-21 16:03:48.000000 pysonrpc-1.0.7/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9575 2024-05-21 16:03:48.000000 pysonrpc-1.0.7/test/test_jsonrpc.py
```

### Comparing `pysonrpc-1.0.6/LICENSE` & `pysonrpc-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pysonrpc-1.0.6/PKG-INFO` & `pysonrpc-1.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysonrpc
-Version: 1.0.6
+Version: 1.0.7
 Summary: JSON RPC Python client with autodiscovery and methods mapping
 Author-email: Vivien Chene <viv@vivc.org>
 Maintainer-email: Vivien Chene <viv@vivc.org>
 License: MIT License
         Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -61,15 +61,15 @@
 # List all methods available, autodetected from a schema json file
 pysonrpc -r http://127.0.0.1:8080/jsonrpc -f schema.json list
 
 # List methods filtered with VideoLibrary
 pysonrpc -r http://127.0.0.1:8080/jsonrpc -am "JSONRPC.Introspect" list -s -f VideoLibrary
 
 # Get favaourites list
-pysonrpc -r http://127.0.0.1:8080/jsonrpc -a run Favourites.GetFavourites
+pysonrpc -r http://127.0.0.1:8080/jsonrpc -a run -m Favourites.GetFavourites
 
 # Get information on movie 1419
 pysonrpc -r http://127.0.0.1:8080/jsonrpc -a run -m VideoLibrary.GetMovieDetails -p '{"movieid": 1419}'
 ```
 
 Help
 ```bash
@@ -144,11 +144,24 @@
 ```
 
 If mypy fails due to missing import stubs:
 ```sh
 .tox/checkers/bin/mypy --install-types
 ```
 
+### Release
+
+To push to main and increment the current version:
+```sh
+pixi run release
+```
+
+To push to main and specify the new version current version:
+```sh
+pixi run release 1.2.3
+```
+
+_Note: A workflow is validating, building, releasing and publishing push requests and tagged commits_
+
 ### TODO:
 - better way for parameters ? (add a list arg for a method only)
-- tests and coverage
```

### Comparing `pysonrpc-1.0.6/README.md` & `pysonrpc-1.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # List all methods available, autodetected from a schema json file
 pysonrpc -r http://127.0.0.1:8080/jsonrpc -f schema.json list
 
 # List methods filtered with VideoLibrary
 pysonrpc -r http://127.0.0.1:8080/jsonrpc -am "JSONRPC.Introspect" list -s -f VideoLibrary
 
 # Get favaourites list
-pysonrpc -r http://127.0.0.1:8080/jsonrpc -a run Favourites.GetFavourites
+pysonrpc -r http://127.0.0.1:8080/jsonrpc -a run -m Favourites.GetFavourites
 
 # Get information on movie 1419
 pysonrpc -r http://127.0.0.1:8080/jsonrpc -a run -m VideoLibrary.GetMovieDetails -p '{"movieid": 1419}'
 ```
 
 Help
 ```bash
@@ -105,11 +105,24 @@
 ```
 
 If mypy fails due to missing import stubs:
 ```sh
 .tox/checkers/bin/mypy --install-types
 ```
 
+### Release
+
+To push to main and increment the current version:
+```sh
+pixi run release
+```
+
+To push to main and specify the new version current version:
+```sh
+pixi run release 1.2.3
+```
+
+_Note: A workflow is validating, building, releasing and publishing push requests and tagged commits_
+
 ### TODO:
 - better way for parameters ? (add a list arg for a method only)
-- tests and coverage
```

### Comparing `pysonrpc-1.0.6/pyproject.toml` & `pysonrpc-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pysonrpc-1.0.6/src/pysonrpc/cli.py` & `pysonrpc-1.0.7/src/pysonrpc/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,14 @@
             password=args.password,
             auto_detect=args.schema_discover,
             schema_path=args.schema_discover_path,
             schema_method=args.schema_discover_method,
             json_file=args.method_file,
         )
 
-        print(args)
         if hasattr(args, "func") and args.func:
             args.func(cli, args)
         else:
             raise pysonrpc.JsonRpcClientError(f"No processing defined for command {args.command}")
 
         sys.exit(0)
     except pysonrpc.JsonRpcClientError as e:
```

### Comparing `pysonrpc-1.0.6/src/pysonrpc/jsonrpc.py` & `pysonrpc-1.0.7/src/pysonrpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `pysonrpc-1.0.6/src/pysonrpc.egg-info/PKG-INFO` & `pysonrpc-1.0.7/src/pysonrpc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysonrpc
-Version: 1.0.6
+Version: 1.0.7
 Summary: JSON RPC Python client with autodiscovery and methods mapping
 Author-email: Vivien Chene <viv@vivc.org>
 Maintainer-email: Vivien Chene <viv@vivc.org>
 License: MIT License
         Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -61,15 +61,15 @@
 # List all methods available, autodetected from a schema json file
 pysonrpc -r http://127.0.0.1:8080/jsonrpc -f schema.json list
 
 # List methods filtered with VideoLibrary
 pysonrpc -r http://127.0.0.1:8080/jsonrpc -am "JSONRPC.Introspect" list -s -f VideoLibrary
 
 # Get favaourites list
-pysonrpc -r http://127.0.0.1:8080/jsonrpc -a run Favourites.GetFavourites
+pysonrpc -r http://127.0.0.1:8080/jsonrpc -a run -m Favourites.GetFavourites
 
 # Get information on movie 1419
 pysonrpc -r http://127.0.0.1:8080/jsonrpc -a run -m VideoLibrary.GetMovieDetails -p '{"movieid": 1419}'
 ```
 
 Help
 ```bash
@@ -144,11 +144,24 @@
 ```
 
 If mypy fails due to missing import stubs:
 ```sh
 .tox/checkers/bin/mypy --install-types
 ```
 
+### Release
+
+To push to main and increment the current version:
+```sh
+pixi run release
+```
+
+To push to main and specify the new version current version:
+```sh
+pixi run release 1.2.3
+```
+
+_Note: A workflow is validating, building, releasing and publishing push requests and tagged commits_
+
 ### TODO:
 - better way for parameters ? (add a list arg for a method only)
-- tests and coverage
```

### Comparing `pysonrpc-1.0.6/test/test_cli.py` & `pysonrpc-1.0.7/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `pysonrpc-1.0.6/test/test_jsonrpc.py` & `pysonrpc-1.0.7/test/test_jsonrpc.py`

 * *Files identical despite different names*

