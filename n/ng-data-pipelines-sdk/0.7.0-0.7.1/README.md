# Comparing `tmp/ng_data_pipelines_sdk-0.7.0.tar.gz` & `tmp/ng_data_pipelines_sdk-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-0.7.0.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-0.7.1.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-0.7.0.tar` & `ng_data_pipelines_sdk-0.7.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-05-16 12:33:29.095550 ng_data_pipelines_sdk-0.7.0/README.md
--rw-r--r--   0        0        0        0 2024-05-16 12:33:29.131551 ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     9155 2024-05-16 12:33:29.095550 ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-05-16 12:33:29.095550 ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    28114 2024-05-16 12:33:29.095550 ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0    15903 2024-05-16 12:33:29.095550 ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     5093 2024-05-16 12:33:29.096551 ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     1453 2024-05-16 12:33:29.096551 ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      695 2024-05-16 12:33:29.100551 ng_data_pipelines_sdk-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-05-21 12:53:15.051813 ng_data_pipelines_sdk-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 12:53:15.085813 ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     9155 2024-05-21 12:53:15.051813 ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-05-21 12:53:15.052813 ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    28114 2024-05-21 12:53:15.052813 ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0    15903 2024-05-21 12:53:15.052813 ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     5093 2024-05-21 12:53:15.052813 ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     1453 2024-05-21 12:53:15.052813 ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      695 2024-05-21 12:53:15.055813 ng_data_pipelines_sdk-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.7.1/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/interfaces.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.7.0/pyproject.toml` & `ng_data_pipelines_sdk-0.7.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "0.7.0"
+version = "0.7.1"
 description = "A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 pyspark = "^3.2.0"
-pydantic = "^2.5.3"
-boto3 = "^1.33.13"
+pydantic = "^2.4.2"
+boto3 = "^1.28.17"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.29.4"
 ruff = "^0.3.7"
 load-dotenv = "^0.1.0"
 
 [build-system]
```

### Comparing `ng_data_pipelines_sdk-0.7.0/PKG-INFO` & `ng_data_pipelines_sdk-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 0.7.0
+Version: 0.7.1
 Summary: A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: boto3 (>=1.33.13,<2.0.0)
-Requires-Dist: pydantic (>=2.5.3,<3.0.0)
+Requires-Dist: boto3 (>=1.28.17,<2.0.0)
+Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: pyspark (>=3.2.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 docker run --rm -it -d -e PYTHONPATH="/ng-data-pipelines-sdk" -v $pwd:/ng-data-pipelines-sdk pyspark-local
```

