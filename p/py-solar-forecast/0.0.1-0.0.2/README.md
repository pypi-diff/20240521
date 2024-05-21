# Comparing `tmp/py_solar_forecast-0.0.1.tar.gz` & `tmp/py_solar_forecast-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_solar_forecast-0.0.1.tar", max compression
+gzip compressed data, was "py_solar_forecast-0.0.2.tar", max compression
```

## Comparing `py_solar_forecast-0.0.1.tar` & `py_solar_forecast-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1100 2024-05-19 22:00:24.856985 py_solar_forecast-0.0.1/LICENSE
--rw-r--r--   0        0        0     3912 2024-05-19 22:24:36.676586 py_solar_forecast-0.0.1/README.md
--rw-r--r--   0        0        0     3151 2024-05-19 22:41:37.771533 py_solar_forecast-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      636 2024-05-19 21:39:40.267886 py_solar_forecast-0.0.1/src/py_solar_forecast/__init__.py
--rw-r--r--   0        0        0     1772 2024-05-19 21:38:46.517875 py_solar_forecast-0.0.1/src/py_solar_forecast/exceptions.py
--rw-r--r--   0        0        0     5481 2024-05-19 21:38:46.517875 py_solar_forecast-0.0.1/src/py_solar_forecast/models.py
--rw-r--r--   0        0        0        0 2024-05-19 21:38:46.517875 py_solar_forecast-0.0.1/src/py_solar_forecast/py.typed
--rw-r--r--   0        0        0     4518 2024-05-19 22:26:37.736896 py_solar_forecast-0.0.1/src/py_solar_forecast/py_solar_forecast.py
--rw-r--r--   0        0        0     5100 1970-01-01 00:00:00.000000 py_solar_forecast-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1100 2024-05-19 22:00:24.856985 py_solar_forecast-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3912 2024-05-19 22:24:36.676586 py_solar_forecast-0.0.2/README.md
+-rw-r--r--   0        0        0     3151 2024-05-21 10:15:04.762943 py_solar_forecast-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      636 2024-05-19 21:39:40.267886 py_solar_forecast-0.0.2/src/py_solar_forecast/__init__.py
+-rw-r--r--   0        0        0     1772 2024-05-19 21:38:46.517875 py_solar_forecast-0.0.2/src/py_solar_forecast/exceptions.py
+-rw-r--r--   0        0        0     5621 2024-05-21 10:14:40.412948 py_solar_forecast-0.0.2/src/py_solar_forecast/models.py
+-rw-r--r--   0        0        0        0 2024-05-19 21:38:46.517875 py_solar_forecast-0.0.2/src/py_solar_forecast/py.typed
+-rw-r--r--   0        0        0     4518 2024-05-19 22:26:37.736896 py_solar_forecast-0.0.2/src/py_solar_forecast/py_solar_forecast.py
+-rw-r--r--   0        0        0     5100 1970-01-01 00:00:00.000000 py_solar_forecast-0.0.2/PKG-INFO
```

### Comparing `py_solar_forecast-0.0.1/LICENSE` & `py_solar_forecast-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_solar_forecast-0.0.1/README.md` & `py_solar_forecast-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `py_solar_forecast-0.0.1/pyproject.toml` & `py_solar_forecast-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-solar-forecast"
-version = "0.0.1"
+version = "0.0.2"
 description = "Asynchronous Python client for getting forecast solar information"
 authors = ["Klaas Schoute <hello@student-techlife.com>", "Rany <rany@riseup.net>"]
 maintainers = ["Rany <rany@riseup.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rany2/py-solar-forecast"
 repository = "https://github.com/rany2/py-solar-forecast"
```

### Comparing `py_solar_forecast-0.0.1/src/py_solar_forecast/__init__.py` & `py_solar_forecast-0.0.2/src/py_solar_forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `py_solar_forecast-0.0.1/src/py_solar_forecast/exceptions.py` & `py_solar_forecast-0.0.2/src/py_solar_forecast/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_solar_forecast-0.0.1/src/py_solar_forecast/models.py` & `py_solar_forecast-0.0.2/src/py_solar_forecast/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 from zoneinfo import ZoneInfo
 
 
 def _timed_value(at: datetime, data: dict[datetime, int]) -> int | None:
     """Return the value for a specific time."""
     value = None
     for timestamp, cur_value in data.items():
+        # Don't show values that have already passed
+        if timestamp < at:
+            continue
+
         if timestamp > at:
             return value
         value = cur_value
 
     return None
 
 
@@ -119,15 +123,15 @@
     def peak_production_time(self, specific_date: date) -> datetime:
         """Return the peak time on a specific date."""
         value = max(
             (watt for date, watt in self.watts.items() if date.date() == specific_date),
             default=None,
         )
         for timestamp, watt in self.watts.items():
-            if watt == value:
+            if watt == value and timestamp.date() == specific_date:
                 return timestamp
         raise RuntimeError("No peak production time found")
 
     def power_production_at_time(self, time: datetime) -> int:
         """Return estimated power production at a specific time."""
         return _timed_value(time, self.watts) or 0
```

### Comparing `py_solar_forecast-0.0.1/src/py_solar_forecast/py_solar_forecast.py` & `py_solar_forecast-0.0.2/src/py_solar_forecast/py_solar_forecast.py`

 * *Files identical despite different names*

### Comparing `py_solar_forecast-0.0.1/PKG-INFO` & `py_solar_forecast-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-solar-forecast
-Version: 0.0.1
+Version: 0.0.2
 Summary: Asynchronous Python client for getting forecast solar information
 Home-page: https://github.com/rany2/py-solar-forecast
 License: MIT
 Keywords: forecast,solar,power,energy,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Rany
```

