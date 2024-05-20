# Comparing `tmp/aws_stuff_doer-0.1.2.tar.gz` & `tmp/aws_stuff_doer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_stuff_doer-0.1.2.tar", max compression
+gzip compressed data, was "aws_stuff_doer-0.1.3.tar", max compression
```

## Comparing `aws_stuff_doer-0.1.2.tar` & `aws_stuff_doer-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1062 2024-02-17 18:46:32.476469 aws_stuff_doer-0.1.2/LICENSE
--rw-r--r--   0        0        0     1770 2024-05-20 00:17:33.839532 aws_stuff_doer-0.1.2/README.md
--rw-r--r--   0        0        0       36 2024-05-19 21:57:31.595516 aws_stuff_doer-0.1.2/cmd/__init__.py
--rw-r--r--   0        0        0      490 2024-04-14 18:46:05.938170 aws_stuff_doer-0.1.2/cmd/get_version.py
--rw-r--r--   0        0        0     7789 2024-05-20 01:03:15.368378 aws_stuff_doer-0.1.2/cmd/login.py
--rw-r--r--   0        0        0     1662 2024-05-20 22:23:34.883393 aws_stuff_doer-0.1.2/main.py
--rw-r--r--   0        0        0      926 2024-05-20 22:22:27.584033 aws_stuff_doer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 aws_stuff_doer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-02-17 18:46:32.476469 aws_stuff_doer-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1770 2024-05-20 00:17:33.839532 aws_stuff_doer-0.1.3/README.md
+-rw-r--r--   0        0        0       48 2024-05-20 22:54:57.163674 aws_stuff_doer-0.1.3/aws-stuff-doer/__init__.py
+-rw-r--r--   0        0        0       36 2024-05-19 21:57:31.595516 aws_stuff_doer-0.1.3/aws-stuff-doer/cmd/__init__.py
+-rw-r--r--   0        0        0      490 2024-04-14 18:46:05.938170 aws_stuff_doer-0.1.3/aws-stuff-doer/cmd/get_version.py
+-rw-r--r--   0        0        0     7789 2024-05-20 01:03:15.368378 aws_stuff_doer-0.1.3/aws-stuff-doer/cmd/login.py
+-rw-r--r--   0        0        0     1662 2024-05-20 22:23:34.883393 aws_stuff_doer-0.1.3/aws-stuff-doer/main.py
+-rw-r--r--   0        0        0      889 2024-05-20 22:58:09.097528 aws_stuff_doer-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 aws_stuff_doer-0.1.3/PKG-INFO
```

### Comparing `aws_stuff_doer-0.1.2/LICENSE` & `aws_stuff_doer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_stuff_doer-0.1.2/README.md` & `aws_stuff_doer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aws_stuff_doer-0.1.2/cmd/login.py` & `aws_stuff_doer-0.1.3/aws-stuff-doer/cmd/login.py`

 * *Files identical despite different names*

### Comparing `aws_stuff_doer-0.1.2/main.py` & `aws_stuff_doer-0.1.3/aws-stuff-doer/main.py`

 * *Files identical despite different names*

### Comparing `aws_stuff_doer-0.1.2/pyproject.toml` & `aws_stuff_doer-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 [tool.poetry]
 name = "aws-stuff-doer"
-version = "0.1.2"
+version = "0.1.3"
 description = "ASD is a utility to help manage your AWS projects and sso sessions."
 authors = [
     "Aaron West <aphexlog@gmail.com>",
     "ant <anthony.chiarello132@gmail.com>",
 ]
 repository = "https://github.com/aphexlog/aws-stuff-doer"
 license = "MIT"
 readme = "README.md"
-packages = [
-    { from = ".", include = "main.py" },
-    { from = "cmd", include = "*" },
-]
+packages = [{ from = "aws-stuff-doer", include = "*" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 boto3 = "^1.34.36"
 gitpython = "^3.1.41"
 aws-cdk-lib = "^2.126.0"
 boto3-stubs = "^1.34.36"
```

### Comparing `aws_stuff_doer-0.1.2/PKG-INFO` & `aws_stuff_doer-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-stuff-doer
-Version: 0.1.2
+Version: 0.1.3
 Summary: ASD is a utility to help manage your AWS projects and sso sessions.
 Home-page: https://github.com/aphexlog/aws-stuff-doer
 License: MIT
 Author: Aaron West
 Author-email: aphexlog@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

