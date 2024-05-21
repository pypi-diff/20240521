# Comparing `tmp/mostlyai-0.3.5.tar.gz` & `tmp/mostlyai-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mostlyai-0.3.5.tar", max compression
+gzip compressed data, was "mostlyai-0.3.6.tar", max compression
```

## Comparing `mostlyai-0.3.5.tar` & `mostlyai-0.3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-03-08 15:08:04.881678 mostlyai-0.3.5/LICENSE
--rw-r--r--   0        0        0     2303 2024-05-13 12:51:10.053542 mostlyai-0.3.5/README.md
--rw-r--r--   0        0        0       26 2024-03-19 14:08:19.064057 mostlyai-0.3.5/mostlyai/__init__.py
--rw-r--r--   0        0        0    14643 2024-05-13 12:51:10.056448 mostlyai-0.3.5/mostlyai/api.py
--rw-r--r--   0        0        0     9150 2024-05-13 12:51:10.057253 mostlyai-0.3.5/mostlyai/base.py
--rw-r--r--   0        0        0     3103 2024-05-13 12:51:10.058056 mostlyai-0.3.5/mostlyai/connectors.py
--rw-r--r--   0        0        0      574 2024-03-19 14:08:19.083253 mostlyai-0.3.5/mostlyai/exceptions.py
--rw-r--r--   0        0        0     4193 2024-05-13 12:51:10.058284 mostlyai-0.3.5/mostlyai/generators.py
--rw-r--r--   0        0        0    42470 2024-05-13 12:51:10.058814 mostlyai-0.3.5/mostlyai/model.py
--rw-r--r--   0        0        0     1694 2024-05-13 12:51:10.058978 mostlyai-0.3.5/mostlyai/shares.py
--rw-r--r--   0        0        0     7215 2024-05-13 12:51:10.059430 mostlyai-0.3.5/mostlyai/synthetic_datasets.py
--rw-r--r--   0        0        0     5217 2024-03-19 14:08:19.082058 mostlyai-0.3.5/mostlyai/utils.py
--rw-r--r--   0        0        0     1370 2024-05-13 14:28:07.566943 mostlyai-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 mostlyai-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-12-22 12:47:38.462094 mostlyai-0.3.6/LICENSE
+-rw-r--r--   0        0        0     2438 2024-05-21 10:29:45.117002 mostlyai-0.3.6/README.md
+-rw-r--r--   0        0        0       58 2024-05-15 08:25:32.630029 mostlyai-0.3.6/mostlyai/__init__.py
+-rw-r--r--   0        0        0    14463 2024-05-21 10:29:45.117812 mostlyai-0.3.6/mostlyai/api.py
+-rw-r--r--   0        0        0     9150 2024-04-19 16:58:34.132208 mostlyai-0.3.6/mostlyai/base.py
+-rw-r--r--   0        0        0     3103 2024-05-13 15:27:45.794003 mostlyai-0.3.6/mostlyai/connectors.py
+-rw-r--r--   0        0        0      574 2024-04-19 16:58:25.136734 mostlyai-0.3.6/mostlyai/exceptions.py
+-rw-r--r--   0        0        0     4232 2024-05-21 10:29:45.118404 mostlyai-0.3.6/mostlyai/generators.py
+-rw-r--r--   0        0        0    44710 2024-05-21 10:29:45.119013 mostlyai-0.3.6/mostlyai/model.py
+-rw-r--r--   0        0        0     1694 2024-04-22 07:20:07.509641 mostlyai-0.3.6/mostlyai/shares.py
+-rw-r--r--   0        0        0     6701 2024-05-21 10:29:45.119700 mostlyai-0.3.6/mostlyai/synthetic_datasets.py
+-rw-r--r--   0        0        0     9491 2024-05-21 10:29:45.120294 mostlyai-0.3.6/mostlyai/utils.py
+-rw-r--r--   0        0        0     1269 2024-05-21 10:55:44.122851 mostlyai-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3205 1970-01-01 00:00:00.000000 mostlyai-0.3.6/PKG-INFO
```

### Comparing `mostlyai-0.3.5/LICENSE` & `mostlyai-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.5/README.md` & `mostlyai-0.3.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ```shell
 pip install mostlyai
 ```
 
 ## Basic Usage
 ```python
 from mostlyai import MostlyAI
-mostly = MostlyAI(api_key='your_api_key') 
+mostly = MostlyAI(api_key='your_api_key')
 g = mostly.train(data)      # train a generator on your data
 sd = mostly.generate(g)     # generate a synthetic dataset
 syn = sd.data()             # consume synthetic as pd.DataFrame
 ```
 
 ## Supported Methods
 
@@ -87,14 +87,21 @@
 sd.generation.cancel()
 sd.generation.wait()
 
 sd.data()
 sd.download(file, format)
 ```
 
+### Synthetic Probes
+```python
+sp = mostly.probe(g, seed=seed)
+sp = mostly.probe(g, size=size)
+sp = mostly.probe(g, config=config)
+```
+
 ### Sharing
 
 ```python
 mostly.share(g | sd | c, email)
 mostly.unshare(g | sd | c, email)
 
 g.shares()
```

### Comparing `mostlyai-0.3.5/mostlyai/api.py` & `mostlyai-0.3.6/mostlyai/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from pathlib import Path
-from typing import Any, Optional, Union
+from typing import Any, Optional, Union, Literal
 
 import pandas as pd
 import rich
 
 from mostlyai.base import GET, _MostlyBaseClient
 from mostlyai.connectors import _MostlyConnectorsClient
 from mostlyai.generators import _MostlyGeneratorsClient
 from mostlyai.model import (
     Connector,
     CurrentUser,
     Generator,
     PermissionLevel,
     ProgressStatus,
+    SyntheticDataset,
 )
 from mostlyai.shares import _MostlySharesClient
-from mostlyai.synthetic_datasets import _MostlySyntheticDatasetsClient
+from mostlyai.synthetic_datasets import (
+    _MostlySyntheticDatasetsClient,
+    _MostlySyntheticProbesClient,
+)
 from mostlyai.utils import (
     ShareableResource,
-    _get_subject_table_names,
     _read_table_from_path,
+    _harmonize_sd_config,
+    Seed,
 )
 
 
 class MostlyAI(_MostlyBaseClient):
     """
     Client for interacting with the Mostly AI Public API.
 
@@ -48,156 +53,136 @@
             "api_key": self.api_key,
             "timeout": self.timeout,
             "ssl_verify": self.ssl_verify,
         }
         self.connectors = _MostlyConnectorsClient(**client_kwargs)
         self.generators = _MostlyGeneratorsClient(**client_kwargs)
         self.synthetic_datasets = _MostlySyntheticDatasetsClient(**client_kwargs)
+        self.synthetic_probes = _MostlySyntheticProbesClient(**client_kwargs)
         self.shares = _MostlySharesClient(**client_kwargs)
 
     def connect(self, config: dict[str, Any]) -> Connector:
         """
         Create a connector, and optionally validate the connection before saving.
 
         If validation fails, a 400 status with an error message will be returned.
 
         `config` is a dictionary with the keys `type`, `config`, `secrets`, and `ssl`.
         The structures of the `config`, `secrets` and `ssl` parameters depend on the connector `type`:
 
         - Cloud storage:
-            - \t
-            ```yaml
-            type: AZURE_STORAGE
+          ```yaml
+          - type: AZURE_STORAGE
             config:
               accountName: string
               clientId: string (required for auth via service principal)
               tenantId: string (required for auth via service principal)
             secrets:
               accountKey: string (required for regular auth)
               clientSecret: string (required for auth via service principal)
-            ```
-            - \t
-            ```yaml
-            type: GOOGLE_CLOUD_STORAGE
+
+          - type: GOOGLE_CLOUD_STORAGE
             config:
             secrets:
               keyFile: string
-            ```
-            - \t
-            ```yaml
-            type: S3_STORAGE
+
+          - type: S3_STORAGE
             config:
               accessKey: string
+              endpointUrl: string (only needed for S3-compatible storage services other than AWS)
             secrets:
               secretKey: string
-            ```
+          ```
         - Database:
-            - \t
-                ```yaml
-                type: BIGQUERY
-                config:
-                secrets:
-                  keyFile: string
-                ```
-            - \t
-                ```yaml
-                type: DATABRICKS
-                config:
-                  host: string
-                  httpPath: string
-                  catalog: string
-                  clientId: string (required for auth via service principal)
-                  tenantId: string (required for auth via service principal)
-                secrets:
-                  accessToken: string (required for regular auth)
-                  clientSecret: string (required for auth via service principal)
-                ```
-            - \t
-                ```yaml
-                type: HIVE
-                config:
-                  host: string
-                  port: integer, default: 10000
-                  username: string (required for regular auth)
-                  kerberos_enabled: boolean, default: false
-                  kerberos_principal: string (required if kerberos_enabled)
-                  kerberos_krb5_conf: string (required if kerberos_enabled)
-                secrets:
-                  password: string (required for regular auth)
-                  kerberos_keytab: base64-encoded string (required if kerberos_enabled)
-                ```
-            - \t
-                ```yaml
-                type: MARIADB
-                config:
-                  host: string
-                  port: integer, default: 3306
-                  username: string
-                secrets:
-                  password: string
-                ```
-            - \t
-                ```yaml
-                type: MSSQL
-                config:
-                  host: string
-                  port: integer, default: 1433
-                  username: string
-                  database: string
-                secrets:
-                 password: string
-                ```
-            - \t
-                ```yaml
-                type: MYSQL
-                config:
-                  host: string
-                  port: integer, default: 3306
-                  username: string
-                secrets:
-                  password: string
-                ```
-            - \t
-                ```yaml
-                type: ORACLE
-                config:
-                  host: string
-                  port: integer, default: 1521
-                  username: string
-                  connectionType: enum {SID, SERVICE_NAME}, default: SID
-                  database: string, default: ORCL
-                secrets:
-                  password: string
-                ```
-            - \t
-                ```yaml
-                type: POSTGRES
-                config:
-                  host: string
-                  port: integer, default: 5432
-                  username: string
-                  database: string
-                secrets:
-                  password: string
-                ssl:
-                  rootCertificate: string
-                  sslCertificate: string
-                  sslCertificateKey: string
-                ```
-            - \t
-                ```yaml
-                type: SNOWFLAKE
-                config:
-                  account: string
-                  username: string
-                  warehouse: string, default: COMPUTE_WH
-                  database: string
-                secrets:
-                  password: string
-                ```
+          ```yaml
+          - type: BIGQUERY
+            config:
+            secrets:
+              keyFile: string
+
+          - type: DATABRICKS
+            config:
+              host: string
+              httpPath: string
+              catalog: string
+              clientId: string (required for auth via service principal)
+              tenantId: string (required for auth via service principal)
+            secrets:
+              accessToken: string (required for regular auth)
+              clientSecret: string (required for auth via service principal)
+
+          - type: HIVE
+            config:
+              host: string
+              port: integer, default: 10000
+              username: string (required for regular auth)
+              kerberos_enabled: boolean, default: false
+              kerberos_principal: string (required if kerberos_enabled)
+              kerberos_krb5_conf: string (required if kerberos_enabled)
+            secrets:
+              password: string (required for regular auth)
+              kerberos_keytab: base64-encoded string (required if kerberos_enabled)
+
+          - type: MARIADB
+            config:
+              host: string
+              port: integer, default: 3306
+              username: string
+            secrets:
+              password: string
+
+          - type: MSSQL
+            config:
+              host: string
+              port: integer, default: 1433
+              username: string
+              database: string
+            secrets:
+             password: string
+
+          - type: MYSQL
+            config:
+              host: string
+              port: integer, default: 3306
+              username: string
+            secrets:
+              password: string
+
+          - type: ORACLE
+            config:
+              host: string
+              port: integer, default: 1521
+              username: string
+              connectionType: enum {SID, SERVICE_NAME}, default: SID
+              database: string, default: ORCL
+            secrets:
+              password: string
+
+          - type: POSTGRES
+            config:
+              host: string
+              port: integer, default: 5432
+              username: string
+              database: string
+            secrets:
+              password: string
+            ssl:
+              rootCertificate: string
+              sslCertificate: string
+              sslCertificateKey: string
+
+          - type: SNOWFLAKE
+            config:
+              account: string
+              username: string
+              warehouse: string, default: COMPUTE_WH
+              database: string
+            secrets:
+              password: string
+          ```
 
         :return: The created connector.
         """
         c = self.connectors.create(config)
         rich.print(
             f"Created connector [link={self.base_url}/d/connectors/{c.id} blue underline]{c.id}[/]"
         )
@@ -206,23 +191,25 @@
     def train(
         self,
         data: Union[pd.DataFrame, str, Path, None] = None,
         config: Union[dict, None] = None,
         name: Optional[str] = None,
         start: bool = True,
         wait: bool = True,
-    ):
+        progress_bar: bool = True,
+    ) -> Generator:
         """
         Train a generator
 
         :param data: Either a single pandas DataFrame data, a path to a CSV or PARQUET file. Note: Either 'data' or 'config' must be provided.
         :param config: The configuration parameters of the generator to be created. See Generator.config for the structure of the parameters. Note: Either 'data' or 'config' must be provided.
         :param name: Optional. The name of the generator.
         :param start: If true, then training is started right away. Default: true.
         :param wait: If true, then the function only returns once training has finished. Default: true.
+        :param progress_bar: If true, then the progress bar will be displayed, in case of wait=True
         :return: The created generator.
         """
         if data is not None and config is not None:
             raise ValueError("Either data or config must be provided, but not both")
         if isinstance(data, (str, Path)):
             name, df = _read_table_from_path(data)
             config = {"name": name, "tables": [{"data": df, "name": name}]}
@@ -240,99 +227,92 @@
         rich.print(
             f"Created generator [link={self.base_url}/d/generators/{g.id} blue underline]{g.id}[/]"
         )
         if start:
             g.training.start()
             rich.print("Started generator training")
         if start and wait:
-            g = g.training.wait()
+            g = g.training.wait(progress_bar=progress_bar)
             if g.training_status == ProgressStatus.done:
                 rich.print(
                     ":tada: [bold green]Your generator is ready![/] "
                     "Use it to create synthetic data. "
                     "Share it so others can do the same."
                 )
         return g
 
     def generate(
         self,
         generator: Union[Generator, str, None] = None,
         size: Union[int, dict[str, int], None] = None,
-        seed: Union[
-            pd.DataFrame, str, Path, dict[str, Union[pd.DataFrame, str, Path]], None
-        ] = None,
+        seed: Union[Seed, dict[str, Seed], None] = None,
         config: Union[dict, None] = None,
         name: Optional[str] = None,
         start: bool = True,
         wait: bool = True,
-    ):
+        progress_bar: bool = True,
+    ) -> SyntheticDataset:
         """
-        Train a generator
+        Generate synthetic data
 
         :param generator: The generator instance or its UUID, that is to be used for generating synthetic data.
         :param config: The configuration parameters of the synthetic dataset to be created. See SyntheticDataset.config for the structure of the parameters.
         :param size: Optional. Either a single integer, or a dictionary of integers. Used for specifying the sample_size of the subject table(s).
         :param seed: Optional. Either a single pandas DataFrame data, or a path to a CSV or PARQUET file, or a dictionary of those. Used for seeding the subject table(s).
         :param name: Optional. The name of the synthetic dataset.
         :param start: If true, then generation is started right away. Default: true.
         :param wait: If true, then the function only returns once generation has finished. Default: true.
+        :param progress_bar: If true, then the progress bar will be displayed, in case of wait=True
         :return: The created synthetic dataset.
         """
-        if config is None:
-            config = {}
-        if isinstance(generator, Generator):
-            config["generatorId"] = str(generator.id)
-        elif generator is not None:
-            config["generatorId"] = str(generator)
-        elif "generatorId" not in config:
-            raise ValueError(
-                "Either a generator or a configuration with a generatorId must be provided."
-            )
-
-        if "tables" not in config:
-            g = self.generators.get(config["generatorId"])
-            subject_tables = _get_subject_table_names(g.config())
-            config["tables"] = [
-                {
-                    "name": table,
-                    "configuration": {
-                        "sampleSize": (
-                            size.get(table) if isinstance(size, dict) else size
-                        ),
-                        "sampleSeedData": (
-                            seed.get(table) if isinstance(seed, dict) else seed
-                        ),
-                    },
-                }
-                for table in subject_tables
-            ]
-
-        if name is not None:
-            config |= {"name": name}
-
+        config = _harmonize_sd_config(generator, size, seed, config, name)
         sd = self.synthetic_datasets.create(config)
         rich.print(
             f"Created synthetic dataset "
             f"[link={self.base_url}/d/synthetic-datasets/{sd.id} blue underline]{sd.id}[/] "
             f"with generator "
             f"[link={self.base_url}/d/generators/{sd.generator.id} blue underline]{sd.generator.id}[/]"
         )
         if start:
             sd.generation.start()
             rich.print("Started synthetic dataset generation")
         if start and wait:
-            sd = sd.generation.wait()
+            sd = sd.generation.wait(progress_bar=progress_bar)
             if sd.generation_status == ProgressStatus.done:
                 rich.print(
                     ":tada: [bold green]Your synthetic dataset is ready![/] "
                     "Use it to consume the generated data. "
                     "Share it so others can do the same."
                 )
         return sd
 
+    def probe(
+        self,
+        generator: Union[Generator, str, None] = None,
+        size: Union[int, dict[str, int], None] = None,
+        seed: Union[Seed, dict[str, Seed], None] = None,
+        config: Union[dict, None] = None,
+        return_type: Literal["auto", "dict"] = "auto",
+    ) -> Union[pd.DataFrame, dict[str, pd.DataFrame]]:
+        """
+        Probe a generator
+
+        :param generator: The generator instance or its UUID, that is to be used for generating synthetic data.
+        :param config: The configuration parameters of the synthetic dataset to be created. See SyntheticDataset.config for the structure of the parameters.
+        :param size: Optional. Either a single integer, or a dictionary of integers. Used for specifying the sample_size of the subject table(s).
+        :param seed: Optional. Either a single pandas DataFrame data, or a path to a CSV or PARQUET file, or list of samples, or a dictionary of those. Used for seeding the subject table(s).
+        :return: The created synthetic probe.
+        """
+        config = _harmonize_sd_config(generator, size, seed, config)
+        dfs = self.synthetic_probes.create(config)
+        if return_type == "auto" and len(dfs) == 1:
+            return list(dfs.values())[0]
+        else:
+            return dfs
+
     # SHARES
 
     def share(
         self,
         resource: ShareableResource,
         user_email: str,
         permission_level: Union[str, PermissionLevel] = PermissionLevel.view,
```

### Comparing `mostlyai-0.3.5/mostlyai/base.py` & `mostlyai-0.3.6/mostlyai/base.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.5/mostlyai/connectors.py` & `mostlyai-0.3.6/mostlyai/connectors.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.5/mostlyai/exceptions.py` & `mostlyai-0.3.6/mostlyai/exceptions.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.5/mostlyai/generators.py` & `mostlyai-0.3.6/mostlyai/generators.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Iterator, Optional, Union
 
 import pandas as pd
 
 from mostlyai.base import DELETE, GET, PATCH, POST, Paginator, _MostlyBaseClient
 from mostlyai.model import Generator, JobProgress
 from mostlyai.shares import _MostlySharesMixin
-from mostlyai.utils import _convert_df_to_base64, _job_wait, _read_table_from_path
+from mostlyai.utils import _convert_to_base64, _job_wait, _read_table_from_path
 
 
 class _MostlyGeneratorsClient(_MostlyBaseClient, _MostlySharesMixin):
     SECTION = ["generators"]
 
     # PUBLIC METHODS #
 
@@ -57,20 +57,20 @@
     def create(self, config: dict) -> Generator:
         # convert `data` to base64-encoded Parquet files
         if "tables" in config and config["tables"]:
             for table in config["tables"]:
                 if "data" in table and table["data"] is not None:
                     if isinstance(table["data"], (str, Path)):
                         name, df = _read_table_from_path(table["data"])
-                        table["data"] = _convert_df_to_base64(df)
+                        table["data"] = _convert_to_base64(df)
                         if "name" not in table:
                             table["name"] = name
                         del df
                     elif isinstance(table["data"], pd.DataFrame):
-                        table["data"] = _convert_df_to_base64(table["data"])
+                        table["data"] = _convert_to_base64(table["data"])
                     else:
                         raise ValueError("data must be a DataFrame or a file path")
 
         generator = self.request(
             verb=POST, path=[], json=config, response_type=Generator
         )
         return generator
@@ -104,11 +104,13 @@
 
     def _training_progress(self, generator_id: str) -> JobProgress:
         response = self.request(
             verb=GET, path=[generator_id, "training"], response_type=JobProgress
         )
         return response
 
-    def _training_wait(self, generator_id: str, interval: float) -> Generator:
-        _job_wait(lambda: self._training_progress(generator_id), interval)
+    def _training_wait(
+        self, generator_id: str, progress_bar: bool, interval: float
+    ) -> Generator:
+        _job_wait(lambda: self._training_progress(generator_id), interval, progress_bar)
         generator = self.get(generator_id)
         return generator
```

### Comparing `mostlyai-0.3.5/mostlyai/model.py` & `mostlyai-0.3.6/mostlyai/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # generated by datamodel-codegen:
 #   timestamp: 2024-05-13T11:50:56+00:00
 
 from __future__ import annotations
 
-from datetime import datetime
 from enum import Enum
 from pathlib import Path
 from typing import Annotated, Any, ClassVar, Dict, List, Literal, Optional, Union
 
 import pandas as pd
-from pydantic import Field, RootModel
+from pydantic import AwareDatetime, Field, RootModel
 
 from mostlyai.base import CustomBaseModel
 
 
 class PermissionLevel(str, Enum):
     """
     The permission level of the user or group with respect to this entity
@@ -28,96 +27,105 @@
     edit = "EDIT"
     admin = "ADMIN"
 
 
 class Credits(CustomBaseModel):
     current: Annotated[
         Optional[float],
-        Field(description="The credit balance for the current time period"),
+        Field(None, description="The credit balance for the current time period"),
     ] = None
     limit: Annotated[
         Optional[float],
         Field(
-            description="The credit limit for the current time period. If empty, then there is no limit."
+            None,
+            description="The credit limit for the current time period. If empty, then there is no limit.",
         ),
     ] = None
     period_start: Annotated[
-        Optional[datetime],
+        Optional[AwareDatetime],
         Field(
+            None,
             alias="periodStart",
             description="The UTC date and time when the current time period started",
         ),
     ] = None
     period_end: Annotated[
-        Optional[datetime],
+        Optional[AwareDatetime],
         Field(
+            None,
             alias="periodEnd",
             description="The UTC date and time when the current time period ends",
         ),
     ] = None
 
 
 class ParallelTrainingJobs(CustomBaseModel):
     current: Annotated[
         Optional[int],
-        Field(description="The number of currently running training jobs"),
+        Field(None, description="The number of currently running training jobs"),
     ] = None
     limit: Annotated[
         Optional[int],
         Field(
-            description="The maximum number of running training jobs at any time. If empty, then there is no limit."
+            None,
+            description="The maximum number of running training jobs at any time. If empty, then there is no limit.",
         ),
     ] = None
 
 
 class ParallelGenerationJobs(CustomBaseModel):
     current: Annotated[
         Optional[int],
-        Field(description="The number of currently running generation jobs"),
+        Field(None, description="The number of currently running generation jobs"),
     ] = None
     limit: Annotated[
         Optional[int],
         Field(
-            description="The maximum number of running generation jobs at any time. If empty, then there is no limit."
+            None,
+            description="The maximum number of running generation jobs at any time. If empty, then there is no limit.",
         ),
     ] = None
 
 
 class UserUsage(CustomBaseModel):
     credits: Optional[Credits] = None
     parallel_training_jobs: Annotated[
-        Optional[ParallelTrainingJobs], Field(alias="parallelTrainingJobs")
+        Optional[ParallelTrainingJobs], Field(None, alias="parallelTrainingJobs")
     ] = None
     parallel_generation_jobs: Annotated[
-        Optional[ParallelGenerationJobs], Field(alias="parallelGenerationJobs")
+        Optional[ParallelGenerationJobs], Field(None, alias="parallelGenerationJobs")
     ] = None
 
 
 class Metadata(CustomBaseModel):
     created_at: Annotated[
-        Optional[datetime],
+        Optional[AwareDatetime],
         Field(
+            None,
             alias="createdAt",
             description="The UTC date and time when the resource has been created.\n",
-            example="2023‐09‐07T18:40:39Z",
+            examples=["2023‐09‐07T18:40:39Z"],
         ),
     ] = None
     owner_id: Annotated[
         Optional[str],
         Field(
+            None,
             alias="ownerId",
             description="The unique identifier of the owner of the entity",
         ),
     ] = None
     owner_name: Annotated[
         Optional[str],
-        Field(alias="ownerName", description="The name of the owner of the entity"),
+        Field(
+            None, alias="ownerName", description="The name of the owner of the entity"
+        ),
     ] = None
     current_user_permission_level: Annotated[
-        Optional[PermissionLevel], Field(alias="currentUserPermissionLevel")
+        Optional[PermissionLevel], Field(None, alias="currentUserPermissionLevel")
     ] = None
 
 
 class PaginatedTotalCount(RootModel[int]):
     root: Annotated[
         int, Field(description="The total number of entities within the list")
     ]
@@ -183,19 +191,22 @@
         ),
     ]
 
 
 class ConnectorUsage(CustomBaseModel):
     no_of_shares: Annotated[
         Optional[int],
-        Field(alias="noOfShares", description="Number of shares of this connector."),
+        Field(
+            None, alias="noOfShares", description="Number of shares of this connector."
+        ),
     ] = None
     no_of_generators: Annotated[
         Optional[int],
         Field(
+            None,
             alias="noOfGenerators",
             description="Number of generators using this connector.",
         ),
     ] = None
 
 
 class ConnectorListItem(CustomBaseModel):
@@ -216,14 +227,15 @@
     secrets: Optional[Dict[str, str]] = None
     ssl: Optional[Dict[str, str]] = None
     metadata: Optional[Metadata] = None
     usage: Optional[ConnectorUsage] = None
     table_id: Annotated[
         Optional[str],
         Field(
+            None,
             alias="tableId",
             description="Optional. ID of a source table or a synthetic table, that this connector belongs to.\nIf not set, then this connector is managed independently of any generator or synthetic dataset.\n",
         ),
     ] = None
     OPEN_URL_PARTS: ClassVar[list] = ["d", "connectors"]
 
     def update(self, config) -> "Connector":
@@ -296,35 +308,40 @@
         return self.client._shares(resource=self)
 
 
 class GeneratorUsage(CustomBaseModel):
     total_datapoints: Annotated[
         Optional[int],
         Field(
+            None,
             alias="totalDatapoints",
             description="The total number of datapoints generated by this generator.",
         ),
     ] = None
     total_compute_time: Annotated[
         Optional[int],
         Field(
+            None,
             alias="totalComputeTime",
             description="The total compute time in seconds used for training this generator. \nThis is the sum of the compute time of all trained tasks.\n",
         ),
     ] = None
     no_of_synthetic_datasets: Annotated[
         Optional[int],
         Field(
+            None,
             alias="noOfSyntheticDatasets",
             description="Number of synthetic datasets generated by this generator.",
         ),
     ] = None
     no_of_shares: Annotated[
         Optional[int],
-        Field(alias="noOfShares", description="Number of shares of this generator."),
+        Field(
+            None, alias="noOfShares", description="Number of shares of this generator."
+        ),
     ] = None
 
 
 class SourceTableData(RootModel[str]):
     root: Annotated[
         str,
         Field(
@@ -390,15 +407,15 @@
         Optional[SourceColumnValueRange], Field(alias="valueRange")
     ] = None
 
 
 class SourceForeignKey(CustomBaseModel):
     id: Annotated[str, Field(description="The unique identifier of a foreign key")]
     column: Annotated[
-        Optional[str], Field(description="The column name of a foreign key.")
+        Optional[str], Field(None, description="The column name of a foreign key.")
     ] = None
     referenced_table: Annotated[
         str,
         Field(
             alias="referencedTable",
             description="The table name of the referenced table. That table must have a primary key already defined.",
         ),
@@ -440,129 +457,144 @@
     """
     The training configuration for a AI model
     """
 
     max_sample_size: Annotated[
         Optional[int],
         Field(
+            None,
             alias="maxSampleSize",
             description="The maximum number of samples to consider for training.\nIf not provided, then all available samples will be taken.\n",
             ge=1,
             le=1000000000,
         ),
     ] = None
     batch_size: Annotated[
         Optional[int],
         Field(
+            None,
             alias="batchSize",
             description="The batch size used for training the model.\nIf not provided, batchSize will be chosen automatically.\n",
             ge=1,
             le=1000000,
         ),
     ] = None
     model_size: Annotated[
         Optional[ModelSize],
         Field(
+            "M",
             alias="modelSize",
             description="The size of the model, with the default being M(edium).\nChoose S(mall) for faster training, or L(arge) for better results for large dataset.\nNote, that larger model sizes will require more memory and more compute.\n",
         ),
     ] = "M"
     max_training_time: Annotated[
         Optional[int],
         Field(
+            10,
             alias="maxTrainingTime",
             description="The maximum number of minutes to train the model.",
             ge=0,
             le=100000,
         ),
     ] = 10
     max_epochs: Annotated[
         Optional[int],
         Field(
+            100,
             alias="maxEpochs",
             description="The maximum number of epochs to train the model.",
             ge=0,
             le=100000,
         ),
     ] = 100
     max_sequence_window: Annotated[
         Optional[int],
         Field(
+            100,
             alias="maxSequenceWindow",
             description="The maximum sequence window to consider for training.",
             ge=1,
             le=100000,
         ),
     ] = 100
     enable_flexible_generation: Annotated[
         Optional[bool],
         Field(
+            True,
             alias="enableFlexibleGeneration",
             description="If true, then the trained generator can be used for rebalancing and imputation.\n",
         ),
     ] = True
     value_protection: Annotated[
         Optional[bool],
         Field(
+            True,
             alias="valueProtection",
             description="Defines if Rare Category, Extreme value, or Sequence length protection will be applied.\n",
         ),
     ] = True
     rare_category_replacement_method: Annotated[
         Optional[RareCategoryReplacementMethod],
         Field(
+            "CONSTANT",
             alias="rareCategoryReplacementMethod",
             description="Specifies, if the rare categories for categoricals will be replaced by a constant \n_RARE_ or by a sample from non-rare categories.\n",
         ),
     ] = "CONSTANT"
 
 
 class Accuracy(CustomBaseModel):
     overall: Annotated[
         Optional[float],
-        Field(description="The overall accuracy of the model.", ge=0.0, le=1.0),
+        Field(None, description="The overall accuracy of the model.", ge=0.0, le=1.0),
     ] = None
     univariate: Annotated[
         Optional[float],
-        Field(description="The univariate accuracy of the model.", ge=0.0, le=1.0),
+        Field(
+            None, description="The univariate accuracy of the model.", ge=0.0, le=1.0
+        ),
     ] = None
     bivariate: Annotated[
         Optional[float],
-        Field(description="The bivariate accuracy of the model.", ge=0.0, le=1.0),
+        Field(None, description="The bivariate accuracy of the model.", ge=0.0, le=1.0),
     ] = None
     coherence: Annotated[
         Optional[float],
         Field(
+            None,
             description="The coherence accuracy of the model, in case of sequential data.",
             ge=0.0,
             le=1.0,
         ),
     ] = None
     overall_max: Annotated[
         Optional[float],
         Field(
+            None,
             alias="overallMax",
             description="The overall accuracy for an actual holdout dataset.\nThis serves as a reference for the overall accuracy of the trained generator.\n",
             ge=0.0,
             le=1.0,
         ),
     ] = None
 
 
 class Distances(CustomBaseModel):
     dcr_original: Annotated[
         Optional[float],
         Field(
+            None,
             alias="dcrOriginal",
             description="The average DCR between the original records.",
         ),
     ] = None
     dcr_synthetic: Annotated[
         Optional[float],
         Field(
+            None,
             alias="dcrSynthetic",
             description="The average DCR between the synthetic and the original records.",
         ),
     ] = None
 
 
 class ModelMetrics(CustomBaseModel):
@@ -612,54 +644,59 @@
     canceled = "CANCELED"
 
 
 class SyntheticDatasetUsage(CustomBaseModel):
     total_datapoints: Annotated[
         Optional[int],
         Field(
+            None,
             alias="totalDatapoints",
             description="The number of datapoints in the synthetic dataset",
         ),
     ] = None
     total_credits: Annotated[
         Optional[float],
         Field(
+            None,
             alias="totalCredits",
             description="The number of credits used for the synthetic dataset",
         ),
     ] = None
     total_compute_time: Annotated[
         Optional[int],
         Field(
+            None,
             alias="totalComputeTime",
             description="The total compute time in seconds used for generating this synthetic dataset. \nThis is the sum of the compute time of all trained tasks.\n",
         ),
     ] = None
     no_of_shares: Annotated[
         Optional[int],
         Field(
+            None,
             alias="noOfShares",
             description="Number of shares of this synthetic dataset.",
         ),
     ] = None
 
 
 class SyntheticDatasetListItem(CustomBaseModel):
     id: Annotated[
         str, Field(description="The unique identifier of a synthetic dataset")
     ]
     metadata: Metadata
     name: Annotated[str, Field(description="The name of a synthetic dataset")]
     description: Annotated[
-        Optional[str], Field(description="The description of a synthetic dataset")
+        Optional[str], Field(None, description="The description of a synthetic dataset")
     ] = None
     generation_status: Annotated[ProgressStatus, Field(alias="generationStatus")]
     generation_time: Annotated[
-        Optional[datetime],
+        Optional[AwareDatetime],
         Field(
+            None,
             alias="generationTime",
             description="The UTC date and time when the generation has finished.",
         ),
     ] = None
     usage: Optional[SyntheticDatasetUsage] = None
 
 
@@ -680,71 +717,88 @@
     Only applicable for categorical columns of a subject table.
 
     """
 
     column: Annotated[
         Optional[str],
         Field(
-            description="The name of the column to be rebalanced.\nThat column must be of modelEncodingType CATEGORICAL.\n"
+            None,
+            description="The name of the column to be rebalanced.\nThat column must be of modelEncodingType CATEGORICAL.\n",
         ),
     ] = None
     probabilities: Annotated[
         Optional[Dict[str, float]],
         Field(
+            None,
             description="The target distribution of samples values. \nThe keys are the categorical values, and the values are the probabilities.\n",
-            example=[{"US": 0.8}, {"male": 0.5, "female": 0.5}],
+            examples=[[{"US": 0.8}, {"male": 0.5, "female": 0.5}]],
         ),
     ] = None
 
 
 class SyntheticTableConfiguration(CustomBaseModel):
     """
     The sample configuration for a synthetic table
     """
 
     sample_size: Annotated[
         Optional[int],
         Field(
+            None,
             alias="sampleSize",
             description="Number of generated samples. Only applicable for subject tables.\n",
             ge=1,
         ),
     ] = None
     sample_seed_connector_id: Annotated[
         Optional[str],
         Field(
+            None,
             alias="sampleSeedConnectorId",
             description="The connector id of the seed data for conditional generation. \nOnly applicable for subject tables.\n",
         ),
     ] = None
+    sample_seed_dict: Annotated[
+        Optional[str],
+        Field(
+            None,
+            alias="sampleSeedDict",
+            description="The base64-encoded string derived from a json line file containing the specified sample seed data.\n",
+        ),
+    ] = None
     sample_seed_data: Annotated[
         Optional[str],
         Field(
+            None,
             alias="sampleSeedData",
             description="The base64-encoded string derived from a Parquet file containing the specified sample seed data.\n",
         ),
     ] = None
     sampling_temperature: Annotated[
         Optional[float],
         Field(
+            None,
             alias="samplingTemperature",
             description="temperature for sampling",
             ge=0.0,
             le=10.0,
         ),
     ] = None
     sampling_top_p: Annotated[
         Optional[float],
-        Field(alias="samplingTopP", description="topP for sampling", ge=0.0, le=1.0),
+        Field(
+            None, alias="samplingTopP", description="topP for sampling", ge=0.0, le=1.0
+        ),
     ] = None
     rebalancing: Optional[SyntheticTableRebalancing] = None
     imputation: Annotated[
         Optional[List[str]],
         Field(
-            description="Specify a list of column names that are to be imputed.\nImputed columns will suppress the sampling of NULL values.\n"
+            None,
+            description="Specify a list of column names that are to be imputed.\nImputed columns will suppress the sampling of NULL values.\n",
         ),
     ] = None
 
 
 class SyntheticTableName(RootModel[str]):
     root: Annotated[
         str,
@@ -770,27 +824,31 @@
             description="If true, then the foreign key will be considered as a context relation.\nNote, that only one foreign key relation per table can be a context relation.\n",
         ),
     ]
 
 
 class SyntheticTable(CustomBaseModel):
     id: Annotated[
-        Optional[str], Field(description="The unique identifier of a synthetic table")
+        Optional[str],
+        Field(None, description="The unique identifier of a synthetic table"),
     ] = None
     name: Annotated[
         Optional[str],
         Field(
-            description="The name of a source table. It must be unique within a generator."
+            None,
+            description="The name of a source table. It must be unique within a generator.",
         ),
     ] = None
     configuration: Optional[SyntheticTableConfiguration] = None
-    model_metrics: Annotated[Optional[ModelMetrics], Field(alias="modelMetrics")] = None
+    model_metrics: Annotated[
+        Optional[ModelMetrics], Field(None, alias="modelMetrics")
+    ] = None
     foreign_keys: Annotated[
         Optional[List[ForeignKey]],
-        Field(alias="foreignKeys", description="The foreign keys of this table."),
+        Field(None, alias="foreignKeys", description="The foreign keys of this table."),
     ] = None
 
 
 class SyntheticDatasetDelivery(CustomBaseModel):
     overwrite_tables: Annotated[
         bool,
         Field(
@@ -808,109 +866,126 @@
     location: Annotated[
         str, Field(description="The location for the destination connector.")
     ]
 
 
 class BaseResource(CustomBaseModel):
     id: Annotated[
-        Optional[str], Field(description="The unique identifier of the entity")
+        Optional[str], Field(None, description="The unique identifier of the entity")
+    ] = None
+    name: Annotated[
+        Optional[str], Field(None, description="The name of the entity")
     ] = None
-    name: Annotated[Optional[str], Field(description="The name of the entity")] = None
     uri: Annotated[
         Optional[str],
         Field(
+            None,
             description="The API service endpoint of the entity",
-            example="/generators/94c77249-42bf-443a-8e17-6e18a19d60b8",
+            examples=["/generators/94c77249-42bf-443a-8e17-6e18a19d60b8"],
         ),
     ] = None
     current_user_permission_level: Annotated[
-        Optional[PermissionLevel], Field(alias="currentUserPermissionLevel")
+        Optional[PermissionLevel], Field(None, alias="currentUserPermissionLevel")
     ] = None
 
 
 class User(CustomBaseModel):
     id: Annotated[
-        Optional[str], Field(description="The unique identifier of a user")
+        Optional[str], Field(None, description="The unique identifier of a user")
     ] = None
-    name: Annotated[Optional[str], Field(description="The name of a user")] = None
-    email: Annotated[Optional[str], Field(description="The email of a user")] = None
+    name: Annotated[Optional[str], Field(None, description="The name of a user")] = None
+    email: Annotated[Optional[str], Field(None, description="The email of a user")] = (
+        None
+    )
 
 
 class CurrentUser(CustomBaseModel):
     id: Annotated[
-        Optional[str], Field(description="The unique identifier of a user")
+        Optional[str], Field(None, description="The unique identifier of a user")
     ] = None
-    name: Annotated[Optional[str], Field(description="The name of a user")] = None
-    email: Annotated[Optional[str], Field(description="The email of a user")] = None
+    name: Annotated[Optional[str], Field(None, description="The name of a user")] = None
+    email: Annotated[Optional[str], Field(None, description="The email of a user")] = (
+        None
+    )
     settings: Optional[Dict[str, Any]] = None
     usage: Optional[UserUsage] = None
 
 
 class GeneratorListItem(CustomBaseModel):
     id: Annotated[str, Field(description="The unique identifier of a generator")]
-    name: Annotated[Optional[str], Field(description="The name of a generator")] = None
+    name: Annotated[
+        Optional[str], Field(None, description="The name of a generator")
+    ] = None
     description: Annotated[
-        Optional[str], Field(description="The description of a generator")
+        Optional[str], Field(None, description="The description of a generator")
     ] = None
     training_status: Annotated[ProgressStatus, Field(alias="trainingStatus")]
     training_time: Annotated[
-        Optional[datetime],
+        Optional[AwareDatetime],
         Field(
+            None,
             alias="trainingTime",
             description="The UTC date and time when the training has finished.",
         ),
     ] = None
     usage: Optional[GeneratorUsage] = None
     metadata: Metadata
     accuracy: Annotated[
         Optional[float],
         Field(
-            description="The overall accuracy of the trained generator.\nThis is the average of the overall accuracy scores of all trained models.\n"
+            None,
+            description="The overall accuracy of the trained generator.\nThis is the average of the overall accuracy scores of all trained models.\n",
         ),
     ] = None
 
 
 class SourceTable(CustomBaseModel):
     id: Annotated[str, Field(description="The unique identifier of a source table")]
     source_connector: Annotated[
-        Optional[BaseResource], Field(alias="sourceConnector")
+        Optional[BaseResource], Field(None, alias="sourceConnector")
     ] = None
     location: Annotated[
         Optional[str],
         Field(
-            description="The location of a source table. Together with the source connector it uniquely\nidentifies a source, and samples data from there.\n"
+            None,
+            description="The location of a source table. Together with the source connector it uniquely\nidentifies a source, and samples data from there.\n",
         ),
     ] = None
     name: Annotated[
         str,
         Field(
             description="The name of a source table. It must be unique within a generator."
         ),
     ]
     primary_key: Annotated[
         Optional[str],
-        Field(alias="primaryKey", description="The column name of the primary key"),
+        Field(
+            None, alias="primaryKey", description="The column name of the primary key"
+        ),
     ] = None
     columns: Annotated[
         List[SourceColumn], Field(description="The columns of this generator table.")
     ]
     foreign_keys: Annotated[
         Optional[List[SourceForeignKey]],
-        Field(alias="foreignKeys", description="The foreign keys of a table."),
+        Field(None, alias="foreignKeys", description="The foreign keys of a table."),
+    ] = None
+    model_metrics: Annotated[
+        Optional[ModelMetrics], Field(None, alias="modelMetrics")
     ] = None
-    model_metrics: Annotated[Optional[ModelMetrics], Field(alias="modelMetrics")] = None
     model_configuration: Annotated[
-        Optional[ModelConfiguration], Field(alias="modelConfiguration")
+        Optional[ModelConfiguration], Field(None, alias="modelConfiguration")
     ] = None
     text_model_configuration: Annotated[
-        Optional[ModelConfiguration], Field(alias="textModelConfiguration")
+        Optional[ModelConfiguration], Field(None, alias="textModelConfiguration")
     ] = None
     total_rows: Annotated[
         Optional[int],
         Field(
+            None,
             alias="totalRows",
             description="The total number of rows in the source table while fetching data for training.\n",
         ),
     ] = None
 
     def model_qa_report(self):
         if self.client and hasattr(self.client, "model_qa_report"):
@@ -955,39 +1030,49 @@
             return self.client.delete_foreign_key(
                 generator_id=self.extra_key_values["generator_id"],
                 table_id=self.id,
                 **kwargs,
             )
 
 
+class Probe(CustomBaseModel):
+    name: Annotated[Optional[str], Field(None, description="The name of the table")] = (
+        None
+    )
+    rows: Optional[List[Dict[str, Any]]] = None
+
+
 class ProgressStep(CustomBaseModel):
     id: Optional[str] = None
     model_label: Annotated[
         Optional[str],
         Field(
+            None,
             alias="modelLabel",
             description="The unique label for the model, consisting of table name and an optional suffix for text model.\nThis will be empty for steps that are not related to a model.\n",
-            example=["census", "census:text"],
+            examples=[["census", "census:text"]],
         ),
     ] = None
-    step_code: Annotated[Optional[StepCode], Field(alias="stepCode")] = None
+    step_code: Annotated[Optional[StepCode], Field(None, alias="stepCode")] = None
     start_date: Annotated[
-        Optional[datetime],
+        Optional[AwareDatetime],
         Field(
+            None,
             alias="startDate",
             description="The UTC date and time when the job has started.\nIf the job has not started yet, then this is None.\n",
-            example="2024-01-25T12:34:56Z",
+            examples=["2024-01-25T12:34:56Z"],
         ),
     ] = None
     end_date: Annotated[
-        Optional[datetime],
+        Optional[AwareDatetime],
         Field(
+            None,
             alias="endDate",
             description="The UTC date and time when the job has ended. \nIf the job is still, then this is None.\n",
-            example="2024-01-25T12:34:56Z",
+            examples=["2024-01-25T12:34:56Z"],
         ),
     ] = None
     messages: Optional[List[Dict[str, Any]]] = None
     progress: Optional[ProgressValue] = None
     status: Optional[ProgressStatus] = None
 
 
@@ -995,33 +1080,35 @@
     id: Annotated[
         str, Field(description="The unique identifier of a synthetic dataset")
     ]
     generator: Optional[BaseResource] = None
     metadata: Metadata
     name: Annotated[str, Field(description="The name of a synthetic dataset")]
     description: Annotated[
-        Optional[str], Field(description="The description of a synthetic dataset")
+        Optional[str], Field(None, description="The description of a synthetic dataset")
     ] = None
     generation_status: Annotated[ProgressStatus, Field(alias="generationStatus")]
     generation_time: Annotated[
-        Optional[datetime],
+        Optional[AwareDatetime],
         Field(
+            None,
             alias="generationTime",
             description="The UTC date and time when the generation has finished.",
         ),
     ] = None
     tables: Annotated[
         Optional[List[SyntheticTable]],
-        Field(description="The tables of this synthetic dataset."),
+        Field(None, description="The tables of this synthetic dataset."),
     ] = None
     delivery: Optional[SyntheticDatasetDelivery] = None
     accuracy: Annotated[
         Optional[float],
         Field(
-            description="The overall accuracy of the trained generator.\nThis is the average of the overall accuracy scores of all trained models.\n"
+            None,
+            description="The overall accuracy of the trained generator.\nThis is the average of the overall accuracy scores of all trained models.\n",
         ),
     ] = None
     usage: Optional[SyntheticDatasetUsage] = None
     OPEN_URL_PARTS: ClassVar[list] = ["d", "synthetic-datasets"]
     generation: Annotated[Optional[Any], Field(exclude=True)] = None
 
     def __init__(self, *args, **kwargs):
@@ -1113,55 +1200,61 @@
             """
             Retrieve job progress of generation
             """
             return self.synthetic_dataset.client._generation_progress(
                 self.synthetic_dataset.id
             )
 
-        def wait(self, interval: float = 2) -> "SyntheticDataset":
+        def wait(self, progress_bar: bool, interval: float = 2) -> "SyntheticDataset":
             """
             Poll generation progress and loop until generation has completed
 
+            :param progress_bar: If true, then the progress bar will be displayed.
             :param interval: The interval in seconds to poll the job progress
             """
             return self.synthetic_dataset.client._generation_wait(
-                self.synthetic_dataset.id, interval=interval
+                self.synthetic_dataset.id, progress_bar=progress_bar, interval=interval
             )
 
 
 class Share(User):
     permission_level: Annotated[
-        Optional[PermissionLevel], Field(alias="permissionLevel")
+        Optional[PermissionLevel], Field(None, alias="permissionLevel")
     ] = None
 
 
 class Generator(CustomBaseModel):
     id: Annotated[str, Field(description="The unique identifier of a generator")]
-    name: Annotated[Optional[str], Field(description="The name of a generator")] = None
+    name: Annotated[
+        Optional[str], Field(None, description="The name of a generator")
+    ] = None
     description: Annotated[
-        Optional[str], Field(description="The description of a generator")
+        Optional[str], Field(None, description="The description of a generator")
     ] = None
     training_status: Annotated[ProgressStatus, Field(alias="trainingStatus")]
     training_time: Annotated[
-        Optional[datetime],
+        Optional[AwareDatetime],
         Field(
+            None,
             alias="trainingTime",
             description="The UTC date and time when the training has finished.",
         ),
     ] = None
     usage: Optional[GeneratorUsage] = None
     metadata: Metadata
     accuracy: Annotated[
         Optional[float],
         Field(
-            description="The overall accuracy of the trained generator.\nThis is the average of the overall accuracy scores of all trained models.\n"
+            None,
+            description="The overall accuracy of the trained generator.\nThis is the average of the overall accuracy scores of all trained models.\n",
         ),
     ] = None
     tables: Annotated[
-        Optional[List[SourceTable]], Field(description="The tables of this generator")
+        Optional[List[SourceTable]],
+        Field(None, description="The tables of this generator"),
     ] = None
     OPEN_URL_PARTS: ClassVar[list] = ["d", "generators"]
     training: Annotated[Optional[Any], Field(exclude=True)] = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.training = self.Training(self)
@@ -1211,22 +1304,23 @@
 
         def progress(self) -> JobProgress:
             """
             Retrieve job progress of training
             """
             return self.generator.client._training_progress(self.generator.id)
 
-        def wait(self, interval: float = 2) -> "Generator":
+        def wait(self, progress_bar: bool, interval: float = 2) -> "Generator":
             """
             Poll training progress and loop until training has completed
 
+            :param progress_bar: If true, then the progress bar will be displayed.
             :param interval: The interval in seconds to poll the job progress
             """
             return self.generator.client._training_wait(
-                self.generator.id, interval=interval
+                self.generator.id, progress_bar=progress_bar, interval=interval
             )
 
         def list_synthetic_dataset(self) -> list["SyntheticDataset"]:
             """
             List synthetic datasets
 
             List the synthetic datasets that were created based on this generator.
@@ -1237,25 +1331,27 @@
             # return self.generator.client._list_synthetic_datasets(self.generator.id)
             pass
 
 
 class JobProgress(CustomBaseModel):
     id: Optional[str] = None
     start_date: Annotated[
-        Optional[datetime],
+        Optional[AwareDatetime],
         Field(
+            None,
             alias="startDate",
             description="The UTC date and time when the job has started.\nIf the job has not started yet, then this is None.\n",
-            example="2024-01-25T12:34:56Z",
+            examples=["2024-01-25T12:34:56Z"],
         ),
     ] = None
     end_date: Annotated[
-        Optional[datetime],
+        Optional[AwareDatetime],
         Field(
+            None,
             alias="endDate",
             description="The UTC date and time when the job has ended. \nIf the job is still, then this is None.\n",
-            example="2024-01-25T12:34:56Z",
+            examples=["2024-01-25T12:34:56Z"],
         ),
     ] = None
     progress: Optional[ProgressValue] = None
     status: Optional[ProgressStatus] = None
     steps: Optional[List[ProgressStep]] = None
```

### Comparing `mostlyai-0.3.5/mostlyai/shares.py` & `mostlyai-0.3.6/mostlyai/shares.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.5/mostlyai/synthetic_datasets.py` & `mostlyai-0.3.6/mostlyai/synthetic_datasets.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import io
 import re
 import zipfile
-from pathlib import Path
 from typing import Any, Iterator, Optional, Union
 
 import pandas as pd
 
 from mostlyai.base import DELETE, GET, PATCH, POST, Paginator, _MostlyBaseClient
 from mostlyai.model import JobProgress, SyntheticDataset, SyntheticDatasetFormat
-from mostlyai.utils import _convert_df_to_base64, _job_wait, _read_table_from_path
+from mostlyai.utils import _job_wait
 
 
 class _MostlySyntheticDatasetsClient(_MostlyBaseClient):
     SECTION = ["synthetic-datasets"]
 
     # PUBLIC METHODS #
 
@@ -63,37 +62,14 @@
         Create synthetic dataset
 
         See SyntheticDataset.config for the structure of the parameters.
 
         :param config: The configuration parameters of the synthetic dataset to be created.
         :return: The created synthetic dataset.
         """
-        # convert `sample_seed_data` to base64-encoded Parquet files
-        tables = config["tables"] if "tables" in config else []
-        for table in tables:
-            if (
-                "sampleSeedData" in table["configuration"]
-                and table["configuration"]["sampleSeedData"] is not None
-            ):
-                if isinstance(table["configuration"]["sampleSeedData"], pd.DataFrame):
-                    table["configuration"]["sampleSeedData"] = _convert_df_to_base64(
-                        table["configuration"]["sampleSeedData"]
-                    )
-                elif isinstance(table["configuration"]["sampleSeedData"], (Path, str)):
-                    _, df = _read_table_from_path(
-                        table["configuration"]["sampleSeedData"]
-                    )
-                    table["configuration"]["sampleSeedData"] = _convert_df_to_base64(df)
-                    del df
-                else:
-                    raise ValueError(
-                        "sampleSeedData must be a DataFrame or a file path"
-                    )
-        # convert generator_id to str
-        config["generatorId"] = str(config["generatorId"])
         synthetic_dataset = self.request(
             verb=POST,
             path=[],
             json=dict(config),
             response_type=SyntheticDataset,
         )
         return synthetic_dataset
@@ -182,12 +158,38 @@
             verb=GET,
             path=[synthetic_dataset_id, "generation"],
             response_type=JobProgress,
         )
         return response
 
     def _generation_wait(
-        self, synthetic_dataset_id: str, interval: float
+        self, synthetic_dataset_id: str, progress_bar: bool, interval: float
     ) -> SyntheticDataset:
-        _job_wait(lambda: self._generation_progress(synthetic_dataset_id), interval)
+        _job_wait(
+            lambda: self._generation_progress(synthetic_dataset_id),
+            interval,
+            progress_bar,
+        )
         synthetic_dataset = self.get(synthetic_dataset_id)
         return synthetic_dataset
+
+
+class _MostlySyntheticProbesClient(_MostlyBaseClient):
+    SECTION = ["synthetic-probes"]
+
+    def create(
+        self, config: dict[str, Any]
+    ) -> Union[pd.DataFrame, dict[str, pd.DataFrame]]:
+        """
+        Create synthetic probe
+
+        See SyntheticDataset.config for the structure of the parameters.
+
+        :param config: The configuration parameters of the synthetic dataset to be created.
+        :return: The created synthetic dataset.
+        """
+        dicts = self.request(
+            verb=POST,
+            path=[],
+            json=dict(config),
+        )
+        return {dct["name"]: pd.DataFrame(dct["rows"]) for dct in dicts}
```

### Comparing `mostlyai-0.3.5/pyproject.toml` & `mostlyai-0.3.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 [tool.poetry]
 name = "mostlyai"
-version = "0.3.5"
+version = "0.3.6"
 description = "The official Python client for the MOSTLY AI platform."
 homepage = "https://app.mostly.ai/"
 authors = ["MOSTLY AI <office@mostly.ai>"]
 license = "Proprietary"
 readme = "README.md"
 packages = [
     { include = "mostlyai" }
 ]
 exclude = ["tools/", "tools/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^2.4.2"
-httpx = "^0.25.1"
+httpx = ">=0.25.0"
 pandas = ">=1.5.3,<2.0.0 || ^2.0.0"
-pyarrow = "^14.0.2"
-rich = "^13.7.0"
+pyarrow = ">=14.0.0"
+rich = ">=13.7.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.0.0"
-mypy = "^0.931"
-pylint = "^2.12.2"
-isort = "^5.10.1"
-black = "^24.4.0"
 pre-commit = "^2.17.0"
-datamodel-code-generator = { version = "^0.22.0", extras = ["http"] }
-
-[tool.poetry.group.dev.dependencies]
+datamodel-code-generator = { version = "^0.25.0", extras = ["http"] }
 vcrpy = "^5.1.0"
-ruff = "^0.2.2"
+ruff = "0.4.4"
 respx = "^0.20.2"
 twine = "^5.0.0"
 commitizen = "^3.18.0"
 mkdocs = "^1.5.3"
 mkdocstrings = "^0.24.1"
 mkdocs-material = "^9.5.13"
```

### Comparing `mostlyai-0.3.5/PKG-INFO` & `mostlyai-0.3.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mostlyai
-Version: 0.3.5
+Version: 0.3.6
 Summary: The official Python client for the MOSTLY AI platform.
 Home-page: https://app.mostly.ai/
 License: Proprietary
 Author: MOSTLY AI
 Author-email: office@mostly.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: httpx (>=0.25.1,<0.26.0)
+Requires-Dist: httpx (>=0.25.0)
 Requires-Dist: pandas (>=1.5.3,<3.0.0)
-Requires-Dist: pyarrow (>=14.0.2,<15.0.0)
+Requires-Dist: pyarrow (>=14.0.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
-Requires-Dist: rich (>=13.7.0,<14.0.0)
+Requires-Dist: rich (>=13.7.0)
 Description-Content-Type: text/markdown
 
 # MOSTLY AI - GenAI for Tabular Data
 
 A Python wrapper for the MOSTLY AI platform (https://app.mostly.ai/).
 
 | Intent                                          | Primitive                  |
@@ -40,15 +40,15 @@
 ```shell
 pip install mostlyai
 ```
 
 ## Basic Usage
 ```python
 from mostlyai import MostlyAI
-mostly = MostlyAI(api_key='your_api_key') 
+mostly = MostlyAI(api_key='your_api_key')
 g = mostly.train(data)      # train a generator on your data
 sd = mostly.generate(g)     # generate a synthetic dataset
 syn = sd.data()             # consume synthetic as pd.DataFrame
 ```
 
 ## Supported Methods
 
@@ -109,14 +109,21 @@
 sd.generation.cancel()
 sd.generation.wait()
 
 sd.data()
 sd.download(file, format)
 ```
 
+### Synthetic Probes
+```python
+sp = mostly.probe(g, seed=seed)
+sp = mostly.probe(g, size=size)
+sp = mostly.probe(g, config=config)
+```
+
 ### Sharing
 
 ```python
 mostly.share(g | sd | c, email)
 mostly.unshare(g | sd | c, email)
 
 g.shares()
```

