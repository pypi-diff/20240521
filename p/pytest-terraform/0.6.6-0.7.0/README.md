# Comparing `tmp/pytest_terraform-0.6.6.tar.gz` & `tmp/pytest_terraform-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_terraform-0.6.6.tar", max compression
+gzip compressed data, was "pytest_terraform-0.7.0.tar", max compression
```

## Comparing `pytest_terraform-0.6.6.tar` & `pytest_terraform-0.7.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     9196 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/README.md
--rw-r--r--   0        0        0     1466 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pyproject.toml
--rw-r--r--   0        0        0      670 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pytest_terraform/__init__.py
--rw-r--r--   0        0        0      500 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pytest_terraform/exceptions.py
--rw-r--r--   0        0        0       93 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pytest_terraform/hooks.py
--rw-r--r--   0        0        0     2003 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pytest_terraform/lock.py
--rw-r--r--   0        0        0      835 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pytest_terraform/options.py
--rw-r--r--   0        0        0     3102 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pytest_terraform/plugin.py
--rw-r--r--   0        0        0    16910 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pytest_terraform/tf.py
--rw-r--r--   0        0        0     7414 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pytest_terraform/xdist.py
--rw-r--r--   0        0        0    10260 1970-01-01 00:00:00.000000 pytest_terraform-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     9196 2024-05-21 17:01:22.016882 pytest_terraform-0.7.0/README.md
+-rw-r--r--   0        0        0     1466 2024-05-21 17:01:22.020882 pytest_terraform-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      670 2024-05-21 17:01:22.020882 pytest_terraform-0.7.0/pytest_terraform/__init__.py
+-rw-r--r--   0        0        0      500 2024-05-21 17:01:22.020882 pytest_terraform-0.7.0/pytest_terraform/exceptions.py
+-rw-r--r--   0        0        0       93 2024-05-21 17:01:22.020882 pytest_terraform-0.7.0/pytest_terraform/hooks.py
+-rw-r--r--   0        0        0     2003 2024-05-21 17:01:22.020882 pytest_terraform-0.7.0/pytest_terraform/lock.py
+-rw-r--r--   0        0        0      835 2024-05-21 17:01:22.020882 pytest_terraform-0.7.0/pytest_terraform/options.py
+-rw-r--r--   0        0        0     3159 2024-05-21 17:01:22.020882 pytest_terraform-0.7.0/pytest_terraform/plugin.py
+-rw-r--r--   0        0        0    16910 2024-05-21 17:01:22.020882 pytest_terraform-0.7.0/pytest_terraform/tf.py
+-rw-r--r--   0        0        0     7414 2024-05-21 17:01:22.020882 pytest_terraform-0.7.0/pytest_terraform/xdist.py
+-rw-r--r--   0        0        0    10311 1970-01-01 00:00:00.000000 pytest_terraform-0.7.0/PKG-INFO
```

### Comparing `pytest_terraform-0.6.6/README.md` & `pytest_terraform-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_terraform-0.6.6/pyproject.toml` & `pytest_terraform-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-terraform"
-version = "0.6.6"
+version = "0.7.0"
 description = "A pytest plugin for using terraform fixtures"
 authors = ["Kapil Thangavelu <kapilt@gmail.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/cloud-custodian/pytest-terraform"
 classifiers=[
    "Topic :: Software Development :: Testing",
    "Topic :: System :: Systems Administration",
```

### Comparing `pytest_terraform-0.6.6/pytest_terraform/__init__.py` & `pytest_terraform-0.7.0/pytest_terraform/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_terraform-0.6.6/pytest_terraform/lock.py` & `pytest_terraform-0.7.0/pytest_terraform/lock.py`

 * *Files identical despite different names*

### Comparing `pytest_terraform-0.6.6/pytest_terraform/options.py` & `pytest_terraform-0.7.0/pytest_terraform/options.py`

 * *Files identical despite different names*

### Comparing `pytest_terraform-0.6.6/pytest_terraform/plugin.py` & `pytest_terraform-0.7.0/pytest_terraform/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,20 @@
     tf.LazyModuleDir.value = config.getoption("dest_tf_mod_dir") or config.getini(
         "terraform-mod-dir"
     )
 
     if tf.LazyReplay.value is None:
         tf.LazyReplay.value = config.getoption("dest_tf_replay")
 
-    tf.LazyTfBin.value = config.getoption("dest_tf_binary") or shutil.which("terraform")
+    tf.LazyTfBin.value = (
+        config.getoption("dest_tf_binary")
+        or shutil.which("tofu")
+        or shutil.which("terraform")
+    )
+
     if tf.LazyTfBin.value is None and not tf.LazyReplay.value:
         raise ValueError(
             "pytest-terraform requires terraform binary on PATH or "
             "specified with --tf-binary"
         )
 
     tf.PytestConfig.value = config
```

### Comparing `pytest_terraform-0.6.6/pytest_terraform/tf.py` & `pytest_terraform-0.7.0/pytest_terraform/tf.py`

 * *Files identical despite different names*

### Comparing `pytest_terraform-0.6.6/pytest_terraform/xdist.py` & `pytest_terraform-0.7.0/pytest_terraform/xdist.py`

 * *Files identical despite different names*

### Comparing `pytest_terraform-0.6.6/PKG-INFO` & `pytest_terraform-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pytest-terraform
-Version: 0.6.6
+Version: 0.7.0
 Summary: A pytest plugin for using terraform fixtures
 Home-page: https://github.com/cloud-custodian/pytest-terraform
 License: Apache-2.0
 Author: Kapil Thangavelu
 Author-email: kapilt@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Systems Administration
 Requires-Dist: jmespath (>=0.10.0)
 Requires-Dist: portalocker (>=1.7.0)
 Requires-Dist: pytest (>=6.0)
 Requires-Dist: pytest-xdist (>=1.31.0)
```

