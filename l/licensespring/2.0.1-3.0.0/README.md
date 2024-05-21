# Comparing `tmp/licensespring-2.0.1.tar.gz` & `tmp/licensespring-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "licensespring-2.0.1.tar", max compression
+gzip compressed data, was "licensespring-3.0.0.tar", max compression
```

## Comparing `licensespring-2.0.1.tar` & `licensespring-3.0.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0       64 2023-12-29 10:00:28.397852 licensespring-2.0.1/LICENSE
--rw-r--r--   0        0        0    23192 2024-04-24 06:32:12.240855 licensespring-2.0.1/README.md
--rw-r--r--   0        0        0       37 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/__init__.py
--rw-r--r--   0        0        0    23871 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/api/__init__.py
--rw-r--r--   0        0        0     1146 2024-03-22 07:52:05.771346 licensespring-2.0.1/licensespring/api/authorization.py
--rw-r--r--   0        0        0      551 2024-03-22 07:52:05.771346 licensespring-2.0.1/licensespring/api/error.py
--rw-r--r--   0        0        0     1804 2024-03-22 07:52:05.771346 licensespring-2.0.1/licensespring/api/signature.py
--rw-r--r--   0        0        0     2281 2024-03-22 07:52:05.771346 licensespring-2.0.1/licensespring/hardware/__init__.py
--rw-r--r--   0        0        0    24041 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/licensefile/__init__.py
--rw-r--r--   0        0        0     2507 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/licensefile/config.py
--rw-r--r--   0        0        0     5206 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/licensefile/data_storage.py
--rw-r--r--   0        0        0     1984 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/licensefile/default_crypto.py
--rw-r--r--   0        0        0     2612 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/licensefile/error.py
--rw-r--r--   0        0        0     7856 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/licensefile/feature_manager.py
--rw-r--r--   0        0        0    14587 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/licensefile/license_data.py
--rw-r--r--   0        0        0     6729 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/licensefile/license_manager.py
--rw-r--r--   0        0        0     7450 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/watchdog/__init__.py
--rw-r--r--   0        0        0      342 2024-01-04 12:24:20.611987 licensespring-2.0.1/licensespring/webhook/__init__.py
--rw-r--r--   0        0        0      300 2023-12-29 10:00:28.397852 licensespring-2.0.1/licensespring/webhook/error.py
--rw-r--r--   0        0        0     2086 2024-03-22 07:52:05.781346 licensespring-2.0.1/licensespring/webhook/signature.py
--rw-r--r--   0        0        0      980 2023-12-29 10:00:28.397852 licensespring-2.0.1/licensespring/webhook/utils.py
--rw-r--r--   0        0        0      687 2024-04-24 06:32:12.240855 licensespring-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    24025 1970-01-01 00:00:00.000000 licensespring-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-12-29 10:00:28.397852 licensespring-3.0.0/LICENSE
+-rw-r--r--   0        0        0    30355 2024-05-21 09:09:00.045223 licensespring-3.0.0/README.md
+-rw-r--r--   0        0        0       37 2024-05-21 09:09:00.045223 licensespring-3.0.0/licensespring/__init__.py
+-rw-r--r--   0        0        0    24501 2024-05-21 09:09:00.045223 licensespring-3.0.0/licensespring/api/__init__.py
+-rw-r--r--   0        0        0     1146 2024-03-22 07:52:05.771346 licensespring-3.0.0/licensespring/api/authorization.py
+-rw-r--r--   0        0        0      551 2024-03-22 07:52:05.771346 licensespring-3.0.0/licensespring/api/error.py
+-rw-r--r--   0        0        0     1804 2024-03-22 07:52:05.771346 licensespring-3.0.0/licensespring/api/signature.py
+-rw-r--r--   0        0        0     2281 2024-03-22 07:52:05.771346 licensespring-3.0.0/licensespring/hardware/__init__.py
+-rw-r--r--   0        0        0    27454 2024-05-21 09:09:00.045223 licensespring-3.0.0/licensespring/licensefile/__init__.py
+-rw-r--r--   0        0        0     2702 2024-05-21 09:09:00.045223 licensespring-3.0.0/licensespring/licensefile/config.py
+-rw-r--r--   0        0        0    10497 2024-05-21 09:09:00.045223 licensespring-3.0.0/licensespring/licensefile/data_storage.py
+-rw-r--r--   0        0        0     1984 2024-05-03 06:03:02.615945 licensespring-3.0.0/licensespring/licensefile/default_crypto.py
+-rw-r--r--   0        0        0     2835 2024-05-21 09:09:00.045223 licensespring-3.0.0/licensespring/licensefile/error.py
+-rw-r--r--   0        0        0     7856 2024-05-03 06:02:57.925946 licensespring-3.0.0/licensespring/licensefile/feature_manager.py
+-rw-r--r--   0        0        0    15314 2024-05-21 09:09:00.045223 licensespring-3.0.0/licensespring/licensefile/license_data.py
+-rw-r--r--   0        0        0    10940 2024-05-21 09:09:00.045223 licensespring-3.0.0/licensespring/licensefile/license_manager.py
+-rw-r--r--   0        0        0     1654 2024-05-21 09:09:00.045223 licensespring-3.0.0/licensespring/licensefile/offline_activation_guard.py
+-rw-r--r--   0        0        0     7450 2024-05-03 06:03:02.615945 licensespring-3.0.0/licensespring/watchdog/__init__.py
+-rw-r--r--   0        0        0      342 2024-01-04 12:24:20.611987 licensespring-3.0.0/licensespring/webhook/__init__.py
+-rw-r--r--   0        0        0      300 2023-12-29 10:00:28.397852 licensespring-3.0.0/licensespring/webhook/error.py
+-rw-r--r--   0        0        0     2086 2024-03-22 07:52:05.781346 licensespring-3.0.0/licensespring/webhook/signature.py
+-rw-r--r--   0        0        0      980 2023-12-29 10:00:28.397852 licensespring-3.0.0/licensespring/webhook/utils.py
+-rw-r--r--   0        0        0      687 2024-05-21 09:09:00.045223 licensespring-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    31188 1970-01-01 00:00:00.000000 licensespring-3.0.0/PKG-INFO
```

### Comparing `licensespring-2.0.1/README.md` & `licensespring-3.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -152,18 +152,17 @@
 api_client.deactivate_license(product=product, license_key=license_key)
 ```
 
 ### Deactivate user based license
 ```python
 product = "uprod1"
 username = "user1@email.com"
-password = "nq64k1!@"
 
 api_client.deactivate_license(
-    product=product, username=username, password=password
+    product=product, username=username
 )
 ```
 
 ### Check key based license
 ```python
 product = "lkprod1"
 license_key = "GPBQ-DZCP-E9SK-CQLK"
@@ -405,14 +404,26 @@
     ls_activation_data = file.read()
 
 license_data = api_client.activate_offline_load(ls_activation_data)
 
 print(license_data)
 ```
 
+### Check offline load
+```python
+# Read from file
+with open('./license_refresh.lic') as file:
+    license_refresh_data = file.read()
+
+license_data = api_client.check_offline_load(license_refresh_data)
+
+print(license_data)
+```
+
+
 ### Deactivate offline
 ```python
 product = "lkprod1"
 license_key = "GPYC-X5J2-L5SK-C3LK"
 
 # Generate data for offline deactivation
 deactivate_offline_data = api_client.deactivate_offline_dump(
@@ -521,15 +532,15 @@
 manager = LicenseManager(conf)
 ```
 #### Configuration parametres
 
 conf (Configuration): **[A configuration object](#configuration-setup)**
 
 #### activate_license
-Activates a license with the license server and updates local license data.Returns an instance of the License
+Activates a license with the license server and updates local license data.
 
 **Key-based**
 ```python
 manager = LicenseManager(conf)
 
 license_id = LicenseID.from_key("H6QM-6H5R-ZENJ-VBLK")
 
@@ -539,14 +550,20 @@
 ```python
 manager = LicenseManager(conf)
 
 license_id = LicenseID.from_user(username="python@gmail.com",password="7t_x3!o9")
 
 license = manager.activate_license(license_id)
 ```
+**Parameters**:  
+* **license_id** (LicenseID): An instance containing the license key or user credentials.    
+
+**Return**:
+**License** object representing the activated license.
+
 #### load_license  
 Loads the license file and sets attributes for the LicenseData instance. Returns an instance of the License class reflecting the loaded license.
 
 ```python
 manager = LicenseManager(conf)
 
 license = manager.load_license()
@@ -555,14 +572,54 @@
 Checks if the licensing server is accessible. Returns True if online, False otherwise.
 
 ```python
 manager = LicenseManager(conf)
 
 license = manager.is_online()
 ```
+
+#### create_offline_activation_file
+Creates .req file for offline activation, including various optional parameters related to the device and software environment. 
+
+**Parameters**:
+
+* **license_id** (LicenseID): An instance containing the license key or user credentials.  
+* **req_path** (str): Specify the path where to create .req file.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H94R-S6KB-L7AJ-SXLK")
+
+req_file_path = manager.create_offline_activation_file(license_id,'offline_files/test')              
+```
+**Return** (str): Path of the .req file created for activation.
+
+#### activate_license_offline
+Activates a license offline using a .lic file provided via the specified path.
+
+**Parameters**:
+
+* **ls_activation_path** (str): Path to the activation file.
+
+```python
+file_path = 'offline_files/ls_activation.lic'
+
+manager = LicenseManager(conf)
+
+license = manager.activate_license_offline(file_path)
+```
+**Raises**:
+
+* **LicenseActivationException**: Activation data is not valid.
+* **LicenseActivationException**: Response file ID mismatch.
+* L**icenseActivationException**: License does not belong to this device.
+
+**Return**(License): Returns a License object representing the activated license.
+
 ### License object
 
 Object responsible for license operations
 
 
 #### is_validity_period_expired
 
@@ -731,27 +788,261 @@
 boolean = license.is_grace_period()
 ```
 **Return (bool)**: True if the license is within its grace period, False otherwise
 
 #### change_password
 
 Changes password of a user
+
+**Parameters**:
+
+* **password** (str): Old password of license user
+* **new_password**(str): New password of license user
+
  
 ```python
 manager = LicenseManager(conf)
 
 license_id = LicenseID.from_user(username="python@gmail.com",password="7t_x3!o9")
 
 license = manager.activate_license(license_id)
 
-license.change_password("7t_x3!o9","12345678")                    
+license.change_password(password="7t_x3!o9",new_password="12345678")                    
 ```
 **Return (str)**: "password_changed"
 
 
+#### setup_license_watch_dog
+
+Initializes and starts the license watchdog with the specified callback and timeout settings to monitor license activity or conditions.
+
+**Parameters**:
+
+**callback** (Callable): A callable to be executed by the watchdog in response to specific events or conditions.  
+**timeout** (int): The period in minutes after which the watchdog should perform its checks.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H7G3-F4PJ-4AEJ-UKYL")
+
+license = manager.activate_license(license_id)
+
+license.setup_license_watch_dog(callback,timeout)                   
+```
+
+
+**Return**: None
+
+#### stop_license_watch_dog
+
+Stops the license watchdog if it is currently running, effectively halting its monitoring and callback activities.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H7G3-F4PJ-4AEJ-UKYL")
+
+license = manager.activate_license(license_id)
+
+license.setup_license_watch_dog(callback,timeout)
+                                
+license.stop_license_watch_dog()                  
+```
+**Return**: None
+
+#### add_local_feature_consumption
+Adds local consumption to the feature.
+
+**Parameters**:
+* **feature** (str): feature code.
+* **consumptions** (int,optional): Number of consumptions.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H7G3-F4PJ-4AEJ-UKYL")
+
+license = manager.activate_license(license_id)
+
+license.add_local_feature_consumption("lkprod1cf1",3) 
+```    
+
+**Raises**:
+
+* **ItemNotFoundError**: If the feature specified by `feature_code` does not exist.
+
+* **LicenseSpringTypeError**: If the identified feature is not of the "consumption" type.
+
+* **ConsumptionError**: If adding the specified number of consumptions would exceed the feature's consumption limits.
+
+
+
+**Return**: None
+
+
+#### sync_feature_consumption
+Synchronizes local consumption data with the server.
+**Parameters**:
+
+* **feature** (str): feature code.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H7G3-F4PJ-4AEJ-UKYL")
+
+license = manager.activate_license(license_id)
+
+license.add_local_feature_consumption("lkprod1cf1",3)
+
+license.sync_feature_consumption("lkprod1cf1")
+```             
+
+**Return** (bool): True if the consumption data was successfully synchronized; False otherwise.
+
+
+#### floating_borrow
+Attempts to borrow a floating license until the specified date, updating the system status based on the outcome of the borrow attempt.
+
+**Parameters**:
+
+* **borrow_until** (str): A string representing the date until which the license should be borrowed.
+* **password** (str,optional): Password for the license if required.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H7G3-F4PJ-4AEJ-UKYL")
+
+license = manager.activate_license(license_id)
+
+license.floating_borrow("2031-05-06T00:00:00Z")    
+```  
+**Return**: None
+
+#### floating_release
+Releases a borrowed floating license and updates the license status accordingly.
+
+**Parameters**:
+
+* **throw_e**(bool): A boolean indicating whether to raise an exception on failure.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H7G3-F4PJ-4AEJ-UKYL")
+
+license = manager.activate_license(license_id)
+
+license.check()
+
+license.floating_release(False)   
+```  
+
+**Return**: None
+
+#### check_feature
+Checks for a specific license feature and updates the license cache accordingly.
+
+**Parameters**:
+
+* **feature**(str): feature code.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H7G3-F4PJ-4AEJ-UKYL")
+
+license = manager.activate_license(license_id)
+
+license.check_feature("lkprod1f1fc1")    
+```  
+
+**Return**: None
+
+#### release_feature
+Releases a borrowed license feature and updates the license cache accordingly.
+
+**Parameters**:
+
+* **feature**(str): feature code.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H7G3-F4PJ-4AEJ-UKYL")
+
+license = manager.activate_license(license_id)
+
+license.check_feature("lkprod1f1fc1")
+
+license.release_feature("lkprod1f1fc1")   
+```  
+
+**Return**: None
+
+#### update_offline
+Updates license via refresh file
+
+**Parameters**:
+
+* **path** (str): path of the refresh file
+* **reset_consumption** (bool): True resets consumption otherwise False
+
+
+```python
+file_path = 'path_to_lic_file/license.lic'
+
+manager = LicenseManager(conf)
+
+license = manager.activate_license_offline(file_path)
+
+license.update_offline('offline_files/license_refresh.lic',False)                      
+```  
+**Raises**:
+
+* **ConfigurationMismatch**: The update file does not belong to this device
+* **ConfigurationMismatch**: The update file does not belong to this product  
+
+**Return**(bool): True if license was successfully updated otherwise False
+
+#### deactivate_offline
+Generates .req file for the offline deactivation
+
+**Parameters**:
+
+* **offline_path**(str): path of the .req file
+
+
+```python
+file_path = 'path_to_lic_file/license.lic'
+
+manager = LicenseManager(conf)
+
+license = manager.activate_license_offline(file_path)
+
+license.deactivate_offline('path_where_to_create_req_file')
+
+                                
+                                  
+```  
+**Raises**:
+
+* **ConfigurationMismatch**: The update file does not belong to this device
+* **ConfigurationMismatch**: The update file does not belong to this product  
+
+**Return**(bool): True if license was successfully updated otherwise False
+
+
+
+
+
+                                
+
 ## License
 
 Copyright (C) 2023 by Cense Data Inc., support@licensespring.com
 
 ### Dependency licenses
 
 | Name               | Version   | License                                             | URL                                                      |
```

### Comparing `licensespring-2.0.1/licensespring/api/__init__.py` & `licensespring-3.0.0/licensespring/api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,18 +215,17 @@
     def deactivate_license(
         self,
         product,
         bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
-        password=None,
     ):
         data = self.request_generic_data(
-            {}, product, bundle_code, hardware_id, license_key, username, password
+            {}, product, bundle_code, hardware_id, license_key, username
         )
 
         response = self.send_request(
             method="post",
             endpoint="/deactivate_license",
             json_data=data,
         )
@@ -303,15 +302,15 @@
         data["signature"] = offline_signature(
             self.api_key, self.shared_key, data["hardware_id"], license_key, username
         )
         data["request_id"] = self.hardware_id_provider.get_request_id()
 
         return base64.b64encode(json.dumps(data).encode()).decode()
 
-    def activate_offline_load(self, data, hardware_id=None):
+    def activate_offline_load(self, data):
         decoded_data = base64.b64decode(data).decode()
         response_json = json.loads(decoded_data)
 
         if self.verify_license_signature:
             response_json_sig_v2_check_data = json.loads(
                 decoded_data, object_pairs_hook=OrderedDict
             )
@@ -324,14 +323,34 @@
             )
             self.signature_verifier.verify_license_signature_v2(
                 response_json_sig_v2_check_string.encode(), license_signature_v2
             )
 
         return response_json
 
+    def check_offline_load(self, data):
+        decoded_data = base64.b64decode(data).decode()
+        response_json = json.loads(decoded_data)
+
+        if self.verify_license_signature:
+            response_json_sig_v2_check_data = json.loads(
+                decoded_data, object_pairs_hook=OrderedDict
+            )
+            license_signature_v2 = response_json_sig_v2_check_data.pop(
+                "license_signature_v2"
+            )
+            response_json_sig_v2_check_string = json.dumps(
+                response_json_sig_v2_check_data, separators=(",", ":")
+            )
+            self.signature_verifier.verify_license_signature_v2(
+                response_json_sig_v2_check_string.encode(), license_signature_v2
+            )
+
+        return response_json
+
     def activate_offline(self, data):
         response = self.send_request(
             method="post",
             endpoint="/activate_offline",
             custom_headers={"Content-type": "text/plain"},
             data=data,
         )
@@ -357,26 +376,25 @@
     def deactivate_offline_dump(
         self,
         product,
         bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
-        password=None,
         app_ver=None,
         os_ver=None,
         hostname=None,
         ip=None,
         mac_address=None,
         consumptions=None,
         product_features=None,
     ):
         data = {"request": "deactivation"}
         data = self.request_generic_data(
-            data, product, bundle_code, hardware_id, license_key, username, password
+            data, product, bundle_code, hardware_id, license_key, username
         )
         data = self.request_hardware_data(
             data=data,
             os_ver=os_ver,
             hostname=hostname,
             ip=ip,
             mac_address=mac_address,
@@ -412,21 +430,20 @@
     def add_consumption(
         self,
         product,
         bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
-        password=None,
         consumptions=None,
         max_overages=None,
         allow_overages=None,
     ):
         data = self.request_generic_data(
-            {}, product, bundle_code, hardware_id, license_key, username, password
+            {}, product, bundle_code, hardware_id, license_key, username
         )
         data = self.request_additional_data(
             data=data,
             additional_data={
                 "consumptions": consumptions,
                 "max_overages": max_overages,
                 "allow_overages": allow_overages,
@@ -449,20 +466,19 @@
     def add_feature_consumption(
         self,
         product,
         bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
-        password=None,
         feature=None,
         consumptions=None,
     ):
         data = self.request_generic_data(
-            {}, product, bundle_code, hardware_id, license_key, username, password
+            {}, product, bundle_code, hardware_id, license_key, username
         )
         data["feature"] = feature
         data = self.request_additional_data(
             data=data,
             additional_data={
                 "consumptions": consumptions,
             },
```

### Comparing `licensespring-2.0.1/licensespring/api/authorization.py` & `licensespring-3.0.0/licensespring/api/authorization.py`

 * *Files identical despite different names*

### Comparing `licensespring-2.0.1/licensespring/api/error.py` & `licensespring-3.0.0/licensespring/api/error.py`

 * *Files identical despite different names*

### Comparing `licensespring-2.0.1/licensespring/api/signature.py` & `licensespring-3.0.0/licensespring/api/signature.py`

 * *Files identical despite different names*

### Comparing `licensespring-2.0.1/licensespring/hardware/__init__.py` & `licensespring-3.0.0/licensespring/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `licensespring-2.0.1/licensespring/licensefile/__init__.py` & `licensespring-3.0.0/licensespring/licensefile/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     ClockTamperedException,
     ConfigurationMismatch,
     ErrorType,
     LicenseStateException,
     TimeoutExpiredException,
     VMIsNotAllowedException,
 )
+from licensespring.licensefile.offline_activation_guard import OfflineActivation
 from licensespring.watchdog import LicenseWatchdog
 
 
 class License:
     """
     Represents and manages license operations including activation, deactivation,
     and consumption tracking for a software product.
@@ -125,18 +126,22 @@
 
         try:
             # Add logic for floating server
             logging.info("Online check started")
 
             response = self.api_client.check_license(
                 product=self.licensefile_handler._cache.product,
-                bundle_code=self.licensefile_handler._cache.bundle_code,
+                bundle_code=getattr(
+                    self.licensefile_handler._cache, "bundle_code", None
+                ),
                 hardware_id=None,
-                license_key=self.licensefile_handler._cache.license_key,
-                username=self.licensefile_handler._cache.username,
+                license_key=getattr(
+                    self.licensefile_handler._cache, "license_key", None
+                ),
+                username=getattr(self.licensefile_handler._cache, "username", None),
                 include_expired_features=include_expired_features,
             )
 
             self.licensefile_handler._cache.update_cache("check_license", response)
             self.licensefile_handler._cache.update_floating_period(
                 self.licensefile_handler._cache.borrowed_until
             )
@@ -190,19 +195,18 @@
         if not self.licensefile_handler._cache.license_active:
             if delete_license:
                 self.licensefile_handler.delete_licensefile()
             return None
 
         self.api_client.deactivate_license(
             product=self.licensefile_handler._cache.product,
-            bundle_code=self.licensefile_handler._cache.bundle_code,
+            bundle_code=getattr(self.licensefile_handler._cache, "bundle_code", None),
             hardware_id=None,
-            license_key=self.licensefile_handler._cache.license_key,
-            username=self.licensefile_handler._cache.username,
-            password=self.licensefile_handler._cache.password,
+            license_key=getattr(self.licensefile_handler._cache, "license_key", None),
+            username=getattr(self.licensefile_handler._cache, "username", None),
         )
 
         if delete_license:
             self.licensefile_handler.delete_licensefile()
             return None
 
         self.licensefile_handler._cache.deactivate()
@@ -271,21 +275,19 @@
         Returns:
             str: password was changed.
         """
 
         self.check_license_status()
 
         response = self.api_client.change_password(
-            self.licensefile_handler._cache.username,
+            username=getattr(self.licensefile_handler._cache, "username", None),
             password=password,
             new_password=new_password,
         )
 
-        self.licensefile_handler._cache.update_password(new_password)
-
         return response
 
     def add_local_consumption(self, consumptions=1) -> None:
         """
         Adds local consumption to the license
         Params:
             consumptions (int,optional): Number of consumptions.
@@ -329,19 +331,22 @@
 
         if feature_obj.local_consumption == 0:
             return False
 
         try:
             response = self.api_client.add_feature_consumption(
                 product=self.product,
-                bundle_code=self.licensefile_handler._cache.bundle_code,
+                bundle_code=getattr(
+                    self.licensefile_handler._cache, "bundle_code", None
+                ),
                 hardware_id=None,
-                license_key=self.licensefile_handler._cache.license_key,
-                username=self.licensefile_handler._cache.username,
-                password=self.licensefile_handler._cache.password,
+                license_key=getattr(
+                    self.licensefile_handler._cache, "license_key", None
+                ),
+                username=getattr(self.licensefile_handler._cache, "username", None),
                 feature=feature,
                 consumptions=feature_obj.local_consumption,
             )
 
         except ClientError as ex:
             logging.info(ex)
             raise ex
@@ -403,18 +408,21 @@
 
             else:
                 max_overages = None
                 allow_overages = None
 
             response = self.api_client.add_consumption(
                 product=self.licensefile_handler._cache.product,
-                bundle_code=self.licensefile_handler._cache.bundle_code,
-                license_key=self.licensefile_handler._cache.license_key,
-                username=self.licensefile_handler._cache.username,
-                password=self.licensefile_handler._cache.password,
+                bundle_code=getattr(
+                    self.licensefile_handler._cache, "bundle_code", None
+                ),
+                license_key=getattr(
+                    self.licensefile_handler._cache, "license_key", None
+                ),
+                username=getattr(self.licensefile_handler._cache, "username", None),
                 consumptions=self.licensefile_handler._cache.local_consumption,
                 max_overages=max_overages,
                 allow_overages=allow_overages,
             )
 
         except ClientError as ex:
             logging.info(ex)
@@ -483,29 +491,30 @@
             callback: A callable to be executed by the watchdog in response to specific events or conditions.
             timeout: The period in minutes after which the watchdog should perform its checks.
 
         Side Effects:
             - Instantiates the LicenseWatchdog class and stores the instance.
             - Starts the watchdog thread.
         """
+
         self.watch_dog = LicenseWatchdog(self, callback, timeout)
         self.watch_dog.run()
 
     def stop_license_watch_dog(self) -> None:
         """
         Stops the license watchdog if it is currently running.
 
         Side Effects:
             - Stops the watchdog thread, if it exists.
         """
 
         if self.watch_dog:
             self.watch_dog.stop()
 
-    def floating_borrow(self, borrow_until: str) -> None:
+    def floating_borrow(self, borrow_until: str, password: str = None) -> None:
         """
         Attempts to borrow a floating license until the specified date.
 
         Args:
             borrow_until: A string representing the date until which the license should be borrowed.
 
         Returns:
@@ -517,25 +526,24 @@
         """
 
         if not self.licensefile_handler._cache.is_floating_license():
             return None
 
         response = self.api_client.floating_borrow(
             product=self.licensefile_handler._cache.product,
-            bundle_code=self.licensefile_handler._cache.bundle_code,
+            bundle_code=getattr(self.licensefile_handler._cache, "bundle_code", None),
             hardware_id=None,
-            license_key=self.licensefile_handler._cache.license_key,
-            username=self.licensefile_handler._cache.username,
+            license_key=getattr(self.licensefile_handler._cache, "license_key", None),
+            username=getattr(self.licensefile_handler._cache, "username", None),
+            password=password,
             borrowed_until=borrow_until,
         )
 
         self.licensefile_handler._cache.set_boolean("is_borrowed", True)
-
         self.stop_license_watch_dog()
-
         self.licensefile_handler._cache.update_cache("normal", response)
         self.licensefile_handler._cache.update_floating_period(
             self.licensefile_handler._cache.borrowed_until
         )
         self.licensefile_handler.save_licensefile()
 
     def floating_release(self, throw_e: bool):
@@ -556,22 +564,25 @@
         if not self.licensefile_handler._cache.is_floating_license():
             return None
 
         try:
             self.check_license_status()
 
             # Add logic for both floating cloud and floating license
-
             if self.licensefile_handler._cache.is_active_floating_cloud():
                 self.api_client.floating_release(
                     product=self.licensefile_handler._cache.product,
-                    bundle_code=self.licensefile_handler._cache.bundle_code,
+                    bundle_code=getattr(
+                        self.licensefile_handler._cache, "bundle_code", None
+                    ),
                     hardware_id=None,
-                    license_key=self.licensefile_handler._cache.license_key,
-                    username=self.licensefile_handler._cache.username,
+                    license_key=getattr(
+                        self.licensefile_handler._cache, "license_key", None
+                    ),
+                    username=getattr(self.licensefile_handler._cache, "username", None),
                 )
 
                 self.licensefile_handler._cache.release_license()
                 self.licensefile_handler.save_licensefile()
 
         except Exception as ex:
             if throw_e:
@@ -584,26 +595,28 @@
 
         Args:
             feature: feature code.
             add_to_watchdog: A boolean indicating whether to add the feature check to a watchdog routine.
 
         Returns:
             None
-
-
         """
         # Add watchdog logic
         try:
             response = self.api_client.check_license_feature(
                 product=self.licensefile_handler._cache.product,
                 feature=feature,
-                bundle_code=self.licensefile_handler._cache.bundle_code,
+                bundle_code=getattr(
+                    self.licensefile_handler._cache, "bundle_code", None
+                ),
                 hardware_id=None,
-                license_key=self.licensefile_handler._cache.license_key,
-                username=self.licensefile_handler._cache.username,
+                license_key=getattr(
+                    self.licensefile_handler._cache, "license_key", None
+                ),
+                username=getattr(self.licensefile_handler._cache, "username", None),
             )
 
             self.licensefile_handler._cache.register_feature(feature)
             self.licensefile_handler._cache.update_cache(
                 "register_feature", response, feature
             )
 
@@ -625,19 +638,95 @@
         """
 
         # Add watchdog logic
         try:
             self.api_client.floating_feature_release(
                 product=self.licensefile_handler._cache.product,
                 feature=feature,
-                bundle_code=self.licensefile_handler._cache.bundle_code,
+                bundle_code=getattr(
+                    self.licensefile_handler._cache, "bundle_code", None
+                ),
                 hardware_id=None,
-                license_key=self.licensefile_handler._cache.license_key,
-                username=self.licensefile_handler._cache.username,
+                license_key=getattr(
+                    self.licensefile_handler._cache, "license_key", None
+                ),
+                username=getattr(self.licensefile_handler._cache, "username", None),
             )
 
             self.licensefile_handler._cache.release_feature(feature)
             self.licensefile_handler.save_licensefile()
 
         except Exception as ex:
             logging.info(ex)
             raise ex
+
+    def update_offline(self, path: str, reset_consumption: bool) -> bool:
+        """
+        Updates license via refresh file
+
+        Args:
+            path (str): path of the refresh file
+            reset_consumption (bool): True resets consumption otherwise False
+
+        Raises:
+            ConfigurationMismatch: The update file does not belong to this device
+            ConfigurationMismatch: The update file does not belong to this product
+
+        Returns:
+            bool: True if license was successfully updated otherwise False
+        """
+
+        data = self.licensefile_handler.load_offline_response(path)
+        decoded_data = self.api_client.check_offline_load(data)
+
+        if decoded_data["hardware_id"] != self.licensefile_handler._cache.hardware_id:
+            raise ConfigurationMismatch(
+                ErrorType.HARDWARE_ID_MISMATCH,
+                " The update file does not belong to this device. ",
+            )
+
+        if (
+            decoded_data["product_details"]["short_code"]
+            != self.licensefile_handler._cache.product
+        ):
+            raise ConfigurationMismatch(
+                ErrorType.PRODUCT_MISMATCH,
+                " The update file does not belong to this product.",
+            )
+
+        if (
+            reset_consumption == True
+            and self.licensefile_handler._cache.license_type == "consumption"
+        ):
+            self.licensefile_handler._cache.reset_consumption()
+
+        self.licensefile_handler._cache.update_cache(
+            "activate_license_offline", decoded_data
+        )
+        self.licensefile_handler.save_licensefile()
+
+        return True
+
+    def deactivate_offline(self, offline_path: str) -> str:
+        """
+        Generates .req file for the offline deactivation
+
+        Args:
+            offline_path (str): path of the .req file
+
+        Returns:
+            str: path of the deactivation file
+        """
+
+        self.licensefile_handler._cache.deactivate()
+        data = self.api_client.deactivate_offline_dump(
+            product=self.product,
+            bundle_code=getattr(self.licensefile_handler._cache, "bundle_code", None),
+            hardware_id=self.licensefile_handler._cache.hardware_id,
+            license_key=getattr(self.licensefile_handler._cache, "license_key", None),
+            username=getattr(self.licensefile_handler._cache, "username", None),
+        )
+        offline_data = OfflineActivation()
+        offline_data.set_is_activation(False)
+        offline_data.set_data(data)
+
+        return self.licensefile_handler.create_request_file(offline_data, offline_path)
```

### Comparing `licensespring-2.0.1/licensespring/licensefile/config.py` & `licensespring-3.0.0/licensespring/licensefile/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         verify_license_signature (bool): Flag to enable/disable signature verification. Default is True.
         signature_verifier (object): Verifier class for checking signatures. Default is SignatureVerifier.
         api_domain (str): Domain for the API server. Default is "api.licensespring.com".
         api_version (str): Version of the API. Default is "v4".
         filename (str): Name for the license file. Default is "License".
         file_path (str): Path to save the license file. Default is None.
         grace_period_conf (int): Grace period configuration in days. Default is 12.
+        is_guard_file_enabled (bool): Enables guard protection for offline licenses if set to True.
     """
 
     def __init__(
         self,
         product: str,
         api_key: str,
         shared_key: str,
@@ -39,14 +40,15 @@
         verify_license_signature=True,
         signature_verifier=SignatureVerifier,
         api_domain="api.licensespring.com",
         api_version="v4",
         filename="License",
         file_path=None,
         grace_period_conf=24,
+        is_guard_file_enabled=True,
     ) -> None:
         self._product = product
 
         self._api_key = api_key
         self._shared_key = shared_key
 
         self._file_key = file_key
@@ -58,7 +60,8 @@
         self._signature_verifier = signature_verifier
         self._api_domain = api_domain
         self._api_version = api_version
 
         self._filename = filename
         self._file_path = file_path
         self.grace_period_conf = grace_period_conf
+        self.is_guard_file_enabled = is_guard_file_enabled
```

### Comparing `licensespring-2.0.1/licensespring/licensefile/default_crypto.py` & `licensespring-3.0.0/licensespring/licensefile/default_crypto.py`

 * *Files identical despite different names*

### Comparing `licensespring-2.0.1/licensespring/licensefile/error.py` & `licensespring-3.0.0/licensespring/licensefile/error.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,18 @@
     CLOCK_TAMPERED = auto()
 
     NOT_ENOUGH_LICENSE_CONSUMPTIONS = auto()
     NOT_ENOUGH_FEATURE_CONSUMPTIONS = auto()
 
     UNSUPPORTED_PRODUCT_FEATURE = auto()
 
+    """activation"""
+
+    OFFLINE_ACTIVATION_ERROR = auto()
+
 
 class LicenseSpringException(Exception):
     """Base exception class for all LicenseSpring-related errors."""
 
     def __init__(self, error_type: ErrorType, message):
         self.error_type = error_type
         self.message = message
@@ -48,14 +52,19 @@
             self.message,
         )
 
     def __str__(self) -> str:
         return f"{self.error_type} ({self.error_type.value}): {self.message}"
 
 
+class LicenseActivationException(LicenseSpringException):
+    def __init__(self, error_type: ErrorType, message):
+        super().__init__(error_type, message)
+
+
 class LicenseDeleted(LicenseSpringException):
     def __init__(self, error_type: ErrorType, message):
         super().__init__(error_type, message)
 
 
 class LicenseStateException(LicenseSpringException):
     def __init__(self, error_type: ErrorType, message):
```

### Comparing `licensespring-2.0.1/licensespring/licensefile/feature_manager.py` & `licensespring-3.0.0/licensespring/licensefile/feature_manager.py`

 * *Files identical despite different names*

### Comparing `licensespring-2.0.1/licensespring/licensefile/license_data.py` & `licensespring-3.0.0/licensespring/licensefile/license_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,14 @@
         update_feature_consumption(feature, consumptions=1): Adds a specified number of local consumptions to a feature.
 
         release_license():Handles operations on licensefile for releasing license.
         register_feature(feature_code): Handles feature check.
         release_feature(feature_code:str): Handles feature release.
         set_boolean(field_name:str,bool:bool): set boolean of field_name.
 
-
-
-
     """
 
     datetime_attributes = [
         "last_check",
         "last_usage",
         "floating_period",
         "maintenance_period",
@@ -160,21 +157,30 @@
         Returns: None
         """
         with self._lock:
             self.last_usage = datetime.now(timezone.utc).replace(tzinfo=None)
 
             if method == "check_license":
                 self.last_check = datetime.now(timezone.utc).replace(tzinfo=None)
-
                 self.from_json_to_attr(response)
 
             elif method == "activate_license":
                 self.from_json_to_attr(response)
                 self.local_consumption_setup()
+                self.grace_period_setup()
 
+                self.license_enabled = True
+                self.is_expired = False
+                self.license_active = True
+
+            elif method == "activate_license_offline":
+                response.update(response["product_details"])
+                del response["product_details"]
+                self.from_json_to_attr(response)
+                self.local_consumption_setup()
                 self.grace_period_setup()
 
                 self.license_enabled = True
                 self.is_expired = False
                 self.license_active = True
 
             elif method == "normal":
@@ -279,18 +285,14 @@
                 self.times_activated -= 1
 
             else:
                 self.times_activated = 0
 
             self.license_active = False
 
-    def update_password(self, new_password):
-        with self._lock:
-            self.password = new_password
-
     def update_consumption(self, consumptions: int):
         """
         Adds local consumptions for consumption-based licenses.
 
         Args:
             consumptions (int): The number of consumptions to add locally.
 
@@ -319,25 +321,37 @@
                     ErrorType.NOT_ENOUGH_LICENSE_CONSUMPTIONS,
                     "Not enough conusmptions left!",
                 )
 
             else:
                 self.local_consumption += consumptions
 
+    def reset_consumption(self):
+        with self._lock:
+            self.local_consumption = 0
+
     def is_floating_license(self):
         return self.is_floating or self.is_floating_cloud
 
     def update_feature_consumption(self, feature, consumptions=1):
         """
         Adds a specified number of consumptions to a local feature, updating its consumption count.
         """
+
         with self._lock:
             self.feature_manager.add_local_consumption(feature, consumptions)
 
     def update_floating_period(self, end_date: datetime) -> None:
+        """
+        Updates floating end time if needed
+
+        Args:
+            end_date (datetime): end date of floating
+        """
+
         with self._lock:
             if self.is_floating_license():
                 floating_end = (
                     timedelta(minutes=self.floating_timeout) + self.floating_period
                 )
 
                 if isinstance(end_date, datetime):
@@ -350,30 +364,41 @@
         """
         Handles operations on licensefile for releasing license
 
         1. Sets `self.is_borrowed` to False, indicating the license is no longer borrowed.
         2. Resets `self.borrowed_until` to None, clearing the timestamp until which the license was borrowed.
         3. Decrements `self.floating_in_use_devices` by 1, reducing the count of devices currently using a floating license by one.
         """
+
         with self._lock:
             self.is_borrowed = False
             self.borrowed_until = None
             self.floating_in_use_devices -= 1
             self.floating_period = datetime.now(timezone.utc).replace(tzinfo=None)
 
     def register_feature(self, feature_code: str):
         """
         Handles feature check
         """
+
         with self._lock:
             self.feature_manager.register_feature(feature_code)
 
     def release_feature(self, feature_code: str):
         """
         Handles feature release
         """
+
         with self._lock:
             self.feature_manager.release_feature(feature_code)
 
     def set_boolean(self, field_name: str, bool: bool):
+        """
+        Changes/Sets LicenseData field to boolean value
+
+        Args:
+            field_name (str): field name
+            bool (bool): True/False
+        """
+
         with self._lock:
             setattr(self, field_name, bool)
```

### Comparing `licensespring-2.0.1/licensespring/watchdog/__init__.py` & `licensespring-3.0.0/licensespring/watchdog/__init__.py`

 * *Files identical despite different names*

### Comparing `licensespring-2.0.1/licensespring/webhook/signature.py` & `licensespring-3.0.0/licensespring/webhook/signature.py`

 * *Files identical despite different names*

### Comparing `licensespring-2.0.1/licensespring/webhook/utils.py` & `licensespring-3.0.0/licensespring/webhook/utils.py`

 * *Files identical despite different names*

### Comparing `licensespring-2.0.1/pyproject.toml` & `licensespring-3.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "licensespring"
-version = "2.0.1"
+version = "3.0.0"
 description = "LicenseSpring Python Library"
 license = "MIT"
 authors = ["Toni Sredanović <toni@licensespring.com>"]
 readme = "README.md"
 homepage = "https://licensespring.com/"
 documentation = "https://docs.licensespring.com/sdks/python"
```

### Comparing `licensespring-2.0.1/PKG-INFO` & `licensespring-3.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensespring
-Version: 2.0.1
+Version: 3.0.0
 Summary: LicenseSpring Python Library
 Home-page: https://licensespring.com/
 License: MIT
 Author: Toni Sredanović
 Author-email: toni@licensespring.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -174,18 +174,17 @@
 api_client.deactivate_license(product=product, license_key=license_key)
 ```
 
 ### Deactivate user based license
 ```python
 product = "uprod1"
 username = "user1@email.com"
-password = "nq64k1!@"
 
 api_client.deactivate_license(
-    product=product, username=username, password=password
+    product=product, username=username
 )
 ```
 
 ### Check key based license
 ```python
 product = "lkprod1"
 license_key = "GPBQ-DZCP-E9SK-CQLK"
@@ -427,14 +426,26 @@
     ls_activation_data = file.read()
 
 license_data = api_client.activate_offline_load(ls_activation_data)
 
 print(license_data)
 ```
 
+### Check offline load
+```python
+# Read from file
+with open('./license_refresh.lic') as file:
+    license_refresh_data = file.read()
+
+license_data = api_client.check_offline_load(license_refresh_data)
+
+print(license_data)
+```
+
+
 ### Deactivate offline
 ```python
 product = "lkprod1"
 license_key = "GPYC-X5J2-L5SK-C3LK"
 
 # Generate data for offline deactivation
 deactivate_offline_data = api_client.deactivate_offline_dump(
@@ -543,15 +554,15 @@
 manager = LicenseManager(conf)
 ```
 #### Configuration parametres
 
 conf (Configuration): **[A configuration object](#configuration-setup)**
 
 #### activate_license
-Activates a license with the license server and updates local license data.Returns an instance of the License
+Activates a license with the license server and updates local license data.
 
 **Key-based**
 ```python
 manager = LicenseManager(conf)
 
 license_id = LicenseID.from_key("H6QM-6H5R-ZENJ-VBLK")
 
@@ -561,14 +572,20 @@
 ```python
 manager = LicenseManager(conf)
 
 license_id = LicenseID.from_user(username="python@gmail.com",password="7t_x3!o9")
 
 license = manager.activate_license(license_id)
 ```
+**Parameters**:  
+* **license_id** (LicenseID): An instance containing the license key or user credentials.    
+
+**Return**:
+**License** object representing the activated license.
+
 #### load_license  
 Loads the license file and sets attributes for the LicenseData instance. Returns an instance of the License class reflecting the loaded license.
 
 ```python
 manager = LicenseManager(conf)
 
 license = manager.load_license()
@@ -577,14 +594,54 @@
 Checks if the licensing server is accessible. Returns True if online, False otherwise.
 
 ```python
 manager = LicenseManager(conf)
 
 license = manager.is_online()
 ```
+
+#### create_offline_activation_file
+Creates .req file for offline activation, including various optional parameters related to the device and software environment. 
+
+**Parameters**:
+
+* **license_id** (LicenseID): An instance containing the license key or user credentials.  
+* **req_path** (str): Specify the path where to create .req file.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H94R-S6KB-L7AJ-SXLK")
+
+req_file_path = manager.create_offline_activation_file(license_id,'offline_files/test')              
+```
+**Return** (str): Path of the .req file created for activation.
+
+#### activate_license_offline
+Activates a license offline using a .lic file provided via the specified path.
+
+**Parameters**:
+
+* **ls_activation_path** (str): Path to the activation file.
+
+```python
+file_path = 'offline_files/ls_activation.lic'
+
+manager = LicenseManager(conf)
+
+license = manager.activate_license_offline(file_path)
+```
+**Raises**:
+
+* **LicenseActivationException**: Activation data is not valid.
+* **LicenseActivationException**: Response file ID mismatch.
+* L**icenseActivationException**: License does not belong to this device.
+
+**Return**(License): Returns a License object representing the activated license.
+
 ### License object
 
 Object responsible for license operations
 
 
 #### is_validity_period_expired
 
@@ -753,27 +810,261 @@
 boolean = license.is_grace_period()
 ```
 **Return (bool)**: True if the license is within its grace period, False otherwise
 
 #### change_password
 
 Changes password of a user
+
+**Parameters**:
+
+* **password** (str): Old password of license user
+* **new_password**(str): New password of license user
+
  
 ```python
 manager = LicenseManager(conf)
 
 license_id = LicenseID.from_user(username="python@gmail.com",password="7t_x3!o9")
 
 license = manager.activate_license(license_id)
 
-license.change_password("7t_x3!o9","12345678")                    
+license.change_password(password="7t_x3!o9",new_password="12345678")                    
 ```
 **Return (str)**: "password_changed"
 
 
+#### setup_license_watch_dog
+
+Initializes and starts the license watchdog with the specified callback and timeout settings to monitor license activity or conditions.
+
+**Parameters**:
+
+**callback** (Callable): A callable to be executed by the watchdog in response to specific events or conditions.  
+**timeout** (int): The period in minutes after which the watchdog should perform its checks.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H7G3-F4PJ-4AEJ-UKYL")
+
+license = manager.activate_license(license_id)
+
+license.setup_license_watch_dog(callback,timeout)                   
+```
+
+
+**Return**: None
+
+#### stop_license_watch_dog
+
+Stops the license watchdog if it is currently running, effectively halting its monitoring and callback activities.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H7G3-F4PJ-4AEJ-UKYL")
+
+license = manager.activate_license(license_id)
+
+license.setup_license_watch_dog(callback,timeout)
+                                
+license.stop_license_watch_dog()                  
+```
+**Return**: None
+
+#### add_local_feature_consumption
+Adds local consumption to the feature.
+
+**Parameters**:
+* **feature** (str): feature code.
+* **consumptions** (int,optional): Number of consumptions.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H7G3-F4PJ-4AEJ-UKYL")
+
+license = manager.activate_license(license_id)
+
+license.add_local_feature_consumption("lkprod1cf1",3) 
+```    
+
+**Raises**:
+
+* **ItemNotFoundError**: If the feature specified by `feature_code` does not exist.
+
+* **LicenseSpringTypeError**: If the identified feature is not of the "consumption" type.
+
+* **ConsumptionError**: If adding the specified number of consumptions would exceed the feature's consumption limits.
+
+
+
+**Return**: None
+
+
+#### sync_feature_consumption
+Synchronizes local consumption data with the server.
+**Parameters**:
+
+* **feature** (str): feature code.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H7G3-F4PJ-4AEJ-UKYL")
+
+license = manager.activate_license(license_id)
+
+license.add_local_feature_consumption("lkprod1cf1",3)
+
+license.sync_feature_consumption("lkprod1cf1")
+```             
+
+**Return** (bool): True if the consumption data was successfully synchronized; False otherwise.
+
+
+#### floating_borrow
+Attempts to borrow a floating license until the specified date, updating the system status based on the outcome of the borrow attempt.
+
+**Parameters**:
+
+* **borrow_until** (str): A string representing the date until which the license should be borrowed.
+* **password** (str,optional): Password for the license if required.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H7G3-F4PJ-4AEJ-UKYL")
+
+license = manager.activate_license(license_id)
+
+license.floating_borrow("2031-05-06T00:00:00Z")    
+```  
+**Return**: None
+
+#### floating_release
+Releases a borrowed floating license and updates the license status accordingly.
+
+**Parameters**:
+
+* **throw_e**(bool): A boolean indicating whether to raise an exception on failure.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H7G3-F4PJ-4AEJ-UKYL")
+
+license = manager.activate_license(license_id)
+
+license.check()
+
+license.floating_release(False)   
+```  
+
+**Return**: None
+
+#### check_feature
+Checks for a specific license feature and updates the license cache accordingly.
+
+**Parameters**:
+
+* **feature**(str): feature code.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H7G3-F4PJ-4AEJ-UKYL")
+
+license = manager.activate_license(license_id)
+
+license.check_feature("lkprod1f1fc1")    
+```  
+
+**Return**: None
+
+#### release_feature
+Releases a borrowed license feature and updates the license cache accordingly.
+
+**Parameters**:
+
+* **feature**(str): feature code.
+
+```python
+manager = LicenseManager(conf)
+
+license_id = LicenseID.from_key("H7G3-F4PJ-4AEJ-UKYL")
+
+license = manager.activate_license(license_id)
+
+license.check_feature("lkprod1f1fc1")
+
+license.release_feature("lkprod1f1fc1")   
+```  
+
+**Return**: None
+
+#### update_offline
+Updates license via refresh file
+
+**Parameters**:
+
+* **path** (str): path of the refresh file
+* **reset_consumption** (bool): True resets consumption otherwise False
+
+
+```python
+file_path = 'path_to_lic_file/license.lic'
+
+manager = LicenseManager(conf)
+
+license = manager.activate_license_offline(file_path)
+
+license.update_offline('offline_files/license_refresh.lic',False)                      
+```  
+**Raises**:
+
+* **ConfigurationMismatch**: The update file does not belong to this device
+* **ConfigurationMismatch**: The update file does not belong to this product  
+
+**Return**(bool): True if license was successfully updated otherwise False
+
+#### deactivate_offline
+Generates .req file for the offline deactivation
+
+**Parameters**:
+
+* **offline_path**(str): path of the .req file
+
+
+```python
+file_path = 'path_to_lic_file/license.lic'
+
+manager = LicenseManager(conf)
+
+license = manager.activate_license_offline(file_path)
+
+license.deactivate_offline('path_where_to_create_req_file')
+
+                                
+                                  
+```  
+**Raises**:
+
+* **ConfigurationMismatch**: The update file does not belong to this device
+* **ConfigurationMismatch**: The update file does not belong to this product  
+
+**Return**(bool): True if license was successfully updated otherwise False
+
+
+
+
+
+                                
+
 ## License
 
 Copyright (C) 2023 by Cense Data Inc., support@licensespring.com
 
 ### Dependency licenses
 
 | Name               | Version   | License                                             | URL                                                      |
```

