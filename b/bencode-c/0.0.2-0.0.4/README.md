# Comparing `tmp/bencode_c-0.0.2.tar.gz` & `tmp/bencode_c-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bencode_c-0.0.2.tar", last modified: Mon May 20 22:42:18 2024, max compression
+gzip compressed data, was "bencode_c-0.0.4.tar", last modified: Mon May 20 23:05:43 2024, max compression
```

## Comparing `bencode_c-0.0.2.tar` & `bencode_c-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:42:18.296928 bencode_c-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 22:42:18.296928 bencode_c-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-20 22:42:15.000000 bencode_c-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-20 22:42:15.000000 bencode_c-0.0.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 22:42:18.296928 bencode_c-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-20 22:42:15.000000 bencode_c-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:42:18.292928 bencode_c-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:42:18.292928 bencode_c-0.0.2/src/bencode_c/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 22:42:15.000000 bencode_c-0.0.2/src/bencode_c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-20 22:42:15.000000 bencode_c-0.0.2/src/bencode_c/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-20 22:42:15.000000 bencode_c-0.0.2/src/bencode_c/bencode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:42:18.292928 bencode_c-0.0.2/src/bencode_c.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 22:42:18.000000 bencode_c-0.0.2/src/bencode_c.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 22:42:18.000000 bencode_c-0.0.2/src/bencode_c.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:42:18.000000 bencode_c-0.0.2/src/bencode_c.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-20 22:42:18.000000 bencode_c-0.0.2/src/bencode_c.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 22:42:18.000000 bencode_c-0.0.2/src/bencode_c.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:42:18.292928 bencode_c-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-20 22:42:15.000000 bencode_c-0.0.2/tests/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-20 22:42:15.000000 bencode_c-0.0.2/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-20 22:42:15.000000 bencode_c-0.0.2/tests/test_torrent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:05:43.523172 bencode_c-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 23:05:43.523172 bencode_c-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-20 23:05:39.000000 bencode_c-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-20 23:05:39.000000 bencode_c-0.0.4/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 23:05:43.523172 bencode_c-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-20 23:05:39.000000 bencode_c-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:05:43.519172 bencode_c-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:05:43.523172 bencode_c-0.0.4/src/bencode_c/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 23:05:39.000000 bencode_c-0.0.4/src/bencode_c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-20 23:05:39.000000 bencode_c-0.0.4/src/bencode_c/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-20 23:05:39.000000 bencode_c-0.0.4/src/bencode_c/bencode.c
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 23:05:39.000000 bencode_c-0.0.4/src/bencode_c/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-20 23:05:39.000000 bencode_c-0.0.4/src/bencode_c/decode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-05-20 23:05:39.000000 bencode_c-0.0.4/src/bencode_c/encode.h
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 23:05:39.000000 bencode_c-0.0.4/src/bencode_c/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:05:43.523172 bencode_c-0.0.4/src/bencode_c.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 23:05:43.000000 bencode_c-0.0.4/src/bencode_c.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-20 23:05:43.000000 bencode_c-0.0.4/src/bencode_c.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 23:05:43.000000 bencode_c-0.0.4/src/bencode_c.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-20 23:05:43.000000 bencode_c-0.0.4/src/bencode_c.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 23:05:43.000000 bencode_c-0.0.4/src/bencode_c.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:05:43.523172 bencode_c-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-20 23:05:39.000000 bencode_c-0.0.4/tests/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-20 23:05:39.000000 bencode_c-0.0.4/tests/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-20 23:05:39.000000 bencode_c-0.0.4/tests/test_torrent.py
```

### Comparing `bencode_c-0.0.2/PKG-INFO` & `bencode_c-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bencode-c
-Version: 0.0.2
+Version: 0.0.4
 Summary: A fast and correct bencode serialize/deserialize library
 Author-email: trim21 <trim21me@gmail.com>
 License: MIT
 Keywords: bencode,bittorrent,bit-torrent,serialize,deserialize,p2p
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bencode_c-0.0.2/pyproject.toml` & `bencode_c-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pyproject.toml
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bencode-c"
-version = "0.0.2"
+version = "0.0.4"
 description = "A fast and correct bencode serialize/deserialize library"
 license = { text = "MIT" }
 requires-python = ">=3.8,<4.0"
 authors = [
     { name = "trim21", email = "trim21me@gmail.com" },
 ]
 readme = 'readme.md'
@@ -33,12 +33,12 @@
 
 [project.optional-dependencies]
 testing = [
     'pytest==8.2.0',
     "pytest-github-actions-annotate-failures==0.2.0",
 ]
 
-[tool.distutils.bdist_wheel]
-py-limited-api = 'cp38'
+#[tool.distutils.bdist_wheel]
+#py-limited-api = 'cp38'
 
 [tool.pytest.ini_options]
 pythonpath = ['src']
```

### Comparing `bencode_c-0.0.2/src/bencode_c/bencode.c` & `bencode_c-0.0.4/src/bencode_c/bencode.c`

 * *Files identical despite different names*

### Comparing `bencode_c-0.0.2/src/bencode_c.egg-info/PKG-INFO` & `bencode_c-0.0.4/src/bencode_c.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bencode-c
-Version: 0.0.2
+Version: 0.0.4
 Summary: A fast and correct bencode serialize/deserialize library
 Author-email: trim21 <trim21me@gmail.com>
 License: MIT
 Keywords: bencode,bittorrent,bit-torrent,serialize,deserialize,p2p
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bencode_c-0.0.2/tests/test_decode.py` & `bencode_c-0.0.4/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `bencode_c-0.0.2/tests/test_encode.py` & `bencode_c-0.0.4/tests/test_encode.py`

 * *Files identical despite different names*

