# Comparing `tmp/pass_operator-0.4.0.tar.gz` & `tmp/pass_operator-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pass_operator-0.4.0.tar", max compression
+gzip compressed data, was "pass_operator-0.4.1.tar", max compression
```

## Comparing `pass_operator-0.4.0.tar` & `pass_operator-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35140 2024-05-19 14:56:44.759517 pass_operator-0.4.0/LICENSE
--rw-r--r--   0        0        0     7833 2024-05-19 14:56:44.759517 pass_operator-0.4.0/README.md
--rw-r--r--   0        0        0     1606 2024-05-19 14:56:57.055595 pass_operator-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1562 2024-05-19 14:56:44.763517 pass_operator-0.4.0/src/passoperator/__init__.py
--rw-r--r--   0        0        0    14494 2024-05-19 14:56:44.763517 pass_operator-0.4.0/src/passoperator/daemon.py
--rw-r--r--   0        0        0     2017 2024-05-19 14:56:44.763517 pass_operator-0.4.0/src/passoperator/git.py
--rw-r--r--   0        0        0     1218 2024-05-19 14:56:44.763517 pass_operator-0.4.0/src/passoperator/gpg.py
--rw-r--r--   0        0        0     8500 2024-05-19 14:56:44.763517 pass_operator-0.4.0/src/passoperator/secret.py
--rw-r--r--   0        0        0     1313 2024-05-19 14:56:44.763517 pass_operator-0.4.0/src/passoperator/utils.py
--rw-r--r--   0        0        0     8770 1970-01-01 00:00:00.000000 pass_operator-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35140 2024-05-21 06:10:18.891776 pass_operator-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3343 2024-05-21 06:10:18.891776 pass_operator-0.4.1/README.md
+-rw-r--r--   0        0        0     1606 2024-05-21 06:10:31.815980 pass_operator-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1562 2024-05-21 06:10:18.899777 pass_operator-0.4.1/src/passoperator/__init__.py
+-rw-r--r--   0        0        0    14494 2024-05-21 06:10:18.899777 pass_operator-0.4.1/src/passoperator/daemon.py
+-rw-r--r--   0        0        0     2017 2024-05-21 06:10:18.899777 pass_operator-0.4.1/src/passoperator/git.py
+-rw-r--r--   0        0        0     1218 2024-05-21 06:10:18.899777 pass_operator-0.4.1/src/passoperator/gpg.py
+-rw-r--r--   0        0        0     8500 2024-05-21 06:10:18.899777 pass_operator-0.4.1/src/passoperator/secret.py
+-rw-r--r--   0        0        0     1313 2024-05-21 06:10:18.899777 pass_operator-0.4.1/src/passoperator/utils.py
+-rw-r--r--   0        0        0     4280 1970-01-01 00:00:00.000000 pass_operator-0.4.1/PKG-INFO
```

### Comparing `pass_operator-0.4.0/LICENSE` & `pass_operator-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.0/pyproject.toml` & `pass_operator-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pass-operator"
-version = "v0.4.0"
+version = "v0.4.1"
 description = "A kubernetes operator that syncs and decrypts secrets from pass git repositories"
 authors = ["Emma Doyle <emma@premiscale.com>"]
 maintainers = ["Emma Doyle <emma@premiscale.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [
   { include = "passoperator", from = "src" }
```

### Comparing `pass_operator-0.4.0/src/passoperator/__init__.py` & `pass_operator-0.4.1/src/passoperator/__init__.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.0/src/passoperator/daemon.py` & `pass_operator-0.4.1/src/passoperator/daemon.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.0/src/passoperator/git.py` & `pass_operator-0.4.1/src/passoperator/git.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.0/src/passoperator/gpg.py` & `pass_operator-0.4.1/src/passoperator/gpg.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.0/src/passoperator/secret.py` & `pass_operator-0.4.1/src/passoperator/secret.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.0/src/passoperator/utils.py` & `pass_operator-0.4.1/src/passoperator/utils.py`

 * *Files identical despite different names*

