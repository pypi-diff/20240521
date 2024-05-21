# Comparing `tmp/streaming_indicators-0.0.9.tar.gz` & `tmp/streaming_indicators-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streaming_indicators-0.0.9.tar", last modified: Mon Feb 19 12:09:56 2024, max compression
+gzip compressed data, was "streaming_indicators-0.1.0.tar", last modified: Tue May 21 12:27:03 2024, max compression
```

## Comparing `streaming_indicators-0.0.9.tar` & `streaming_indicators-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-02-19 12:09:56.933625 streaming_indicators-0.0.9/
--rw-rw-rw-   0        0        0     1082 2023-05-12 14:45:21.000000 streaming_indicators-0.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0     5760 2024-02-19 12:09:56.933625 streaming_indicators-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3938 2024-02-19 07:52:24.000000 streaming_indicators-0.0.9/README.md
--rw-rw-rw-   0        0        0       86 2023-05-12 14:44:06.000000 streaming_indicators-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0      871 2024-02-19 12:09:56.951667 streaming_indicators-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-19 12:09:56.615597 streaming_indicators-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2024-02-19 12:09:56.634864 streaming_indicators-0.0.9/src/streaming_indicators/
--rw-rw-rw-   0        0        0       35 2023-05-12 17:50:29.000000 streaming_indicators-0.0.9/src/streaming_indicators/__init__.py
--rw-rw-rw-   0        0        0    13187 2024-02-19 11:52:28.000000 streaming_indicators-0.0.9/src/streaming_indicators/streaming_indicators.py
-drwxrwxrwx   0        0        0        0 2024-02-19 12:09:56.914953 streaming_indicators-0.0.9/src/streaming_indicators.egg-info/
--rw-rw-rw-   0        0        0     5760 2024-02-19 12:09:56.000000 streaming_indicators-0.0.9/src/streaming_indicators.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-02-19 12:09:56.000000 streaming_indicators-0.0.9/src/streaming_indicators.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-19 12:09:56.000000 streaming_indicators-0.0.9/src/streaming_indicators.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-02-19 12:09:56.000000 streaming_indicators-0.0.9/src/streaming_indicators.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-02-19 12:09:56.000000 streaming_indicators-0.0.9/src/streaming_indicators.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 12:27:03.346746 streaming_indicators-0.1.0/
+-rw-rw-rw-   0        0        0     1082 2023-05-12 14:45:21.000000 streaming_indicators-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     5867 2024-05-21 12:27:03.345633 streaming_indicators-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4050 2024-05-21 12:23:01.000000 streaming_indicators-0.1.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-12 14:44:06.000000 streaming_indicators-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      865 2024-05-21 12:27:03.367934 streaming_indicators-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 12:27:03.186980 streaming_indicators-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 12:27:03.265487 streaming_indicators-0.1.0/src/streaming_indicators/
+-rw-rw-rw-   0        0        0       35 2023-05-12 17:50:29.000000 streaming_indicators-0.1.0/src/streaming_indicators/__init__.py
+-rw-rw-rw-   0        0        0    17178 2024-05-21 12:19:59.000000 streaming_indicators-0.1.0/src/streaming_indicators/streaming_indicators.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:27:03.337114 streaming_indicators-0.1.0/src/streaming_indicators.egg-info/
+-rw-rw-rw-   0        0        0     5867 2024-05-21 12:27:03.000000 streaming_indicators-0.1.0/src/streaming_indicators.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-05-21 12:27:03.000000 streaming_indicators-0.1.0/src/streaming_indicators.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 12:27:03.000000 streaming_indicators-0.1.0/src/streaming_indicators.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-21 12:27:03.000000 streaming_indicators-0.1.0/src/streaming_indicators.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-21 12:27:03.000000 streaming_indicators-0.1.0/src/streaming_indicators.egg-info/top_level.txt
```

### Comparing `streaming_indicators-0.0.9/LICENSE.txt` & `streaming_indicators-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streaming_indicators-0.0.9/PKG-INFO` & `streaming_indicators-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: streaming_indicators
-Version: 0.0.9
+Version: 0.1.0
 Summary: A python library for computing technical analysis indicators on streaming data.
 Home-page: https://github.com/mr-easy/streaming_indicators
 Author: Rishabh Gupta
 Author-email: rishabhg1997@gmail.com
 Project-URL: Bug Tracker, https://github.com/mr-easy/streaming_indicators/issues
 Project-URL: Code, https://github.com/mr-easy/streaming_indicators
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.13.3
-Requires-Dist: pandas_ta>=0.3.14b
+Requires-Dist: pandas>=2.0.0
 
 # Streaming Indicators 
 
 A python library for computing technical analysis indicators on streaming data.
 
 ## Installation
 ```
@@ -68,24 +68,25 @@
 ```
 atr_period = 20
 ATR = si.ATR(atr_period)
 for idx, candle in candles.iterrows():
     atr = ATR.update(candle)  # Assumes candle to have 'open',high','low','close' - TODO: give multiple inputs to update.
     print(atr)
 ```
+- Bollinger Bands (BBands)
 - SuperTrend (SuperTrend) 
 ```
 st_atr_length = 10
 st_factor = 3
 ST = si.SuperTrend(st_atr_length, st_factor)
 for idx, candle in candles.iterrows():
     st = ST.update(candle)
     print(st) # (st_direction:1/-1, band_value)
 ```
-To use some historical candles to initiate, use: `ST = si.SuperTrend(st_atr_length, st_factor, candles=initial_candles)` where `initial_candles` is pandas dataframe with `open,high,low,close` columns.  
+To use some historical candles to initiate, use: `ST = si.SuperTrend(st_atr_length, st_factor, candles=initial_candles)` where `initial_candles` is pandas dataframe with `open,high,low,close` columns, and requires talib package.
 - Heikin Ashi Candlesticks (HeikinAshi)
 ```
 HA = si.HeikinAshi()
 for idx, candle in candles.iterrows():
     ha_candle = HA.update(candle)
     print(ha_candle) # {'close': float, 'open': float, 'high': float, 'low': float}
 ```
@@ -120,14 +121,17 @@
 ```
 ## TODO
 - Not all indicators currently support compute method.
 - Add documentation.
 - SuperTrend,HeikinAshi,ATR depends on key names, eg ('open','close'). Should be independent, i.e. given in input. (similar to pandas_ta)
 - Add initalisation to all indicators similar to SuperTrend.
 - Implement more indicators.
+
+## Changelogs
+- [Version History](version_history.md)
 MIT License
 
 Copyright (c) [2023] [Rishabh Gupta]
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `streaming_indicators-0.0.9/README.md` & `streaming_indicators-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -50,24 +50,25 @@
 ```
 atr_period = 20
 ATR = si.ATR(atr_period)
 for idx, candle in candles.iterrows():
     atr = ATR.update(candle)  # Assumes candle to have 'open',high','low','close' - TODO: give multiple inputs to update.
     print(atr)
 ```
+- Bollinger Bands (BBands)
 - SuperTrend (SuperTrend) 
 ```
 st_atr_length = 10
 st_factor = 3
 ST = si.SuperTrend(st_atr_length, st_factor)
 for idx, candle in candles.iterrows():
     st = ST.update(candle)
     print(st) # (st_direction:1/-1, band_value)
 ```
-To use some historical candles to initiate, use: `ST = si.SuperTrend(st_atr_length, st_factor, candles=initial_candles)` where `initial_candles` is pandas dataframe with `open,high,low,close` columns.  
+To use some historical candles to initiate, use: `ST = si.SuperTrend(st_atr_length, st_factor, candles=initial_candles)` where `initial_candles` is pandas dataframe with `open,high,low,close` columns, and requires talib package.
 - Heikin Ashi Candlesticks (HeikinAshi)
 ```
 HA = si.HeikinAshi()
 for idx, candle in candles.iterrows():
     ha_candle = HA.update(candle)
     print(ha_candle) # {'close': float, 'open': float, 'high': float, 'low': float}
 ```
@@ -101,8 +102,11 @@
     print(is_increasing) # True/False
 ```
 ## TODO
 - Not all indicators currently support compute method.
 - Add documentation.
 - SuperTrend,HeikinAshi,ATR depends on key names, eg ('open','close'). Should be independent, i.e. given in input. (similar to pandas_ta)
 - Add initalisation to all indicators similar to SuperTrend.
-- Implement more indicators.
+- Implement more indicators.
+
+## Changelogs
+- [Version History](version_history.md)
```

### Comparing `streaming_indicators-0.0.9/setup.cfg` & `streaming_indicators-0.1.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7472 6561 6d69 6e67 5f69 6e64   = streaming_ind
 00000020: 6963 6174 6f72 730d 0a76 6572 7369 6f6e  icators..version
-00000030: 203d 2030 2e30 2e39 0d0a 6175 7468 6f72   = 0.0.9..author
+00000030: 203d 2030 2e31 2e30 0d0a 6175 7468 6f72   = 0.1.0..author
 00000040: 203d 2052 6973 6861 6268 2047 7570 7461   = Rishabh Gupta
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2072 6973 6861 6268 6731 3939 3740 676d   rishabhg1997@gm
 00000070: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000080: 7469 6f6e 203d 2041 2070 7974 686f 6e20  tion = A python 
 00000090: 6c69 6272 6172 7920 666f 7220 636f 6d70  library for comp
 000000a0: 7574 696e 6720 7465 6368 6e69 6361 6c20  uting technical 
@@ -42,14 +42,14 @@
 00000290: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
 000002a0: 0a09 3d20 7372 630d 0a70 6163 6b61 6765  ..= src..package
 000002b0: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
 000002c0: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
 000002d0: 2e34 0d0a 696e 7374 616c 6c5f 7265 7175  .4..install_requ
 000002e0: 6972 6573 203d 200d 0a09 6e75 6d70 7920  ires = ...numpy 
 000002f0: 3e3d 2031 2e31 332e 330d 0a09 7061 6e64  >= 1.13.3...pand
-00000300: 6173 5f74 6120 3e3d 2020 302e 332e 3134  as_ta >=  0.3.14
-00000310: 620d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  b....[options.pa
-00000320: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
-00000330: 6572 6520 3d20 7372 630d 0a0d 0a5b 6567  ere = src....[eg
-00000340: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-00000350: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-00000360: 3d20 300d 0a0d 0a                        = 0....
+00000300: 6173 203e 3d20 322e 302e 300d 0a0d 0a5b  as >= 2.0.0....[
+00000310: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
+00000320: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
+00000330: 7372 630d 0a0d 0a5b 6567 675f 696e 666f  src....[egg_info
+00000340: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000350: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000360: 0a                                       .
```

### Comparing `streaming_indicators-0.0.9/src/streaming_indicators/streaming_indicators.py` & `streaming_indicators-0.1.0/src/streaming_indicators/streaming_indicators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,137 @@
 import numpy as np
-import pandas_ta as ta
+import pandas as pd
 from collections import deque
 
 class SMA:
-    def __init__(self, period):
+    '''Simple Moving Average'''
+    def __init__(self, period:int, points=None):
         self.period = period
-        self.points = []
+        if(points is None): self.points = deque(maxlen=period)
+        else: self.points = deque(points[-period:], maxlen=period)
         self.value = None
-    def compute(self, point):
-        return np.mean(self.points + [float(point)])
-    def update(self, point):
+    def compute(self, point:float):
+        points = (list(self.points) + [float(point)])[-self.period:]
+        if(len(points) == self.period):
+            return np.mean(points)
+        return None
+    def update(self, point:float):
         self.points.append(float(point))
-        self.points = self.points[-self.period:]
         if(len(self.points) == self.period):
             self.value = np.mean(self.points)
         return self.value
     
+class SD:
+    '''Standard Deviation'''
+    def __init__(self, period:int, points=None):
+        self.period = period
+        if(points is None): self.points = deque(maxlen=period)
+        else: self.points = deque(points[-period:], maxlen=period)
+        self.value = None
+    def compute(self, point:float):
+        points = (list(self.points) + [float(point)])[-self.period:]
+        if(len(points) == self.period):
+            return np.std(points)
+        return None
+    def update(self, point:float):
+        self.points.append(float(point))
+        if(len(self.points) == self.period):
+            self.value = np.std(self.points)
+        return self.value
+
 class EMA:
-    def __init__(self, period, smoothing_factor=2):
+    '''Exponential Moving Average'''
+    def __init__(self, period:int, smoothing_factor:int=2):
         self.period = period
         self.smoothing_factor = smoothing_factor
-        self.mult = self.smoothing_factor / (1+self.period)
-        self.points = []
+        self.mult = smoothing_factor / (1+period)
+        self.points = deque(maxlen=period+1)
         self.value = None
-    def update(self, point):
+    def compute(self, point:float):
+        points = (list(self.points) + [float(point)])[-self.period:]
+        if(len(points) == self.period):
+            return np.mean(self.points) # Simple SMA
+        elif(len(points) > self.period):
+            return (point * self.mult) + (self.value * (1-self.mult))
+        return None
+    def update(self, point:float):
         self.points.append(point)
-        self.points = self.points[-(self.period+1):]
         if(len(self.points) == self.period):
             self.value = np.mean(self.points) # Simple SMA
         elif(len(self.points) > self.period):
             self.value = (point * self.mult) + (self.value * (1-self.mult))
         return self.value
 
 class WMA:
-    def __init__(self, period):
+    '''Weighted Moving Average'''
+    def __init__(self, period:int):
         self.period = period
         self.points = deque(maxlen=period)
         self._den = (period*(period+1))//2
         self._weights = np.arange(1,period+1)
         self.value = None
-    def update(self, point):
+    def compute(self, point:float):
+        points = (list(self.points) + [float(point)])[-self.period:]
+        if(len(points) == self.period):
+            return sum(self._weights*points)/self._den
+        return None
+    def update(self, point:float):
         self.points.append(point)
         if(len(self.points) == self.period):
             self.value = sum(self._weights*self.points)/self._den
         return self.value
 
 class SMMA:
     '''Smoothed Moving Average'''
-    def __init__(self, period):
+    def __init__(self, period:int):
         assert period > 1, "Period needs to be greater than 1."
         self.period = period
-        self.ema_period = self.period*2-1
+        self.ema_period = period*2-1
         # https://stackoverflow.com/a/72533211/6430403
-        self.ema = EMA(self.ema_period)
-    def update(self, point):
+        self.ema = EMA(ema_period)
+    def compute(self, point:float):
+        return self.ema.compute(point)
+    def update(self, point:float):
         self.value = self.ema.update(point)
         return self.value
     
 class RSI:
-    def __init__(self, period):
+    '''Relative Strength Index'''
+    def __init__(self, period:int):
         self.period = period
-        self.points = []
-        self.losses = []
-        self.gains = []
+        self._period_minus_1 = period-1
+        self._period_plus_1 = period+1
+        self.points = deque(maxlen=self._period_plus_1)
+        self.losses = deque(maxlen=self._period_plus_1)
+        self.gains = deque(maxlen=self._period_plus_1)
         self.avg_gain = None
         self.avg_loss = None
         self.rsi = None
         self.value = None
-    # def compute(self, point):
-    #     points = self.points + [float(point)]
-        
-    def update(self, point):
-        self.points.append(float(point))
+    def update(self, point:float):
+        self.points.append(point)
         if(len(self.points) > 1):
             diff = self.points[-1] - self.points[-2]
             if(diff >= 0):
                 self.gains.append(diff)
                 self.losses.append(0)
             else:
                 self.gains.append(0)
                 self.losses.append(-diff)
-        self.points = self.points[-(self.period+1):]
-        self.gains = self.gains[-(self.period):]
-        self.losses = self.losses[-(self.period):]
-
-        if(len(self.points) == self.period+1):
-            if(self.avg_gain is None):
-                self.avg_gain = np.mean(self.gains)
-                self.avg_loss = np.mean(self.losses)
-            else:
-                self.avg_gain = ((self.avg_gain*(self.period-1)) + self.gains[-1])/self.period
-                self.avg_loss = ((self.avg_loss*(self.period-1)) + self.losses[-1])/self.period
-            rs = self.avg_gain / self.avg_loss
-            self.rsi = 100 - (100/(1+rs))
-            self.value = self.rsi
+
+            if(len(self.points) == self._period_plus_1):
+                if(self.avg_gain is None):
+                    self.avg_gain = np.mean(self.gains)
+                    self.avg_loss = np.mean(self.losses)
+                else:
+                    self.avg_gain = ((self.avg_gain*(self._period_minus_1)) + self.gains[-1])/self.period
+                    self.avg_loss = ((self.avg_loss*(self._period_minus_1)) + self.losses[-1])/self.period
+                rs = self.avg_gain / self.avg_loss
+                self.rsi = 100 - (100/(1+rs))
+                self.value = self.rsi
         return self.value
 
 class TRANGE:
     '''True Range'''
     def __init__(self):
         self.prev_close = None
         self.value = None
@@ -118,78 +152,137 @@
 class ATR:
     '''Average True Range'''
     def __init__(self, period, candles=None):
         self.period = period
         self.period_1 = period-1
         self.TR = TRANGE()
         if(candles is None):
-            self.atr = 0
+            self.atr = 0 # initialised to 0, because values are added to it
             self.value = None
             self.count = 0
         else:
-            ta_ATR = ta.atr(candles['high'], candles['low'], candles['close'], length=period)
-            if(ta_ATR is None):
+            from talib import ATR
+            ta_atr = ATR(candles['high'],candles['low'],candles['close'],period)
+            if(pd.notna(ta_atr.iloc[-1])):
+                self.atr = ta_atr.iloc[-1]
+                self.value = self.atr
+            else:
                 self.atr = 0
                 self.value = None
-            else:
-                self.atr = ta_ATR.iloc[-1]
-                self.value = self.atr
             self.count = len(candles)
             self.TR.update(candles.iloc[-1])
     def compute(self, candle):
         tr = self.TR.compute(candle)
         if(self.count < self.period):
             return None
         elif(self.count == self.period):
             return (self.atr + tr)/self.period
         else:
             return (self.atr*self.period_1 + tr)/self.period
-
     def update(self, candle):
         self.count += 1
         tr = self.TR.update(candle)
         if(self.count < self.period):
             self.atr += tr
             return None
         if(self.count == self.period):
             self.atr += tr
             self.atr /= self.period
         else:
             self.atr = (self.atr*self.period_1 + tr)/self.period
         self.value = self.atr
         return self.value
 
+class BBands:
+    '''Bollinger Bands'''
+    def __init__(self, period:int, stddev_mult:float, ma=SMA, points=None):
+        self.period = period
+        self.stddev_mult = stddev_mult
+        if(isinstance(ma, type)): # if class
+            self.MA = ma(self.period, points=points)
+        else:
+            self.MA = ma
+        self.SD = SD(period, points=points)
+    @property
+    def middleband(self):
+        return self.MA.value
+    @property
+    def upperband(self):
+        if(self.SD.value is None): return None
+        return self.MA.value + self.SD.value * self.stddev_mult
+    @property
+    def lowerband(self):
+        if(self.SD.value is None): return None
+        return self.MA.value - self.SD.value * self.stddev_mult
+    @property
+    def value(self):
+        return (self.upperband, self.middleband, self.lowerband)
+    def compute(self, point:float):
+        ma = self.MA.compute(point)
+        sd = self.SD.compute(point)
+        if(ma is not None and sd is not None):
+            middleband = ma
+            upperband = ma + sd*self.stddev_mult
+            lowerband = ma - sd*self.stddev_mult
+            return (upperband, middleband, lowerband)
+        return (None, None, None)
+    def update(self, point:float):
+        ma = self.MA.update(point)
+        sd = self.SD.update(point)
+        return self.value
+
 class SuperTrend:
     def __init__(self, atr_length, factor, candles=None):
         self.factor = factor
+        self.super_trend = 1
         if(candles is None):
             self.ATR = ATR(atr_length)
             self.lower_band = None
             self.upper_band = None
-            self.super_trend = 1
             self.final_band = None
-            self.value = (None, None) # direction, value
         else:
-            self.ATR = ATR(atr_length, candles=candles)
-            ta_ST = ta.supertrend(candles['high'], candles['low'], candles['close'], length=atr_length, multiplier=self.factor, offset=0)
-            ta_ST.columns = ta_ST.columns.str.replace('_.*','',regex=True)
-            ta_ST_last = ta_ST.iloc[-1]
-            self.lower_band = ta_ST_last['SUPERTl']
-            self.upper_band = ta_ST_last['SUPERTs']
-            self.super_trend = int(ta_ST_last['SUPERTd'])
-            self.final_band = ta_ST_last['SUPERT']
-            self.value = (self.super_trend, self.final_band) # direction, value
+            self.ATR = ATR(atr_length, candles=candles) # TODO: ATR is getting computed twice
+            # Adapted from pandas_ta supertrend.py
+            # https://github.com/twopirllc/pandas-ta/blob/main/pandas_ta/overlap/supertrend.py
+            from talib import ATR as talib_ATR
+            _open = candles['open']
+            _high = candles['high']
+            _low = candles['low']
+            _close = candles['close']
+            _median = 0.5 * (_high + _low) # hl2
+            _fatr = factor * talib_ATR(_high, _low, _close, atr_length)
+            _basic_upperband = _median + _fatr
+            _basic_lowerband = _median - _fatr
+            self.lower_band = _basic_lowerband.iloc[0]
+            self.upper_band = _basic_upperband.iloc[0]
+            for i in range(1,len(candles)):
+                if self.super_trend == 1:
+                    self.upper_band = _basic_upperband.iloc[i]
+                    self.lower_band = max(_basic_lowerband.iloc[i], self.lower_band)
+                    if _close.iloc[i] <= self.lower_band:
+                        self.super_trend = -1
+                else:
+                    self.lower_band = _basic_lowerband.iloc[i]
+                    self.upper_band = min(_basic_upperband.iloc[i], self.upper_band)
+                    if _close.iloc[i] >= self.upper_band:
+                        self.super_trend = 1
+            if(self.super_trend == 1):
+                self.final_band = self.lower_band
+            else:
+                self.final_band = self.upper_band
+        self.value = (self.super_trend, self.final_band) # direction, value
                         
     def compute(self, candle):
         median = round((candle['high']+candle['low'])/2, 4)
         atr = self.ATR.compute(candle)
         if(atr is None):
             return None, None
-        basic_upper_band = round(median + self.factor * atr, 4)
-        basic_lower_band = round(median - self.factor * atr, 4)
+        _fatr = self.factor * atr
+        basic_upper_band = round(median + _fatr, 4)
+        basic_lower_band = round(median - _fatr, 4)
         super_trend = self.super_trend
         if self.super_trend == 1:
             upper_band = basic_upper_band
             lower_band = max(basic_lower_band, self.lower_band) if self.lower_band is not None else basic_lower_band
             if candle['close'] <= self.lower_band: super_trend = -1
         else:
             lower_band = basic_lower_band
@@ -218,14 +311,15 @@
             if candle['close'] >= self.upper_band:
                 self.super_trend = 1
 
         if(self.super_trend == 1):
             self.final_band = self.lower_band
         else:
             self.final_band = self.upper_band
+        
         self.value = (self.super_trend, self.final_band)
         return self.value
 
 class HeikinAshi:
     def __init__(self):
         self.value = None
 
@@ -321,18 +415,21 @@
     '>': operator.gt,
     '<': operator.lt,
     '>=': operator.ge,
     '<=': operator.le,
     '==': operator.eq    
 }
 class IsOrder:
-    ''' Checks if a given list of elements is in an order. eg. all increasing '''
-    ''' all_increasing = IsOrder('>', len) '''
-    ''' all_decreasing = IsOrder('<=', len) '''
-    ''' doubling = IsOrder(lambda a,b: a == 2*b, len) '''
+    ''' 
+        Checks if a given list of elements is in an order. eg. all increasing
+        examples:
+        - all_increasing = IsOrder('>', len)
+        - all_decreasing = IsOrder('<=', len)
+        - doubling = IsOrder(lambda a,b: a == 2*b, len)
+    '''
     def __init__(self, comparator, length):
         self.comparator = COMPARATORS.get(comparator, comparator)
         self.length = length
         self.q = deque(length*[None], maxlen=length)
         self.fresh = True
         self.order_idx = 1
         self.is_ordered = False
```

### Comparing `streaming_indicators-0.0.9/src/streaming_indicators.egg-info/PKG-INFO` & `streaming_indicators-0.1.0/src/streaming_indicators.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: streaming_indicators
-Version: 0.0.9
+Version: 0.1.0
 Summary: A python library for computing technical analysis indicators on streaming data.
 Home-page: https://github.com/mr-easy/streaming_indicators
 Author: Rishabh Gupta
 Author-email: rishabhg1997@gmail.com
 Project-URL: Bug Tracker, https://github.com/mr-easy/streaming_indicators/issues
 Project-URL: Code, https://github.com/mr-easy/streaming_indicators
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.13.3
-Requires-Dist: pandas_ta>=0.3.14b
+Requires-Dist: pandas>=2.0.0
 
 # Streaming Indicators 
 
 A python library for computing technical analysis indicators on streaming data.
 
 ## Installation
 ```
@@ -68,24 +68,25 @@
 ```
 atr_period = 20
 ATR = si.ATR(atr_period)
 for idx, candle in candles.iterrows():
     atr = ATR.update(candle)  # Assumes candle to have 'open',high','low','close' - TODO: give multiple inputs to update.
     print(atr)
 ```
+- Bollinger Bands (BBands)
 - SuperTrend (SuperTrend) 
 ```
 st_atr_length = 10
 st_factor = 3
 ST = si.SuperTrend(st_atr_length, st_factor)
 for idx, candle in candles.iterrows():
     st = ST.update(candle)
     print(st) # (st_direction:1/-1, band_value)
 ```
-To use some historical candles to initiate, use: `ST = si.SuperTrend(st_atr_length, st_factor, candles=initial_candles)` where `initial_candles` is pandas dataframe with `open,high,low,close` columns.  
+To use some historical candles to initiate, use: `ST = si.SuperTrend(st_atr_length, st_factor, candles=initial_candles)` where `initial_candles` is pandas dataframe with `open,high,low,close` columns, and requires talib package.
 - Heikin Ashi Candlesticks (HeikinAshi)
 ```
 HA = si.HeikinAshi()
 for idx, candle in candles.iterrows():
     ha_candle = HA.update(candle)
     print(ha_candle) # {'close': float, 'open': float, 'high': float, 'low': float}
 ```
@@ -120,14 +121,17 @@
 ```
 ## TODO
 - Not all indicators currently support compute method.
 - Add documentation.
 - SuperTrend,HeikinAshi,ATR depends on key names, eg ('open','close'). Should be independent, i.e. given in input. (similar to pandas_ta)
 - Add initalisation to all indicators similar to SuperTrend.
 - Implement more indicators.
+
+## Changelogs
+- [Version History](version_history.md)
 MIT License
 
 Copyright (c) [2023] [Rishabh Gupta]
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

