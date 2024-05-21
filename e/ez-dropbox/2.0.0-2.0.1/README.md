# Comparing `tmp/ez-dropbox-2.0.0.tar.gz` & `tmp/ez-dropbox-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-dropbox-2.0.0.tar", last modified: Tue May 21 18:28:54 2024, max compression
+gzip compressed data, was "ez-dropbox-2.0.1.tar", last modified: Tue May 21 19:10:40 2024, max compression
```

## Comparing `ez-dropbox-2.0.0.tar` & `ez-dropbox-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:28:54.306918 ez-dropbox-2.0.0/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-12 12:48:02.000000 ez-dropbox-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3197 2024-05-21 18:28:54.306656 ez-dropbox-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2935 2024-05-12 12:48:02.000000 ez-dropbox-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:28:54.304244 ez-dropbox-2.0.0/ez_dropbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3197 2024-05-21 18:28:54.000000 ez-dropbox-2.0.0/ez_dropbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2024-05-21 18:28:54.000000 ez-dropbox-2.0.0/ez_dropbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 18:28:54.000000 ez-dropbox-2.0.0/ez_dropbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-21 18:28:54.000000 ez-dropbox-2.0.0/ez_dropbox.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-21 18:28:54.000000 ez-dropbox-2.0.0/ez_dropbox.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:28:54.305806 ez-dropbox-2.0.0/ezdbx/
--rw-r--r--   0 root         (0) root         (0)      117 2024-05-12 12:48:02.000000 ez-dropbox-2.0.0/ezdbx/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18948 2024-05-21 18:25:05.000000 ez-dropbox-2.0.0/ezdbx/main.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 18:28:54.307118 ez-dropbox-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      888 2024-05-15 10:09:33.000000 ez-dropbox-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:10:40.200416 ez-dropbox-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-12 12:48:02.000000 ez-dropbox-2.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5000 2024-05-21 19:10:40.200121 ez-dropbox-2.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4738 2024-05-21 19:09:21.000000 ez-dropbox-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:10:40.197597 ez-dropbox-2.0.1/ez_dropbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5000 2024-05-21 19:10:40.000000 ez-dropbox-2.0.1/ez_dropbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2024-05-21 19:10:40.000000 ez-dropbox-2.0.1/ez_dropbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 19:10:40.000000 ez-dropbox-2.0.1/ez_dropbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-21 19:10:40.000000 ez-dropbox-2.0.1/ez_dropbox.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-21 19:10:40.000000 ez-dropbox-2.0.1/ez_dropbox.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:10:40.199144 ez-dropbox-2.0.1/ezdbx/
+-rw-r--r--   0 root         (0) root         (0)      117 2024-05-12 12:48:02.000000 ez-dropbox-2.0.1/ezdbx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19582 2024-05-21 19:04:02.000000 ez-dropbox-2.0.1/ezdbx/main.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 19:10:40.200605 ez-dropbox-2.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      888 2024-05-21 19:02:48.000000 ez-dropbox-2.0.1/setup.py
```

### Comparing `ez-dropbox-2.0.0/LICENSE` & `ez-dropbox-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ez-dropbox-2.0.0/ezdbx/main.py` & `ez-dropbox-2.0.1/ezdbx/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import dropbox
 import requests
 import joblib
 from tqdm import tqdm
 from datetime import datetime
+import zipfile
 
 # Issuance of access token. (アクセストークンの発行)
 def issue_access_token(APP_KEY, APP_SECRET):
     """
     発行したアクセストークンを返します。
     :param APP_KEY: Dropbox APIのアプリキー
     :param APP_SECRET: Dropbox APIのアプリシークレット
@@ -193,16 +194,28 @@
         local_files = self._list_local_files(local_folder)
         dropbox_files, dropbox_folders = self._list_dropbox_files_and_folders(dropbox_folder, 'file')
 
         for local_file in local_files:
             relative_path = os.path.relpath(local_file, local_folder)
             dropbox_path = os.path.join(dropbox_folder, relative_path).replace(os.sep, '/')
 
-            if dropbox_path in dropbox_files:
+            try:
+                # ファイルの最終更新日時を取得
                 local_mod_time = datetime.fromtimestamp(os.path.getmtime(local_file))
+            except OSError as e:
+                # ファイルを開けない場合はZIPアーカイブに圧縮してアップロード
+                print(f'Compressing file {local_file} due to error: {e}')
+                zip_path = local_file + '.zip'
+                with zipfile.ZipFile(zip_path, 'w') as zipf:
+                    zipf.write(local_file, os.path.basename(local_file))
+                self.upload(zip_path, os.path.dirname(dropbox_path), overwrite=True)
+                os.remove(zip_path)
+                continue
+
+            if dropbox_path in dropbox_files:
                 dropbox_mod_time = dropbox_files[dropbox_path]
                 if local_mod_time > dropbox_mod_time:
                     self.upload(local_file, os.path.dirname(dropbox_path), overwrite=True)
             else:
                 self.upload(local_file, os.path.dirname(dropbox_path), overwrite=True)
 
     def read_sync(self, local_folder, dropbox_folder):
```

### Comparing `ez-dropbox-2.0.0/setup.py` & `ez-dropbox-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 packages = [
     'ezdbx'
 ]
 
 setup(
     name='ez-dropbox',
-    version='2.0.0',
+    version='2.0.1',
     license="MIT License",
     description="You can easily operate Dropbox!",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='TorDataScientist',
     url='https://github.com/TorDataScientist/ez-dropbox',
     packages=packages,
```

