# Comparing `tmp/ixontray-0.2.8.tar.gz` & `tmp/ixontray-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixontray-0.2.8.tar", last modified: Mon Nov 27 20:33:07 2023, max compression
+gzip compressed data, was "ixontray-0.3.0.tar", last modified: Tue May 21 06:31:02 2024, max compression
```

## Comparing `ixontray-0.2.8.tar` & `ixontray-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,28 @@
--rw-r--r--   0        0        0     1224 2023-11-27 20:32:08.446262 ixontray-0.2.8/README.md
--rw-r--r--   0        0        0     2405 2023-11-27 20:33:07.902436 ixontray-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       22 2023-11-27 20:33:02.306419 ixontray-0.2.8/src/ixontray/__init__.py
--rw-r--r--   0        0        0     2881 2023-11-03 06:14:26.363830 ixontray-0.2.8/src/ixontray/base_model_store.py
--rw-r--r--   0        0        0     1024 2023-08-31 08:03:34.827347 ixontray-0.2.8/src/ixontray/commands-windows.yaml
--rw-r--r--   0        0        0     1562 2023-11-06 14:21:03.555473 ixontray-0.2.8/src/ixontray/commands.yaml
--rw-r--r--   0        0        0      579 2023-09-05 07:42:07.591353 ixontray-0.2.8/src/ixontray/config.py
--rw-r--r--   0        0        0    18724 2023-08-31 08:03:34.827347 ixontray-0.2.8/src/ixontray/icon.png
--rw-r--r--   0        0        0     3425 2023-08-31 08:03:34.827347 ixontray-0.2.8/src/ixontray/icon_not_connected.png
--rw-r--r--   0        0        0      227 2023-08-31 08:03:34.827347 ixontray-0.2.8/src/ixontray/install.sh
--rw-r--r--   0        0        0     5299 2023-11-01 19:04:15.013687 ixontray-0.2.8/src/ixontray/ixon_cloud_api.py
--rwxr-xr-x   0        0        0    24211 2023-11-27 20:27:05.337379 ixontray-0.2.8/src/ixontray/ixon_tray.py
--rw-r--r--   0        0        0     3497 2023-09-05 07:42:07.603353 ixontray-0.2.8/src/ixontray/ixon_vpn_client_api.py
--rw-r--r--   0        0        0     7340 2023-11-27 20:22:01.740494 ixontray-0.2.8/src/ixontray/launcher.py
--rw-r--r--   0        0        0    16563 2023-11-27 20:20:26.520216 ixontray-0.2.8/src/ixontray/settings_window.py
--rw-r--r--   0        0        0     5194 2023-11-27 19:49:24.434788 ixontray-0.2.8/src/ixontray/telemetry.py
--rw-r--r--   0        0        0      352 2023-08-31 08:03:34.831347 ixontray-0.2.8/src/ixontray/types/__init__.py
--rw-r--r--   0        0        0     2549 2023-09-05 07:42:07.603353 ixontray-0.2.8/src/ixontray/types/api.py
--rw-r--r--   0        0        0     1216 2023-08-31 19:07:34.470186 ixontray-0.2.8/src/ixontray/types/common.py
--rw-r--r--   0        0        0      863 2023-11-01 20:59:06.205905 ixontray-0.2.8/src/ixontray/update.py
--rw-r--r--   0        0        0       37 2023-04-16 19:25:38.117726 ixontray-0.2.8/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-04-16 19:25:38.117726 ixontray-0.2.8/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2023-04-16 19:25:38.117726 ixontray-0.2.8/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0       35 2023-11-27 19:45:30.802107 ixontray-0.2.8/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1411 2023-11-27 19:50:16.386939 ixontray-0.2.8/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-11-27 19:50:16.386939 ixontray-0.2.8/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      352 2023-08-31 08:03:34.831347 ixontray-0.2.8/tests/__init__.py
--rw-r--r--   0        0        0      562 2023-08-31 08:03:34.831347 ixontray-0.2.8/tests/conftest.py
--rw-r--r--   0        0        0     3467 2023-08-31 08:03:34.831347 ixontray-0.2.8/tests/test_basemodel_store.py
--rw-r--r--   0        0        0     1320 2023-09-05 07:42:07.603353 ixontray-0.2.8/tests/test_ixon_cloud_api_v1.py
--rw-r--r--   0        0        0     1441 2023-09-05 07:42:07.603353 ixontray-0.2.8/tests/test_ixon_cloud_api_v2.py
--rw-r--r--   0        0        0     1623 2023-08-31 08:03:34.831347 ixontray-0.2.8/tests/test_ixon_vpn_api.py
--rw-r--r--   0        0        0     1247 2023-11-27 19:51:26.055142 ixontray-0.2.8/tests/test_telemetry.py
--rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 ixontray-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1273 2024-01-12 19:04:27.438207 ixontray-0.3.0/README.md
+-rw-r--r--   0        0        0     2405 2024-05-21 06:31:02.350226 ixontray-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-21 06:24:02.838938 ixontray-0.3.0/src/ixontray/__init__.py
+-rw-r--r--   0        0        0     2881 2023-11-03 06:14:26.000000 ixontray-0.3.0/src/ixontray/base_model_store.py
+-rw-r--r--   0        0        0     1024 2023-08-31 08:03:34.000000 ixontray-0.3.0/src/ixontray/commands-windows.yaml
+-rw-r--r--   0        0        0     1562 2023-11-06 14:21:03.000000 ixontray-0.3.0/src/ixontray/commands.yaml
+-rw-r--r--   0        0        0      579 2023-09-05 07:42:07.000000 ixontray-0.3.0/src/ixontray/config.py
+-rw-r--r--   0        0        0    18724 2023-08-31 08:03:34.000000 ixontray-0.3.0/src/ixontray/icon.png
+-rw-r--r--   0        0        0     3425 2023-08-31 08:03:34.000000 ixontray-0.3.0/src/ixontray/icon_not_connected.png
+-rw-r--r--   0        0        0      227 2023-08-31 08:03:34.000000 ixontray-0.3.0/src/ixontray/install.sh
+-rw-r--r--   0        0        0     5299 2023-11-01 19:04:15.000000 ixontray-0.3.0/src/ixontray/ixon_cloud_api.py
+-rwxr-xr-x   0        0        0    24495 2024-05-21 06:23:07.359037 ixontray-0.3.0/src/ixontray/ixon_tray.py
+-rw-r--r--   0        0        0     3497 2023-09-05 07:42:07.000000 ixontray-0.3.0/src/ixontray/ixon_vpn_client_api.py
+-rw-r--r--   0        0        0     7340 2023-11-27 20:22:01.000000 ixontray-0.3.0/src/ixontray/launcher.py
+-rw-r--r--   0        0        0    16738 2024-05-21 06:23:07.247038 ixontray-0.3.0/src/ixontray/settings_window.py
+-rw-r--r--   0        0        0     5194 2023-11-27 19:49:24.000000 ixontray-0.3.0/src/ixontray/telemetry.py
+-rw-r--r--   0        0        0      352 2023-08-31 08:03:34.000000 ixontray-0.3.0/src/ixontray/types/__init__.py
+-rw-r--r--   0        0        0     2549 2023-09-05 07:42:07.000000 ixontray-0.3.0/src/ixontray/types/api.py
+-rw-r--r--   0        0        0     1216 2023-08-31 19:07:34.000000 ixontray-0.3.0/src/ixontray/types/common.py
+-rw-r--r--   0        0        0      863 2023-11-01 20:59:06.000000 ixontray-0.3.0/src/ixontray/update.py
+-rw-r--r--   0        0        0      352 2024-01-12 16:09:11.201816 ixontray-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      562 2024-01-12 16:09:11.201816 ixontray-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     3467 2024-01-12 16:09:11.201816 ixontray-0.3.0/tests/test_basemodel_store.py
+-rw-r--r--   0        0        0     1320 2024-01-12 16:09:11.201816 ixontray-0.3.0/tests/test_ixon_cloud_api_v1.py
+-rw-r--r--   0        0        0     1441 2024-01-12 16:09:11.201816 ixontray-0.3.0/tests/test_ixon_cloud_api_v2.py
+-rw-r--r--   0        0        0     1623 2024-01-12 16:09:11.201816 ixontray-0.3.0/tests/test_ixon_vpn_api.py
+-rw-r--r--   0        0        0     1247 2024-01-12 19:04:27.450207 ixontray-0.3.0/tests/test_telemetry.py
+-rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 ixontray-0.3.0/PKG-INFO
```

### Comparing `ixontray-0.2.8/README.md` & `ixontray-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,48 @@
-# Ixontray
+== Ixontray
 Small utility to connect quickly to a given ixon system.
 
-## Installation
+== Installation
 To install the application run:
 
-### Ubuntu 22.04
-
-```bash
+=== Ubuntu 22.04
+[source, bash]
+----
 sudo apt-get -qq install libegl1 libxcb-cursor0 libxcb-icccm4 libxcb-image0 libxcb-keysyms1 libxcb-randr0 libxcb-render-util0 libxcb-shape0 libxkbcommon-x11-0
 pipx install ixontray
-```
+----
 
 
-### Ubuntu 20.04
-```bash
+=== Ubuntu 20.04
+[source, bash]
+----
 sudo apt install software-properties-common -y
 sudo add-apt-repository ppa:deadsnakes/ppa
 sudo apt install python3.10
 pipx install ixontray --python <path-to-python3.10>  #in my case: /usr/bin/python3.10
 sudo apt-get -qq install libegl1 libxcb-cursor0 libxcb-icccm4 libxcb-image0 libxcb-keysyms1 libxcb-randr0 libxcb-render-util0 libxcb-shape0 libxkbcommon-x11-0
-```
+----
+
 You can run the application:
 
 
 
-```bash
+[source, bash]
+----
 ixontray
-```
+----
 
 Or run the laucher
 
-```bash
+[source, bash]
+----
 ixontray --launcher
-```
-
+----
 TIP:: Best to add that to a system wide shortcut. I have it at `WIN+X` ( System Settings > Keyboard > Keyboard Shortcuts > Custom Shortcuts > Add a new one )
 
 INFO:: The first time you will need to enter your login credentials in the window that will open.
 
 NOTE:: You need to run the application first before you can run the launcher.
 
 A tray icon like this will appear:
 
-![tray.png](tray.png)
+image::tray.png[]
```

### Comparing `ixontray-0.2.8/pyproject.toml` & `ixontray-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -159,14 +159,14 @@
     "packaging>=23.2",
 ]
 requires-python = ">=3.10"
 keywords = [
     "tool",
     "ixon",
 ]
-version = "0.2.8"
+version = "0.3.0"
 
 [project.license]
 text = "BSD"
 
 [project.scripts]
 ixontray = "ixontray.ixon_tray:main"
```

### Comparing `ixontray-0.2.8/src/ixontray/base_model_store.py` & `ixontray-0.3.0/src/ixontray/base_model_store.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/src/ixontray/commands-windows.yaml` & `ixontray-0.3.0/src/ixontray/commands-windows.yaml`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/src/ixontray/commands.yaml` & `ixontray-0.3.0/src/ixontray/commands.yaml`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/src/ixontray/config.py` & `ixontray-0.3.0/src/ixontray/config.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/src/ixontray/icon.png` & `ixontray-0.3.0/src/ixontray/icon.png`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/src/ixontray/icon_not_connected.png` & `ixontray-0.3.0/src/ixontray/icon_not_connected.png`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/src/ixontray/ixon_cloud_api.py` & `ixontray-0.3.0/src/ixontray/ixon_cloud_api.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/src/ixontray/ixon_tray.py` & `ixontray-0.3.0/src/ixontray/ixon_tray.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 from typing import Any
 
 import requests
 import urllib3
 from PyQt6 import QtCore, QtGui
 from PyQt6.QtCore import QEvent, QThread, QTimer
 from PyQt6.QtGui import QAction, QCloseEvent, QIcon
-from PyQt6.QtWidgets import QApplication, QMenu, QMessageBox, QSystemTrayIcon
+from PyQt6.QtWidgets import (
+    QApplication,
+    QInputDialog,
+    QMenu,
+    QMessageBox,
+    QSystemTrayIcon,
+)
 
 import ixontray
 from ixontray.base_model_store import BaseModelStore
 from ixontray.config import (
     AGENTS_FILE_PATH,
     COMMAND_FILE_NAME,
     COMMAND_FILE_PATH,
@@ -182,17 +188,22 @@
         self._commands = self._command_store.load()
         self.setup_menu()
 
     def _has_login_details(self) -> bool:
         """Check if login details are there."""
         return all(self._settings_window.general_tab.get_auth())
 
-    def get_auth_string(self, otp: str = "") -> str:
+    def get_auth_string(self, otp: str | None = None) -> str:
         email, password = self._settings_window.general_tab.get_auth()
 
+        if otp is None and self._settings_window.general_tab.ch_2fa.isChecked():
+            otp, ok = QInputDialog.getText(self._settings_window, "OTP required", "Enter OTP")
+            if not ok:
+                otp = ""
+
         if not email or not password:
             logger.error("No login details found please supply them")
             self.show_login_credentials()
             return ""
 
         return IxonCloudAPIv1.generate_auth(email=email, pwd=password, otp=otp)
 
@@ -282,15 +293,15 @@
 
         # Update agents every 10m seconds
         self.update_agents()
         self._update_agents_timer.timeout.connect(self.update_agents)
         self._update_agents_timer.start(1000 * 60 * 5)
         self._update_agents_timer.moveToThread(self._worker_thread)
 
-        if not self.get_auth_string():
+        if not self.get_auth_string(otp="Dummy"):
             logger.info("Please provide login credentials")
 
         logger.info("Started application, use tray icon to interact")
         telemetry.send()
 
     def load_favourite_ixon_ids(self) -> None:
         self._settings.beginGroup("favourite_clients")
```

### Comparing `ixontray-0.2.8/src/ixontray/ixon_vpn_client_api.py` & `ixontray-0.3.0/src/ixontray/ixon_vpn_client_api.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/src/ixontray/launcher.py` & `ixontray-0.3.0/src/ixontray/launcher.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/src/ixontray/settings_window.py` & `ixontray-0.3.0/src/ixontray/settings_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,19 @@
         self.le_organization_id = QLineEdit()
 
         username, password = self.get_auth()
         self.le_email = QLineEdit(username)
         self.le_password = QLineEdit(password)
         self.le_password.setEchoMode(QLineEdit.EchoMode.Password)
 
+        otp_required = self._settings.value("otp", False)
         self.ch_2fa = QCheckBox()
+
+        self.ch_2fa.setChecked(bool(otp_required))
+
         self.btn_save = QPushButton("Save")
         self.btn_save.clicked.connect(self.save_auth)
 
         self._layout = QFormLayout()
         self._layout.addRow("Auto start application", self.cb_enable_autostart)
         # self._layout.addRow("Organization ID", self.le_organization_id)
         # self._layout.addRow("Application ID", self.le_application_id)
@@ -67,14 +71,15 @@
 
     def save_auth(self) -> None:
         """Store user name and password."""
         logging.info("Saved the login details.")
         username = self.le_email.text()
         password = self.le_password.text()
         self._settings.setValue("email", username)
+        self._settings.setValue("otp", self.ch_2fa.isChecked())
         keyring.set_password("Ixontray", username, password)
         self.save_btn_clicked.emit()
 
     def get_auth(self) -> tuple[str, str]:
         """Returns user name and password."""
         username = self._settings.value("email", "")
         password = keyring.get_password("Ixontray", username)
```

### Comparing `ixontray-0.2.8/src/ixontray/telemetry.py` & `ixontray-0.3.0/src/ixontray/telemetry.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/src/ixontray/types/api.py` & `ixontray-0.3.0/src/ixontray/types/api.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/src/ixontray/types/common.py` & `ixontray-0.3.0/src/ixontray/types/common.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/src/ixontray/update.py` & `ixontray-0.3.0/src/ixontray/update.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/tests/conftest.py` & `ixontray-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/tests/test_basemodel_store.py` & `ixontray-0.3.0/tests/test_basemodel_store.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/tests/test_ixon_cloud_api_v1.py` & `ixontray-0.3.0/tests/test_ixon_cloud_api_v1.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/tests/test_ixon_cloud_api_v2.py` & `ixontray-0.3.0/tests/test_ixon_cloud_api_v2.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/tests/test_ixon_vpn_api.py` & `ixontray-0.3.0/tests/test_ixon_vpn_api.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/tests/test_telemetry.py` & `ixontray-0.3.0/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `ixontray-0.2.8/PKG-INFO` & `ixontray-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 Metadata-Version: 2.1
 Name: ixontray
-Version: 0.2.8
+Version: 0.3.0
 Summary: A tray application and launcher to connect to remote systems using IXON
-Keywords: tool ixon
+Keywords: tool,ixon
 Author-Email: Mart Moerdijk <mart@mmoerdijk.nl>
 License: BSD
 Requires-Python: >=3.10
 Requires-Dist: PyQt6
 Requires-Dist: pydantic
 Requires-Dist: icecream
 Requires-Dist: requests
 Requires-Dist: ruamel.yaml
 Requires-Dist: keyring
 Requires-Dist: pypi-json>=0.4.0
 Requires-Dist: packaging>=23.2
 Description-Content-Type: text/markdown
 
-# Ixontray
+== Ixontray
 Small utility to connect quickly to a given ixon system.
 
-## Installation
+== Installation
 To install the application run:
 
-### Ubuntu 22.04
-
-```bash
+=== Ubuntu 22.04
+[source, bash]
+----
 sudo apt-get -qq install libegl1 libxcb-cursor0 libxcb-icccm4 libxcb-image0 libxcb-keysyms1 libxcb-randr0 libxcb-render-util0 libxcb-shape0 libxkbcommon-x11-0
 pipx install ixontray
-```
+----
 
 
-### Ubuntu 20.04
-```bash
+=== Ubuntu 20.04
+[source, bash]
+----
 sudo apt install software-properties-common -y
 sudo add-apt-repository ppa:deadsnakes/ppa
 sudo apt install python3.10
 pipx install ixontray --python <path-to-python3.10>  #in my case: /usr/bin/python3.10
 sudo apt-get -qq install libegl1 libxcb-cursor0 libxcb-icccm4 libxcb-image0 libxcb-keysyms1 libxcb-randr0 libxcb-render-util0 libxcb-shape0 libxkbcommon-x11-0
-```
+----
+
 You can run the application:
 
 
 
-```bash
+[source, bash]
+----
 ixontray
-```
+----
 
 Or run the laucher
 
-```bash
+[source, bash]
+----
 ixontray --launcher
-```
-
+----
 TIP:: Best to add that to a system wide shortcut. I have it at `WIN+X` ( System Settings > Keyboard > Keyboard Shortcuts > Custom Shortcuts > Add a new one )
 
 INFO:: The first time you will need to enter your login credentials in the window that will open.
 
 NOTE:: You need to run the application first before you can run the launcher.
 
 A tray icon like this will appear:
 
-![tray.png](tray.png)
+image::tray.png[]
```

