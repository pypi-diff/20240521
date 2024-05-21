# Comparing `tmp/bioturing_connector-1.8.0.tar.gz` & `tmp/bioturing_connector-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioturing_connector-1.8.0.tar", max compression
+gzip compressed data, was "bioturing_connector-1.9.0.tar", max compression
```

## Comparing `bioturing_connector-1.8.0.tar` & `bioturing_connector-1.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      359 2024-01-22 05:58:48.195299 bioturing_connector-1.8.0/README.md
--rw-r--r--   0        0        0      299 2024-03-15 08:26:55.476364 bioturing_connector-1.8.0/bioturing_connector/__init__.py
--rw-r--r--   0        0        0    23448 2024-03-15 08:26:55.476364 bioturing_connector-1.8.0/bioturing_connector/bbrowserx_connector.py
--rw-r--r--   0        0        0      453 2024-01-18 05:43:58.078051 bioturing_connector-1.8.0/bioturing_connector/common/__init__.py
--rw-r--r--   0        0        0     2935 2024-01-18 06:33:21.567020 bioturing_connector-1.8.0/bioturing_connector/common/common.py
--rw-r--r--   0        0        0       16 2024-03-15 08:26:55.476364 bioturing_connector-1.8.0/bioturing_connector/common/constants.py
--rw-r--r--   0        0        0     2016 2024-02-28 07:20:24.738281 bioturing_connector-1.8.0/bioturing_connector/common/https_agent.py
--rw-r--r--   0        0        0    26944 2024-03-15 08:26:55.476364 bioturing_connector-1.8.0/bioturing_connector/connector.py
--rw-r--r--   0        0        0    14617 2024-01-18 05:43:58.078051 bioturing_connector-1.8.0/bioturing_connector/lens_bulk_connector.py
--rw-r--r--   0        0        0    25947 2024-01-18 05:43:58.078051 bioturing_connector-1.8.0/bioturing_connector/lens_sc_connector.py
--rw-r--r--   0        0        0     1837 2024-03-15 08:26:55.476364 bioturing_connector-1.8.0/bioturing_connector/typing/__init__.py
--rw-r--r--   0        0        0      525 2024-03-15 08:26:55.476364 bioturing_connector-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 bioturing_connector-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      359 2024-03-12 03:29:03.485486 bioturing_connector-1.9.0/README.md
+-rw-r--r--   0        0        0      299 2024-05-20 04:41:06.137549 bioturing_connector-1.9.0/bioturing_connector/__init__.py
+-rw-r--r--   0        0        0    23448 2024-03-14 09:22:37.032097 bioturing_connector-1.9.0/bioturing_connector/bbrowserx_connector.py
+-rw-r--r--   0        0        0      453 2024-03-12 03:29:03.485486 bioturing_connector-1.9.0/bioturing_connector/common/__init__.py
+-rw-r--r--   0        0        0     2935 2024-05-20 01:33:59.237924 bioturing_connector-1.9.0/bioturing_connector/common/common.py
+-rw-r--r--   0        0        0       16 2024-03-14 09:22:37.032097 bioturing_connector-1.9.0/bioturing_connector/common/constants.py
+-rw-r--r--   0        0        0     2016 2024-05-20 01:53:13.390636 bioturing_connector-1.9.0/bioturing_connector/common/https_agent.py
+-rw-r--r--   0        0        0    32724 2024-05-20 10:14:57.609699 bioturing_connector-1.9.0/bioturing_connector/connector.py
+-rw-r--r--   0        0        0    14617 2024-03-12 03:29:03.485486 bioturing_connector-1.9.0/bioturing_connector/lens_bulk_connector.py
+-rw-r--r--   0        0        0    25947 2024-03-12 03:29:03.485486 bioturing_connector-1.9.0/bioturing_connector/lens_sc_connector.py
+-rw-r--r--   0        0        0     1837 2024-03-14 09:22:37.032097 bioturing_connector-1.9.0/bioturing_connector/typing/__init__.py
+-rw-r--r--   0        0        0      525 2024-05-20 04:40:52.777031 bioturing_connector-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 bioturing_connector-1.9.0/PKG-INFO
```

### Comparing `bioturing_connector-1.8.0/bioturing_connector/bbrowserx_connector.py` & `bioturing_connector-1.9.0/bioturing_connector/bbrowserx_connector.py`

 * *Files identical despite different names*

### Comparing `bioturing_connector-1.8.0/bioturing_connector/common/common.py` & `bioturing_connector-1.9.0/bioturing_connector/common/common.py`

 * *Files identical despite different names*

### Comparing `bioturing_connector-1.8.0/bioturing_connector/common/https_agent.py` & `bioturing_connector-1.9.0/bioturing_connector/common/https_agent.py`

 * *Files identical despite different names*

### Comparing `bioturing_connector-1.8.0/bioturing_connector/connector.py` & `bioturing_connector-1.9.0/bioturing_connector/connector.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 from pathlib import Path
 
 from .common import common
 from .common import get_uuid
 from .common import decode_base64_array
 from .common.https_agent import HttpsAgent
 from .typing import StudyUnit
+from .typing import Species
+from .typing import StudyType
+from .typing import ChunkSize
 
 
 class Connector(object):
   """
   Shared functions of all platforms
   """
 
@@ -978,8 +981,183 @@
       'leaf_id': leaf_id,
     }
     result = self.post_request(
       api_route='api/v1/study/assign_standardized_term',
       data=data
     )
     common.check_result_status(result)
-    return 'Successul'
+    return 'Successul'
+
+  def get_export_log(self, group_id: str, task_id: str):
+    last_status = []
+    while True:
+      export_log = self.post_request(
+        api_route='api/v1/get_submission_log',
+        data={'task_id': task_id},
+        check_error=False
+      )
+      message = self._get_error_message(export_log)
+      if message:
+        print(message)
+        break
+
+      current_status = export_log['data']['log'].split('\n')[:-1]
+      new_status = current_status[len(last_status):]
+      if len(new_status):
+        print('\n'.join(new_status))
+
+      last_status += new_status
+      if export_log['data']['status'] != 'SUCCESS':
+        time.sleep(5)
+        continue
+      else:
+        res = self.post_request(
+          api_route='api/v1/get_export_result',
+          data={
+            'group_id': group_id,
+            'task_id': task_id
+          },
+          check_error=False
+        )
+        message = self._get_error_message(res)
+        if message:
+          print(message)
+          break
+        else:
+          return {
+            'status': True,
+            'data': {
+              'url': urljoin(self.__host, res['data']['file_path'].lstrip('/')),
+              'file_name': res['data']['file_name']
+            }
+          }
+    return False
+
+  def get_download_study_url(
+      self,
+      group_id,
+      study_id,
+      study_type = StudyType.H5AD.value,
+      species = Species.HUMAN.value,
+    ):
+    """
+    Get the url of an exported study.
+
+    Parameters
+    ----------
+    group_id : str
+          ID of the group to which the study belongs.
+    study_id : str
+          The UUID of the study to be downloaded.
+    study_type : str, optional
+          Format of the study. Default: bioturing_connector.typing.StudyType.H5AD.value\n
+          Support:
+                bioturing_connector.typing.StudyType.H5AD.value\n
+                bioturing_connector.typing.StudyType.RDS.value\n
+    species : str, optional
+          Species of the study. Default: 'human'\n
+          Support:
+                bioturing_connector.typing.Species.HUMAN.value\n
+                bioturing_connector.typing.Species.MOUSE.value\n
+                bioturing_connector.typing.Species.NON_HUMAN_PRIMATE.value\n
+                bioturing_connector.typing.Species.OTHERS.value\n
+    dest_path : str, optional
+          The destination file path to save the downloaded study.
+          If not provided, the default file name from the response will be used.
+
+    Returns
+    -------
+    Submission status : bool | str
+      True or Error log
+    """
+    data = {
+      'species': species,
+      'group_id': group_id,
+      'study_id': study_id,
+      'context': [],
+      'study_type': study_type,
+    }
+    export_status = self.post_request(
+      api_route='api/v1/export_study',
+      data=data,
+    )
+    task_id = common.parse_submission_status(export_status)
+    if task_id is None:
+      return False
+
+    res = self.get_export_log(
+      group_id=group_id,
+      task_id=task_id,
+    )
+    return res if res else False
+
+  def download_study(
+      self,
+      group_id,
+      study_id,
+      study_type = StudyType.H5AD.value,
+      species = Species.HUMAN.value,
+      dest_path = None,
+      chunk_size = ChunkSize.CHUNK_100_MB.value,
+    ):
+    """
+    Download a private study.
+
+    Parameters
+    ----------
+    group_id : str
+          ID of the group to which the study belongs.
+    study_id : str
+          The UUID of the study to be downloaded.
+    study_type : str, optional
+          Format of the study. Default: bioturing_connector.typing.StudyType.H5AD.value\n
+          Support:
+                bioturing_connector.typing.StudyType.H5AD.value\n
+                bioturing_connector.typing.StudyType.RDS.value\n
+    species : str, optional
+          Species of the study. Default: 'human'\n
+          Support:
+                bioturing_connector.typing.Species.HUMAN.value\n
+                bioturing_connector.typing.Species.MOUSE.value\n
+                bioturing_connector.typing.Species.NON_HUMAN_PRIMATE.value\n
+                bioturing_connector.typing.Species.OTHERS.value\n
+    dest_path : str, optional
+          The destination file path to save the downloaded study.
+          If not provided, the default file name from the response will be used.
+    chunk_size : bioturing_connector.typing.ChunkSize, optional
+          Size of each separated chunk for uploading. Default: 104857600\n
+          Support:
+                bioturing_connector.typing.ChunkSize.CHUNK_5_MB.value\n
+                bioturing_connector.typing.ChunkSize.CHUNK_100_MB.value\n
+                bioturing_connector.typing.ChunkSize.CHUNK_500_MB.value\n
+                bioturing_connector.typing.ChunkSize.CHUNK_1_GB.value\n
+
+    Returns
+    -------
+    Submission status : bool | str
+      True or Error log
+    """
+    res = self.get_download_study_url(group_id, study_id, study_type, species)
+    if not res:
+      return res
+    url = res['data']['url']
+    dest_path = dest_path or res['data']['file_name']
+    print('Downloading')
+    response = requests.get(url, timeout=3600, stream=True)
+    if response.status_code == 200:
+      total_size = int(response.headers.get('content-length', 0))
+      with open(dest_path, 'wb') as f, tqdm(
+          desc=os.path.basename(dest_path),
+          total=total_size,
+          unit='iB',
+          unit_scale=True,
+          unit_divisor=1024,
+        ) as progress:
+        for chunk in response.iter_content(chunk_size=chunk_size):
+          if not chunk:
+            return False
+          f.write(chunk)
+          progress.update(len(chunk))
+      print('DONE!')
+      return True
+    print('Failed to download', url)
+    return False
```

### Comparing `bioturing_connector-1.8.0/bioturing_connector/lens_bulk_connector.py` & `bioturing_connector-1.9.0/bioturing_connector/lens_bulk_connector.py`

 * *Files identical despite different names*

### Comparing `bioturing_connector-1.8.0/bioturing_connector/lens_sc_connector.py` & `bioturing_connector-1.9.0/bioturing_connector/lens_sc_connector.py`

 * *Files identical despite different names*

### Comparing `bioturing_connector-1.8.0/bioturing_connector/typing/__init__.py` & `bioturing_connector-1.9.0/bioturing_connector/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `bioturing_connector-1.8.0/pyproject.toml` & `bioturing_connector-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bioturing-connector"
-version = "1.8.0"
+version = "1.9.0"
 description = "A set of python modules for accessing Bioturing's services on private server"
 authors = ["BioTuring <support@bioturing.com>"]
 readme = "README.md"
 packages = [{include = "bioturing_connector"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `bioturing_connector-1.8.0/PKG-INFO` & `bioturing_connector-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioturing-connector
-Version: 1.8.0
+Version: 1.9.0
 Summary: A set of python modules for accessing Bioturing's services on private server
 Author: BioTuring
 Author-email: support@bioturing.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

