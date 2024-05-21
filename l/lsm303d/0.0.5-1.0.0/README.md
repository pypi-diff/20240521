# Comparing `tmp/lsm303d-0.0.5.tar.gz` & `tmp/lsm303d-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lsm303d-0.0.5.tar", last modified: Thu Sep 12 14:17:10 2019, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `lsm303d-0.0.5.tar` & `lsm303d-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-09-12 14:17:10.000000 lsm303d-0.0.5/
--rw-r--r--   0 pi        (1000) pi        (1000)     1699 2019-09-12 14:17:10.000000 lsm303d-0.0.5/PKG-INFO
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-09-12 14:17:10.000000 lsm303d-0.0.5/lsm303d.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)        8 2019-09-12 14:17:10.000000 lsm303d-0.0.5/lsm303d.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1699 2019-09-12 14:17:10.000000 lsm303d-0.0.5/lsm303d.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2019-09-12 14:17:10.000000 lsm303d-0.0.5/lsm303d.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       17 2019-09-12 14:17:10.000000 lsm303d-0.0.5/lsm303d.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      241 2019-09-12 14:17:10.000000 lsm303d-0.0.5/lsm303d.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      109 2019-09-12 10:44:22.000000 lsm303d-0.0.5/MANIFEST.in
--rw-r--r--   0 pi        (1000) pi        (1000)      412 2019-09-12 10:44:22.000000 lsm303d-0.0.5/README.rst
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-09-12 14:17:10.000000 lsm303d-0.0.5/lsm303d/
--rw-r--r--   0 pi        (1000) pi        (1000)    17639 2019-09-12 14:15:32.000000 lsm303d-0.0.5/lsm303d/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)      248 2019-09-12 14:14:57.000000 lsm303d-0.0.5/CHANGELOG.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1070 2019-09-12 10:44:22.000000 lsm303d-0.0.5/LICENSE.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      134 2019-09-12 14:17:10.000000 lsm303d-0.0.5/setup.cfg
--rwxr-xr-x   0 pi        (1000) pi        (1000)     2117 2019-09-12 14:15:17.000000 lsm303d-0.0.5/setup.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 lsm303d-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 lsm303d-1.0.0/Makefile
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 lsm303d-1.0.0/README.md
+-rwxr-xr-x   0        0        0     2050 2020-02-02 00:00:00.000000 lsm303d-1.0.0/check.sh
+-rwxr-xr-x   0        0        0     9720 2020-02-02 00:00:00.000000 lsm303d-1.0.0/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 lsm303d-1.0.0/requirements-dev.txt
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 lsm303d-1.0.0/test.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 lsm303d-1.0.0/tox.ini
+-rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 lsm303d-1.0.0/uninstall.sh
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 lsm303d-1.0.0/examples/README.md
+-rwxr-xr-x   0        0        0      276 2020-02-02 00:00:00.000000 lsm303d-1.0.0/examples/accelerometer.py
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 lsm303d-1.0.0/examples/magnetometer.py
+-rw-r--r--   0        0        0    17697 2020-02-02 00:00:00.000000 lsm303d-1.0.0/lsm303d/__init__.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 lsm303d-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 lsm303d-1.0.0/tests/test_setup.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 lsm303d-1.0.0/tests/tools.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 lsm303d-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lsm303d-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 lsm303d-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 lsm303d-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lsm303d-0.0.5/lsm303d/__init__.py` & `lsm303d-1.0.0/lsm303d/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from i2cdevice import Device, Register, BitField, _int_to_bytes
-from i2cdevice.adapter import Adapter, LookupAdapter, U16ByteSwapAdapter
 import struct
 
+from i2cdevice import BitField, Device, Register, _int_to_bytes
+from i2cdevice.adapter import Adapter, LookupAdapter, U16ByteSwapAdapter
 
-__version__ = '0.0.5'
+__version__ = "1.0.0"
 
 
 class TemperatureAdapter(Adapter):
     """
     Decode the two's compliment, right-justified, 12-bit temperature value.
     1LSb = 8degC
     """
@@ -33,408 +33,410 @@
 
 class LSM303D:
     def __init__(self, i2c_addr=0x1D, i2c_dev=None):
         self._i2c_addr = i2c_addr
         self._i2c_dev = i2c_dev
         self._lsm303d = Device([0x1D, 0x1E], i2c_dev=self._i2c_dev, bit_width=8, registers=(
 
-            Register('TEMPERATURE', 0x05 | 0x80, fields=(
-                BitField('temperature', 0xFFFF, adapter=TemperatureAdapter()),
+            Register("TEMPERATURE", 0x05 | 0x80, fields=(
+                BitField("temperature", 0xFFFF, adapter=TemperatureAdapter()),
             ), bit_width=16),
 
             # Magnetometer interrupt status
-            Register('MAGNETOMETER_STATUS', 0x07, fields=(
-                BitField('xdata', 0b00000001),
-                BitField('ydata', 0b00000010),
-                BitField('zdata', 0b00000100),
-                BitField('data', 0b00001000),
-                BitField('xoverrun', 0b00010000),
-                BitField('yoverrun', 0b00100000),
-                BitField('zoverrun', 0b01000000),
-                BitField('overrun', 0b10000000),
+            Register("MAGNETOMETER_STATUS", 0x07, fields=(
+                BitField("xdata", 0b00000001),
+                BitField("ydata", 0b00000010),
+                BitField("zdata", 0b00000100),
+                BitField("data", 0b00001000),
+                BitField("xoverrun", 0b00010000),
+                BitField("yoverrun", 0b00100000),
+                BitField("zoverrun", 0b01000000),
+                BitField("overrun", 0b10000000),
             )),
 
-            Register('MAGNETOMETER', 0x08 | 0x80, fields=(
-                BitField('x', 0xFFFF00000000, adapter=S16ByteSwapAdapter()),
-                BitField('y', 0x0000FFFF0000, adapter=S16ByteSwapAdapter()),
-                BitField('z', 0x00000000FFFF, adapter=S16ByteSwapAdapter()),
+            Register("MAGNETOMETER", 0x08 | 0x80, fields=(
+                BitField("x", 0xFFFF00000000, adapter=S16ByteSwapAdapter()),
+                BitField("y", 0x0000FFFF0000, adapter=S16ByteSwapAdapter()),
+                BitField("z", 0x00000000FFFF, adapter=S16ByteSwapAdapter()),
             ), bit_width=8 * 6),
 
-            Register('WHOAMI', 0x0F, fields=(
-                BitField('id', 0xFF),
+            Register("WHOAMI", 0x0F, fields=(
+                BitField("id", 0xFF),
             )),
 
-            Register('MAGNETOMETER_INTERRUPT', 0x12, fields=(
-                BitField('enable', 0b00000001),
-                BitField('enable_4d', 0b00000010),
-                BitField('latch', 0b00000100),
-                BitField('polarity', 0b00001000),    # 0 = active-low, 1 = active-high
-                BitField('pin_config', 0b00010000),  # 0 = push-pull, 1 = open-drain
-                BitField('z_enable', 0b00100000),
-                BitField('y_enable', 0b01000000),
-                BitField('x_enable', 0b10000000),
-            )),
-
-            Register('MAGNETOMETER_INTERRUPT_SOURCE', 0x13, fields=(
-                BitField('event', 0b00000001),
-                BitField('overflow', 0b00000010),
-                BitField('z_negative', 0b00000100),
-                BitField('y_negative', 0b00001000),
-                BitField('x_negative', 0b00010000),
-                BitField('z_positive', 0b00100000),
-                BitField('y_positive', 0b01000000),
-                BitField('x_positive', 0b10000000),
+            Register("MAGNETOMETER_INTERRUPT", 0x12, fields=(
+                BitField("enable", 0b00000001),
+                BitField("enable_4d", 0b00000010),
+                BitField("latch", 0b00000100),
+                BitField("polarity", 0b00001000),    # 0 = active-low, 1 = active-high
+                BitField("pin_config", 0b00010000),  # 0 = push-pull, 1 = open-drain
+                BitField("z_enable", 0b00100000),
+                BitField("y_enable", 0b01000000),
+                BitField("x_enable", 0b10000000),
+            )),
+
+            Register("MAGNETOMETER_INTERRUPT_SOURCE", 0x13, fields=(
+                BitField("event", 0b00000001),
+                BitField("overflow", 0b00000010),
+                BitField("z_negative", 0b00000100),
+                BitField("y_negative", 0b00001000),
+                BitField("x_negative", 0b00010000),
+                BitField("z_positive", 0b00100000),
+                BitField("y_positive", 0b01000000),
+                BitField("x_positive", 0b10000000),
             )),
 
-            Register('MAGNETOMETER_INTERRUPT_THRESHOLD', 0x14 | 0x80, fields=(
-                BitField('threshold', 0xFFFF, adapter=U16ByteSwapAdapter()),
+            Register("MAGNETOMETER_INTERRUPT_THRESHOLD", 0x14 | 0x80, fields=(
+                BitField("threshold", 0xFFFF, adapter=U16ByteSwapAdapter()),
             ), bit_width=16),
 
-            Register('MAGNETOMETER_OFFSET', 0x16 | 0x80, fields=(
-                BitField('x', 0xFFFF00000000, adapter=S16ByteSwapAdapter()),
-                BitField('y', 0x0000FFFF0000, adapter=S16ByteSwapAdapter()),
-                BitField('z', 0x00000000FFFF, adapter=S16ByteSwapAdapter()),
+            Register("MAGNETOMETER_OFFSET", 0x16 | 0x80, fields=(
+                BitField("x", 0xFFFF00000000, adapter=S16ByteSwapAdapter()),
+                BitField("y", 0x0000FFFF0000, adapter=S16ByteSwapAdapter()),
+                BitField("z", 0x00000000FFFF, adapter=S16ByteSwapAdapter()),
             ), bit_width=8 * 6),
 
-            Register('HP_ACCELEROMETER_REFERENCE', 0x1c | 0x80, fields=(
-                BitField('x', 0xFF0000),
-                BitField('y', 0x00FF00),
-                BitField('z', 0x0000FF),
+            Register("HP_ACCELEROMETER_REFERENCE", 0x1c | 0x80, fields=(
+                BitField("x", 0xFF0000),
+                BitField("y", 0x00FF00),
+                BitField("z", 0x0000FF),
             ), bit_width=8 * 3),
 
-            Register('CONTROL0', 0x1f, fields=(
-                BitField('int2_high_pass', 0b00000001),
-                BitField('int1_high_pass', 0b00000010),
-                BitField('click_high_pass', 0b00000100),
-                BitField('fifo_threshold', 0b00100000),
-                BitField('fifo_enable', 0b01000000),
-                BitField('reboot_memory', 0b10000000),
+            Register("CONTROL0", 0x1f, fields=(
+                BitField("int2_high_pass", 0b00000001),
+                BitField("int1_high_pass", 0b00000010),
+                BitField("click_high_pass", 0b00000100),
+                BitField("fifo_threshold", 0b00100000),
+                BitField("fifo_enable", 0b01000000),
+                BitField("reboot_memory", 0b10000000),
             )),
 
-            Register('CONTROL1', 0x20, fields=(
-                BitField('accel_x_enable', 0b00000001),
-                BitField('accel_y_enable', 0b00000010),
-                BitField('accel_z_enable', 0b00000100),
-                BitField('block_data_update', 0b00001000),
-                BitField('accel_data_rate_hz', 0b11110000, adapter=LookupAdapter({
+            Register("CONTROL1", 0x20, fields=(
+                BitField("accel_x_enable", 0b00000001),
+                BitField("accel_y_enable", 0b00000010),
+                BitField("accel_z_enable", 0b00000100),
+                BitField("block_data_update", 0b00001000),
+                BitField("accel_data_rate_hz", 0b11110000, adapter=LookupAdapter({
                     0: 0,
                     3.125: 0b0001,
                     6.25: 0b0010,
                     12.5: 0b0011,
                     25: 0b0100,
                     50: 0b0101,
                     100: 0b0110,
                     200: 0b0111,
                     400: 0b1000,
                     800: 0b1001,
                     1600: 0b1010
                 })),
             )),
 
-            Register('CONTROL2', 0x21, fields=(
-                BitField('serial_interface_mode', 0b00000001),
-                BitField('accel_self_test', 0b00000010),
-                BitField('accel_full_scale_g', 0b00111000, adapter=LookupAdapter({
+            Register("CONTROL2", 0x21, fields=(
+                BitField("serial_interface_mode", 0b00000001),
+                BitField("accel_self_test", 0b00000010),
+                BitField("accel_full_scale_g", 0b00111000, adapter=LookupAdapter({
                     2: 0b000,
                     4: 0b001,
                     6: 0b010,
                     8: 0b011,
                     16: 0b100
                 })),
-                BitField('accel_antialias_bw_hz', 0b11000000, adapter=LookupAdapter({
+                BitField("accel_antialias_bw_hz", 0b11000000, adapter=LookupAdapter({
                     50: 0b11,
                     362: 0b10,
                     194: 0b01,
                     773: 0b00
                 })),
             )),
 
             # Known in the datasheet as CTRL3
-            Register('INTERRUPT1', 0x22, fields=(
-                BitField('enable_fifo_empty', 0b00000001),
-                BitField('enable_accel_dataready', 0b00000010),
-                BitField('enable_accelerometer', 0b00000100),
-                BitField('enable_magnetometer', 0b00001000),
-                BitField('enable_ig2', 0b00010000),
-                BitField('enable_ig1', 0b00100000),
-                BitField('enable_click', 0b01000000),
-                BitField('enable_boot', 0b10000000),
+            Register("INTERRUPT1", 0x22, fields=(
+                BitField("enable_fifo_empty", 0b00000001),
+                BitField("enable_accel_dataready", 0b00000010),
+                BitField("enable_accelerometer", 0b00000100),
+                BitField("enable_magnetometer", 0b00001000),
+                BitField("enable_ig2", 0b00010000),
+                BitField("enable_ig1", 0b00100000),
+                BitField("enable_click", 0b01000000),
+                BitField("enable_boot", 0b10000000),
             )),
 
             # Known in the datasheet as CTRL4
-            Register('INTERRUPT2', 0x23, fields=(
-                BitField('enable_fifo', 0b00000001),
-                BitField('enable_fifo_overrun', 0b00000010),
-                BitField('enable_mag_dataready', 0b00000100),
-                BitField('enable_accel_dataready', 0b00001000),
-                BitField('enable_magnetometer', 0b00010000),
-                BitField('enable_ig2', 0b00100000),
-                BitField('enable_ig1', 0b01000000),
-                BitField('enable_click', 0b10000000),
+            Register("INTERRUPT2", 0x23, fields=(
+                BitField("enable_fifo", 0b00000001),
+                BitField("enable_fifo_overrun", 0b00000010),
+                BitField("enable_mag_dataready", 0b00000100),
+                BitField("enable_accel_dataready", 0b00001000),
+                BitField("enable_magnetometer", 0b00010000),
+                BitField("enable_ig2", 0b00100000),
+                BitField("enable_ig1", 0b01000000),
+                BitField("enable_click", 0b10000000),
             )),
 
-            Register('CONTROL5', 0x24, fields=(
-                BitField('latch_int1', 0b00000001),
-                BitField('latch_int2', 0b00000010),
-                BitField('mag_data_rate_hz', 0b00011100, adapter=LookupAdapter({
+            Register("CONTROL5", 0x24, fields=(
+                BitField("latch_int1", 0b00000001),
+                BitField("latch_int2", 0b00000010),
+                BitField("mag_data_rate_hz", 0b00011100, adapter=LookupAdapter({
                     3.125: 0b000,
                     6.25: 0b001,
                     12.5: 0b010,
                     25: 0b011,
                     50: 0b100,
                     100: 0b101,
                 })),
-                BitField('mag_resolution', 0b01100000),
-                BitField('enable_temperature', 0b10000000),
+                BitField("mag_resolution", 0b01100000),
+                BitField("enable_temperature", 0b10000000),
             )),
 
-            Register('CONTROL6', 0x25, fields=(
-                BitField('mag_full_scale_gauss', 0b01100000, adapter=LookupAdapter({
+            Register("CONTROL6", 0x25, fields=(
+                BitField("mag_full_scale_gauss", 0b01100000, adapter=LookupAdapter({
                     2: 0b00,
                     4: 0b01,
                     8: 0b10,
                     12: 0b11
                 })),
             )),
 
-            Register('CONTROL7', 0x26, fields=(
-                BitField('mag_mode', 0b00000011, adapter=LookupAdapter({'continuous': 0b00, 'single': 0b01, 'off': 0b10})),
-                BitField('mag_lowpowermode', 0b00000100),
-                BitField('temperature_only', 0b00010000),
-                BitField('filter_accel', 0b00100000),
-                BitField('high_pass_mode_accel', 0b11000000),  # See page 39 of lsm303d.pdf
+            Register("CONTROL7", 0x26, fields=(
+                BitField("mag_mode", 0b00000011, adapter=LookupAdapter({"continuous": 0b00, "single": 0b01, "off": 0b10})),
+                BitField("mag_lowpowermode", 0b00000100),
+                BitField("temperature_only", 0b00010000),
+                BitField("filter_accel", 0b00100000),
+                BitField("high_pass_mode_accel", 0b11000000),  # See page 39 of lsm303d.pdf
             )),
 
             # Accelerometer interrupt status register
-            Register('ACCELEROMETER_STATUS', 0x27, fields=(
-                BitField('xdata', 0b00000001),
-                BitField('ydata', 0b00000010),
-                BitField('zdata', 0b00000100),
-                BitField('data', 0b00001000),
-                BitField('xoverrun', 0b00010000),
-                BitField('yoverrun', 0b00100000),
-                BitField('zoverrun', 0b01000000),
-                BitField('overrun', 0b10000000)
+            Register("ACCELEROMETER_STATUS", 0x27, fields=(
+                BitField("xdata", 0b00000001),
+                BitField("ydata", 0b00000010),
+                BitField("zdata", 0b00000100),
+                BitField("data", 0b00001000),
+                BitField("xoverrun", 0b00010000),
+                BitField("yoverrun", 0b00100000),
+                BitField("zoverrun", 0b01000000),
+                BitField("overrun", 0b10000000)
             )),
 
             # X/Y/Z values from accelerometer
-            Register('ACCELEROMETER', 0x28 | 0x80, fields=(
-                BitField('x', 0xFFFF00000000, adapter=S16ByteSwapAdapter()),
-                BitField('y', 0x0000FFFF0000, adapter=S16ByteSwapAdapter()),
-                BitField('z', 0x00000000FFFF, adapter=S16ByteSwapAdapter()),
+            Register("ACCELEROMETER", 0x28 | 0x80, fields=(
+                BitField("x", 0xFFFF00000000, adapter=S16ByteSwapAdapter()),
+                BitField("y", 0x0000FFFF0000, adapter=S16ByteSwapAdapter()),
+                BitField("z", 0x00000000FFFF, adapter=S16ByteSwapAdapter()),
             ), bit_width=8 * 6),
 
             # FIFO control register
-            Register('FIFO_CONTROL', 0x2e, fields=(
-                BitField('mode', 0b11100000),
-                BitField('threshold', 0b00011111),
+            Register("FIFO_CONTROL", 0x2e, fields=(
+                BitField("mode", 0b11100000),
+                BitField("threshold", 0b00011111),
             )),
 
             # FIFO status register
-            Register('FIFO_STATUS', 0x2f, fields=(
-                BitField('threshold_exceeded', 1 << 7),
-                BitField('overrun', 1 << 6),
-                BitField('empty', 1 << 5),
-                BitField('unread_levels', 0b00011111),  # Current number of unread FIFO levels
+            Register("FIFO_STATUS", 0x2f, fields=(
+                BitField("threshold_exceeded", 1 << 7),
+                BitField("overrun", 1 << 6),
+                BitField("empty", 1 << 5),
+                BitField("unread_levels", 0b00011111),  # Current number of unread FIFO levels
             )),
 
             # 0x30: Internal interrupt generator 1: configuration register
             # 0x31: Internal interrupt generator 1: status register
             # 0x32: Internal interrupt generator 1: threshold register
             # 0x33: Internal interrupt generator 1: duration register
-            Register('IG_CONFIG1', 0x30 | 0x80, fields=(
+            Register("IG_CONFIG1", 0x30 | 0x80, fields=(
                 # 0x30
-                BitField('and_or_combination', 1 << 31),
-                BitField('enable_6d', 1 << 30),
-                BitField('z_high_enable', 1 << 29),
-                BitField('z_low_enable', 1 << 28),
-                BitField('y_high_enable', 1 << 27),
-                BitField('y_low_enable', 1 << 26),
-                BitField('x_high_enable', 1 << 25),
-                BitField('x_low_enble', 1 << 24),
+                BitField("and_or_combination", 1 << 31),
+                BitField("enable_6d", 1 << 30),
+                BitField("z_high_enable", 1 << 29),
+                BitField("z_low_enable", 1 << 28),
+                BitField("y_high_enable", 1 << 27),
+                BitField("y_low_enable", 1 << 26),
+                BitField("x_high_enable", 1 << 25),
+                BitField("x_low_enble", 1 << 24),
                 # 0x31
-                BitField('interrupt_status', 1 << 23),
-                BitField('z_high', 1 << 22),
-                BitField('z_low', 1 << 21),
-                BitField('y_high', 1 << 20),
-                BitField('y_low', 1 << 19),
-                BitField('x_high', 1 << 18),
-                BitField('x_low', 1 << 17),
-                BitField('status', 1 << 16),
+                BitField("interrupt_status", 1 << 23),
+                BitField("z_high", 1 << 22),
+                BitField("z_low", 1 << 21),
+                BitField("y_high", 1 << 20),
+                BitField("y_low", 1 << 19),
+                BitField("x_high", 1 << 18),
+                BitField("x_low", 1 << 17),
+                BitField("status", 1 << 16),
                 # 0x32
-                BitField('threshold', 0xff << 8),
+                BitField("threshold", 0xff << 8),
                 # 0x33
-                BitField('duration', 0xff),
+                BitField("duration", 0xff),
             ), bit_width=32),
 
             # 0x34: Internal interrupt generator 2: configuration register
             # 0x35: Internal interrupt generator 2: status register
             # 0x36: Internal interrupt generator 2: threshold register
             # 0x37: Internal interrupt generator 2: duration register
-            Register('IG_CONFIG1', 0x30 | 0x80, fields=(
+            Register("IG_CONFIG1", 0x30 | 0x80, fields=(
                 # 0x34
-                BitField('and_or_combination', 1 << 31),
-                BitField('enable_6d', 1 << 30),
-                BitField('z_high_enable', 1 << 29),
-                BitField('z_low_enable', 1 << 28),
-                BitField('y_high_enable', 1 << 27),
-                BitField('y_low_enable', 1 << 26),
-                BitField('x_high_enable', 1 << 25),
-                BitField('x_low_enble', 1 << 24),
+                BitField("and_or_combination", 1 << 31),
+                BitField("enable_6d", 1 << 30),
+                BitField("z_high_enable", 1 << 29),
+                BitField("z_low_enable", 1 << 28),
+                BitField("y_high_enable", 1 << 27),
+                BitField("y_low_enable", 1 << 26),
+                BitField("x_high_enable", 1 << 25),
+                BitField("x_low_enble", 1 << 24),
                 # 0x35
-                BitField('interrupt_status', 1 << 23),
-                BitField('z_high', 1 << 22),
-                BitField('z_low', 1 << 21),
-                BitField('y_high', 1 << 20),
-                BitField('y_low', 1 << 19),
-                BitField('x_high', 1 << 18),
-                BitField('x_low', 1 << 17),
-                BitField('status', 1 << 16),
+                BitField("interrupt_status", 1 << 23),
+                BitField("z_high", 1 << 22),
+                BitField("z_low", 1 << 21),
+                BitField("y_high", 1 << 20),
+                BitField("y_low", 1 << 19),
+                BitField("x_high", 1 << 18),
+                BitField("x_low", 1 << 17),
+                BitField("status", 1 << 16),
                 # 0x36
-                BitField('threshold', 0xff << 8),
+                BitField("threshold", 0xff << 8),
                 # 0x37
-                BitField('duration', 0xff),
+                BitField("duration", 0xff),
             ), bit_width=32),
 
             # 0x38: Click: configuration register
             # 0x39: Click: status register
             # 0x3A: Click: threshold register
             # 0x3B: Click: time limit register
             # 0x3C: Click: time latency register
             # 0x3D: Click: time window register
-            Register('CLICK', 0x38 | 0x80, fields=(
+            Register("CLICK", 0x38 | 0x80, fields=(
                 # 0x38
                 # bits 1 << 47 and 1 << 46 are unimplemented
-                BitField('z_doubleclick_enable', 1 << 45),
-                BitField('z_click_enable', 1 << 44),
-                BitField('y_doubleclick_enable', 1 << 43),
-                BitField('y_click_enable', 1 << 42),
-                BitField('x_doubleclick_enable', 1 << 41),
-                BitField('x_click_enable', 1 << 40),
+                BitField("z_doubleclick_enable", 1 << 45),
+                BitField("z_click_enable", 1 << 44),
+                BitField("y_doubleclick_enable", 1 << 43),
+                BitField("y_click_enable", 1 << 42),
+                BitField("x_doubleclick_enable", 1 << 41),
+                BitField("x_click_enable", 1 << 40),
                 # 0x39
                 # bit 1 << 39 is unimplemented
-                BitField('interrupt_enable', 1 << 38),
-                BitField('doubleclick_enable', 1 << 37),
-                BitField('click_enable', 1 << 36),
-                BitField('sign', 1 << 35),  # 0 positive detection, 1 negative detection
-                BitField('z', 1 << 34),
-                BitField('y', 1 << 33),
-                BitField('x', 1 << 32),
+                BitField("interrupt_enable", 1 << 38),
+                BitField("doubleclick_enable", 1 << 37),
+                BitField("click_enable", 1 << 36),
+                BitField("sign", 1 << 35),  # 0 positive detection, 1 negative detection
+                BitField("z", 1 << 34),
+                BitField("y", 1 << 33),
+                BitField("x", 1 << 32),
                 # 0x3A
-                BitField('threshod', 0xFF << 24),
+                BitField("threshold", 0xFF << 24),
                 # 0x3B
-                BitField('time_limit', 0xFF << 16),
+                BitField("time_limit", 0xFF << 16),
                 # 0x3C
-                BitField('time_latency', 0xFF << 8),
+                BitField("time_latency", 0xFF << 8),
                 # 0x3D
-                BitField('time_window', 0xFF),
+                BitField("time_window", 0xFF),
             ), bit_width=8 * 6),
 
             # Controls the threshold and duration of returning to sleep mode
-            Register('ACT', 0x3e | 0x80, fields=(
-                BitField('threshold', 0xFF00),  # 1 LSb = 16mg
-                BitField('duration', 0x00FF)    # (duration + 1) * 8/output_data_rate
+            Register("ACT", 0x3e | 0x80, fields=(
+                BitField("threshold", 0xFF00),  # 1 LSb = 16mg
+                BitField("duration", 0x00FF)    # (duration + 1) * 8/output_data_rate
             ), bit_width=16)
 
         ))
 
         self._is_setup = False
 
         self._accel_full_scale_g = 2
-        self._mag_full_scale_guass = 2
+        self._mag_full_scale_gauss = 2
 
     def set_accel_full_scale_g(self, scale):
         """Set the full scale range for the accelerometer in g
 
         :param scale: One of 2, 4, 6, 8 or 16 g
 
         """
         self._accel_full_scale_g = scale
-        self._lsm303d.set('CONTROL2', accel_full_scale_g=self._accel_full_scale_g)
+        self._lsm303d.set("CONTROL2", accel_full_scale_g=self._accel_full_scale_g)
 
-    def set_mag_full_scale_guass(self, scale):
-        """Set the full scale range for the magnetometer in guass
+    def set_mag_full_scale_gauss(self, scale):
+        """Set the full scale range for the magnetometer in gauss
 
-        :param scale: One of 2, 4, 8 or 12 guass
+        :param scale: One of 2, 4, 8 or 12 gauss
 
         """
-        self._mag_full_scale_guass = scale
-        self._lsm303d.set('CONTROL6', mag_full_scale_gauss=scale)  # +-2
+        self._mag_full_scale_gauss = scale
+        self._lsm303d.set("CONTROL6", mag_full_scale_gauss=scale)  # +-2
+
+    set_mag_full_scale_guass = set_mag_full_scale_gauss
 
     def setup(self):
         if self._is_setup:
             return
         self._is_setup = True
 
         self._lsm303d.select_address(self._i2c_addr)
 
         try:
-            chip = self._lsm303d.get('WHOAMI')
+            chip = self._lsm303d.get("WHOAMI")
             if chip.id != 0x49:
                 raise RuntimeError("Unable to find lsm303d on 0x{:02x}, WHOAMI returned {:02x}".format(self._i2c_addr, chip.id))
         except IOError:
             raise RuntimeError("Unable to find lsm303d on 0x{:02x}, IOError".format(self._i2c_addr))
 
-        self._lsm303d.set('CONTROL1',
+        self._lsm303d.set("CONTROL1",
                           accel_x_enable=1,
                           accel_y_enable=1,
                           accel_z_enable=1,
                           accel_data_rate_hz=50)
 
         self.set_accel_full_scale_g(2)
 
-        self._lsm303d.set('INTERRUPT1',
+        self._lsm303d.set("INTERRUPT1",
                           enable_fifo_empty=0,
                           enable_accel_dataready=0,
                           enable_accelerometer=0,
                           enable_magnetometer=0,
                           enable_ig2=0,
                           enable_ig1=0,
                           enable_click=0,
                           enable_boot=0)
 
-        self._lsm303d.set('INTERRUPT2',
+        self._lsm303d.set("INTERRUPT2",
                           enable_fifo=0,
                           enable_fifo_overrun=0,
                           enable_mag_dataready=0,
                           enable_accel_dataready=0,
                           enable_magnetometer=0,
                           enable_ig2=0,
                           enable_ig1=0,
                           enable_click=0)
 
-        self._lsm303d.set('CONTROL5',
+        self._lsm303d.set("CONTROL5",
                           mag_data_rate_hz=50,
                           enable_temperature=1)
 
-        self.set_mag_full_scale_guass(2)
+        self.set_mag_full_scale_gauss(2)
 
-        self._lsm303d.set('CONTROL7', mag_mode='continuous')
+        self._lsm303d.set("CONTROL7", mag_mode="continuous")
 
     def magnetometer(self):
         """Return magnetometer x, y and z readings.
 
-        These readings are given in guass and should be +/- the given mag_full_scale_guass value.
+        These readings are given in gauss and should be +/- the given mag_full_scale_gauss value.
 
         """
         self.setup()
-        mag = self._lsm303d.get('MAGNETOMETER')
+        mag = self._lsm303d.get("MAGNETOMETER")
         x, y, z = mag.x, mag.y, mag.z
-        x, y, z = [(p / 32676.0) * self._mag_full_scale_guass for p in (x, y, z)]
+        x, y, z = [(p / 32767.0) * self._mag_full_scale_gauss for p in (x, y, z)]
         return x, y, z
 
     def accelerometer(self):
-        """Return acelerometer x, y and z readings.
+        """Return accelerometer x, y and z readings.
 
-        These readings are given in g annd should be +/- the given accel_full_scale_g value.
+        These readings are given in g and should be +/- the given accel_full_scale_g value.
 
         """
         self.setup()
-        accel = self._lsm303d.get('ACCELEROMETER')
+        accel = self._lsm303d.get("ACCELEROMETER")
         x, y, z = accel.x, accel.y, accel.z
         x, y, z = [(p / 32767.0) * self._accel_full_scale_g for p in (x, y, z)]
         return x, y, z
 
     def temperature(self):
         """Return the temperature"""
         self.setup()
-        return self._lsm303d.get('TEMPERATURE').temperature
+        return self._lsm303d.get("TEMPERATURE").temperature
```

### Comparing `lsm303d-0.0.5/LICENSE.txt` & `lsm303d-1.0.0/LICENSE`

 * *Files identical despite different names*

