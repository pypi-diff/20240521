# Comparing `tmp/brightify-0.1.0.tar.gz` & `tmp/brightify-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brightify-0.1.0.tar", last modified: Mon May 20 11:52:09 2024, max compression
+gzip compressed data, was "brightify-0.1.1.tar", last modified: Mon May 20 23:30:08 2024, max compression
```

## Comparing `brightify-0.1.0.tar` & `brightify-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:52:09.287206 brightify-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:52:09.283206 brightify-0.1.0/Brightify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-20 11:52:09.000000 brightify-0.1.0/Brightify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-20 11:52:09.000000 brightify-0.1.0/Brightify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:52:09.000000 brightify-0.1.0/Brightify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-20 11:52:09.000000 brightify-0.1.0/Brightify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 11:52:09.000000 brightify-0.1.0/Brightify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-20 11:52:04.000000 brightify-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-20 11:52:09.283206 brightify-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-20 11:52:04.000000 brightify-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:52:09.283206 brightify-0.1.0/brightify/
--rw-r--r--   0 runner    (1001) docker     (127)    11184 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/BaseApp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/Brightylog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/SensorComm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/UIConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/log_config.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:52:09.283206 brightify-0.1.0/brightify/monitors/
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/monitors/MonitorBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/monitors/MonitorDDCCI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/monitors/MonitorGeneric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/monitors/MonitorUSB.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/monitors/m27q.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:52:09.283206 brightify-0.1.0/brightify/res/
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/res/icon_dark.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/res/icon_light.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:52:09.279206 brightify-0.1.0/brightify/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:52:09.283206 brightify-0.1.0/brightify/scripts/windows/
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/scripts/windows/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/scripts/windows/add_startup_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/scripts/windows/remove_startup_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:52:09.283206 brightify-0.1.0/brightify/sensor_firmware/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/sensor_firmware/platformio.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:52:09.283206 brightify-0.1.0/brightify/sensor_firmware/src/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/sensor_firmware/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:52:09.283206 brightify-0.1.0/brightify/windows/
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/windows/WindowsApp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-20 11:52:04.000000 brightify-0.1.0/brightify/windows/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-20 11:52:04.000000 brightify-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 11:52:09.287206 brightify-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:30:08.841576 brightify-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:30:08.841576 brightify-0.1.1/Brightify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-20 23:30:08.000000 brightify-0.1.1/Brightify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-20 23:30:08.000000 brightify-0.1.1/Brightify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 23:30:08.000000 brightify-0.1.1/Brightify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-20 23:30:08.000000 brightify-0.1.1/Brightify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 23:30:08.000000 brightify-0.1.1/Brightify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-20 23:30:04.000000 brightify-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-20 23:30:08.841576 brightify-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-20 23:30:04.000000 brightify-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:30:08.841576 brightify-0.1.1/brightify/
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/BaseApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/Brightylog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/SensorComm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/UIConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/log_config.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:30:08.841576 brightify-0.1.1/brightify/monitors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/monitors/MonitorBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/monitors/MonitorDDCCI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/monitors/MonitorGeneric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/monitors/MonitorUSB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/monitors/m27q.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:30:08.841576 brightify-0.1.1/brightify/res/
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/res/icon_dark.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/res/icon_light.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:30:08.841576 brightify-0.1.1/brightify/sensor_firmware/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/sensor_firmware/platformio.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:30:08.841576 brightify-0.1.1/brightify/sensor_firmware/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/sensor_firmware/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:30:08.841576 brightify-0.1.1/brightify/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/windows/WindowsApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/windows/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/windows/add_startup_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/windows/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/windows/remove_startup_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-20 23:30:04.000000 brightify-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 23:30:08.841576 brightify-0.1.1/setup.cfg
```

### Comparing `brightify-0.1.0/Brightify.egg-info/PKG-INFO` & `brightify-0.1.1/Brightify.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 Metadata-Version: 2.1
 Name: Brightify
-Version: 0.1.0
-Summary: A tool to control the brightness of your screens.
+Version: 0.1.1
+Summary: The Brightify application allows users to adjust the brightness of their monitors.
 Author-email: "Robin S." <brightify@rs-web.net>
 Keywords: brightness,monitor,screen,control,tool
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: platformio
 Requires-Dist: pyserial
 Requires-Dist: libusb1
 Requires-Dist: PyQt6
 Requires-Dist: monitorcontrol
 Requires-Dist: pywin32; platform_system == "Windows"
 Requires-Dist: winshell; platform_system == "Windows"
 
-# Getting started
-
-1. Install brightify by running `pip install .` in the main directory. When developing, you can use `pip install -e .`
-   to install the package in editable mode.
+# Brightify
+This app allows you to set the brightness of your monitor(s). It is essentially a wrapper around the [DDC/CI](https://en.wikipedia.org/wiki/Display_Data_Channel#DDC/CI) protocol, which is supported by most monitors.
+It also supports adding custom communication protocols to control the brightness of USB monitors. For this, you most likely need to reverse engineer the communication protocol of the monitor. In my experience, this provides a more stable experience than using the DDC/CI protocol.
+You can find an example implementation for the [Gigabyte M27Q](https://www.gigabyte.com/Monitor/M27Q) in [here](brightify/monitors/m27q.py).
+The app is designed to be run in the background and can be controlled via a taskbar icon. It also supports a brightness sensor that can automatically adjust the brightness based on the ambient light.
+
+## Getting started
+1. Install brightify by running `pip install Brightify`. This package is regularly uploaded to PyPi. If you want to install the latest version, you can clone this repository from 
+[GitHub](https://github.com/RerikOp/Brightify) and install it with `pip install -e .` in the root directory.
 2. To start the app: `python -m brightify run`. You can exit either by right-clicking the icon in the taskbar and
    selecting "Exit" or by pressing `Ctrl+C` in the terminal.
-3. There are several other arguments you can pass to the app, see `python -m brightify --help` for more information.
-    1. To start the app at startup `python -m add startup` (Equivalent
-       to `python -m add startup --mode startup-folder`).
-       By default, the terminal will be hidden, but you can change
-       this by passing the `--force-console` argument.
-       To remove the startup task, run `python -m remove startup`. On Windows you can also use the Task Scheduler, which
-       requires elevated permissions to add the app to startup.
-       For this, run `python -m brightify add startup --mode task_scheduler` and to remove it `python -m brightify
-       remove startup --mode task_scheduler`.
-    2. To add a menu icon `python -m brightify add menu-icon`. Again, you can pass the `--force-console` argument
-       force the terminal.
-       To remove the icon, run `python -m remove menu-icon`.
-
-# Set up the brightness sensor
-
-1. Modify the [SensorComm](brightify/SensorComm.py) class to match your device and firmware
-2. Modify the code that is polling from the brightness sensor [Device Firmware](brightify/sensor_firmware/src)
-3. Modify [platformio.ini](brightify/sensor_firmware/platformio.ini) and enter your board (
+3. To start the app at startup (or logon) and add a menu icon, run `python -m add all`. To remove the both, run
+   `python -m remove all`.
+
+## Optional arguments
+There are several other arguments you can pass to the app, see `python -m brightify --help` for more information.
+- To target add/remove only the startup run `python -m brightify add/remove startup`.
+   - To add a task to the task scheduler on Windows, pass `--use-scheduler`. It will request elevated permissions.
+   - By default, the terminal will be hidden, but you can change this by passing the `--force-console` argument.
+- To add/remove only the menu icon run `python -m brightify add/remove menu-icon`.
+   - You can again force the console to be shown by passing the `--force-console` argument.
+
+## Set up the brightness sensor
+- Modify the [SensorComm](brightify/SensorComm.py) class to match your device and firmware
+- Modify the code that is polling from the brightness sensor [Device Firmware](brightify/sensor_firmware/src)
+- Modify [platformio.ini](brightify/sensor_firmware/platformio.ini) and enter your board (
    see [supported boards](https://docs.platformio.org/en/latest/boards/index.html))
-4. Run `pio run -t upload` in the terminal to upload the firmware to the board.
+- Run `pio run -t upload` in the terminal to upload the firmware to the board.
    If everything is working, the *Auto* Checkbox for each supported Monitor should now be clickable
 
-# Remarks
-
-+ Currently, only the Windows task bar icon is supported, the main part of this app is OS independent
-+ Feel free to create a pull request and add your own USB Monitor
+## Remarks
+- Currently, only the Windows task bar icon is supported, the main part of this app is OS independent.
+- Feel free to create a pull request and add your own USB Monitor
```

### Comparing `brightify-0.1.0/Brightify.egg-info/SOURCES.txt` & `brightify-0.1.1/Brightify.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,14 @@
 brightify/monitors/MonitorBase.py
 brightify/monitors/MonitorDDCCI.py
 brightify/monitors/MonitorGeneric.py
 brightify/monitors/MonitorUSB.py
 brightify/monitors/m27q.py
 brightify/res/icon_dark.ico
 brightify/res/icon_light.ico
-brightify/scripts/windows/actions.py
-brightify/scripts/windows/add_startup_task.py
-brightify/scripts/windows/remove_startup_task.py
 brightify/sensor_firmware/platformio.ini
 brightify/sensor_firmware/src/main.cpp
 brightify/windows/WindowsApp.py
-brightify/windows/helpers.py
+brightify/windows/actions.py
+brightify/windows/add_startup_task.py
+brightify/windows/helpers.py
+brightify/windows/remove_startup_task.py
```

### Comparing `brightify-0.1.0/PKG-INFO` & `brightify-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 Metadata-Version: 2.1
 Name: Brightify
-Version: 0.1.0
-Summary: A tool to control the brightness of your screens.
+Version: 0.1.1
+Summary: The Brightify application allows users to adjust the brightness of their monitors.
 Author-email: "Robin S." <brightify@rs-web.net>
 Keywords: brightness,monitor,screen,control,tool
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: platformio
 Requires-Dist: pyserial
 Requires-Dist: libusb1
 Requires-Dist: PyQt6
 Requires-Dist: monitorcontrol
 Requires-Dist: pywin32; platform_system == "Windows"
 Requires-Dist: winshell; platform_system == "Windows"
 
-# Getting started
-
-1. Install brightify by running `pip install .` in the main directory. When developing, you can use `pip install -e .`
-   to install the package in editable mode.
+# Brightify
+This app allows you to set the brightness of your monitor(s). It is essentially a wrapper around the [DDC/CI](https://en.wikipedia.org/wiki/Display_Data_Channel#DDC/CI) protocol, which is supported by most monitors.
+It also supports adding custom communication protocols to control the brightness of USB monitors. For this, you most likely need to reverse engineer the communication protocol of the monitor. In my experience, this provides a more stable experience than using the DDC/CI protocol.
+You can find an example implementation for the [Gigabyte M27Q](https://www.gigabyte.com/Monitor/M27Q) in [here](brightify/monitors/m27q.py).
+The app is designed to be run in the background and can be controlled via a taskbar icon. It also supports a brightness sensor that can automatically adjust the brightness based on the ambient light.
+
+## Getting started
+1. Install brightify by running `pip install Brightify`. This package is regularly uploaded to PyPi. If you want to install the latest version, you can clone this repository from 
+[GitHub](https://github.com/RerikOp/Brightify) and install it with `pip install -e .` in the root directory.
 2. To start the app: `python -m brightify run`. You can exit either by right-clicking the icon in the taskbar and
    selecting "Exit" or by pressing `Ctrl+C` in the terminal.
-3. There are several other arguments you can pass to the app, see `python -m brightify --help` for more information.
-    1. To start the app at startup `python -m add startup` (Equivalent
-       to `python -m add startup --mode startup-folder`).
-       By default, the terminal will be hidden, but you can change
-       this by passing the `--force-console` argument.
-       To remove the startup task, run `python -m remove startup`. On Windows you can also use the Task Scheduler, which
-       requires elevated permissions to add the app to startup.
-       For this, run `python -m brightify add startup --mode task_scheduler` and to remove it `python -m brightify
-       remove startup --mode task_scheduler`.
-    2. To add a menu icon `python -m brightify add menu-icon`. Again, you can pass the `--force-console` argument
-       force the terminal.
-       To remove the icon, run `python -m remove menu-icon`.
-
-# Set up the brightness sensor
-
-1. Modify the [SensorComm](brightify/SensorComm.py) class to match your device and firmware
-2. Modify the code that is polling from the brightness sensor [Device Firmware](brightify/sensor_firmware/src)
-3. Modify [platformio.ini](brightify/sensor_firmware/platformio.ini) and enter your board (
+3. To start the app at startup (or logon) and add a menu icon, run `python -m add all`. To remove the both, run
+   `python -m remove all`.
+
+## Optional arguments
+There are several other arguments you can pass to the app, see `python -m brightify --help` for more information.
+- To target add/remove only the startup run `python -m brightify add/remove startup`.
+   - To add a task to the task scheduler on Windows, pass `--use-scheduler`. It will request elevated permissions.
+   - By default, the terminal will be hidden, but you can change this by passing the `--force-console` argument.
+- To add/remove only the menu icon run `python -m brightify add/remove menu-icon`.
+   - You can again force the console to be shown by passing the `--force-console` argument.
+
+## Set up the brightness sensor
+- Modify the [SensorComm](brightify/SensorComm.py) class to match your device and firmware
+- Modify the code that is polling from the brightness sensor [Device Firmware](brightify/sensor_firmware/src)
+- Modify [platformio.ini](brightify/sensor_firmware/platformio.ini) and enter your board (
    see [supported boards](https://docs.platformio.org/en/latest/boards/index.html))
-4. Run `pio run -t upload` in the terminal to upload the firmware to the board.
+- Run `pio run -t upload` in the terminal to upload the firmware to the board.
    If everything is working, the *Auto* Checkbox for each supported Monitor should now be clickable
 
-# Remarks
-
-+ Currently, only the Windows task bar icon is supported, the main part of this app is OS independent
-+ Feel free to create a pull request and add your own USB Monitor
+## Remarks
+- Currently, only the Windows task bar icon is supported, the main part of this app is OS independent.
+- Feel free to create a pull request and add your own USB Monitor
```

### Comparing `brightify-0.1.0/brightify/BaseApp.py` & `brightify-0.1.1/brightify/BaseApp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import threading
 from typing import List, Tuple, Type, Callable, Generator, Optional, Literal, Dict
 
 from PyQt6 import QtCore
 from PyQt6.QtCore import QPoint, Qt, QRect, QPropertyAnimation, QTimer, QThread
+from PyQt6.QtGui import QFocusEvent, QCursor, QRegion, QPainterPath
 from PyQt6.QtWidgets import QMainWindow, QWidget, QVBoxLayout
 
 from brightify import app_name, root_dir
 from brightify.SensorComm import SensorComm
 from brightify.UIConfig import UIConfig, Theme
 from brightify.UIConfig import MonitorRow
 
@@ -17,14 +18,18 @@
 from brightify.monitors.MonitorUSB import MonitorUSB
 
 # use global logger
 logger = logging.getLogger(app_name)
 
 
 def _supported_usb_impls() -> List[Type[MonitorUSB]]:
+    """
+    Finds all user implemented MonitorUSB classes in the monitors directory.
+    :return: a list of all MonitorUSB implementations
+    """
     import os, importlib, inspect
     monitor_impls = set()
     directory = "monitors"
     for filename in os.listdir(root_dir / directory):
         if not filename.endswith(".py"):
             continue
         module_name = filename.replace(".py", "")
@@ -36,28 +41,37 @@
                     monitor_impls.add(obj)
         except ImportError:
             pass
     return list(monitor_impls)
 
 
 def _usb_monitors(monitor_impls: List[Type[MonitorUSB]]) -> List[MonitorUSB]:
+    """
+    Finds all USB devices connected to the system and instantiates the corresponding MonitorUSB classes.
+    :param monitor_impls: a list of all MonitorUSB implementations
+    :return: a list of all MonitorUSB implementations with a connected USB device
+    """
     import usb1
     context = usb1.USBContext()
     devices = context.getDeviceList(skip_on_error=True)
     monitor_inst: List[Tuple[Type[MonitorUSB], usb1.USBDevice]] = []
     for dev in devices:
         for impl in monitor_impls:
             if impl.vid() == dev.getVendorID() and impl.pid() == dev.getProductID():
                 monitor_inst.append((impl, dev))
                 break
 
     return [impl(dev) for impl, dev in monitor_inst]
 
 
 def _ddcci_monitors() -> List[MonitorDDCCI]:
+    """
+    Finds all monitors connected to the system and instantiates the MonitorDDCCI class.
+    :return: a list of all MonitorDDCCI implementations
+    """
     import monitorcontrol
     monitors = monitorcontrol.get_monitors()
     return [MonitorDDCCI(monitor) for monitor in monitors]
 
 
 def get_supported_monitors() -> List[MonitorBase]:
     """
@@ -70,14 +84,18 @@
     logger.info(f"Found {len(usb_monitors)} USB monitor(s) with implementation: {[m.name() for m in usb_monitors]}")
     ddcci_monitors = _ddcci_monitors()
     logger.info(f"Found {len(ddcci_monitors)} DDCCI monitor(s)")
     return usb_monitors + ddcci_monitors
 
 
 class BaseApp(QMainWindow):
+    """
+    The main application window that contains all MonitorRows.
+    """
+
     def __init__(self, theme_cb: Callable[[], Theme], parent=None):
         super(BaseApp, self).__init__(parent, Qt.WindowType.Tool)
 
         # The rows contain one MonitorRow for each supported Monitor connected
         self.rows: QVBoxLayout = QVBoxLayout()
         self.central_widget = QWidget(self)
         self.central_widget.setLayout(self.rows)
@@ -95,17 +113,22 @@
         self.__sensor_comm.moveToThread(self.__sensor_thread)
 
         self.__sensor_timer = QTimer(self)
         self.__sensor_timer.timeout.connect(self.__sensor_comm.update_signal.emit)
         self.__sensor_timer.timeout.connect(self.update_ui_from_sensor)
 
         # Animations:
-        self.fade_animation = QPropertyAnimation(self, b"geometry")
-        self.fade_animation.finished.connect(lambda: self.__anim_lock.release())
-        self.fade_animation.finished.connect(self.activateWindow)
+        self.fade_up_animation = QPropertyAnimation(self, b"geometry")
+        self.fade_up_animation.finished.connect(self.__anim_lock.release)
+        self.fade_up_animation.finished.connect(self.activateWindow)
+        self.fade_up_animation.finished.connect(self.setFocus)
+
+        self.fade_down_animation = QPropertyAnimation(self, b"geometry")
+        self.fade_down_animation.finished.connect(self.__anim_lock.release)
+        self.fade_down_animation.finished.connect(self.clearFocus)
 
     @property
     def ui_config(self) -> UIConfig:
         return self.__ui_config
 
     def __config_layout(self):
         self.setWindowTitle(app_name)
@@ -209,57 +232,67 @@
             logger.debug("No theme update needed")
             return
         self.ui_config.theme = theme
         logger.debug(f"Theme updated to: {theme}")
 
     def redraw(self):
         logger.debug("Redrawing the app")
-        self.hide()
+        self.change_state("hide")
         self.__update_theme()
         self.__config_layout()
         self.setStyleSheet(self.ui_config.style_sheet)
         self.__load_rows()
         # The OS must set the top left corner, and invoke this function
         self.move(self.top_left)
         # start the sensor thread if it is not running
         if not self.__sensor_thread.isRunning():
             logger.debug("Starting sensor thread")
             self.__sensor_thread.start()
         # start the sensor timer if it is not running
         if not self.__sensor_timer.isActive():
             logger.debug("Starting sensor timer")
             self.__sensor_timer.start(250)
-        self.show()
+
+    # catch outside clicks, which should change the state of the window to hide
+    def focusOutEvent(self, event: QFocusEvent):
+        # get the position of the cursor and check if it is outside the window
+        if event.lostFocus():
+            if not self.geometry().contains(QCursor.pos()):
+                self.change_state("hide")
+                return
+
+        super().focusOutEvent(event)
 
     def change_state(self, new_state: Literal["show", "hide", "invert"] = "invert"):
         if self.top_left is None:
             logger.error("Top left corner not set")
             return
         # prevent multiple animations
         if self.__anim_lock.locked():
-            logger.debug("Animation already running")
             return
 
         # lock the animation
         self.__anim_lock.acquire()
         if new_state == "invert":
             new_state = "show" if self.geometry().topLeft() != self.top_left else "hide"
         # TODO verify that screen rotation does not affect the animation on darwin and linux
         up = QRect(self.top_left, QPoint(self.top_left.x() + self.minimumSizeHint().width(),
                                          self.top_left.y() + self.minimumSizeHint().height()))
 
         down = QRect(QPoint(self.top_left.x(), self.top_left.y() + self.minimumSizeHint().height()),
                      QPoint(self.top_left.x() + self.minimumSizeHint().width(),
                             self.top_left.y() + 2 * self.height()))
-
+        # make visible before animating
+        self.show()
         if new_state == "show":
             logger.debug(f"Showing window")
-            self.show()
-            self.ui_config.config_fade_animation(self.fade_animation, down, up)
-            self.fade_animation.start()
+            self.ui_config.config_fade_animation(self.fade_up_animation, down, up)
+            self.fade_up_animation.start()
         else:
             logger.debug(f"Hiding window")
-            self.ui_config.config_fade_animation(self.fade_animation, up, down)
-            self.fade_animation.start()
+            self.ui_config.config_fade_animation(self.fade_down_animation, up, down)
+            self.fade_down_animation.start()
+
+        self.updateGeometry()
 
     def show(self):
         super().show()
```

### Comparing `brightify-0.1.0/brightify/Brightylog.py` & `brightify-0.1.1/brightify/Brightylog.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.0/brightify/SensorComm.py` & `brightify-0.1.1/brightify/SensorComm.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.0/brightify/UIConfig.py` & `brightify-0.1.1/brightify/UIConfig.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from PyQt6 import QtCore
 from PyQt6.QtCore import QPropertyAnimation, QEasingCurve
 from PyQt6.QtGui import QFont, QFontMetrics
 
 from PyQt6.QtWidgets import QWidget, QSlider, QCheckBox, QLabel, QHBoxLayout
 
-from brightify import root_dir
+from brightify import icon_light, icon_dark
 from brightify.monitors.MonitorBase import MonitorBase
 from brightify.monitors.MonitorUSB import MonitorUSB
 from brightify.monitors.MonitorDDCCI import MonitorDDCCI
 
 
 @dataclasses.dataclass
 class Theme:
@@ -44,16 +44,14 @@
         # Set properties
         self.slider.setRange(0, 100)
         self.slider.setStyleSheet(self.__slider_style(theme))
         self.is_auto_tick.setStyleSheet(self.__checkbox_style(theme))
 
         # the brightness label should be 4 characters wide (including the % sign)
         self.brightness_label.setFixedWidth(QFontMetrics(self.font).horizontalAdvance("100%"))
-        # The type label should support the longest type name (DDCCI) + brackets + al little padding
-        #self.type_label.setFixedWidth(QFontMetrics(self.font).horizontalAdvance("[DDCCI]"))
 
         # Create layout and add components
         layout = QHBoxLayout()
         layout.addWidget(self.type_label)
         layout.addWidget(self.name_label)
         layout.addWidget(self.slider)
         layout.addWidget(self.brightness_label)
@@ -116,24 +114,21 @@
     pad_horizontal: int = 5
     pad_vertical: int = 25
 
     # The maximum width of the label in the MonitorRow, or -1 if unbounded
     max_label_width: int = -1
 
     # Icon
-    _icon_path: Path = dataclasses.field(default=root_dir / "res" / "icon_light.ico")
+    _icon_path: Path = dataclasses.field(default=icon_light)
 
     animation_duration: int = 100
 
     @property
     def icon_path(self):
-        if self.theme.mode == "dark":
-            return root_dir / "res" / "icon_light.ico"
-        if self.theme.mode == "light":
-            return root_dir / "res" / "icon_dark.ico"
+        return icon_light if self.theme.mode == "dark" else icon_dark
 
     @property
     def style_sheet(self):
         return f"""
             background-color: {self.theme.bg_color};
             color: {self.theme.text_color};
         """
```

### Comparing `brightify-0.1.0/brightify/log_config.toml` & `brightify-0.1.1/brightify/log_config.toml`

 * *Files identical despite different names*

### Comparing `brightify-0.1.0/brightify/monitors/MonitorBase.py` & `brightify-0.1.1/brightify/monitors/MonitorBase.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.0/brightify/monitors/MonitorDDCCI.py` & `brightify-0.1.1/brightify/monitors/MonitorDDCCI.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.0/brightify/monitors/MonitorGeneric.py` & `brightify-0.1.1/brightify/monitors/MonitorGeneric.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.0/brightify/monitors/MonitorUSB.py` & `brightify-0.1.1/brightify/monitors/MonitorUSB.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.0/brightify/monitors/m27q.py` & `brightify-0.1.1/brightify/monitors/m27q.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.0/brightify/res/icon_dark.ico` & `brightify-0.1.1/brightify/res/icon_dark.ico`

 * *Files identical despite different names*

### Comparing `brightify-0.1.0/brightify/res/icon_light.ico` & `brightify-0.1.1/brightify/res/icon_light.ico`

 * *Files identical despite different names*

### Comparing `brightify-0.1.0/brightify/windows/WindowsApp.py` & `brightify-0.1.1/brightify/windows/WindowsApp.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         self.base_app.top_left = QPoint(x, y)
 
     def _on_restart(self, hwnd=None, msg=None, wparam=None, lparam=None):
         logger.debug("Taskbar restarted")
         self._update_top_left()
         self.base_app.redraw()
         self._create_icon()
-        self.base_app.hide()
+        self.base_app.change_state("hide")
         return 0
 
     def _on_command(self, hwnd=None, msg=None, wparam=None, lparam=None):
         cmd = win32api.LOWORD(wparam)
         if cmd in self.cmd_id_map:
             # invoke corresponding function
             self.cmd_id_map[cmd]()
```

### Comparing `brightify-0.1.0/brightify/windows/helpers.py` & `brightify-0.1.1/brightify/windows/helpers.py`

 * *Files identical despite different names*

