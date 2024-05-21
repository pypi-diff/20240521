# Comparing `tmp/robocad-py-0.0.2.3.tar.gz` & `tmp/robocad-py-1.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\robocad-py-0.0.2.3.tar", last modified: Sat Feb 24 16:08:52 2024, max compression
+gzip compressed data, was "dist\robocad-py-1.0.2.2.tar", last modified: Tue May 21 20:30:44 2024, max compression
```

## Comparing `robocad-py-0.0.2.3.tar` & `robocad-py-1.0.2.2.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-02-24 16:08:52.000000 robocad-py-0.0.2.3/
--rw-rw-rw-   0        0        0      364 2023-07-23 09:23:41.000000 robocad-py-0.0.2.3/CHANGELOG.md
--rw-rw-rw-   0        0        0     1090 2023-03-30 12:51:13.000000 robocad-py-0.0.2.3/LICENSE
--rw-rw-rw-   0        0        0      109 2023-04-03 12:09:29.000000 robocad-py-0.0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1213 2024-02-24 16:08:52.000000 robocad-py-0.0.2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-02-24 16:08:52.000000 robocad-py-0.0.2.3/robocad/
--rw-rw-rw-   0        0        0        0 2023-04-03 12:05:15.000000 robocad-py-0.0.2.3/robocad/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-24 16:08:52.000000 robocad-py-0.0.2.3/robocad/pycad/
--rw-rw-rw-   0        0        0     5584 2023-08-13 14:13:51.000000 robocad-py-0.0.2.3/robocad/pycad/COM.py
--rw-rw-rw-   0        0        0     4202 2023-08-12 13:26:30.000000 robocad-py-0.0.2.3/robocad/pycad/SPI.py
--rw-rw-rw-   0        0        0        0 2023-03-30 13:39:56.000000 robocad-py-0.0.2.3/robocad/pycad/__init__.py
--rw-rw-rw-   0        0        0     3884 2023-08-12 13:06:20.000000 robocad-py-0.0.2.3/robocad/pycad/shared.py
--rw-rw-rw-   0        0        0    12554 2023-08-12 13:23:30.000000 robocad-py-0.0.2.3/robocad/robocad.py
-drwxrwxrwx   0        0        0        0 2024-02-24 16:08:52.000000 robocad-py-0.0.2.3/robocad/robocadSim/
--rw-rw-rw-   0        0        0        0 2023-03-30 13:43:09.000000 robocad-py-0.0.2.3/robocad/robocadSim/__init__.py
--rw-rw-rw-   0        0        0     7058 2023-08-12 13:26:30.000000 robocad-py-0.0.2.3/robocad/robocadSim/connection.py
--rw-rw-rw-   0        0        0     1201 2023-07-23 09:12:30.000000 robocad-py-0.0.2.3/robocad/robocadSim/connection_helper_vmx_titan.py
-drwxrwxrwx   0        0        0        0 2024-02-24 16:08:52.000000 robocad-py-0.0.2.3/robocad/shufflecad/
--rw-rw-rw-   0        0        0        0 2023-08-12 13:09:52.000000 robocad-py-0.0.2.3/robocad/shufflecad/__init__.py
--rw-rw-rw-   0        0        0    15822 2024-02-24 16:07:39.000000 robocad-py-0.0.2.3/robocad/shufflecad/connections.py
--rw-rw-rw-   0        0        0      843 2024-02-18 15:08:09.000000 robocad-py-0.0.2.3/robocad/shufflecad/logger.py
--rw-rw-rw-   0        0        0     2655 2023-08-12 13:14:52.000000 robocad-py-0.0.2.3/robocad/shufflecad/shared.py
--rw-rw-rw-   0        0        0      965 2023-08-12 13:20:01.000000 robocad-py-0.0.2.3/robocad/shufflecad/shufflecad.py
--rw-rw-rw-   0        0        0     3713 2024-02-24 16:04:30.000000 robocad-py-0.0.2.3/robocad/vex.py
-drwxrwxrwx   0        0        0        0 2024-02-24 16:08:52.000000 robocad-py-0.0.2.3/robocad_py.egg-info/
--rw-rw-rw-   0        0        0     1213 2024-02-24 16:08:51.000000 robocad-py-0.0.2.3/robocad_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      626 2024-02-24 16:08:51.000000 robocad-py-0.0.2.3/robocad_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-24 16:08:51.000000 robocad-py-0.0.2.3/robocad_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-02-24 16:08:51.000000 robocad-py-0.0.2.3/robocad_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-02-24 16:08:51.000000 robocad-py-0.0.2.3/robocad_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-24 16:08:52.000000 robocad-py-0.0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      865 2024-02-24 16:07:53.000000 robocad-py-0.0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:30:44.000000 robocad-py-1.0.2.2/
+-rw-rw-rw-   0        0        0      364 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     4029 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      109 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1208 2024-05-21 20:30:44.000000 robocad-py-1.0.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-21 20:30:44.000000 robocad-py-1.0.2.2/robocad/
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/robocad/__init__.py
+-rw-rw-rw-   0        0        0      506 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/robocad/common.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:30:44.000000 robocad-py-1.0.2.2/robocad/internal/
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/robocad/internal/__init__.py
+-rw-rw-rw-   0        0        0      654 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/robocad/internal/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:30:44.000000 robocad-py-1.0.2.2/robocad/internal/studica/
+-rw-rw-rw-   0        0        0     5521 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/robocad/internal/studica/COM.py
+-rw-rw-rw-   0        0        0     4134 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/robocad/internal/studica/SPI.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/robocad/internal/studica/__init__.py
+-rw-rw-rw-   0        0        0     6346 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/robocad/internal/studica/connection.py
+-rw-rw-rw-   0        0        0      298 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/robocad/internal/studica/connection_base.py
+-rw-rw-rw-   0        0        0     1873 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/robocad/internal/studica/connection_real.py
+-rw-rw-rw-   0        0        0     4221 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/robocad/internal/studica/connection_sim.py
+-rw-rw-rw-   0        0        0     4169 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/robocad/internal/studica/shared.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:30:44.000000 robocad-py-1.0.2.2/robocad/shufflecad/
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/robocad/shufflecad/__init__.py
+-rw-rw-rw-   0        0        0    15018 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/robocad/shufflecad/connections.py
+-rw-rw-rw-   0        0        0     1188 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/robocad/shufflecad/shufflecad.py
+-rw-rw-rw-   0        0        0     2177 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/robocad/shufflecad/shufflecad_holder.py
+-rw-rw-rw-   0        0        0     4568 2024-05-21 20:28:00.000000 robocad-py-1.0.2.2/robocad/studica.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:30:44.000000 robocad-py-1.0.2.2/robocad_py.egg-info/
+-rw-rw-rw-   0        0        0     1208 2024-05-21 20:30:43.000000 robocad-py-1.0.2.2/robocad_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2024-05-21 20:30:44.000000 robocad-py-1.0.2.2/robocad_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 20:30:43.000000 robocad-py-1.0.2.2/robocad_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-21 20:30:43.000000 robocad-py-1.0.2.2/robocad_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-21 20:30:43.000000 robocad-py-1.0.2.2/robocad_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 20:30:44.000000 robocad-py-1.0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      860 2024-05-21 20:30:37.000000 robocad-py-1.0.2.2/setup.py
```

### Comparing `robocad-py-0.0.2.3/PKG-INFO` & `robocad-py-1.0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.1
 Name: robocad-py
-Version: 0.0.2.3
+Version: 1.0.2.2
 Summary: python lib for real and virtual robots
-Home-page: https://github.com/CrackAndDie/robocad-py
+Home-page: https://github.com/Soft-V/robocad-py
 Author: Airat Abdrakov
 Author-email: softvery@yandex.ru
 License: MIT
 Description: Python library for real and virtual robots
         
         # Change Log
```

### Comparing `robocad-py-0.0.2.3/robocad/pycad/COM.py` & `robocad-py-1.0.2.2/robocad/internal/studica/COM.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 import time
 from threading import Thread
 
-from robocad.shufflecad.shared import InfoHolder
+from robocad.common import Common
 from .shared import TitanStatic
 from .shared import LibHolder
 from funcad.funcad import Funcad
 
 
 class TitanCOM:
     th: Thread = None
@@ -27,37 +27,37 @@
 
             start_time: int = round(time.time() * 10000)
             send_count_time: float = time.time()
             comm_counter = 0
             while not cls.stop_th:
                 tx_time: float = time.time() * 1000
                 tx_data = cls.set_up_tx_data()
-                InfoHolder.tx_com_time_dev = str(round(time.time() * 1000 - tx_time, 2))
+                Common.tx_com_time_dev = round(time.time() * 1000 - tx_time, 2)
 
                 rx_data: bytearray = LibHolder.rw_usb(tx_data)
 
                 rx_time: float = time.time() * 1000
                 cls.set_up_rx_data(rx_data)
-                InfoHolder.rx_com_time_dev = str(round(time.time() * 1000 - rx_time, 2))
+                Common.rx_com_time_dev = round(time.time() * 1000 - rx_time, 2)
 
                 comm_counter += 1
                 if time.time() - send_count_time > 1:
                     send_count_time = time.time()
-                    InfoHolder.com_count_dev = str(comm_counter)
+                    Common.com_count_dev = comm_counter
                     comm_counter = 0
 
                 time.sleep(0.001)
-                InfoHolder.com_time_dev = str(round(time.time() * 10000) - start_time)
+                Common.com_time_dev = round(time.time() * 10000) - start_time
                 start_time = round(time.time() * 10000)
         except Exception as e:
             LibHolder.stop_usb()
             exc_type, exc_obj, exc_tb = sys.exc_info()
             file_name = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-            InfoHolder.logger.write_main_log(" ".join(map(str, [exc_type, file_name, exc_tb.tb_lineno])))
-            InfoHolder.logger.write_main_log(str(e))
+            Common.logger.write_main_log(" ".join(map(str, [exc_type, file_name, exc_tb.tb_lineno])))
+            Common.logger.write_main_log(str(e))
 
     @staticmethod
     def set_up_rx_data(data: bytearray) -> None:
         if data[42] != 33:
             if data[0] == 1:
                 if data[24] == 111:
                     raw_enc_0: int = (data[2] & 0xff) << 8 | (data[1] & 0xff)
@@ -72,15 +72,15 @@
                     TitanStatic.limit_h_1 = Funcad.access_bit(data[9], 4)
                     TitanStatic.limit_l_2 = Funcad.access_bit(data[9], 5)
                     TitanStatic.limit_h_2 = Funcad.access_bit(data[9], 6)
                     TitanStatic.limit_l_3 = Funcad.access_bit(data[10], 1)
                     TitanStatic.limit_h_3 = Funcad.access_bit(data[10], 2)
 
         else:
-            InfoHolder.logger.write_main_log("received wrong data " + " ".join(map(str, data)))
+            Common.logger.write_main_log("received wrong data " + " ".join(map(str, data)))
 
     @staticmethod
     def set_up_tx_data() -> bytearray:
         tx_data: bytearray = bytearray([0] * 48)
         tx_data[0] = 1
 
         motor_speeds: bytearray = Funcad.int_to_4_bytes(abs(int(TitanStatic.speed_motor_0 / 100 * 65535)))
```

### Comparing `robocad-py-0.0.2.3/robocad/pycad/SPI.py` & `robocad-py-1.0.2.2/robocad/internal/studica/SPI.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 import time
 from threading import Thread
 
-from robocad.shufflecad.shared import InfoHolder
+from robocad.common import Common
 from .shared import VMXStatic
 from .shared import LibHolder
 from funcad.funcad import Funcad
 
 
 class VMXSPI:
     toggler: int = 0
@@ -29,49 +29,49 @@
 
             start_time: float = time.time() * 1000
             send_count_time: float = time.time()
             comm_counter = 0
             while not cls.stop_th:
                 tx_time: float = time.time() * 1000
                 tx_list = cls.set_up_tx_data()
-                InfoHolder.tx_spi_time_dev = str(round(time.time() * 1000 - tx_time, 2))
+                Common.tx_spi_time_dev = round(time.time() * 1000 - tx_time, 2)
 
                 rx_list: bytearray = LibHolder.rw_spi(tx_list)
 
                 rx_time: float = time.time() * 1000
                 cls.set_up_rx_data(rx_list)
-                InfoHolder.rx_spi_time_dev = str(round(time.time() * 1000 - rx_time, 2))
+                Common.rx_spi_time_dev = round(time.time() * 1000 - rx_time, 2)
 
                 comm_counter += 1
                 if time.time() - send_count_time > 1:
                     send_count_time = time.time()
-                    InfoHolder.spi_count_dev = str(comm_counter)
+                    Common.spi_count_dev = comm_counter
                     comm_counter = 0
 
                 time.sleep(0.002)
-                InfoHolder.spi_time_dev = str(round(time.time() * 1000 - start_time, 2))
+                Common.spi_time_dev = round(time.time() * 1000 - start_time, 2)
                 start_time = time.time() * 1000
         except (Exception, EOFError) as e:
             LibHolder.stop_spi()
             exc_type, exc_obj, exc_tb = sys.exc_info()
             file_name = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-            InfoHolder.logger.write_main_log(" ".join(map(str, [exc_type, file_name, exc_tb.tb_lineno])))
-            InfoHolder.logger.write_main_log(str(e))
+            Common.logger.write_main_log(" ".join(map(str, [exc_type, file_name, exc_tb.tb_lineno])))
+            Common.logger.write_main_log(str(e))
 
     @classmethod
     def set_up_rx_data(cls, data: bytearray) -> None:
         if data[0] == 1:
             yaw_ui: int = (data[2] & 0xff) << 8 | (data[1] & 0xff)
             us1_ui: int = (data[4] & 0xff) << 8 | (data[3] & 0xff)
             VMXStatic.ultrasound_1 = us1_ui / 100
             us2_ui: int = (data[6] & 0xff) << 8 | (data[5] & 0xff)
             VMXStatic.ultrasound_2 = us2_ui / 100
 
             power: float = ((data[8] & 0xff) << 8 | (data[7] & 0xff)) / 100
-            InfoHolder.power = str(power)
+            Common.power = power
 
             # calc yaw unlim
             new_yaw = (yaw_ui / 100) * (1 if Funcad.access_bit(data[9], 1) else -1)
             cls.calc_yaw_unlim(new_yaw, VMXStatic.yaw)
             VMXStatic.yaw = new_yaw
 
             VMXStatic.flex_0 = Funcad.access_bit(data[9], 2)
```

### Comparing `robocad-py-0.0.2.3/robocad/pycad/shared.py` & `robocad-py-1.0.2.2/robocad/internal/studica/shared.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
 import ctypes
+from robocad.common import Common
 
 
 class LibHolder:
     lib = None
 
     @classmethod
     def init(cls):
@@ -96,33 +97,41 @@
     flex_2: bool = False
     flex_3: bool = False
     flex_4: bool = False
     flex_5: bool = False
     flex_6: bool = False
     flex_7: bool = False
 
+    hcdio_values: list = [0.0] * 10
+
     @classmethod
     def set_servo_angle(cls, angle: float, pin: int):
         dut: float = 0.000666 * angle + 0.05
+        cls.hcdio_values[pin] = dut
         VMXStatic.echo_to_file(str(cls.HCDIO_CONST_ARRAY[pin]) + "=" + str(dut))
 
     @classmethod
     def set_led_state(cls, state: bool, pin: int):
         dut: float = 0.2 if state else 0.0
+        cls.hcdio_values[pin] = dut
         VMXStatic.echo_to_file(str(cls.HCDIO_CONST_ARRAY[pin]) + "=" + str(dut))
 
     @classmethod
     def set_servo_pwm(cls, pwm: float, pin: int):
         dut: float = pwm
+        cls.hcdio_values[pin] = dut
         VMXStatic.echo_to_file(str(cls.HCDIO_CONST_ARRAY[pin]) + "=" + str(dut))
 
     @classmethod
     def disable_servo(cls, pin: int):
+        cls.hcdio_values[pin] = 0.0
         VMXStatic.echo_to_file(str(cls.HCDIO_CONST_ARRAY[pin]) + "=" + "0.0")
 
     @staticmethod
     def echo_to_file(st: str):
+        if not Common.on_real_robot:
+            return None
         original_stdout = sys.stdout
         with open('/dev/pi-blaster', 'w') as f:
             sys.stdout = f  # Change the standard output to the file we created.
             print(st)
             sys.stdout = original_stdout  # Reset the standard output to its original value
```

### Comparing `robocad-py-0.0.2.3/robocad/robocadSim/connection.py` & `robocad-py-1.0.2.2/robocad/internal/studica/connection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,167 +1,155 @@
 import socket
 import threading
 import time
 import warnings
+import struct
 
-from robocad.shufflecad.shared import InfoHolder
+from robocad.common import Common
 
 
 class ListenPort:
-    def __init__(self, port: int, is_camera=False):
+    def __init__(self, port: int):
         self.__port = port
-        self.__is_camera = is_camera
 
         # other
         self.__stop_thread = False
-        self.out_string = ''
         self.out_bytes = b''
 
         self.__sct = None
         self.__thread = None
 
     def start_listening(self):
         self.__thread = threading.Thread(target=self.listening, args=())
         self.__thread.start()
 
     def listening(self):
         self.__sct = socket.socket(socket.AF_INET, socket.SOCK_STREAM, socket.IPPROTO_TCP)
         self.__sct.connect(('127.0.0.1', self.__port))
-        InfoHolder.logger.write_main_log("connected: " + str(self.__port))
+        Common.logger.write_main_log("connected: " + str(self.__port))
         while not self.__stop_thread:
             try:
-                if self.__is_camera:
-                    self.__sct.sendall("Wait for size".encode('utf-16-le'))
-                    image_size = self.__sct.recv(4)
-                    if len(image_size) < 4:
-                        continue
-                    buffer_size = (image_size[3] & 0xff) << 24 | (image_size[2] & 0xff) << 16 | \
-                                  (image_size[1] & 0xff) << 8 | (image_size[0] & 0xff)
-                    self.__sct.sendall("Wait for image".encode('utf-16-le'))
-                    self.out_bytes = self.__sct.recv(buffer_size)
-                else:
-                    self.__sct.sendall("Wait for data".encode('utf-16-le'))
-                    data_size = self.__sct.recv(4)
-                    if len(data_size) < 4:
-                        continue
-                    length = (data_size[3] & 0xff) << 24 | (data_size[2] & 0xff) << 16 | \
-                             (data_size[1] & 0xff) << 8 | (data_size[0] & 0xff)
-                    self.out_bytes = self.__sct.recv(length)
-                    self.out_string = self.out_bytes.decode('utf-16-le')
+                dt = "Wait for data".encode('utf-16-le')
+                dt_ln = struct.pack('<I', len(dt))
+                self.__sct.sendall(dt_ln)
+                self.__sct.sendall(dt)
+
+                data_size = self.__sct.recv(4)
+                if len(data_size) < 4:
+                    continue
+                length = (data_size[3] & 0xff) << 24 | (data_size[2] & 0xff) << 16 | \
+                            (data_size[1] & 0xff) << 8 | (data_size[0] & 0xff)
+                self.out_bytes = self.__sct.recv(length)
                 # задержка для слабых компов
                 time.sleep(0.004)
-            except (ConnectionAbortedError, BrokenPipeError):
+            except (ConnectionAbortedError, BrokenPipeError, OSError):
                 # возникает при отключении сокета
                 break
-        InfoHolder.logger.write_main_log("disconnected: " + str(self.__port))
-        self.__sct.shutdown(socket.SHUT_RDWR)
-        self.__sct.close()
+        Common.logger.write_main_log("disconnected: " + str(self.__port))
+        try:
+            self.__sct.shutdown(socket.SHUT_RDWR)
+            self.__sct.close()
+        except (OSError, Exception): pass  # idc
 
     def reset_out(self):
-        self.out_string = ''
         self.out_bytes = b''
 
     def stop_listening(self):
         self.__stop_thread = True
         self.reset_out()
         if self.__sct is not None:
             try:
                 self.__sct.shutdown(socket.SHUT_RDWR)
             except (OSError, Exception):
-                InfoHolder.logger.write_main_log("Something went wrong while shutting down socket on port " +
+                Common.logger.write_main_log("Something went wrong while shutting down socket on port " +
                                                  str(self.__port))
             if self.__thread is not None:
                 st_time = time.time()
                 # если поток все еще живой, ждем 1 секунды и закрываем сокет
                 while self.__thread.is_alive():
                     if time.time() - st_time > 1:
-                        InfoHolder.logger.write_main_log("Something went wrong. Rude disconnection on port " +
+                        Common.logger.write_main_log("Something went wrong. Rude disconnection on port " +
                                                          str(self.__port))
                         try:
                             self.__sct.close()
                         except (OSError, Exception):
-                            InfoHolder.logger.write_main_log("Something went wrong while closing socket on port " +
+                            Common.logger.write_main_log("Something went wrong while closing socket on port " +
                                                              str(self.__port))
                         st_time = time.time()
 
 
 class TalkPort:
     def __init__(self, port: int):
         self.__port = port
 
         # other
         self.__stop_thread = False
-        self.out_string = ''
+        self.out_bytes = b''
 
         self.__sct = None
         self.__thread = None
 
     def start_talking(self):
         self.__thread = threading.Thread(target=self.talking, args=())
         self.__thread.start()
 
     def talking(self):
         self.__sct = socket.socket(socket.AF_INET, socket.SOCK_STREAM, socket.IPPROTO_TCP)
         self.__sct.connect(('127.0.0.1', self.__port))
-        InfoHolder.logger.write_main_log("connected: " + str(self.__port))
+        Common.logger.write_main_log("connected: " + str(self.__port))
         while not self.__stop_thread:
             try:
-                self.__sct.sendall((self.out_string + "$").encode('utf-16-le'))
-                _ = self.__sct.recv(1024)  # ответ сервера
+                dt_ln = struct.pack('<I', len(self.out_bytes))
+                self.__sct.sendall(dt_ln)
+                self.__sct.sendall(self.out_bytes)
+                _ = self.__sct.recv(4)  # ответ сервера
+                _ = self.__sct.recv(4)  # ответ сервера
                 # задержка для слабых компов
                 time.sleep(0.004)
-            except (ConnectionAbortedError, BrokenPipeError):
+            except (ConnectionAbortedError, BrokenPipeError, OSError):
                 # возникает при отключении сокета
                 break
-        InfoHolder.logger.write_main_log("disconnected: " + str(self.__port))
-        self.__sct.shutdown(socket.SHUT_RDWR)
-        self.__sct.close()
+        Common.logger.write_main_log("disconnected: " + str(self.__port))
+        try:
+            self.__sct.shutdown(socket.SHUT_RDWR)
+            self.__sct.close()
+        except (OSError, Exception): pass  # idc
 
     def reset_out(self):
-        self.out_string = ''
+        self.out_bytes = b''
 
     def stop_talking(self):
         self.__stop_thread = True
         self.reset_out()
         if self.__sct is not None:
             try:
                 self.__sct.shutdown(socket.SHUT_RDWR)
             except (OSError, Exception):
-                InfoHolder.logger.write_main_log("Something went wrong while shutting down socket on port " +
+                Common.logger.write_main_log("Something went wrong while shutting down socket on port " +
                                                  str(self.__port))
             if self.__thread is not None:
                 st_time = time.time()
                 # если поток все еще живой, ждем 1 секунды и закрываем сокет
                 while self.__thread.is_alive():
                     if time.time() - st_time > 1:
-                        InfoHolder.logger.write_main_log("Something went wrong. Rude disconnection on port " +
+                        Common.logger.write_main_log("Something went wrong. Rude disconnection on port " +
                                                          str(self.__port))
                         try:
                             self.__sct.close()
                         except (OSError, Exception):
-                            InfoHolder.logger.write_main_log("Something went wrong while closing socket on port " +
+                            Common.logger.write_main_log("Something went wrong while closing socket on port " +
                                                              str(self.__port))
                         st_time = time.time()
 
 
 class ParseChannels:
     @staticmethod
-    def parse_float_channel(txt: str):
-        try:
-            return tuple(map(float, txt.replace(',', '.').split(';')))
-        except (Exception, ValueError):
-            return tuple()
-
+    def join_studica_channel(lst: tuple) -> bytes:
+        if len(lst) < 14:
+            return b''
+        return struct.pack('14f', *lst)
+    
     @staticmethod
-    def parse_bool_channel(txt: str):
-        try:
-            return tuple(map(bool, map(int, txt.split(';'))))
-        except (Exception, ValueError):
+    def parse_studica_channel(data: bytes) -> tuple:
+        if len(data) < 52:
             return tuple()
-
-    @staticmethod
-    def join_float_channel(lst: tuple):
-        return ';'.join(map(str, lst))
-
-    @staticmethod
-    def join_bool_channel(lst: tuple):
-        return ';'.join(map(str, map(int, lst)))
+        return struct.unpack('<4I2f4Hf16B', data)
```

### Comparing `robocad-py-0.0.2.3/robocad/shufflecad/connections.py` & `robocad-py-1.0.2.2/robocad/shufflecad/connections.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import sys
 import io
 import socket
 import struct
 import time
 from threading import Thread
 
-from .shared import ShuffleVariable, InfoHolder
-
+from robocad.common import Common
+from .shufflecad_holder import CameraVariable, ShufflecadHolder, ShuffleVariable
 
 class ListenPort:
     def __init__(self, port: int, event_handler=None, delay: float = 0.004):
         self.__port = port
 
         # other
         self.__stop_thread = False
@@ -34,69 +34,63 @@
 
     def listening(self):
         self.__sct = socket.socket(socket.AF_INET, socket.SOCK_STREAM, socket.IPPROTO_TCP)
         self.__sct.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self.__sct.bind(('0.0.0.0', self.__port))
         self.__sct.listen(1)
 
-        try:
-            connection_out = self.__sct.accept()[0].makefile('rwb')
-            handler = SplitFrames(connection_out)
-            while not self.__stop_thread:
-                try:
-                    handler.write("Waiting for data".encode("utf-8"))
-                    self.out_string = handler.read().decode("utf-8")
-
-                    self.event_call()
-
-                    # задержка для слабых компов
-                    time.sleep(self.__delay)
-                except (ConnectionAbortedError, BrokenPipeError) as e:
-                    # возникает при отключении сокета
-                    exc_type, exc_obj, exc_tb = sys.exc_info()
-                    file_name = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-                    InfoHolder.logger.write_main_log(" ".join(map(str, [exc_type, file_name, exc_tb.tb_lineno])))
-                    InfoHolder.logger.write_main_log(str(e))
-                    break
-            self.__sct.shutdown(socket.SHUT_RDWR)
-            self.__sct.close()
-        except Exception as e:
-            exc_type, exc_obj, exc_tb = sys.exc_info()
-            file_name = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-            InfoHolder.logger.write_main_log(" ".join(map(str, [exc_type, file_name, exc_tb.tb_lineno])))
-            InfoHolder.logger.write_main_log(str(e))
+        connection_out = self.__sct.accept()[0].makefile('rwb')
+        handler = SplitFrames(connection_out)
+        while not self.__stop_thread:
+            try:
+                handler.write("Waiting for data".encode("utf-8"))
+                self.out_string = handler.read().decode("utf-8")
+
+                self.event_call()
+
+                # задержка для слабых компов
+                time.sleep(self.__delay)
+            except (ConnectionAbortedError, BrokenPipeError) as e:
+                # возникает при отключении сокета
+                exc_type, exc_obj, exc_tb = sys.exc_info()
+                file_name = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
+                Common.logger.write_main_log(" ".join(map(str, [exc_type, file_name, exc_tb.tb_lineno])))
+                Common.logger.write_main_log(str(e))
+                break
+        self.__sct.shutdown(socket.SHUT_RDWR)
+        self.__sct.close()
 
     def reset_out(self):
         self.out_string = 'null'
         self.out_bytes = b'null'
 
     def stop_listening(self):
         self.__stop_thread = True
         self.reset_out()
         if self.__sct is not None:
             try:
                 self.__sct.shutdown(socket.SHUT_RDWR)
             except (OSError, Exception) as e:
                 exc_type, exc_obj, exc_tb = sys.exc_info()
                 file_name = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-                InfoHolder.logger.write_main_log(" ".join(map(str, [exc_type, file_name, exc_tb.tb_lineno])))
-                InfoHolder.logger.write_main_log(str(e))
+                Common.logger.write_main_log(" ".join(map(str, [exc_type, file_name, exc_tb.tb_lineno])))
+                Common.logger.write_main_log(str(e))
             if self.__thread is not None:
                 st_time = time.time()
                 # если поток все еще живой, ждем и закрываем сокет
                 while self.__thread.is_alive():
                     if time.time() - st_time > 0.2:
                         try:
                             self.__sct.close()
                         except (OSError, Exception) as e:
                             exc_type, exc_obj, exc_tb = sys.exc_info()
                             file_name = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-                            InfoHolder.logger.write_main_log(" ".join(map(str,
+                            Common.logger.write_main_log(" ".join(map(str,
                                                                           [exc_type, file_name, exc_tb.tb_lineno])))
-                            InfoHolder.logger.write_main_log(str(e))
+                            Common.logger.write_main_log(str(e))
                         st_time = time.time()
 
 
 class TalkPort:
     def __init__(self, port: int, event_handler=None, delay: float = 0.004, is_camera: bool = False):
         self.__port = port
 
@@ -125,75 +119,69 @@
 
     def talking(self):
         self.__sct = socket.socket(socket.AF_INET, socket.SOCK_STREAM, socket.IPPROTO_TCP)
         self.__sct.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self.__sct.bind(('0.0.0.0', self.__port))
         self.__sct.listen(1)
 
-        try:
-            connection_out = self.__sct.accept()[0].makefile('rwb')
-            handler = SplitFrames(connection_out)
-            while not self.__stop_thread:
-                try:
-                    self.event_call()
-
-                    if self.__is_camera:
-                        handler.write(self.out_string.encode("utf-8"))
-                        _ = handler.read()
-                        handler.write(self.out_bytes)
-                        self.str_from_client = handler.read()
-                    else:
-                        handler.write(self.out_string.encode("utf-8"))
-                        self.str_from_client = handler.read().decode("utf-8")
-
-                    # задержка для слабых компов
-                    time.sleep(self.__delay)
-                except (ConnectionAbortedError, BrokenPipeError) as e:
-                    # возникает при отключении сокета
-                    exc_type, exc_obj, exc_tb = sys.exc_info()
-                    file_name = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-                    InfoHolder.logger.write_main_log(" ".join(map(str, [exc_type, file_name, exc_tb.tb_lineno])))
-                    InfoHolder.logger.write_main_log(str(e))
-                    break
-            self.__sct.shutdown(socket.SHUT_RDWR)
-            self.__sct.close()
-        except Exception as e:
-            exc_type, exc_obj, exc_tb = sys.exc_info()
-            file_name = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-            InfoHolder.logger.write_main_log(" ".join(map(str, [exc_type, file_name, exc_tb.tb_lineno])))
-            InfoHolder.logger.write_main_log(str(e))
+        connection_out = self.__sct.accept()[0].makefile('rwb')
+        handler = SplitFrames(connection_out)
+        while not self.__stop_thread:
+            try:
+                self.event_call()
+
+                if self.__is_camera:
+                    handler.write(self.out_string.encode("utf-8"))
+                    _ = handler.read()
+                    handler.write(self.out_bytes)
+                    self.str_from_client = handler.read()
+                else:
+                    handler.write(self.out_string.encode("utf-8"))
+                    self.str_from_client = handler.read().decode("utf-8")
+
+                # задержка для слабых компов
+                time.sleep(self.__delay)
+            except (ConnectionAbortedError, BrokenPipeError) as e:
+                # возникает при отключении сокета
+                exc_type, exc_obj, exc_tb = sys.exc_info()
+                file_name = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
+                Common.logger.write_main_log(" ".join(map(str, [exc_type, file_name, exc_tb.tb_lineno])))
+                Common.logger.write_main_log(str(e))
+                break
+        self.__sct.shutdown(socket.SHUT_RDWR)
+        self.__sct.close()
 
     def reset_out(self):
         self.out_string = 'null'
         self.str_from_client = '-1'
 
     def stop_talking(self):
         self.__stop_thread = True
         self.reset_out()
         if self.__sct is not None:
             try:
                 self.__sct.shutdown(socket.SHUT_RDWR)
             except (OSError, Exception) as e:
                 exc_type, exc_obj, exc_tb = sys.exc_info()
                 file_name = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-                InfoHolder.logger.write_main_log(" ".join(map(str, [exc_type, file_name, exc_tb.tb_lineno])))
-                InfoHolder.logger.write_main_log(str(e))
+                Common.logger.write_main_log(" ".join(map(str, [exc_type, file_name, exc_tb.tb_lineno])))
+                Common.logger.write_main_log(str(e))
             if self.__thread is not None:
                 st_time = time.time()
                 # если поток все еще живой, ждем и закрываем сокет
                 while self.__thread.is_alive():
                     if time.time() - st_time > 0.2:
                         try:
                             self.__sct.close()
                         except (OSError, Exception) as e:
                             exc_type, exc_obj, exc_tb = sys.exc_info()
                             file_name = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-                            InfoHolder.logger.write_main_log(" ".join(map(str,
+                            Common.logger.write_main_log(" ".join(map(str,
                                                                           [exc_type, file_name, exc_tb.tb_lineno])))
-                            InfoHolder.logger.write_main_log(str(e))
+                            Common.logger.write_main_log(str(e))
                         st_time = time.time()
 
 
 class ConnectionHelper:
     out_variables_channel: TalkPort
     in_variables_channel: ListenPort
     chart_variables_channel: TalkPort
@@ -242,95 +230,95 @@
         cls.outcad_variables_channel.stop_talking()
         cls.rpi_variables_channel.stop_talking()
         cls.camera_variables_channel.stop_talking()
         cls.joy_variables_channel.stop_listening()
 
     @classmethod
     def on_out_vars(cls):
-        without_charts = [i for i in InfoHolder.variables_array if i.type_ != ShuffleVariable.CHART_TYPE]
+        without_charts = [i for i in ShufflecadHolder.variables_array if i.type_ != ShuffleVariable.CHART_TYPE]
         if len(without_charts) > 0:
             strings = ["{0};{1};{2};{3}".format(i.name, i.value, i.type_, i.direction) for i in without_charts]
             cls.out_variables_channel.out_string = "&".join(strings)
         else:
             cls.out_variables_channel.out_string = "null"
 
     @classmethod
     def on_in_vars(cls):
         if len(cls.in_variables_channel.out_string) > 0 and cls.in_variables_channel.out_string != "null":
             string_vars = cls.in_variables_channel.out_string.split("&")
             for i in string_vars:
                 name, value = i.split(";")
-                curr_var = [x for x in InfoHolder.variables_array if x.name == name][0]
+                curr_var = [x for x in ShufflecadHolder.variables_array if x.name == name][0]
                 curr_var.value = value
 
     @classmethod
     def on_chart_vars(cls):
-        only_charts = [i for i in InfoHolder.variables_array if i.type_ == ShuffleVariable.CHART_TYPE]
+        only_charts = [i for i in ShufflecadHolder.variables_array if i.type_ == ShuffleVariable.CHART_TYPE]
         if len(only_charts) > 0:
             strings = ["{0};{1}".format(i.name, i.value) for i in only_charts]
             cls.chart_variables_channel.out_string = "&".join(strings)
         else:
             cls.chart_variables_channel.out_string = "null"
 
     @classmethod
     def on_outcad_vars(cls):
-        if len(InfoHolder.get_print_array()) > 0:
-            to_print: str = "&".join(InfoHolder.get_print_array())
+        if len(ShufflecadHolder.get_print_array()) > 0:
+            to_print: str = "&".join(ShufflecadHolder.get_print_array())
             cls.outcad_variables_channel.out_string = to_print
-            InfoHolder.clear_print_array()
+            ShufflecadHolder.clear_print_array()
         else:
             cls.outcad_variables_channel.out_string = "null"
 
     @classmethod
     def on_rpi_vars(cls):
-        out_lst = [InfoHolder.temperature, InfoHolder.memory_load,
-                   InfoHolder.cpu_load, InfoHolder.power, InfoHolder.spi_time_dev,
-                   InfoHolder.rx_spi_time_dev, InfoHolder.tx_spi_time_dev,
-                   InfoHolder.spi_count_dev, InfoHolder.com_time_dev,
-                   InfoHolder.rx_com_time_dev, InfoHolder.tx_com_time_dev,
-                   InfoHolder.com_count_dev]
-        cls.rpi_variables_channel.out_string = "&".join(out_lst)
+        out_lst = [Common.temperature, Common.memory_load,
+                   Common.cpu_load, Common.power, Common.spi_time_dev,
+                   Common.rx_spi_time_dev, Common.tx_spi_time_dev,
+                   Common.spi_count_dev, Common.com_time_dev,
+                   Common.rx_com_time_dev, Common.tx_com_time_dev,
+                   Common.com_count_dev]
+        cls.rpi_variables_channel.out_string = "&".join(map(str, out_lst))
 
     __camera_toggler = 0
 
     @classmethod
     def on_camera_vars(cls):
         # Logger.write_main_log(str(len(Shared.InfoHolder.camera_variables_array)))
-        if len(InfoHolder.camera_variables_array) > 0:
+        if len(ShufflecadHolder.camera_variables_array) > 0:
             if int(cls.camera_variables_channel.str_from_client) == -1:
-                curr_var = InfoHolder.camera_variables_array[cls.__camera_toggler]
+                curr_var = ShufflecadHolder.camera_variables_array[cls.__camera_toggler]
                 to_send_first = "{0};{1}".format(curr_var.name, ":".join(map(str, curr_var.shape)))
                 # Logger.write_main_log(to_send_first)
 
                 cls.camera_variables_channel.out_string = to_send_first
                 cls.camera_variables_channel.out_bytes = curr_var.get_value()
 
                 # Logger.write_main_log("sent")
 
-                if cls.__camera_toggler + 1 == len(InfoHolder.camera_variables_array):
+                if cls.__camera_toggler + 1 == len(ShufflecadHolder.camera_variables_array):
                     cls.__camera_toggler = 0
                 else:
                     cls.__camera_toggler += 1
             else:
-                curr_var = InfoHolder.camera_variables_array[int(cls.camera_variables_channel.str_from_client)]
+                curr_var = ShufflecadHolder.camera_variables_array[int(cls.camera_variables_channel.str_from_client)]
                 to_send_first = "{0};{1}".format(curr_var.name, ":".join(map(str, curr_var.shape)))
 
                 cls.camera_variables_channel.out_string = to_send_first
                 cls.camera_variables_channel.out_bytes = curr_var.get_value()
         else:
             cls.camera_variables_channel.out_string = "null"
             cls.camera_variables_channel.out_bytes = b'null'
 
     @classmethod
     def on_joy_vars(cls):
         if len(cls.joy_variables_channel.out_string) > 0 and cls.joy_variables_channel.out_string != "null":
             string_vars = cls.joy_variables_channel.out_string.split("&")
             for i in string_vars:
                 name, value = i.split(";")
-                InfoHolder.joystick_values[name] = int(value)
+                ShufflecadHolder.joystick_values[name] = int(value)
 
 
 class SplitFrames(object):
     def __init__(self, connection):
         self.connection = connection
         self.stream = io.BytesIO()
         self.count = 0
```

### Comparing `robocad-py-0.0.2.3/robocad/shufflecad/shared.py` & `robocad-py-1.0.2.2/robocad/shufflecad/shufflecad_holder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+
 from typing import List
+
 import cv2
 import numpy as np
 
 
 class ShuffleVariable(object):
     FLOAT_TYPE: str = "float"
     STRING_TYPE: str = "string"
@@ -54,45 +56,25 @@
 
     def set_mat(self, mat) -> None:
         if mat is not None:
             self.shape = (mat.shape[1], mat.shape[0])
             self.value = mat
 
 
-class InfoHolder:
-    # logger object
-    logger = None
-    # control the type of the shufflecad work
-    on_real_robot: bool = True
-
-    power: str = "0"
-
-    # some things
-    spi_time_dev: str = "0"
-    rx_spi_time_dev: str = "0"
-    tx_spi_time_dev: str = "0"
-    spi_count_dev: str = "0"
-    com_time_dev: str = "0"
-    rx_com_time_dev: str = "0"
-    tx_com_time_dev: str = "0"
-    com_count_dev: str = "0"
-    temperature: str = "0"
-    memory_load: str = "0"
-    cpu_load: str = "0"
-
+class ShufflecadHolder:
     variables_array: List[ShuffleVariable] = list()
     camera_variables_array: List[CameraVariable] = list()
     joystick_values: dict = dict()
     print_array: List[str] = list()
 
     # outcad methods
     @classmethod
-    def print_to_log(cls, var: str, color: str = "#e0d4ab") -> None:
-        cls.print_array.append(var + color)
+    def print_to_log(cls, var: str) -> None:
+        ShufflecadHolder.print_array.append(var)
 
     @classmethod
     def get_print_array(cls) -> List[str]:
-        return cls.print_array
+        return ShufflecadHolder.print_array
 
     @classmethod
     def clear_print_array(cls) -> None:
-        cls.print_array = list()
+        ShufflecadHolder.print_array = list()
```

### Comparing `robocad-py-0.0.2.3/robocad_py.egg-info/PKG-INFO` & `robocad-py-1.0.2.2/robocad_py.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.1
 Name: robocad-py
-Version: 0.0.2.3
+Version: 1.0.2.2
 Summary: python lib for real and virtual robots
-Home-page: https://github.com/CrackAndDie/robocad-py
+Home-page: https://github.com/Soft-V/robocad-py
 Author: Airat Abdrakov
 Author-email: softvery@yandex.ru
 License: MIT
 Description: Python library for real and virtual robots
         
         # Change Log
```

### Comparing `robocad-py-0.0.2.3/robocad_py.egg-info/SOURCES.txt` & `robocad-py-1.0.2.2/robocad_py.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 setup.py
 robocad/__init__.py
-robocad/robocad.py
-robocad/vex.py
-robocad/pycad/COM.py
-robocad/pycad/SPI.py
-robocad/pycad/__init__.py
-robocad/pycad/shared.py
-robocad/robocadSim/__init__.py
-robocad/robocadSim/connection.py
-robocad/robocadSim/connection_helper_vmx_titan.py
+robocad/common.py
+robocad/studica.py
+robocad/internal/__init__.py
+robocad/internal/logger.py
+robocad/internal/studica/COM.py
+robocad/internal/studica/SPI.py
+robocad/internal/studica/__init__.py
+robocad/internal/studica/connection.py
+robocad/internal/studica/connection_base.py
+robocad/internal/studica/connection_real.py
+robocad/internal/studica/connection_sim.py
+robocad/internal/studica/shared.py
 robocad/shufflecad/__init__.py
 robocad/shufflecad/connections.py
-robocad/shufflecad/logger.py
-robocad/shufflecad/shared.py
 robocad/shufflecad/shufflecad.py
+robocad/shufflecad/shufflecad_holder.py
 robocad_py.egg-info/PKG-INFO
 robocad_py.egg-info/SOURCES.txt
 robocad_py.egg-info/dependency_links.txt
 robocad_py.egg-info/requires.txt
 robocad_py.egg-info/top_level.txt
```

### Comparing `robocad-py-0.0.2.3/setup.py` & `robocad-py-1.0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='robocad-py',
-    version='0.0.2.3',
+    version='1.0.2.2',
     description='python lib for real and virtual robots',
     long_description="Python library for real and virtual robots" + '\n\n' + open('CHANGELOG.md').read(),
-    url='https://github.com/CrackAndDie/robocad-py',
+    url='https://github.com/Soft-V/robocad-py',
     author='Airat Abdrakov',
     author_email='softvery@yandex.ru',
     license='MIT',
     classifiers=classifiers,
     keywords=['simulator', 'robotics', 'robot', '3d', 'raspberry', 'control'],
     packages=find_packages(),
     install_requires=['numpy', 'funcad']
```

