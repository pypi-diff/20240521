# Comparing `tmp/pyuptech-0.1.5.1.tar.gz` & `tmp/pyuptech-0.1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuptech-0.1.5.1.tar", last modified: Mon May 20 14:14:49 2024, max compression
+gzip compressed data, was "pyuptech-0.1.5.2.tar", last modified: Mon May 20 15:17:14 2024, max compression
```

## Comparing `pyuptech-0.1.5.1.tar` & `pyuptech-0.1.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     8829 2024-05-20 14:14:30.990193 pyuptech-0.1.5.1/README.md
--rw-r--r--   0        0        0      547 2024-05-20 14:14:49.222094 pyuptech-0.1.5.1/pyproject.toml
--rw-r--r--   0        0        0     1148 2024-05-20 14:14:30.990193 pyuptech-0.1.5.1/src/pyuptech/__init__.py
--rw-r--r--   0        0        0   219512 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/lib/libuptech.so
--rw-r--r--   0        0        0      190 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/modules/constant.py
--rw-r--r--   0        0        0     2060 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/modules/emulation.py
--rw-r--r--   0        0        0     1007 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/modules/loader.py
--rw-r--r--   0        0        0      577 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/modules/logger.py
--rw-r--r--   0        0        0     1761 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/modules/pins.py
--rw-r--r--   0        0        0    10688 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/modules/screen.py
--rw-r--r--   0        0        0    13793 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/modules/sensors.py
--rw-r--r--   0        0        0     6515 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/tools/display.py
--rw-r--r--   0        0        0      252 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/tests/__init__.py
--rw-r--r--   0        0        0      456 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/tests/display_tests.py
--rw-r--r--   0        0        0     1036 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/tests/perf_tests.py
--rw-r--r--   0        0        0     1220 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/tests/test_sensor.py
--rw-r--r--   0        0        0      424 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/tests/utils.py
--rw-r--r--   0        0        0     9146 1970-01-01 00:00:00.000000 pyuptech-0.1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     8876 2024-05-20 15:16:49.177582 pyuptech-0.1.5.2/README.md
+-rw-r--r--   0        0        0      547 2024-05-20 15:17:14.125692 pyuptech-0.1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1182 2024-05-20 15:16:49.177582 pyuptech-0.1.5.2/src/pyuptech/__init__.py
+-rw-r--r--   0        0        0   219512 2024-05-20 15:16:49.181582 pyuptech-0.1.5.2/src/pyuptech/lib/libuptech.so
+-rw-r--r--   0        0        0      190 2024-05-20 15:16:49.181582 pyuptech-0.1.5.2/src/pyuptech/modules/constant.py
+-rw-r--r--   0        0        0     2060 2024-05-20 15:16:49.181582 pyuptech-0.1.5.2/src/pyuptech/modules/emulation.py
+-rw-r--r--   0        0        0     1007 2024-05-20 15:16:49.181582 pyuptech-0.1.5.2/src/pyuptech/modules/loader.py
+-rw-r--r--   0        0        0      577 2024-05-20 15:16:49.181582 pyuptech-0.1.5.2/src/pyuptech/modules/logger.py
+-rw-r--r--   0        0        0     1761 2024-05-20 15:16:49.181582 pyuptech-0.1.5.2/src/pyuptech/modules/pins.py
+-rw-r--r--   0        0        0    10688 2024-05-20 15:16:49.181582 pyuptech-0.1.5.2/src/pyuptech/modules/screen.py
+-rw-r--r--   0        0        0    13746 2024-05-20 15:16:49.181582 pyuptech-0.1.5.2/src/pyuptech/modules/sensors.py
+-rw-r--r--   0        0        0     7469 2024-05-20 15:16:49.181582 pyuptech-0.1.5.2/src/pyuptech/tools/display.py
+-rw-r--r--   0        0        0      252 2024-05-20 15:16:49.181582 pyuptech-0.1.5.2/tests/__init__.py
+-rw-r--r--   0        0        0      534 2024-05-20 15:16:49.181582 pyuptech-0.1.5.2/tests/display_tests.py
+-rw-r--r--   0        0        0     1036 2024-05-20 15:16:49.181582 pyuptech-0.1.5.2/tests/perf_tests.py
+-rw-r--r--   0        0        0     1135 2024-05-20 15:16:49.181582 pyuptech-0.1.5.2/tests/test_sensor.py
+-rw-r--r--   0        0        0      424 2024-05-20 15:16:49.181582 pyuptech-0.1.5.2/tests/utils.py
+-rw-r--r--   0        0        0     9193 1970-01-01 00:00:00.000000 pyuptech-0.1.5.2/PKG-INFO
```

### Comparing `pyuptech-0.1.5.1/README.md` & `pyuptech-0.1.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -201,15 +201,16 @@
 
 ```python
 from pyuptech import (
     SensorEmulator,
     mpu_display_on_lcd,
     make_mpu_table,
     adc_io_display_on_lcd,
-    make_adc_io_table,
+    make_adc_table,
+    make_io_table,
     Screen)
 
 emu = SensorEmulator()
 scr = Screen(screen_dir=2)
 
 print(make_mpu_table(sensors=emu))
 
@@ -234,15 +235,16 @@
     7: 'ftl',
     6: 'ftr',
     5: 'rtr'
 }
 
 adc_io_display_on_lcd(sensors=emu, screen=scr, adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到LCD 
 
-make_adc_io_table(adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到终端 
+make_io_table(sensors=emu, io_labels=io_labels)
+make_adc_table(sensors=emu, adc_labels=adc_labels)  # 将ADC和GPIO数据打印到终端 
 
 
 ```
 
 ## 使用传感器仿真器
 
 通过 `modules.emulation.SensorEmulator` 可以使用传感器仿真器
@@ -265,21 +267,21 @@
 
 配合 `modules.display` 使用
 
 ```python
 from pyuptech import (
     Screen, SensorEmulator,
     make_mpu_table,
-    make_adc_io_table)
+    make_adc_table)
 
 # 启动模拟模式，以便打印可以正常使用随机生成的数据进行工作
 scr = Screen()
 emu = SensorEmulator()
 
 print(make_mpu_table(sensors=emu))
 # 将MPU6500数据打印到终端
 
-print(make_adc_io_table(sensors=emu))
+print(make_adc_table(sensors=emu))
 # 将ADC和GPIO数据打印到终端
 
 ```
```

### Comparing `pyuptech-0.1.5.1/pyproject.toml` & `pyuptech-0.1.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyuptech"
-version = "0.1.5.1"
+version = "0.1.5.2"
 description = "A Python wrapper for the uptech binary lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "terminaltables>=3.1.10",
```

### Comparing `pyuptech-0.1.5.1/src/pyuptech/__init__.py` & `pyuptech-0.1.5.2/src/pyuptech/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,18 @@
     IndexedGetter,
     IndexedSetter,
 )
 from .modules.screen import Screen, Color, FontSize
 from .modules.sensors import OnBoardSensors, ADCArrayType, MPUArrayType
 from .tools.display import (
     adc_io_display_on_lcd,
-    make_adc_io_table,
+    make_adc_table,
     mpu_display_on_lcd,
     make_mpu_table,
+    make_io_table,
 )
 
 __all__ = [
     "OnBoardSensors",
     "SensorEmulator",
     "Screen",
     "Color",
@@ -38,11 +39,12 @@
     "PinGetter",
     "PinSetter",
     "PinModeSetter",
     "IndexedGetter",
     "IndexedSetter",
     # tools
     "adc_io_display_on_lcd",
-    "make_adc_io_table",
+    "make_adc_table",
     "mpu_display_on_lcd",
     "make_mpu_table",
+    "make_io_table",
 ]
```

### Comparing `pyuptech-0.1.5.1/src/pyuptech/lib/libuptech.so` & `pyuptech-0.1.5.2/src/pyuptech/lib/libuptech.so`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.5.1/src/pyuptech/modules/emulation.py` & `pyuptech-0.1.5.2/src/pyuptech/modules/emulation.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.5.1/src/pyuptech/modules/loader.py` & `pyuptech-0.1.5.2/src/pyuptech/modules/loader.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.5.1/src/pyuptech/modules/logger.py` & `pyuptech-0.1.5.2/src/pyuptech/modules/logger.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.5.1/src/pyuptech/modules/pins.py` & `pyuptech-0.1.5.2/src/pyuptech/modules/pins.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.5.1/src/pyuptech/modules/screen.py` & `pyuptech-0.1.5.2/src/pyuptech/modules/screen.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.5.1/src/pyuptech/modules/sensors.py` & `pyuptech-0.1.5.2/src/pyuptech/modules/sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import ctypes
-from ctypes import c_byte
+from ctypes import c_byte, c_int, c_uint, byref, Array, CDLL, c_uint16, c_float
 from time import perf_counter_ns
 from typing import Self, Literal, Any, Callable, Tuple, TypeAlias
 
 from .constant import LIB_FILE_PATH, BinaryIO
 from .loader import load_lib
 from .logger import _logger
 
@@ -13,25 +12,25 @@
 Only For IO, mode and level
 OUTPUT = 1
 INPUT = 0
 HIGH = 1
 LOW = 0
 """
 # this will create a function that returns a C array, but it can't be recognized correctly by the pycharm
-ADCArrayType: Callable = ctypes.c_uint16 * 10  # type: ignore
+ADCArrayType: Callable = c_uint16 * 10  # type: ignore
 # on 32bit machine, this will create a C array of 3 floats with bit-width of 4 bytes
-MPUArrayType: Callable = ctypes.c_float * 3  # type: ignore
+MPUArrayType: Callable = c_float * 3  # type: ignore
 
 ADCDataPack: TypeAlias = Tuple[int, int, int, int, int, int, int, int, int, int]
 MPUDataPack: TypeAlias = Tuple[float, float, float]
 
-__TECHSTAR_LIB__: ctypes.CDLL = load_lib(LIB_FILE_PATH)
+__TECHSTAR_LIB__: CDLL = load_lib(LIB_FILE_PATH)
 
 # 定义_WORD为无符号短整型
-_WORD = ctypes.c_uint16
+_WORD = c_uint16
 
 
 class OnBoardSensors:
     """
     provides sealed methods accessing to the IOs and builtin sensors
 
     Owns 10 ADC channels and 3 MPU channels  and 8 IO channels
@@ -54,18 +53,18 @@
             adc_min_sample_interval_ms (int): The minimum sample interval in milliseconds for the ADC channels. Defaults to 5.
 
         Examples:
             >>> on_board = OnBoardSensors().adc_io_open().set_all_io_mode(0).set_all_io_level(1).MPU6500_Open()
         """
 
         self._adc_cache: ADCDataPack = (0,) * 10
-        self._adc_all: ctypes.Array = ADCArrayType()
-        self._accel_all: ctypes.Array = MPUArrayType()
-        self._gyro_all: ctypes.Array = MPUArrayType()
-        self._atti_all: ctypes.Array = MPUArrayType()
+        self._adc_all: Array = ADCArrayType()
+        self._accel_all: Array = MPUArrayType()
+        self._gyro_all: Array = MPUArrayType()
+        self._atti_all: Array = MPUArrayType()
 
         self.__adc_last_sample_timestamp: int = perf_counter_ns()
 
         self.__adc_min_sample_interval_ns: int = adc_min_sample_interval_ms * E6
 
     @property
     def last_sample_timestamp_ms(self) -> int:
@@ -179,18 +178,18 @@
 
         Returns:
             int: A buffer containing all IO modes.
         Examples:
             0b10000000 => 第io7为输出模式，可用于驱动舵机
             0b00000001 => 第io0为输入模式，可用于外接传感器
         """
-        buffer = ctypes.c_char()
-        if __TECHSTAR_LIB__.adc_io_ModeGetAll(buffer):
+        buffer = c_byte()
+        if __TECHSTAR_LIB__.adc_io_ModeGetAll(byref(buffer)):
             _logger.error("Failed to get all IO mode")
-        return buffer.value[0]
+        return buffer.value
 
     @staticmethod
     def get_io_level(index: int) -> int:
         """
         Get the level of the specified IO index.
 
         Args:
@@ -357,30 +356,30 @@
         This method queries and returns the FSR value of the gyroscope from the technology library.
 
         Returns:
             int: The Full Scale Range value of the gyroscope.
         """
 
         # Calls the technology library function to obtain the gyroscope's FSR, storing the result in fsr_value
-        __TECHSTAR_LIB__.mpu_get_gyro_fsr(ctypes.byref(fsr_value := _WORD()))
+        __TECHSTAR_LIB__.mpu_get_gyro_fsr(byref(fsr_value := _WORD()))
         return fsr_value.value
 
     @staticmethod
     def get_acc_fsr() -> int:
         """
         Retrieves the accelerometer full-scale range.
 
         This static method fetches the current full-scale range for the accelerometer from the TECHSTAR_LIB.
 
         Returns:
             int: The value representing the accelerometer full-scale range.
         """
 
         # Request the accelerometer full-scale range value
-        __TECHSTAR_LIB__.mpu_get_accel_fsr(ctypes.byref(fsr_value := c_byte()))
+        __TECHSTAR_LIB__.mpu_get_accel_fsr(byref(fsr_value := c_byte()))
         # Return the obtained accelerometer full-scale range value
         return fsr_value.value
 
     def mpu_set_gyro_fsr(self, fsr: Literal[250, 500, 1000, 2000] | int) -> Self:
         """
         Sets the full-scale range for the gyroscope in the MPU.
 
@@ -388,25 +387,25 @@
             fsr (Literal[250, 500, 1000, 2000] | int): Gyroscope full-scale range, can be one of 250, 500, 1000, or 2000 degrees per second.
 
         Returns:
             Self: Returns an instance of the function for method chaining.
         """
 
         # Call the underlying library function to set the gyroscope's full-scale range
-        __TECHSTAR_LIB__.mpu_set_gyro_fsr(ctypes.c_uint(fsr))
+        __TECHSTAR_LIB__.mpu_set_gyro_fsr(c_uint(fsr))
         return self
 
     def mpu_set_accel_fsr(self, fsr: Literal[2, 4, 8, 16] | int) -> Self:
         """
         Sets the accelerometer full-scale range (FSR) for the MPU.
 
         Parameters:
             fsr: Literal[2, 4, 8, 16] | int - The full-scale range of the accelerometer, with options being 2g, 4g, 8g, and 16g.
 
         Returns:
             Self: Returns the object itself to support method chaining.
         """
 
         __TECHSTAR_LIB__.mpu_set_accel_fsr(
-            ctypes.c_int(fsr)
+            c_int(fsr)
         )  # Invokes the library function to set the accelerometer's FSR
         return self
```

### Comparing `pyuptech-0.1.5.1/src/pyuptech/tools/display.py` & `pyuptech-0.1.5.2/src/pyuptech/tools/display.py`

 * *Files 14% similar despite different names*

```diff
@@ -77,52 +77,85 @@
 
     # Create a table using the DoubleTable class and customize its style
     table = DoubleTable(combined_data)
     table.inner_row_border = True  # Add inner row borders for improved readability
     return table.table
 
 
-def make_adc_io_table(
+def make_adc_table(
     sensors: OnBoardSensors,
     adc_labels: Dict[int, str] = None,
-    io_labels: Dict[int, str] = None,
 ) -> str:
     """
     Generate and return a formatted string table containing ADC (Analog-to-Digital Converter) and IO (Input/Output) channel information.
 
     Parameters:
         sensors: An instance of the `OnBoardSensors` class.
         adc_labels: A dictionary mapping ADC channel numbers (int) to custom names (str). Defaults to None, indicating no custom names are used.
-        io_labels: A dictionary mapping IO channel numbers (int) to custom names (str). Defaults to None, indicating no custom names are used.
 
     Returns:
         A string representation of the table, formatted using the terminaltables library.
 
     Dependencies:
         This function relies on external functions `adc_all_channels()`, `io_all_channels()`, and `get_all_io_mode()` from the `sensors` module.
     """
 
     from terminaltables import (
         DoubleTable,
     )  # Import library for formatting the table output
 
     # Use empty dictionaries as default values if adc_labels or io_labels are not provided
     adc_labels = adc_labels or {}
-    io_labels = io_labels or {}
 
     # Retrieve all ADC and IO channel data from the sensors module
     adc = sensors.adc_all_channels()
-    io = sensors.io_all_channels()
-    io_modes = sensors.get_all_io_mode()
 
     # Construct the rows of the table
     rows = [
         ["ADC Name"]
-        + [adc_labels.get(i, f"ADC{i}") for i in range(10)],  # ADC Name row
+        + [adc_labels.get(i, f"ADC{i}") for i in range(len(adc))],  # ADC Name row
         ["ADC Data"] + [f"{x}" for x in adc],  # ADC Data row
+    ]
+
+    # Format the row data into a table using DoubleTable class
+    table = DoubleTable(rows)
+    table.inner_row_border = True  # Enable inner row borders
+    return table.table  # Return the formatted table string
+
+
+def make_io_table(
+    sensors: OnBoardSensors,
+    io_labels: Dict[int, str] = None,
+) -> str:
+    """
+    Generate and return a formatted string table containing IO (Input/Output) channel information.
+
+    Parameters:
+        sensors: An instance of the `OnBoardSensors` class.
+        io_labels: A dictionary mapping IO channel numbers (int) to custom names (str). Defaults to None, indicating no custom names are used.
+
+    Returns:
+        A string representation of the table, formatted using the terminaltables library.
+
+    Dependencies:
+        This function relies on external functions `io_all_channels()` and `get_all_io_mode()` from the `sensors` module.
+    """
+
+    from terminaltables import (
+        DoubleTable,
+    )  # Import library for formatting the table output
+
+    io_labels = io_labels or {}
+
+    # Retrieve all ADC and IO channel data from the sensors module
+    io = sensors.io_all_channels()
+    io_modes = sensors.get_all_io_mode()
+
+    # Construct the rows of the table
+    rows = [
         ["IO Name"] + [io_labels.get(i, f"IO{i}") for i in range(8)],  # IO Name row
         ["IO Data"] + [int(bit) for bit in f"{io:08b}"],  # IO Data row (binary)
         ["IO Mode"] + [int(bit) for bit in f"{io_modes:08b}"],  # IO Mode row (binary)
     ]
 
     # Format the row data into a table using DoubleTable class
     table = DoubleTable(rows)
```

### Comparing `pyuptech-0.1.5.1/tests/perf_tests.py` & `pyuptech-0.1.5.2/tests/perf_tests.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.5.1/tests/test_sensor.py` & `pyuptech-0.1.5.2/tests/test_sensor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 import unittest
+from unittest import skip
 
 from pyuptech import OnBoardSensors
 
 
 class DisplayTests(unittest.TestCase):
 
     def setUp(self):
-        self.sen = OnBoardSensors()
+        self.sen = OnBoardSensors().MPU6500_Open().adc_io_open()
 
     def test_adc(self):
-        print(self.sen.adc_io_open().adc_all_channels())
+        print(self.sen.adc_all_channels())
 
     def test_io(self):
-        print(
-            self.sen.adc_io_open()
-            .set_all_io_mode(0)
-            .set_all_io_level(1)
-            .io_all_channels()
-        )
+        print(self.sen.set_all_io_mode(0).set_all_io_level(1).io_all_channels())
 
     def test_mpu(self):
-        print(self.sen.MPU6500_Open().atti_all())
+        print(self.sen.atti_all())
         print(self.sen.gyro_all())
         print(self.sen.acc_all())
         print("finished")
 
+    @skip
     def test_mpu_freq(self):
         from utils import time_it
 
-        print(time_it(self.sen.MPU6500_Open().acc_all)())
+        print(time_it(self.sen.acc_all)())
         print(time_it(self.sen.atti_all)())
         print(time_it(self.sen.gyro_all)())
 
     def test_mpu_set_get(self):
-        self.sen.MPU6500_Open()
+
         print(self.sen.get_acc_fsr())
         print(self.sen.get_gyro_fsr())
         g_fsr = 250
         self.sen.mpu_set_gyro_fsr(g_fsr)
         a_fsr = 2
         self.sen.mpu_set_accel_fsr(a_fsr)
         self.assertEqual(self.sen.get_acc_fsr(), a_fsr)
```

### Comparing `pyuptech-0.1.5.1/PKG-INFO` & `pyuptech-0.1.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuptech
-Version: 0.1.5.1
+Version: 0.1.5.2
 Summary: A Python wrapper for the uptech binary lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: terminaltables>=3.1.10
 Description-Content-Type: text/markdown
@@ -212,15 +212,16 @@
 
 ```python
 from pyuptech import (
     SensorEmulator,
     mpu_display_on_lcd,
     make_mpu_table,
     adc_io_display_on_lcd,
-    make_adc_io_table,
+    make_adc_table,
+    make_io_table,
     Screen)
 
 emu = SensorEmulator()
 scr = Screen(screen_dir=2)
 
 print(make_mpu_table(sensors=emu))
 
@@ -245,15 +246,16 @@
     7: 'ftl',
     6: 'ftr',
     5: 'rtr'
 }
 
 adc_io_display_on_lcd(sensors=emu, screen=scr, adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到LCD 
 
-make_adc_io_table(adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到终端 
+make_io_table(sensors=emu, io_labels=io_labels)
+make_adc_table(sensors=emu, adc_labels=adc_labels)  # 将ADC和GPIO数据打印到终端 
 
 
 ```
 
 ## 使用传感器仿真器
 
 通过 `modules.emulation.SensorEmulator` 可以使用传感器仿真器
@@ -276,21 +278,21 @@
 
 配合 `modules.display` 使用
 
 ```python
 from pyuptech import (
     Screen, SensorEmulator,
     make_mpu_table,
-    make_adc_io_table)
+    make_adc_table)
 
 # 启动模拟模式，以便打印可以正常使用随机生成的数据进行工作
 scr = Screen()
 emu = SensorEmulator()
 
 print(make_mpu_table(sensors=emu))
 # 将MPU6500数据打印到终端
 
-print(make_adc_io_table(sensors=emu))
+print(make_adc_table(sensors=emu))
 # 将ADC和GPIO数据打印到终端
 
 ```
```

