# Comparing `tmp/ng_data_pipelines_sdk-0.7.1.tar.gz` & `tmp/ng_data_pipelines_sdk-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-0.7.1.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-0.8.0.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-0.7.1.tar` & `ng_data_pipelines_sdk-0.8.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-05-21 12:53:15.051813 ng_data_pipelines_sdk-0.7.1/README.md
--rw-r--r--   0        0        0        0 2024-05-21 12:53:15.085813 ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     9155 2024-05-21 12:53:15.051813 ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-05-21 12:53:15.052813 ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    28114 2024-05-21 12:53:15.052813 ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0    15903 2024-05-21 12:53:15.052813 ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     5093 2024-05-21 12:53:15.052813 ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     1453 2024-05-21 12:53:15.052813 ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      695 2024-05-21 12:53:15.055813 ng_data_pipelines_sdk-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-05-21 19:33:47.203868 ng_data_pipelines_sdk-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 19:33:47.236868 ng_data_pipelines_sdk-0.8.0/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     9155 2024-05-21 19:33:47.203868 ng_data_pipelines_sdk-0.8.0/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-05-21 19:33:47.203868 ng_data_pipelines_sdk-0.8.0/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    28614 2024-05-21 19:33:47.203868 ng_data_pipelines_sdk-0.8.0/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0    16231 2024-05-21 19:33:47.203868 ng_data_pipelines_sdk-0.8.0/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     5093 2024-05-21 19:33:47.204868 ng_data_pipelines_sdk-0.8.0/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     1453 2024-05-21 19:33:47.204868 ng_data_pipelines_sdk-0.8.0/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      695 2024-05-21 19:33:47.207868 ng_data_pipelines_sdk-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.8.0/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-0.8.0/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-0.8.0/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,19 +113,23 @@
 
         Raises:
             ValueError: If there is an issue retrieving or handling the schema.
         """
 
         if s3_read_schema_params is None:
             raise ValueError(
-                "s3_schema_path_params must be provided to retrieve schema from S3"
+                "s3_schema_path_params must be provided"
             )
 
         if s3_read_schema_params.bucket_params.bucket_name is None:
-            raise ValueError("bucket_name must be provided to retrieve schema from S3")
+            raise ValueError("bucket_name must be provided")
+
+        if s3_read_schema_params.bucket_params.env is None:
+            raise ValueError("env must be provided")
+
 
         bucket_name = s3_read_schema_params.bucket_params.bucket_name
         path_to_file = s3_read_schema_params.path
         full_s3_file_path = f"{self.file_system}://{bucket_name}/{path_to_file}"
 
         logger.debug(f"Retrieving schema from path '{full_s3_file_path}'...")
         try:
@@ -164,14 +168,17 @@
             df_params (InputDataFrameParams): The parameters for reading the DataFrame.
 
         Returns:
             DataFrame: The read DataFrame.
 
         """
         read_params = df_params.df_params
+        if read_params.bucket_params.env is None:
+            raise ValueError("env must be provided")
+
         bucket_url = self._get_bucket_url(read_params.bucket_params)
         if read_params.specific_path:
             if isinstance(read_params.specific_path, list):
                 path = [f"{bucket_url}/{path}" for path in read_params.specific_path]
             else:
                 path = f"{bucket_url}/{read_params.specific_path}"
         else:
@@ -227,17 +234,19 @@
         Parameters:
         - df (DataFrame): The DataFrame whose schema is to be written.
 
         Raises:
         - ValueError: If there is an issue with writing the schema object to AWS S3.
         """
         pyspark_schema_json = df.schema.jsonValue()
-        bucket_name = write_params.bucket_params.bucket_name
 
-        if bucket_name is None:
+        if write_params.bucket_params.env is None:
+            raise ValueError("env must be provided")
+
+        if write_params.bucket_params.bucket_name is None:
             raise ValueError("bucket_name must be provided to write schema to S3")
 
         if write_params.specific_path:
             if isinstance(write_params.specific_path, list):
                 raise ValueError(
                     "Specific path is set as a list. Only a single path is allowed for writing the schema."
                 )
@@ -255,21 +264,21 @@
                 write_params.path_to_dataframe_root.split("/")[:-1]
             )
             path_to_schema = f"{parent_folder_of_dataframe_root}/schema.json"
 
         try:
             self.aws_interface.put_object_aws(
                 env=write_params.bucket_params.env,
-                bucket_name=bucket_name,
+                bucket_name=write_params.bucket_params.bucket_name,
                 object_name=path_to_schema,
                 object_data=pyspark_schema_json,
             )
         except Exception as e:
             raise ValueError(
-                f"Error writing schema to {bucket_name}/{path_to_schema}: {e}"
+                f"Error writing schema to {write_params.bucket_params.bucket_name}/{path_to_schema}: {e}"
             )
 
     def _get_partitions(self, write_params: DataFrameReadWriteParams) -> List[str]:
         date_partition_columns: List[str] = []
         if write_params.processing_date_partitions:
             for date_partition in write_params.processing_date_partitions:
                 date_partition_columns.append(date_partition.value)
@@ -294,14 +303,17 @@
 
         return partitions
 
     def write_dataframe_specific_path(
         self, df: DataFrame, df_params: OutputDataFrameParams
     ) -> None:
         write_params = df_params.df_params
+        if write_params.bucket_params.env is None:
+            raise ValueError("env must be provided")
+
         bucket_url = self._get_bucket_url(write_params.bucket_params)
         write_path_url = f"{bucket_url}/{write_params.path_to_dataframe_root}"
 
         logger.info(f"Writing DataFrame to path: {write_path_url}...")
         self.spark_manager.write(
             env=write_params.bucket_params.env,
             df=df,
@@ -326,14 +338,17 @@
             df (DataFrame): The DataFrame to be written.
             df_params (OutputDataFrameParams): The parameters for writing the DataFrame.
 
         Returns:
             None
         """
         write_params = df_params.df_params
+        if write_params.bucket_params.env is None:
+            raise ValueError("env must be provided")
+
         bucket_url = self._get_bucket_url(write_params.bucket_params)
         write_path_url = f"{bucket_url}/{write_params.path_to_dataframe_root}"
         logger.debug(f"Write root path: {write_path_url}")
 
         partitions = self._get_partitions(write_params)
         logger.debug(f"Using partitions: {partitions}")
```

### Comparing `ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-0.8.0/ng_data_pipelines_sdk/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,21 +145,32 @@
     Attributes:
         env (Env): The environment. Must be one of "Env.DEV" or "Env.PRD".
         layer (Optional[Layer]): The layer (optional).
         ng_prefix (str): The NG prefix. Defaults to "ng".
         bucket_name (Optional[str]): The bucket name (optional). If not provided, it will be generated based on the layer, environment, and NG prefix.
     """
 
-    env: Env
+    env: Optional[Env] = None
     layer: Optional[Layer] = None
     ng_prefix: str = "ng"
     bucket_name: Optional[str] = None
 
     @model_validator(mode="before")
-    def set_bucket_name_if_not_provided(cls, data):
+    def set_env_and_bucket_name_if_not_provided(cls, data):
+        env = data.get("env")
+        if env is None:
+            env = os.environ.get("ENV")
+
+            if env is None:
+                raise ValueError(
+                    "If 'env' is not provided, the environment variable 'ENV' must be set"
+                )
+
+            data["env"] = Env(env)
+
         layer = data.get("layer").value if data.get("layer") is not None else None
         env = data.get("env").value
         ng_prefix = data.get("ng_prefix", "ng")
         bucket_name = data.get("bucket_name")
 
         if bucket_name is None:
             if layer is None:
```

### Comparing `ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-0.8.0/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.7.1/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-0.8.0/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.7.1/pyproject.toml` & `ng_data_pipelines_sdk-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "0.7.1"
+version = "0.8.0"
 description = "A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `ng_data_pipelines_sdk-0.7.1/PKG-INFO` & `ng_data_pipelines_sdk-0.8.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 0.7.1
+Version: 0.8.0
 Summary: A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

