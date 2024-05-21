# Comparing `tmp/ebb_time_series-0.3.0.tar.gz` & `tmp/ebb_time_series-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebb_time_series-0.3.0.tar", max compression
+gzip compressed data, was "ebb_time_series-0.3.1.tar", max compression
```

## Comparing `ebb_time_series-0.3.0.tar` & `ebb_time_series-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1067 2024-05-10 22:25:27.000848 ebb_time_series-0.3.0/LICENSE
--rw-r--r--   0        0        0     2264 2024-05-13 22:11:05.101506 ebb_time_series-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-05-10 22:25:27.006306 ebb_time_series-0.3.0/ebb_time_series/__init__.py
--rw-r--r--   0        0        0      431 2024-05-16 21:52:46.364371 ebb_time_series-0.3.0/ebb_time_series/constants.py
--rw-r--r--   0        0        0      233 2024-05-16 16:14:33.959702 ebb_time_series-0.3.0/ebb_time_series/data_schema.py
--rw-r--r--   0        0        0     1195 2024-05-16 16:14:33.959938 ebb_time_series-0.3.0/ebb_time_series/event_parser_helpers.py
--rw-r--r--   0        0        0      305 2024-05-16 21:52:46.364838 ebb_time_series-0.3.0/ebb_time_series/exceptions.py
--rw-r--r--   0        0        0    10159 2024-05-17 17:09:44.320307 ebb_time_series-0.3.0/ebb_time_series/writers/aws_timestream_data_writer.py
--rw-r--r--   0        0        0     2110 2024-05-16 16:14:33.960966 ebb_time_series-0.3.0/ebb_time_series/writers/base_data_writer.py
--rw-r--r--   0        0        0      551 2024-05-17 17:09:44.320624 ebb_time_series-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 ebb_time_series-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-10 22:25:27.000848 ebb_time_series-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2264 2024-05-13 22:11:05.101506 ebb_time_series-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 22:25:27.006306 ebb_time_series-0.3.1/ebb_time_series/__init__.py
+-rw-r--r--   0        0        0      431 2024-05-16 21:52:46.364371 ebb_time_series-0.3.1/ebb_time_series/constants.py
+-rw-r--r--   0        0        0     1191 2024-05-21 19:52:55.984719 ebb_time_series-0.3.1/ebb_time_series/event_parser_helpers.py
+-rw-r--r--   0        0        0      305 2024-05-16 21:52:46.364838 ebb_time_series-0.3.1/ebb_time_series/exceptions.py
+-rw-r--r--   0        0        0    10155 2024-05-21 19:52:55.985110 ebb_time_series-0.3.1/ebb_time_series/writers/aws_timestream_data_writer.py
+-rw-r--r--   0        0        0     2110 2024-05-16 16:14:33.960966 ebb_time_series-0.3.1/ebb_time_series/writers/base_data_writer.py
+-rw-r--r--   0        0        0      551 2024-05-21 19:52:55.985928 ebb_time_series-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 ebb_time_series-0.3.1/PKG-INFO
```

### Comparing `ebb_time_series-0.3.0/LICENSE` & `ebb_time_series-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ebb_time_series-0.3.0/README.md` & `ebb_time_series-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ebb_time_series-0.3.0/ebb_time_series/event_parser_helpers.py` & `ebb_time_series-0.3.1/ebb_time_series/event_parser_helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 from marshmallow import ValidationError
+from ebb_events.event_schema import DataSchema
 from ebb_time_series.constants import DATA_UNITS_FIELDNAME
-from ebb_time_series.data_schema import DataSchema
 
 
 def slugify_name_and_units(variable_name: str, data_dict: dict) -> str:
     """
     Helper returns string name of variable__units combined with double underscore separator.
     If no units are provided, variable name ends with double underscore (my_var__)
```

### Comparing `ebb_time_series-0.3.0/ebb_time_series/writers/aws_timestream_data_writer.py` & `ebb_time_series-0.3.1/ebb_time_series/writers/aws_timestream_data_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import boto3
 import logging
 from botocore.config import Config
 from botocore.exceptions import ClientError
 from enum import Enum
 from ebb_events.consumers.event_consumer import EventConsumer
+from ebb_events.event_schema import DataSchema
 from ebb_time_series.constants import (
     DATA_VALUE_FIELDNAME,
     MAX_ATTEMPTS,
     MAX_POOL_CONNECTIONS,
     ORGANIZATION_FIELDNAME,
     READ_TIMEOUT,
     SYSTEM_FIELDNAME,
     SUBSYSTEM_FIELDNAME,
     DEVICE_FIELDNAME,
     SERIAL_NUMBER_FIELDNAME,
     EVENT_ID_FIELDNAME,
 )
-from ebb_time_series.data_schema import DataSchema
 from ebb_time_series.event_parser_helpers import slugify_name_and_units
 from ebb_time_series.exceptions import TimeSeriesWriteException
 from ebb_time_series.writers.base_data_writer import BaseDataWriter
 from marshmallow import ValidationError
 
 
 class AwsTimestreamFields(Enum):
```

### Comparing `ebb_time_series-0.3.0/ebb_time_series/writers/base_data_writer.py` & `ebb_time_series-0.3.1/ebb_time_series/writers/base_data_writer.py`

 * *Files identical despite different names*

### Comparing `ebb_time_series-0.3.0/pyproject.toml` & `ebb_time_series-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "ebb-time-series"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Ryan Bloom <ryan.bloom@ebbcarbon.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-ebb-events = "^0.3.2"
+ebb-events = "^0.3.4"
 boto3 = "^1.34.103"
 botocore = "^1.34.103"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
 black = "^24.4.0"
 pytest = "^8.1.1"
```

### Comparing `ebb_time_series-0.3.0/PKG-INFO` & `ebb_time_series-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ebb-time-series
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Ryan Bloom
 Author-email: ryan.bloom@ebbcarbon.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.103,<2.0.0)
 Requires-Dist: botocore (>=1.34.103,<2.0.0)
-Requires-Dist: ebb-events (>=0.3.2,<0.4.0)
+Requires-Dist: ebb-events (>=0.3.4,<0.4.0)
 Description-Content-Type: text/markdown
 
 # Ebb Time Series
 EbbCarbon package for working with time series data and databases. Time series data is a type of data that is collected over certain time intervals and is used to analyze trends, patterns, and behavior over time. This `ebb-time-series` package is built to be used in tandem with the [ebb-events](https://pypi.org/project/ebb-events/) package to assist in the flow of time series data from event messages to various time series databases and and to read from various time series databases to export and analyze the data.
 
 For writing to time series databases: Once an event is consumed off of a message broker, use this package to write the event's data to your desired database for storage and further analysis. The combined use of these two EbbCarbon packages will enable you to streamline your data pipeline from edge node all the way to the cloud. NOTE: In order to use this package, the event writers expect to receive `ebb-event EventConsumer` objects with payloads of the `ebb-event` structure.
```

