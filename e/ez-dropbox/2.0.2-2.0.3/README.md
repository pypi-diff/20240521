# Comparing `tmp/ez-dropbox-2.0.2.tar.gz` & `tmp/ez-dropbox-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-dropbox-2.0.2.tar", last modified: Tue May 21 19:22:58 2024, max compression
+gzip compressed data, was "ez-dropbox-2.0.3.tar", last modified: Tue May 21 19:45:31 2024, max compression
```

## Comparing `ez-dropbox-2.0.2.tar` & `ez-dropbox-2.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:22:58.716215 ez-dropbox-2.0.2/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-12 12:48:02.000000 ez-dropbox-2.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5000 2024-05-21 19:22:58.715947 ez-dropbox-2.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4738 2024-05-21 19:09:21.000000 ez-dropbox-2.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:22:58.713641 ez-dropbox-2.0.2/ez_dropbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5000 2024-05-21 19:22:58.000000 ez-dropbox-2.0.2/ez_dropbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2024-05-21 19:22:58.000000 ez-dropbox-2.0.2/ez_dropbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 19:22:58.000000 ez-dropbox-2.0.2/ez_dropbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-21 19:22:58.000000 ez-dropbox-2.0.2/ez_dropbox.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-21 19:22:58.000000 ez-dropbox-2.0.2/ez_dropbox.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:22:58.715038 ez-dropbox-2.0.2/ezdbx/
--rw-r--r--   0 root         (0) root         (0)      117 2024-05-12 12:48:02.000000 ez-dropbox-2.0.2/ezdbx/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19854 2024-05-21 19:19:47.000000 ez-dropbox-2.0.2/ezdbx/main.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 19:22:58.716410 ez-dropbox-2.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      888 2024-05-21 19:20:14.000000 ez-dropbox-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:45:31.001172 ez-dropbox-2.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-12 12:48:02.000000 ez-dropbox-2.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5000 2024-05-21 19:45:31.000877 ez-dropbox-2.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4738 2024-05-21 19:09:21.000000 ez-dropbox-2.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:45:30.998294 ez-dropbox-2.0.3/ez_dropbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5000 2024-05-21 19:45:30.000000 ez-dropbox-2.0.3/ez_dropbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2024-05-21 19:45:30.000000 ez-dropbox-2.0.3/ez_dropbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 19:45:30.000000 ez-dropbox-2.0.3/ez_dropbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-21 19:45:30.000000 ez-dropbox-2.0.3/ez_dropbox.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-21 19:45:30.000000 ez-dropbox-2.0.3/ez_dropbox.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:45:30.999749 ez-dropbox-2.0.3/ezdbx/
+-rw-r--r--   0 root         (0) root         (0)      117 2024-05-12 12:48:02.000000 ez-dropbox-2.0.3/ezdbx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20426 2024-05-21 19:44:39.000000 ez-dropbox-2.0.3/ezdbx/main.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 19:45:31.001367 ez-dropbox-2.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      888 2024-05-21 19:44:49.000000 ez-dropbox-2.0.3/setup.py
```

### Comparing `ez-dropbox-2.0.2/LICENSE` & `ez-dropbox-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ez-dropbox-2.0.2/PKG-INFO` & `ez-dropbox-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-dropbox
-Version: 2.0.2
+Version: 2.0.3
 Summary: You can easily operate Dropbox!
 Home-page: https://github.com/TorDataScientist/ez-dropbox
 Author: TorDataScientist
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ez-dropbox-2.0.2/README.md` & `ez-dropbox-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ez-dropbox-2.0.2/ez_dropbox.egg-info/PKG-INFO` & `ez-dropbox-2.0.3/ez_dropbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-dropbox
-Version: 2.0.2
+Version: 2.0.3
 Summary: You can easily operate Dropbox!
 Home-page: https://github.com/TorDataScientist/ez-dropbox
 Author: TorDataScientist
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ez-dropbox-2.0.2/ezdbx/main.py` & `ez-dropbox-2.0.3/ezdbx/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         """
         クラスの初期化
         :param DROPBOX_ACCESS_TOKEN: Dropboxのアクセストークン
         """
         self.dbx = dropbox.Dropbox(DROPBOX_ACCESS_TOKEN, timeout=300)
         self.entry_list = []
         self.current_path = '/'
+        self.cant_save_files = []
         self.output = True
     
     def ls(self, file_or_folder='all'):
         """
         現在のパスのファイルやフォルダをリスト表示します。
         :param file_or_folder: 'file', 'folder', 'all'のいずれかを指定
         """
@@ -299,14 +300,21 @@
         指定したフォルダ内のファイルやフォルダを再帰的にリストします。
         :param folder: フォルダのパス
         """
         entries = self._get_entries(folder, 'all', recursive=True)
         for entry in entries:
             print(entry.path_display)
 
+    def cant_savefile(self):
+        """
+        保存できなかったファイルのリストを返します。
+        :return: 保存できなかったファイルのリスト
+        """
+        return self.cant_save_files
+
     def _list_local_files(self, folder):
         """
         ローカルフォルダ内のファイルをリストします。
         :param folder: フォルダのパス
         :return: ファイルのリスト
         """
         file_list = []
@@ -429,12 +437,16 @@
                             pbar.update(chunk_size)
         except OSError as e:
             print(f'Error uploading file {upload_file}: {e}')
             self._handle_unsupported_file(upload_file, os.path.join(upload_path, os.path.basename(upload_file)))
 
                         
     def _handle_unsupported_file(self, local_file, dropbox_path):
-        zip_path = local_file + '.zip'
-        with zipfile.ZipFile(zip_path, 'w') as zipf:
-            zipf.write(local_file, os.path.basename(local_file))
-        self.upload(zip_path, os.path.dirname(dropbox_path), overwrite=True)
-        os.remove(zip_path)
+        try : 
+            zip_path = local_file + '.zip'
+            with zipfile.ZipFile(zip_path, 'w') as zipf:
+                zipf.write(local_file, os.path.basename(local_file))
+            self.upload(zip_path, os.path.dirname(dropbox_path), overwrite=True)
+            os.remove(zip_path)
+        except Exception as e:
+            print(f'{local_file} は保存できませんでした。保存できなかったファイルを確認する場合は cant_savefile メソッドを参照してください。')
+            self.cant_save_files.append(local_file)
```

### Comparing `ez-dropbox-2.0.2/setup.py` & `ez-dropbox-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 packages = [
     'ezdbx'
 ]
 
 setup(
     name='ez-dropbox',
-    version='2.0.2',
+    version='2.0.3',
     license="MIT License",
     description="You can easily operate Dropbox!",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='TorDataScientist',
     url='https://github.com/TorDataScientist/ez-dropbox',
     packages=packages,
```

