# Comparing `tmp/kline-0.4.3-py3-none-any.whl.zip` & `tmp/kline-0.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 7865 bytes, number of entries: 12
+Zip file size: 7871 bytes, number of entries: 12
 -rw-r--r--  2.0 unx       95 b- defN 80-Jan-01 00:00 kline/__init__.py
 -rw-r--r--  2.0 unx      454 b- defN 80-Jan-01 00:00 kline/base.py
--rw-r--r--  2.0 unx     3645 b- defN 80-Jan-01 00:00 kline/ccxt.py
+-rw-r--r--  2.0 unx     3694 b- defN 80-Jan-01 00:00 kline/ccxt.py
 -rw-r--r--  2.0 unx     2568 b- defN 80-Jan-01 00:00 kline/cli.py
 -rw-r--r--  2.0 unx     2739 b- defN 80-Jan-01 00:00 kline/deribit.py
 -rw-r--r--  2.0 unx     4503 b- defN 80-Jan-01 00:00 kline/max.py
 -rw-r--r--  2.0 unx      579 b- defN 80-Jan-01 00:00 kline/utils.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 kline-0.4.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      598 b- defN 80-Jan-01 00:00 kline-0.4.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 kline-0.4.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       39 b- defN 80-Jan-01 00:00 kline-0.4.3.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      870 b- defN 16-Jan-01 00:00 kline-0.4.3.dist-info/RECORD
-12 files, 17244 bytes uncompressed, 6433 bytes compressed:  62.7%
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 kline-0.4.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      598 b- defN 80-Jan-01 00:00 kline-0.4.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 kline-0.4.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       39 b- defN 80-Jan-01 00:00 kline-0.4.4.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      870 b- defN 16-Jan-01 00:00 kline-0.4.4.dist-info/RECORD
+12 files, 17293 bytes uncompressed, 6439 bytes compressed:  62.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: kline/max.py
 Comment: 
 
 Filename: kline/utils.py
 Comment: 
 
-Filename: kline-0.4.3.dist-info/LICENSE
+Filename: kline-0.4.4.dist-info/LICENSE
 Comment: 
 
-Filename: kline-0.4.3.dist-info/METADATA
+Filename: kline-0.4.4.dist-info/METADATA
 Comment: 
 
-Filename: kline-0.4.3.dist-info/WHEEL
+Filename: kline-0.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: kline-0.4.3.dist-info/entry_points.txt
+Filename: kline-0.4.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: kline-0.4.3.dist-info/RECORD
+Filename: kline-0.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kline/ccxt.py

```diff
@@ -49,14 +49,17 @@
                 break
 
             ohlcv = self.exchange.fetch_ohlcv(
                 symbol=symbol, timeframe=timeframe, since=since
             )
             ohlcv.sort(key=lambda k: k[0])
 
+            if not ohlcv:
+                break
+
             if ohlcvs and ohlcv[0][0] == ohlcvs[0][0]:
                 break
 
             ohlcvs = ohlcv + ohlcvs
 
             # a small amount of overlap to make sure the final data is continuous
             since = ohlcv[0][0] - to_milliseconds(timeframe) * (len(ohlcv) - 1)
```

## Comparing `kline-0.4.3.dist-info/LICENSE` & `kline-0.4.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kline-0.4.3.dist-info/METADATA` & `kline-0.4.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kline
-Version: 0.4.3
+Version: 0.4.4
 Summary: 
 Author: narumi
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

