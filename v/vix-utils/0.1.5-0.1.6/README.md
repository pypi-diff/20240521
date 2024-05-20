# Comparing `tmp/vix_utils-0.1.5.tar.gz` & `tmp/vix_utils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vix_utils-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vix_utils-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vix_utils-0.1.5.tar` & `vix_utils-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3306 2024-02-02 18:07:29.867223 vix_utils-0.1.5/README.md
--rw-r--r--   0        0        0     1434 2024-02-02 18:07:29.887223 vix_utils-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      767 2024-02-02 18:07:29.887223 vix_utils-0.1.5/src/vix_utils/__init__.py
--rw-r--r--   0        0        0  1851085 2024-02-02 18:07:29.895223 vix_utils-0.1.5/src/vix_utils/cfe-rule-book.pdf
--rw-r--r--   0        0        0     5329 2024-02-02 18:07:29.895223 vix_utils-0.1.5/src/vix_utils/continuous_maturity.py
--rw-r--r--   0        0        0     4570 2024-02-02 18:07:29.895223 vix_utils-0.1.5/src/vix_utils/data_notes.md
--rw-r--r--   0        0        0    26917 2024-02-02 18:07:29.899223 vix_utils-0.1.5/src/vix_utils/download_vix_futures.py
--rw-r--r--   0        0        0      764 2024-02-02 18:07:29.899223 vix_utils-0.1.5/src/vix_utils/examples/a_t.ipynb
--rw-r--r--   0        0        0      259 2024-02-02 18:07:29.899223 vix_utils-0.1.5/src/vix_utils/examples/hello_x.py
--rw-r--r--   0        0        0     4063 2024-02-02 18:07:29.899223 vix_utils-0.1.5/src/vix_utils/examples/sample_load_data.py
--rw-r--r--   0        0        0     4670 2024-02-02 18:07:29.899223 vix_utils-0.1.5/src/vix_utils/examples/sample_plots.py
--rw-r--r--   0        0        0    49112 2024-02-02 18:07:29.899223 vix_utils-0.1.5/src/vix_utils/examples/vix_utils xarray.ipynb
--rw-r--r--   0        0        0   264522 2024-02-02 18:07:29.899223 vix_utils-0.1.5/src/vix_utils/examples/vix_utils.ipynb
--rw-r--r--   0        0        0     1234 2024-02-02 18:07:29.899223 vix_utils-0.1.5/src/vix_utils/futures_utils.py
--rw-r--r--   0        0        0      503 2024-02-02 18:07:29.899223 vix_utils-0.1.5/src/vix_utils/location.py
--rw-r--r--   0        0        0    27994 2024-02-02 18:07:29.899223 vix_utils-0.1.5/src/vix_utils/old_download_vix_futures.py
--rw-r--r--   0        0        0     3805 2024-02-02 18:07:29.899223 vix_utils-0.1.5/src/vix_utils/vix_cash_term_structure.py
--rw-r--r--   0        0        0    12834 2024-02-02 18:07:29.899223 vix_utils-0.1.5/src/vix_utils/vix_futures_dates.py
--rw-r--r--   0        0        0     4502 2024-02-02 18:07:29.899223 vix_utils-0.1.5/src/vix_utils/vixutil.py
--rw-r--r--   0        0        0     4260 1970-01-01 00:00:00.000000 vix_utils-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3306 2024-05-20 23:38:16.423488 vix_utils-0.1.6/README.md
+-rw-r--r--   0        0        0     1443 2024-05-20 23:38:16.443489 vix_utils-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      767 2024-05-20 23:38:16.443489 vix_utils-0.1.6/src/vix_utils/__init__.py
+-rw-r--r--   0        0        0  1851085 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/cfe-rule-book.pdf
+-rw-r--r--   0        0        0     5329 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/continuous_maturity.py
+-rw-r--r--   0        0        0     4570 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/data_notes.md
+-rw-r--r--   0        0        0    26919 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/download_vix_futures.py
+-rw-r--r--   0        0        0      764 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/examples/a_t.ipynb
+-rw-r--r--   0        0        0      259 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/examples/hello_x.py
+-rw-r--r--   0        0        0     4063 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/examples/sample_load_data.py
+-rw-r--r--   0        0        0     4670 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/examples/sample_plots.py
+-rw-r--r--   0        0        0    49112 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/examples/vix_utils xarray.ipynb
+-rw-r--r--   0        0        0   264522 2024-05-20 23:38:16.455489 vix_utils-0.1.6/src/vix_utils/examples/vix_utils.ipynb
+-rw-r--r--   0        0        0     1234 2024-05-20 23:38:16.455489 vix_utils-0.1.6/src/vix_utils/futures_utils.py
+-rw-r--r--   0        0        0      503 2024-05-20 23:38:16.455489 vix_utils-0.1.6/src/vix_utils/location.py
+-rw-r--r--   0        0        0    27994 2024-05-20 23:38:16.455489 vix_utils-0.1.6/src/vix_utils/old_download_vix_futures.py
+-rw-r--r--   0        0        0     3805 2024-05-20 23:38:16.455489 vix_utils-0.1.6/src/vix_utils/vix_cash_term_structure.py
+-rw-r--r--   0        0        0    12835 2024-05-20 23:38:16.455489 vix_utils-0.1.6/src/vix_utils/vix_futures_dates.py
+-rw-r--r--   0        0        0     4502 2024-05-20 23:38:16.455489 vix_utils-0.1.6/src/vix_utils/vixutil.py
+-rw-r--r--   0        0        0     4269 1970-01-01 00:00:00.000000 vix_utils-0.1.6/PKG-INFO
```

### Comparing `vix_utils-0.1.5/README.md` & `vix_utils-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.5/pyproject.toml` & `vix_utils-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 readme="README.md"
 requires-python=">=3.10"
 
 dynamic=["version"]
 
 dependencies= [
     "pandas",
-    "pandas-market-calendars",
+    "pandas-market-calendars >= 4.4.0",
     "aiofiles",
     "aiohttp[speedups]",
     "openpyxl",
     "appdirs",
     "more_itertools"]
```

### Comparing `vix_utils-0.1.5/src/vix_utils/__init__.py` & `vix_utils-0.1.6/src/vix_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 A library for preparing   VIX Futures and Cash Term Structures for analysis,
 including a  continuous maturity VIX Futures term structure.
 """
-__version__ = '0.1.5'
+__version__ = '0.1.6'
 
 from .download_vix_futures import  \
 pivot_futures_on_monthly_tenor,select_monthly_futures,async_load_vix_term_structure,load_vix_term_structure
 
 from .vix_cash_term_structure import \
     async_get_vix_index_histories,  \
     get_vix_index_histories,    \
```

### Comparing `vix_utils-0.1.5/src/vix_utils/cfe-rule-book.pdf` & `vix_utils-0.1.6/src/vix_utils/cfe-rule-book.pdf`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.5/src/vix_utils/continuous_maturity.py` & `vix_utils-0.1.6/src/vix_utils/continuous_maturity.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.5/src/vix_utils/data_notes.md` & `vix_utils-0.1.6/src/vix_utils/data_notes.md`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.5/src/vix_utils/download_vix_futures.py` & `vix_utils-0.1.6/src/vix_utils/download_vix_futures.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     url=f"https://cdn.cboe.com/resources/futures/archive/volume-and-price/CFE_{code}{yy}_VX.csv"
     return url, settlement_date_str
 
 def generate_monthly_url_dates():
      """
      Returns  the possible monthly urls and the date strings for all years and months in the default range.
      """
-     return (generate_monthly_url_date(y,m) for y,m in years_and_months)
+     return (generate_monthly_url_date(y,m) for y,m in years_and_months())
 
 def generate_weekly_url_date(date):
     """
     Returns the URL for the pattern of CBO to retreive the vix future expiring on date, even
     if no futures expired on date (which would give an URL to a non-existant resource)
     """
     date_str=date.isoformat()[0:10]
```

### Comparing `vix_utils-0.1.5/src/vix_utils/examples/a_t.ipynb` & `vix_utils-0.1.6/src/vix_utils/examples/a_t.ipynb`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.5/src/vix_utils/examples/sample_load_data.py` & `vix_utils-0.1.6/src/vix_utils/examples/sample_load_data.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.5/src/vix_utils/examples/sample_plots.py` & `vix_utils-0.1.6/src/vix_utils/examples/sample_plots.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.5/src/vix_utils/examples/vix_utils xarray.ipynb` & `vix_utils-0.1.6/src/vix_utils/examples/vix_utils xarray.ipynb`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.5/src/vix_utils/examples/vix_utils.ipynb` & `vix_utils-0.1.6/src/vix_utils/examples/vix_utils.ipynb`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.5/src/vix_utils/futures_utils.py` & `vix_utils-0.1.6/src/vix_utils/futures_utils.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.5/src/vix_utils/old_download_vix_futures.py` & `vix_utils-0.1.6/src/vix_utils/old_download_vix_futures.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.5/src/vix_utils/vix_cash_term_structure.py` & `vix_utils-0.1.6/src/vix_utils/vix_cash_term_structure.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.5/src/vix_utils/vix_futures_dates.py` & `vix_utils-0.1.6/src/vix_utils/vix_futures_dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     friday_expiration = any(_valid_cfe_days.isin([option_expiry_date]))
     if not friday_expiration:
         # the preceding day will be the option expiry date
         option_expiry_date = option_expiry_date - dt.timedelta(days=1)
 
     futures_expiry_date = option_expiry_date - dt.timedelta(days=30)
     # also check for a holiday on the 30 days before the 3d friday
-    if friday_expiration and not any(_valid_cfe_days.isin([option_expiry_date])):
+    if friday_expiration and not any(_valid_cfe_days.isin([futures_expiry_date])):
         futures_expiry_date = futures_expiry_date - dt.timedelta(days=1)
 
     return futures_expiry_date
 
 
 def vix_futures_expiry_date_from_trade_date(year, month, day, tenor):
     """
```

### Comparing `vix_utils-0.1.5/src/vix_utils/vixutil.py` & `vix_utils-0.1.6/src/vix_utils/vixutil.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.5/PKG-INFO` & `vix_utils-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: vix_utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: Provide VIX Cash and Futures Term Structure as Pandas dataframes
 Keywords: vix,volatility,pandas,vix term structure,cboe
 Author-email: Doug Ransom <doug@ransom.vip>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Dist: pandas
-Requires-Dist: pandas-market-calendars
+Requires-Dist: pandas-market-calendars >= 4.4.0
 Requires-Dist: aiofiles
 Requires-Dist: aiohttp[speedups]
 Requires-Dist: openpyxl
 Requires-Dist: appdirs
 Requires-Dist: more_itertools
 Requires-Dist: matplotlib ; extra == "examples"
 Requires-Dist: scipy ; extra == "examples"
```

