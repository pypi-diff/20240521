# Comparing `tmp/backtesting_server-0.6.0.tar.gz` & `tmp/backtesting_server-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtesting_server-0.6.0.tar", max compression
+gzip compressed data, was "backtesting_server-0.7.0.tar", max compression
```

## Comparing `backtesting_server-0.6.0.tar` & `backtesting_server-0.7.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 backtesting_server-0.6.0/LICENSE
--rw-r--r--   0        0        0      628 2024-05-12 13:36:16.558091 backtesting_server-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1858 2024-04-15 23:43:05.933161 backtesting_server-0.6.0/README.md
--rw-r--r--   0        0        0      202 2024-05-06 11:19:03.439830 backtesting_server-0.6.0/src/backtesting_server/__init__.py
--rw-r--r--   0        0        0    29714 2024-05-12 13:36:02.145416 backtesting_server-0.6.0/src/backtesting_server/main.py
--rw-r--r--   0        0        0     2465 1970-01-01 00:00:00.000000 backtesting_server-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 backtesting_server-0.7.0/LICENSE
+-rw-r--r--   0        0        0      628 2024-05-20 23:38:55.323935 backtesting_server-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1858 2024-04-15 23:43:05.933161 backtesting_server-0.7.0/README.md
+-rw-r--r--   0        0        0      222 2024-05-20 23:38:04.584896 backtesting_server-0.7.0/src/backtesting_server/__init__.py
+-rw-r--r--   0        0        0    35711 2024-05-20 23:38:04.586016 backtesting_server-0.7.0/src/backtesting_server/main.py
+-rw-r--r--   0        0        0     2465 1970-01-01 00:00:00.000000 backtesting_server-0.7.0/PKG-INFO
```

### Comparing `backtesting_server-0.6.0/LICENSE` & `backtesting_server-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `backtesting_server-0.6.0/pyproject.toml` & `backtesting_server-0.7.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "backtesting-server"
-version = "0.6.0"
+version = "0.7.0"
 description = "Package to interact with MySQL server, recording results of the backtesting."
 authors = ["hnewey7 <hnewey7@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `backtesting_server-0.6.0/README.md` & `backtesting_server-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `backtesting_server-0.6.0/src/backtesting_server/main.py` & `backtesting_server-0.7.0/src/backtesting_server/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -645,14 +645,82 @@
       previous_epoch = current_epoch
     
     # Creating dataframe.
     df = pd.DataFrame(results, columns=['Datetime', 'Open', 'High', 'Low', 'Close'])
     df.set_index("Datetime",inplace=True)
     return df
 
+  def patch_entire_historical_data(self, ig: ig_package.IG, previous_days: int) -> None:
+    """ Checking all historical data stored on the server and ensuring no gaps within the data. If the patch necessary is more severe (greater gap in data), higher resolution patch applied and repeated until patched.
+    
+    Parameters
+    ----------
+    ig: ig_package.IG
+      IG object.
+    previous_days: int
+      Previous days to patch historical data."""
+    # Getting all instruments with historical data on the server.
+    uploaded_instruments = self.get_uploaded_instruments(ig)
+    # Getting all gaps in instruments.
+    gaps: list[HistoricalPriceGap] = []
+    for instrument in uploaded_instruments:
+      gaps.extend(self.get_historical_price_gaps(instrument,previous_days))
+    # Sorting gaps.
+    gaps.sort(reverse=True)
+
+    # Resolutions.
+    resolutions = {
+      "MINUTE": 60,
+      "MINUTE_15": 15*60,
+      "HOUR": 60*60,
+      "HOUR_4": 4*60*60,
+      "DAY": 24*60*60
+    }
+
+    # Filling in all gaps.
+    set_resolution = "SECOND"
+    for gap in gaps:
+      for resolution in resolutions.items():
+        if gap.time_range / resolution[1] < 1:
+          break
+        set_resolution = resolution[0]
+      
+      if set_resolution != "SECOND":
+        self.get_historical_data(gap.instrument,set_resolution,gap.start_datetime.strftime("%y-%m-%d %H:%M:%S"),gap.end_datetime.strftime("%y-%m-%d %H:%M:%S"))
+
+  def get_historical_price_gaps(self, instrument: ig_package.Instrument, previous_days: int) -> list[HistoricalPriceGap]:
+    """ Getting all historical data price gaps for the given instrument.
+    
+      Parameters
+      ----------
+      instrument: ig_package.Instrument
+        Instrument to get price gaps for.
+      previous_days: int
+        Number of days previously to check.
+      
+      Returns
+      -------
+      list[HistoricalPriceGap]
+        List of all historical data price gaps."""
+    # Getting datetime.
+    current_datetime = datetime.now().timestamp()
+    previous_epoch = current_datetime - (previous_days * 60 * 60 * 24)
+    previous_datetime = datetime.fromtimestamp(previous_epoch)
+    previous_datetime_str = previous_datetime.strftime("%Y-%m-%d %H:%M:%S")
+    # Requesting all data within timeframe for datetime index.
+    self.cursor.execute("SELECT DatetimeIndex FROM {}_HistoricalDataset WHERE DatetimeIndex > '{}';".format(instrument.name.replace(" ","_"),previous_datetime_str))
+    results = self.cursor.fetchall()
+    # Getting all time differences.
+    time_differences = []
+    for index,datetime_index in enumerate(results):
+      if index > 0:
+        gap = HistoricalPriceGap(instrument,results[index-1][0],datetime_index[0])
+        time_differences.append(gap)
+    return time_differences
+
 # - - - - - - - - - - - - - -
 
 class InstrumentGroup():
   """ Class for representing a group of instruments on the Backtesting Server. These instruments can have entire actions performed on them, allowing for easy management of specific instruments."""
 
   def __init__(self, name:str, cursor:pymysql.cursors.Cursor) -> None:
     self.name: str = name
@@ -717,15 +785,75 @@
     # Getting epics.
     epics = self._get_instrument_epics()
     # Creating instruments.
     instrument_list = []
     for epic in epics:
       instrument_list.append(ig_package.Instrument(epic,ig))
     return instrument_list
+
+# - - - - - - - - - - - - - -
+
+class HistoricalPriceGap():
+  """ Class for representing a gap in the historical price data of an Instrument."""
+
+  def __init__(self, instrument: ig_package.Instrument, start_datetime: datetime, end_datetime: datetime):
+    # Instrument and opening hours.
+    self.instrument: ig_package.Instrument = instrument
+    if self.instrument.open_time and self.instrument.close_time:
+      self.open_time = (int(instrument.open_time[:2]),int(instrument.open_time[-2:]))
+      self.close_time = (int(instrument.close_time[:2]),int(instrument.close_time[-2:]))
+    else:
+      self.open_time = (0,0)
+      self.close_time = (0,0)
+
+    # Datetimes.
+    self.start_datetime: datetime = start_datetime
+    self.end_datetime: datetime = end_datetime
+
+    # Calculating time range.
+    start_epoch = start_datetime.timestamp()
+    end_epoch = end_datetime.timestamp()
+    current_starting_day_epoch = (start_epoch // (60*60*24)) * (60*60*24)
+    current_ending_day_epoch = current_starting_day_epoch + (60*60*24)
+    running_time_range = 0
     
+    while current_starting_day_epoch < end_epoch:
+      # Checking current day.
+      day_int = datetime.fromtimestamp(current_starting_day_epoch).weekday()
+      if day_int < 5:
+        # Get open/close datetimes for current day.
+        current_day_datetime = datetime.fromtimestamp(current_starting_day_epoch)
+        current_day_open_datetime = datetime(current_day_datetime.year,current_day_datetime.month,current_day_datetime.day,self.open_time[0],self.open_time[1])
+        current_day_close_datetime = datetime(current_day_datetime.year,current_day_datetime.month,current_day_datetime.day,self.close_time[0],self.close_time[1]) if self.close_time != (0,0) else datetime(current_day_datetime.year,current_day_datetime.month,current_day_datetime.day + 1,self.close_time[0],self.close_time[1])
+        
+        # Checking start to trading hours.
+        if current_day_close_datetime.timestamp() < end_epoch:
+          if start_epoch <= current_day_open_datetime.timestamp():
+            running_time_range += current_day_close_datetime.timestamp() - current_day_open_datetime.timestamp()
+          elif start_epoch > current_day_open_datetime.timestamp() and start_epoch < current_day_close_datetime.timestamp():
+            running_time_range += current_day_close_datetime.timestamp() - start_epoch
+        else:
+          if start_epoch <= current_day_open_datetime.timestamp():
+            running_time_range += end_epoch - current_day_open_datetime.timestamp()
+          elif start_epoch > current_day_open_datetime.timestamp() and start_epoch < current_day_close_datetime.timestamp():
+            running_time_range += end_epoch - start_epoch
+
+      current_starting_day_epoch += 60*60*24
+      current_ending_day_epoch += 60*60*24
+      start_epoch = current_starting_day_epoch
+    self.time_range = running_time_range
+
+  def __lt__(self, other):
+    result = True if self.time_range < other.time_range else False
+    return result
+  
+  def __gt__(self,other):
+    result = True if self.time_range > other.time_range else False
+    return result
+
 # - - - - - - - - - - - - - -
 
 if __name__ == "__main__":
 
   with open("logging_config.json") as f:
     config_dict = json.load(f)
     logging.config.dictConfig(config_dict)
```

### Comparing `backtesting_server-0.6.0/PKG-INFO` & `backtesting_server-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backtesting-server
-Version: 0.6.0
+Version: 0.7.0
 Summary: Package to interact with MySQL server, recording results of the backtesting.
 License: MIT
 Author: hnewey7
 Author-email: hnewey7@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

