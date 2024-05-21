# Comparing `tmp/slurpit_sdk-0.9.20.tar.gz` & `tmp/slurpit_sdk-0.9.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurpit_sdk-0.9.20.tar", max compression
+gzip compressed data, was "slurpit_sdk-0.9.22.tar", max compression
```

## Comparing `slurpit_sdk-0.9.20.tar` & `slurpit_sdk-0.9.22.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1064 2024-05-21 08:59:38.455182 slurpit_sdk-0.9.20/LICENSE
--rw-r--r--   0        0        0     1712 2024-05-21 12:12:56.770682 slurpit_sdk-0.9.20/README.md
--rw-r--r--   0        0        0      297 2024-05-21 12:14:07.339204 slurpit_sdk-0.9.20/pyproject.toml
--rw-r--r--   0        0        0       57 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/__init__.py
--rw-r--r--   0        0        0     2225 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/api.py
--rw-r--r--   0        0        0        0 2024-05-21 12:14:07.459205 slurpit_sdk-0.9.20/src/slurpit/apis/__init__.py
--rw-r--r--   0        0        0     7053 2024-05-14 19:35:54.536903 slurpit_sdk-0.9.20/src/slurpit/apis/baseapi.py
--rw-r--r--   0        0        0    11256 2024-05-20 10:32:39.146951 slurpit_sdk-0.9.20/src/slurpit/apis/deviceapi.py
--rw-r--r--   0        0        0     4068 2024-05-21 08:05:20.334037 slurpit_sdk-0.9.20/src/slurpit/apis/planningapi.py
--rw-r--r--   0        0        0     1198 2024-05-20 12:11:15.309046 slurpit_sdk-0.9.20/src/slurpit/apis/platformapi.py
--rw-r--r--   0        0        0     7944 2024-05-20 10:32:39.146951 slurpit_sdk-0.9.20/src/slurpit/apis/scannerapi.py
--rw-r--r--   0        0        0    14816 2024-05-20 12:11:15.309046 slurpit_sdk-0.9.20/src/slurpit/apis/scraperapi.py
--rw-r--r--   0        0        0     8150 2024-05-21 08:05:20.334037 slurpit_sdk-0.9.20/src/slurpit/apis/templateapi.py
--rw-r--r--   0        0        0     4839 2024-05-20 10:32:39.146951 slurpit_sdk-0.9.20/src/slurpit/apis/userapi.py
--rw-r--r--   0        0        0     4431 2024-05-20 10:32:39.146951 slurpit_sdk-0.9.20/src/slurpit/apis/vaultapi.py
--rw-r--r--   0        0        0        0 2024-05-21 12:14:07.463205 slurpit_sdk-0.9.20/src/slurpit/models/__init__.py
--rw-r--r--   0        0        0       27 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/models/basemodel.py
--rw-r--r--   0        0        0     2606 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/models/device.py
--rw-r--r--   0        0        0     1301 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/models/planning.py
--rw-r--r--   0        0        0      396 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/models/platform.py
--rw-r--r--   0        0        0     2017 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/models/scanner.py
--rw-r--r--   0        0        0     1932 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/models/template.py
--rw-r--r--   0        0        0     2107 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/models/user.py
--rw-r--r--   0        0        0     2738 2024-05-12 14:26:16.355136 slurpit_sdk-0.9.20/src/slurpit/models/vault.py
--rw-r--r--   0        0        0     2209 1970-01-01 00:00:00.000000 slurpit_sdk-0.9.20/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-21 13:11:58.110837 slurpit_sdk-0.9.22/LICENSE
+-rw-r--r--   0        0        0     1712 2024-05-21 13:11:58.110837 slurpit_sdk-0.9.22/README.md
+-rw-r--r--   0        0        0      297 2024-05-21 14:00:11.741582 slurpit_sdk-0.9.22/pyproject.toml
+-rw-r--r--   0        0        0       57 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/__init__.py
+-rw-r--r--   0        0        0     2225 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/api.py
+-rw-r--r--   0        0        0        0 2024-05-21 14:28:23.168757 slurpit_sdk-0.9.22/src/slurpit/apis/__init__.py
+-rw-r--r--   0        0        0     7758 2024-05-21 13:57:31.144522 slurpit_sdk-0.9.22/src/slurpit/apis/baseapi.py
+-rw-r--r--   0        0        0    11278 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/apis/deviceapi.py
+-rw-r--r--   0        0        0     4077 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/apis/planningapi.py
+-rw-r--r--   0        0        0     1182 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/apis/platformapi.py
+-rw-r--r--   0        0        0     7962 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/apis/scannerapi.py
+-rw-r--r--   0        0        0    14842 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/apis/scraperapi.py
+-rw-r--r--   0        0        0     8168 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/apis/templateapi.py
+-rw-r--r--   0        0        0     4847 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/apis/userapi.py
+-rw-r--r--   0        0        0     4441 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/apis/vaultapi.py
+-rw-r--r--   0        0        0        0 2024-05-21 14:28:23.172757 slurpit_sdk-0.9.22/src/slurpit/models/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/models/basemodel.py
+-rw-r--r--   0        0        0     2606 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/models/device.py
+-rw-r--r--   0        0        0     1301 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/models/planning.py
+-rw-r--r--   0        0        0      396 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/models/platform.py
+-rw-r--r--   0        0        0     2017 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/models/scanner.py
+-rw-r--r--   0        0        0     1932 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/models/template.py
+-rw-r--r--   0        0        0     2107 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/models/user.py
+-rw-r--r--   0        0        0     2738 2024-05-21 13:11:58.114837 slurpit_sdk-0.9.22/src/slurpit/models/vault.py
+-rw-r--r--   0        0        0     2209 1970-01-01 00:00:00.000000 slurpit_sdk-0.9.22/PKG-INFO
```

### Comparing `slurpit_sdk-0.9.20/LICENSE` & `slurpit_sdk-0.9.22/LICENSE`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.20/README.md` & `slurpit_sdk-0.9.22/README.md`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.20/src/slurpit/api.py` & `slurpit_sdk-0.9.22/src/slurpit/api.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.20/src/slurpit/apis/baseapi.py` & `slurpit_sdk-0.9.22/src/slurpit/apis/baseapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,21 +33,29 @@
             requests.exceptions.ConnectionError: If there was a network problem.
             requests.exceptions.HTTPError: If the HTTP request returned an error response.
             requests.exceptions.RequestException: If there was an ambiguous exception that occurred while handling your request.
         """
         try:
             response = self.session.get(url, **kwargs)  # Sends a GET request
             response.raise_for_status()  # Raises an exception for HTTP error codes
-        except (requests.exceptions.Timeout,
-                requests.exceptions.ConnectionError,
-                requests.exceptions.HTTPError,
-                requests.exceptions.RequestException) as e:
-            print(f"Error occurred: {e}")  # Optionally print or log the error
-            raise  # Re-raises the caught exception
-        return response
+            return response
+        except requests.exceptions.Timeout:
+            print("The request timed out")
+            raise
+        except requests.exceptions.ConnectionError:
+            print("Network problem (e.g., DNS failure, refused connection, etc)")
+            raise
+        except requests.exceptions.HTTPError as e:
+            error_message = e.response.json().get('messages', {}).get('error', 'No error message provided')
+            print(f"HTTP Error: {e}")
+            print(f"Error Message: {error_message}")
+            raise
+        except requests.exceptions.RequestException as e:
+            print(f"Request Error: {e}")
+            raise
     
     def post(self, url, data, **kwargs):
         """
         Sends a POST request with JSON data to the specified URL.
 
         Args:
             url (str): The URL to send the POST request to.
@@ -56,28 +64,30 @@
 
         Returns:
             requests.Response | None: The response object if the request was successful; otherwise, None.
         """
         try:
             response = self.session.post(url, json=data, **kwargs)  # Sends a POST request with JSON payload
             response.raise_for_status()
+            return response
         except requests.exceptions.Timeout:
             print("The request timed out")
             raise
         except requests.exceptions.ConnectionError:
             print("Network problem (e.g., DNS failure, refused connection, etc)")
             raise
         except requests.exceptions.HTTPError as e:
+            error_message = e.response.json().get('messages', {}).get('error', 'No error message provided')
             print(f"HTTP Error: {e}")
-            print(f"Error: {e.response.text}")
+            print(f"Error Message: {error_message}")
             raise
         except requests.exceptions.RequestException as e:
             print(f"Request Error: {e}")
             raise
-        return response
+
     
     def put(self, url, data, **kwargs):
         """
         Sends a PUT request with JSON data to the specified URL.
 
         Args:
             url (str): The URL to send the PUT request to.
@@ -86,28 +96,29 @@
 
         Returns:
             requests.Response | None: The response object if the request was successful; otherwise, None.
         """
         try:
             response = self.session.put(url, json=data, **kwargs)
             response.raise_for_status()
+            return response
         except requests.exceptions.Timeout:
             print("The request timed out")
             raise
         except requests.exceptions.ConnectionError:
             print("Network problem (e.g., DNS failure, refused connection, etc)")
             raise
         except requests.exceptions.HTTPError as e:
+            error_message = e.response.json().get('messages', {}).get('error', 'No error message provided')
             print(f"HTTP Error: {e}")
-            print(f"Error: {e.response.text}")
+            print(f"Error Message: {error_message}")
             raise
         except requests.exceptions.RequestException as e:
             print(f"Request Error: {e}")
             raise
-        return response
     
     def delete(self, url, **kwargs):
         """
         Sends a DELETE request to the specified URL.
 
         Args:
             url (str): The URL to send the DELETE request to.
@@ -115,28 +126,29 @@
 
         Returns:
             requests.Response | None: The response object if the request was successful; otherwise, None.
         """
         try:
             response = self.session.delete(url, **kwargs)
             response.raise_for_status()
+            return response
         except requests.exceptions.Timeout:
             print("The request timed out")
             raise
         except requests.exceptions.ConnectionError:
             print("Network problem (e.g., DNS failure, refused connection, etc)")
             raise
         except requests.exceptions.HTTPError as e:
+            error_message = e.response.json().get('messages', {}).get('error', 'No error message provided')
             print(f"HTTP Error: {e}")
-            print(f"Error: {e.response.text}")
+            print(f"Error Message: {error_message}")
             raise
         except requests.exceptions.RequestException as e:
             print(f"Request Error: {e}")
             raise
-        return response
 
 
     def json_to_csv_bytes(self, json_data):
         """
         Converts JSON data to CSV byte array.
 
         Args:
@@ -156,15 +168,15 @@
             # Convert DataFrame to CSV and save it to buffer
             df.to_csv(buffer, index=False)
             buffer.seek(0)  # Rewind the buffer to the beginning
             
             # Return bytes
             return buffer.getvalue()
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Data error while converting CSV file: {e}")
             raise
         
     
     def save_csv_bytes(self, byte_data, filename):
         """
         Saves CSV byte array data to a CSV file.
 
@@ -178,9 +190,9 @@
                 os.makedirs(directory)
                 
             # Open file in binary write mode and write byte data
             with open(filename, 'wb') as file:
                 file.write(byte_data)
             return True
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Data error while saving CSV file: {e}")
             raise
```

### Comparing `slurpit_sdk-0.9.20/src/slurpit/apis/deviceapi.py` & `slurpit_sdk-0.9.22/src/slurpit/apis/deviceapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(devices_data)
                 elif export_df:
                     return pd.DataFrame(devices_data)
                 else:
                     return [Device(**item) for item in devices_data]
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def get_device(self, device_id: int):
         """
         Fetches a single device by its ID.
 
         Args:
@@ -59,15 +59,15 @@
         url = f"{self.base_url}/devices/{device_id}"
         try:
             response = self.get(url)
             if response:
                 device_data = response.json()
                 return Device(**device_data)
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def update_device(self, device_id: int, update_data: dict):
         """
         Updates a specific device using its ID.
 
         Args:
@@ -80,15 +80,15 @@
         url = f"{self.base_url}/devices/{device_id}"
         try:
             response = self.put(url, update_data)
             if response:
                 device_data = response.json()
                 return Device(**device_data)
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def create_device(self, device_data: dict):
         """
         Creates a new device in the system.
 
         Args:
@@ -100,15 +100,15 @@
         url = f"{self.base_url}/devices"
         try:
             response = self.post(url, device_data)
             if response:
                 device_data = response.json()
                 return Device(**device_data)
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def delete_device(self, device_id: int):
         """
         Deletes a device using its ID.
 
         Args:
@@ -120,15 +120,15 @@
         url = f"{self.base_url}/devices/{device_id}"
         try:
             response = self.delete(url)
             if response:
                 device_data = response.json()
                 return Device(**device_data)
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def sync_device(self, sync_result: dict):
         """
         Synchronizes a device with the given device data. Insert or Update a new device with the provided data.
 
         Args:
@@ -145,15 +145,15 @@
                 sync_result = response.json()
                 if sync_result.get('success'):
                     print("Sync response:", )
                     raise Exception(f"Sync failed. {sync_result['success']}")
                 else:
                     return Device(**sync_result)
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def get_vendors(self, export_csv: bool = False, export_df: bool = False):
         """
         Retrieves a list of vendors from the API and optionally exports the data to a CSV format or pandas DataFrame.
         
         Args:
@@ -173,15 +173,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(vendors_data)
                 elif export_df:
                     return pd.DataFrame(vendors_data)
                 else:
                     return [Vendor(**item) for item in vendors_data]
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def get_types(self, export_csv: bool = False, export_df: bool = False):
         """
         Retrieves a list of device types from the API and optionally exports the data to CSV format or pandas DataFrame.
         
         Args:
@@ -201,15 +201,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(types_data)
                 elif export_df:
                     return pd.DataFrame(types_data)
                 else:
                     return types_data
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def get_snapshots(self, hostname: str, date: str = None, export_csv: bool = False, export_df: bool = False):
         """
         Retrieve latest data for a given hostname for all plannings, optionally filtered by date,
         and optionally exports the data to a CSV format or pandas DataFrame.
         
@@ -233,15 +233,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(snapshots_data)
                 elif export_df:
                     return pd.DataFrame(snapshots_data)
                 else:
                     return snapshots_data
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def get_snapshot(self, hostname: str, planning_id: int, date: str = None):
         """
         Retrieves latest data for a given hostname and planning id, optionally filtered by date.
 
         Args:
@@ -256,15 +256,15 @@
         params = {'date': date}
         try:
             response = self.get(url, params=params)
             if response:
                 snapshot_data = response.json()
                 return snapshot_data
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def test_ssh(self, ssh_info: dict):
         """
         Tests SSH connectivity using the provided SSH information.
 
         Args:
@@ -276,9 +276,9 @@
         url = f"{self.base_url}/devices/test/ssh"
         try:
             response = self.post(url, ssh_info)
             if response:
                 ssh_response = response.json()
                 return ssh_response
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
```

### Comparing `slurpit_sdk-0.9.20/src/slurpit/apis/planningapi.py` & `slurpit_sdk-0.9.22/src/slurpit/apis/planningapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(plannings_data)
                 elif export_df:
                     return pd.DataFrame(plannings_data)
                 else:
                     return [Planning(**item) for item in plannings_data]
         except Exception as e:
-            print(f"Value error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
 
     def search_plannings(self, search_data: dict, export_csv: bool = False, export_df: bool = False):
         """
         A more flexible way to search over the unique planning data and optionally exports the data to CSV format or pandas DataFrame.
 
@@ -66,15 +66,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(search_result)
                 elif export_df:
                     return pd.DataFrame(search_result)
                 else:
                     return search_result
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def regenerate_unique(self, planning_id: int):
         """
         Regenerates unique data for a planning entry based on the given ID. This is necessary when key attributes are changed and unique results need to be updated.
 
         Args:
@@ -89,9 +89,9 @@
         }
         try:
             response = self.post(url, planning_data)
             if response:
                 update_info = response.json()
                 return update_info
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
```

### Comparing `slurpit_sdk-0.9.20/src/slurpit/apis/platformapi.py` & `slurpit_sdk-0.9.22/src/slurpit/apis/platformapi.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,9 +24,9 @@
         url = f"{self.base_url}/platform/ping" 
         try:
             response = self.get(url)
             if response:
                 platform_data = response.json()  
                 return Platform(**platform_data)  
         except Exception as e:
-            print(f"Error retrieving platform data: {e}")  
+            print(f"Unexpected error: {e}")
             raise
```

### Comparing `slurpit_sdk-0.9.20/src/slurpit/apis/scannerapi.py` & `slurpit_sdk-0.9.22/src/slurpit/apis/scannerapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(nodes_data)
                 elif export_df:
                     return pd.DataFrame(nodes_data)
                 else:
                     return nodes_data
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def get_finders(self, export_csv: bool = False, export_df: bool = False):
         """
         Retrieves a list of configured finders from the scanner API and optionally exports the data to CSV format or pandas DataFrame.
 
         Args:
@@ -65,15 +65,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(finders_data)
                 elif export_df:
                     return pd.DataFrame(finders_data)
                 else:
                     return finders_data
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def get_crawlers(self, export_csv: bool = False, export_df: bool = False):
         """
         Retrieves a list of configured crawlers from the scanner API and optionally exports the data to CSV format or pandas DataFrame.
 
         Args:
@@ -92,15 +92,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(crawlers_data)
                 elif export_df:
                     return pd.DataFrame(crawlers_data)
                 else:
                     return crawlers_data
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def start_scanner(self, scanner_data: dict):
         """
         Starts a scanning process with provided scanner configuration data.
 
         Returns:
@@ -109,15 +109,15 @@
         url = f"{self.base_url}/scanner"
         try:
             response = self.post(url, scanner_data)
             if response:
                 scanner_status = response.json()
                 return scanner_status
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def clean_logging(self, datetime: str):
         """
         Triggers a cleaning process for scanner logs older than the specified datetime.
 
         Returns:
@@ -127,15 +127,15 @@
         request_data = {"datetime": datetime}
         try:
             response = self.post(url, request_data)
             if response:
                 clean_result = response.json()
                 return clean_result
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def get_status(self):
         """
         Retrieves the current status of the scanner.
 
         Returns:
@@ -144,15 +144,15 @@
         url = f"{self.base_url}/scanner/status"
         try:
             response = self.get(url)
             if response:
                 status_result = response.json()
                 return status_result
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def test_snmp(self, ip_data: dict):
         """
         Tests SNMP configuration by attempting to gather device information from the specified IP.
 
         Returns:
@@ -161,15 +161,15 @@
         url = f"{self.base_url}/scanner/test"
         try:
             response = self.post(url, ip_data)
             if response:
                 device_info = response.json()
                 return device_info
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def get_queue_list(self, export_csv: bool = False):
         """
         Gives a list of currently queued tasks for the scanner.
 
         Args:
@@ -184,15 +184,15 @@
             if response:
                 queue_list = response.json()
                 if export_csv:
                     return self.json_to_csv_bytes(queue_list)
                 else:
                     return queue_list
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
     
     def clear_queue(self):
         """
         Clears the queue of the scanner by sending a DELETE request to the queue list endpoint.
 
         Returns:
@@ -203,9 +203,9 @@
         try:
             response = self.delete(url)
             
             if response:
                 clear_result = response.json()
                 return clear_result
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
```

### Comparing `slurpit_sdk-0.9.20/src/slurpit/apis/scraperapi.py` & `slurpit_sdk-0.9.22/src/slurpit/apis/scraperapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(collected_data)
                 elif export_df:
                     return pd.DataFrame(collected_data)
                 else:
                     return collected_data
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def scrape_planning(self, planning_id: int, offset: int = 0, limit: int = 1000, export_csv: bool = False, export_df: bool = False):
         """
         Retrieve all unique data for a given planning ID from the scraper endpoint and optionally exports the data to CSV format or pandas DataFrame.
 
         Args:
@@ -68,15 +68,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(scraped_planning)
                 elif export_df:
                     return pd.DataFrame(scraped_planning)
                 else:
                     return scraped_planning
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def scrape_planning_ips(self, planning_id: int, date: str = None):
         """
         Retrieves IP addresses related to a specific planning ID and date from the scraper endpoint.
 
         Args:
@@ -90,15 +90,15 @@
         params = {'date': date}
         try:
             response = self.get(url, params=params)
             
             planning_ips = response.json()
             return planning_ips
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def scrape_planning_ipam(self, planning_id: int = None, date: str = None):
         """
         Retrieve all IPs for a given planning id new then given datetime value
 
         Args:
@@ -118,15 +118,15 @@
         params = {'date': date}
         try:
             response = self.get(url, params=params)
             
             planning_ipams = response.json()
             return planning_ipams
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     
     def scrape_planning_by_hostname(self, planning_id: int, hostname: str, offset: int = 0, limit: int = 1000, export_csv: bool = False, export_df: bool = False):
         """
         Retrieves all unique data for a specific planning ID and hostname from the scraper endpoint, optionally exporting the data to CSV or pandas DataFrame.
 
@@ -151,15 +151,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(scraped_planning)
                 elif export_df:
                     return pd.DataFrame(scraped_planning)
                 else:
                     return scraped_planning
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def scrape_device(self, hostname: str, offset: int = 0, limit: int = 1000, export_csv: bool = False, export_df: bool = False):
         """
         Retrieves scraped data for a specific hostname from the scraper endpoint, optionally exporting the data to CSV or pandas DataFrame.
 
         Args:
@@ -182,15 +182,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(scraped_data)
                 elif export_df:
                     return pd.DataFrame(scraped_data)
                 else:
                     return scraped_data
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def scrape_batches_latest(self, export_csv: bool = False, export_df: bool = False):
         """
         Retrieves the latest batch IDs and their corresponding planning IDs, optionally exporting the data to CSV or pandas DataFrame.
 
         Args:
@@ -209,15 +209,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(scraped_data)
                 elif export_df:
                     return pd.DataFrame(scraped_data)
                 else:
                     return scraped_data
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def scrape_batches(self, planning_id: int, hostname: str, export_csv: bool = False, export_df: bool = False):
         """
         Retrieves a list of all batch IDs and timestamps for the specified hostname and planning ID, optionally exporting the data to CSV or pandas DataFrame.
 
         Args:
@@ -238,15 +238,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(scraped_data)
                 elif export_df:
                     return pd.DataFrame(scraped_data)
                 else:
                     return scraped_data
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def start_scraper(self, scraper_info: dict):
         """
         Start the Data Collector
 
         Args:
@@ -258,15 +258,15 @@
         url = f"{self.base_url}/scraper"
         try:
             response = self.post(url, scraper_info)
             
             started_result = response.json()
             return started_result
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def clean_logs(self, datetime: str):
         """
         Cleans results and logging older than given datetime.
 
         Args:
@@ -281,15 +281,15 @@
         url = f"{self.base_url}/scraper/clean"
         try:
             response = self.post(url, request_data)
             
             clean_result = response.json()
             return clean_result
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def get_status(self):
         """
         Retrieves the status of the scraper.
 
         Returns:
@@ -298,15 +298,15 @@
         url = f"{self.base_url}/scraper/status"
         try:
             response = self.get(url)
             
             scraper_status = response.json()
             return scraper_status
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def get_queue_list(self, export_csv: bool = False, export_df: bool = False):
         """
         Gives a list of currently queued tasks for the scraper and optionally exports the data to CSV format or pandas DataFrame.
 
         Args:
@@ -325,15 +325,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(queue_list)
                 elif export_df:
                     return pd.DataFrame(queue_list)
                 else:
                     return queue_list
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def clear_queue(self):
         """
         Clears the queue of the scraper by sending a DELETE request to the queue list endpoint.
 
         Returns:
@@ -342,9 +342,9 @@
         url = f"{self.base_url}/scraper/queue/clear"
         try:
             response = self.delete(url)
             
             clear_result = response.json()
             return clear_result
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
```

### Comparing `slurpit_sdk-0.9.20/src/slurpit/apis/templateapi.py` & `slurpit_sdk-0.9.22/src/slurpit/apis/templateapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(templates_data)
                 elif export_df:
                     return pd.DataFrame(templates_data)
                 else:
                     return [Template(**item) for item in templates_data]
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def get_template(self, template_id: int):
         """
         Fetches a template by its ID from the API and returns it as an instance of the Template model.
         
         Args:
@@ -69,15 +69,15 @@
         """
         url = f"{self.base_url}/templates/{template_id}"
         try:
             response = self.get(url)
             
             return Template(**response.json())
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def update_template(self, template_id: int, update_data: dict):
         """
         Updates a template by its ID with the provided data.
         
         Args:
@@ -89,15 +89,15 @@
         """
         url = f"{self.base_url}/templates/{template_id}"
         try:
             response = self.put(url, update_data)
             
             return Template(**response.json())
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def delete_template(self, template_id: int):
         """
         Deletes a template by its ID.
         
         Args:
@@ -108,15 +108,15 @@
         """
         url = f"{self.base_url}/templates/{template_id}"
         try:
             response = self.delete(url)
             
             return Template(**response.json())
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def create_template(self, new_template: dict):
         """
         Creates a new template with the provided data.
         
         Args:
@@ -127,15 +127,15 @@
         """
         url = f"{self.base_url}/templates"
         try:
             response = self.post(url, new_template)
             
             return Template(**response.json())
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     
     def search_template(self, search_data: dict, export_csv: bool = False, export_df: bool = False):
         """
         Searches for templates based on the provided search criteria and optionally exports the data to a CSV format or pandas DataFrame.
         
@@ -156,15 +156,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(templates_data)
                 elif export_df:
                     return pd.DataFrame(templates_data)
                 else:
                     return [Template(**item) for item in templates_data]
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def run_template(self, run_info: dict):
         """
         Get realtime parsed and raw results from a device.
 
         Args:
@@ -175,15 +175,15 @@
         """
         url = f"{self.base_url}/templates/run"
         try:
             response = self.post(url, run_info)
             
             return response.json()
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def validate_textfsm(self, textfsm: str):
         """
         Validates if the textFSM has validation/syntax errors.
 
         Args:
@@ -195,15 +195,15 @@
         request_data = {"textfsm": textfsm}
         url = f"{self.base_url}/templates/validate"
         try:
             response = self.post(url, request_data)
             
             return response.json()
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def test_textfsm(self, test_data: dict):
         """
         Tests the TextFSM template against a device.
         
         Args:
@@ -214,9 +214,9 @@
         """
         url = f"{self.base_url}/templates/test"
         try:
             response = self.post(url, test_data)
             
             return response.json()
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
```

### Comparing `slurpit_sdk-0.9.20/src/slurpit/apis/userapi.py` & `slurpit_sdk-0.9.22/src/slurpit/apis/userapi.py`

 * *Files 16% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         url = f"{self.base_url}/users/{user_id}"
         try:
             response = self.get(url)
             
             user_data = response.json()
             return User(**user_data)
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def update_user(self, user_id: int, update_data: dict):
         """
         Updates a user's information on the server.
 
         Args:
@@ -88,15 +88,15 @@
         try:
             response = self.put(url, update_data)
             
             user_data = response.json()
             print("User updated successfully")
             return User(**user_data)
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def create_user(self, new_user: dict):
         """
         Creates a new user in the system.
 
         Args:
@@ -108,15 +108,15 @@
         url = f"{self.base_url}/users"
         try:
             response = self.post(url, new_user)
             user_data = response.json()
             print("User created successfully")
             return User(**user_data)
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
 
     def delete_user(self, user_id: int):
         """
         Deletes a user from the system by user ID.
 
         Args:
@@ -128,9 +128,9 @@
         url = f"{self.base_url}/users/{user_id}"
         try:
             response = self.delete(url)
             user_data = response.json()
             print("User deleted successfully")
             return User(**user_data)
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
```

### Comparing `slurpit_sdk-0.9.20/src/slurpit/apis/vaultapi.py` & `slurpit_sdk-0.9.22/src/slurpit/apis/vaultapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                 if export_csv:
                     return self.json_to_csv_bytes(vaults_data)
                 elif export_df:
                     return pd.DataFrame(vaults_data)
                 else:
                     return [Vault(**item) for item in vaults_data]
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
         
     def get_vault(self, vault_id: int):
         """
         Fetches a single vault by its ID.
 
         Args:
@@ -55,15 +55,15 @@
         url = f"{self.base_url}/vault/{vault_id}"
         try:
             response = self.get(url)
             if response:
                 vault_data = response.json()
                 return SingleVault(**vault_data)
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
     
     def update_vault(self, vault_id: int, update_data: dict):
         """
         Updates a vault with specified data.
 
         Args:
@@ -77,15 +77,15 @@
         try:
             response = self.put(url, update_data)
             if response:
                 vault_data = response.json()
                 print("vault_data", vault_data)
                 return SingleVault(**vault_data)
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
     
     def create_vault(self, new_vault: dict):
         """
         Creates a new vault with the specified data.
 
         Args:
@@ -98,15 +98,15 @@
         try:
             response = self.post(url, new_vault)
             if response:
                 vault_data = response.json()
                 print("new data", vault_data)
                 return SingleVault(**vault_data)
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
     
     def delete_vault(self, vault_id: int):
         """
         Deletes a vault by its ID.
 
         Args:
@@ -119,9 +119,9 @@
         try:
             response = self.delete(url)
             if response:
                 vault_data = response.json()
                 print("new data", vault_data)
                 return SingleVault(**vault_data)
         except Exception as e:
-            print(f"Response error: {e}")
+            print(f"Unexpected error: {e}")
             raise
```

### Comparing `slurpit_sdk-0.9.20/src/slurpit/models/device.py` & `slurpit_sdk-0.9.22/src/slurpit/models/device.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.20/src/slurpit/models/planning.py` & `slurpit_sdk-0.9.22/src/slurpit/models/planning.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.20/src/slurpit/models/scanner.py` & `slurpit_sdk-0.9.22/src/slurpit/models/scanner.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.20/src/slurpit/models/template.py` & `slurpit_sdk-0.9.22/src/slurpit/models/template.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.20/src/slurpit/models/user.py` & `slurpit_sdk-0.9.22/src/slurpit/models/user.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.20/src/slurpit/models/vault.py` & `slurpit_sdk-0.9.22/src/slurpit/models/vault.py`

 * *Files identical despite different names*

### Comparing `slurpit_sdk-0.9.20/PKG-INFO` & `slurpit_sdk-0.9.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurpit_sdk
-Version: 0.9.20
+Version: 0.9.22
 Summary: A robust Python SDK for slurpit
 Author: Slurp'it
 Author-email: info@slurpit.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

