# Comparing `tmp/ez-dropbox-2.0.1.tar.gz` & `tmp/ez-dropbox-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-dropbox-2.0.1.tar", last modified: Tue May 21 19:10:40 2024, max compression
+gzip compressed data, was "ez-dropbox-2.0.2.tar", last modified: Tue May 21 19:22:58 2024, max compression
```

## Comparing `ez-dropbox-2.0.1.tar` & `ez-dropbox-2.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:10:40.200416 ez-dropbox-2.0.1/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-12 12:48:02.000000 ez-dropbox-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5000 2024-05-21 19:10:40.200121 ez-dropbox-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4738 2024-05-21 19:09:21.000000 ez-dropbox-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:10:40.197597 ez-dropbox-2.0.1/ez_dropbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5000 2024-05-21 19:10:40.000000 ez-dropbox-2.0.1/ez_dropbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2024-05-21 19:10:40.000000 ez-dropbox-2.0.1/ez_dropbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 19:10:40.000000 ez-dropbox-2.0.1/ez_dropbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-21 19:10:40.000000 ez-dropbox-2.0.1/ez_dropbox.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-21 19:10:40.000000 ez-dropbox-2.0.1/ez_dropbox.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:10:40.199144 ez-dropbox-2.0.1/ezdbx/
--rw-r--r--   0 root         (0) root         (0)      117 2024-05-12 12:48:02.000000 ez-dropbox-2.0.1/ezdbx/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19582 2024-05-21 19:04:02.000000 ez-dropbox-2.0.1/ezdbx/main.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 19:10:40.200605 ez-dropbox-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      888 2024-05-21 19:02:48.000000 ez-dropbox-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:22:58.716215 ez-dropbox-2.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-12 12:48:02.000000 ez-dropbox-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5000 2024-05-21 19:22:58.715947 ez-dropbox-2.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4738 2024-05-21 19:09:21.000000 ez-dropbox-2.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:22:58.713641 ez-dropbox-2.0.2/ez_dropbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5000 2024-05-21 19:22:58.000000 ez-dropbox-2.0.2/ez_dropbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2024-05-21 19:22:58.000000 ez-dropbox-2.0.2/ez_dropbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 19:22:58.000000 ez-dropbox-2.0.2/ez_dropbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-21 19:22:58.000000 ez-dropbox-2.0.2/ez_dropbox.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-21 19:22:58.000000 ez-dropbox-2.0.2/ez_dropbox.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:22:58.715038 ez-dropbox-2.0.2/ezdbx/
+-rw-r--r--   0 root         (0) root         (0)      117 2024-05-12 12:48:02.000000 ez-dropbox-2.0.2/ezdbx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19854 2024-05-21 19:19:47.000000 ez-dropbox-2.0.2/ezdbx/main.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 19:22:58.716410 ez-dropbox-2.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      888 2024-05-21 19:20:14.000000 ez-dropbox-2.0.2/setup.py
```

### Comparing `ez-dropbox-2.0.1/LICENSE` & `ez-dropbox-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ez-dropbox-2.0.1/PKG-INFO` & `ez-dropbox-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-dropbox
-Version: 2.0.1
+Version: 2.0.2
 Summary: You can easily operate Dropbox!
 Home-page: https://github.com/TorDataScientist/ez-dropbox
 Author: TorDataScientist
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ez-dropbox-2.0.1/README.md` & `ez-dropbox-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ez-dropbox-2.0.1/ez_dropbox.egg-info/PKG-INFO` & `ez-dropbox-2.0.2/ez_dropbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-dropbox
-Version: 2.0.1
+Version: 2.0.2
 Summary: You can easily operate Dropbox!
 Home-page: https://github.com/TorDataScientist/ez-dropbox
 Author: TorDataScientist
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ez-dropbox-2.0.1/ezdbx/main.py` & `ez-dropbox-2.0.2/ezdbx/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,32 +195,27 @@
         dropbox_files, dropbox_folders = self._list_dropbox_files_and_folders(dropbox_folder, 'file')
 
         for local_file in local_files:
             relative_path = os.path.relpath(local_file, local_folder)
             dropbox_path = os.path.join(dropbox_folder, relative_path).replace(os.sep, '/')
 
             try:
-                # ファイルの最終更新日時を取得
                 local_mod_time = datetime.fromtimestamp(os.path.getmtime(local_file))
-            except OSError as e:
-                # ファイルを開けない場合はZIPアーカイブに圧縮してアップロード
-                print(f'Compressing file {local_file} due to error: {e}')
-                zip_path = local_file + '.zip'
-                with zipfile.ZipFile(zip_path, 'w') as zipf:
-                    zipf.write(local_file, os.path.basename(local_file))
-                self.upload(zip_path, os.path.dirname(dropbox_path), overwrite=True)
-                os.remove(zip_path)
-                continue
+            except OSError:
+                local_mod_time = None
 
             if dropbox_path in dropbox_files:
                 dropbox_mod_time = dropbox_files[dropbox_path]
                 if local_mod_time > dropbox_mod_time:
                     self.upload(local_file, os.path.dirname(dropbox_path), overwrite=True)
             else:
-                self.upload(local_file, os.path.dirname(dropbox_path), overwrite=True)
+                if local_mod_time is None:
+                    self._handle_unsupported_file(local_file, dropbox_path)
+                else:
+                    self.upload(local_file, os.path.dirname(dropbox_path), overwrite=True)
 
     def read_sync(self, local_folder, dropbox_folder):
         """
         Dropboxフォルダの内容をローカルフォルダに同期します。
         :param local_folder: ローカルフォルダのパス
         :param dropbox_folder: Dropboxフォルダのパス
         """
@@ -404,30 +399,42 @@
     def _upload_file(self, upload_file, upload_path, use_full_path):
         """
         ファイルをアップロードします。
         :param upload_file: アップロードするファイルのパス
         :param upload_path: アップロード先のパス
         :param use_full_path: フルパスを使用するかどうか
         """
-        with open(upload_file, "rb") as f:
-            file_size = os.path.getsize(upload_file)
-            print(f'{upload_file} : {file_size} byte')
-            chunk_size = 100 * 1024 * 1024
-            if file_size <= chunk_size:
-                if use_full_path:
-                    db_upload_path = os.path.join(upload_path, upload_file.replace(os.sep, '/'))
+        try:
+            with open(upload_file, "rb") as f:
+                file_size = os.path.getsize(upload_file)
+                print(f'{upload_file} : {file_size} byte')
+                chunk_size = 100 * 1024 * 1024
+                if file_size <= chunk_size:
+                    if use_full_path:
+                        db_upload_path = os.path.join(upload_path, upload_file.replace(os.sep, '/'))
+                    else:
+                        db_upload_path = os.path.join(upload_path, os.path.basename(upload_file))
+                    self.dbx.files_upload(f.read(), db_upload_path, mode=dropbox.files.WriteMode('overwrite'))
                 else:
-                    db_upload_path = os.path.join(upload_path, os.path.basename(upload_file))
-                self.dbx.files_upload(f.read(), db_upload_path, mode=dropbox.files.WriteMode('overwrite'))
-            else:
-                with tqdm(total=file_size, desc="Uploaded") as pbar:
-                    upload_session_start_result = self.dbx.files_upload_session_start(f.read(chunk_size))
-                    pbar.update(chunk_size)
-                    cursor = dropbox.files.UploadSessionCursor(session_id=upload_session_start_result.session_id, offset=f.tell())
-                    commit = dropbox.files.CommitInfo(path=os.path.join(upload_path, os.path.basename(upload_file)), mode=dropbox.files.WriteMode('overwrite'))
-                    while f.tell() < file_size:
-                        if (file_size - f.tell()) <= chunk_size:
-                            self.dbx.files_upload_session_finish(f.read(chunk_size), cursor, commit)
-                        else:
-                            self.dbx.files_upload_session_append(f.read(chunk_size), cursor.session_id, cursor.offset)
-                            cursor.offset = f.tell()
+                    with tqdm(total=file_size, desc="Uploaded") as pbar:
+                        upload_session_start_result = self.dbx.files_upload_session_start(f.read(chunk_size))
                         pbar.update(chunk_size)
+                        cursor = dropbox.files.UploadSessionCursor(session_id=upload_session_start_result.session_id, offset=f.tell())
+                        commit = dropbox.files.CommitInfo(path=os.path.join(upload_path, os.path.basename(upload_file)), mode=dropbox.files.WriteMode('overwrite'))
+                        while f.tell() < file_size:
+                            if (file_size - f.tell()) <= chunk_size:
+                                self.dbx.files_upload_session_finish(f.read(chunk_size), cursor, commit)
+                            else:
+                                self.dbx.files_upload_session_append(f.read(chunk_size), cursor.session_id, cursor.offset)
+                                cursor.offset = f.tell()
+                            pbar.update(chunk_size)
+        except OSError as e:
+            print(f'Error uploading file {upload_file}: {e}')
+            self._handle_unsupported_file(upload_file, os.path.join(upload_path, os.path.basename(upload_file)))
+
+                        
+    def _handle_unsupported_file(self, local_file, dropbox_path):
+        zip_path = local_file + '.zip'
+        with zipfile.ZipFile(zip_path, 'w') as zipf:
+            zipf.write(local_file, os.path.basename(local_file))
+        self.upload(zip_path, os.path.dirname(dropbox_path), overwrite=True)
+        os.remove(zip_path)
```

### Comparing `ez-dropbox-2.0.1/setup.py` & `ez-dropbox-2.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 packages = [
     'ezdbx'
 ]
 
 setup(
     name='ez-dropbox',
-    version='2.0.1',
+    version='2.0.2',
     license="MIT License",
     description="You can easily operate Dropbox!",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='TorDataScientist',
     url='https://github.com/TorDataScientist/ez-dropbox',
     packages=packages,
```

