# Comparing `tmp/kthutils-1.8.tar.gz` & `tmp/kthutils-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kthutils-1.8.tar", max compression
+gzip compressed data, was "kthutils-1.9.tar", max compression
```

## Comparing `kthutils-1.8.tar` & `kthutils-1.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1074 2023-03-28 06:51:16.830958 kthutils-1.8/LICENSE
--rw-r--r--   0        0        0      921 2023-11-06 08:19:10.580862 kthutils-1.8/README.md
--rw-r--r--   0        0        0      720 2023-11-06 08:35:15.294440 kthutils-1.8/pyproject.toml
--rw-r--r--   0        0        0      113 2023-11-06 08:35:07.986250 kthutils-1.8/src/kthutils/.gitignore
--rw-r--r--   0        0        0      483 2023-11-06 08:35:07.986250 kthutils-1.8/src/kthutils/Makefile
--rw-r--r--   0        0        0        0 2022-11-07 09:18:59.264876 kthutils-1.8/src/kthutils/__init__.py
--rw-r--r--   0        0        0     4074 2023-11-06 08:35:07.986250 kthutils-1.8/src/kthutils/cli.nw
--rw-r--r--   0        0        0      492 2023-11-06 08:37:48.434709 kthutils-1.8/src/kthutils/cli.py
--rw-r--r--   0        0        0      755 2023-11-06 08:37:48.438709 kthutils-1.8/src/kthutils/credentials.py
--rw-r--r--   0        0        0     7336 2023-11-06 08:35:07.986250 kthutils-1.8/src/kthutils/iprange.nw
--rw-r--r--   0        0        0      796 2023-11-06 08:37:48.466710 kthutils-1.8/src/kthutils/iprange.py
--rw-r--r--   0        0        0    14910 2023-11-06 08:37:48.582713 kthutils-1.8/src/kthutils/iprange.tex
--rw-r--r--   0        0        0    14478 2023-11-06 06:50:41.697239 kthutils-1.8/src/kthutils/participants.nw
--rw-r--r--   0        0        0     6371 2023-11-06 08:37:48.454710 kthutils-1.8/src/kthutils/participants.py
--rw-r--r--   0        0        0    18914 2023-08-25 17:14:42.445089 kthutils-1.8/src/kthutils/ug.nw
--rw-r--r--   0        0        0     9929 2023-11-06 08:37:48.446709 kthutils-1.8/src/kthutils/ug.py
--rw-r--r--   0        0        0      917 2023-11-06 08:38:11.107379 kthutils-1.8/tests/test_participants.py
--rw-r--r--   0        0        0      745 2023-11-06 08:38:11.111379 kthutils-1.8/tests/test_ug.py
--rw-r--r--   0        0        0     1880 1970-01-01 00:00:00.000000 kthutils-1.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-28 06:51:16.830958 kthutils-1.9/LICENSE
+-rw-r--r--   0        0        0      921 2023-11-06 08:19:10.580862 kthutils-1.9/README.md
+-rw-r--r--   0        0        0      733 2023-11-06 08:47:27.041094 kthutils-1.9/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-11-06 08:35:07.986250 kthutils-1.9/src/kthutils/.gitignore
+-rw-r--r--   0        0        0      483 2023-11-06 08:35:07.986250 kthutils-1.9/src/kthutils/Makefile
+-rw-r--r--   0        0        0        0 2022-11-07 09:18:59.264876 kthutils-1.9/src/kthutils/__init__.py
+-rw-r--r--   0        0        0     4074 2023-11-06 08:35:07.986250 kthutils-1.9/src/kthutils/cli.nw
+-rw-r--r--   0        0        0      492 2023-11-06 08:48:14.414657 kthutils-1.9/src/kthutils/cli.py
+-rw-r--r--   0        0        0      755 2023-11-06 08:48:14.418657 kthutils-1.9/src/kthutils/credentials.py
+-rw-r--r--   0        0        0     7336 2023-11-06 08:35:07.986250 kthutils-1.9/src/kthutils/iprange.nw
+-rw-r--r--   0        0        0      796 2023-11-06 08:48:14.434657 kthutils-1.9/src/kthutils/iprange.py
+-rwxr-xr-x   0        0        0     1129 2023-11-06 08:48:14.430657 kthutils-1.9/src/kthutils/iprange.sh
+-rw-r--r--   0        0        0    14910 2023-11-06 08:48:14.526661 kthutils-1.9/src/kthutils/iprange.tex
+-rw-r--r--   0        0        0    14478 2023-11-06 06:50:41.697239 kthutils-1.9/src/kthutils/participants.nw
+-rw-r--r--   0        0        0     6371 2023-11-06 08:48:14.426657 kthutils-1.9/src/kthutils/participants.py
+-rw-r--r--   0        0        0    18914 2023-08-25 17:14:42.445089 kthutils-1.9/src/kthutils/ug.nw
+-rw-r--r--   0        0        0     9929 2023-11-06 08:48:14.422657 kthutils-1.9/src/kthutils/ug.py
+-rw-r--r--   0        0        0      917 2023-11-06 08:48:32.959269 kthutils-1.9/tests/test_participants.py
+-rw-r--r--   0        0        0      745 2023-11-06 08:48:32.963269 kthutils-1.9/tests/test_ug.py
+-rw-r--r--   0        0        0     1880 1970-01-01 00:00:00.000000 kthutils-1.9/PKG-INFO
```

### Comparing `kthutils-1.8/LICENSE` & `kthutils-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kthutils-1.8/README.md` & `kthutils-1.9/README.md`

 * *Files identical despite different names*

### Comparing `kthutils-1.8/pyproject.toml` & `kthutils-1.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "kthutils"
-version = "1.8"
+version = "1.9"
 description = "Various tools for automation at KTH"
 authors = ["Daniel Bosk <dbosk@kth.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbosk/kthutils"
-include = ["*/**/*.py"]
+include = ["*/**/*.py", "*/**/*.sh"]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/dbosk/kthutils/issues"
 "Releases" = "https://github.com/dbosk/kthutils/releases"
 
 [tool.poetry.scripts]
 kthutils = "kthutils.cli:cli"
```

### Comparing `kthutils-1.8/src/kthutils/cli.nw` & `kthutils-1.9/src/kthutils/cli.nw`

 * *Files identical despite different names*

### Comparing `kthutils-1.8/src/kthutils/credentials.py` & `kthutils-1.9/src/kthutils/credentials.py`

 * *Files identical despite different names*

### Comparing `kthutils-1.8/src/kthutils/iprange.nw` & `kthutils-1.9/src/kthutils/iprange.nw`

 * *Files identical despite different names*

### Comparing `kthutils-1.8/src/kthutils/iprange.py` & `kthutils-1.9/src/kthutils/iprange.py`

 * *Files identical despite different names*

### Comparing `kthutils-1.8/src/kthutils/iprange.tex` & `kthutils-1.9/src/kthutils/iprange.tex`

 * *Files identical despite different names*

### Comparing `kthutils-1.8/src/kthutils/participants.nw` & `kthutils-1.9/src/kthutils/participants.nw`

 * *Files identical despite different names*

### Comparing `kthutils-1.8/src/kthutils/participants.py` & `kthutils-1.9/src/kthutils/participants.py`

 * *Files identical despite different names*

### Comparing `kthutils-1.8/src/kthutils/ug.nw` & `kthutils-1.9/src/kthutils/ug.nw`

 * *Files identical despite different names*

### Comparing `kthutils-1.8/src/kthutils/ug.py` & `kthutils-1.9/src/kthutils/ug.py`

 * *Files identical despite different names*

### Comparing `kthutils-1.8/tests/test_participants.py` & `kthutils-1.9/tests/test_participants.py`

 * *Files identical despite different names*

### Comparing `kthutils-1.8/tests/test_ug.py` & `kthutils-1.9/tests/test_ug.py`

 * *Files identical despite different names*

### Comparing `kthutils-1.8/PKG-INFO` & `kthutils-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kthutils
-Version: 1.8
+Version: 1.9
 Summary: Various tools for automation at KTH
 Home-page: https://github.com/dbosk/kthutils
 License: MIT
 Author: Daniel Bosk
 Author-email: dbosk@kth.se
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

