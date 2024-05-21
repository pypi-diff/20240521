# Comparing `tmp/ArducamEvkSDK-0.0.9b0-cp39-cp39-manylinux_2_24_x86_64.whl.zip` & `tmp/ArducamEvkSDK-1.0.0-cp312-cp312-manylinux_2_24_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 2159569 bytes, number of entries: 9
-drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-07 08:26 ArducamEvkSDK.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-07 08:26 ArducamEvkSDK-0.0.9b0.dist-info/
--rw-r--r--  2.0 unx    37571 b- defN 23-Nov-07 08:26 ArducamEvkSDK.pyi
--rwxr-xr-x  2.0 unx  5822961 b- defN 23-Nov-07 08:26 ArducamEvkSDK.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx    18209 b- defN 23-Nov-07 08:26 ArducamEvkSDK.libs/libarducam_config_parser-f72a97e8.so
--rw-r--r--  2.0 unx      119 b- defN 23-Nov-07 08:26 ArducamEvkSDK-0.0.9b0.dist-info/METADATA
--rw-r--r--  2.0 unx      112 b- defN 23-Nov-07 08:26 ArducamEvkSDK-0.0.9b0.dist-info/WHEEL
--rw-rw-r--  2.0 unx      629 b- defN 23-Nov-07 08:26 ArducamEvkSDK-0.0.9b0.dist-info/RECORD
--rw-r--r--  2.0 unx       14 b- defN 23-Nov-07 08:26 ArducamEvkSDK-0.0.9b0.dist-info/top_level.txt
-9 files, 5879615 bytes uncompressed, 2158209 bytes compressed:  63.3%
+Zip file size: 1877421 bytes, number of entries: 9
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 06:48 ArducamEvkSDK-1.0.0.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 06:48 ArducamEvkSDK.libs/
+-rwxr-xr-x  2.0 unx  4915241 b- defN 24-May-20 06:48 ArducamEvkSDK.cpython-312-aarch64-linux-gnu.so
+-rw-r--r--  2.0 unx    36975 b- defN 24-May-20 06:48 ArducamEvkSDK.pyi
+-rw-rw-r--  2.0 unx      623 b- defN 24-May-20 06:48 ArducamEvkSDK-1.0.0.dist-info/RECORD
+-rw-r--r--  2.0 unx       14 b- defN 24-May-20 06:48 ArducamEvkSDK-1.0.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      115 b- defN 24-May-20 06:48 ArducamEvkSDK-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      117 b- defN 24-May-20 06:48 ArducamEvkSDK-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx    66617 b- defN 24-May-20 06:48 ArducamEvkSDK.libs/libarducam_config_parser-7fcaacc5.so
+9 files, 5019702 bytes uncompressed, 1876077 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: ArducamEvkSDK.libs/
+Filename: ArducamEvkSDK-1.0.0.dist-info/
 Comment: 
 
-Filename: ArducamEvkSDK-0.0.9b0.dist-info/
+Filename: ArducamEvkSDK.libs/
 Comment: 
 
-Filename: ArducamEvkSDK.pyi
+Filename: ArducamEvkSDK.cpython-312-aarch64-linux-gnu.so
 Comment: 
 
-Filename: ArducamEvkSDK.cpython-39-x86_64-linux-gnu.so
+Filename: ArducamEvkSDK.pyi
 Comment: 
 
-Filename: ArducamEvkSDK.libs/libarducam_config_parser-f72a97e8.so
+Filename: ArducamEvkSDK-1.0.0.dist-info/RECORD
 Comment: 
 
-Filename: ArducamEvkSDK-0.0.9b0.dist-info/METADATA
+Filename: ArducamEvkSDK-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ArducamEvkSDK-0.0.9b0.dist-info/WHEEL
+Filename: ArducamEvkSDK-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: ArducamEvkSDK-0.0.9b0.dist-info/RECORD
+Filename: ArducamEvkSDK-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: ArducamEvkSDK-0.0.9b0.dist-info/top_level.txt
+Filename: ArducamEvkSDK.libs/libarducam_config_parser-7fcaacc5.so
 Comment: 
 
 Zip file comment:
```

## ArducamEvkSDK.pyi

```diff
@@ -1,1230 +1,1098 @@
-#
-# Automatically generated file, do not edit!
-#
-
 """
+
     ArducamEvkSDK
 """
 from __future__ import annotations
-import ArducamEvkSDK
+import numpy
 import typing
-
-__all__ = [
-    "Camera",
-    "CameraConfig",
-    "CaptureMethodConflict",
-    "CaptureTimeout",
-    "ConfigFileEmpty",
-    "ConfigFormatError",
-    "Control",
-    "ControlFormatError",
-    "Critical",
-    "DMA",
-    "Debug",
-    "Device",
-    "DeviceConnect",
-    "DeviceDisconnect",
-    "DeviceToHost",
-    "Empty",
-    "Err",
-    "ErrorCode",
-    "EventCode",
-    "Exit",
-    "Format",
-    "FormatMode",
-    "Frame",
-    "FrameEnd",
-    "FrameStart",
-    "FreeEmptyBuffer",
-    "FreeUnknowBuffer",
-    "Full",
-    "High",
-    "HostToDevice",
-    "I2CMode",
-    "I2C_MODE_16_16",
-    "I2C_MODE_16_32",
-    "I2C_MODE_16_8",
-    "I2C_MODE_8_16",
-    "I2C_MODE_8_8",
-    "Info",
-    "InitCameraFailed",
-    "JPG",
-    "LoggerLevel",
-    "Low",
-    "MON",
-    "MON_D",
-    "MemType",
-    "MemoryAllocateFailed",
-    "NotSupport",
-    "Off",
-    "OpenCameraFailed",
-    "Param",
-    "RAM",
-    "RAW",
-    "RAW_D",
-    "RGB",
-    "ReadConfigFileFailed",
-    "RegisterMultipleCallback",
-    "STATS",
-    "StateError",
-    "Success",
-    "Super",
-    "SuperPlus",
-    "Trace",
-    "TransferError",
-    "TransferTimeout",
-    "USBSpeed",
-    "USBTypeMismatch",
-    "Unknown",
-    "UnknownDeviceType",
-    "UnknownError",
-    "UnknownUSBType",
-    "UserdataAddrError",
-    "UserdataLenError",
-    "VRCommandDirection",
-    "VRCommandError",
-    "Warn",
-    "YUV",
-    "free_device_list",
-    "get_error_name",
-    "list_devices"
-]
-
-
-class Camera():
-    def __init__(self) -> None: ...
-    def add_log_file(self, filename: str) -> bool: 
+__all__ = ['Camera', 'CameraConfig', 'CaptureMethodConflict', 'CaptureTimeout', 'ConfigFileEmpty', 'ConfigFormatError', 'Control', 'ControlFormatError', 'Critical', 'DMA', 'Debug', 'Device', 'DeviceConnect', 'DeviceDisconnect', 'DeviceList', 'DeviceToHost', 'Empty', 'Err', 'ErrorCode', 'EventCode', 'Exit', 'Format', 'FormatMode', 'Frame', 'FrameEnd', 'FrameStart', 'FreeEmptyBuffer', 'FreeUnknowBuffer', 'Full', 'High', 'HostToDevice', 'I2CMode', 'I2C_MODE_16_16', 'I2C_MODE_16_32', 'I2C_MODE_16_8', 'I2C_MODE_8_16', 'I2C_MODE_8_8', 'Info', 'InitCameraFailed', 'JPG', 'LoggerLevel', 'Low', 'MON', 'MON_D', 'MemType', 'MemoryAllocateFailed', 'NotSupported', 'Off', 'OpenCameraFailed', 'Param', 'RAM', 'RAW', 'RAW_D', 'RGB', 'RGB_IR', 'ReadConfigFileFailed', 'RegisterMultipleCallback', 'STATS', 'StateError', 'Success', 'Super', 'SuperPlus', 'TOF', 'Trace', 'TransferError', 'TransferLengthError', 'TransferTimeout', 'USBSpeed', 'USBTypeMismatch', 'Unknown', 'UnknownDeviceType', 'UnknownError', 'UnknownUSBType', 'UserdataAddrError', 'UserdataLenError', 'VRCommandDirection', 'VRCommandError', 'Warn', 'YUV', 'get_error_name']
+class Camera:
+    def __init__(self) -> None:
+        ...
+    def add_log_file(self, filename: str) -> bool:
         """
         add a log file
         """
-    def capture(self, timeout: int = 2000) -> typing.Optional[Frame]: 
+    def capture(self, timeout: int = 2000) -> typing.Any:
         """
         capture a image, return a object of Frame, or None if failed
         """
-    def check_usb_type(self) -> bool: 
+    def check_usb_type(self) -> bool:
         """
         check the connection usb type is expected or not
         """
-    def close(self) -> bool: 
+    def clear_buffer(self) -> bool:
+        """
+        clear the buffer
+        """
+    def close(self) -> bool:
         """
         close the camera
         """
-    def enable_console_log(self, enable: bool = True) -> None: 
+    def enable_console_log(self, enable: bool = True) -> None:
         """
         enable/disable console log
         """
-    def has_capture_callback(self) -> bool: 
+    def get_auto_transfer(self) -> typing.Any:
+        """
+        get the recommended transfer configuration
+        """
+    def get_avail_count(self) -> int:
+        """
+        get the available frame count
+        """
+    def has_capture_callback(self) -> bool:
         """
         check if the callback function for reading a frame is set
         """
-    def has_event_callback(self) -> bool: 
+    def has_event_callback(self) -> bool:
         """
         check if the callback function for event is set
         """
-    def has_message_callback(self) -> bool: 
+    def has_message_callback(self) -> bool:
         """
         check if the callback function for message is set
         """
-    def init(self) -> bool: 
+    def init(self) -> bool:
         """
         init the camera
         """
-    def open(self, param: Param) -> bool: 
+    def is_opened(self) -> bool:
+        """
+        check if the camera is opened
+        """
+    def open(self, param: Param) -> bool:
         """
         open the camera
         """
-    def read_board_config(self, command: int, value: int, index: int, buf_size: int) -> typing.Optional[typing.List[int]]: 
+    def read_board_config(self, command: int, value: int, index: int, buf_size: int) -> typing.Any:
         """
         read sensor register
         """
-    def read_reg(self, mode: I2CMode, i2c_addr: int, regAddr: int) -> typing.Optional[int]: 
+    def read_reg(self, mode: I2CMode, i2c_addr: int, regAddr: int) -> typing.Any:
         """
         read sensor register
         """
-    def read_reg_16_16(self, ship_addr: int, reg_addr: int) -> typing.Optional[int]: 
+    def read_reg_16_16(self, ship_addr: int, reg_addr: int) -> typing.Any:
         """
         Reads a register value with 16 bit address and 16-bit value.
         """
-    def read_reg_16_8(self, ship_addr: int, reg_addr: int) -> typing.Optional[int]: 
+    def read_reg_16_8(self, ship_addr: int, reg_addr: int) -> typing.Any:
         """
         Reads a register value with 16 bit address and 8-bit value.
         """
-    def read_reg_8_16(self, ship_addr: int, reg_addr: int) -> typing.Optional[int]: 
+    def read_reg_8_16(self, ship_addr: int, reg_addr: int) -> typing.Any:
         """
         Reads a register value with 8 bit address and 16-bit value.
         """
-    def read_reg_8_8(self, ship_addr: int, reg_addr: int) -> typing.Optional[int]: 
+    def read_reg_8_8(self, ship_addr: int, reg_addr: int) -> typing.Any:
         """
         Reads a register value with 8 bit address and 8-bit value.
         """
-    def read_sensor_reg(self, reg_addr: int) -> typing.Optional[int]: 
+    def read_sensor_reg(self, reg_addr: int) -> typing.Any:
         """
         read sensor register
         """
-    def read_user_data(self, addr: int, len: int) -> typing.Optional[typing.List[int]]: 
+    def read_user_data(self, addr: int, len: int) -> typing.Any:
         """
         read sensor register
         """
-    def register_control(self, controls: typing.List[Control]) -> bool: 
+    def register_control(self, controls: list[Control]) -> bool:
         """
         register controls
         """
-    def send_vr(self, command: int, direction: int, value: int, index: int, buffer: typing.List[int]) -> bool: 
+    def send_vr(self, command: int, direction: int, value: int, index: int, buffer: list[int]) -> typing.Any:
         """
         send vendor request
         """
-    def set_auto_transfer(self, auto_transfer: bool) -> bool: 
+    def set_auto_transfer(self, auto_transfer: bool) -> bool:
         """
-        enable or disable the automatic transfer configuration setting before starting the camera
+        enable or disable the automatic transfer configuration before starting the camera
         """
-    def set_capture_callback(self, callback: typing.Callable[[Frame], None]) -> None: 
+    def set_capture_callback(self, callback: typing.Callable[[Frame], None]) -> None:
         """
         set the callback function for reading a frame, or None to disable it
         """
-    def set_control(self, controlId: str, value: int) -> bool: 
+    def set_control(self, controlId: str, value: int) -> bool:
         """
         set control value
         """
-    def set_event_callback(self, callback: typing.Callable[[EventCode], None]) -> None: 
+    def set_event_callback(self, callback: typing.Callable[[EventCode], None]) -> None:
         """
         set the callback function for event, or None to disable it
         """
-    def set_message_callback(self, callback: typing.Callable[[LoggerLevel, str], None]) -> None: 
+    def set_message_callback(self, callback: typing.Callable[[LoggerLevel, str], None]) -> None:
         """
         set the callback function for messages, or None to disable it
         """
-    def set_transfer(self, transfer_size: int, transfer_buffer_size: int) -> bool: 
+    def set_transfer(self, transfer_size: int, transfer_buffer_size: int) -> bool:
         """
         set transfer size and buffer size
         """
-    def start(self) -> bool: 
+    def start(self) -> bool:
         """
         start the camera
         """
-    def stop(self) -> None: 
+    def stop(self) -> bool:
         """
         stop the camera
         """
-    def switch_mode(self, mode_id: int) -> bool: 
+    def switch_mode(self, mode_id: int) -> bool:
         """
         switch the camera mode
         """
-    def write_board_config(self, command: int, value: int, index: int, buf: typing.List[int]) -> bool: 
+    def wait_capture(self, timeout: int = 2000) -> bool:
+        """
+        wait for a frame to be captured, return True if success, False if timeout
+        """
+    def write_board_config(self, command: int, value: int, index: int, buffer: list[int]) -> bool:
         """
         write sensor register
         """
-    def write_reg(self, mode: I2CMode, i2c_addr: int, regAddr: int, value: int) -> bool: 
+    def write_reg(self, mode: I2CMode, i2c_addr: int, regAddr: int, value: int) -> bool:
         """
         write sensor register
         """
-    def write_reg_16_16(self, ship_addr: int, reg_addr: int, value: int) -> bool: 
+    def write_reg_16_16(self, ship_addr: int, reg_addr: int, value: int) -> bool:
         """
         Writes a register value with 16 bit address and 16-bit value.
         """
-    def write_reg_16_8(self, ship_addr: int, reg_addr: int, value: int) -> bool: 
+    def write_reg_16_8(self, ship_addr: int, reg_addr: int, value: int) -> bool:
         """
         Writes a register value with 16 bit address and 8-bit value.
         """
-    def write_reg_8_16(self, ship_addr: int, reg_addr: int, value: int) -> bool: 
+    def write_reg_8_16(self, ship_addr: int, reg_addr: int, value: int) -> bool:
         """
         Writes a register value with 8 bit address and 16-bit value.
         """
-    def write_reg_8_8(self, ship_addr: int, reg_addr: int, value: int) -> bool: 
+    def write_reg_8_8(self, ship_addr: int, reg_addr: int, value: int) -> bool:
         """
         Writes a register value with 8 bit address and 8-bit value.
         """
-    def write_sensor_reg(self, reg_addr: int, value: int) -> bool: 
+    def write_sensor_reg(self, reg_addr: int, value: int) -> bool:
         """
         write sensor register
         """
-    def write_user_data(self, addr: int, data: typing.List[int]) -> bool: 
+    def write_user_data(self, addr: int, data: list[int]) -> bool:
         """
         write sensor register
         """
     @property
     def bandwidth(self) -> int:
         """
         A property of bandwidth (read-only).
-
-        :type: int
         """
     @bandwidth.setter
-    def bandwidth(self) -> None:
-        """
-        A property of bandwidth (read-only).
-        """
+    def bandwidth() -> None:
+        ...
     @property
     def bin_config(self) -> dict:
         """
         A property of bin_config (read-only).
-
-        :type: dict
         """
     @bin_config.setter
-    def bin_config(self) -> None:
-        """
-        A property of bin_config (read-only).
-        """
+    def bin_config() -> None:
+        ...
     @property
     def capture_fps(self) -> int:
         """
         A property of capture_fps (read-only).
-
-        :type: int
         """
     @capture_fps.setter
-    def capture_fps(self) -> None:
-        """
-        A property of capture_fps (read-only).
-        """
+    def capture_fps() -> None:
+        ...
     @property
     def config(self) -> CameraConfig:
         """
         A property of config.
-
-        :type: CameraConfig
         """
     @config.setter
-    def config(self, arg1: CameraConfig) -> None:
-        """
-        A property of config.
-        """
+    def config(self, arg1: CameraConfig) -> bool:
+        ...
     @property
     def config_type(self) -> str:
         """
-        A property of config_type (read-only). (NONE | TEXT | BINARY)
-
-        :type: str
+        A property of config_type (read-only). ('NONE' | 'TEXT' | 'BINARY')
         """
     @config_type.setter
-    def config_type(self) -> None:
-        """
-        A property of config_type (read-only). (NONE | TEXT | BINARY)
-        """
+    def config_type() -> None:
+        ...
     @property
-    def controls(self) -> typing.List[Control]:
+    def controls(self) -> list[Control]:
         """
         A property of controls (read-only).
-
-        :type: typing.List[Control]
         """
     @controls.setter
-    def controls(self) -> None:
-        """
-        A property of controls (read-only).
-        """
+    def controls() -> None:
+        ...
     @property
     def force_capture(self) -> bool:
         """
         A property of force_capture.
-
-        :type: bool
         """
     @force_capture.setter
     def force_capture(self, arg1: bool) -> None:
-        """
-        A property of force_capture.
-        """
+        ...
     @property
     def last_error(self) -> int:
         """
         A property of last_error (read-only).
-
-        :type: int
         """
     @last_error.setter
-    def last_error(self) -> None:
-        """
-        A property of last_error (read-only).
-        """
+    def last_error() -> None:
+        ...
     @property
     def last_error_message(self) -> str:
         """
         A property of last_error_message (read-only).
-
-        :type: str
         """
     @last_error_message.setter
-    def last_error_message(self) -> None:
-        """
-        A property of last_error_message (read-only).
-        """
+    def last_error_message() -> None:
+        ...
     @property
     def log_level(self) -> LoggerLevel:
         """
         A property of log_level.
-
-        :type: LoggerLevel
         """
     @log_level.setter
     def log_level(self, arg1: LoggerLevel) -> None:
-        """
-        A property of log_level.
-        """
+        ...
     @property
     def mem_type(self) -> MemType:
         """
         A property of mem_type.
-
-        :type: MemType
         """
     @mem_type.setter
-    def mem_type(self, arg1: MemType) -> None:
-        """
-        A property of mem_type.
-        """
+    def mem_type(self, arg1: MemType) -> bool:
+        ...
     @property
     def usb_type(self) -> str:
         """
         A property of usb_type (read-only).
-
-        :type: str
         """
     @usb_type.setter
-    def usb_type(self) -> None:
+    def usb_type() -> None:
+        ...
+    @property
+    def usb_type_num(self) -> int:
         """
-        A property of usb_type (read-only).
+        A property of usb_type_num (read-only).
         """
-    pass
-class CameraConfig():
-    def __init__(self) -> None: ...
+    @usb_type_num.setter
+    def usb_type_num() -> None:
+        ...
+class CameraConfig:
+    def __init__(self) -> None:
+        ...
     @property
     def bit_width(self) -> int:
         """
         A property of bit_width.
-
-        :type: int
         """
     @bit_width.setter
     def bit_width(self, arg0: int) -> None:
-        """
-        A property of bit_width.
-        """
+        ...
     @property
     def format(self) -> int:
         """
         A property of format.
-
-        :type: int
         """
     @format.setter
     def format(self, arg0: int) -> None:
-        """
-        A property of format.
-        """
+        ...
     @property
     def height(self) -> int:
         """
         A property of height.
-
-        :type: int
         """
     @height.setter
     def height(self, arg0: int) -> None:
-        """
-        A property of height.
-        """
+        ...
     @property
     def i2c_addr(self) -> int:
         """
         A property of i2c_addr.
-
-        :type: int
         """
     @i2c_addr.setter
     def i2c_addr(self, arg0: int) -> None:
-        """
-        A property of i2c_addr.
-        """
+        ...
     @property
     def i2c_mode(self) -> int:
         """
         A property of i2c_mode.
-
-        :type: int
         """
     @i2c_mode.setter
     def i2c_mode(self, arg0: int) -> None:
-        """
-        A property of i2c_mode.
-        """
+        ...
     @property
     def width(self) -> int:
         """
         A property of width.
-
-        :type: int
         """
     @width.setter
     def width(self, arg0: int) -> None:
-        """
-        A property of width.
-        """
-    pass
-class Control():
-    def __init__(self) -> None: 
+        ...
+class Control:
+    def __init__(self) -> None:
         """
         Creates a new control.
         """
-    def __repr__(self) -> str: 
+    def __repr__(self) -> str:
         """
         Returns a string representation of the control.
         """
-    def __str__(self) -> str: 
+    def __str__(self) -> str:
         """
         Returns a string representation of the control.
         """
     @property
     def code(self) -> str:
         """
         A property of code.
-
-        :type: str
         """
     @code.setter
     def code(self, arg0: str) -> None:
-        """
-        A property of code.
-        """
+        ...
     @property
     def default(self) -> int:
         """
         A property of default.
-
-        :type: int
         """
     @default.setter
     def default(self, arg0: int) -> None:
-        """
-        A property of default.
-        """
+        ...
     @property
     def flags(self) -> int:
         """
         A property of flags.
-
-        :type: int
         """
     @flags.setter
     def flags(self, arg0: int) -> None:
-        """
-        A property of flags.
-        """
+        ...
     @property
     def func(self) -> str:
         """
         A property of func (read-only).
-
-        :type: str
         """
     @func.setter
-    def func(self) -> None:
-        """
-        A property of func (read-only).
-        """
+    def func() -> None:
+        ...
     @property
     def max(self) -> int:
         """
         A property of max.
-
-        :type: int
         """
     @max.setter
     def max(self, arg0: int) -> None:
-        """
-        A property of max.
-        """
+        ...
     @property
     def min(self) -> int:
         """
         A property of min.
-
-        :type: int
         """
     @min.setter
     def min(self, arg0: int) -> None:
-        """
-        A property of min.
-        """
+        ...
     @property
     def name(self) -> str:
         """
         A property of name (read-only).
-
-        :type: str
         """
     @name.setter
-    def name(self) -> None:
-        """
-        A property of name (read-only).
-        """
+    def name() -> None:
+        ...
     @property
     def step(self) -> int:
         """
         A property of step.
-
-        :type: int
         """
     @step.setter
     def step(self, arg0: int) -> None:
+        ...
+class Device:
+    def __eq__(self, arg0: Device) -> bool:
         """
-        A property of step.
+        Check the Devices are same.
+        """
+    def __hash__(self) -> int:
         """
-    pass
-class Device():
-    def __repr__(self) -> str: 
+        Returns the hash value of the device.
+        """
+    def __repr__(self) -> str:
         """
         Returns a string representation of the device.
         """
     @property
+    def dev_path(self) -> str:
+        """
+        A property of dev_path (const).
+        """
+    @property
     def id_product(self) -> int:
         """
         A property of id_product (const).
-
-        :type: int
         """
     @property
     def id_vendor(self) -> int:
         """
         A property of id_vendor (const).
-
-        :type: int
         """
     @property
     def in_used(self) -> bool:
         """
         A property of in_used (const).
-
-        :type: bool
         """
     @property
-    def serial_number(self) -> typing.List[int]:
+    def serial_number(self) -> list[int]:
         """
         A property of serial_number (const).This is a list with 12 elements.
-
-        :type: typing.List[int]
         """
     @property
     def speed(self) -> USBSpeed:
         """
         A property of speed (const).
-
-        :type: USBSpeed
         """
     @property
     def usb_type(self) -> int:
         """
         A property of usb_type (const).
-
-        :type: int
         """
-    pass
-class ErrorCode():
+class DeviceList:
+    def __init__(self) -> None:
+        ...
+    def devices(self) -> list[Device]:
+        """
+        All supported devices
+        """
+    def has_event_callback(self) -> bool:
+        """
+        Check if the callback function for event is set
+        """
+    def refresh(self) -> bool:
+        """
+        Refreshes the device list
+        """
+    def set_event_callback(self, callback: typing.Callable[[EventCode, Device | None], None]) -> bool:
+        """
+        Set the callback function for event, or None to disable it
+        """
+class ErrorCode:
     """
     Members:
-
+    
       Success : Success.
-
+    
       Empty : Empty.
-
+    
       ReadConfigFileFailed : Failed to read configuration file.
-
+    
       ConfigFileEmpty : Configuration file is empty.
-
+    
       ConfigFormatError : Camera configuration format error.
-
+    
       ControlFormatError : Camera control format error.
-
+    
       OpenCameraFailed : Failed to open camera.
-
+    
       UnknownUSBType : Unknown USB type.
-
+    
       UnknownDeviceType : Unknown Device type.
-
+    
       InitCameraFailed : Failed to initialize camera.
-
+    
       MemoryAllocateFailed : Failed to allocate memory.
-
+    
       USBTypeMismatch : USB type mismatch.
-
+    
       CaptureTimeout : Capture timeout.
-
+    
       CaptureMethodConflict : Capture method conflict.
-
+    
       FreeEmptyBuffer : Free empty buffer.
-
+    
       FreeUnknowBuffer : Free unknown buffer.
-
+    
       RegisterMultipleCallback : Register multiple callback.
-
+    
       StateError : Camera state error.
-
-      NotSupport : Not support.
-
+    
+      NotSupported : Not supported.
+    
       VRCommandError : Vendor command error.
-
+    
       UserdataAddrError : Userdata address error.
-
+    
       UserdataLenError : Userdata length error.
-
+    
       UnknownError : Unknown error.
     """
-    def __eq__(self, other: object) -> bool: ...
-    def __getstate__(self) -> int: ...
-    def __hash__(self) -> int: ...
-    def __index__(self) -> int: ...
-    def __init__(self, value: int) -> None: ...
-    def __int__(self) -> int: ...
-    def __ne__(self, other: object) -> bool: ...
-    def __repr__(self) -> str: ...
-    def __setstate__(self, state: int) -> None: ...
+    CaptureMethodConflict: typing.ClassVar[ErrorCode]  # value = <ErrorCode.CaptureMethodConflict: 1538>
+    CaptureTimeout: typing.ClassVar[ErrorCode]  # value = <ErrorCode.CaptureTimeout: 1537>
+    ConfigFileEmpty: typing.ClassVar[ErrorCode]  # value = <ErrorCode.ConfigFileEmpty: 258>
+    ConfigFormatError: typing.ClassVar[ErrorCode]  # value = <ErrorCode.ConfigFormatError: 259>
+    ControlFormatError: typing.ClassVar[ErrorCode]  # value = <ErrorCode.ControlFormatError: 260>
+    Empty: typing.ClassVar[ErrorCode]  # value = <ErrorCode.Empty: 16>
+    FreeEmptyBuffer: typing.ClassVar[ErrorCode]  # value = <ErrorCode.FreeEmptyBuffer: 1793>
+    FreeUnknowBuffer: typing.ClassVar[ErrorCode]  # value = <ErrorCode.FreeUnknowBuffer: 1794>
+    InitCameraFailed: typing.ClassVar[ErrorCode]  # value = <ErrorCode.InitCameraFailed: 769>
+    MemoryAllocateFailed: typing.ClassVar[ErrorCode]  # value = <ErrorCode.MemoryAllocateFailed: 770>
+    NotSupported: typing.ClassVar[ErrorCode]  # value = <ErrorCode.NotSupported: 61441>
+    OpenCameraFailed: typing.ClassVar[ErrorCode]  # value = <ErrorCode.OpenCameraFailed: 513>
+    ReadConfigFileFailed: typing.ClassVar[ErrorCode]  # value = <ErrorCode.ReadConfigFileFailed: 257>
+    RegisterMultipleCallback: typing.ClassVar[ErrorCode]  # value = <ErrorCode.RegisterMultipleCallback: 2049>
+    StateError: typing.ClassVar[ErrorCode]  # value = <ErrorCode.StateError: 32769>
+    Success: typing.ClassVar[ErrorCode]  # value = <ErrorCode.Success: 0>
+    USBTypeMismatch: typing.ClassVar[ErrorCode]  # value = <ErrorCode.USBTypeMismatch: 1025>
+    UnknownDeviceType: typing.ClassVar[ErrorCode]  # value = <ErrorCode.UnknownDeviceType: 515>
+    UnknownError: typing.ClassVar[ErrorCode]  # value = <ErrorCode.UnknownError: 65535>
+    UnknownUSBType: typing.ClassVar[ErrorCode]  # value = <ErrorCode.UnknownUSBType: 514>
+    UserdataAddrError: typing.ClassVar[ErrorCode]  # value = <ErrorCode.UserdataAddrError: 65377>
+    UserdataLenError: typing.ClassVar[ErrorCode]  # value = <ErrorCode.UserdataLenError: 65378>
+    VRCommandError: typing.ClassVar[ErrorCode]  # value = <ErrorCode.VRCommandError: 65283>
+    __members__: typing.ClassVar[dict[str, ErrorCode]]  # value = {'Success': <ErrorCode.Success: 0>, 'Empty': <ErrorCode.Empty: 16>, 'ReadConfigFileFailed': <ErrorCode.ReadConfigFileFailed: 257>, 'ConfigFileEmpty': <ErrorCode.ConfigFileEmpty: 258>, 'ConfigFormatError': <ErrorCode.ConfigFormatError: 259>, 'ControlFormatError': <ErrorCode.ControlFormatError: 260>, 'OpenCameraFailed': <ErrorCode.OpenCameraFailed: 513>, 'UnknownUSBType': <ErrorCode.UnknownUSBType: 514>, 'UnknownDeviceType': <ErrorCode.UnknownDeviceType: 515>, 'InitCameraFailed': <ErrorCode.InitCameraFailed: 769>, 'MemoryAllocateFailed': <ErrorCode.MemoryAllocateFailed: 770>, 'USBTypeMismatch': <ErrorCode.USBTypeMismatch: 1025>, 'CaptureTimeout': <ErrorCode.CaptureTimeout: 1537>, 'CaptureMethodConflict': <ErrorCode.CaptureMethodConflict: 1538>, 'FreeEmptyBuffer': <ErrorCode.FreeEmptyBuffer: 1793>, 'FreeUnknowBuffer': <ErrorCode.FreeUnknowBuffer: 1794>, 'RegisterMultipleCallback': <ErrorCode.RegisterMultipleCallback: 2049>, 'StateError': <ErrorCode.StateError: 32769>, 'NotSupported': <ErrorCode.NotSupported: 61441>, 'VRCommandError': <ErrorCode.VRCommandError: 65283>, 'UserdataAddrError': <ErrorCode.UserdataAddrError: 65377>, 'UserdataLenError': <ErrorCode.UserdataLenError: 65378>, 'UnknownError': <ErrorCode.UnknownError: 65535>}
+    def __eq__(self, other: typing.Any) -> bool:
+        ...
+    def __getstate__(self) -> int:
+        ...
+    def __hash__(self) -> int:
+        ...
+    def __index__(self) -> int:
+        ...
+    def __init__(self, value: int) -> None:
+        ...
+    def __int__(self) -> int:
+        ...
+    def __ne__(self, other: typing.Any) -> bool:
+        ...
+    def __repr__(self) -> str:
+        ...
+    def __setstate__(self, state: int) -> None:
+        ...
+    def __str__(self) -> str:
+        ...
     @property
     def name(self) -> str:
-        """
-        :type: str
-        """
+        ...
     @property
     def value(self) -> int:
-        """
-        :type: int
-        """
-    CaptureMethodConflict: ArducamEvkSDK.ErrorCode # value = <ErrorCode.CaptureMethodConflict: 1538>
-    CaptureTimeout: ArducamEvkSDK.ErrorCode # value = <ErrorCode.CaptureTimeout: 1537>
-    ConfigFileEmpty: ArducamEvkSDK.ErrorCode # value = <ErrorCode.ConfigFileEmpty: 258>
-    ConfigFormatError: ArducamEvkSDK.ErrorCode # value = <ErrorCode.ConfigFormatError: 259>
-    ControlFormatError: ArducamEvkSDK.ErrorCode # value = <ErrorCode.ControlFormatError: 260>
-    Empty: ArducamEvkSDK.ErrorCode # value = <ErrorCode.Empty: 16>
-    FreeEmptyBuffer: ArducamEvkSDK.ErrorCode # value = <ErrorCode.FreeEmptyBuffer: 1793>
-    FreeUnknowBuffer: ArducamEvkSDK.ErrorCode # value = <ErrorCode.FreeUnknowBuffer: 1794>
-    InitCameraFailed: ArducamEvkSDK.ErrorCode # value = <ErrorCode.InitCameraFailed: 769>
-    MemoryAllocateFailed: ArducamEvkSDK.ErrorCode # value = <ErrorCode.MemoryAllocateFailed: 770>
-    NotSupport: ArducamEvkSDK.ErrorCode # value = <ErrorCode.NotSupport: 61441>
-    OpenCameraFailed: ArducamEvkSDK.ErrorCode # value = <ErrorCode.OpenCameraFailed: 513>
-    ReadConfigFileFailed: ArducamEvkSDK.ErrorCode # value = <ErrorCode.ReadConfigFileFailed: 257>
-    RegisterMultipleCallback: ArducamEvkSDK.ErrorCode # value = <ErrorCode.RegisterMultipleCallback: 2049>
-    StateError: ArducamEvkSDK.ErrorCode # value = <ErrorCode.StateError: 32769>
-    Success: ArducamEvkSDK.ErrorCode # value = <ErrorCode.Success: 0>
-    USBTypeMismatch: ArducamEvkSDK.ErrorCode # value = <ErrorCode.USBTypeMismatch: 1025>
-    UnknownDeviceType: ArducamEvkSDK.ErrorCode # value = <ErrorCode.UnknownDeviceType: 515>
-    UnknownError: ArducamEvkSDK.ErrorCode # value = <ErrorCode.UnknownError: 65535>
-    UnknownUSBType: ArducamEvkSDK.ErrorCode # value = <ErrorCode.UnknownUSBType: 514>
-    UserdataAddrError: ArducamEvkSDK.ErrorCode # value = <ErrorCode.UserdataAddrError: 65377>
-    UserdataLenError: ArducamEvkSDK.ErrorCode # value = <ErrorCode.UserdataLenError: 65378>
-    VRCommandError: ArducamEvkSDK.ErrorCode # value = <ErrorCode.VRCommandError: 65283>
-    __members__: dict # value = {'Success': <ErrorCode.Success: 0>, 'Empty': <ErrorCode.Empty: 16>, 'ReadConfigFileFailed': <ErrorCode.ReadConfigFileFailed: 257>, 'ConfigFileEmpty': <ErrorCode.ConfigFileEmpty: 258>, 'ConfigFormatError': <ErrorCode.ConfigFormatError: 259>, 'ControlFormatError': <ErrorCode.ControlFormatError: 260>, 'OpenCameraFailed': <ErrorCode.OpenCameraFailed: 513>, 'UnknownUSBType': <ErrorCode.UnknownUSBType: 514>, 'UnknownDeviceType': <ErrorCode.UnknownDeviceType: 515>, 'InitCameraFailed': <ErrorCode.InitCameraFailed: 769>, 'MemoryAllocateFailed': <ErrorCode.MemoryAllocateFailed: 770>, 'USBTypeMismatch': <ErrorCode.USBTypeMismatch: 1025>, 'CaptureTimeout': <ErrorCode.CaptureTimeout: 1537>, 'CaptureMethodConflict': <ErrorCode.CaptureMethodConflict: 1538>, 'FreeEmptyBuffer': <ErrorCode.FreeEmptyBuffer: 1793>, 'FreeUnknowBuffer': <ErrorCode.FreeUnknowBuffer: 1794>, 'RegisterMultipleCallback': <ErrorCode.RegisterMultipleCallback: 2049>, 'StateError': <ErrorCode.StateError: 32769>, 'NotSupport': <ErrorCode.NotSupport: 61441>, 'VRCommandError': <ErrorCode.VRCommandError: 65283>, 'UserdataAddrError': <ErrorCode.UserdataAddrError: 65377>, 'UserdataLenError': <ErrorCode.UserdataLenError: 65378>, 'UnknownError': <ErrorCode.UnknownError: 65535>}
-    pass
-class EventCode():
+        ...
+class EventCode:
     """
     Members:
-
+    
       FrameStart : Frame start
-
+    
       FrameEnd : Frame end
-
+    
       Exit : Exit
-
+    
       TransferError : Transfer error
-
+    
       TransferTimeout : Transfer timeout
-
+    
+      TransferLengthError : Transfer length error
+    
       DeviceConnect : Device connect
-
+    
       DeviceDisconnect : Device disconnect
     """
-    def __eq__(self, other: object) -> bool: ...
-    def __getstate__(self) -> int: ...
-    def __hash__(self) -> int: ...
-    def __index__(self) -> int: ...
-    def __init__(self, value: int) -> None: ...
-    def __int__(self) -> int: ...
-    def __ne__(self, other: object) -> bool: ...
-    def __repr__(self) -> str: ...
-    def __setstate__(self, state: int) -> None: ...
+    DeviceConnect: typing.ClassVar[EventCode]  # value = <EventCode.DeviceConnect: 512>
+    DeviceDisconnect: typing.ClassVar[EventCode]  # value = <EventCode.DeviceDisconnect: 514>
+    Exit: typing.ClassVar[EventCode]  # value = <EventCode.Exit: 3>
+    FrameEnd: typing.ClassVar[EventCode]  # value = <EventCode.FrameEnd: 2>
+    FrameStart: typing.ClassVar[EventCode]  # value = <EventCode.FrameStart: 1>
+    TransferError: typing.ClassVar[EventCode]  # value = <EventCode.TransferError: 256>
+    TransferLengthError: typing.ClassVar[EventCode]  # value = <EventCode.TransferLengthError: 258>
+    TransferTimeout: typing.ClassVar[EventCode]  # value = <EventCode.TransferTimeout: 257>
+    __members__: typing.ClassVar[dict[str, EventCode]]  # value = {'FrameStart': <EventCode.FrameStart: 1>, 'FrameEnd': <EventCode.FrameEnd: 2>, 'Exit': <EventCode.Exit: 3>, 'TransferError': <EventCode.TransferError: 256>, 'TransferTimeout': <EventCode.TransferTimeout: 257>, 'TransferLengthError': <EventCode.TransferLengthError: 258>, 'DeviceConnect': <EventCode.DeviceConnect: 512>, 'DeviceDisconnect': <EventCode.DeviceDisconnect: 514>}
+    def __eq__(self, other: typing.Any) -> bool:
+        ...
+    def __getstate__(self) -> int:
+        ...
+    def __hash__(self) -> int:
+        ...
+    def __index__(self) -> int:
+        ...
+    def __init__(self, value: int) -> None:
+        ...
+    def __int__(self) -> int:
+        ...
+    def __ne__(self, other: typing.Any) -> bool:
+        ...
+    def __repr__(self) -> str:
+        ...
+    def __setstate__(self, state: int) -> None:
+        ...
+    def __str__(self) -> str:
+        ...
     @property
     def name(self) -> str:
-        """
-        :type: str
-        """
+        ...
     @property
     def value(self) -> int:
-        """
-        :type: int
-        """
-    DeviceConnect: ArducamEvkSDK.EventCode # value = <EventCode.DeviceConnect: 512>
-    DeviceDisconnect: ArducamEvkSDK.EventCode # value = <EventCode.DeviceDisconnect: 513>
-    Exit: ArducamEvkSDK.EventCode # value = <EventCode.Exit: 3>
-    FrameEnd: ArducamEvkSDK.EventCode # value = <EventCode.FrameEnd: 2>
-    FrameStart: ArducamEvkSDK.EventCode # value = <EventCode.FrameStart: 1>
-    TransferError: ArducamEvkSDK.EventCode # value = <EventCode.TransferError: 256>
-    TransferTimeout: ArducamEvkSDK.EventCode # value = <EventCode.TransferTimeout: 257>
-    __members__: dict # value = {'FrameStart': <EventCode.FrameStart: 1>, 'FrameEnd': <EventCode.FrameEnd: 2>, 'Exit': <EventCode.Exit: 3>, 'TransferError': <EventCode.TransferError: 256>, 'TransferTimeout': <EventCode.TransferTimeout: 257>, 'DeviceConnect': <EventCode.DeviceConnect: 512>, 'DeviceDisconnect': <EventCode.DeviceDisconnect: 513>}
-    pass
-class Format():
-    def __init__(self) -> None: ...
+        ...
+class Format:
+    def __init__(self) -> None:
+        ...
     @property
     def bit_depth(self) -> int:
         """
         A property of bit_depth.
-
-        :type: int
         """
     @bit_depth.setter
     def bit_depth(self, arg0: int) -> None:
-        """
-        A property of bit_depth.
-        """
+        ...
     @property
     def format_code(self) -> int:
         """
         A property of format_code.
-
-        :type: int
         """
     @format_code.setter
     def format_code(self, arg0: int) -> None:
-        """
-        A property of format_code.
-        """
+        ...
     @property
     def height(self) -> int:
         """
         A property of height.
-
-        :type: int
         """
     @height.setter
     def height(self, arg0: int) -> None:
-        """
-        A property of height.
-        """
+        ...
     @property
     def width(self) -> int:
         """
         A property of width.
-
-        :type: int
         """
     @width.setter
     def width(self, arg0: int) -> None:
-        """
-        A property of width.
-        """
-    pass
-class FormatMode():
+        ...
+class FormatMode:
     """
     Members:
-
+    
       RAW : RAW
-
+    
       RGB : RGB
-
+    
       YUV : YUV
-
+    
       JPG : JPG
-
+    
       MON : MON
-
+    
       RAW_D : RAW_D
-
+    
       MON_D : MON_D
-
+    
+      TOF : TOF, deprecated
+    
       STATS : STATS
+    
+      RGB_IR : RGB_IR
     """
-    def __eq__(self, other: object) -> bool: ...
-    def __getstate__(self) -> int: ...
-    def __hash__(self) -> int: ...
-    def __index__(self) -> int: ...
-    def __init__(self, value: int) -> None: ...
-    def __int__(self) -> int: ...
-    def __ne__(self, other: object) -> bool: ...
-    def __repr__(self) -> str: ...
-    def __setstate__(self, state: int) -> None: ...
+    JPG: typing.ClassVar[FormatMode]  # value = <FormatMode.JPG: 3>
+    MON: typing.ClassVar[FormatMode]  # value = <FormatMode.MON: 4>
+    MON_D: typing.ClassVar[FormatMode]  # value = <FormatMode.MON_D: 6>
+    RAW: typing.ClassVar[FormatMode]  # value = <FormatMode.RAW: 0>
+    RAW_D: typing.ClassVar[FormatMode]  # value = <FormatMode.RAW_D: 5>
+    RGB: typing.ClassVar[FormatMode]  # value = <FormatMode.RGB: 1>
+    RGB_IR: typing.ClassVar[FormatMode]  # value = <FormatMode.RGB_IR: 9>
+    STATS: typing.ClassVar[FormatMode]  # value = <FormatMode.STATS: 8>
+    TOF: typing.ClassVar[FormatMode]  # value = <FormatMode.TOF: 7>
+    YUV: typing.ClassVar[FormatMode]  # value = <FormatMode.YUV: 2>
+    __members__: typing.ClassVar[dict[str, FormatMode]]  # value = {'RAW': <FormatMode.RAW: 0>, 'RGB': <FormatMode.RGB: 1>, 'YUV': <FormatMode.YUV: 2>, 'JPG': <FormatMode.JPG: 3>, 'MON': <FormatMode.MON: 4>, 'RAW_D': <FormatMode.RAW_D: 5>, 'MON_D': <FormatMode.MON_D: 6>, 'TOF': <FormatMode.TOF: 7>, 'STATS': <FormatMode.STATS: 8>, 'RGB_IR': <FormatMode.RGB_IR: 9>}
+    def __eq__(self, other: typing.Any) -> bool:
+        ...
+    def __getstate__(self) -> int:
+        ...
+    def __hash__(self) -> int:
+        ...
+    def __index__(self) -> int:
+        ...
+    def __init__(self, value: int) -> None:
+        ...
+    def __int__(self) -> int:
+        ...
+    def __ne__(self, other: typing.Any) -> bool:
+        ...
+    def __repr__(self) -> str:
+        ...
+    def __setstate__(self, state: int) -> None:
+        ...
+    def __str__(self) -> str:
+        ...
     @property
     def name(self) -> str:
-        """
-        :type: str
-        """
+        ...
     @property
     def value(self) -> int:
-        """
-        :type: int
-        """
-    JPG: ArducamEvkSDK.FormatMode # value = <FormatMode.JPG: 3>
-    MON: ArducamEvkSDK.FormatMode # value = <FormatMode.MON: 4>
-    MON_D: ArducamEvkSDK.FormatMode # value = <FormatMode.MON_D: 6>
-    RAW: ArducamEvkSDK.FormatMode # value = <FormatMode.RAW: 0>
-    RAW_D: ArducamEvkSDK.FormatMode # value = <FormatMode.RAW_D: 5>
-    RGB: ArducamEvkSDK.FormatMode # value = <FormatMode.RGB: 1>
-    STATS: ArducamEvkSDK.FormatMode # value = <FormatMode.STATS: 8>
-    YUV: ArducamEvkSDK.FormatMode # value = <FormatMode.YUV: 2>
-    __members__: dict # value = {'RAW': <FormatMode.RAW: 0>, 'RGB': <FormatMode.RGB: 1>, 'YUV': <FormatMode.YUV: 2>, 'JPG': <FormatMode.JPG: 3>, 'MON': <FormatMode.MON: 4>, 'RAW_D': <FormatMode.RAW_D: 5>, 'MON_D': <FormatMode.MON_D: 6>, 'STATS': <FormatMode.STATS: 8>}
-    pass
-class Frame():
-    def __init__(self) -> None: ...
+        ...
+class Frame:
+    def __init__(self) -> None:
+        ...
     @property
     def bad(self) -> bool:
         """
         A property of bad.
-
-        :type: bool
         """
     @bad.setter
     def bad(self, arg0: bool) -> None:
-        """
-        A property of bad.
-        """
+        ...
     @property
-    def data(self) -> numpy.ndarray[numpy.uint8]:
+    def data(self) -> numpy.ndarray[typing.Any, numpy.dtype[numpy.uint8]]:
         """
         A property of data.
-
-        :type: numpy.ndarray[numpy.uint8]
         """
     @data.setter
-    def data(self, arg0: numpy.ndarray[numpy.uint8]) -> None:
-        """
-        A property of data.
-        """
+    def data(self, arg0: numpy.ndarray[typing.Any, numpy.dtype[numpy.uint8]]) -> None:
+        ...
     @property
     def format(self) -> Format:
         """
         A property of format.
-
-        :type: Format
         """
     @format.setter
     def format(self, arg0: Format) -> None:
-        """
-        A property of format.
-        """
+        ...
     @property
     def seq(self) -> int:
         """
         A property of seq.
-
-        :type: int
         """
     @seq.setter
     def seq(self, arg0: int) -> None:
-        """
-        A property of seq.
-        """
-    pass
-class I2CMode():
+        ...
+class I2CMode:
     """
     Members:
-
+    
       I2C_MODE_8_8 : 8-bit register address and 8-bit data
-
+    
       I2C_MODE_8_16 : 8-bit register address and 16-bit data
-
+    
       I2C_MODE_16_8 : 16-bit register address and 8-bit data
-
+    
       I2C_MODE_16_16 : 16-bit register address and 16-bit data
-
+    
       I2C_MODE_16_32 : 16-bit register address and 32-bit data
     """
-    def __eq__(self, other: object) -> bool: ...
-    def __getstate__(self) -> int: ...
-    def __hash__(self) -> int: ...
-    def __index__(self) -> int: ...
-    def __init__(self, value: int) -> None: ...
-    def __int__(self) -> int: ...
-    def __ne__(self, other: object) -> bool: ...
-    def __repr__(self) -> str: ...
-    def __setstate__(self, state: int) -> None: ...
+    I2C_MODE_16_16: typing.ClassVar[I2CMode]  # value = <I2CMode.I2C_MODE_16_16: 3>
+    I2C_MODE_16_32: typing.ClassVar[I2CMode]  # value = <I2CMode.I2C_MODE_16_32: 4>
+    I2C_MODE_16_8: typing.ClassVar[I2CMode]  # value = <I2CMode.I2C_MODE_16_8: 2>
+    I2C_MODE_8_16: typing.ClassVar[I2CMode]  # value = <I2CMode.I2C_MODE_8_16: 1>
+    I2C_MODE_8_8: typing.ClassVar[I2CMode]  # value = <I2CMode.I2C_MODE_8_8: 0>
+    __members__: typing.ClassVar[dict[str, I2CMode]]  # value = {'I2C_MODE_8_8': <I2CMode.I2C_MODE_8_8: 0>, 'I2C_MODE_8_16': <I2CMode.I2C_MODE_8_16: 1>, 'I2C_MODE_16_8': <I2CMode.I2C_MODE_16_8: 2>, 'I2C_MODE_16_16': <I2CMode.I2C_MODE_16_16: 3>, 'I2C_MODE_16_32': <I2CMode.I2C_MODE_16_32: 4>}
+    def __eq__(self, other: typing.Any) -> bool:
+        ...
+    def __getstate__(self) -> int:
+        ...
+    def __hash__(self) -> int:
+        ...
+    def __index__(self) -> int:
+        ...
+    def __init__(self, value: int) -> None:
+        ...
+    def __int__(self) -> int:
+        ...
+    def __ne__(self, other: typing.Any) -> bool:
+        ...
+    def __repr__(self) -> str:
+        ...
+    def __setstate__(self, state: int) -> None:
+        ...
+    def __str__(self) -> str:
+        ...
     @property
     def name(self) -> str:
-        """
-        :type: str
-        """
+        ...
     @property
     def value(self) -> int:
-        """
-        :type: int
-        """
-    I2C_MODE_16_16: ArducamEvkSDK.I2CMode # value = <I2CMode.I2C_MODE_16_16: 3>
-    I2C_MODE_16_32: ArducamEvkSDK.I2CMode # value = <I2CMode.I2C_MODE_16_32: 4>
-    I2C_MODE_16_8: ArducamEvkSDK.I2CMode # value = <I2CMode.I2C_MODE_16_8: 2>
-    I2C_MODE_8_16: ArducamEvkSDK.I2CMode # value = <I2CMode.I2C_MODE_8_16: 1>
-    I2C_MODE_8_8: ArducamEvkSDK.I2CMode # value = <I2CMode.I2C_MODE_8_8: 0>
-    __members__: dict # value = {'I2C_MODE_8_8': <I2CMode.I2C_MODE_8_8: 0>, 'I2C_MODE_8_16': <I2CMode.I2C_MODE_8_16: 1>, 'I2C_MODE_16_8': <I2CMode.I2C_MODE_16_8: 2>, 'I2C_MODE_16_16': <I2CMode.I2C_MODE_16_16: 3>, 'I2C_MODE_16_32': <I2CMode.I2C_MODE_16_32: 4>}
-    pass
-class LoggerLevel():
+        ...
+class LoggerLevel:
     """
     Members:
-
+    
       Trace : trace log level
-
+    
       Debug : debug log level
-
+    
       Info : info log level
-
+    
       Warn : warn log level
-
+    
       Err : err log level
-
+    
       Critical : critical log level
-
+    
       Off : off log level
     """
-    def __eq__(self, other: object) -> bool: ...
-    def __getstate__(self) -> int: ...
-    def __hash__(self) -> int: ...
-    def __index__(self) -> int: ...
-    def __init__(self, value: int) -> None: ...
-    def __int__(self) -> int: ...
-    def __ne__(self, other: object) -> bool: ...
-    def __repr__(self) -> str: ...
-    def __setstate__(self, state: int) -> None: ...
+    Critical: typing.ClassVar[LoggerLevel]  # value = <LoggerLevel.Critical: 5>
+    Debug: typing.ClassVar[LoggerLevel]  # value = <LoggerLevel.Debug: 1>
+    Err: typing.ClassVar[LoggerLevel]  # value = <LoggerLevel.Err: 4>
+    Info: typing.ClassVar[LoggerLevel]  # value = <LoggerLevel.Info: 2>
+    Off: typing.ClassVar[LoggerLevel]  # value = <LoggerLevel.Off: 6>
+    Trace: typing.ClassVar[LoggerLevel]  # value = <LoggerLevel.Trace: 0>
+    Warn: typing.ClassVar[LoggerLevel]  # value = <LoggerLevel.Warn: 3>
+    __members__: typing.ClassVar[dict[str, LoggerLevel]]  # value = {'Trace': <LoggerLevel.Trace: 0>, 'Debug': <LoggerLevel.Debug: 1>, 'Info': <LoggerLevel.Info: 2>, 'Warn': <LoggerLevel.Warn: 3>, 'Err': <LoggerLevel.Err: 4>, 'Critical': <LoggerLevel.Critical: 5>, 'Off': <LoggerLevel.Off: 6>}
+    def __eq__(self, other: typing.Any) -> bool:
+        ...
+    def __getstate__(self) -> int:
+        ...
+    def __hash__(self) -> int:
+        ...
+    def __index__(self) -> int:
+        ...
+    def __init__(self, value: int) -> None:
+        ...
+    def __int__(self) -> int:
+        ...
+    def __ne__(self, other: typing.Any) -> bool:
+        ...
+    def __repr__(self) -> str:
+        ...
+    def __setstate__(self, state: int) -> None:
+        ...
+    def __str__(self) -> str:
+        ...
     @property
     def name(self) -> str:
-        """
-        :type: str
-        """
+        ...
     @property
     def value(self) -> int:
-        """
-        :type: int
-        """
-    Critical: ArducamEvkSDK.LoggerLevel # value = <LoggerLevel.Critical: 5>
-    Debug: ArducamEvkSDK.LoggerLevel # value = <LoggerLevel.Debug: 1>
-    Err: ArducamEvkSDK.LoggerLevel # value = <LoggerLevel.Err: 4>
-    Info: ArducamEvkSDK.LoggerLevel # value = <LoggerLevel.Info: 2>
-    Off: ArducamEvkSDK.LoggerLevel # value = <LoggerLevel.Off: 6>
-    Trace: ArducamEvkSDK.LoggerLevel # value = <LoggerLevel.Trace: 0>
-    Warn: ArducamEvkSDK.LoggerLevel # value = <LoggerLevel.Warn: 3>
-    __members__: dict # value = {'Trace': <LoggerLevel.Trace: 0>, 'Debug': <LoggerLevel.Debug: 1>, 'Info': <LoggerLevel.Info: 2>, 'Warn': <LoggerLevel.Warn: 3>, 'Err': <LoggerLevel.Err: 4>, 'Critical': <LoggerLevel.Critical: 5>, 'Off': <LoggerLevel.Off: 6>}
-    pass
-class MemType():
+        ...
+class MemType:
     """
     Members:
-
+    
       DMA : DMA
-
+    
       RAM : RAM
     """
-    def __eq__(self, other: object) -> bool: ...
-    def __getstate__(self) -> int: ...
-    def __hash__(self) -> int: ...
-    def __index__(self) -> int: ...
-    def __init__(self, value: int) -> None: ...
-    def __int__(self) -> int: ...
-    def __ne__(self, other: object) -> bool: ...
-    def __repr__(self) -> str: ...
-    def __setstate__(self, state: int) -> None: ...
+    DMA: typing.ClassVar[MemType]  # value = <MemType.DMA: 1>
+    RAM: typing.ClassVar[MemType]  # value = <MemType.RAM: 2>
+    __members__: typing.ClassVar[dict[str, MemType]]  # value = {'DMA': <MemType.DMA: 1>, 'RAM': <MemType.RAM: 2>}
+    def __eq__(self, other: typing.Any) -> bool:
+        ...
+    def __getstate__(self) -> int:
+        ...
+    def __hash__(self) -> int:
+        ...
+    def __index__(self) -> int:
+        ...
+    def __init__(self, value: int) -> None:
+        ...
+    def __int__(self) -> int:
+        ...
+    def __ne__(self, other: typing.Any) -> bool:
+        ...
+    def __repr__(self) -> str:
+        ...
+    def __setstate__(self, state: int) -> None:
+        ...
+    def __str__(self) -> str:
+        ...
     @property
     def name(self) -> str:
-        """
-        :type: str
-        """
+        ...
     @property
     def value(self) -> int:
-        """
-        :type: int
-        """
-    DMA: ArducamEvkSDK.MemType # value = <MemType.DMA: 1>
-    RAM: ArducamEvkSDK.MemType # value = <MemType.RAM: 2>
-    __members__: dict # value = {'DMA': <MemType.DMA: 1>, 'RAM': <MemType.RAM: 2>}
-    pass
-class Param():
-    def __init__(self) -> None: 
+        ...
+class Param:
+    def __init__(self) -> None:
         """
         construct a default param
         """
     @property
     def bin_config(self) -> bool:
         """
         A property of bin_config.
-
-        :type: bool
         """
     @bin_config.setter
     def bin_config(self, arg0: bool) -> None:
-        """
-        A property of bin_config.
-        """
+        ...
     @property
     def config_file_name(self) -> str:
         """
         A property of config_file_name.
-
-        :type: str
         """
     @config_file_name.setter
     def config_file_name(self, arg0: str) -> None:
-        """
-        A property of config_file_name.
-        """
+        ...
     @property
     def device(self) -> Device:
         """
         A property of device.
-
-        :type: Device
         """
     @device.setter
     def device(self, arg0: Device) -> None:
+        ...
+    @property
+    def ext_config_file_name(self) -> str:
         """
-        A property of device.
+        A property of ext_config_file_name.
         """
+    @ext_config_file_name.setter
+    def ext_config_file_name(self, arg0: str) -> None:
+        ...
     @property
     def mem_type(self) -> MemType:
         """
         A property of mem_type.
-
-        :type: MemType
         """
     @mem_type.setter
     def mem_type(self, arg0: MemType) -> None:
-        """
-        A property of mem_type.
-        """
-    pass
-class USBSpeed():
+        ...
+class USBSpeed:
     """
     Members:
-
+    
       Unknown : The OS doesn't report or know the device speed.
-
+    
       Low : The device is operating at low speed (1.5MBit/s).
-
+    
       Full : The device is operating at full speed (12MBit/s).
-
+    
       High : The device is operating at high speed (480MBit/s).
-
+    
       Super : The device is operating at super speed (5000MBit/s).
-
+    
       SuperPlus : The device is operating at super speed plus (10000MBit/s).
     """
-    def __eq__(self, other: object) -> bool: ...
-    def __getstate__(self) -> int: ...
-    def __hash__(self) -> int: ...
-    def __index__(self) -> int: ...
-    def __init__(self, value: int) -> None: ...
-    def __int__(self) -> int: ...
-    def __ne__(self, other: object) -> bool: ...
-    def __repr__(self) -> str: ...
-    def __setstate__(self, state: int) -> None: ...
+    Full: typing.ClassVar[USBSpeed]  # value = <USBSpeed.Full: 2>
+    High: typing.ClassVar[USBSpeed]  # value = <USBSpeed.High: 3>
+    Low: typing.ClassVar[USBSpeed]  # value = <USBSpeed.Low: 1>
+    Super: typing.ClassVar[USBSpeed]  # value = <USBSpeed.Super: 4>
+    SuperPlus: typing.ClassVar[USBSpeed]  # value = <USBSpeed.SuperPlus: 5>
+    Unknown: typing.ClassVar[USBSpeed]  # value = <USBSpeed.Unknown: 0>
+    __members__: typing.ClassVar[dict[str, USBSpeed]]  # value = {'Unknown': <USBSpeed.Unknown: 0>, 'Low': <USBSpeed.Low: 1>, 'Full': <USBSpeed.Full: 2>, 'High': <USBSpeed.High: 3>, 'Super': <USBSpeed.Super: 4>, 'SuperPlus': <USBSpeed.SuperPlus: 5>}
+    def __eq__(self, other: typing.Any) -> bool:
+        ...
+    def __getstate__(self) -> int:
+        ...
+    def __hash__(self) -> int:
+        ...
+    def __index__(self) -> int:
+        ...
+    def __init__(self, value: int) -> None:
+        ...
+    def __int__(self) -> int:
+        ...
+    def __ne__(self, other: typing.Any) -> bool:
+        ...
+    def __repr__(self) -> str:
+        ...
+    def __setstate__(self, state: int) -> None:
+        ...
+    def __str__(self) -> str:
+        ...
     @property
     def name(self) -> str:
-        """
-        :type: str
-        """
+        ...
     @property
     def value(self) -> int:
-        """
-        :type: int
-        """
-    Full: ArducamEvkSDK.USBSpeed # value = <USBSpeed.Full: 2>
-    High: ArducamEvkSDK.USBSpeed # value = <USBSpeed.High: 3>
-    Low: ArducamEvkSDK.USBSpeed # value = <USBSpeed.Low: 1>
-    Super: ArducamEvkSDK.USBSpeed # value = <USBSpeed.Super: 4>
-    SuperPlus: ArducamEvkSDK.USBSpeed # value = <USBSpeed.SuperPlus: 5>
-    Unknown: ArducamEvkSDK.USBSpeed # value = <USBSpeed.Unknown: 0>
-    __members__: dict # value = {'Unknown': <USBSpeed.Unknown: 0>, 'Low': <USBSpeed.Low: 1>, 'Full': <USBSpeed.Full: 2>, 'High': <USBSpeed.High: 3>, 'Super': <USBSpeed.Super: 4>, 'SuperPlus': <USBSpeed.SuperPlus: 5>}
-    pass
-class VRCommandDirection():
+        ...
+class VRCommandDirection:
     """
     Members:
-
+    
       HostToDevice : Host to device
-
+    
       DeviceToHost : Device to host
     """
-    def __eq__(self, other: object) -> bool: ...
-    def __getstate__(self) -> int: ...
-    def __hash__(self) -> int: ...
-    def __index__(self) -> int: ...
-    def __init__(self, value: int) -> None: ...
-    def __int__(self) -> int: ...
-    def __ne__(self, other: object) -> bool: ...
-    def __repr__(self) -> str: ...
-    def __setstate__(self, state: int) -> None: ...
+    DeviceToHost: typing.ClassVar[VRCommandDirection]  # value = <VRCommandDirection.DeviceToHost: 128>
+    HostToDevice: typing.ClassVar[VRCommandDirection]  # value = <VRCommandDirection.HostToDevice: 0>
+    __members__: typing.ClassVar[dict[str, VRCommandDirection]]  # value = {'HostToDevice': <VRCommandDirection.HostToDevice: 0>, 'DeviceToHost': <VRCommandDirection.DeviceToHost: 128>}
+    def __eq__(self, other: typing.Any) -> bool:
+        ...
+    def __getstate__(self) -> int:
+        ...
+    def __hash__(self) -> int:
+        ...
+    def __index__(self) -> int:
+        ...
+    def __init__(self, value: int) -> None:
+        ...
+    def __int__(self) -> int:
+        ...
+    def __ne__(self, other: typing.Any) -> bool:
+        ...
+    def __repr__(self) -> str:
+        ...
+    def __setstate__(self, state: int) -> None:
+        ...
+    def __str__(self) -> str:
+        ...
     @property
     def name(self) -> str:
-        """
-        :type: str
-        """
+        ...
     @property
     def value(self) -> int:
-        """
-        :type: int
-        """
-    DeviceToHost: ArducamEvkSDK.VRCommandDirection # value = <VRCommandDirection.DeviceToHost: 128>
-    HostToDevice: ArducamEvkSDK.VRCommandDirection # value = <VRCommandDirection.HostToDevice: 0>
-    __members__: dict # value = {'HostToDevice': <VRCommandDirection.HostToDevice: 0>, 'DeviceToHost': <VRCommandDirection.DeviceToHost: 128>}
-    pass
-def free_device_list() -> None:
-    """
-    free the device list
-    """
+        ...
 def get_error_name(ec: int) -> str:
     """
     get the error name
     """
-def list_devices() -> typing.List[Device]:
-    """
-    list all supported devices
-    """
-CaptureMethodConflict: ArducamEvkSDK.ErrorCode # value = <ErrorCode.CaptureMethodConflict: 1538>
-CaptureTimeout: ArducamEvkSDK.ErrorCode # value = <ErrorCode.CaptureTimeout: 1537>
-ConfigFileEmpty: ArducamEvkSDK.ErrorCode # value = <ErrorCode.ConfigFileEmpty: 258>
-ConfigFormatError: ArducamEvkSDK.ErrorCode # value = <ErrorCode.ConfigFormatError: 259>
-ControlFormatError: ArducamEvkSDK.ErrorCode # value = <ErrorCode.ControlFormatError: 260>
-Critical: ArducamEvkSDK.LoggerLevel # value = <LoggerLevel.Critical: 5>
-DMA: ArducamEvkSDK.MemType # value = <MemType.DMA: 1>
-Debug: ArducamEvkSDK.LoggerLevel # value = <LoggerLevel.Debug: 1>
-DeviceConnect: ArducamEvkSDK.EventCode # value = <EventCode.DeviceConnect: 512>
-DeviceDisconnect: ArducamEvkSDK.EventCode # value = <EventCode.DeviceDisconnect: 513>
-DeviceToHost: ArducamEvkSDK.VRCommandDirection # value = <VRCommandDirection.DeviceToHost: 128>
-Empty: ArducamEvkSDK.ErrorCode # value = <ErrorCode.Empty: 16>
-Err: ArducamEvkSDK.LoggerLevel # value = <LoggerLevel.Err: 4>
-Exit: ArducamEvkSDK.EventCode # value = <EventCode.Exit: 3>
-FrameEnd: ArducamEvkSDK.EventCode # value = <EventCode.FrameEnd: 2>
-FrameStart: ArducamEvkSDK.EventCode # value = <EventCode.FrameStart: 1>
-FreeEmptyBuffer: ArducamEvkSDK.ErrorCode # value = <ErrorCode.FreeEmptyBuffer: 1793>
-FreeUnknowBuffer: ArducamEvkSDK.ErrorCode # value = <ErrorCode.FreeUnknowBuffer: 1794>
-Full: ArducamEvkSDK.USBSpeed # value = <USBSpeed.Full: 2>
-High: ArducamEvkSDK.USBSpeed # value = <USBSpeed.High: 3>
-HostToDevice: ArducamEvkSDK.VRCommandDirection # value = <VRCommandDirection.HostToDevice: 0>
-I2C_MODE_16_16: ArducamEvkSDK.I2CMode # value = <I2CMode.I2C_MODE_16_16: 3>
-I2C_MODE_16_32: ArducamEvkSDK.I2CMode # value = <I2CMode.I2C_MODE_16_32: 4>
-I2C_MODE_16_8: ArducamEvkSDK.I2CMode # value = <I2CMode.I2C_MODE_16_8: 2>
-I2C_MODE_8_16: ArducamEvkSDK.I2CMode # value = <I2CMode.I2C_MODE_8_16: 1>
-I2C_MODE_8_8: ArducamEvkSDK.I2CMode # value = <I2CMode.I2C_MODE_8_8: 0>
-Info: ArducamEvkSDK.LoggerLevel # value = <LoggerLevel.Info: 2>
-InitCameraFailed: ArducamEvkSDK.ErrorCode # value = <ErrorCode.InitCameraFailed: 769>
-JPG: ArducamEvkSDK.FormatMode # value = <FormatMode.JPG: 3>
-Low: ArducamEvkSDK.USBSpeed # value = <USBSpeed.Low: 1>
-MON: ArducamEvkSDK.FormatMode # value = <FormatMode.MON: 4>
-MON_D: ArducamEvkSDK.FormatMode # value = <FormatMode.MON_D: 6>
-MemoryAllocateFailed: ArducamEvkSDK.ErrorCode # value = <ErrorCode.MemoryAllocateFailed: 770>
-NotSupport: ArducamEvkSDK.ErrorCode # value = <ErrorCode.NotSupport: 61441>
-Off: ArducamEvkSDK.LoggerLevel # value = <LoggerLevel.Off: 6>
-OpenCameraFailed: ArducamEvkSDK.ErrorCode # value = <ErrorCode.OpenCameraFailed: 513>
-RAM: ArducamEvkSDK.MemType # value = <MemType.RAM: 2>
-RAW: ArducamEvkSDK.FormatMode # value = <FormatMode.RAW: 0>
-RAW_D: ArducamEvkSDK.FormatMode # value = <FormatMode.RAW_D: 5>
-RGB: ArducamEvkSDK.FormatMode # value = <FormatMode.RGB: 1>
-ReadConfigFileFailed: ArducamEvkSDK.ErrorCode # value = <ErrorCode.ReadConfigFileFailed: 257>
-RegisterMultipleCallback: ArducamEvkSDK.ErrorCode # value = <ErrorCode.RegisterMultipleCallback: 2049>
-STATS: ArducamEvkSDK.FormatMode # value = <FormatMode.STATS: 8>
-StateError: ArducamEvkSDK.ErrorCode # value = <ErrorCode.StateError: 32769>
-Success: ArducamEvkSDK.ErrorCode # value = <ErrorCode.Success: 0>
-Super: ArducamEvkSDK.USBSpeed # value = <USBSpeed.Super: 4>
-SuperPlus: ArducamEvkSDK.USBSpeed # value = <USBSpeed.SuperPlus: 5>
-Trace: ArducamEvkSDK.LoggerLevel # value = <LoggerLevel.Trace: 0>
-TransferError: ArducamEvkSDK.EventCode # value = <EventCode.TransferError: 256>
-TransferTimeout: ArducamEvkSDK.EventCode # value = <EventCode.TransferTimeout: 257>
-USBTypeMismatch: ArducamEvkSDK.ErrorCode # value = <ErrorCode.USBTypeMismatch: 1025>
-Unknown: ArducamEvkSDK.USBSpeed # value = <USBSpeed.Unknown: 0>
-UnknownDeviceType: ArducamEvkSDK.ErrorCode # value = <ErrorCode.UnknownDeviceType: 515>
-UnknownError: ArducamEvkSDK.ErrorCode # value = <ErrorCode.UnknownError: 65535>
-UnknownUSBType: ArducamEvkSDK.ErrorCode # value = <ErrorCode.UnknownUSBType: 514>
-UserdataAddrError: ArducamEvkSDK.ErrorCode # value = <ErrorCode.UserdataAddrError: 65377>
-UserdataLenError: ArducamEvkSDK.ErrorCode # value = <ErrorCode.UserdataLenError: 65378>
-VRCommandError: ArducamEvkSDK.ErrorCode # value = <ErrorCode.VRCommandError: 65283>
-Warn: ArducamEvkSDK.LoggerLevel # value = <LoggerLevel.Warn: 3>
-YUV: ArducamEvkSDK.FormatMode # value = <FormatMode.YUV: 2>
-__version__ = 'dev'
+CaptureMethodConflict: ErrorCode  # value = <ErrorCode.CaptureMethodConflict: 1538>
+CaptureTimeout: ErrorCode  # value = <ErrorCode.CaptureTimeout: 1537>
+ConfigFileEmpty: ErrorCode  # value = <ErrorCode.ConfigFileEmpty: 258>
+ConfigFormatError: ErrorCode  # value = <ErrorCode.ConfigFormatError: 259>
+ControlFormatError: ErrorCode  # value = <ErrorCode.ControlFormatError: 260>
+Critical: LoggerLevel  # value = <LoggerLevel.Critical: 5>
+DMA: MemType  # value = <MemType.DMA: 1>
+Debug: LoggerLevel  # value = <LoggerLevel.Debug: 1>
+DeviceConnect: EventCode  # value = <EventCode.DeviceConnect: 512>
+DeviceDisconnect: EventCode  # value = <EventCode.DeviceDisconnect: 514>
+DeviceToHost: VRCommandDirection  # value = <VRCommandDirection.DeviceToHost: 128>
+Empty: ErrorCode  # value = <ErrorCode.Empty: 16>
+Err: LoggerLevel  # value = <LoggerLevel.Err: 4>
+Exit: EventCode  # value = <EventCode.Exit: 3>
+FrameEnd: EventCode  # value = <EventCode.FrameEnd: 2>
+FrameStart: EventCode  # value = <EventCode.FrameStart: 1>
+FreeEmptyBuffer: ErrorCode  # value = <ErrorCode.FreeEmptyBuffer: 1793>
+FreeUnknowBuffer: ErrorCode  # value = <ErrorCode.FreeUnknowBuffer: 1794>
+Full: USBSpeed  # value = <USBSpeed.Full: 2>
+High: USBSpeed  # value = <USBSpeed.High: 3>
+HostToDevice: VRCommandDirection  # value = <VRCommandDirection.HostToDevice: 0>
+I2C_MODE_16_16: I2CMode  # value = <I2CMode.I2C_MODE_16_16: 3>
+I2C_MODE_16_32: I2CMode  # value = <I2CMode.I2C_MODE_16_32: 4>
+I2C_MODE_16_8: I2CMode  # value = <I2CMode.I2C_MODE_16_8: 2>
+I2C_MODE_8_16: I2CMode  # value = <I2CMode.I2C_MODE_8_16: 1>
+I2C_MODE_8_8: I2CMode  # value = <I2CMode.I2C_MODE_8_8: 0>
+Info: LoggerLevel  # value = <LoggerLevel.Info: 2>
+InitCameraFailed: ErrorCode  # value = <ErrorCode.InitCameraFailed: 769>
+JPG: FormatMode  # value = <FormatMode.JPG: 3>
+Low: USBSpeed  # value = <USBSpeed.Low: 1>
+MON: FormatMode  # value = <FormatMode.MON: 4>
+MON_D: FormatMode  # value = <FormatMode.MON_D: 6>
+MemoryAllocateFailed: ErrorCode  # value = <ErrorCode.MemoryAllocateFailed: 770>
+NotSupported: ErrorCode  # value = <ErrorCode.NotSupported: 61441>
+Off: LoggerLevel  # value = <LoggerLevel.Off: 6>
+OpenCameraFailed: ErrorCode  # value = <ErrorCode.OpenCameraFailed: 513>
+RAM: MemType  # value = <MemType.RAM: 2>
+RAW: FormatMode  # value = <FormatMode.RAW: 0>
+RAW_D: FormatMode  # value = <FormatMode.RAW_D: 5>
+RGB: FormatMode  # value = <FormatMode.RGB: 1>
+RGB_IR: FormatMode  # value = <FormatMode.RGB_IR: 9>
+ReadConfigFileFailed: ErrorCode  # value = <ErrorCode.ReadConfigFileFailed: 257>
+RegisterMultipleCallback: ErrorCode  # value = <ErrorCode.RegisterMultipleCallback: 2049>
+STATS: FormatMode  # value = <FormatMode.STATS: 8>
+StateError: ErrorCode  # value = <ErrorCode.StateError: 32769>
+Success: ErrorCode  # value = <ErrorCode.Success: 0>
+Super: USBSpeed  # value = <USBSpeed.Super: 4>
+SuperPlus: USBSpeed  # value = <USBSpeed.SuperPlus: 5>
+TOF: FormatMode  # value = <FormatMode.TOF: 7>
+Trace: LoggerLevel  # value = <LoggerLevel.Trace: 0>
+TransferError: EventCode  # value = <EventCode.TransferError: 256>
+TransferLengthError: EventCode  # value = <EventCode.TransferLengthError: 258>
+TransferTimeout: EventCode  # value = <EventCode.TransferTimeout: 257>
+USBTypeMismatch: ErrorCode  # value = <ErrorCode.USBTypeMismatch: 1025>
+Unknown: USBSpeed  # value = <USBSpeed.Unknown: 0>
+UnknownDeviceType: ErrorCode  # value = <ErrorCode.UnknownDeviceType: 515>
+UnknownError: ErrorCode  # value = <ErrorCode.UnknownError: 65535>
+UnknownUSBType: ErrorCode  # value = <ErrorCode.UnknownUSBType: 514>
+UserdataAddrError: ErrorCode  # value = <ErrorCode.UserdataAddrError: 65377>
+UserdataLenError: ErrorCode  # value = <ErrorCode.UserdataLenError: 65378>
+VRCommandError: ErrorCode  # value = <ErrorCode.VRCommandError: 65283>
+Warn: LoggerLevel  # value = <LoggerLevel.Warn: 3>
+YUV: FormatMode  # value = <FormatMode.YUV: 2>
+__version__: str = 'v1.0.0-32-g3232694'
```

