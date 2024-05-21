# Comparing `tmp/bitbucket_pipeline_runner-0.4.2.tar.gz` & `tmp/bitbucket_pipeline_runner-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitbucket_pipeline_runner-0.4.2.tar", max compression
+gzip compressed data, was "bitbucket_pipeline_runner-0.4.3.tar", max compression
```

## Comparing `bitbucket_pipeline_runner-0.4.2.tar` & `bitbucket_pipeline_runner-0.4.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1070 2024-05-01 22:12:59.144712 bitbucket_pipeline_runner-0.4.2/LICENSE
--rw-r--r--   0        0        0     1046 2024-05-01 22:12:59.144712 bitbucket_pipeline_runner-0.4.2/README.md
--rw-r--r--   0        0        0       29 2024-05-01 22:12:59.144712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/__init__.py
--rw-r--r--   0        0        0       61 2024-05-01 22:12:59.144712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/__main__.py
--rw-r--r--   0        0        0     3057 2024-05-01 22:12:59.144712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/artifacts.py
--rw-r--r--   0        0        0    10673 2024-05-01 22:12:59.144712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/cache.py
--rw-r--r--   0        0        0     5267 2024-05-01 22:12:59.144712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/cli.py
--rw-r--r--   0        0        0     3227 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/config.py
--rw-r--r--   0        0        0    18041 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/container.py
--rw-r--r--   0        0        0     5831 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/context.py
--rw-r--r--   0        0        0      608 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/errors.py
--rw-r--r--   0        0        0    14998 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/models.py
--rw-r--r--   0        0        0      357 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/parse.py
--rw-r--r--   0        0        0        0 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/py.typed
--rw-r--r--   0        0        0     4193 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/repository.py
--rw-r--r--   0        0        0    15676 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/runner.py
--rw-r--r--   0        0        0     9283 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/service.py
--rw-r--r--   0        0        0        0 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/static/__init__.py
--rw-r--r--   0        0        0     1665 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/static/known_hosts
--rwxr-xr-x   0        0        0      451 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/static/runit.sh
--rw-r--r--   0        0        0     4331 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/utils.py
--rw-r--r--   0        0        0     2844 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2308 1970-01-01 00:00:00.000000 bitbucket_pipeline_runner-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/LICENSE
+-rw-r--r--   0        0        0     1046 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/README.md
+-rw-r--r--   0        0        0       29 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/__init__.py
+-rw-r--r--   0        0        0       61 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/__main__.py
+-rw-r--r--   0        0        0     3057 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/artifacts.py
+-rw-r--r--   0        0        0    10673 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/cache.py
+-rw-r--r--   0        0        0     5267 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/cli.py
+-rw-r--r--   0        0        0     3227 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/config.py
+-rw-r--r--   0        0        0    18041 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/container.py
+-rw-r--r--   0        0        0     5831 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/context.py
+-rw-r--r--   0        0        0      608 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/errors.py
+-rw-r--r--   0        0        0    14998 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/models.py
+-rw-r--r--   0        0        0      357 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/parse.py
+-rw-r--r--   0        0        0        0 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/py.typed
+-rw-r--r--   0        0        0     4460 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/repository.py
+-rw-r--r--   0        0        0    15676 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/runner.py
+-rw-r--r--   0        0        0     9283 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/service.py
+-rw-r--r--   0        0        0        0 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/static/__init__.py
+-rw-r--r--   0        0        0     1665 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/static/known_hosts
+-rwxr-xr-x   0        0        0      451 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/static/runit.sh
+-rw-r--r--   0        0        0     4331 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pipeline_runner/utils.py
+-rw-r--r--   0        0        0     2844 2024-05-21 15:30:26.565894 bitbucket_pipeline_runner-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2308 1970-01-01 00:00:00.000000 bitbucket_pipeline_runner-0.4.3/PKG-INFO
```

### Comparing `bitbucket_pipeline_runner-0.4.2/LICENSE` & `bitbucket_pipeline_runner-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.2/README.md` & `bitbucket_pipeline_runner-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.2/pipeline_runner/artifacts.py` & `bitbucket_pipeline_runner-0.4.3/pipeline_runner/artifacts.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.2/pipeline_runner/cache.py` & `bitbucket_pipeline_runner-0.4.3/pipeline_runner/cache.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.2/pipeline_runner/cli.py` & `bitbucket_pipeline_runner-0.4.3/pipeline_runner/cli.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.2/pipeline_runner/config.py` & `bitbucket_pipeline_runner-0.4.3/pipeline_runner/config.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.2/pipeline_runner/container.py` & `bitbucket_pipeline_runner-0.4.3/pipeline_runner/container.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.2/pipeline_runner/context.py` & `bitbucket_pipeline_runner-0.4.3/pipeline_runner/context.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.2/pipeline_runner/errors.py` & `bitbucket_pipeline_runner-0.4.3/pipeline_runner/errors.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.2/pipeline_runner/models.py` & `bitbucket_pipeline_runner-0.4.3/pipeline_runner/models.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.2/pipeline_runner/repository.py` & `bitbucket_pipeline_runner-0.4.3/pipeline_runner/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,20 @@
             self._data_volume_name,
             self._environment,
             self._output_logger,
         )
         runner.start()
 
         try:
+            exec_result = runner.run_command(
+                f"git config --system --add safe.directory '{config.remote_workspace_dir}/.git'", user=0
+            )
+            if exec_result.exit_code:
+                raise Exception("Error setting up repository")
+
             clone_script = self._get_clone_script()
             exit_code = runner.run_script(clone_script)
 
             if exit_code:
                 raise Exception("Error setting up repository")
         finally:
             runner.stop()
```

### Comparing `bitbucket_pipeline_runner-0.4.2/pipeline_runner/runner.py` & `bitbucket_pipeline_runner-0.4.3/pipeline_runner/runner.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.2/pipeline_runner/service.py` & `bitbucket_pipeline_runner-0.4.3/pipeline_runner/service.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.2/pipeline_runner/static/known_hosts` & `bitbucket_pipeline_runner-0.4.3/pipeline_runner/static/known_hosts`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.2/pipeline_runner/utils.py` & `bitbucket_pipeline_runner-0.4.3/pipeline_runner/utils.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.2/pyproject.toml` & `bitbucket_pipeline_runner-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bitbucket-pipeline-runner"
-version = "0.4.2"
+version = "0.4.3"
 description = "Run a bitbucket pipeline locally"
 authors = ["Mathieu Lemay <acidrain1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mathieu-lemay/pipeline-runner"
 packages = [
     {include = "pipeline_runner"}
```

### Comparing `bitbucket_pipeline_runner-0.4.2/PKG-INFO` & `bitbucket_pipeline_runner-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitbucket-pipeline-runner
-Version: 0.4.2
+Version: 0.4.3
 Summary: Run a bitbucket pipeline locally
 Home-page: https://github.com/mathieu-lemay/pipeline-runner
 License: MIT
 Author: Mathieu Lemay
 Author-email: acidrain1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

