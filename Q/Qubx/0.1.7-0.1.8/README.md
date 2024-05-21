# Comparing `tmp/qubx-0.1.7.tar.gz` & `tmp/qubx-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qubx-0.1.7.tar", max compression
+gzip compressed data, was "qubx-0.1.8.tar", max compression
```

## Comparing `qubx-0.1.7.tar` & `qubx-0.1.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      940 2024-04-25 07:51:17.473695 qubx-0.1.7/README.md
--rw-r--r--   0        0        0     9305 2024-04-21 10:35:06.164526 qubx-0.1.7/build.py
--rw-r--r--   0        0        0     1555 2024-05-15 12:37:23.844753 qubx-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5428 2024-04-21 10:35:06.176526 qubx-0.1.7/src/qubx/__init__.py
--rw-r--r--   0        0        0     1875 2024-05-12 17:27:41.499398 qubx-0.1.7/src/qubx/_nb_magic.py
--rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.7/src/qubx/core/__init__.py
--rw-r--r--   0        0        0     6707 2024-04-25 07:51:17.477695 qubx-0.1.7/src/qubx/core/account.py
--rw-r--r--   0        0        0    14777 2024-05-07 13:17:10.565607 qubx-0.1.7/src/qubx/core/basics.py
--rw-r--r--   0        0        0    11559 2024-05-07 13:17:10.565607 qubx-0.1.7/src/qubx/core/helpers.py
--rw-r--r--   0        0        0    11910 2024-05-07 13:17:10.565607 qubx-0.1.7/src/qubx/core/loggers.py
--rw-r--r--   0        0        0    13688 2024-04-21 10:35:06.176526 qubx-0.1.7/src/qubx/core/lookups.py
--rw-r--r--   0        0        0     2847 2024-04-21 10:35:06.176526 qubx-0.1.7/src/qubx/core/series.pxd
--rw-r--r--   0        0        0    28108 2024-04-21 10:35:06.176526 qubx-0.1.7/src/qubx/core/series.pyx
--rw-r--r--   0        0        0    30330 2024-05-07 13:17:10.565607 qubx-0.1.7/src/qubx/core/strategy.py
--rw-r--r--   0        0        0     1368 2024-02-29 14:43:31.739720 qubx-0.1.7/src/qubx/core/utils.pyx
--rw-r--r--   0        0        0    23350 2024-05-15 12:37:23.844753 qubx-0.1.7/src/qubx/data/readers.py
--rw-r--r--   0        0        0     9150 2024-05-07 13:17:10.565607 qubx-0.1.7/src/qubx/impl/ccxt_connector.py
--rw-r--r--   0        0        0     3488 2024-05-07 13:17:10.565607 qubx-0.1.7/src/qubx/impl/ccxt_customizations.py
--rw-r--r--   0        0        0     9097 2024-05-07 13:17:10.565607 qubx-0.1.7/src/qubx/impl/ccxt_trading.py
--rw-r--r--   0        0        0     3565 2024-05-07 13:17:10.565607 qubx-0.1.7/src/qubx/impl/ccxt_utils.py
--rw-r--r--   0        0        0       33 2024-02-29 14:43:31.739720 qubx-0.1.7/src/qubx/math/__init__.py
--rw-r--r--   0        0        0     1176 2024-02-29 14:43:31.739720 qubx-0.1.7/src/qubx/math/stats.py
--rw-r--r--   0        0        0      175 2024-05-12 17:27:41.499398 qubx-0.1.7/src/qubx/pandaz/__init__.py
--rw-r--r--   0        0        0    85271 2024-05-12 17:27:41.503398 qubx-0.1.7/src/qubx/pandaz/ta.py
--rw-r--r--   0        0        0    19109 2024-05-12 17:27:41.503398 qubx-0.1.7/src/qubx/pandaz/utils.py
--rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.7/src/qubx/ta/__init__.py
--rw-r--r--   0        0        0     7708 2024-02-29 14:43:31.739720 qubx-0.1.7/src/qubx/ta/indicators.pyx
--rw-r--r--   0        0        0       60 2024-04-21 10:35:06.176526 qubx-0.1.7/src/qubx/trackers/__init__.py
--rw-r--r--   0        0        0     5522 2024-04-21 10:35:06.176526 qubx-0.1.7/src/qubx/trackers/rebalancers.py
--rw-r--r--   0        0        0      273 2024-05-07 13:17:10.569607 qubx-0.1.7/src/qubx/utils/__init__.py
--rw-r--r--   0        0        0    12017 2024-05-14 18:44:12.292214 qubx-0.1.7/src/qubx/utils/_pyxreloader.py
--rw-r--r--   0        0        0    35158 2024-05-07 13:17:10.569607 qubx-0.1.7/src/qubx/utils/charting/mpl_helpers.py
--rw-r--r--   0        0        0    10993 2024-05-12 17:27:41.503398 qubx-0.1.7/src/qubx/utils/marketdata/binance.py
--rw-r--r--   0        0        0     9831 2024-05-12 17:27:41.503398 qubx-0.1.7/src/qubx/utils/misc.py
--rw-r--r--   0        0        0     9306 2024-05-12 17:27:41.503398 qubx-0.1.7/src/qubx/utils/runner.py
--rw-r--r--   0        0        0     4911 2024-05-14 18:44:12.292214 qubx-0.1.7/src/qubx/utils/time.py
--rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 qubx-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      940 2024-04-25 07:51:17.473695 qubx-0.1.8/README.md
+-rw-r--r--   0        0        0     9305 2024-04-21 10:35:06.164526 qubx-0.1.8/build.py
+-rw-r--r--   0        0        0     1555 2024-05-21 12:08:17.509203 qubx-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5428 2024-04-21 10:35:06.176526 qubx-0.1.8/src/qubx/__init__.py
+-rw-r--r--   0        0        0     1875 2024-05-12 17:27:41.499398 qubx-0.1.8/src/qubx/_nb_magic.py
+-rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.8/src/qubx/core/__init__.py
+-rw-r--r--   0        0        0     6707 2024-04-25 07:51:17.477695 qubx-0.1.8/src/qubx/core/account.py
+-rw-r--r--   0        0        0    14777 2024-05-07 13:17:10.565607 qubx-0.1.8/src/qubx/core/basics.py
+-rw-r--r--   0        0        0    11559 2024-05-07 13:17:10.565607 qubx-0.1.8/src/qubx/core/helpers.py
+-rw-r--r--   0        0        0    11910 2024-05-07 13:17:10.565607 qubx-0.1.8/src/qubx/core/loggers.py
+-rw-r--r--   0        0        0    13688 2024-04-21 10:35:06.176526 qubx-0.1.8/src/qubx/core/lookups.py
+-rw-r--r--   0        0        0     2847 2024-04-21 10:35:06.176526 qubx-0.1.8/src/qubx/core/series.pxd
+-rw-r--r--   0        0        0    28108 2024-04-21 10:35:06.176526 qubx-0.1.8/src/qubx/core/series.pyx
+-rw-r--r--   0        0        0    30330 2024-05-07 13:17:10.565607 qubx-0.1.8/src/qubx/core/strategy.py
+-rw-r--r--   0        0        0     1368 2024-02-29 14:43:31.739720 qubx-0.1.8/src/qubx/core/utils.pyx
+-rw-r--r--   0        0        0    24786 2024-05-21 12:08:17.509203 qubx-0.1.8/src/qubx/data/readers.py
+-rw-r--r--   0        0        0     9150 2024-05-07 13:17:10.565607 qubx-0.1.8/src/qubx/impl/ccxt_connector.py
+-rw-r--r--   0        0        0     3488 2024-05-07 13:17:10.565607 qubx-0.1.8/src/qubx/impl/ccxt_customizations.py
+-rw-r--r--   0        0        0     9097 2024-05-07 13:17:10.565607 qubx-0.1.8/src/qubx/impl/ccxt_trading.py
+-rw-r--r--   0        0        0     3565 2024-05-07 13:17:10.565607 qubx-0.1.8/src/qubx/impl/ccxt_utils.py
+-rw-r--r--   0        0        0       33 2024-02-29 14:43:31.739720 qubx-0.1.8/src/qubx/math/__init__.py
+-rw-r--r--   0        0        0     1176 2024-02-29 14:43:31.739720 qubx-0.1.8/src/qubx/math/stats.py
+-rw-r--r--   0        0        0      175 2024-05-12 17:27:41.499398 qubx-0.1.8/src/qubx/pandaz/__init__.py
+-rw-r--r--   0        0        0    85271 2024-05-12 17:27:41.503398 qubx-0.1.8/src/qubx/pandaz/ta.py
+-rw-r--r--   0        0        0    19109 2024-05-12 17:27:41.503398 qubx-0.1.8/src/qubx/pandaz/utils.py
+-rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.8/src/qubx/ta/__init__.py
+-rw-r--r--   0        0        0     7708 2024-02-29 14:43:31.739720 qubx-0.1.8/src/qubx/ta/indicators.pyx
+-rw-r--r--   0        0        0       60 2024-04-21 10:35:06.176526 qubx-0.1.8/src/qubx/trackers/__init__.py
+-rw-r--r--   0        0        0     5522 2024-04-21 10:35:06.176526 qubx-0.1.8/src/qubx/trackers/rebalancers.py
+-rw-r--r--   0        0        0      273 2024-05-07 13:17:10.569607 qubx-0.1.8/src/qubx/utils/__init__.py
+-rw-r--r--   0        0        0    12017 2024-05-14 18:44:12.292214 qubx-0.1.8/src/qubx/utils/_pyxreloader.py
+-rw-r--r--   0        0        0    35158 2024-05-07 13:17:10.569607 qubx-0.1.8/src/qubx/utils/charting/mpl_helpers.py
+-rw-r--r--   0        0        0    10993 2024-05-12 17:27:41.503398 qubx-0.1.8/src/qubx/utils/marketdata/binance.py
+-rw-r--r--   0        0        0     9831 2024-05-12 17:27:41.503398 qubx-0.1.8/src/qubx/utils/misc.py
+-rw-r--r--   0        0        0     9306 2024-05-12 17:27:41.503398 qubx-0.1.8/src/qubx/utils/runner.py
+-rw-r--r--   0        0        0     4911 2024-05-14 18:44:12.292214 qubx-0.1.8/src/qubx/utils/time.py
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 qubx-0.1.8/PKG-INFO
```

### Comparing `qubx-0.1.7/README.md` & `qubx-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/build.py` & `qubx-0.1.8/build.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/pyproject.toml` & `qubx-0.1.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Qubx"
-version = "0.1.7"
+version = "0.1.8"
 description = "Qubx - quantitative trading framework"
 authors = ["Dmitry Marienko <dmitry@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "qubx", from = "src" },
 ]
 repository = "https://github.com/dmarienko/Qubx"
```

### Comparing `qubx-0.1.7/src/qubx/__init__.py` & `qubx-0.1.8/src/qubx/__init__.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/_nb_magic.py` & `qubx-0.1.8/src/qubx/_nb_magic.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/core/account.py` & `qubx-0.1.8/src/qubx/core/account.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/core/basics.py` & `qubx-0.1.8/src/qubx/core/basics.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/core/helpers.py` & `qubx-0.1.8/src/qubx/core/helpers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/core/loggers.py` & `qubx-0.1.8/src/qubx/core/loggers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/core/lookups.py` & `qubx-0.1.8/src/qubx/core/lookups.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/core/series.pxd` & `qubx-0.1.8/src/qubx/core/series.pxd`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/core/series.pyx` & `qubx-0.1.8/src/qubx/core/series.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/core/strategy.py` & `qubx-0.1.8/src/qubx/core/strategy.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/core/utils.pyx` & `qubx-0.1.8/src/qubx/core/utils.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/data/readers.py` & `qubx-0.1.8/src/qubx/data/readers.py`

 * *Files 6% similar despite different names*

```diff
@@ -503,31 +503,33 @@
     return wrapper
 
 
 class QuestDBConnector(DataReader):
     """
     Very first version of QuestDB connector
 
-    # Connect to an existing QuestDB instance
-    >>> db = QuestDBConnector('user=admin password=quest host=localhost port=8812', OhlcvPandasDataProcessor())
-    >>> db.read('BINANCEF.ETHUSDT', '2024-01-01')
+    ### Connect to an existing QuestDB instance
+    >>> db = QuestDBConnector()
+    >>> db.read('BINANCE.UM:ETHUSDT', '2024-01-01', transform=AsPandasFrame())
     """
     _reconnect_tries = 5
     _reconnect_idle = 0.1  # wait seconds before retying
 
-    def __init__(self, connection_url: str) -> None:
+    def __init__(self, host='localhost', user='admin', password='quest', port=8812) -> None:
         self._connection = None
         self._cursor = None
-        self.connection_url = connection_url
+        self._host = host
+        self._port = port
+        self.connection_url = f'user={user} password={password} host={host} port={port}'
         self._connect()
 
     def _connect(self):
-        logger.info("Connecting to QuestDB ...")
         self._connection = pg.connect(self.connection_url, autocommit=True)
         self._cursor = self._connection.cursor()
+        logger.debug(f"Connected to QuestDB at {self._host}:{self._port}")
 
     @_retry
     def read(self, data_id: str, start: str|None=None, stop: str|None=None, 
              transform: DataTransformer = DataTransformer(),
              chunksize=0,  # TODO: use self._cursor.fetchmany in this case !!!!
              timeframe: str='1m') -> Any:
         start, end = handle_start_stop(start, stop)
@@ -538,35 +540,69 @@
 
         names = [d.name for d in self._cursor.description] # type: ignore
         transform.start_transform(data_id, names)
 
         transform.process_data(records)
         return transform.collect()
 
-    def _prepare_data_sql(self, data_id: str, start: str|None, end: str|None, resample: str) -> str:
-        # just a temp hack - actually we need to discuss symbology etc
-        symbol = data_id#.split('.')[-1]
+    @staticmethod
+    def _convert_time_delta_to_qdb_resample_format(c_tf: str):
+        if c_tf:
+            _t = re.match(r'(\d+)(\w+)', c_tf)
+            if _t and len(_t.groups()) > 1:
+                c_tf = f"{_t[1]}{_t[2][0].lower()}"
+        return c_tf 
+
+    def _get_table_name(self, data_id: str, sfx: str='') -> str:
+        """
+        Get table name for data_id
+        data_id can have format <exchange>.<type>:<symbol>
+        for example: 
+            BINANCE.UM:BTCUSDT or BINANCE:BTCUSDT for spot 
+        """
+        _aliases = {'um': 'umfutures', 'cm': 'cmfutures', 'f': 'futures'}
+        table_name = data_id
+        _ss = data_id.split(':')
+        if len(_ss) > 1:
+            _exch, symb = _ss
+            _mktype = 'spot'
+            _ss = _exch.split('.')
+            if len(_ss) > 1:
+                _exch = _ss[0]
+                _mktype = _ss[1]
+            _mktype = _mktype.lower()
+            table_name = '.'.join(filter(lambda x: x, [_exch.lower(), _aliases.get(_mktype, _mktype), symb.lower(), sfx]))
+        return table_name
 
+    def _prepare_data_sql(self, data_id: str, start: str|None, end: str|None, resample: str) -> str:
+        where = ''
         w0 = f"timestamp >= '{start}'" if start else ''
         w1 = f"timestamp <= '{end}'" if end else ''
-        where = f'where {w0} and {w1}' if (w0 and w1) else f"where {(w0 or w1)}"
 
+        # - fix: when no data ranges are provided we must skip empy where keyword
+        if w0 or w1: 
+            where = f'where {w0} and {w1}' if (w0 and w1) else f"where {(w0 or w1)}"
+
+        # - check resample format
+        resample = QuestDBConnector._convert_time_delta_to_qdb_resample_format(resample) if resample else resample
+        _rsmpl = f"SAMPLE by {resample}" if resample else ''
+
+        table_name = self._get_table_name(data_id, 'candles_1m')
         return f"""
                 select timestamp, 
                 first(open) as open, 
                 max(high) as high,
                 min(low) as low,
                 last(close) as close,
                 sum(volume) as volume,
                 sum(quote_volume) as quote_volume,
                 sum(count) as count,
                 sum(taker_buy_volume) as taker_buy_volume,
                 sum(taker_buy_quote_volume) as taker_buy_quote_volume
-                from "{symbol.upper()}" {where}
-                SAMPLE by {resample};
+                from "{table_name}" {where} {_rsmpl};
             """ 
 
     def _prepare_names_sql(self) -> str:
         return "select table_name from tables()"
 
     @_retry
     def get_names(self) -> List[str] :
```

### Comparing `qubx-0.1.7/src/qubx/impl/ccxt_connector.py` & `qubx-0.1.8/src/qubx/impl/ccxt_connector.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/impl/ccxt_customizations.py` & `qubx-0.1.8/src/qubx/impl/ccxt_customizations.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/impl/ccxt_trading.py` & `qubx-0.1.8/src/qubx/impl/ccxt_trading.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/impl/ccxt_utils.py` & `qubx-0.1.8/src/qubx/impl/ccxt_utils.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/math/stats.py` & `qubx-0.1.8/src/qubx/math/stats.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/pandaz/ta.py` & `qubx-0.1.8/src/qubx/pandaz/ta.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/pandaz/utils.py` & `qubx-0.1.8/src/qubx/pandaz/utils.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/ta/indicators.pyx` & `qubx-0.1.8/src/qubx/ta/indicators.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/trackers/rebalancers.py` & `qubx-0.1.8/src/qubx/trackers/rebalancers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/utils/_pyxreloader.py` & `qubx-0.1.8/src/qubx/utils/_pyxreloader.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/utils/charting/mpl_helpers.py` & `qubx-0.1.8/src/qubx/utils/charting/mpl_helpers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/utils/marketdata/binance.py` & `qubx-0.1.8/src/qubx/utils/marketdata/binance.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/utils/misc.py` & `qubx-0.1.8/src/qubx/utils/misc.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/utils/runner.py` & `qubx-0.1.8/src/qubx/utils/runner.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/src/qubx/utils/time.py` & `qubx-0.1.8/src/qubx/utils/time.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.7/PKG-INFO` & `qubx-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Qubx
-Version: 0.1.7
+Version: 0.1.8
 Summary: Qubx - quantitative trading framework
 Home-page: https://github.com/dmarienko/Qubx
 Author: Dmitry Marienko
 Author-email: dmitry@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

