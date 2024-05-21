# Comparing `tmp/pyxet-0.1.8.tar.gz` & `tmp/pyxet-0.1.9.tar.gz`

## Comparing `pyxet-0.1.8.tar` & `pyxet-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1253 1970-01-01 00:00:00.000000 pyxet-0.1.8/Cargo.toml
--rw-r--r--   0        0        0      685 2023-12-08 22:32:09.000000 pyxet-0.1.8/.gitignore
--rw-r--r--   0        0        0      597 2023-12-08 22:32:09.000000 pyxet-0.1.8/README.md
--rw-r--r--   0        0        0       81 2023-12-08 22:32:09.000000 pyxet-0.1.8/develop.sh
--rw-r--r--   0        0        0      985 2023-12-08 22:32:09.000000 pyxet-0.1.8/pypireadme.md
--rw-r--r--   0        0        0     1236 2023-12-08 22:32:09.000000 pyxet-0.1.8/pyxet/README.md
--rw-r--r--   0        0        0     2875 2023-12-08 22:32:09.000000 pyxet-0.1.8/pyxet/__init__.py
--rw-r--r--   0        0        0    22339 2023-12-08 22:32:09.000000 pyxet-0.1.8/pyxet/cli.py
--rw-r--r--   0        0        0     6217 2023-12-08 22:32:09.000000 pyxet-0.1.8/pyxet/commit_transaction.py
--rw-r--r--   0        0        0     3642 2023-12-08 22:32:09.000000 pyxet-0.1.8/pyxet/file_interface.py
--rw-r--r--   0        0        0    16789 2024-01-26 00:25:27.000000 pyxet-0.1.8/pyxet/file_operations.py
--rw-r--r--   0        0        0    28126 2023-12-08 22:32:09.000000 pyxet-0.1.8/pyxet/file_system.py
--rw-r--r--   0        0        0     6333 2023-12-08 22:32:09.000000 pyxet-0.1.8/pyxet/pathlib.py
--rw-r--r--   0        0        0        0 2023-12-08 22:32:09.000000 pyxet-0.1.8/pyxet/rpyxet/__init__.py
--rw-r--r--   0        0        0     9573 2024-01-26 00:25:27.000000 pyxet-0.1.8/pyxet/sync.py
--rw-r--r--   0        0        0     7338 2023-12-08 22:32:09.000000 pyxet-0.1.8/pyxet/url_parsing.py
--rw-r--r--   0        0        0     3602 2024-01-26 00:25:27.000000 pyxet-0.1.8/pyxet/util.py
--rw-r--r--   0        0        0       22 2024-01-26 01:10:00.000000 pyxet-0.1.8/pyxet/version.py
--rw-r--r--   0        0        0    30334 2023-12-08 22:32:09.000000 pyxet-0.1.8/src/lib.rs
--rw-r--r--   0        0        0     7689 2023-12-08 22:32:09.000000 pyxet-0.1.8/src/transactions.rs
--rw-r--r--   0        0        0     1843 2023-12-08 22:32:09.000000 pyxet-0.1.8/tests/arrow_test.py
--rw-r--r--   0        0        0    13135 2023-12-08 22:32:09.000000 pyxet-0.1.8/tests/cli_cp_test.py
--rw-r--r--   0        0        0     6654 2023-12-08 22:32:09.000000 pyxet-0.1.8/tests/file_test.py
--rw-r--r--   0        0        0     2279 2023-12-08 22:32:09.000000 pyxet-0.1.8/tests/fsspec_test.py
--rw-r--r--   0        0        0     1171 2023-12-08 22:32:09.000000 pyxet-0.1.8/tests/pandas_test.py
--rw-r--r--   0        0        0       64 2023-12-08 22:32:09.000000 pyxet-0.1.8/tests/requirements.txt
--rw-r--r--   0        0        0     4177 2023-12-08 22:32:09.000000 pyxet-0.1.8/tests/sync_test.py
--rw-r--r--   0        0        0     5279 2023-12-08 22:32:09.000000 pyxet-0.1.8/tests/utils.py
--rw-r--r--   0        0        0   120879 2024-01-26 01:10:29.000000 pyxet-0.1.8/Cargo.lock
--rw-r--r--   0        0        0     1719 2024-01-26 01:09:41.000000 pyxet-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2535 1970-01-01 00:00:00.000000 pyxet-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1475 1970-01-01 00:00:00.000000 pyxet-0.1.9/Cargo.toml
+-rw-r--r--   0        0        0      685 2023-12-08 22:32:09.000000 pyxet-0.1.9/.gitignore
+-rw-r--r--   0        0        0      597 2023-12-08 22:32:09.000000 pyxet-0.1.9/README.md
+-rw-r--r--   0        0        0       81 2023-12-08 22:32:09.000000 pyxet-0.1.9/develop.sh
+-rw-r--r--   0        0        0      985 2023-12-08 22:32:09.000000 pyxet-0.1.9/pypireadme.md
+-rw-r--r--   0        0        0     1236 2023-12-08 22:32:09.000000 pyxet-0.1.9/pyxet/README.md
+-rw-r--r--   0        0        0     2875 2023-12-08 22:32:09.000000 pyxet-0.1.9/pyxet/__init__.py
+-rw-r--r--   0        0        0    22396 2024-03-08 01:18:28.000000 pyxet-0.1.9/pyxet/cli.py
+-rw-r--r--   0        0        0     6217 2023-12-08 22:32:09.000000 pyxet-0.1.9/pyxet/commit_transaction.py
+-rw-r--r--   0        0        0     3642 2023-12-08 22:32:09.000000 pyxet-0.1.9/pyxet/file_interface.py
+-rw-r--r--   0        0        0    16789 2024-01-26 00:25:27.000000 pyxet-0.1.9/pyxet/file_operations.py
+-rw-r--r--   0        0        0    28126 2023-12-08 22:32:09.000000 pyxet-0.1.9/pyxet/file_system.py
+-rw-r--r--   0        0        0     6333 2023-12-08 22:32:09.000000 pyxet-0.1.9/pyxet/pathlib.py
+-rw-r--r--   0        0        0        0 2023-12-08 22:32:09.000000 pyxet-0.1.9/pyxet/rpyxet/__init__.py
+-rw-r--r--   0        0        0    10411 2024-03-08 01:18:28.000000 pyxet-0.1.9/pyxet/sync.py
+-rw-r--r--   0        0        0     7338 2023-12-08 22:32:09.000000 pyxet-0.1.9/pyxet/url_parsing.py
+-rw-r--r--   0        0        0     3602 2024-01-26 00:25:27.000000 pyxet-0.1.9/pyxet/util.py
+-rw-r--r--   0        0        0       22 2024-03-08 01:57:51.000000 pyxet-0.1.9/pyxet/version.py
+-rw-r--r--   0        0        0    30375 2024-03-08 01:18:28.000000 pyxet-0.1.9/src/lib.rs
+-rw-r--r--   0        0        0     7689 2023-12-08 22:32:09.000000 pyxet-0.1.9/src/transactions.rs
+-rw-r--r--   0        0        0     1843 2023-12-08 22:32:09.000000 pyxet-0.1.9/tests/arrow_test.py
+-rw-r--r--   0        0        0    13135 2023-12-08 22:32:09.000000 pyxet-0.1.9/tests/cli_cp_test.py
+-rw-r--r--   0        0        0     6654 2023-12-08 22:32:09.000000 pyxet-0.1.9/tests/file_test.py
+-rw-r--r--   0        0        0     2279 2023-12-08 22:32:09.000000 pyxet-0.1.9/tests/fsspec_test.py
+-rw-r--r--   0        0        0     1171 2023-12-08 22:32:09.000000 pyxet-0.1.9/tests/pandas_test.py
+-rw-r--r--   0        0        0       64 2023-12-08 22:32:09.000000 pyxet-0.1.9/tests/requirements.txt
+-rw-r--r--   0        0        0     3993 2024-03-08 01:18:28.000000 pyxet-0.1.9/tests/sync_test.py
+-rw-r--r--   0        0        0     5279 2023-12-08 22:32:09.000000 pyxet-0.1.9/tests/utils.py
+-rw-r--r--   0        0        0   118949 2024-03-08 01:58:11.000000 pyxet-0.1.9/Cargo.lock
+-rw-r--r--   0        0        0     1729 2024-03-08 01:57:40.000000 pyxet-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2535 1970-01-01 00:00:00.000000 pyxet-0.1.9/PKG-INFO
```

### Comparing `pyxet-0.1.8/Cargo.toml` & `pyxet-0.1.9/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyxet"
-version = "0.1.8"
+version = "0.1.9"
 edition = "2021"
 
 [lib]
 # The name of the native library. This is the name which will be used in Python to import the
 # library (i.e. `import string_sum`). If you change this, you must also change the name of the
 # `#[pymodule]` in `src/lib.rs`.
 name = "pyxet"
@@ -15,22 +15,33 @@
 # crate-type = ["cdylib", "rlib"]
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = { version = "0.18.0", features = ["extension-module", "abi3-py37", "generate-import-lib"] }
 xetblob = { git = "https://github.com/xetdata/xet-core" }
 progress_reporting = { git = "https://github.com/xetdata/xet-core" }
-gitxetcore = { git = "https://github.com/xetdata/xet-core" }
 tempfile = "3.2.0"
 pyo3-asyncio = { version = "0.18", features = ["attributes", "tokio-runtime"] }
 libc = "0.2"
 url = "2.3.1"
 tracing = "0.1.*"
 tokio = { version = "1", features = ["full"] }
 futures = "0.3.21"
-thiserror = "1.0.30"
 anyhow = "1"
 lazy_static = "1.4.0"
 
+[target.'cfg(target_os = "windows")'.dependencies.gitxetcore]
+git = "https://github.com/xetdata/xet-core"
+features = []
+
+[target.'cfg(not(target_os = "windows"))'.dependencies.gitxetcore]
+git = "https://github.com/xetdata/xet-core"
+features = ["openssl_vendored"]
+
 [build-dependencies]
 pyo3-build-config = "0.18.0"
 cc = "1.0"
+
+[release]
+opt-level = 3
+debug = true
+
```

### Comparing `pyxet-0.1.8/.gitignore` & `pyxet-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/README.md` & `pyxet-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/pypireadme.md` & `pyxet-0.1.9/pypireadme.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/pyxet/README.md` & `pyxet-0.1.9/pyxet/README.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/pyxet/__init__.py` & `pyxet-0.1.9/pyxet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/pyxet/cli.py` & `pyxet-0.1.9/pyxet/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,16 @@
         if not message:
             message = f"sync {source} to {target}"
         util.MAX_CONCURRENT_COPIES = threading.Semaphore(parallel)
         cmd = SyncCommand(source, target, use_mtime, message, dryrun, update_size)
         print(f"Checking sync")
         cmd.validate()
         print(f"Starting sync")
+        if dryrun:
+            print("This is a dryrun")
         stats = cmd.run()
         if not dryrun:
             print(f"Completed sync. Copied: {stats.copied} files, ignored: {stats.ignored} files")
             if stats.failed > 0:
                 print(f"{stats.failed} entries failed to copy")
 
     @staticmethod
```

### Comparing `pyxet-0.1.8/pyxet/commit_transaction.py` & `pyxet-0.1.9/pyxet/commit_transaction.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/pyxet/file_interface.py` & `pyxet-0.1.9/pyxet/file_interface.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/pyxet/file_operations.py` & `pyxet-0.1.9/pyxet/file_operations.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/pyxet/file_system.py` & `pyxet-0.1.9/pyxet/file_system.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/pyxet/pathlib.py` & `pyxet-0.1.9/pyxet/pathlib.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/pyxet/sync.py` & `pyxet-0.1.9/pyxet/sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 from functools import partial
 
-from pyxet.util import _get_fs_and_path, _isdir, _rel_path, _path_join, _path_dirname, _is_illegal_subdirectory_file_name
+from pyxet.util import _get_fs_and_path, _isdir, _rel_path, _path_join, _path_split, _path_dirname, _is_illegal_subdirectory_file_name
 from pyxet.file_operations import _single_file_copy_impl, CopyUnit
 
 XET_MTIME_FORMAT = '%Y-%m-%dT%H:%M:%S%z'
 
 
 class SyncCommand:
 
@@ -37,17 +37,14 @@
         if self._src_proto == 'xet':
             raise ValueError(f"Unsupported source protocol: {self._src_proto}, only non-xet sources are supported")
 
         # check that the destination specifies an existing branch
         # TODO: we may want to be able to sync remote location to a new branch?
         self._dest_fs.branch_info(self._dest_root)
 
-        # source should be a directory
-        if not _isdir(self._src_fs, self._src_root):
-            raise ValueError(f"source: {self._src_root} needs to be a directory")
         # s3 needs a bucket
         if self._src_proto == 's3' and (self._src_root == '/' or self._src_root == ''):
             raise ValueError(f"S3 source needs a specified bucket")
 
         # wildcards not supported
         if '*' in self._src_root or '*' in self._dest_root:
             raise ValueError(f"Wildcards not supported in paths")
@@ -55,19 +52,21 @@
     def run(self):
         """
         Runs this Sync command, returning SyncStats containing the number of files copied
         during the sync.
         """
         sync_stats = SyncStats()
 
+        srcpath_is_dir = _isdir(self._src_fs, self._src_root)
         if not self._dryrun:
             self._dest_fs.start_transaction(self._message)
         with ThreadPoolExecutor() as executor:
             futures = []
-            if self._use_mtime:
+            # if src is a single file, we always use sync_with_info
+            if self._use_mtime or srcpath_is_dir == False:
                 self._sync_with_info(executor, futures, self._src_root, self._dest_root)
             else:
                 self._sync_with_ls(executor, futures, self._src_root, self._dest_root)
 
             # Waiting for all copy jobs to complete
             for future in futures:
                 try:
@@ -89,14 +88,15 @@
         """
         Sync the src_path to the dest_path using ls calls on both paths and comparing the
         two.
 
         Note that ls on xet-fs doesn't return an mtime and thus, will not be able to compare
         on that field.
         """
+        # This only syncs folders. single files should always go to sync_with_info
         try:
             dest_files = self._dest_fs.find(dest_path, detail=True)
         except RuntimeError:
             dest_files = {}
         total_size = 0
         for abs_path, src_info in self._src_fs.find(src_path, detail=True).items():
             relpath = _rel_path(abs_path, src_path)
@@ -117,26 +117,37 @@
 
     def _sync_with_info(self, executor, futures, src_path, dest_path):
         """
         Sync the src_path to the dest_path by calling `info` on the destination for files
         found in the source. This is much slower than
         """
         total_size = 0
-        for abs_path, src_info in self._src_fs.find(src_path, detail=True).items():
-            relpath = _rel_path(abs_path, src_path)
-
-            if _is_illegal_subdirectory_file_name(relpath):
-                print(f"{abs_path} is an invalid file (not copied).")
-                continue
+        if not _isdir(self._src_fs, src_path):
+            src_info = self._src_fs.info(src_path)
+            abs_path = src_info['name']
+            # get the last component name. This is the filename
+            fname = _path_split(self._src_fs, abs_path)[-1]
+            # Tack it on to the end of the dest path to make the output name
+            dest_for_this_path = _path_join(self._dest_fs, dest_path, fname)
+            partial_func = partial(self._sync_with_mtime_task, abs_path, dest_for_this_path, src_info)
+            futures.append(executor.submit(partial_func))
+            total_size += src_info.get('size', 0)
+        else:
+            for abs_path, src_info in self._src_fs.find(src_path, detail=True).items():
+                relpath = _rel_path(abs_path, src_path)
 
-            dest_for_this_path = _path_join(self._dest_fs, dest_path, relpath)
-            if src_info['type'] != 'directory':
-                partial_func = partial(self._sync_with_mtime_task, abs_path, dest_for_this_path, src_info)
-                futures.append(executor.submit(partial_func))
-                total_size += src_info.get('size', 0)
+                if _is_illegal_subdirectory_file_name(relpath):
+                    print(f"{abs_path} is an invalid file (not copied).")
+                    continue
+
+                dest_for_this_path = _path_join(self._dest_fs, dest_path, relpath)
+                if src_info['type'] != 'directory':
+                    partial_func = partial(self._sync_with_mtime_task, abs_path, dest_for_this_path, src_info)
+                    futures.append(executor.submit(partial_func))
+                    total_size += src_info.get('size', 0)
 
         if self._update_size:
             self._update_remote_size(total_size)
 
     def _sync_with_mtime_task(self, src_path, dest_path, src_info):
         """
         Fetch info for the dest_path from remote and use that to sync the file
@@ -160,14 +171,16 @@
 
         size = src_info.get('size', None)
         if dest_info is None or self._cmp.should_sync(src_info, dest_info):
             if not self._dryrun:
                 dest_dir = _path_dirname(self._dest_fs, dest_path)
                 cp_copy = CopyUnit(src_path=src_path, dest_path=dest_path, dest_dir = dest_dir, size = size)
                 _single_file_copy_impl(cp_copy, self._src_fs, self._dest_fs)
+            else:
+                print(f"Copying {src_path} to {dest_path}")
             return True
         # ignored
         return False
 
     def _update_remote_size(self, size):
         """
         Update Xetea with the new bucket size.
```

### Comparing `pyxet-0.1.8/pyxet/url_parsing.py` & `pyxet-0.1.9/pyxet/url_parsing.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/pyxet/util.py` & `pyxet-0.1.9/pyxet/util.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/src/lib.rs` & `pyxet-0.1.9/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use anyhow::{anyhow, Result};
 use gitxetcore::command::login::*;
 use gitxetcore::command::mount::*;
 use gitxetcore::command::*;
 use gitxetcore::config::ConfigGitPathOption;
 use gitxetcore::config::ConfigGitPathOption::NoPath;
 use gitxetcore::config::XetConfig;
-use gitxetcore::log::initialize_tracing_subscriber;
+use gitxetcore::environment::log::initialize_tracing_subscriber;
 use progress_reporting::DataProgressReporter;
 use pyo3::exceptions::*;
 use pyo3::prelude::*;
 use pyo3::types::{PyByteArray, PyBytes, PyList};
 use std::sync::Arc;
 use tokio::sync::{RwLock, RwLockReadGuard, RwLockWriteGuard};
 use tracing::{error, info};
@@ -651,18 +651,18 @@
             ))
         }
     }
 
     async fn complete_impl(&mut self, commit: bool, cleanup_immediately: bool) -> Result<()> {
         let Some(tr) = self.pwt.take() else {
             // This means either we've called close() on the transaction, then tried to use it;
-            // or all associated write files complete and close before calling close(). 
+            // or all associated write files complete and close before calling close().
             // Either case this should be a NOP.
             info!("Complete called after PyTransaction object committed");
-            return Ok(())
+            return Ok(());
         };
 
         {
             let mut trw = tr.write().await;
 
             if commit {
                 trw.set_commit_when_ready();
@@ -799,27 +799,29 @@
 }
 
 impl PyWriteTransactionAccessToken {
     async fn access_transaction_for_write<'a>(
         &'a self,
     ) -> Result<RwLockWriteGuard<'a, WriteTransaction>> {
         let Some(t) = &self.tr else {
-            // This should only happen if it's been closed explicitly, then 
+            // This should only happen if it's been closed explicitly, then
             // access is attempted.
-            return Err(anyhow!("Transaction accessed for write after being closed."));
+            return Err(anyhow!(
+                "Transaction accessed for write after being closed."
+            ));
         };
 
         Ok(t.write().await)
     }
 
     async fn access_transaction_for_read<'a>(
         &'a self,
     ) -> Result<RwLockReadGuard<'a, WriteTransaction>> {
         let Some(t) = &self.tr else {
-            // This should only happen if it's been closed explicitly, then 
+            // This should only happen if it's been closed explicitly, then
             // access is attempted.
             return Err(anyhow!("Transaction accessed for read after being closed."));
         };
 
         Ok(t.read().await)
     }
```

### Comparing `pyxet-0.1.8/src/transactions.rs` & `pyxet-0.1.9/src/transactions.rs`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/tests/arrow_test.py` & `pyxet-0.1.9/tests/arrow_test.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/tests/cli_cp_test.py` & `pyxet-0.1.9/tests/cli_cp_test.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/tests/file_test.py` & `pyxet-0.1.9/tests/file_test.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/tests/fsspec_test.py` & `pyxet-0.1.9/tests/fsspec_test.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/tests/pandas_test.py` & `pyxet-0.1.9/tests/pandas_test.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/tests/sync_test.py` & `pyxet-0.1.9/tests/sync_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,14 @@
         assert not is_valid
 
 
 def test_sync_command_validate_local():
     pyxet.login(CONSTANTS.TESTING_USERNAME, CONSTANTS.TESTING_TOKEN, email="a@a.com")
 
     check_sync_validate('.', f'xet://{CONSTANTS.TESTING_SYNCREPO}/main', True)
-    check_sync_validate('/nonexistent', f'xet://{CONSTANTS.TESTING_SYNCREPO}/main', False)
-    check_sync_validate('./sync_test.py', f'xet://{CONSTANTS.TESTING_SYNCREPO}/main', False)
     check_sync_validate('xet://XetHub/grapp2/main', f'xet://{CONSTANTS.TESTING_SYNCREPO}/sync-branch/sync', False)
     check_sync_validate('.', f'xet://{CONSTANTS.TESTING_SYNCREPO}/nonexistent-branch', False)
     check_sync_validate('.', './other', False)
     check_sync_validate('.', f'xet://{CONSTANTS.TESTING_SYNCREPO}', False)
     check_sync_validate('.', 'xet://', False)
     check_sync_validate('./*', f'xet://{CONSTANTS.TESTING_SYNCREPO}/main', False)
     check_sync_validate('./*.py', f'xet://{CONSTANTS.TESTING_SYNCREPO}/main', False)
```

### Comparing `pyxet-0.1.8/tests/utils.py` & `pyxet-0.1.9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.8/Cargo.lock` & `pyxet-0.1.9/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,31 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "addr2line"
+version = "0.21.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8a30b2e23b9e17a9f90641c7ab1549cd9b44f296d3ccbf309d2863cfe398a0cb"
+dependencies = [
+ "gimli",
+]
+
+[[package]]
+name = "adler"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
+
+[[package]]
 name = "ahash"
-version = "0.7.6"
+version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
+checksum = "891477e0c6a8957309ee5c45a6368af3ae14bb510732d2684ffa19af310920f9"
 dependencies = [
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
@@ -19,14 +34,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
 name = "android_system_properties"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
@@ -38,17 +59,17 @@
 checksum = "d52a9bb7ec0cf484c551830a7ce27bd20d67eac647e1befb56b0be4ee39a55d2"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.70"
+version = "1.0.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
+checksum = "5ad32ce52e4161730f7098c077cd2ed6229b5804ccf99e5366be1ab72a98b4e1"
 
 [[package]]
 name = "approx"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
@@ -59,17 +80,17 @@
 name = "arrayref"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6b4930d2cb77ce62f89ee5d5289b4ac049559b1c45539271f5ed4fdc7db34545"
 
 [[package]]
 name = "arrayvec"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8da52d66c7071e2e3fa2a1e5c6d088fec47b593032b254f5e980de8ea54454d6"
+checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "async-scoped"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e7a6a57c8aeb40da1ec037f5d455836852f7a57e69e1b1ad3d8f38ac1d6cadf"
 dependencies = [
@@ -77,43 +98,43 @@
  "pin-project",
  "slab",
  "tokio",
 ]
 
 [[package]]
 name = "async-stream"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad445822218ce64be7a341abfb0b1ea43b5c23aa83902542a4542e78309d8e5e"
+checksum = "cd56dd203fef61ac097dd65721a419ddccb106b2d2b70ba60a6b529f03961a51"
 dependencies = [
  "async-stream-impl",
  "futures-core",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "async-stream-impl"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4655ae1a7b0cdf149156f780c5bf3f1352bc53cbd9e0a361a7ef7b22947e965"
+checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.67"
+version = "0.1.77"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86ea188f25f0255d8f92797797c97ebf5631fa88178beb1a46fdf5622c9a00e4"
+checksum = "c980ee35e870bd1a4d2c8294d4c04d0499e67bca1e4b5cefcc693c2fa00caea9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "atoi"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d7c57d12312ff59c811c0643f4d80830505833c9ffaebd193d819392b265be8e"
@@ -142,19 +163,19 @@
 name = "axum"
 version = "0.6.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3b829e4e32b91e643de6eafe82b1d90675f5874230191a4ffbc1b336dec4d6bf"
 dependencies = [
  "async-trait",
  "axum-core",
- "bitflags",
+ "bitflags 1.3.2",
  "bytes",
  "futures-util",
- "http 0.2.9",
- "http-body 0.4.5",
+ "http 0.2.11",
+ "http-body 0.4.6",
  "hyper 0.14.28",
  "itoa",
  "matchit",
  "memchr",
  "mime",
  "percent-encoding",
  "pin-project-lite",
@@ -171,33 +192,48 @@
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "759fa577a247914fd3f7f76d62972792636412fbfd634cd452f6a385a74d2d2c"
 dependencies = [
  "async-trait",
  "bytes",
  "futures-util",
- "http 0.2.9",
- "http-body 0.4.5",
+ "http 0.2.11",
+ "http-body 0.4.6",
  "mime",
  "rustversion",
  "tower-layer",
  "tower-service",
 ]
 
 [[package]]
+name = "backtrace"
+version = "0.3.69"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+dependencies = [
+ "addr2line",
+ "cc",
+ "cfg-if 1.0.0",
+ "libc",
+ "miniz_oxide",
+ "object",
+ "rustc-demangle",
+]
+
+[[package]]
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
 name = "base64"
-version = "0.21.0"
+version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4a4ddaa51a5bc52a6948f74c06d20aaaddb71924eab79b8c97a8c556e942d6a"
+checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
 name = "binary-heap-plus"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e4551d8382e911ecc0d0f0ffb602777988669be09447d536ff4388d1def11296"
 dependencies = [
@@ -216,25 +252,30 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+
+[[package]]
 name = "blake3"
-version = "1.3.3"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42ae2468a89544a466886840aa467a25b766499f4f04bf7d9fcd10ecee9fccef"
+checksum = "0231f06152bf547e9c2b5194f247cd97aacf6dcd8b15d8e5ec0663f64580da87"
 dependencies = [
  "arrayref",
  "arrayvec",
  "cc",
  "cfg-if 1.0.0",
  "constant_time_eq",
- "digest 0.10.7",
 ]
 
 [[package]]
 name = "block-buffer"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4152116fd6e9dadb291ae18fc1ec3575ed6d84c29642d97890f4b4a3417297e4"
@@ -256,49 +297,55 @@
 name = "block-padding"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8d696c370c750c948ada61c69a0ee2cbbb9c50b1019ddb86d9317157a99c2cae"
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.15.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "8ea184aa71bb362a1157c896979544cc23974e08fd265f29ea96b59f0b4a555b"
 
 [[package]]
 name = "bytecount"
-version = "0.6.3"
+version = "0.6.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1e5f035d16fc623ae5f74981db80a439803888314e3a555fd6f04acd51a3205"
+
+[[package]]
+name = "bytemuck"
+version = "1.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c676a478f63e9fa2dd5368a42f28bba0d6c560b775f38583c8bbaa7fcd67c9c"
+checksum = "a2ef034f05691a48569bd920a96c81b9d91bbad1ab5ac7c4616c1f6ef36cb79f"
 
 [[package]]
 name = "byteorder"
-version = "1.4.3"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
+checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
-version = "1.4.0"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
+checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
 
 [[package]]
 name = "bytestream"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04f720842a717d6afaf69fee2dc69b771edc165f12cc3eb1b0e8eeef53a86454"
 dependencies = [
  "byteorder",
 ]
 
 [[package]]
 name = "cache"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.13.1",
  "byteorder",
  "chrono",
  "lazy_static",
@@ -314,44 +361,44 @@
  "tracing-test",
  "utils",
  "xet_error",
 ]
 
 [[package]]
 name = "cas_client"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "anyhow",
  "async-trait",
  "bincode",
  "bytes",
  "cache",
  "clap 2.34.0",
  "common_constants",
  "deadpool",
  "error_printer",
  "futures",
- "http 0.2.9",
+ "http 0.2.11",
  "http-body-util",
- "hyper 1.1.0",
+ "hyper 1.2.0",
  "hyper-rustls",
  "hyper-util",
- "itertools",
+ "itertools 0.10.5",
  "lazy_static",
  "merkledb",
  "merklehash",
  "opentelemetry",
  "opentelemetry-http",
  "opentelemetry-jaeger",
  "parutils",
  "progress_reporting",
  "prost",
  "retry_strategy",
- "rustls-pemfile 2.0.0",
+ "rustls-pemfile 2.1.0",
  "serde_json",
  "tempfile",
  "tokio",
  "tokio-native-tls",
  "tokio-retry",
  "tokio-rustls 0.25.0",
  "tonic",
@@ -361,19 +408,19 @@
  "utils",
  "uuid",
  "xet_error",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.79"
+version = "1.0.88"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+checksum = "02f341c093d19155a6e41631ce5971aac4e9a868262212153124c15fa22d1cdc"
 dependencies = [
- "jobserver",
+ "libc",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4785bdd1c96b2a846b2bd7cc02e86b6b3dbf14e7e53446c4f54c92a361040822"
@@ -382,65 +429,64 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.24"
+version = "0.4.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
+checksum = "5bc015644b92d5890fab7489e49d21f879d5c990186827d42ec511919404f38b"
 dependencies = [
+ "android-tzdata",
  "iana-time-zone",
  "js-sys",
- "num-integer",
  "num-traits",
  "serde",
- "time 0.1.45",
  "wasm-bindgen",
- "winapi",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "clap"
 version = "2.34.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0610544180c38b88101fecf2dd634b174a62eef6946f84dfc6a7127512b381c"
 dependencies = [
  "ansi_term",
  "atty",
- "bitflags",
+ "bitflags 1.3.2",
  "strsim 0.8.0",
  "textwrap 0.11.0",
  "unicode-width",
  "vec_map",
 ]
 
 [[package]]
 name = "clap"
-version = "3.2.23"
+version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
+checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
 dependencies = [
  "atty",
- "bitflags",
+ "bitflags 1.3.2",
  "clap_derive",
  "clap_lex",
- "indexmap 1.9.2",
+ "indexmap 1.9.3",
  "once_cell",
  "strsim 0.10.0",
  "termcolor",
- "textwrap 0.16.0",
+ "textwrap 0.16.1",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "3.2.18"
+version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea0c8bce528c4be4da13ea6fead8965e95b6073585a2f05204bd8f4119f82a65"
+checksum = "ae6371b8bdc8b7d3959e9cf7b22d4435ef3e79e138688421ec654acf8c81b008"
 dependencies = [
  "heck 0.4.1",
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
@@ -462,39 +508,38 @@
 dependencies = [
  "termcolor",
  "unicode-width",
 ]
 
 [[package]]
 name = "colored"
-version = "2.0.0"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3616f750b84d8f0de8a58bda93e08e2a81ad3f523089b05f1dffecab48c6cbd"
+checksum = "cbf2150cce219b664a8a70df7a1f933836724b503f8a413af9365b4dcc4d90b8"
 dependencies = [
- "atty",
  "lazy_static",
- "winapi",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "common_constants"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 
 [[package]]
 name = "compare"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "120133d4db2ec47efe2e26502ee984747630c67f51974fca0b6c1340cf2368d3"
 
 [[package]]
 name = "config"
-version = "0.13.3"
+version = "0.13.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d379af7f68bfc21714c6c7dea883544201741d2ce8274bb12fa54f89507f52a7"
+checksum = "23738e11972c7643e4ec947840fc463b6a571afcd3e735bdfce7d03c7a784aca"
 dependencies = [
  "async-trait",
  "json5",
  "lazy_static",
  "nom",
  "pathdiff",
  "ron 0.7.1",
@@ -503,104 +548,89 @@
  "serde_json",
  "toml",
  "yaml-rust",
 ]
 
 [[package]]
 name = "const_format"
-version = "0.2.30"
+version = "0.2.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7309d9b4d3d2c0641e018d449232f2e28f1b22933c137f157d3dbc14228b8c0e"
+checksum = "e3a214c7af3d04997541b18d432afaff4c455e79e2029079647e72fc2bd27673"
 dependencies = [
  "const_format_proc_macros",
 ]
 
 [[package]]
 name = "const_format_proc_macros"
-version = "0.2.29"
+version = "0.2.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d897f47bf7270cf70d370f8f98c1abb6d2d4cf60a6845d30e05bfb90c6568650"
+checksum = "c7f6ff08fd20f4f299298a28e2dfa8a8ba1036e6cd2460ac1de7b425d76f2500"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-xid",
 ]
 
 [[package]]
 name = "constant_time_eq"
-version = "0.2.5"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13418e745008f7349ec7e449155f419a61b92b58a99cc3616942b926825ec76b"
+checksum = "f7144d30dcf0fafbce74250a3963025d8d52177934239851c917d29f1df280c2"
 
 [[package]]
 name = "core-foundation"
-version = "0.9.3"
+version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
+checksum = "91e195e091a93c46f7102ec7818a2aa394e1e1771c3ab4825963fa03e45afb8f"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.5"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
+checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
-name = "crc32fast"
-version = "1.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
-dependencies = [
- "cfg-if 1.0.0",
-]
-
-[[package]]
 name = "crossbeam-channel"
-version = "0.5.7"
+version = "0.5.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf2b3e8478797446514c91ef04bafcb59faba183e621ad488df88983cc14128c"
+checksum = "ab3db02a9c5b5121e1e42fbdb1aeb65f5e02624cc58c43f2884c6ccac0b82f95"
 dependencies = [
- "cfg-if 1.0.0",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
-version = "0.8.3"
+version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
+checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
 dependencies = [
- "cfg-if 1.0.0",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.14"
+version = "0.9.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
+checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
- "autocfg",
- "cfg-if 1.0.0",
  "crossbeam-utils",
- "memoffset",
- "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-queue"
 version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "df0346b5d5e76ac2fe4e327c5fd1118d6be7c51dfb18f9b7922923f287471e35"
@@ -616,29 +646,29 @@
 
 [[package]]
 name = "crossterm"
 version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e64e6c0fbe2c17357405f7c758c1ef960fce08bdfb2c03d88d2a18d7e09c4b67"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "crossterm_winapi",
  "libc",
  "mio",
  "parking_lot 0.12.1",
  "signal-hook",
  "signal-hook-mio",
  "winapi",
 ]
 
 [[package]]
 name = "crossterm_winapi"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2ae1b35a484aa10e07fe0638d02301c5ad24de82d310ccbd2f3693da5f09bf1c"
+checksum = "acdd7c62a3665c7f6830a51635d9ac9b23ed385797f70a83bb8bafe9c572ab2b"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
@@ -646,84 +676,74 @@
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
-name = "crypto-mac"
-version = "0.11.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25fab6889090c8133f3deb8f73ba3c65a7f456f66436fc012a1b1e272b1e103e"
-dependencies = [
- "generic-array",
- "subtle",
-]
-
-[[package]]
 name = "csv-core"
-version = "0.1.10"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
+checksum = "5efa2b3d7902f4b634a20cae3c9c4e6209dc4779feb6863329607560143efa70"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "ctrlc"
-version = "3.2.5"
+version = "3.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbcf33c2a618cbe41ee43ae6e9f2e48368cd9f9db2896f10167d8d762679f639"
+checksum = "b467862cc8610ca6fc9a1532d7777cee0804e678ab45410897b9396495994a0b"
 dependencies = [
  "nix",
- "windows-sys 0.45.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "cxx"
-version = "1.0.93"
+version = "1.0.118"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9c00419335c41018365ddf7e4d5f1c12ee3659ddcf3e01974650ba1de73d038"
+checksum = "2673ca5ae28334544ec2a6b18ebe666c42a2650abfb48abbd532ed409a44be2b"
 dependencies = [
  "cc",
  "cxxbridge-flags",
  "cxxbridge-macro",
  "link-cplusplus",
 ]
 
 [[package]]
 name = "cxx-build"
-version = "1.0.93"
+version = "1.0.118"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb8307ad413a98fff033c8545ecf133e3257747b3bae935e7602aab8aa92d4ca"
+checksum = "9df46fe0eb43066a332586114174c449a62c25689f85a08f28fdcc8e12c380b9"
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn 2.0.38",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
-version = "1.0.93"
+version = "1.0.118"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "edc52e2eb08915cb12596d29d55f0b5384f00d697a646dbd269b6ecb0fbd9d31"
+checksum = "886acf875df67811c11cd015506b3392b9e1820b1627af1a6f4e93ccdfc74d11"
 
 [[package]]
 name = "cxxbridge-macro"
-version = "1.0.93"
+version = "1.0.118"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "631569015d0d8d54e6c241733f944042623ab6df7bc3be7466874b05fcdb1c5f"
+checksum = "1d151cc139c3080e07f448f93a1284577ab2283d2a44acd902c6fba9ec20b6de"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "darling"
 version = "0.13.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a01d95850c592940db9b8194bc39f4bc0e89dee5c4265e4b1807c34a9aba453c"
@@ -755,16 +775,16 @@
  "darling_core",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "data_analysis"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "approx",
  "cxx",
  "cxx-build",
  "float-cmp",
  "serde",
  "truncrate",
@@ -781,17 +801,17 @@
  "num_cpus",
  "retain_mut",
  "tokio",
 ]
 
 [[package]]
 name = "deadpool-runtime"
-version = "0.1.2"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eaa37046cc0f6c3cc6090fbdbf73ef0b8ef4cfcc37f6befc0020f63e8cf121e1"
+checksum = "63dfa964fe2a66f3fde91fc70b267fe193d822c7e603e2a675a49a7f46ad3f49"
 dependencies = [
  "tokio",
 ]
 
 [[package]]
 name = "deadqueue"
 version = "0.2.4"
@@ -799,14 +819,23 @@
 checksum = "16a2561fd313df162315935989dceb8c99db4ee1933358270a57a3cfb8c957f3"
 dependencies = [
  "crossbeam-queue",
  "tokio",
 ]
 
 [[package]]
+name = "deranged"
+version = "0.3.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
+dependencies = [
+ "powerfmt",
+]
+
+[[package]]
 name = "difflib"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6184e33543162437515c2e2b48714794e37845ec9851711914eec9d308f6ebe8"
 
 [[package]]
 name = "digest"
@@ -821,15 +850,14 @@
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer 0.10.4",
  "crypto-common",
- "subtle",
 ]
 
 [[package]]
 name = "dirs"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "13aea89a5c93364a98e9b37b2fa237effbb694d5cfe01c5b70941f7eb087d5e3"
@@ -844,144 +872,109 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca3aa72a6f96ea37bbc5aa912f6788242832f75369bdfdadcb0e38423f100059"
 dependencies = [
  "dirs-sys",
 ]
 
 [[package]]
-name = "dirs-next"
-version = "2.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b98cf8ebf19c3d1b223e151f99a4f9f0690dca41414773390fc824184ac833e1"
-dependencies = [
- "cfg-if 1.0.0",
- "dirs-sys-next",
-]
-
-[[package]]
 name = "dirs-sys"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b1d1d91c932ef41c0f2663aa8b0ca0342d444d842c06914aa0a7e352d0bada6"
 dependencies = [
  "libc",
  "redox_users",
  "winapi",
 ]
 
 [[package]]
-name = "dirs-sys-next"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ebda144c4fe02d1f7ea1a7d9641b6fc6b580adcfa024ae48797ecdeb6825b4d"
-dependencies = [
- "libc",
- "redox_users",
- "winapi",
-]
-
-[[package]]
 name = "dlv-list"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0688c2a7f92e427f44895cd63841bff7b29f8d7a1648b9e7e07a4a365b2e1257"
 
 [[package]]
 name = "downcast"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1435fa1053d8b2fbbe9be7e97eca7f33d37b28409959813daefc1446a14247f1"
 
 [[package]]
 name = "either"
-version = "1.8.1"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
 name = "encoding_rs"
-version = "0.8.32"
+version = "0.8.33"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
+checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
 dependencies = [
  "cfg-if 1.0.0",
 ]
 
 [[package]]
 name = "enum_dispatch"
-version = "0.3.11"
+version = "0.3.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11f36e95862220b211a6e2aa5eca09b4fa391b13cd52ceb8035a24bf65a79de2"
+checksum = "8f33313078bb8d4d05a2733a94ac4c2d8a0df9a2b84424ebf4f33bfc224a890e"
 dependencies = [
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
-version = "0.2.8"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
+checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
- "errno-dragonfly",
- "libc",
- "winapi",
-]
-
-[[package]]
-name = "errno-dragonfly"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
-dependencies = [
- "cc",
  "libc",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "error_printer"
-version = "0.1.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "tracing",
 ]
 
 [[package]]
 name = "fallible-iterator"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4443176a9f2c162692bd3d352d745ef9413eec5782a80d8fd6f8a1ac692a07f7"
 
 [[package]]
 name = "fastrand"
-version = "1.9.0"
+version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
-dependencies = [
- "instant",
-]
+checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
 
 [[package]]
 name = "filetime"
-version = "0.2.20"
+version = "0.2.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a3de6e8d11b22ff9edc6d916f890800597d60f8b2da1caf2955c274638d6412"
+checksum = "1ee447700ac8aa0b2f2bd7bc4462ad686ba06baa6727ac149a2d6277f0d240fd"
 dependencies = [
  "cfg-if 1.0.0",
  "libc",
- "redox_syscall",
- "windows-sys 0.45.0",
+ "redox_syscall 0.4.1",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
@@ -1014,17 +1007,17 @@
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
 
 [[package]]
 name = "form_urlencoded"
-version = "1.1.0"
+version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
+checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "fragile"
 version = "2.0.0"
@@ -1035,88 +1028,88 @@
 name = "fuchsia-cprng"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a06f77d526c1a601b7c4cdd98f54b5eaabffc14d5f2f0296febdc7f357c6d3ba"
 
 [[package]]
 name = "futures"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
+checksum = "645c6916888f6cb6350d2550b80fb63e734897a8498abe35cfb732b6487804b0"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
+checksum = "eac8f7d7865dcb88bd4373ab671c8cf4508703796caa2b1985a9ca867b3fcb78"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
+checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
+checksum = "a576fc72ae164fca6b9db127eaa9a9dda0d61316034f33a0a0d4eda41f02b01d"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
+checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
+checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
+checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
 
 [[package]]
 name = "futures-task"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
+checksum = "38d84fa142264698cdce1a9f9172cf383a0c82de1bddcf3092901442c4097004"
 
 [[package]]
 name = "futures-util"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
+checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -1133,84 +1126,88 @@
 checksum = "c8cf82cf76cd16485e56295a1377c775ce708c9f1a0be6b029076d60a245d213"
 dependencies = [
  "cfg-if 0.1.10",
 ]
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
 dependencies = [
  "cfg-if 1.0.0",
  "libc",
- "wasi 0.11.0+wasi-snapshot-preview1",
+ "wasi",
 ]
 
 [[package]]
+name = "gimli"
+version = "0.28.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
+
+[[package]]
 name = "git-version"
-version = "0.3.5"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f6b0decc02f4636b9ccad390dcbe77b722a77efedfa393caf8379a51d5c61899"
+checksum = "1ad568aa3db0fcbc81f2f116137f263d7304f512a1209b35b85150d3ef88ad19"
 dependencies = [
  "git-version-macro",
- "proc-macro-hack",
 ]
 
 [[package]]
 name = "git-version-macro"
-version = "0.3.5"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fe69f1cbdb6e28af2bac214e943b99ce8a0a06b447d15d3e61161b0423139f3f"
+checksum = "53010ccb100b96a67bc32c0175f0ed1426b31b655d562898e57325f81c023ac0"
 dependencies = [
- "proc-macro-hack",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "git2"
-version = "0.14.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0155506aab710a86160ddb504a480d2964d7ab5b9e62419be69e0032bc5931c"
+version = "0.18.2"
+source = "git+https://github.com/xetdata/git2-rs#dfffd3d1eb9e87a9e7e98b24d0a0f54db664cbcc"
 dependencies = [
- "bitflags",
+ "bitflags 2.4.2",
  "libc",
  "libgit2-sys",
  "log",
  "openssl-probe",
  "openssl-sys",
  "url",
 ]
 
 [[package]]
 name = "gitxetcore"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "anyhow",
  "async-trait",
  "atoi",
  "atty",
  "base64 0.13.1",
  "bincode",
+ "blake3",
  "cas_client",
  "chrono",
- "clap 3.2.23",
+ "clap 3.2.25",
  "colored",
  "common_constants",
  "const_format",
  "csv-core",
  "ctrlc",
  "data_analysis",
  "dirs 4.0.0",
@@ -1219,19 +1216,19 @@
  "fallible-iterator",
  "filetime",
  "futures",
  "futures-core",
  "git-version",
  "git2",
  "hex",
- "http 0.2.9",
+ "http 0.2.11",
  "humantime",
  "intaglio",
  "is_executable",
- "itertools",
+ "itertools 0.10.5",
  "lazy",
  "lazy_static",
  "libc",
  "libmagic",
  "lru",
  "mdb_shard",
  "merkledb",
@@ -1243,34 +1240,36 @@
  "normalize-path",
  "openssl",
  "opentelemetry",
  "opentelemetry-jaeger",
  "parutils",
  "pathdiff",
  "pbr",
- "pointer_file",
  "progress_reporting",
  "prometheus",
  "prometheus_dict_encoder",
  "rand 0.8.5",
  "regex",
  "reqwest",
+ "retry_strategy",
  "ring 0.16.20",
- "s3",
  "same-file",
  "serde",
  "serde_json",
  "serde_with",
  "shard_client",
+ "shellexpand",
  "slog",
  "slog-async",
  "slog-json",
  "snailquote",
  "sorted-vec",
  "sysinfo",
+ "tabled",
+ "tempdir",
  "tempfile",
  "tokio",
  "toml",
  "tracing",
  "tracing-attributes",
  "tracing-futures",
  "tracing-opentelemetry",
@@ -1285,25 +1284,25 @@
  "winapi",
  "xet_config",
  "xet_error",
 ]
 
 [[package]]
 name = "h2"
-version = "0.3.23"
+version = "0.3.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b553656127a00601c8ae5590fcfdc118e4083a7924b6cf4ffc1ea4b99dc429d7"
+checksum = "bb2c4422095b67ee78da96fbb51a4cc413b3b25883c7717ff7ca1ab31022c9c9"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
- "http 0.2.9",
- "indexmap 2.1.0",
+ "http 0.2.11",
+ "indexmap 2.2.3",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
@@ -1314,15 +1313,15 @@
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http 1.0.0",
- "indexmap 2.1.0",
+ "indexmap 2.2.3",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
@@ -1338,17 +1337,17 @@
 name = "hashbrown"
 version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
 
 [[package]]
 name = "hashring"
-version = "0.3.0"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd0ddd025eccd8a2fff9865e82ef4c8ce00c4a67709036847d95cf3ccffd07a8"
+checksum = "aa283406d74fcfeb4778f4e300beaae30db96793371da168d003cbc833e149e0"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
 name = "heck"
 version = "0.3.3"
@@ -1361,58 +1360,87 @@
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
-name = "hermit-abi"
-version = "0.1.19"
+name = "heed"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
+checksum = "269c7486ed6def5d7b59a427cec3e87b4d4dd4381d01e21c8c9f2d3985688392"
 dependencies = [
+ "bytemuck",
+ "byteorder",
+ "heed-traits",
+ "heed-types",
  "libc",
+ "lmdb-rkv-sys",
+ "once_cell",
+ "page_size",
+ "serde",
+ "synchronoise",
+ "url",
+]
+
+[[package]]
+name = "heed-traits"
+version = "0.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a53a94e5b2fd60417e83ffdfe136c39afacff0d4ac1d8d01cd66928ac610e1a2"
+
+[[package]]
+name = "heed-types"
+version = "0.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9a6cf0a6952fcedc992602d5cddd1e3fff091fbe87d38636e3ec23a31f32acbd"
+dependencies = [
+ "bincode",
+ "bytemuck",
+ "byteorder",
+ "heed-traits",
+ "serde",
+ "serde_json",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
+version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
+checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.1"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+checksum = "379dada1584ad501b383485dd706b8afb7a70fcbc7f4da7d780638a5a6124a60"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
-name = "hmac"
-version = "0.11.0"
+name = "home"
+version = "0.5.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a2a2320eb7ec0ebe8da8f744d7812d9fc4cb4d09344ac01898dbcb6a20ae69b"
+checksum = "e3d1354bf6b7235cb4a0576c2619fd4ed18183f689b12b006a0ee7329eeff9a5"
 dependencies = [
- "crypto-mac",
- "digest 0.9.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "http"
-version = "0.2.9"
+version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
+checksum = "8947b1a6fad4393052c7ba1f4cd97bed3e953a95c79c92ad9b051a04611d9fbb"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
@@ -1424,20 +1452,20 @@
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
 name = "http-body"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d5f38f16d184e36f2408a55281cd658ecbd3ca05cce6d6510a176eca393e26d1"
+checksum = "7ceab25649e9960c0311ea418d17bee82c0dcec1bd053b5f9a66e265a693bed2"
 dependencies = [
  "bytes",
- "http 0.2.9",
+ "http 0.2.11",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "http-body"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1464,17 +1492,17 @@
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
 
 [[package]]
 name = "httpdate"
-version = "1.0.2"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4a1e36c821dbe04574f602848a19f742f4fb3c98d40449f11bcad18d6b17421"
+checksum = "df3b46402a9d5adb4c86a0cf463f42e19994e3ee891101b1841f30a545cb49a9"
 
 [[package]]
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
@@ -1484,56 +1512,57 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
- "h2 0.3.23",
- "http 0.2.9",
- "http-body 0.4.5",
+ "h2 0.3.24",
+ "http 0.2.11",
+ "http-body 0.4.6",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
- "socket2 0.5.5",
+ "socket2",
  "tokio",
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
 name = "hyper"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5aa53871fc917b1a9ed87b683a5d86db645e23acb32c2e0785a353e522fb75"
+checksum = "186548d73ac615b32a73aafe38fb4f56c0d340e110e5a200bcadbaf2e199263a"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-util",
  "h2 0.4.2",
  "http 1.0.0",
  "http-body 1.0.0",
  "httparse",
  "itoa",
  "pin-project-lite",
+ "smallvec",
  "tokio",
  "want",
 ]
 
 [[package]]
 name = "hyper-rustls"
 version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0bea761b46ae2b24eb4aef630d8d1c398157b6fc29e6350ecf090a0b70c952c"
 dependencies = [
  "futures-util",
  "http 1.0.0",
- "hyper 1.1.0",
+ "hyper 1.2.0",
  "hyper-util",
  "log",
  "rustls 0.22.2",
  "rustls-native-certs 0.7.0",
  "rustls-pki-types",
  "tokio",
  "tokio-rustls 0.25.0",
@@ -1563,87 +1592,86 @@
  "native-tls",
  "tokio",
  "tokio-native-tls",
 ]
 
 [[package]]
 name = "hyper-util"
-version = "0.1.2"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdea9aac0dbe5a9240d68cfd9501e2db94222c6dc06843e06640b9e07f0fdc67"
+checksum = "ca38ef113da30126bbff9cd1705f9273e15d45498615d138b0c20279ac7a76aa"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-util",
  "http 1.0.0",
  "http-body 1.0.0",
- "hyper 1.1.0",
+ "hyper 1.2.0",
  "pin-project-lite",
- "socket2 0.5.5",
+ "socket2",
  "tokio",
  "tower",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.54"
+version = "0.1.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c17cc76786e99f8d2f055c11159e7f0091c42474dcc3189fbab96072e873e6d"
+checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
- "windows",
+ "windows-core",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
-version = "0.1.1"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
- "cxx",
- "cxx-build",
+ "cc",
 ]
 
 [[package]]
 name = "ident_case"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
 
 [[package]]
 name = "idna"
-version = "0.3.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
+checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.1.0"
+version = "2.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d530e1a18b1cb4c484e6e34556a0d948706958449fca0cab753d649f2bce3d1f"
+checksum = "233cf39063f058ea2caae4091bf4a3ef70a653afbc026f5c4a4135d114e3c177"
 dependencies = [
  "equivalent",
  "hashbrown 0.14.3",
 ]
 
 [[package]]
 name = "indoc"
@@ -1669,29 +1697,18 @@
 [[package]]
 name = "integer-encoding"
 version = "3.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8bb03732005da905c88227371639bf1ad885cc712789c011c31c5fb3ab3ccf02"
 
 [[package]]
-name = "io-lifetimes"
-version = "1.0.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09270fd4fa1111bc614ed2246c7ef56239a3063d5be0d1ec3b589c505d400aeb"
-dependencies = [
- "hermit-abi 0.3.1",
- "libc",
- "windows-sys 0.45.0",
-]
-
-[[package]]
 name = "ipnet"
-version = "2.7.1"
+version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30e22bd8629359895450b59ea7a776c850561b96a3b1d31321c1949d9e6c9146"
+checksum = "8f518f335dce6725a761382244631d86cf0ccb2863413590b31338feb467f9c3"
 
 [[package]]
 name = "is_executable"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fa9acdc6d67b75e626ad644734e8bc6df893d9cd2a834129065d3dd6158ea9c8"
 dependencies = [
@@ -1704,33 +1721,33 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
-name = "itoa"
-version = "1.0.6"
+name = "itertools"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
+dependencies = [
+ "either",
+]
 
 [[package]]
-name = "jobserver"
-version = "0.1.26"
+name = "itoa"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
-dependencies = [
- "libc",
-]
+checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
 
 [[package]]
 name = "js-sys"
-version = "0.3.61"
+version = "0.3.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
+checksum = "406cda4b368d531c842222cf9d2600a9a4acce8d29423695379c6868a143a9ee"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "json5"
 version = "0.4.1"
@@ -1740,25 +1757,25 @@
  "pest",
  "pest_derive",
  "serde",
 ]
 
 [[package]]
 name = "keccak"
-version = "0.1.3"
+version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3afef3b6eff9ce9d8ff9b3601125eec7f0c8cbac7abd14f355d053fa56c98768"
+checksum = "ecc2af9a1119c51f12a14607e783cb977bde58bc069ff0c3da1095e635d70654"
 dependencies = [
  "cpufeatures",
 ]
 
 [[package]]
 name = "lazy"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "lazy_static",
  "tokio",
  "tracing",
  "xet_error",
 ]
 
@@ -1775,111 +1792,129 @@
 checksum = "723558ab8acaa07cb831b424cd164b587ddc1648b34748a30953c404e9a4a65b"
 dependencies = [
  "cfg-if 0.1.10",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.152"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13e3bf6590cbc649f4d1a3eefc9d5d6eb746f5200ffb04e5e142700b8faa56e7"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libgit2-sys"
-version = "0.13.5+1.4.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "51e5ea06c26926f1002dd553fded6cfcdc9784c1f60feeb58368b4d9b07b6dba"
+version = "0.16.2+1.7.2"
+source = "git+https://github.com/xetdata/git2-rs#dfffd3d1eb9e87a9e7e98b24d0a0f54db664cbcc"
 dependencies = [
  "cc",
  "libc",
  "libssh2-sys",
  "libz-sys",
  "openssl-sys",
  "pkg-config",
 ]
 
 [[package]]
 name = "libmagic"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "anyhow",
  "phf",
  "serde",
  "serde_json",
  "tracing",
  "tracing-attributes",
  "tracing-subscriber",
 ]
 
 [[package]]
+name = "libredox"
+version = "0.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "85c833ca1e66078851dba29046874e38f08b2c883700aa29a03ddd3b23814ee8"
+dependencies = [
+ "bitflags 2.4.2",
+ "libc",
+ "redox_syscall 0.4.1",
+]
+
+[[package]]
 name = "libssh2-sys"
-version = "0.2.23"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b094a36eb4b8b8c8a7b4b8ae43b2944502be3e59cd87687595cf6b0a71b3f4ca"
+checksum = "2dc8a030b787e2119a731f1951d6a773e2280c660f8ec4b0f5e1505a386e71ee"
 dependencies = [
  "cc",
  "libc",
  "libz-sys",
  "openssl-sys",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
 name = "libz-sys"
-version = "1.1.8"
+version = "1.1.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9702761c3935f8cc2f101793272e202c72b99da8f4224a19ddcf1279a6450bbf"
+checksum = "037731f5d3aaa87a5675e895b63ddff1a87624bc29f77004ea829809654e48f6"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
 name = "link-cplusplus"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
+checksum = "9d240c6f7e1ba3a28b0249f774e6a9dd0175054b52dfbb61b16eb8505c3785c9"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.1.4"
+version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f051f77a7c8e6957c0696eac88f26b0117e54f52d3fc682ab19397a8812846a4"
+checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
+
+[[package]]
+name = "lmdb-rkv-sys"
+version = "0.11.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "61b9ce6b3be08acefa3003c57b7565377432a89ec24476bbe72e11d101f852fe"
+dependencies = [
+ "cc",
+ "libc",
+ "pkg-config",
+]
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if 1.0.0",
-]
+checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
 
 [[package]]
 name = "lru"
 version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999beba7b6e8345721bd280141ed958096a2e4abdf74f67ff4ce49b4b54e47a"
 dependencies = [
@@ -1898,34 +1933,23 @@
 [[package]]
 name = "matchit"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e7465ac9959cc2b1404e8e2367b43684a6d13790fe23056cc8c6c5a6b7bcb94"
 
 [[package]]
-name = "md-5"
-version = "0.9.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b5a279bb9607f9f53c22d496eade00d138d1bdcccd07d74650387cf94942a15"
-dependencies = [
- "block-buffer 0.9.0",
- "digest 0.9.0",
- "opaque-debug",
-]
-
-[[package]]
 name = "mdb_shard"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "anyhow",
  "async-scoped",
  "async-trait",
  "binary-heap-plus",
- "clap 3.2.23",
+ "clap 3.2.25",
  "lazy_static",
  "merkledb",
  "merklehash",
  "more-asserts",
  "rand 0.8.5",
  "regex",
  "serde",
@@ -1935,40 +1959,40 @@
  "tracing",
  "uuid",
  "xet_error",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.5.0"
+version = "2.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
+checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
 
 [[package]]
 name = "memoffset"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "merkledb"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "async-trait",
  "bincode",
- "bitflags",
+ "bitflags 1.3.2",
  "blake3",
- "clap 3.2.23",
+ "clap 3.2.25",
  "futures",
  "gearhash",
- "itertools",
+ "itertools 0.10.5",
  "lazy_static",
  "merklehash",
  "parutils",
  "rand 0.8.5",
  "rand_chacha",
  "rand_core 0.6.4",
  "rayon",
@@ -1981,19 +2005,20 @@
  "tracing",
  "walkdir",
  "xet_error",
 ]
 
 [[package]]
 name = "merklehash"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "blake3",
  "generic-array",
+ "heed",
  "rand 0.8.5",
  "rand_chacha",
  "rand_core 0.6.4",
  "safe-transmute",
  "serde",
  "sha3",
  "structopt",
@@ -2008,62 +2033,71 @@
 [[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
+name = "miniz_oxide"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
+dependencies = [
+ "adler",
+]
+
+[[package]]
 name = "mio"
-version = "0.8.6"
+version = "0.8.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
+checksum = "8f3d0b296e374a4e6f3c7b0a1f5a51d748a0d34c85e7dc48fc3fa9a87657fe09"
 dependencies = [
  "libc",
  "log",
- "wasi 0.11.0+wasi-snapshot-preview1",
- "windows-sys 0.45.0",
+ "wasi",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "mockall"
-version = "0.11.3"
+version = "0.11.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50e4a1c770583dac7ab5e2f6c139153b783a53a1bbee9729613f193e59828326"
+checksum = "4c84490118f2ee2d74570d114f3d0493cbf02790df303d2707606c3e14e07c96"
 dependencies = [
  "cfg-if 1.0.0",
  "downcast",
  "fragile",
  "lazy_static",
  "mockall_derive",
  "predicates",
  "predicates-tree",
 ]
 
 [[package]]
 name = "mockall_derive"
-version = "0.11.3"
+version = "0.11.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "832663583d5fa284ca8810bf7015e46c9fff9622d3cf34bd1eea5003fec06dd0"
+checksum = "22ce75669015c4f47b289fd4d4f56e894e4c96003ffdf3ac51313126f94c6cbb"
 dependencies = [
  "cfg-if 1.0.0",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "mockall_double"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae71c7bb287375187c775cf82e2dcf1bef3388aaf58f0789a77f9c7ab28466f6"
+checksum = "f1ca96e5ac35256ae3e13536edd39b172b88f41615e1d7b653c8ad24524113e8"
 dependencies = [
  "cfg-if 1.0.0",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "more-asserts"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fafa6961cabd9c63bcd77a45d7e3b7f3b552b70417831fb0f56db717e72407e"
@@ -2112,22 +2146,21 @@
  "tracing",
  "tracing-attributes",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "nix"
-version = "0.26.2"
+version = "0.27.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfdda3d196821d6af13126e40375cdf7da646a96114af134d5f417a9a1dc8e1a"
+checksum = "2eb04e9c688eff1c89d72b407f168cf79bb9e867a9d3323ed6c01519eb9cc053"
 dependencies = [
- "bitflags",
+ "bitflags 2.4.2",
  "cfg-if 1.0.0",
  "libc",
- "static_assertions",
 ]
 
 [[package]]
 name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
@@ -2146,17 +2179,17 @@
 name = "normalize-path"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5c11b7fa387f3c9874e60670ac6d009cefc5ffa8c23437137a9998c0a154e77"
 
 [[package]]
 name = "ntapi"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc51db7b362b205941f71232e56c625156eb9a929f8cf74a428fd5bc094a4afc"
+checksum = "e8a3895c6391c39d7fe7ebc444a87eb2991b2a0bc718fdabd071eec617fc68e4"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "nu-ansi-term"
 version = "0.46.0"
@@ -2164,113 +2197,117 @@
 checksum = "77a8165726e8236064dbb45459242600304b42a5ea24ee2948e18e023bf7ba84"
 dependencies = [
  "overload",
  "winapi",
 ]
 
 [[package]]
+name = "num-conv"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "51d515d32fb182ee37cda2ccdcb92950d6a3c2893aa280e540671c2cd0f3b1d9"
+
+[[package]]
 name = "num-derive"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "876a53fff98e03a936a674b29568b0e605f06b29372c2489ff4de23f1949743d"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
-name = "num-integer"
-version = "0.1.45"
+name = "num-traits"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
- "num-traits",
 ]
 
 [[package]]
-name = "num-traits"
-version = "0.2.15"
+name = "num_cpus"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "autocfg",
+ "hermit-abi 0.3.8",
+ "libc",
 ]
 
 [[package]]
-name = "num_cpus"
-version = "1.15.0"
+name = "object"
+version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
- "hermit-abi 0.2.6",
- "libc",
+ "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "opaque-debug"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "624a8340c38c1b80fd549087862da4ba43e08858af025b236e509b6649fc13d5"
 
 [[package]]
 name = "openssl"
-version = "0.10.47"
+version = "0.10.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8b277f87dacc05a6b709965d1cbafac4649d6ce9f3ce9ceb88508b5666dfec9"
+checksum = "95a0481286a310808298130d22dd1fef0fa571e05a8f44ec801801e84b216b1f"
 dependencies = [
- "bitflags",
+ "bitflags 2.4.2",
  "cfg-if 1.0.0",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
 
 [[package]]
 name = "openssl-macros"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b501e44f11665960c7e7fcf062c7d96a14ade4aa98116c004b2e37b5be7d736c"
+checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-src"
-version = "111.25.2+1.1.1t"
+version = "300.2.3+3.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "320708a054ad9b3bf314688b5db87cf4d6683d64cfc835e2337924ae62bf4431"
+checksum = "5cff92b6f71555b61bb9315f7c64da3ca43d87531622120fea0195fc761b4843"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.82"
+version = "0.9.101"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a95792af3c4e0153c3914df2261bedd30a98476f94dc892b67dfe1d89d433a04"
+checksum = "dda2b0f344e78efc2facf7d195d098df0dd72151b26ab98da807afc26c198dff"
 dependencies = [
- "autocfg",
  "cc",
  "libc",
  "openssl-src",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -2299,15 +2336,15 @@
 name = "opentelemetry-http"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "449048140ee61e28f57abe6e9975eedc1f3a29855c7407bd6c12b18578863379"
 dependencies = [
  "async-trait",
  "bytes",
- "http 0.2.9",
+ "http 0.2.11",
  "opentelemetry",
 ]
 
 [[package]]
 name = "opentelemetry-jaeger"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2348,29 +2385,39 @@
 dependencies = [
  "dlv-list",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "os_str_bytes"
-version = "6.5.0"
+version = "6.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ceedf44fb00f2d1984b0bc98102627ce622e083e49a5bacdb3e514fa4238e267"
+checksum = "e2355d85b9a3786f481747ced0e0ff2ba35213a1f9bd406ed906554d7af805a1"
 
 [[package]]
 name = "overload"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
+name = "page_size"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eebde548fbbf1ea81a99b128872779c437752fb99f217c45245e1a61dcd9edcd"
+dependencies = [
+ "libc",
+ "winapi",
+]
+
+[[package]]
 name = "papergrid"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fdfe703c51ddc52887ad78fc69cd2ea78d895ffcd6e955c9d03566db8ab5bb1"
+checksum = "ae7891b22598926e4398790c8fe6447930c72a67d36d983a49d6ce682ce83290"
 dependencies = [
  "bytecount",
  "fnv",
  "unicode-width",
 ]
 
 [[package]]
@@ -2387,48 +2434,48 @@
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
- "parking_lot_core 0.9.7",
+ "parking_lot_core 0.9.9",
 ]
 
 [[package]]
 name = "parking_lot_core"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a2cfe6f0ad2bfc16aefa463b497d5c7a5ecd44a23efa72aa342d90177356dc"
 dependencies = [
  "cfg-if 1.0.0",
  "instant",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "smallvec",
  "winapi",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if 1.0.0",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.4.1",
  "smallvec",
- "windows-sys 0.45.0",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "parutils"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "anyhow",
  "async-scoped",
  "async-trait",
  "deadqueue",
  "futures",
  "len-trait",
@@ -2452,70 +2499,71 @@
  "crossbeam-channel",
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pest"
-version = "2.5.6"
+version = "2.7.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cbd939b234e95d72bc393d51788aec68aeeb5d51e748ca08ff3aad58cb722f7"
+checksum = "219c0dcc30b6a27553f9cc242972b67f75b60eb0db71f0b5462f38b058c41546"
 dependencies = [
+ "memchr",
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "pest_derive"
-version = "2.5.6"
+version = "2.7.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a81186863f3d0a27340815be8f2078dd8050b14cd71913db9fbda795e5f707d7"
+checksum = "22e1288dbd7786462961e69bfd4df7848c1e37e8b74303dbdab82c3a9cdd2809"
 dependencies = [
  "pest",
  "pest_generator",
 ]
 
 [[package]]
 name = "pest_generator"
-version = "2.5.6"
+version = "2.7.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75a1ef20bf3193c15ac345acb32e26b3dc3223aff4d77ae4fc5359567683796b"
+checksum = "1381c29a877c6d34b8c176e734f35d7f7f5b3adaefe940cb4d1bb7af94678e2e"
 dependencies = [
  "pest",
  "pest_meta",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "pest_meta"
-version = "2.5.6"
+version = "2.7.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5e3b284b1f13a20dc5ebc90aff59a51b8d7137c221131b52a7260c08cbc1cc80"
+checksum = "d0934d6907f148c22a3acbda520c7eed243ad7487a30f51f6ce52b58b7077a8a"
 dependencies = [
  "once_cell",
  "pest",
- "sha2 0.10.6",
+ "sha2",
 ]
 
 [[package]]
 name = "petgraph"
-version = "0.6.3"
+version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dd7d28ee937e54fe3080c91faa1c3a46c06de6252988a7f4592ba2310ef22a4"
+checksum = "e1d3afd2628e69da2be385eb6f2fd57c8ac7977ceeff6dc166ff1657b0e386a9"
 dependencies = [
  "fixedbitset",
- "indexmap 1.9.2",
+ "indexmap 2.2.3",
 ]
 
 [[package]]
 name = "phf"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ade2d8b8f33c7333b51bcf0428d37e217e9f32192ae4772156f65063b8ce03dc"
@@ -2540,73 +2588,69 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3444646e286606587e49f3bcf1679b8cef1dc2c5ecc29ddacaffc305180d464b"
 dependencies = [
  "phf_generator",
  "phf_shared",
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "phf_shared"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
 name = "pin-project"
-version = "1.0.12"
+version = "1.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad29a609b6bcd67fee905812e544992d216af9d755757c05ed2d0e15a74c6ecc"
+checksum = "0302c4a0442c456bd56f841aee5c3bfd17967563f6fadc9ceb9f9c23cf3807e0"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.0.12"
+version = "1.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "069bdb1e05adc7a8990dce9cc75370895fbe4e3d58b9b73bf1aee56359344a55"
+checksum = "266c042b60c9c76b8d53061e52b2e0d1116abc57cefc8c5cd671619a56ac3690"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkg-config"
-version = "0.3.26"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
+checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
-name = "pointer_file"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
-dependencies = [
- "merklehash",
- "toml",
- "tracing",
-]
+name = "powerfmt"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
@@ -2614,15 +2658,15 @@
 name = "predicates"
 version = "2.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "59230a63c37f3e18569bdb90e4a89cbf5bf8b06fea0b84e65ea10cc4df47addd"
 dependencies = [
  "difflib",
  "float-cmp",
- "itertools",
+ "itertools 0.10.5",
  "normalize-line-endings",
  "predicates-core",
  "regex",
 ]
 
 [[package]]
 name = "predicates-core"
@@ -2638,20 +2682,20 @@
 dependencies = [
  "predicates-core",
  "termtree",
 ]
 
 [[package]]
 name = "prettyplease"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae005bd773ab59b4725093fd7df83fd7892f7d8eafb48dbd7de6e024e4215f9d"
+checksum = "a41cf62165e97c7f814d2221421dbb9afcbcdb0a88068e5ea206e19951c2cbb5"
 dependencies = [
  "proc-macro2",
- "syn 2.0.38",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
@@ -2671,32 +2715,26 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
-name = "proc-macro-hack"
-version = "0.5.20+deprecated"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
-
-[[package]]
 name = "proc-macro2"
-version = "1.0.68"
+version = "1.0.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b1106fec09662ec6dd98ccac0f81cef56984d0b49f75c92d8cbad76e20c005c"
+checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "progress_reporting"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "atty",
  "crossterm",
  "more-asserts",
  "tokio",
  "tracing",
  "utils",
@@ -2715,16 +2753,16 @@
  "parking_lot 0.12.1",
  "protobuf",
  "thiserror",
 ]
 
 [[package]]
 name = "prometheus_dict_encoder"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "memchr",
  "prometheus",
  "tracing",
 ]
 
 [[package]]
@@ -2741,39 +2779,39 @@
 name = "prost-build"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c55e02e35260070b6f716a2423c2ff1c3bb1642ddca6f99e1f26d06268a0e2d2"
 dependencies = [
  "bytes",
  "heck 0.4.1",
- "itertools",
+ "itertools 0.11.0",
  "log",
  "multimap",
  "once_cell",
  "petgraph",
  "prettyplease",
  "prost",
  "prost-types",
  "regex",
- "syn 2.0.38",
+ "syn 2.0.51",
  "tempfile",
  "which",
 ]
 
 [[package]]
 name = "prost-derive"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "efb6c9a1dd1def8e2124d17e83a20af56f1570d6c2d2bd9e266ccb768df3840e"
 dependencies = [
  "anyhow",
- "itertools",
+ "itertools 0.11.0",
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "prost-types"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "193898f59edcf43c26227dcd4c8427f00d99d61e95dcde58dabd49fa291d470e"
@@ -2785,17 +2823,17 @@
 name = "protobuf"
 version = "2.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "106dd99e98437432fed6519dedecfade6a06a73bb7b2a1e019fdd2bee5778d94"
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if 1.0.0",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot 0.12.1",
  "pyo3-build-config",
@@ -2827,92 +2865,91 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "python3-dll-a",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "python3-dll-a"
-version = "0.2.7"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "212d74540270e3a22eed5f0d4bbc0765dff20958d694e9d4f5ebe6e22778c422"
+checksum = "d5f07cd4412be8fa09a721d40007c483981bbe072cd6a21f2e83e04ec8f8343f"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pyxet"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
  "anyhow",
  "cc",
  "futures",
  "gitxetcore",
  "lazy_static",
  "libc",
  "progress_reporting",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-build-config",
  "tempfile",
- "thiserror",
  "tokio",
  "tracing",
  "url",
  "xetblob",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.33"
+version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
+checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.4.6"
@@ -2969,32 +3006,30 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.7.0"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
+checksum = "e4963ed1bc86e4f3ee217022bd855b297cef07fb9eac5dfa1f788b220b49b3bd"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.11.0"
+version = "1.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
+checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
 dependencies = [
- "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
- "num_cpus",
 ]
 
 [[package]]
 name = "rdrand"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "678054eb77286b51581ba43620cc911abf02758c91f93f479767aed0f90458b2"
@@ -3004,108 +3039,120 @@
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
+]
+
+[[package]]
+name = "redox_syscall"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+dependencies = [
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "redox_users"
-version = "0.4.3"
+version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
+checksum = "a18479200779601e498ada4e8c1e1f50e3ee19deb0259c25825a98b5603b2cb4"
 dependencies = [
  "getrandom",
- "redox_syscall",
+ "libredox",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.9.4"
+version = "1.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12de2eff854e5fa4b1295edd650e227e9d8fb0c9e90b12e7f36d6a6811791a29"
+checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-automata 0.3.7",
- "regex-syntax 0.7.5",
+ "regex-automata 0.4.5",
+ "regex-syntax 0.8.2",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 dependencies = [
  "regex-syntax 0.6.29",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.3.7"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49530408a136e16e5b486e883fbb6ba058e8e4e8ae6621a77b048b314336e629"
+checksum = "5bb987efffd3c6d0d8f5f89510bb458559eab11e4f869acb20bf845e016259cd"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax 0.7.5",
+ "regex-syntax 0.8.2",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.5"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb5fb1acd8a1a18b3dd5be62d25485eb770e05afb408a9627d14d451bae12da"
+checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
 
 [[package]]
 name = "remove_dir_all"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "reqwest"
-version = "0.11.15"
+version = "0.11.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0ba30cc2c0cd02af1222ed216ba659cdb2f879dfe3181852fe7c50b1d0005949"
+checksum = "c6920094eb85afde5e4a138be3f2de8bbdf28000f0029e72c45025a56b042251"
 dependencies = [
- "base64 0.21.0",
+ "base64 0.21.7",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
- "h2 0.3.23",
- "http 0.2.9",
- "http-body 0.4.5",
+ "h2 0.3.24",
+ "http 0.2.11",
+ "http-body 0.4.6",
  "hyper 0.14.28",
  "hyper-tls",
  "ipnet",
  "js-sys",
  "log",
  "mime",
  "native-tls",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
+ "rustls-pemfile 1.0.4",
  "serde",
  "serde_json",
  "serde_urlencoded",
+ "sync_wrapper",
+ "system-configuration",
  "tokio",
  "tokio-native-tls",
  "tower-service",
  "url",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
@@ -3117,16 +3164,16 @@
 name = "retain_mut"
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4389f1d5789befaf6029ebd9f7dac4af7f7e3d61b69d4f30e2ac02b57e7712b0"
 
 [[package]]
 name = "retry_strategy"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "tokio-retry",
 ]
 
 [[package]]
 name = "ring"
 version = "0.16.20"
@@ -3140,191 +3187,106 @@
  "untrusted 0.7.1",
  "web-sys",
  "winapi",
 ]
 
 [[package]]
 name = "ring"
-version = "0.17.3"
+version = "0.17.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9babe80d5c16becf6594aa32ad2be8fe08498e7ae60b77de8df700e67f191d7e"
+checksum = "c17fa4cb658e3583423e915b9f3acc01cceaee1860e33d59ebae66adc3a2dc0d"
 dependencies = [
  "cc",
+ "cfg-if 1.0.0",
  "getrandom",
  "libc",
  "spin 0.9.8",
  "untrusted 0.9.0",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "ron"
 version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "86018df177b1beef6c7c8ef949969c4f7cb9a9344181b92486b23c79995bdaa4"
 dependencies = [
  "base64 0.13.1",
- "bitflags",
+ "bitflags 1.3.2",
  "serde",
 ]
 
 [[package]]
 name = "ron"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "88073939a61e5b7680558e6be56b419e208420c2adb92be54921fa6b72283f1a"
 dependencies = [
  "base64 0.13.1",
- "bitflags",
- "serde",
-]
-
-[[package]]
-name = "rusoto_core"
-version = "0.47.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b4f000e8934c1b4f70adde180056812e7ea6b1a247952db8ee98c94cd3116cc"
-dependencies = [
- "async-trait",
- "base64 0.13.1",
- "bytes",
- "crc32fast",
- "futures",
- "http 0.2.9",
- "hyper 0.14.28",
- "hyper-tls",
- "lazy_static",
- "log",
- "rusoto_credential",
- "rusoto_signature",
- "rustc_version",
- "serde",
- "serde_json",
- "tokio",
- "xml-rs",
-]
-
-[[package]]
-name = "rusoto_credential"
-version = "0.47.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a46b67db7bb66f5541e44db22b0a02fed59c9603e146db3a9e633272d3bac2f"
-dependencies = [
- "async-trait",
- "chrono",
- "dirs-next",
- "futures",
- "hyper 0.14.28",
+ "bitflags 1.3.2",
  "serde",
- "serde_json",
- "shlex",
- "tokio",
- "zeroize",
-]
-
-[[package]]
-name = "rusoto_s3"
-version = "0.47.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "048c2fe811a823ad5a9acc976e8bf4f1d910df719dcf44b15c3e96c5b7a51027"
-dependencies = [
- "async-trait",
- "bytes",
- "futures",
- "rusoto_core",
- "xml-rs",
-]
-
-[[package]]
-name = "rusoto_signature"
-version = "0.47.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6264e93384b90a747758bcc82079711eacf2e755c3a8b5091687b5349d870bcc"
-dependencies = [
- "base64 0.13.1",
- "bytes",
- "chrono",
- "digest 0.9.0",
- "futures",
- "hex",
- "hmac",
- "http 0.2.9",
- "hyper 0.14.28",
- "log",
- "md-5",
- "percent-encoding",
- "pin-project-lite",
- "rusoto_credential",
- "rustc_version",
- "serde",
- "sha2 0.9.9",
- "tokio",
 ]
 
 [[package]]
 name = "rust-ini"
 version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f6d5f2436026b4f6e79dc829837d467cc7e9a55ee40e750d716713540715a2df"
 dependencies = [
  "cfg-if 1.0.0",
  "ordered-multimap",
 ]
 
 [[package]]
-name = "rustc-hash"
-version = "1.1.0"
+name = "rustc-demangle"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
-name = "rustc_version"
-version = "0.4.0"
+name = "rustc-hash"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
-dependencies = [
- "semver",
-]
+checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.36.11"
+version = "0.38.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db4165c9963ab29e422d6c26fbc1d37f15bace6b2810221f9d925023480fcf0e"
+checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
 dependencies = [
- "bitflags",
+ "bitflags 2.4.2",
  "errno",
- "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.45.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls"
 version = "0.21.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
 dependencies = [
  "log",
- "ring 0.17.3",
+ "ring 0.17.8",
  "rustls-webpki 0.101.7",
  "sct",
 ]
 
 [[package]]
 name = "rustls"
 version = "0.22.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e87c9956bd9807afa1f77e0f7594af32566e830e088a5576d27c5b6f30f49d41"
 dependencies = [
  "log",
- "ring 0.17.3",
+ "ring 0.17.8",
  "rustls-pki-types",
- "rustls-webpki 0.102.1",
+ "rustls-webpki 0.102.2",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rustls-native-certs"
 version = "0.6.3"
@@ -3340,95 +3302,77 @@
 [[package]]
 name = "rustls-native-certs"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f1fb85efa936c42c6d5fc28d2629bb51e4b2f4b8a5211e297d599cc5a093792"
 dependencies = [
  "openssl-probe",
- "rustls-pemfile 2.0.0",
+ "rustls-pemfile 2.1.0",
  "rustls-pki-types",
  "schannel",
  "security-framework",
 ]
 
 [[package]]
 name = "rustls-pemfile"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
 dependencies = [
- "base64 0.21.0",
+ "base64 0.21.7",
 ]
 
 [[package]]
 name = "rustls-pemfile"
-version = "2.0.0"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "35e4980fa29e4c4b212ffb3db068a564cbf560e51d3944b7c88bd8bf5bec64f4"
+checksum = "3c333bb734fcdedcea57de1602543590f545f127dc8b533324318fd492c5c70b"
 dependencies = [
- "base64 0.21.0",
+ "base64 0.21.7",
  "rustls-pki-types",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.1.0"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e9d979b3ce68192e42760c7810125eb6cf2ea10efae545a156063e61f314e2a"
+checksum = "5ede67b28608b4c60685c7d54122d4400d90f62b40caee7700e700380a390fa8"
 
 [[package]]
 name = "rustls-webpki"
 version = "0.101.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
 dependencies = [
- "ring 0.17.3",
+ "ring 0.17.8",
  "untrusted 0.9.0",
 ]
 
 [[package]]
 name = "rustls-webpki"
-version = "0.102.1"
+version = "0.102.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef4ca26037c909dedb327b48c3327d0ba91d3dd3c4e05dad328f210ffb68e95b"
+checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
 dependencies = [
- "ring 0.17.3",
+ "ring 0.17.8",
  "rustls-pki-types",
  "untrusted 0.9.0",
 ]
 
 [[package]]
 name = "rustversion"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
-
-[[package]]
-name = "s3"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
-dependencies = [
- "chrono",
- "more-asserts",
- "parutils",
- "pbr",
- "rusoto_core",
- "rusoto_s3",
- "tokio",
- "tokio-retry",
- "tracing",
- "url",
- "xet_error",
-]
+checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "safe-transmute"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98a01dab6acf992653be49205bdd549f32f17cb2803e8eacf1560bf97259aae8"
 
@@ -3439,97 +3383,91 @@
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "schannel"
-version = "0.1.21"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
+checksum = "fbc91545643bcf3a0bbb6569265615222618bdf33ce4ffbbd13c4bbd4c093534"
 dependencies = [
- "windows-sys 0.42.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "scratch"
-version = "1.0.5"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1792db035ce95be60c3f8853017b3999209281c24e2ba5bc8e59bf97a0c590c1"
+checksum = "a3cf7c11c38cb994f3d40e8a8cde3bbd1f72a435e4c49e85d6553d8312306152"
 
 [[package]]
 name = "sct"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da046153aa2352493d6cb7da4b6e5c0c057d8a1d0a9aa8560baffdd945acd414"
 dependencies = [
- "ring 0.17.3",
+ "ring 0.17.8",
  "untrusted 0.9.0",
 ]
 
 [[package]]
 name = "security-framework"
-version = "2.8.2"
+version = "2.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a332be01508d814fed64bf28f798a146d73792121129962fdf335bb3c49a4254"
+checksum = "05b64fb303737d99b81884b2c63433e9ae28abebe5eb5045dcdd175dc2ecf4de"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.8.0"
+version = "2.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31c9bb296072e961fcbd8853511dd39c2d8be2deb1e17c6860b1d30732b323b4"
+checksum = "e932934257d3b408ed8f30db49d85ea163bfe74961f017f405b025af298f0c7a"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
-name = "semver"
-version = "1.0.17"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
-
-[[package]]
 name = "serde"
-version = "1.0.158"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "771d4d9c4163ee138805e12c710dd365e4f44be8be0503cb1bb9eb989425d9c9"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.158"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e801c1712f48475582b7696ac71e0ca34ebb30e09338425384269d9717c62cad"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.94"
+version = "1.0.114"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c533a59c9d8a93a09c6ab31f0fd5e5f4dd1b8fc9434804029839884765d04ea"
+checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -3564,30 +3502,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "sha2"
-version = "0.9.9"
+version = "0.10.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d58a1e1bf39749807d89cf2d98ac2dfa0ff1cb3faa38fbb64dd88ac8013d800"
-dependencies = [
- "block-buffer 0.9.0",
- "cfg-if 1.0.0",
- "cpufeatures",
- "digest 0.9.0",
- "opaque-debug",
-]
-
-[[package]]
-name = "sha2"
-version = "0.10.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
+checksum = "793db75ad2bcafc3ffa7c68b215fee268f537982cd901d132f89c6343f3a3dc8"
 dependencies = [
  "cfg-if 1.0.0",
  "cpufeatures",
  "digest 0.10.7",
 ]
 
 [[package]]
@@ -3600,28 +3525,30 @@
  "digest 0.9.0",
  "keccak",
  "opaque-debug",
 ]
 
 [[package]]
 name = "shard_client"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "anyhow",
  "async-trait",
  "bincode",
  "bytes",
  "cas_client",
  "clap 2.34.0",
- "http 0.2.9",
+ "heed",
+ "http 0.2.11",
  "hyper 0.14.28",
- "itertools",
+ "itertools 0.10.5",
  "lazy_static",
  "mdb_shard",
+ "merkledb",
  "merklehash",
  "opentelemetry",
  "opentelemetry-http",
  "opentelemetry-jaeger",
  "progress_reporting",
  "prost",
  "retry_strategy",
@@ -3636,41 +3563,35 @@
  "utils",
  "uuid",
  "xet_error",
 ]
 
 [[package]]
 name = "sharded-slab"
-version = "0.1.4"
+version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "900fba806f70c630b0a382d0d825e17a0f19fcd059a2ade1ff237bcddf446b31"
+checksum = "f40ca3c46823713e0d4209592e8d6e826aa57e928f09752619fc696c499637f6"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "shellexpand"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c7e79eddc7b411f9beeaaf2d421de7e7cb3b1ab9eaf1b79704c0e4130cba6b5"
 dependencies = [
  "dirs 2.0.2",
 ]
 
 [[package]]
-name = "shlex"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43b2853a4d09f215c24cc5489c992ce46052d359b5109343cbafbf26bc62f8a3"
-
-[[package]]
 name = "signal-hook"
-version = "0.3.15"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "732768f1176d21d09e076c23a93123d40bba92d50c4058da34d45c8de8e682b9"
+checksum = "8621587d4798caf8eb44879d42e56b9a93ea5dcd315a6487c357130095b62801"
 dependencies = [
  "libc",
  "signal-hook-registry",
 ]
 
 [[package]]
 name = "signal-hook-mio"
@@ -3690,38 +3611,38 @@
 checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "siphasher"
-version = "0.3.10"
+version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
+checksum = "38b58827f4464d87d377d175e90bf58eb00fd8716ff0a62f80356b5e61555d0d"
 
 [[package]]
 name = "slab"
-version = "0.4.8"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
+checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "slog"
 version = "2.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8347046d4ebd943127157b94d63abb990fcf729dc4e9978927fdf4ac3c998d06"
 
 [[package]]
 name = "slog-async"
-version = "2.7.0"
+version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "766c59b252e62a34651412870ff55d8c4e6d04df19b43eecb2703e417b097ffe"
+checksum = "72c8038f898a2c79507940990f05386455b3a317d8f18d4caea7cbc3d5096b84"
 dependencies = [
  "crossbeam-channel",
  "slog",
  "take_mut",
  "thread_local",
 ]
 
@@ -3730,78 +3651,62 @@
 version = "2.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3e1e53f61af1e3c8b852eef0a9dee29008f55d6dd63794f3f12cef786cf0f219"
 dependencies = [
  "serde",
  "serde_json",
  "slog",
- "time 0.3.20",
+ "time",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
 
 [[package]]
 name = "snailquote"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec62a949bda7f15800481a711909f946e1204f2460f89210eaf7f57730f88f86"
 dependencies = [
  "thiserror",
  "unicode_categories",
 ]
 
 [[package]]
 name = "socket2"
-version = "0.4.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
-dependencies = [
- "libc",
- "winapi",
-]
-
-[[package]]
-name = "socket2"
-version = "0.5.5"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
+checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
 dependencies = [
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "sorted-vec"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0047b8207660638866f228b4b4147e98cc8efb190a70cd63d5cb899a4a539a8"
+checksum = "c6734caf0b6f51addd5eeacca12fb39b2c6c14e8d4f3ac42f3a78955c0467458"
 
 [[package]]
 name = "spin"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
 
 [[package]]
 name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 
 [[package]]
-name = "static_assertions"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
-
-[[package]]
 name = "strsim"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ea5119cdb4c55b55d432abb513a0429384878c15dde60cc77b1c99de1a95a6a"
 
 [[package]]
 name = "strsim"
@@ -3848,30 +3753,39 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.38"
+version = "2.0.51"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e96b79aaa137db8f61e26363a0c9b47d8b4ec75da28b7d1d614c2303e232408b"
+checksum = "6ab617d94515e94ae53b8406c628598680aa0c9587474ecbe58188f7b345d66c"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "sync_wrapper"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
 
 [[package]]
+name = "synchronoise"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3dbc01390fc626ce8d1cffe3376ded2b72a11bb70e1c75f404a210e4daa4def2"
+dependencies = [
+ "crossbeam-queue",
+]
+
+[[package]]
 name = "sysinfo"
 version = "0.26.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c18a6156d1f27a9592ee18c1a846ca8dd5c258b7179fc193ae87c74ebb666f5"
 dependencies = [
  "cfg-if 1.0.0",
  "core-foundation-sys",
@@ -3879,18 +3793,39 @@
  "ntapi",
  "once_cell",
  "rayon",
  "winapi",
 ]
 
 [[package]]
+name = "system-configuration"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ba3a3adc5c275d719af8cb4272ea1c4a6d668a777f37e115f6d11ddbc1c8e0e7"
+dependencies = [
+ "bitflags 1.3.2",
+ "core-foundation",
+ "system-configuration-sys",
+]
+
+[[package]]
+name = "system-configuration-sys"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a75fb188eb626b924683e3b95e3a48e63551fcfb51949de2f06a9d91dbee93c9"
+dependencies = [
+ "core-foundation-sys",
+ "libc",
+]
+
+[[package]]
 name = "tabled"
-version = "0.12.0"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da1a2e56bbf7bfdd08aaa7592157a742205459eff774b73bc01809ae2d99dc2a"
+checksum = "0ce69a5028cd9576063ec1f48edb2c75339fd835e6094ef3e05b3a079bf594a6"
 dependencies = [
  "papergrid",
  "tabled_derive",
  "unicode-width",
 ]
 
 [[package]]
@@ -3910,46 +3845,45 @@
 name = "take_mut"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f764005d11ee5f36500a149ace24e00e3da98b0158b3e2d53a7495660d3f4d60"
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tempdir"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "15f2b5fb00ccdf689e0149d1b1b3c03fead81c2b37735d812fa8bddbbf41b6d8"
 dependencies = [
  "rand 0.4.6",
  "remove_dir_all",
 ]
 
 [[package]]
 name = "tempfile"
-version = "3.4.0"
+version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af18f7ae1acd354b992402e9ec5864359d693cd8a79dcbef59f76891701c1e95"
+checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
  "cfg-if 1.0.0",
  "fastrand",
- "redox_syscall",
  "rustix",
- "windows-sys 0.42.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "termcolor"
-version = "1.2.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
+checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "termtree"
 version = "0.4.1"
@@ -3963,43 +3897,43 @@
 checksum = "d326610f408c7a4eb6f51c37c330e496b08506c9457c9d34287ecc38809fb060"
 dependencies = [
  "unicode-width",
 ]
 
 [[package]]
 name = "textwrap"
-version = "0.16.0"
+version = "0.16.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
+checksum = "23d434d3f8967a09480fb04132ebe0a3e088c173e6d0ee7897abbdf4eab0f8b9"
 
 [[package]]
 name = "thiserror"
-version = "1.0.49"
+version = "1.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1177e8c6d7ede7afde3585fd2513e611227efd6481bd78d2e82ba1ce16557ed4"
+checksum = "1e45bcbe8ed29775f228095caf2cd67af7a4ccf756ebff23a306bf3e8b47b24b"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.49"
+version = "1.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10712f02019e9288794769fba95cd6847df9874d49d871d062172f9dd41bc4cc"
+checksum = "a953cb265bef375dae3de6663da4d3804eee9682ea80d8e2542529b73c531c81"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "thread_local"
-version = "1.1.7"
+version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
+checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
 dependencies = [
  "cfg-if 1.0.0",
  "once_cell",
 ]
 
 [[package]]
 name = "threadpool"
@@ -4021,47 +3955,40 @@
  "log",
  "ordered-float",
  "threadpool",
 ]
 
 [[package]]
 name = "time"
-version = "0.1.45"
+version = "0.3.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
-dependencies = [
- "libc",
- "wasi 0.10.0+wasi-snapshot-preview1",
- "winapi",
-]
-
-[[package]]
-name = "time"
-version = "0.3.20"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd0cbfecb4d19b5ea75bb31ad904eb5b9fa13f21079c3b92017ebdf4999a5890"
+checksum = "c8248b6521bb14bc45b4067159b9b6ad792e2d6d754d6c41fb50e29fefe38749"
 dependencies = [
+ "deranged",
  "itoa",
+ "num-conv",
+ "powerfmt",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
-version = "0.1.0"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e153e1f1acaef8acc537e68b44906d2db6436e2b35ac2c6b42640fff91f00fd"
+checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
 
 [[package]]
 name = "time-macros"
-version = "0.2.8"
+version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
+checksum = "7ba3a3ef41e6672a2f0f001392bb5dcd3ff0a9992d618ca761a11c3121547774"
 dependencies = [
+ "num-conv",
  "time-core",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -4074,50 +4001,50 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.27.0"
+version = "1.36.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0de47a4eecbe11f498978a9b29d792f0d2692d1dd003650c24c76510e3bc001"
+checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
 dependencies = [
- "autocfg",
+ "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot 0.12.1",
  "pin-project-lite",
  "signal-hook-registry",
- "socket2 0.4.9",
+ "socket2",
  "tokio-macros",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-io-timeout"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "30b74022ada614a1b4834de765f9bb43877f910cc8ce4be40e89042c9223a8bf"
 dependencies = [
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "2.0.0"
+version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61a573bdc87985e9d6ddeed1b3d864e8a302c847e40d647746df2f1de209d1ce"
+checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -4156,28 +4083,28 @@
  "rustls 0.22.2",
  "rustls-pki-types",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-stream"
-version = "0.1.12"
+version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8fb52b74f05dbf495a8fba459fdc331812b96aa086d9eb78101fa0d4569c3313"
+checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
 dependencies = [
  "futures-core",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.7"
+version = "0.7.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5427d89453009325de0d8f342c9490009f76e999cb7672d77e46267448f7e6b2"
+checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
  "tracing",
@@ -4197,19 +4124,19 @@
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d560933a0de61cf715926b9cac824d4c883c2c43142f787595e48280c40a1d0e"
 dependencies = [
  "async-stream",
  "async-trait",
  "axum",
- "base64 0.21.0",
+ "base64 0.21.7",
  "bytes",
- "h2 0.3.23",
- "http 0.2.9",
- "http-body 0.4.5",
+ "h2 0.3.24",
+ "http 0.2.11",
+ "http-body 0.4.6",
  "hyper 0.14.28",
  "hyper-timeout",
  "percent-encoding",
  "pin-project",
  "prost",
  "rustls 0.21.10",
  "rustls-native-certs 0.6.3",
@@ -4229,26 +4156,26 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d021fc044c18582b9a2408cd0dd05b1596e3ecdb5c4df822bb0183545683889"
 dependencies = [
  "prettyplease",
  "proc-macro2",
  "prost-build",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "tower"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
 dependencies = [
  "futures-core",
  "futures-util",
- "indexmap 1.9.2",
+ "indexmap 1.9.3",
  "pin-project",
  "pin-project-lite",
  "rand 0.8.5",
  "slab",
  "tokio",
  "tokio-util",
  "tower-layer",
@@ -4284,15 +4211,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -4309,34 +4236,45 @@
 dependencies = [
  "pin-project",
  "tracing",
 ]
 
 [[package]]
 name = "tracing-log"
-version = "0.1.3"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "78ddad33d2d10b1ed7eb9d1f518a5674713876e97e5bb9b7345a7984fbb4f922"
+checksum = "f751112709b4e791d8ce53e32c4ed2d353565a795ce84da2285393f41557bdf2"
+dependencies = [
+ "log",
+ "once_cell",
+ "tracing-core",
+]
+
+[[package]]
+name = "tracing-log"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ee855f1f400bd0e5c02d150ae5de3840039a3f54b025156404e34c23c03f47c3"
 dependencies = [
- "lazy_static",
  "log",
+ "once_cell",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-opentelemetry"
 version = "0.17.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fbbe89715c1dbbb790059e2565353978564924ee85017b5fff365c872ff6721f"
 dependencies = [
  "once_cell",
  "opentelemetry",
  "tracing",
  "tracing-core",
- "tracing-log",
+ "tracing-log 0.1.4",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "tracing-serde"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -4344,30 +4282,30 @@
 dependencies = [
  "serde",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-subscriber"
-version = "0.3.16"
+version = "0.3.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6176eae26dd70d0c919749377897b54a9276bd7061339665dd68777926b5a70"
+checksum = "ad0f048c97dbd9faa9b7df56362b8ebcaa52adb06b498c050d2f4e32f90a7a8b"
 dependencies = [
  "matchers",
  "nu-ansi-term",
  "once_cell",
  "regex",
  "serde",
  "serde_json",
  "sharded-slab",
  "smallvec",
  "thread_local",
  "tracing",
  "tracing-core",
- "tracing-log",
+ "tracing-log 0.2.0",
  "tracing-serde",
 ]
 
 [[package]]
 name = "tracing-test"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -4397,62 +4335,62 @@
 checksum = "73eead03a57feec88e556e6be8c3f6c9917688a15f9d410aedee1b6cb276445f"
 dependencies = [
  "unicode-segmentation",
 ]
 
 [[package]]
 name = "try-lock"
-version = "0.2.4"
+version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3528ecfd12c466c6f163363caf2d02a71161dd5e1cc6ae7b34207ea2d42d81ed"
+checksum = "e421abadd41a4225275504ea4d6566923418b7f05506fbc9c0fe86ba7396114b"
 
 [[package]]
 name = "typenum"
-version = "1.16.0"
+version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
+checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
 name = "ucd-trie"
-version = "0.1.5"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e79c4d996edb816c91e4308506774452e55e95c3c9de07b6729e17e15a5ef81"
+checksum = "ed646292ffc8188ef8ea4d1e0e0150fb15a5c2e12ad9b8fc191ae7a8a7f3c4b9"
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.13"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
+checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unicode-segmentation"
-version = "1.10.1"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
+checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
 
 [[package]]
 name = "unicode-width"
-version = "0.1.10"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
+checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
 
 [[package]]
 name = "unicode-xid"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
 
@@ -4478,41 +4416,42 @@
 name = "untrusted"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
 
 [[package]]
 name = "url"
-version = "2.3.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
+checksum = "31e6302e3bb753d46e83516cae55ae196fc0c309407cf11ab35cc51a4c2a4633"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "utils"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "anyhow",
  "chrono",
  "futures",
  "hashbrown 0.12.3",
  "hashring",
  "lazy_static",
  "merklehash",
  "parking_lot 0.11.2",
  "pin-project",
  "prost",
  "prost-types",
  "regex",
  "serde",
+ "tempfile",
  "tokio",
  "tonic",
  "tonic-build",
  "tracing",
  "xet_error",
 ]
 
@@ -4524,17 +4463,17 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.3.3"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
+checksum = "f00cc9702ca12d3c81455259621e676d0f7251cec66a21e98fe2e9a37db93b2a"
 dependencies = [
  "getrandom",
  "rand 0.8.5",
 ]
 
 [[package]]
 name = "valuable"
@@ -4564,148 +4503,129 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
-version = "2.3.3"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
+checksum = "d71d857dc86794ca4c280d616f7da00d2dbfd8cd788846559a6813e6aa4b54ee"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
 name = "want"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ce8a968cb1cd110d136ff8b819a556d6fb6d919363c61534f6860c7eb172ba0"
+checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
 dependencies = [
- "log",
  "try-lock",
 ]
 
 [[package]]
 name = "wasi"
-version = "0.10.0+wasi-snapshot-preview1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a143597ca7c7793eff794def352d41792a93c481eb1042423ff7ff72ba2c31f"
-
-[[package]]
-name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.84"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
+checksum = "c1e124130aee3fb58c5bdd6b639a0509486b0338acaaae0c84a5124b0f588b7f"
 dependencies = [
  "cfg-if 1.0.0",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.84"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
+checksum = "c9e7e1900c352b609c8488ad12639a311045f40a35491fb69ba8c12f758af70b"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.51",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.34"
+version = "0.4.41"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f219e0d211ba40266969f6dbdd90636da12f75bee4fc9d6c23d1260dadb51454"
+checksum = "877b9c3f61ceea0e56331985743b13f3d25c406a7098d45180fb5f09bc19ed97"
 dependencies = [
  "cfg-if 1.0.0",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.84"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
+checksum = "b30af9e2d358182b5c7449424f017eba305ed32a7010509ede96cdc4696c46ed"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.84"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
+checksum = "642f325be6301eb8107a83d12a8ac6c1e1c54345a7ef1a9261962dfefda09e66"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.51",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.84"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
+checksum = "4f186bd2dcf04330886ce82d6f33dd75a7bfcf69ecf5763b89fcde53b6ac9838"
 
 [[package]]
 name = "web-sys"
-version = "0.3.61"
+version = "0.3.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
+checksum = "96565907687f7aceb35bc5fc03770a8a0471d82e479f25832f54a0e3f4b28446"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
-name = "webpki"
-version = "0.22.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed63aea5ce73d0ff405984102c42de94fc55a6b75765d621c65262469b3c9b53"
-dependencies = [
- "ring 0.17.3",
- "untrusted 0.9.0",
-]
-
-[[package]]
 name = "webpki-roots"
-version = "0.22.6"
+version = "0.25.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b6c71e40d7d2c34a5106301fb632274ca37242cd0c9d3e64dbece371a40a2d87"
-dependencies = [
- "webpki",
-]
+checksum = "5f20c57d8d7db6d3b86154206ae5d8fba62dd39573114de97c2cb0578251f8e1"
 
 [[package]]
 name = "which"
-version = "4.4.0"
+version = "4.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2441c784c52b289a054b7201fc93253e288f094e2f4be9058343127c4226a269"
+checksum = "87ba24419a2078cd2b0f2ede2691b6c66d8e47836da3b6db8265ebad47afbfc7"
 dependencies = [
  "either",
- "libc",
+ "home",
  "once_cell",
+ "rustix",
 ]
 
 [[package]]
 name = "whoami"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "22fc3756b8a9133049b26c7f61ab35416c130e8c09b660f5b3958b446f52cc50"
@@ -4728,82 +4648,52 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.5"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70ec6ce85bb158151cae5e5c87f95a8e97d2c0c4b001223f33a334e3ce5de178"
+checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
-name = "windows"
-version = "0.46.0"
+name = "windows-core"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdacb41e6a96a052c6cb63a144f24900236121c6f63f4f8219fef5977ecb0c25"
+checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.42.2",
-]
-
-[[package]]
-name = "windows-sys"
-version = "0.42.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
-dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
-]
-
-[[package]]
-name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets 0.42.2",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets 0.48.5",
 ]
 
 [[package]]
-name = "windows-targets"
-version = "0.42.2"
+name = "windows-sys"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -4814,176 +4704,168 @@
  "windows_i686_msvc 0.48.5",
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
-name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+name = "windows-targets"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+dependencies = [
+ "windows_aarch64_gnullvm 0.52.4",
+ "windows_aarch64_msvc 0.52.4",
+ "windows_i686_gnu 0.52.4",
+ "windows_i686_msvc 0.52.4",
+ "windows_x86_64_gnu 0.52.4",
+ "windows_x86_64_gnullvm 0.52.4",
+ "windows_x86_64_msvc 0.52.4",
+]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
-name = "windows_aarch64_msvc"
-version = "0.42.2"
+name = "windows_aarch64_gnullvm"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
-name = "windows_i686_gnu"
-version = "0.42.2"
+name = "windows_aarch64_msvc"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
-name = "windows_i686_msvc"
-version = "0.42.2"
+name = "windows_i686_gnu"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
-name = "windows_x86_64_gnu"
-version = "0.42.2"
+name = "windows_i686_msvc"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
-name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+name = "windows_x86_64_gnu"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
-name = "windows_x86_64_msvc"
-version = "0.42.2"
+name = "windows_x86_64_gnullvm"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+
+[[package]]
 name = "winreg"
-version = "0.10.1"
+version = "0.50.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
+checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
 dependencies = [
- "winapi",
+ "cfg-if 1.0.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "xet-error-impl"
 version = "1.0.50"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.51",
 ]
 
 [[package]]
 name = "xet_config"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "config",
  "dirs 4.0.0",
  "serde",
  "toml",
  "tracing",
  "xet_error",
 ]
 
 [[package]]
 name = "xet_error"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "lazy_static",
  "xet-error-impl",
 ]
 
 [[package]]
 name = "xetblob"
-version = "0.13.0"
-source = "git+https://github.com/xetdata/xet-core#d26d24900650f4485869bb45fcc0d4a272a6bb3c"
+version = "0.13.2"
+source = "git+https://github.com/xetdata/xet-core#13e8a20fc917b6b7dbc944cfcc14edbfdac52a66"
 dependencies = [
  "anyhow",
- "async-trait",
- "base64 0.13.1",
- "blake3",
- "clap 3.2.23",
- "dirs 4.0.0",
- "git2",
+ "clap 3.2.25",
  "gitxetcore",
- "mdb_shard",
- "merkledb",
- "merklehash",
- "parutils",
- "pointer_file",
- "reqwest",
- "retry_strategy",
- "serde",
- "serde_json",
- "shellexpand",
  "tabled",
- "tempdir",
  "tokio",
- "tracing",
  "url",
- "utils",
 ]
 
 [[package]]
-name = "xml-rs"
-version = "0.8.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2d7d3948613f75c98fd9328cfdcc45acc4d360655289d0a7d4ec931392200a3"
-
-[[package]]
 name = "yaml-rust"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56c1936c4cc7a1c9ab21a1ebb602eb942ba868cbd44a99cb7cdc5892335e1c85"
 dependencies = [
  "linked-hash-map",
 ]
```

### Comparing `pyxet-0.1.8/pyproject.toml` & `pyxet-0.1.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["maturin>=0.14.17,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "pyxet"
-version = "0.1.8"
+version = "0.1.9"
 description = "pyxet is a Python library that provides a lightweight interface for the XetHub platform."
 keywords = [
     "ai",
     "collaboration",
     "data-science",
     "developer-tools",
     "git",
     "s3",
     "machine-learning",
     "reproducibility",
 ]
-license = "BSD-3-Clause"
+license = { text = "BSD-3-Clause"}
 maintainers = [{ name = "XetHub", email = "contact@xethub.com" }]
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
```

### Comparing `pyxet-0.1.8/PKG-INFO` & `pyxet-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxet
-Version: 0.1.8
+Version: 0.1.9
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

