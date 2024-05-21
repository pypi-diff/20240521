# Comparing `tmp/kocoafab-1.0.4.tar.gz` & `tmp/kocoafab-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kocoafab-1.0.4.tar", last modified: Mon Feb 26 05:03:52 2024, max compression
+gzip compressed data, was "kocoafab-1.0.5.tar", last modified: Tue May 21 04:06:59 2024, max compression
```

## Comparing `kocoafab-1.0.4.tar` & `kocoafab-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 05:03:52.849907 kocoafab-1.0.4/
--rw-rw-rw-   0        0        0     8487 2023-12-11 05:18:23.000000 kocoafab-1.0.4/BlynkLib.py
--rw-rw-rw-   0        0        0      557 2024-02-26 05:03:52.847909 kocoafab-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      131 2023-12-11 05:15:59.000000 kocoafab-1.0.4/README.md
--rw-rw-rw-   0        0        0     3828 2023-07-15 01:40:17.000000 kocoafab-1.0.4/ble_library.py
--rw-rw-rw-   0        0        0     1118 2023-08-28 08:30:16.000000 kocoafab-1.0.4/dht.py
--rw-rw-rw-   0        0        0     3383 2023-07-18 11:20:46.000000 kocoafab-1.0.4/i2c_lcd.py
-drwxrwxrwx   0        0        0        0 2024-02-26 05:03:52.842906 kocoafab-1.0.4/kocoafab.egg-info/
--rw-rw-rw-   0        0        0      557 2024-02-26 05:03:52.000000 kocoafab-1.0.4/kocoafab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-02-26 05:03:52.000000 kocoafab-1.0.4/kocoafab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 05:03:52.000000 kocoafab-1.0.4/kocoafab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-02-26 05:03:52.000000 kocoafab-1.0.4/kocoafab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7461 2023-07-15 08:01:13.000000 kocoafab-1.0.4/lcd_api.py
--rw-rw-rw-   0        0        0     1585 2024-02-26 04:38:21.000000 kocoafab-1.0.4/servo.py
--rw-rw-rw-   0        0        0       42 2024-02-26 05:03:52.849907 kocoafab-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      777 2024-02-26 04:40:33.000000 kocoafab-1.0.4/setup.py
--rw-rw-rw-   0        0        0     4946 2023-08-28 04:22:55.000000 kocoafab-1.0.4/ssd1306.py
--rw-rw-rw-   0        0        0     5624 2023-08-28 08:22:37.000000 kocoafab-1.0.4/tcs34725.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:06:59.587257 kocoafab-1.0.5/
+-rw-rw-rw-   0        0        0     8487 2023-12-11 05:18:23.000000 kocoafab-1.0.5/BlynkLib.py
+-rw-rw-rw-   0        0        0      557 2024-05-21 04:06:59.585255 kocoafab-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2023-12-11 05:15:59.000000 kocoafab-1.0.5/README.md
+-rw-rw-rw-   0        0        0     3844 2024-05-21 04:01:48.000000 kocoafab-1.0.5/ble_library.py
+-rw-rw-rw-   0        0        0     1118 2023-08-28 08:30:16.000000 kocoafab-1.0.5/dht.py
+-rw-rw-rw-   0        0        0     3383 2023-07-18 11:20:46.000000 kocoafab-1.0.5/i2c_lcd.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:06:59.578264 kocoafab-1.0.5/kocoafab.egg-info/
+-rw-rw-rw-   0        0        0      557 2024-05-21 04:06:59.000000 kocoafab-1.0.5/kocoafab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-05-21 04:06:59.000000 kocoafab-1.0.5/kocoafab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 04:06:59.000000 kocoafab-1.0.5/kocoafab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-21 04:06:59.000000 kocoafab-1.0.5/kocoafab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7461 2023-07-15 08:01:13.000000 kocoafab-1.0.5/lcd_api.py
+-rw-rw-rw-   0        0        0     1585 2024-02-26 04:38:21.000000 kocoafab-1.0.5/servo.py
+-rw-rw-rw-   0        0        0       42 2024-05-21 04:06:59.588266 kocoafab-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      777 2024-05-21 04:02:49.000000 kocoafab-1.0.5/setup.py
+-rw-rw-rw-   0        0        0     4946 2023-08-28 04:22:55.000000 kocoafab-1.0.5/ssd1306.py
+-rw-rw-rw-   0        0        0     5624 2023-08-28 08:22:37.000000 kocoafab-1.0.5/tcs34725.py
```

### Comparing `kocoafab-1.0.4/BlynkLib.py` & `kocoafab-1.0.5/BlynkLib.py`

 * *Files identical despite different names*

### Comparing `kocoafab-1.0.4/PKG-INFO` & `kocoafab-1.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kocoafab
-Version: 1.0.4
+Version: 1.0.5
 Summary: Library to get readings from sensors on a ESP32.
 Home-page: https://kocoafab.cc
 Author: kocoafab
 Author-email: kocoafab@kocoa.or.kr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kocoafab-1.0.4/ble_library.py` & `kocoafab-1.0.5/ble_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             self._connections.remove(conn_handle)
             # Start advertising again to allow a new connection.
             self._advertise()
         elif event == _IRQ_GATTS_WRITE:
             conn_handle, value_handle = data
             value = self._ble.gatts_read(value_handle)
             if value_handle == self._handle_rx and self._write_callback:
-                self._write_callback(value)
+                self._write_callback(value.decode('utf-8'))
 
     def send(self, data):
         for conn_handle in self._connections:
             self._ble.gatts_notify(conn_handle, self._handle_tx, data)
 
     def is_connected(self):
         return len(self._connections) > 0
```

### Comparing `kocoafab-1.0.4/dht.py` & `kocoafab-1.0.5/dht.py`

 * *Files identical despite different names*

### Comparing `kocoafab-1.0.4/i2c_lcd.py` & `kocoafab-1.0.5/i2c_lcd.py`

 * *Files identical despite different names*

### Comparing `kocoafab-1.0.4/kocoafab.egg-info/PKG-INFO` & `kocoafab-1.0.5/kocoafab.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kocoafab
-Version: 1.0.4
+Version: 1.0.5
 Summary: Library to get readings from sensors on a ESP32.
 Home-page: https://kocoafab.cc
 Author: kocoafab
 Author-email: kocoafab@kocoa.or.kr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kocoafab-1.0.4/lcd_api.py` & `kocoafab-1.0.5/lcd_api.py`

 * *Files identical despite different names*

### Comparing `kocoafab-1.0.4/servo.py` & `kocoafab-1.0.5/servo.py`

 * *Files identical despite different names*

### Comparing `kocoafab-1.0.4/setup.py` & `kocoafab-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r",encoding='UTF-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kocoafab",
     py_modules=['ble_library','i2c_lcd','lcd_api','ssd1306','tcs34725','dht','BlynkLib','servo'],
-    version="1.0.4",
+    version="1.0.5",
     author="kocoafab",
     author_email="kocoafab@kocoa.or.kr",
     description="Library to get readings from sensors on a ESP32.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://kocoafab.cc",
     packages=setuptools.find_packages(),
```

### Comparing `kocoafab-1.0.4/ssd1306.py` & `kocoafab-1.0.5/ssd1306.py`

 * *Files identical despite different names*

### Comparing `kocoafab-1.0.4/tcs34725.py` & `kocoafab-1.0.5/tcs34725.py`

 * *Files identical despite different names*

