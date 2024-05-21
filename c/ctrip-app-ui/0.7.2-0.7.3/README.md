# Comparing `tmp/ctrip-app-ui-0.7.2.tar.gz` & `tmp/ctrip-app-ui-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.7.2.tar", last modified: Mon May 20 12:10:55 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.7.3.tar", last modified: Tue May 21 06:19:08 2024, max compression
```

## Comparing `ctrip-app-ui-0.7.2.tar` & `ctrip-app-ui-0.7.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 12:10:55.550836 ctrip-app-ui-0.7.2/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.7.2/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-20 12:10:55.549839 ctrip-app-ui-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.7.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 12:10:55.537885 ctrip-app-ui-0.7.2/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.7.2/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.7.2/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.7.2/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.7.2/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.7.2/capp_ui/dir.py
--rw-rw-rw-   0        0        0    55970 2024-05-20 12:05:57.000000 ctrip-app-ui-0.7.2/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.7.2/capp_ui/fee.py
--rw-rw-rw-   0        0        0     5414 2024-05-20 12:10:40.000000 ctrip-app-ui-0.7.2/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.7.2/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.7.2/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.7.2/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.7.2/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.7.2/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-20 12:10:55.548841 ctrip-app-ui-0.7.2/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-20 12:10:55.000000 ctrip-app-ui-0.7.2/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-20 12:10:55.000000 ctrip-app-ui-0.7.2/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 12:10:55.000000 ctrip-app-ui-0.7.2/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-20 12:10:55.000000 ctrip-app-ui-0.7.2/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-20 12:10:55.000000 ctrip-app-ui-0.7.2/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 12:10:55.550836 ctrip-app-ui-0.7.2/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-20 12:10:50.000000 ctrip-app-ui-0.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:19:08.941503 ctrip-app-ui-0.7.3/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.7.3/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-21 06:19:08.940505 ctrip-app-ui-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.7.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 06:19:08.930532 ctrip-app-ui-0.7.3/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.7.3/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.7.3/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.7.3/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.7.3/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.7.3/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    56041 2024-05-21 06:18:09.000000 ctrip-app-ui-0.7.3/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.7.3/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5414 2024-05-20 12:10:40.000000 ctrip-app-ui-0.7.3/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.7.3/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.7.3/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.7.3/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.7.3/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.7.3/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:19:08.939508 ctrip-app-ui-0.7.3/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-21 06:19:08.000000 ctrip-app-ui-0.7.3/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-21 06:19:08.000000 ctrip-app-ui-0.7.3/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 06:19:08.000000 ctrip-app-ui-0.7.3/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-21 06:19:08.000000 ctrip-app-ui-0.7.3/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-21 06:19:08.000000 ctrip-app-ui-0.7.3/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 06:19:08.942500 ctrip-app-ui-0.7.3/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-21 06:19:03.000000 ctrip-app-ui-0.7.3/setup.py
```

### Comparing `ctrip-app-ui-0.7.2/LICENSE` & `ctrip-app-ui-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.2/capp_ui/config.py` & `ctrip-app-ui-0.7.3/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.2/capp_ui/date_extend.py` & `ctrip-app-ui-0.7.3/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.2/capp_ui/device.py` & `ctrip-app-ui-0.7.3/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.2/capp_ui/dir.py` & `ctrip-app-ui-0.7.3/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.2/capp_ui/domain_service.py` & `ctrip-app-ui-0.7.3/capp_ui/domain_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,17 @@
         time.sleep(1.0)
         poco_poxy = PocoProxy()
         self.device.poco = poco_poxy.poco
         self.device.get_po = poco_poxy.get_po
         self.device.get_po_extend = poco_poxy.get_po_extend
 
     def stop(self) -> None:
+        del self.device.poco
+        import gc
+        gc.collect()
         stop_app(self.app_name, device_id=self.device.device_id)
 
     def restart(self) -> bool:
         try:
             stop_app(self.app_name, device_id=self.device.device_id)
             time.sleep(1.0)
             self.device.start_app(self.app_name)
```

### Comparing `ctrip-app-ui-0.7.2/capp_ui/fee.py` & `ctrip-app-ui-0.7.3/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.2/capp_ui/libs.py` & `ctrip-app-ui-0.7.3/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.2/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.7.3/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.2/capp_ui/platforms.py` & `ctrip-app-ui-0.7.3/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.2/capp_ui/test.py` & `ctrip-app-ui-0.7.3/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.2/capp_ui/utils.py` & `ctrip-app-ui-0.7.3/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.2/capp_ui/validators.py` & `ctrip-app-ui-0.7.3/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.2/setup.py` & `ctrip-app-ui-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.7.2',
+    version='0.7.3',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

