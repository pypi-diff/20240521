# Comparing `tmp/dbt_ibmdb2-1.7.0.tar.gz` & `tmp/dbt_ibmdb2-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_ibmdb2-1.7.0.tar", max compression
+gzip compressed data, was "dbt_ibmdb2-1.8.0.tar", max compression
```

## Comparing `dbt_ibmdb2-1.7.0.tar` & `dbt_ibmdb2-1.8.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    10379 2024-03-06 07:04:49.116729 dbt_ibmdb2-1.7.0/LICENSE
--rw-r--r--   0        0        0     5120 2024-03-06 07:04:49.116729 dbt_ibmdb2-1.7.0/README.md
--rw-r--r--   0        0        0      383 2024-03-06 07:04:49.116729 dbt_ibmdb2-1.7.0/dbt/adapters/ibmdb2/__init__.py
--rw-r--r--   0        0        0       17 2024-03-06 07:04:49.116729 dbt_ibmdb2-1.7.0/dbt/adapters/ibmdb2/__version__.py
--rw-r--r--   0        0        0     1401 2024-03-06 07:04:49.116729 dbt_ibmdb2-1.7.0/dbt/adapters/ibmdb2/column.py
--rw-r--r--   0        0        0     3494 2024-03-06 07:04:49.116729 dbt_ibmdb2-1.7.0/dbt/adapters/ibmdb2/connections.py
--rw-r--r--   0        0        0     3854 2024-03-06 07:04:49.116729 dbt_ibmdb2-1.7.0/dbt/adapters/ibmdb2/impl.py
--rw-r--r--   0        0        0      809 2024-03-06 07:04:49.116729 dbt_ibmdb2-1.7.0/dbt/adapters/ibmdb2/relation.py
--rw-r--r--   0        0        0       51 2024-03-06 07:04:49.116729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/__init__.py
--rw-r--r--   0        0        0      137 2024-03-06 07:04:49.116729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/dbt_project.yml
--rw-r--r--   0        0        0     6911 2024-03-06 07:04:49.116729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/adapters.sql
--rw-r--r--   0        0        0      695 2024-03-06 07:04:49.120729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/apply_grants.sql
--rw-r--r--   0        0        0     1661 2024-03-06 07:04:49.120729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/catalog.sql
--rw-r--r--   0        0        0     4368 2024-03-06 07:04:49.120729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/materializations/incremental/incremental.sql
--rw-r--r--   0        0        0       98 2024-03-06 07:04:49.120729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/materializations/seeds/helpers.sql
--rw-r--r--   0        0        0     2524 2024-03-06 07:04:49.120729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/materializations/table/table.sql
--rw-r--r--   0        0        0     3163 2024-03-06 07:04:49.120729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/materializations/view/view.sql
--rw-r--r--   0        0        0       59 2024-03-06 07:04:49.120729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/utils/datatypes.sql
--rw-r--r--   0        0        0      173 2024-03-06 07:04:49.120729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/utils/dateadd.sql
--rw-r--r--   0        0        0     1353 2024-03-06 07:04:49.120729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/utils/datediff.sql
--rw-r--r--   0        0        0       74 2024-03-06 07:04:49.120729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/utils/hash.sql
--rw-r--r--   0        0        0      525 2024-03-06 07:04:49.120729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/utils/last_day.sql
--rw-r--r--   0        0        0      148 2024-03-06 07:04:49.120729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/utils/position.sql
--rw-r--r--   0        0        0     1165 2024-03-06 07:04:49.120729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/utils/split_part.sql
--rw-r--r--   0        0        0      429 2024-03-06 07:04:49.120729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/utils/timestamps.sql
--rw-r--r--   0        0        0      545 2024-03-06 07:04:49.120729 dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/sample_profiles.yml
--rw-r--r--   0        0        0      687 2024-03-06 07:25:16.914813 dbt_ibmdb2-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     5962 1970-01-01 00:00:00.000000 dbt_ibmdb2-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0    10379 2024-05-21 18:50:50.480071 dbt_ibmdb2-1.8.0/LICENSE
+-rw-r--r--   0        0        0     5120 2024-05-21 18:50:50.480071 dbt_ibmdb2-1.8.0/README.md
+-rw-r--r--   0        0        0      383 2024-05-21 18:50:50.480071 dbt_ibmdb2-1.8.0/dbt/adapters/ibmdb2/__init__.py
+-rw-r--r--   0        0        0       17 2024-05-21 18:50:50.480071 dbt_ibmdb2-1.8.0/dbt/adapters/ibmdb2/__version__.py
+-rw-r--r--   0        0        0     1401 2024-05-21 18:50:50.480071 dbt_ibmdb2-1.8.0/dbt/adapters/ibmdb2/column.py
+-rw-r--r--   0        0        0     3591 2024-05-21 18:50:50.480071 dbt_ibmdb2-1.8.0/dbt/adapters/ibmdb2/connections.py
+-rw-r--r--   0        0        0     3868 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/adapters/ibmdb2/impl.py
+-rw-r--r--   0        0        0      818 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/adapters/ibmdb2/relation.py
+-rw-r--r--   0        0        0       51 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/__init__.py
+-rw-r--r--   0        0        0      137 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/dbt_project.yml
+-rw-r--r--   0        0        0     6911 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/adapters.sql
+-rw-r--r--   0        0        0      695 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/apply_grants.sql
+-rw-r--r--   0        0        0     1661 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/catalog.sql
+-rw-r--r--   0        0        0     4368 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0        0        0       98 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0        0        0     2524 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/materializations/table/table.sql
+-rw-r--r--   0        0        0     3163 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/materializations/view/view.sql
+-rw-r--r--   0        0        0       59 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/utils/datatypes.sql
+-rw-r--r--   0        0        0      173 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/utils/dateadd.sql
+-rw-r--r--   0        0        0     1353 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/utils/datediff.sql
+-rw-r--r--   0        0        0       74 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/utils/hash.sql
+-rw-r--r--   0        0        0      525 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/utils/last_day.sql
+-rw-r--r--   0        0        0      148 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/utils/position.sql
+-rw-r--r--   0        0        0     1165 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/utils/split_part.sql
+-rw-r--r--   0        0        0      429 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/utils/timestamps.sql
+-rw-r--r--   0        0        0      545 2024-05-21 18:50:50.484071 dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/sample_profiles.yml
+-rw-r--r--   0        0        0      693 2024-05-21 19:12:26.271384 dbt_ibmdb2-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5959 1970-01-01 00:00:00.000000 dbt_ibmdb2-1.8.0/PKG-INFO
```

### Comparing `dbt_ibmdb2-1.7.0/LICENSE` & `dbt_ibmdb2-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_ibmdb2-1.7.0/README.md` & `dbt_ibmdb2-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt_ibmdb2-1.7.0/dbt/adapters/ibmdb2/column.py` & `dbt_ibmdb2-1.8.0/dbt/adapters/ibmdb2/column.py`

 * *Files identical despite different names*

### Comparing `dbt_ibmdb2-1.7.0/dbt/adapters/ibmdb2/connections.py` & `dbt_ibmdb2-1.8.0/dbt/adapters/ibmdb2/connections.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from contextlib import contextmanager
 
 from dataclasses import dataclass
 
-import dbt.exceptions
-from dbt.adapters.base import Credentials
-from dbt.contracts.connection import AdapterResponse
-from dbt.contracts.connection import Connection
+import dbt_common.exceptions
+from dbt.adapters.contracts.connection import Credentials
+from dbt.adapters.contracts.connection import AdapterResponse
+from dbt.adapters.contracts.connection import Connection
 from dbt.adapters.sql import SQLConnectionManager
-from dbt.logger import GLOBAL_LOGGER as logger
+from dbt.adapters.events.logging import AdapterLogger
 
 from typing import (
     Type,
     Iterable,
     Optional
 )
 
 import ibm_db
 import ibm_db_dbi
 
+logger = AdapterLogger("IBM DB2")
+
 @dataclass
 class IBMDB2Credentials(Credentials):
     host: str
     database: str
     schema: str
     user: str
     password: str
@@ -47,20 +49,20 @@
     def exception_handler(self, sql: str):
         try:
             yield
         except ibm_db_dbi.DatabaseError as exc:
             self.release()
             logger.debug('ibm_db_dbi error: {}'.format(str(exc)))
             logger.debug("Error running SQL: {}".format(sql))
-            raise dbt.exceptions.DbtDatabaseError(str(exc))
+            raise dbt_common.exceptions.DbtDatabaseError(str(exc))
         except Exception as exc:
             self.release()
             logger.debug("Error running SQL: {}".format(sql))
             logger.debug("Rolling back transaction.")
-            raise dbt.exceptions.DbtRuntimeError(str(exc))
+            raise dbt_common.exceptions.DbtRuntimeError(str(exc))
 
     @classmethod
     def open(cls, connection):
         if connection.state == 'open':
             logger.debug('Connection is already open, skipping open.')
             return connection
```

### Comparing `dbt_ibmdb2-1.7.0/dbt/adapters/ibmdb2/impl.py` & `dbt_ibmdb2-1.8.0/dbt/adapters/ibmdb2/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dbt.adapters.sql import SQLAdapter
 from dbt.adapters.ibmdb2 import IBMDB2ConnectionManager
 from dbt.adapters.ibmdb2.relation import IBMDB2Relation
 from dbt.adapters.ibmdb2.column import IBMDB2Column
 
 from typing import Dict
-from dbt.utils import filter_null_values
-from dbt.exceptions import CompilationError
+from dbt_common.utils import filter_null_values
+from dbt_common.exceptions import CompilationError
 from dbt.adapters.base.meta import available
 from typing import Optional
 
 import agate
 
 
 class IBMDB2Adapter(SQLAdapter):
```

### Comparing `dbt_ibmdb2-1.7.0/dbt/adapters/ibmdb2/relation.py` & `dbt_ibmdb2-1.8.0/dbt/adapters/ibmdb2/relation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass, field
 from dbt.adapters.base.relation import BaseRelation, Policy
 
 from typing import Optional, TypeVar, Type
-from dbt.contracts.relation import RelationType
+from dbt.adapters.contracts.relation import RelationType
 
 
 @dataclass
 class IBMDB2QuotePolicy(Policy):
     database: bool = False
     schema: bool = False
     identifier: bool = False
```

### Comparing `dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/adapters.sql` & `dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/apply_grants.sql` & `dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/catalog.sql` & `dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/materializations/incremental/incremental.sql` & `dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/materializations/table/table.sql` & `dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/materializations/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/materializations/view/view.sql` & `dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/materializations/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/utils/datediff.sql` & `dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/utils/last_day.sql` & `dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/utils/last_day.sql`

 * *Files identical despite different names*

### Comparing `dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/macros/utils/split_part.sql` & `dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt_ibmdb2-1.7.0/dbt/include/ibmdb2/sample_profiles.yml` & `dbt_ibmdb2-1.8.0/dbt/include/ibmdb2/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt_ibmdb2-1.7.0/pyproject.toml` & `dbt_ibmdb2-1.8.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-ibmdb2"
-version = "1.7.0"
+version = "1.8.0"
 description = "The db2 adapter plugin for dbt (data build tool)"
 authors = ["aurany <rasmus.nyberg@gmail.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/aurany/dbt-ibmdb2"
 keywords = [
     "dbt",
@@ -15,19 +15,19 @@
 ]
 packages = [
     { include = "dbt" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-dbt-core = "~1.7"
+dbt-core = ">=1.8.0"
 ibm-db = "^3.1.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 tox = "^3.25.1"
 python-dotenv = "^0.20.0"
-dbt-tests-adapter = "~1.7"
+dbt-tests-adapter = ">=1.8.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.8"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dbt_ibmdb2-1.7.0/PKG-INFO` & `dbt_ibmdb2-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: dbt-ibmdb2
-Version: 1.7.0
+Version: 1.8.0
 Summary: The db2 adapter plugin for dbt (data build tool)
 Home-page: https://github.com/aurany/dbt-ibmdb2
 License: Apache Software License 2.0
 Keywords: dbt,ibm,db2,data,engineering
 Author: aurany
 Author-email: rasmus.nyberg@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: dbt-core (>=1.7,<1.8)
+Requires-Dist: dbt-core (>=1.8.0)
 Requires-Dist: ibm-db (>=3.1.0,<4.0.0)
 Project-URL: Repository, https://github.com/aurany/dbt-ibmdb2
 Description-Content-Type: text/markdown
 
 [![pypi](https://badge.fury.io/py/dbt-ibmdb2.svg)](https://pypi.org/project/dbt-ibmdb2/)
 [![python](https://img.shields.io/pypi/pyversions/dbt-ibmdb2)](https://pypi.org/project/dbt-ibmdb2/)
```

