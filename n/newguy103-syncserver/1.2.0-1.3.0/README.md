# Comparing `tmp/newguy103-syncserver-1.2.0.tar.gz` & `tmp/newguy103_syncserver-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newguy103-syncserver-1.2.0.tar", last modified: Thu May 16 06:00:30 2024, max compression
+gzip compressed data, was "newguy103_syncserver-1.3.0.tar", last modified: Tue May 21 06:27:28 2024, max compression
```

## Comparing `newguy103-syncserver-1.2.0.tar` & `newguy103_syncserver-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-05-16 06:00:30.983892 newguy103-syncserver-1.2.0/
--rw-r--r--   0 userc     (1000) userc     (1000)     5011 2024-05-16 06:00:30.983892 newguy103-syncserver-1.2.0/PKG-INFO
--rw-------   0 userc     (1000) userc     (1000)     4529 2024-05-16 05:49:19.000000 newguy103-syncserver-1.2.0/README.md
-drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-05-16 06:00:30.983892 newguy103-syncserver-1.2.0/newguy103_syncserver.egg-info/
--rw-r--r--   0 userc     (1000) userc     (1000)     5011 2024-05-16 06:00:30.000000 newguy103-syncserver-1.2.0/newguy103_syncserver.egg-info/PKG-INFO
--rw-rw-r--   0 userc     (1000) userc     (1000)      532 2024-05-16 06:00:30.000000 newguy103-syncserver-1.2.0/newguy103_syncserver.egg-info/SOURCES.txt
--rw-rw-r--   0 userc     (1000) userc     (1000)        1 2024-05-16 06:00:30.000000 newguy103-syncserver-1.2.0/newguy103_syncserver.egg-info/dependency_links.txt
--rw-rw-r--   0 userc     (1000) userc     (1000)      123 2024-05-16 06:00:30.000000 newguy103-syncserver-1.2.0/newguy103_syncserver.egg-info/entry_points.txt
--rw-rw-r--   0 userc     (1000) userc     (1000)       68 2024-05-16 06:00:30.000000 newguy103-syncserver-1.2.0/newguy103_syncserver.egg-info/requires.txt
--rw-rw-r--   0 userc     (1000) userc     (1000)       11 2024-05-16 06:00:30.000000 newguy103-syncserver-1.2.0/newguy103_syncserver.egg-info/top_level.txt
--rw-rw-r--   0 userc     (1000) userc     (1000)       38 2024-05-16 06:00:30.983892 newguy103-syncserver-1.2.0/setup.cfg
--rw-rw-r--   0 userc     (1000) userc     (1000)     1001 2024-05-16 05:49:47.000000 newguy103-syncserver-1.2.0/setup.py
-drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-05-16 06:00:30.979892 newguy103-syncserver-1.2.0/syncserver/
--rw-rw-r--   0 userc     (1000) userc     (1000)       82 2024-05-16 05:53:40.000000 newguy103-syncserver-1.2.0/syncserver/__init__.py
-drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-05-16 06:00:30.979892 newguy103-syncserver-1.2.0/syncserver/client/
--rw-------   0 userc     (1000) userc     (1000)      212 2024-05-16 05:49:19.000000 newguy103-syncserver-1.2.0/syncserver/client/__init__.py
--rw-rw-r--   0 userc     (1000) userc     (1000)    55359 2024-05-16 05:49:19.000000 newguy103-syncserver-1.2.0/syncserver/client/cui.py
--rw-rw-r--   0 userc     (1000) userc     (1000)    58632 2024-05-16 05:54:38.000000 newguy103-syncserver-1.2.0/syncserver/client/gui.py
--rw-------   0 userc     (1000) userc     (1000)    19711 2024-05-16 05:49:19.000000 newguy103-syncserver-1.2.0/syncserver/client/interface.py
-drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-05-16 06:00:30.983892 newguy103-syncserver-1.2.0/syncserver/server/
--rw-------   0 userc     (1000) userc     (1000)       80 2024-05-16 05:49:19.000000 newguy103-syncserver-1.2.0/syncserver/server/__init__.py
--rw-------   0 userc     (1000) userc     (1000)      445 2024-05-16 05:49:19.000000 newguy103-syncserver-1.2.0/syncserver/server/__main__.py
--rw-------   0 userc     (1000) userc     (1000)    67039 2024-05-16 05:49:19.000000 newguy103-syncserver-1.2.0/syncserver/server/_db.py
--rw-rw-r--   0 userc     (1000) userc     (1000)    43180 2024-05-16 05:54:16.000000 newguy103-syncserver-1.2.0/syncserver/server/_server.py
+drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-05-21 06:27:28.802737 newguy103_syncserver-1.3.0/
+-rw-r--r--   0 userc     (1000) userc     (1000)     5048 2024-05-21 06:27:28.802737 newguy103_syncserver-1.3.0/PKG-INFO
+-rw-------   0 userc     (1000) userc     (1000)     4529 2024-05-21 05:59:03.000000 newguy103_syncserver-1.3.0/README.md
+drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-05-21 06:27:28.802737 newguy103_syncserver-1.3.0/newguy103_syncserver.egg-info/
+-rw-r--r--   0 userc     (1000) userc     (1000)     5048 2024-05-21 06:27:28.000000 newguy103_syncserver-1.3.0/newguy103_syncserver.egg-info/PKG-INFO
+-rw-rw-r--   0 userc     (1000) userc     (1000)      562 2024-05-21 06:27:28.000000 newguy103_syncserver-1.3.0/newguy103_syncserver.egg-info/SOURCES.txt
+-rw-rw-r--   0 userc     (1000) userc     (1000)        1 2024-05-21 06:27:28.000000 newguy103_syncserver-1.3.0/newguy103_syncserver.egg-info/dependency_links.txt
+-rw-rw-r--   0 userc     (1000) userc     (1000)      184 2024-05-21 06:27:28.000000 newguy103_syncserver-1.3.0/newguy103_syncserver.egg-info/entry_points.txt
+-rw-rw-r--   0 userc     (1000) userc     (1000)       54 2024-05-21 06:27:28.000000 newguy103_syncserver-1.3.0/newguy103_syncserver.egg-info/requires.txt
+-rw-rw-r--   0 userc     (1000) userc     (1000)       11 2024-05-21 06:27:28.000000 newguy103_syncserver-1.3.0/newguy103_syncserver.egg-info/top_level.txt
+-rw-rw-r--   0 userc     (1000) userc     (1000)       38 2024-05-21 06:27:28.802737 newguy103_syncserver-1.3.0/setup.cfg
+-rw-rw-r--   0 userc     (1000) userc     (1000)     1111 2024-05-21 06:21:30.000000 newguy103_syncserver-1.3.0/setup.py
+drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-05-21 06:27:28.802737 newguy103_syncserver-1.3.0/syncserver/
+-rw-rw-r--   0 userc     (1000) userc     (1000)       94 2024-05-21 05:58:19.000000 newguy103_syncserver-1.3.0/syncserver/__init__.py
+drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-05-21 06:27:28.802737 newguy103_syncserver-1.3.0/syncserver/client/
+-rw-------   0 userc     (1000) userc     (1000)      212 2024-05-21 05:57:08.000000 newguy103_syncserver-1.3.0/syncserver/client/__init__.py
+-rw-rw-r--   0 userc     (1000) userc     (1000)       67 2024-05-21 05:57:08.000000 newguy103_syncserver-1.3.0/syncserver/client/__main__.py
+-rw-rw-r--   0 userc     (1000) userc     (1000)    55359 2024-05-21 05:57:08.000000 newguy103_syncserver-1.3.0/syncserver/client/cui.py
+-rw-rw-r--   0 userc     (1000) userc     (1000)    58681 2024-05-21 05:58:44.000000 newguy103_syncserver-1.3.0/syncserver/client/gui.py
+-rw-------   0 userc     (1000) userc     (1000)    19710 2024-05-21 05:57:08.000000 newguy103_syncserver-1.3.0/syncserver/client/interface.py
+drwxrwxr-x   0 userc     (1000) userc     (1000)        0 2024-05-21 06:27:28.802737 newguy103_syncserver-1.3.0/syncserver/server/
+-rw-------   0 userc     (1000) userc     (1000)      156 2024-05-21 05:57:08.000000 newguy103_syncserver-1.3.0/syncserver/server/__init__.py
+-rw-------   0 userc     (1000) userc     (1000)       77 2024-05-21 05:57:08.000000 newguy103_syncserver-1.3.0/syncserver/server/__main__.py
+-rw-------   0 userc     (1000) userc     (1000)    78108 2024-05-21 05:57:08.000000 newguy103_syncserver-1.3.0/syncserver/server/_db.py
+-rw-rw-r--   0 userc     (1000) userc     (1000)    44221 2024-05-21 05:58:29.000000 newguy103_syncserver-1.3.0/syncserver/server/_server.py
```

### Comparing `newguy103-syncserver-1.2.0/PKG-INFO` & `newguy103_syncserver-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: newguy103-syncserver
-Version: 1.2.0
+Version: 1.3.0
 Summary: newguy103-syncserver simplifies file synchronization using Flask-based server and client modules.
 Author: NewGuy103
 Author-email: userchouenthusiast@gmail.com
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: cryptography
-Requires-Dist: newguy103-pycrypter
 Requires-Dist: requests
 Requires-Dist: flask
 Requires-Dist: argon2-cffi
 Requires-Dist: msgpack
+Requires-Dist: pyqt5
 
 # newguy103-syncserver
 
 ## Overview
 
 **newguy103-syncserver** is a Python package designed to simplify file synchronization operations through a server-client architecture. The package provides both the server, built on Flask, and a client module for interacting with the server.
```

### Comparing `newguy103-syncserver-1.2.0/README.md` & `newguy103_syncserver-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `newguy103-syncserver-1.2.0/newguy103_syncserver.egg-info/PKG-INFO` & `newguy103_syncserver-1.3.0/newguy103_syncserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: newguy103-syncserver
-Version: 1.2.0
+Version: 1.3.0
 Summary: newguy103-syncserver simplifies file synchronization using Flask-based server and client modules.
 Author: NewGuy103
 Author-email: userchouenthusiast@gmail.com
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: cryptography
-Requires-Dist: newguy103-pycrypter
 Requires-Dist: requests
 Requires-Dist: flask
 Requires-Dist: argon2-cffi
 Requires-Dist: msgpack
+Requires-Dist: pyqt5
 
 # newguy103-syncserver
 
 ## Overview
 
 **newguy103-syncserver** is a Python package designed to simplify file synchronization operations through a server-client architecture. The package provides both the server, built on Flask, and a client module for interacting with the server.
```

### Comparing `newguy103-syncserver-1.2.0/newguy103_syncserver.egg-info/SOURCES.txt` & `newguy103_syncserver-1.3.0/newguy103_syncserver.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 newguy103_syncserver.egg-info/SOURCES.txt
 newguy103_syncserver.egg-info/dependency_links.txt
 newguy103_syncserver.egg-info/entry_points.txt
 newguy103_syncserver.egg-info/requires.txt
 newguy103_syncserver.egg-info/top_level.txt
 syncserver/__init__.py
 syncserver/client/__init__.py
+syncserver/client/__main__.py
 syncserver/client/cui.py
 syncserver/client/gui.py
 syncserver/client/interface.py
 syncserver/server/__init__.py
 syncserver/server/__main__.py
 syncserver/server/_db.py
 syncserver/server/_server.py
```

### Comparing `newguy103-syncserver-1.2.0/setup.py` & `newguy103_syncserver-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from setuptools import setup, find_packages
 
 setup(
     name='newguy103-syncserver',
-    version='1.2.0',
+    version='1.3.0',
     author='NewGuy103',
     author_email='userchouenthusiast@gmail.com',
     description='newguy103-syncserver simplifies file synchronization using Flask-based server and client modules.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'syncserver-server = syncserver.server.__main__:main',
-            'syncserver-server.db = syncserver.server._db:run_cli'
+            'syncserver-server = syncserver.server.__main__:run_simple',
+            'syncserver-server.db = syncserver.server._db:run_cli',
+            'syncserver-client = syncserver.client.__main__:run_gui'
         ]
     },
     install_requires=[
         'cryptography',
-        'newguy103-pycrypter',
         'requests',
         'flask',
         'argon2-cffi',
-        'msgpack'
+        'msgpack',
+        'pyqt5'
     ],
     classifiers=[
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12'
     ],
     include_package_data=True,
     package_data={
         '': ['README.md'],
         'syncserver': ['client/*.py', 'server/*.py'],
-    },
+    }
 )
```

### Comparing `newguy103-syncserver-1.2.0/syncserver/client/cui.py` & `newguy103_syncserver-1.3.0/syncserver/client/cui.py`

 * *Files identical despite different names*

### Comparing `newguy103-syncserver-1.2.0/syncserver/client/gui.py` & `newguy103_syncserver-1.3.0/syncserver/client/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -715,15 +715,15 @@
                 "(DeletedFilesDialog.initUI): Failed to fetch files due to error code [%s] "
                 "with error [%s]", ecode, emsg
             )
             return
         
         for file_path, file_versions in self.deleted_paths.items():
             if not file_versions:
-                logger.info(
+                logger.debug(
                     "(DeletedFilesDialog.initUI): Skipped remote path '%s', "
                     "no deleted file versions available", file_path
                 )
                 continue
 
             self._lw_labels[file_path] = QLabel(f"File: {file_path}")
             self._lw_labels[file_path].setAlignment(Qt.AlignCenter)
@@ -1123,15 +1123,15 @@
 
                 del self._textboxes[key_name]
                 del self._txt_labels[key_name]
         
         self.layout.update()
         for key_name in key_names:
             if key_name in self.key_names:
-                logger.info(
+                logger.debug(
                     "(APIKeyManagerDialog.update_list): Skipped key '%s', already exists in layout",
                     key_name
                 )
                 continue
             
             key_data: list = self.interface.api_keys.get_key_data(key_name=key_name)
             self.key_data[key_name] = key_data
@@ -1658,12 +1658,16 @@
                 del self.list_widgets[dir_path]
                 del self.lw_labels[dir_path]
 
         self.layout.update()
         return 0
 
 
-if __name__ == '__main__':
+def run_gui():
     import sys
     app = QApplication(sys.argv)
-    login = StartLogin()
+    login = StartLogin()  # type: ignore
     sys.exit(app.exec_())
+
+
+if __name__ == '__main__':
+    run_gui()
```

### Comparing `newguy103-syncserver-1.2.0/syncserver/client/interface.py` & `newguy103_syncserver-1.3.0/syncserver/client/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import logging
 import requests
 
 from typing import Literal
 from datetime import datetime
 
-__version__: str = "1.2.0"
+__version__: str = "1.3.0"
 
 logger: logging.Logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
+logger.setLevel(logging.INFO)
 
 formatter: logging.Formatter = logging.Formatter(
     '[syncServer-interface]: [%(asctime)s] - [%(levelname)s] - %(message)s', 
     datefmt='%Y-%m-%d %H:%M:%S'
 )
 
 stream_handler: logging.StreamHandler = logging.StreamHandler()
```

### Comparing `newguy103-syncserver-1.2.0/syncserver/server/_db.py` & `newguy103_syncserver-1.3.0/syncserver/server/_db.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,363 +1,474 @@
 import argparse
 import ast
 import getpass
+
+import copy
 import os
 import sqlite3
 
 import subprocess
 import tempfile
 import uuid
 
 import secrets
 import logging
 
 import argon2  # argon2-cffi
 import cryptography
+import cryptography.exceptions
 import msgpack
 
-from pycrypter import CipherManager  # newguy103-pycrypter
+from cryptography.hazmat.primitives.ciphers.aead import AESGCM
+from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
+from cryptography.hazmat.primitives import hashes
+
 from datetime import datetime
-from typing import BinaryIO, Callable, Generator, Literal, TextIO
+from typing import BinaryIO, Generator, Literal, TextIO
+from contextlib import contextmanager
+
+__version__: str = "1.3.0"
+LOGFILE: str = 'syncServer-serverDB.log'
+
+
+@contextmanager
+def transaction(conn: sqlite3.Connection):
+    try:
+        cursor: sqlite3.Cursor = conn.cursor()
+        with conn:
+            yield cursor
+    except sqlite3.Error:
+        logging.exception("Error thrown during transaction:")
+        raise
+    finally:
+        cursor.close()
+
+
+class SimpleCipher:
+    def __init__(
+            self, cipher_key: bytes | str,
+            hash_method: hashes.HashAlgorithm = None,
+
+            hash_pepper: bytes = b'', password_pepper: bytes = b''
+    ) -> None:
+        if not isinstance(hash_pepper, bytes):
+            raise TypeError("hash pepper is not bytes")
+        
+        if not isinstance(password_pepper, bytes):
+            raise TypeError("password pepper is not bytes")
+        
+        match cipher_key:
+            case bytes():
+                pass
+            case str():
+                cipher_key: bytes = cipher_key.encode('utf-8')
+            case _:
+                raise TypeError("encryption key is not bytes or string")
+        
+        self.__key: bytes = cipher_key
+        
+        if not hash_method:
+            self.hash_method: hashes.SHA3_512 = hashes.SHA3_512()
+        else:
+            self.hash_method: hashes.HashAlgorithm = hash_method
+
+        self.hash_pepper: bytes = hash_pepper
+        self.pw_pepper: bytes = password_pepper
+
+    def encrypt(
+            self, data: bytes | str,
+            associated_data: bytes = b'',
+    ) -> bytes:        
+        match data:
+            case bytes():
+                pass
+            case str():
+                data: bytes = data.encode('utf-8')
+            case _:
+                raise TypeError("data is not bytes or string")
+        
+        salt: bytes = secrets.token_bytes(32)
+        kdf: PBKDF2HMAC = PBKDF2HMAC(
+            algorithm=self.hash_method,
+            length=32,
+            salt=salt + self.hash_pepper,
+            iterations=100_000
+        )
+        
+        aes_key: bytes = kdf.derive(self.pw_pepper + self.__key)
+        aes: AESGCM = AESGCM(aes_key)
 
-__version__: str = "1.2.0"
+        nonce: bytes = secrets.token_bytes(12)
+        encrypted_data: bytes = aes.encrypt(nonce, data, associated_data)
+
+        return salt + nonce + encrypted_data
+
+    def decrypt(
+            self, data: bytes | str,
+            associated_data: bytes = b'',
+    ) -> bytes:
+        match data:
+            case bytes():
+                pass
+            case str():
+                data: bytes = data.encode('utf-8')
+            case _:
+                raise TypeError("data is not bytes or string")
+        
+        salt: bytes = data[0:32]
+        data: bytes = data[32:]
+        
+        nonce: bytes = data[0:12]
+        data: bytes = data[12:]
+
+        kdf: PBKDF2HMAC = PBKDF2HMAC(
+            algorithm=self.hash_method,
+            length=32,
+            salt=salt + self.hash_pepper,
+            iterations=100_000
+        )
+        
+        aes_key: bytes = kdf.derive(self.pw_pepper + self.__key)
+        aes: AESGCM = AESGCM(aes_key)
+
+        decrypted_data: bytes = aes.decrypt(nonce, data, associated_data)
+        return decrypted_data
+    
+    def hash_data(self, data: bytes | str):
+        match data:
+            case bytes():
+                pass
+            case str():
+                data: bytes = data.encode('utf-8')
+            case _:
+                raise TypeError("data is not bytes or string")
+        
+        digest: hashes.Hash = hashes.Hash(self.hash_method)
+        digest.update(data)
+
+        hashed_data: bytes = digest.finalize()
+        return hashed_data.hex()
 
 
 class FileDatabase:
     def __init__(
             self, db_path: str = '', 
             db_password: bytes | str = b'',
-            recovery_mode: bool = False
+            recovery_mode: bool = False,
+            dict_cache: bool = False
     ) -> None:
+        if not isinstance(db_path, (bytes, str)):
+            raise TypeError("database path must be bytes or str")        
+        if not isinstance(db_password, (bytes, str)):
+            raise TypeError("database password must be bytes or str")
+        
+        if not isinstance(recovery_mode, bool):
+            raise TypeError("recovery mode option must be bool")
+        if not isinstance(dict_cache, bool):
+            raise TypeError("dict cache option must be bool")
+        
         if not db_path:
             data_dir: str = os.environ.get(
                 "XDG_DATA_HOME", 
                 os.path.join(os.path.expanduser("~"), ".local", "share")
             )
             
             db_dir: str = os.path.join(data_dir, "syncServer-server", __version__)
             os.makedirs(db_dir, exist_ok=True)
 
             db_path: str = os.path.join(db_dir, 'syncServer.db')
-        
-        self.db: sqlite3.Connection = sqlite3.connect(db_path, check_same_thread=False)
-        self.cursor: sqlite3.Cursor = self.db.cursor()
 
+        self.__closed: bool = False
+
+        self.db: sqlite3.Connection = sqlite3.connect(db_path, check_same_thread=False)
         self.pw_hasher: argon2.PasswordHasher = argon2.PasswordHasher()
-        self.cipher_mgr: CipherManager = CipherManager()
 
-        self.cipher_mgr.hash_method = cryptography.hazmat.primitives.hashes.SHA3_512()
-        self.cursor.executescript("""
-            PRAGMA foreign_keys = ON;
-            CREATE TABLE IF NOT EXISTS users (
-                user_id TEXT PRIMARY KEY,   
-                username TEXT UNIQUE NOT NULL,
-                token TEXT NOT NULL
-            );
-
-            CREATE TABLE IF NOT EXISTS user_apikeys (
-                key_id TEXT PRIMARY KEY,
-                user_id TEXT,
-                
-                key_name TEXT,
-                api_key TEXT,
+        self.hash_method: hashes.SHA512 = hashes.SHA512()
+        self._using_cache: bool = dict_cache
+
+        with transaction(self.db) as cur:
+            cur.executescript("""
+                PRAGMA foreign_keys = ON;
+                PRAGMA journal_mode=WAL;
+                PRAGMA synchronous=FULL;
                 
-                key_perms BLOB,
-                expiry_date DATETIME,
+                CREATE TABLE IF NOT EXISTS users (
+                    user_id TEXT PRIMARY KEY,   
+                    username TEXT UNIQUE NOT NULL,
+                    token TEXT NOT NULL
+                ) STRICT;
+
+                CREATE TABLE IF NOT EXISTS user_apikeys (
+                    key_id TEXT PRIMARY KEY,
+                    user_id TEXT,
+                    
+                    key_name TEXT,
+                    api_key TEXT,
+                    
+                    key_perms BLOB,
+                    expiry_date TEXT, -- datetime
+                    
+                    FOREIGN KEY (user_id) REFERENCES users(user_id)
+                        ON DELETE CASCADE
+                ) STRICT;
+                CREATE TABLE IF NOT EXISTS files (
+                    data_id TEXT PRIMARY KEY,
+                    dir_id TEXT,
+                    
+                    user_id TEXT,
+                    filename TEXT,
+
+                    file_data BLOB,
+                    FOREIGN KEY (user_id) REFERENCES users(user_id)
+                        ON DELETE CASCADE,
+                    FOREIGN KEY (dir_id) REFERENCES directories(dir_id)
+                        ON DELETE CASCADE
+                ) STRICT;
                 
-                FOREIGN KEY (user_id) REFERENCES users(user_id)
-                    ON DELETE CASCADE
-            );
-            CREATE TABLE IF NOT EXISTS files (
-                data_id TEXT PRIMARY KEY,
-                dir_id TEXT,
+                CREATE TABLE IF NOT EXISTS directories (
+                    dir_id TEXT PRIMARY KEY,
+                    user_id TEXT,
+
+                    dir_name TEXT,
+                    FOREIGN KEY (user_id) REFERENCES users(user_id)
+                        ON DELETE CASCADE
+                ) STRICT;
+
+                CREATE TABLE IF NOT EXISTS config (
+                    config_id TEXT PRIMARY KEY,
+                    config_data BLOB,
+                    config_vars BLOB
+                ) STRICT;
                 
-                user_id TEXT,
-                filename TEXT,
-
-                file_data BLOB,
-                FOREIGN KEY (user_id) REFERENCES users(user_id)
-                    ON DELETE CASCADE,
-                FOREIGN KEY (dir_id) REFERENCES directories(dir_id)
-                    ON DELETE CASCADE
-            );
-            
-            CREATE TABLE IF NOT EXISTS directories (
-                dir_id TEXT PRIMARY KEY,
-                user_id TEXT,
-
-                dir_name TEXT,
-                FOREIGN KEY (user_id) REFERENCES users(user_id)
-                    ON DELETE CASCADE
-            );
-
-            CREATE TABLE IF NOT EXISTS config (
-                config_id TEXT PRIMARY KEY,
-                config_data BLOB,
-                config_vars BLOB
-            );
-            
-            CREATE TABLE IF NOT EXISTS deleted_files (
-                delete_id TEXT PRIMARY KEY,
-                data_id TEXT,
+                CREATE TABLE IF NOT EXISTS deleted_files (
+                    delete_id TEXT PRIMARY KEY,
+                    data_id TEXT,
+                    
+                    old_filepath TEXT,
+                    delete_date TEXT DEFAULT (
+                        datetime('now', 'localtime')  
+                        || '.' 
+                        || strftime('%f', 'now', 'localtime')
+                    ), -- timestamp
+                    
+                    FOREIGN KEY (data_id) REFERENCES files(data_id)
+                        ON DELETE CASCADE
+                ) STRICT;
                 
-                old_filepath TEXT,
-                delete_date TIMESTAMP DEFAULT (
-                    datetime('now', 'localtime')  
-                    || '.' 
-                    || strftime('%f', 'now', 'localtime')
-                ),
+                CREATE TABLE IF NOT EXISTS files_config (
+                    id INTEGER PRIMARY KEY,
+                    data_id TEXT,
+
+                    config BLOB,
+                    FOREIGN KEY(data_id) REFERENCES files(data_id)
+                        ON DELETE CASCADE
+                ) STRICT;
+                                    
+                CREATE UNIQUE INDEX IF NOT EXISTS user_id ON users(user_id);
+                CREATE UNIQUE INDEX IF NOT EXISTS dir_id ON directories(dir_id);
                 
-                FOREIGN KEY (data_id) REFERENCES files(data_id)
-                    ON DELETE CASCADE
-            );
-            
-            CREATE TABLE IF NOT EXISTS files_config (
-                id INTEGER PRIMARY KEY,
-                data_id TEXT,
-
-                config BLOB,
-                FOREIGN KEY(data_id) REFERENCES files(data_id)
-                    ON DELETE CASCADE
-            );
-        """)
+                CREATE UNIQUE INDEX IF NOT EXISTS data_id ON files(data_id);
+                CREATE UNIQUE INDEX IF NOT EXISTS key_id ON user_apikeys(key_id);
+                              
+                CREATE INDEX IF NOT EXISTS delete_data ON deleted_files(delete_date);
+            """)
 
         self._load_conf(db_password=db_password, recovery_mode=recovery_mode)
 
     def _load_conf(self, db_password: bytes | str = '', recovery_mode: bool = False):
-        """
-        Load the configuration data from the 'config' table in the database.
-
-        Parameters:
-        - db_password (bytes | str): The database password used for decryption.
-
-        Raises:
-        - RuntimeError: If there is an issue decrypting the configuration data or if the
-          'syncServer-protected' configuration variable is not found.
-
-        Note:
-        - The method retrieves and decrypts configuration data from the 'config' table.
-        - If the configuration data is not present, default values are used and stored in the 'config' table.
-        - The 'syncServer-protected' configuration variable determines whether the database is key-protected.
-        - If protected, the provided database password is used for decryption.
-        - The decrypted config data is stored in 'conf_secrets', 'conf_vars', and 'cipher_conf' attributes.
-        """
-
-        self.cursor.execute("""
-           SELECT config_data, config_vars FROM config 
-           WHERE config_id='main'
-        """)
-        config = self.cursor.fetchone()
-        db_version: str = "1.1.0"  # make sure to only update this when updating the database schema
-
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT config_data, config_vars FROM config 
+                WHERE config_id='main'
+            """)
+            config: tuple[bytes, bytes] = cursor.fetchone()
+        
+        db_version: str = "1.2.0"  # make sure to only update this when updating the database schema
         if not config:
-            config_secrets = {
+            config_secrets: dict = {
                 'use_encryption': False,
                 'encryption_config': {
                     'hash_pepper': b'',
                     'password_pepper': b''
                 }
             }
 
-            config_vars = {
+            config_vars: dict = {
                 'syncServer-db-version': db_version,
                 'syncServer-protected': False,
 
                 'syncServer-recoveryKey': b'',
                 'syncServer-encryptionEnabled': False  # will plan to use this soon
             }
 
             bytes_encoded_secrets = msgpack.packb(config_secrets)
             bytes_encoded_vars = msgpack.packb(config_vars)
 
-            with self.db:
-                self.cursor.execute("""
+            with transaction(self.db) as cur:
+                cur.execute("""
                    INSERT OR IGNORE INTO config
                    VALUES ('main', ?, ?)
-               """, [bytes_encoded_secrets, bytes_encoded_vars])
+                """, [bytes_encoded_secrets, bytes_encoded_vars])
 
             config = (msgpack.packb(config_secrets), msgpack.packb(config_vars))
 
         config_secrets: bytes = config[0]
         config_vars: dict = msgpack.unpackb(config[1])
 
+        self.recovery_mode: bool = recovery_mode
         if recovery_mode:
             # Partially initialize config vars to get the recovery key
             self.conf_vars: dict = config_vars 
+            self.conf_secrets = {}
+
+            self.cipher: SimpleCipher = SimpleCipher('')
+            self.cipher_conf = {}
+
+            self.db_admin: DatabaseAdmin = DatabaseAdmin(self)
             return
         
         stored_db_version: str = config_vars.get('syncServer-db-version', '')
         if not stored_db_version:
             raise RuntimeError("cannot find syncServer database version in config vars")
         
         if stored_db_version != db_version:
             raise RuntimeError(
                 f"database version does not match with current version "
                 f"[database_version == {stored_db_version}, current_version == {db_version}]"
             )
         
         db_protected = config_vars.get('syncServer-protected', -1)
         if db_protected == -1:
-            raise RuntimeError(
-                "config variable 'syncServer-protected' not in config_vars dictionary"
-            )
+            raise RuntimeError("config variable 'syncServer-protected' not in config_vars dictionary")
         
         if not db_protected and db_password:
-            raise RuntimeError(
-                "database password provided but database is not protected"
-            )
+            raise RuntimeError("database password provided but database is not protected")
 
+        init_cipher: SimpleCipher = SimpleCipher(db_password, hash_method=self.hash_method)
         if db_protected:
             try:
-                msgpack_secrets = self.cipher_mgr.fernet.decrypt_data(
-                    config_secrets, password=db_password
-                )
+                msgpack_secrets = init_cipher.decrypt(config_secrets)
                 config_secrets = msgpack.unpackb(msgpack_secrets)
-            except cryptography.fernet.InvalidToken:  # type: ignore
+            except cryptography.exceptions.InvalidTag:  # type: ignore
                 raise RuntimeError(
                     "could not decrypt config_data, either incorrect password or not encrypted, "
                     "if the original key was lost, decrypt the 'syncServer-recoveryKey' entry  "
                     "in config_vars using the exported recovery key"
                 ) from None
         else:
             config_secrets = msgpack.unpackb(config[0])
         
+        hash_pepper: bytes = config_secrets.get('hash-pepper', b'')
+        pw_pepper: bytes = config_secrets.get('password-pepper', b'')
+
+        self.cipher: SimpleCipher = SimpleCipher(
+            db_password, hash_method=self.hash_method,
+            hash_pepper=hash_pepper, password_pepper=pw_pepper
+        )
         self.conf_secrets: dict = config_secrets
         self.conf_vars: dict = config_vars
 
-        self._cipher_key: bytes | str = db_password
         self.cipher_conf: dict = config_secrets['encryption_config']
-
         self.dirs: DirectoryInterface = DirectoryInterface(self)
-        self.deleted_files: DeletedFiles = DeletedFiles(self)
 
+        self.deleted_files: DeletedFiles = DeletedFiles(self)
         self.api_keys: APIKeyInterface = APIKeyInterface(self)
 
-    def set_protection(
-            self, set_protection: bool,
-            cipher_key: bytes | str = b''
-    ) -> None:
-        """
-        Set or unset protection for the database, including encryption.
+        self.db_admin: DatabaseAdmin = DatabaseAdmin(self)
+        self.__data_cache: dict = {}
 
-        Parameters:
-        - set_protection (bool): True to enable protection, False to disable.
-        - cipher_key (bytes or str, optional): Encryption key for protecting the database.
-          Required when set_protection is True.
+        if self._using_cache:
+            with transaction(self.db) as cursor:
+                cursor.execute("SELECT user_id, username, token FROM users") 
+                user_data: list[tuple] = cursor.fetchall()
+                
+            for user_id, username, token in user_data:
+                user_dict: dict = {
+                    'id': user_id,
+                    'token': token
+                }
+                self.__data_cache[username] = user_dict
         
-        Raises:
-        - ValueError: If set_protection is True but cipher_key is not provided.
-        """
-
-        if set_protection and not cipher_key:
-            raise ValueError(
-                "set_protection is True but cipher_key was not provided"
-            )
-
-        if not set_protection:  # False
-            self.conf_secrets['use_encryption'] = False
-            self.conf_vars['syncServer-protected'] = False
-
-            bytes_encoded_secrets = msgpack.packb(self.conf_secrets)
-            bytes_encoded_vars = msgpack.packb(self.conf_vars)
-            with self.db:
-                self.cursor.execute("""
-                    UPDATE config
-                    SET config_data=?, config_vars=?
-                    WHERE config_id='main'
-                """, [bytes_encoded_secrets, bytes_encoded_vars])
-            return
-
-        self.conf_secrets['use_encryption'] = True
-        self.conf_vars['syncServer-protected'] = True
-        self.conf_vars['syncServer-encryptionEnabled'] = True
-
-        encrypted_secrets = self.cipher_mgr.fernet.encrypt_data(
-            msgpack.packb(self.conf_secrets), password=cipher_key
-        )
-        recovery_key = secrets.token_hex(32)
-
-        encrypted_cipher_key = self.cipher_mgr.fernet.encrypt_data(
-            cipher_key, password=recovery_key
-        )
-        self._cipher_key: bytes | str = cipher_key
-
-        self.conf_vars['syncServer-recoveryKey'] = encrypted_cipher_key
-        with self.db, open('syncServer-recoveryKey.key', 'w', encoding='utf-8') as file:
-            self.cursor.execute("""
-                UPDATE config
-                SET config_data=?, config_vars=?
-                WHERE config_id='main'
-            """, [
-                encrypted_secrets,
-                msgpack.packb(self.conf_vars)
-            ])
-            file.write(recovery_key)
+    def _get_userid(self, username: str) -> str:
+        self._ensure_open()
+        if self._using_cache:
+            user_dict: dict = self.__data_cache.get(username)
+            if not user_dict:
+                return ''
+            
+            return user_dict['id']
+        else:
+            with transaction(self.db) as cursor:
+                cursor.execute("""
+                    SELECT user_id FROM users WHERE username=?
+                """, [username])
+                db_result: tuple[str] = cursor.fetchone()
 
-        return
+            if not db_result:
+                return ''
+            
+            return db_result[0]
+    
+    def _get_dirid(self, dir_path: str, user_id: str) -> str:
+        self._ensure_open()
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT dir_id FROM directories
+                WHERE dir_name=? AND user_id=?
+            """, [dir_path, user_id])
 
-    def save_conf(self, secrets: dict = None, _vars: dict = None) -> None:
-        if not secrets:
-            pass
-        elif self.conf_vars['syncServer-protected']:
-            conf_secrets: bytes = self.cipher_mgr.fernet.encrypt_data(
-                msgpack.packb(secrets), password=self._cipher_key
-            )
-        else:
-            conf_secrets: bytes = msgpack.packb(secrets)
-        
-        with self.db:
-            if secrets:
-                self.cursor.execute("""
-                    UPDATE config
-                    SET config_data=?
-                    WHERE config_id='main'
-                """, [conf_secrets])
+            db_result: tuple[str] = cursor.fetchone()
             
-            if _vars:
-                self.cursor.execute("""
-                    UPDATE config
-                    SET config_vars=?
-                    WHERE config_id='main'
-                """, [msgpack.packb(_vars)])
+        if not db_result:
+            return ''
+            
+        return db_result[0]
+    
+    def _ensure_open(self):
+        if self.__closed:
+            raise RuntimeError("working on a closed FileDatabase instance")
+    
+    def close(self):
+        if self.__closed:
+            return
         
-        return 0
+        self.db.close()
+        self.__closed: bool = True
 
+        del self.__data_cache
+        del self.db
+        del self.dirs
+        del self.deleted_files
+        del self.api_keys
+        del self.db_admin
+        del self.cipher
+        del self.pw_hasher
+        del self.hash_method
+        del self.conf_secrets
+        del self.conf_vars
+        del self.cipher_conf
+        del self.recovery_mode
+    
     def verify_user(self, username: str, token: str) -> str | bool:
-        """
-        Verify the authenticity of a user's authentication token.
-
-        Parameters:
-        - username (str): The username of the user to verify.
-        - token (str): The authentication token to be verified.
-
-        Returns:
-        - True: If the user is verified successfully.
-        - "NO_USER": If the specified username is not found in the database.
-        - False: If the verification process fails, indicating an incorrect token.
-        - Exception: If an unexpected exception occurs during the verification process.
-
-        Notes:
-        - Retrieves the stored token for the given username from the database.
-        - Compares the provided token with the stored hashed token using Argon2 password hashing.
-        - Returns True if the verification is successful, "NO_USER" if the user is not found,
-          and False if the verification process fails.
-        - Logs an error if an unexpected exception occurs during the verification process,
-          and returns the exception instance in case of an unexpected error.
-        """
-
-        self.cursor.execute("""
-            SELECT token FROM users WHERE username=?
-        """, [username])
-        db_result = self.cursor.fetchone()
-
-        if not db_result:
-            return "NO_USER"
+        self._ensure_open()
+        if self._using_cache:
+            user_dict: dict = self.__data_cache.get(username)
+            if not user_dict:
+                return "NO_USER"
+            hashed_pw: str = user_dict['token']  # fail intentionally if missing
+        else:
+            with transaction(self.db) as cursor:
+                cursor.execute("""
+                    SELECT token FROM users WHERE username=?
+                """, [username])
+                db_result: tuple[str] = cursor.fetchone()
 
-        hashed_pw = db_result[0]
+            if not db_result:
+                return "NO_USER"
+            hashed_pw: str = db_result[0]
 
         try:
             self.pw_hasher.verify(hashed_pw, token)
         except (argon2.exceptions.VerifyMismatchError, argon2.exceptions.VerificationError):
             return False
         except Exception as exc:
             logging.error("[verify_hash]: Verifying user hash failed: '%s'", exc)
@@ -381,583 +492,795 @@
         - Checks if a user with the given username already exists in the database.
         - If the user exists, returns "USER_EXISTS" without adding a new user.
         - If the user does not exist, generates a unique user ID and directory ID.
         - Inserts the new user into the 'users' table and creates a root directory for the user.
         - Returns 0 upon successful addition of the new user to the database.
         """
 
-        blacklisted_names = {
-            'INVALID_APIKEY', 'APIKEY_NOT_AUTHORIZED', 'NO_USER',
-        }
+        self._ensure_open()
+
+        blacklisted_names: set = {'INVALID_APIKEY', 'APIKEY_NOT_AUTHORIZED', 'NO_USER', ''}
         if username in blacklisted_names:
             raise ValueError('cannot use blacklisted username')
         
-        self.cursor.execute("""
-            SELECT user_id FROM users WHERE username=?
-        """, [username])
-        user_id = self.cursor.fetchone()
-
-        if user_id:
+        user_data: str = self._get_userid(username)
+        if user_data:
             return "USER_EXISTS"
 
-        hashed_pw = self.pw_hasher.hash(token)
-        user_id = str(uuid.uuid4())
+        hashed_pw: str = self.pw_hasher.hash(token)
+        user_id: str = str(uuid.uuid4())
 
-        dir_id = str(uuid.uuid4())
-        with self.db:
-            self.cursor.execute("""
+        dir_id: str = str(uuid.uuid4())
+        with transaction(self.db) as cursor:
+            cursor.execute("""
                 INSERT INTO users (user_id, username, token)
                 VALUES (?, ?, ?)                
             """, [user_id, username, hashed_pw])
-            self.cursor.execute("""
+            cursor.execute("""
                 INSERT INTO directories (dir_id, user_id, dir_name)
                 VALUES (?, ?, '/')
             """, [dir_id, user_id])
 
         return 0
 
     def remove_user(self, username: str) -> Literal["NO_USER"] | int:
-        """
-        Remove a user from the database based on the specified username.
-
-        Parameters:
-        - username (str): The username of the user to be removed.
-
-        Returns:
-        - 0: If the user is successfully removed from the database.
-        - "NO_USER": If the specified username is not found in the database.
-
-        Notes:
-        - Retrieves the stored user ID and hashed token for the given username from the database.
-        - Compares the provided token with the stored hashed token using Argon2 password hashing.
-        - If the user is not found, returns "NO_USER."
-        - If the token verification fails, returns "INVALID_TOKEN."
-        - If the verification is successful, irreversibly removes the user from the 'users' table.
-        - Returns 0 upon successful removal of the user from the database.
-        """
-
-        self.cursor.execute("""
-            SELECT token FROM users WHERE username=?
-        """, [username])
-        db_result = self.cursor.fetchone()
-
-        if not db_result:
+        self._ensure_open()
+        user_id: str = self._get_userid(username)
+        if not user_id:
             return "NO_USER"
-
+        
+        if self._using_cache:
+            self.__data_cache.pop(username, '')
+        
         # irreversible delete
-        with self.db:
-            self.cursor.execute("""
+        with transaction(self.db) as cursor:
+            cursor.execute("""
                 DELETE FROM users
-                WHERE username=?
-            """, [username])
+                WHERE user_id=?
+            """, [user_id])
+        
         return 0
     
-    def dir_checker(self, file_path: str, user_id: str) -> Literal["NO_USER"] | tuple[str]:
+    def dir_checker(self, username: str, file_path: str) -> Literal["NO_USER"] | str:
+        self._ensure_open()
         if not isinstance(file_path, str):
             raise TypeError("'file_path' must be a string")
         
         if not file_path:
             raise ValueError("'file_path' was not passed in args")
 
-        self.cursor.execute("""
-            SELECT user_id FROM users WHERE user_id=?
-        """, [user_id])
-        user_data: tuple[str] = self.cursor.fetchone()
-
-        if not user_data:
+        user_id: str = self._get_userid(username)
+        if not user_id:
             return "NO_USER"
         
         dirs: list[str] = file_path.split("/")
         path_without_file: str = "/".join(dirs[0:-1])
 
         if path_without_file == "":
             path_without_file: str = "/"
         
-        self.cursor.execute("""
-            SELECT dir_id FROM directories
-            WHERE dir_name=? AND user_id=?
-        """, [path_without_file, user_id])
-        db_result: tuple[str] = self.cursor.fetchone()
-        
-        return db_result
+        dir_id: str = self._get_dirid(path_without_file, user_id)
+        if not dir_id:
+            return ''
+
+        return dir_id
     
     def add_file(
             self, username: str,
             file_path: str,
 
             file_stream: BinaryIO | TextIO,
             chunk_size: int = 50 * 1024 * 1024
     ) -> int | str:
+        self._ensure_open()
         if not isinstance(file_path, str):
             raise TypeError("'file_path' must be a string")
         
         if not isinstance(chunk_size, int):
             raise TypeError("'chunk_size' must be an int")
 
-        self.cursor.execute("""
-            SELECT user_id FROM users WHERE username=?
-        """, [username])
-        user_data = self.cursor.fetchone()
-
-        if not user_data:
+        user_id: str = self._get_userid(username)
+        if not user_id:
             return "NO_USER"
-
-        user_id = user_data[0]
-
-        first_chunk = file_stream.read(chunk_size)
+        
+        first_chunk: bytes = file_stream.read(chunk_size)
         if not first_chunk:
             raise IOError("file stream is empty")
         
-        dir_exists = self.dir_checker(file_path, user_id)
-        if not dir_exists:
+        dir_id: str = self.dir_checker(username, file_path)
+        if not dir_id:
             return "NO_DIR_EXISTS"
         
-        dir_id = dir_exists[0]
-        self.cursor.execute("""
-            SELECT data_id FROM files
-            WHERE filename=? AND user_id=? AND dir_id=?
-        """, [file_path, user_id, dir_id])
-
-        file_data = self.cursor.fetchall()
-
-        for file_tuple in file_data:
-            file_id = file_tuple[0]
-            self.cursor.execute("""
-                SELECT data_id FROM deleted_files
-                WHERE data_id=?
-                ORDER BY delete_date DESC
-            """, [file_id])
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT data_id FROM files
+                WHERE filename=? AND user_id=? AND dir_id=?
+            """, [file_path, user_id, dir_id])
+            file_data: list[tuple[str]] = cursor.fetchall()
+
+        with transaction(self.db) as cursor:
+            for file_tuple in file_data:
+                file_id: str = file_tuple[0]
+                cursor.execute("""
+                    SELECT data_id FROM deleted_files
+                    WHERE data_id=?
+                    ORDER BY delete_date DESC
+                """, [file_id])
 
-            tmp_delete_data = self.cursor.fetchone()
-            if not tmp_delete_data:
-                return "FILE_EXISTS"
+                tmp_delete_data: tuple[str] = cursor.fetchone()
+                if not tmp_delete_data:
+                    return "FILE_EXISTS"
         
         if self.conf_secrets['use_encryption']:
-            first_chunk = self.cipher_mgr.fernet.encrypt_data(
-                first_chunk, password=self._cipher_key,
-                hash_pepper=self.cipher_conf['hash_pepper'],
+            first_chunk: bytes = self.cipher.encrypt(first_chunk)
 
-                password_pepper=self.cipher_conf['password_pepper']
-            )
+        data_id: str = str(uuid.uuid4())
+        config_data: dict = {'chunk-size': chunk_size}
 
-        data_id = str(uuid.uuid4())
-        config_data = {
-            'encrypted': self.conf_secrets['use_encryption'],
-            'chunk_size_used': chunk_size
-        }
-
-        with self.db:
-            file_data = [data_id, dir_id, user_id, file_path, first_chunk]
-            self.cursor.execute("""
+        with transaction(self.db) as cursor:
+            file_data: list = [data_id, dir_id, user_id, file_path, first_chunk]
+            cursor.execute("""
                 INSERT INTO files (
                     data_id, dir_id, user_id,
                     filename, file_data
                 )
                 VALUES (?, ?, ?, ?, ?)
             """, file_data)
-            self.cursor.execute("""
+            cursor.execute("""
                 INSERT INTO files_config (data_id, config)
                 VALUES (?, ?)
             """, [data_id, msgpack.packb(config_data)])
 
-            chunk = file_stream.read(chunk_size)
+            chunk: bytes = file_stream.read(chunk_size)
             while chunk:
                 if self.conf_secrets['use_encryption']:
-                    chunk = self.cipher_mgr.fernet.encrypt_data(
-                        chunk, password=self._cipher_key,
-                        hash_pepper=self.cipher_conf['hash_pepper'],
-
-                        password_pepper=self.cipher_conf['password_pepper']
-                    )
+                    chunk: bytes = self.cipher.encrypt(chunk)
                 
-                self.cursor.execute("""
+                cursor.execute("""
                     UPDATE files
-                    SET file_data = file_data || ?
-                    WHERE user_id=? AND data_id=? AND dir_id=?
-                """, [chunk, user_id, data_id, dir_id])
-                chunk = file_stream.read(chunk_size)
+                    SET file_data = cast(file_data || ? AS BLOB)
+                    WHERE data_id=?
+                """, [chunk, user_id])
+                chunk: bytes = file_stream.read(chunk_size)
 
         return 0
 
     def modify_file(
             self, username: str,
             file_path: str,
 
             file_stream: BinaryIO | TextIO,
             chunk_size: int = 50 * 1024 * 1024
     ) -> int | str:
+        self._ensure_open()
         if not isinstance(file_path, str):
             raise TypeError("'file_path' must be string")
         
         if not isinstance(chunk_size, int):
             raise TypeError("'chunk_size' must be an int")
-
-        self.cursor.execute("""
-            SELECT user_id FROM users WHERE username=?
-        """, [username])
-        user_data = self.cursor.fetchone()
-
-        if not user_data:
+        
+        user_id: str = self._get_userid(username)
+        if not user_id:
             return "NO_USER"
-
-        user_id = user_data[0]
-
-        first_chunk = file_stream.read(chunk_size)
+        
+        first_chunk: bytes = file_stream.read(chunk_size)
         if not first_chunk:
             raise IOError("file stream is empty")
         
-        dir_exists = self.dir_checker(file_path, user_id)
-        if not dir_exists:
+        dir_id: str = self.dir_checker(username, file_path)
+        if not dir_id:
             return "NO_DIR_EXISTS"
         
-        dir_id = dir_exists[0]
-        self.cursor.execute("""
-            SELECT data_id FROM files
-            WHERE filename=? AND user_id=? AND dir_id=?
-        """, [file_path, user_id, dir_id])
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT data_id FROM files
+                WHERE filename=? AND user_id=? AND dir_id=?
+            """, [file_path, user_id, dir_id])
+            file_data: list[tuple[str]] = cursor.fetchall()
 
-        file_data = self.cursor.fetchall()
         if not file_data:
             return "NO_FILE_EXISTS"
 
-        # [id1, id2, id3]
-        non_deleted_id = ""
-        for file_tuple in file_data:
-            file_id = file_tuple[0]
-            self.cursor.execute("""
-                SELECT data_id FROM deleted_files
-                WHERE data_id=?
-                ORDER BY delete_date DESC
-            """, [file_id])
+        non_deleted_id: str = ""
+        with transaction(self.db) as cursor:
+            for file_tuple in file_data:
+                file_id: str = file_tuple[0]
+                cursor.execute("""
+                    SELECT data_id FROM deleted_files
+                    WHERE data_id=?
+                    ORDER BY delete_date DESC
+                """, [file_id])
 
-            tmp_delete_data = self.cursor.fetchone()
-            if tmp_delete_data:
-                continue
+                tmp_delete_data: tuple[str] = cursor.fetchone()
+                
+                if tmp_delete_data:
+                    continue
 
-            non_deleted_id = file_id
-            break
+                non_deleted_id: str = file_id
+                break
 
         if not non_deleted_id:
             return "NO_FILE_EXISTS"
         
-        data_id = non_deleted_id
         if self.conf_secrets['use_encryption']:
-            first_chunk = self.cipher_mgr.fernet.encrypt_data(
-                first_chunk, password=self._cipher_key,
-                hash_pepper=self.cipher_conf['hash_pepper'],
-
-                password_pepper=self.cipher_conf['password_pepper']
-            )
+            first_chunk: bytes = self.cipher.encrypt(first_chunk)
         
-        config_data = {
-            'encrypted': self.conf_secrets['use_encryption'],
-            'chunk_size_used': chunk_size
-        }
+        config_data = {'chunk-size': chunk_size}
         
-        with self.db:
-            self.cursor.execute("""
+        with transaction(self.db) as cursor:
+            cursor.execute("""
                 UPDATE files
                 SET file_data=?
-                WHERE user_id=? AND data_id=? AND dir_id=?
-            """, [first_chunk, user_id, non_deleted_id, dir_id])
-            self.cursor.execute("""
+                WHERE data_id=?
+            """, [first_chunk, non_deleted_id])
+            cursor.execute("""
                 UPDATE files_config
                 SET config=?
                 WHERE data_id=?
-            """, [msgpack.packb(config_data), data_id])
+            """, [msgpack.packb(config_data), non_deleted_id])
 
-            chunk = file_stream.read(chunk_size)
+            chunk: bytes = file_stream.read(chunk_size)
             while chunk:
                 if self.conf_secrets['use_encryption']:
-                    chunk = self.cipher_mgr.fernet.encrypt_data(
-                        chunk, password=self._cipher_key,
-                        hash_pepper=self.cipher_conf['hash_pepper'],
-
-                        password_pepper=self.cipher_conf['password_pepper']
-                    )
+                    chunk: bytes = self.cipher.encrypt(chunk)
                 
-                self.cursor.execute("""
+                cursor.execute("""
                     UPDATE files
-                    SET file_data = file_data || ?
-                    WHERE user_id=? AND data_id=?
+                    SET file_data = cast(file_data || ? AS BLOB)
+                    WHERE data_id=?
                 """, [chunk, user_id, non_deleted_id])
-                chunk = file_stream.read(chunk_size)
+                chunk: bytes = file_stream.read(chunk_size)
 
         return 0
 
     def remove_file(
             self, username: str,
             file_path: str,
 
             permanent_delete: bool = False
     ) -> int | str:
+        self._ensure_open()
         if not isinstance(file_path, str):
             raise TypeError("'file_path' must be string")
         
-        self.cursor.execute("""
-            SELECT user_id FROM users WHERE username=?
-        """, [username])
-        user_data = self.cursor.fetchone()
-
-        if not user_data:
+        user_id: str = self._get_userid(username)
+        if not user_id:
             return "NO_USER"
-
-        user_id = user_data[0]
         
-        dir_exists = self.dir_checker(file_path, user_id)
-        if not dir_exists:
+        dir_id: str = self.dir_checker(username, file_path)
+        if not dir_id:
             return "NO_DIR_EXISTS"
-        
-        dir_id = dir_exists[0]
-        self.cursor.execute("""
-            SELECT data_id FROM files
-            WHERE filename=? AND user_id=? AND dir_id=?
-        """, [file_path, user_id, dir_id])
+                        
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT data_id FROM files
+                WHERE filename=? AND user_id=? AND dir_id=?
+            """, [file_path, user_id, dir_id])
+            file_data: list[tuple[str]] = cursor.fetchall()
 
-        file_data = self.cursor.fetchall()
         if not file_data:
             return "NO_FILE_EXISTS"
 
         non_deleted_id = ""
-        for file_tuple in file_data:
-            file_id = file_tuple[0]
-            self.cursor.execute("""
-                SELECT data_id FROM deleted_files
-                WHERE data_id=?
-                ORDER BY delete_date DESC
-            """, [file_id])
-        
-            tmp_delete_data = self.cursor.fetchone()
-            if tmp_delete_data:
-                continue
+        with transaction(self.db) as cursor:
+            for file_tuple in file_data:
+                file_id: str = file_tuple[0]
+                cursor.execute("""
+                    SELECT data_id FROM deleted_files
+                    WHERE data_id=?
+                    ORDER BY delete_date DESC
+                """, [file_id])
 
-            non_deleted_id = file_id
-            break
+                tmp_delete_data: tuple[str] = cursor.fetchone()
+                
+                if tmp_delete_data:
+                    continue
+
+                non_deleted_id: str = file_id
+                break
         
         if not non_deleted_id:
             return "NO_FILE_EXISTS"
-        
-        data_id = non_deleted_id
-        if permanent_delete:
-            with self.db:
-                self.cursor.execute("""
+
+        with transaction(self.db) as cursor:
+            if permanent_delete:
+                cursor.execute("""
                     DELETE FROM files
                     WHERE user_id=? AND filename=? AND data_id=?
-                """, [user_id, file_path, data_id])
-        else: 
-            delete_id = str(uuid.uuid4())
-            with self.db:
-                self.cursor.execute("""
+                """, [user_id, file_path, non_deleted_id])
+            else:
+                delete_id: str = str(uuid.uuid4())
+                cursor.execute("""
                     INSERT INTO deleted_files (
                         delete_id, data_id, old_filepath
                     ) VALUES (?, ?, ?)
-                """, [delete_id, data_id, file_path])
+                """, [delete_id, non_deleted_id, file_path])
+        
         return 0
 
     def read_file(
             self, username: str,
             file_path: str,
             chunk_size: int = 50 * 1024 * 1024
     ) -> str | Generator[bytes, None, None]:
+        self._ensure_open()
         if not isinstance(file_path, str):
             raise TypeError("'file_path' must be string")
         
         if not isinstance(chunk_size, int):
             raise TypeError("'chunk_size' must be an int")
         
-        self.cursor.execute("""
-            SELECT user_id FROM users WHERE username=?
-        """, [username])
-        user_data = self.cursor.fetchone()
-
-        if not user_data:
+        user_id: str = self._get_userid(username)
+        if not user_id:
             return "NO_USER"
-
-        user_id = user_data[0]
         
-        dir_exists = self.dir_checker(file_path, user_id)
-        if not dir_exists:
+        dir_id: str = self.dir_checker(username, file_path)
+        if not dir_id:
             return "NO_DIR_EXISTS"
         
-        dir_id = dir_exists[0]
-        self.cursor.execute("""
-            SELECT data_id, length(file_data) FROM files
-            WHERE filename=? AND user_id=? AND dir_id=?
-        """, [file_path, user_id, dir_id])
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT data_id, length(file_data) FROM files
+                WHERE filename=? AND user_id=? AND dir_id=?
+            """, [file_path, user_id, dir_id])
 
-        file_data = self.cursor.fetchall()
+            file_data: list[tuple[str]] = cursor.fetchall()
+        
         if not file_data:
             return "NO_FILE_EXISTS"
 
-        # [id1, id2, id3]
-        non_deleted_id = ""
-        data_length = 0
+        non_deleted_id: str = ""
+        data_length: int = 0
 
-        for file_tuple in file_data:
-            file_id = file_tuple[0]
-            self.cursor.execute("""
-                SELECT data_id FROM deleted_files
-                WHERE data_id=?
-                ORDER BY delete_date DESC
-            """, [file_id])
+        with transaction(self.db) as cursor:
+            for file_tuple in file_data:
+                file_id: str = file_tuple[0]
+                cursor.execute("""
+                    SELECT data_id FROM deleted_files
+                    WHERE data_id=?
+                    ORDER BY delete_date DESC
+                """, [file_id])
 
-            tmp_delete_data = self.cursor.fetchone()
-            if tmp_delete_data:
-                continue
+                tmp_delete_data: tuple[str] = cursor.fetchone()
+                
+                if tmp_delete_data:
+                    continue
 
-            non_deleted_id = file_id
-            data_length = file_tuple[1]
+                non_deleted_id: str = file_id
+                data_length: int = file_tuple[1]
 
-            break
+                break
 
         if not non_deleted_id:
             return "NO_FILE_EXISTS"
 
-        data_id = non_deleted_id
-        self.cursor.execute("""
-            SELECT config FROM files_config
-            WHERE data_id=?
-        """, [data_id])
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT config FROM files_config
+                WHERE data_id=?
+            """, [non_deleted_id])
 
-        msgpack_config = self.cursor.fetchone()[0]
-        config = msgpack.unpackb(msgpack_config)
+            msgpack_config: bytes = cursor.fetchone()[0]
+        
+        config: dict = msgpack.unpackb(msgpack_config)
 
-        if config['chunk_size_used'] != chunk_size:
-            chunk_size = config['chunk_size_used']
+        if config['chunk-size'] != chunk_size:
+            chunk_size: int = config['chunk-size']
 
         def generator():
-            offset = 0
-            while offset < data_length:
-                self.cursor.execute("""
-                    SELECT substr(file_data, ?, ?) 
-                    FROM files
-                    WHERE data_id=?
-                """, (offset + 1, chunk_size, data_id))
+            offset: int = 1
+            with transaction(self.db) as cursor:
+                while offset < data_length:
+                    cursor.execute("""
+                        SELECT substr(file_data, ?, ?) 
+                        FROM files WHERE data_id=?
+                    """, (offset, chunk_size, non_deleted_id))
 
-                chunk = self.cursor.fetchone()[0]
-                offset += chunk_size
+                    chunk: bytes = cursor.fetchone()[0]
+                    offset += chunk_size
 
-                if config['encrypted']:
-                    chunk = self.cipher_mgr.fernet.decrypt_data(
-                        chunk, password=self._cipher_key,
-                        hash_pepper=self.cipher_conf['hash_pepper'],
-
-                        password_pepper=self.cipher_conf['password_pepper']
-                    )
-                yield chunk
+                    if self.conf_secrets['use_encryption']:
+                        chunk: bytes = self.cipher.decrypt(chunk)
+                    
+                    yield chunk
         
         # Returning generator() instead of yield directly
         # allows the function to return plain values instead of
         # requiring me to use next() and then checking the value
         return generator()
         
 
+class DatabaseAdmin:
+    def __init__(self, parent: FileDatabase, log_level: int = logging.DEBUG) -> None:
+        self.db: sqlite3.Connection = parent.db
+        self.recovery_mode: bool = parent.recovery_mode
+
+        self.pw_hasher: argon2.PasswordHasher = parent.pw_hasher
+        self.cipher: SimpleCipher = parent.cipher
+
+        self.conf_secrets: dict = parent.conf_secrets
+        self.conf_vars: dict = parent.conf_vars
+
+        self.cipher_conf: dict = parent.cipher_conf
+        self.hash_method = parent.hash_method
+
+        self.logger: logging.Logger = logging.getLogger(f"{__name__}: serverDB-DBAdmin")
+        self.logger.setLevel(log_level)
+
+        fmt_msg: str = (
+            '[syncServer-serverDB: DatabaseAdmin]: [%(asctime)s] ' 
+            '- [%(levelname)s] - (%(funcName)s): %(message)s'
+        )
+        formatter: logging.Formatter = logging.Formatter(
+            fmt_msg,
+            datefmt='%Y-%m-%d %H:%M:%S'
+        )
+        file_handler: logging.FileHandler = logging.FileHandler(LOGFILE)
+
+        file_handler.setFormatter(formatter)
+        self.logger.addHandler(file_handler)
+
+    def set_protection(
+            self, cipher_key: bytes | str,
+            recovery_key_path: str = ''
+    ) -> int:
+        """
+        Update encryption key or disable encryption, then write recovery key to file.
+        Set `cipher_key` to an empty string to disable encryption.  
+        """
+        if self.recovery_mode:
+            raise RuntimeError("cannot edit database configuration, currently in recovery mode")
+        
+        if not isinstance(recovery_key_path, str):
+            raise TypeError("recovery key path must be a string")
+        
+        match cipher_key:
+            case bytes():
+                pass
+            case str():
+                cipher_key: bytes = cipher_key.encode('utf-8')
+            case _:
+                raise TypeError("encryption key is not bytes or string")
+
+        if os.path.isfile(recovery_key_path) and cipher_key:
+            raise FileExistsError(f"cannot overwrite existing recovery key file: {recovery_key_path}")
+        
+        if not recovery_key_path and cipher_key:
+            raise ValueError("recovery key path cannot be empty")
+        
+        conf_secrets: dict = copy.deepcopy(self.conf_secrets)
+        conf_vars: dict = copy.deepcopy(self.conf_vars)
+
+        if not cipher_key:  # False
+            conf_secrets['use_encryption'] = False
+            conf_vars['syncServer-protected'] = False
+
+            bytes_encoded_secrets: bytes = msgpack.packb(conf_secrets)
+            bytes_encoded_vars: bytes = msgpack.packb(conf_vars)
+
+            try:
+                with transaction(self.db) as cursor:
+                    cursor.execute("""
+                        UPDATE config
+                        SET config_data=?, config_vars=?
+                        WHERE config_id='main'
+                    """, [bytes_encoded_secrets, bytes_encoded_vars])
+            except sqlite3.Error:  # type: ignore
+                self.logger.exception("(set_protection): Failed to write configuration to database")
+                return 2
+            
+            self.logger.info("(set_protection): Disabled database protection")
+            self.conf_secrets: dict = conf_secrets
+
+            self.conf_vars: dict = conf_vars
+            return 0 
+        
+        recovery_key: str = secrets.token_hex(32)
+        current_umask: int = os.umask(0)
+        
+        mainkey_cipher: SimpleCipher = SimpleCipher(cipher_key, hash_method=self.hash_method)
+        recoverykey_cipher: SimpleCipher = SimpleCipher(recovery_key, hash_method=self.hash_method)
+
+        encrypted_cipher_key: bytes = recoverykey_cipher.encrypt(cipher_key)
+
+        conf_vars['syncServer-recoveryKey'] = encrypted_cipher_key
+        conf_secrets['use_encryption'] = True
+
+        conf_vars['syncServer-protected'] = True
+        conf_vars['syncServer-encryptionEnabled'] = True
+
+        encrypted_secrets: bytes = mainkey_cipher.encrypt(msgpack.packb(conf_secrets))
+        encoded_vars: bytes = msgpack.packb(conf_vars)
+
+        try:
+            with os.fdopen(os.open(recovery_key_path, os.O_WRONLY | os.O_CREAT, 0o600), 'w') as f:
+                f.write(recovery_key)
+            
+            self.logger.info("(set_protection: Wrote recovery key to file '%s'", recovery_key_path)
+        except IOError:
+            self.logger.exception("(set_protection): Failed to write recovery key")
+            return 1
+        finally:
+            os.umask(current_umask)
+        
+        try:
+            with transaction(self.db) as cursor:
+                cursor.execute("""
+                    UPDATE config
+                    SET config_data=?, config_vars=?
+                    WHERE config_id='main'
+                """, [
+                    encrypted_secrets,
+                    encoded_vars
+                ])
+        except Exception:  # type: ignore
+            self.logger.exception("(set_protection): Failed to write configuration to database")
+            os.remove(recovery_key_path)
+
+            self.logger.info("(set_protection): Removed recovery key file '%s'", recovery_key_path)
+            return 2
+
+        self.logger.info("(set_protection): Encrypted config secrets and wrote config to database")
+
+        self.conf_secrets: dict = conf_secrets
+        self.conf_vars: dict = conf_vars
+        return 0
+
+    def save_conf(self, _secrets: dict = None, _vars: dict = None) -> int:
+        if not _secrets:
+            pass
+        elif self.conf_vars['syncServer-protected']:
+            conf_secrets: bytes = self.cipher.encrypt(msgpack.packb(_secrets))
+        else:
+            conf_secrets: bytes = msgpack.packb(_secrets)
+        
+        with transaction(self.db) as cursor:
+            if _secrets:
+                cursor.execute("""
+                    UPDATE config
+                    SET config_data=?
+                    WHERE config_id='main'
+                """, [conf_secrets])
+            if _vars:
+                cursor.execute("""
+                    UPDATE config
+                    SET config_vars=?
+                    WHERE config_id='main'
+                """, [msgpack.packb(_vars)])
+        
+        return 0
+
+    def update_encryption(
+            self, old_key: bytes | str = b'',
+            new_key: bytes | str = b''
+    ) -> int:
+        if self.recovery_mode:
+            raise RuntimeError("cannot edit database configuration, currently in recovery mode")
+        
+        match old_key:
+            case bytes():
+                pass
+            case str():
+                old_key: bytes = old_key.encode('utf-8')
+            case _:
+                raise TypeError("old encryption key is not bytes or string")
+        
+        match new_key:
+            case bytes():
+                pass
+            case str():
+                new_key: bytes = new_key.encode('utf-8')
+            case _:
+                raise TypeError("new encryption key is not bytes or string")
+        
+        # Have to fetch the user_id and dir_id due to SQLite foreign key constraints
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT data_id, length(file_data), user_id, dir_id
+                FROM files
+            """)
+            file_data: list[tuple[str, int, str, str]] = cursor.fetchall()
+
+        oldkey_cipher: SimpleCipher = SimpleCipher(
+            old_key, hash_method=self.hash_method,
+            hash_pepper=self.cipher_conf['hash_pepper'],
+            password_pepper=self.cipher_conf['password_pepper']
+        )
+        newkey_cipher: SimpleCipher = SimpleCipher(
+            new_key, hash_method=self.hash_method,
+            hash_pepper=self.cipher_conf['hash_pepper'],
+            password_pepper=self.cipher_conf['password_pepper']
+        )
+        
+        for file_tuple in file_data:
+            file_id: str = file_tuple[0]
+            data_length: int = file_tuple[1]
+
+            user_id: str = file_tuple[2]
+            dir_id: str = file_tuple[3]
+
+            tmp_id: str = secrets.token_hex(32)
+            with transaction(self.db) as cursor:
+                cursor.execute("""
+                    SELECT config FROM files_config
+                    WHERE data_id=?
+                """, [file_id])
+
+                fetched_conf: tuple[bytes] = cursor.fetchone()
+                if not fetched_conf:
+                    self.logger.warning("(update_encryption): File ID '%s' has no file config data", file_id)
+                    continue
+
+                msgpack_file_conf: bytes = fetched_conf[0]
+                file_conf: dict = msgpack.unpackb(msgpack_file_conf)
+
+                chunk_size: int = file_conf['chunk-size']
+                copy_offset: int = 1
+
+                write_offset: int = 1
+                cursor.execute("""
+                    INSERT INTO files (data_id, dir_id, user_id, filename, file_data)
+                    VALUES (?, ?, ?, ?, ?)
+                """, [tmp_id, dir_id, user_id, '', b''])
+                
+                while copy_offset < data_length:
+                    cursor.execute("""
+                        SELECT substr(file_data, ?, ?)
+                        FROM files
+                        WHERE data_id=?
+                    """, [copy_offset, chunk_size, file_id])
+                    chunk: bytes = cursor.fetchone()[0]
+
+                    copy_offset += chunk_size
+                    cursor.execute("""
+                        UPDATE files
+                        SET file_data = cast(file_data || ? AS BLOB)
+                        WHERE data_id=?
+                    """, [chunk, tmp_id])
+                
+                cursor.execute("""
+                    UPDATE files SET file_data=cast(? AS BLOB)
+                    WHERE data_id=?
+                """, [b'', file_id])
+                
+                while write_offset < data_length:
+                    cursor.execute("""
+                        SELECT substr(file_data, ?, ?)
+                        FROM files
+                        WHERE data_id=?
+                    """, [write_offset, chunk_size, tmp_id])
+                    data: bytes = cursor.fetchone()[0]
+
+                    if old_key:
+                        chunk: bytes = oldkey_cipher.decrypt(data)
+                    
+                    if new_key:
+                        chunk: bytes = newkey_cipher.encrypt(chunk)
+                    
+                    write_offset += chunk_size
+                    cursor.execute("""
+                        UPDATE files SET file_data = cast(file_data || ? AS BLOB)
+                        WHERE data_id=?
+                    """, [chunk, file_id])
+                
+                cursor.execute("DELETE FROM files WHERE data_id=?", [tmp_id])
+            
+            vac_cur: sqlite3.Cursor = self.db.cursor()
+            vac_cur.execute("VACUUM")
+            
+            vac_cur.close()
+            self.logger.info("(update_encryption): Updated file '%s' for user ID '%s'", file_id, user_id)
+
+        return 0
+    
+    def key_recovery(self, recovery_key: bytes | str) -> int | dict:
+        match recovery_key:
+            case bytes():
+                pass
+            case str():
+                recovery_key: bytes = recovery_key.encode('utf-8')
+            case _:
+                raise TypeError("recovery key is not bytes or string")
+        
+        recov_cipher: SimpleCipher = SimpleCipher(recovery_key, hash_method=self.hash_method)
+        original_encrypted_key: bytes = self.conf_vars.get('syncServer-recoveryKey')
+
+        if not original_encrypted_key:
+            raise ValueError("'syncServer-recoveryKey' could not be found in the config variables")
+        
+        try:
+            original_key: bytes = recov_cipher.decrypt(original_encrypted_key)
+        except cryptography.exceptions.InvalidTag:
+            self.logger.error("(key_recovery): Key decryption failed using recovery key")
+            return 1
+        
+        return original_key
+
+
 class DirectoryInterface:
     def __init__(self, parent: FileDatabase) -> None:
         self.db: sqlite3.Connection = parent.db
-        self.cursor: sqlite3.Cursor = parent.cursor
 
         self.pw_hasher: argon2.PasswordHasher = parent.pw_hasher
-        self.cipher_mgr: CipherManager = parent.cipher_mgr
+        self.cipher: SimpleCipher = parent.cipher
 
         self.conf_secrets: dict = parent.conf_secrets
         self.conf_vars: dict = parent.conf_vars
 
-        self._cipher_key: bytes | str = parent._cipher_key
         self.cipher_conf: dict = self.conf_secrets['encryption_config']
+        self._get_userid = parent._get_userid
 
-        self.dir_checker: Callable = parent.dir_checker
+        self._get_dirid = parent._get_dirid
     
     def make_dir(
             self, username: str,
             dir_path: str
     ) -> int | str:
         if not isinstance(dir_path, str):
             raise TypeError("'dir_path' must be string")
         
-        self.cursor.execute("""
-            SELECT user_id FROM users WHERE username=?
-        """, [username])
-        user_data = self.cursor.fetchone()
-
-        if not user_data:
+        user_id: str = self._get_userid(username)
+        if not user_id:
             return "NO_USER"
         
-        user_id = user_data[0]
-        self.cursor.execute("""
-            SELECT dir_id FROM directories
-            WHERE dir_name=? AND user_id=?
-        """, [dir_path, user_id])
-
-        found_filename = self.cursor.fetchone()
-        if found_filename:
+        dir_id: str = self._get_dirid(dir_path, user_id)
+        if dir_id:
             return "DIR_EXISTS"
         
         if not dir_path:
             return "MISSING_PATH"
         
         if dir_path[0] != "/":
             dir_path = "/" + dir_path
         
-        dirs = dir_path.split("/")
+        dirs: list[str] = dir_path.split("/")
         for i, dir_name in enumerate(dirs):
             if i == 0:
                 continue
 
             if not dir_name:
                 return "INVALID_DIR_PATH"
             
-        dir_id = str(uuid.uuid4())
-        with self.db:
-            self.cursor.execute("""
+        dir_id: str = str(uuid.uuid4())
+        with transaction(self.db) as cursor:
+            cursor.execute("""
                 INSERT INTO directories (dir_id, user_id, dir_name)
                 VALUES (?, ?, ?)
             """, [dir_id, user_id, dir_path])
         
         return 0
 
     def remove_dir(
             self, username: str,
             dir_path: str
     ) -> int | str:
         if not isinstance(dir_path, str):
             raise TypeError("'dir_path' must be string")
         
-        self.cursor.execute("""
-            SELECT user_id FROM users WHERE username=?
-        """, [username])
-        user_data = self.cursor.fetchone()
-
-        if not user_data:
+        user_id: str = self._get_userid(username)
+        if not user_id:
             return "NO_USER"
         
-        user_id = user_data[0]
-        self.cursor.execute("""
-            SELECT dir_id FROM directories
-            WHERE dir_name=? AND user_id=?
-        """, [dir_path, user_id])
-
-        found_dir = self.cursor.fetchone()
-        if not found_dir:
+        dir_id: str = self._get_dirid(dir_path, user_id)
+        if not dir_id:
             return "NO_DIR_EXISTS"
         
-        dir_id = found_dir[0]
         if dir_path == "/":
             return "ROOT_DIR"
         
-        dirs = dir_path.split("/")
+        dirs: list[str] = dir_path.split("/")
         for i, dir_name in enumerate(dirs):
             if i == 0:
                 continue
 
             if not dir_name:
                 return "INVALID_DIR_PATH"
 
-        with self.db:
-            self.cursor.execute("""
+        with transaction(self.db) as cursor:
+            cursor.execute("""
                 DELETE FROM directories
                 WHERE dir_id=? AND user_id=?
             """, [dir_id, user_id])
             
         return 0
 
     def list_dir(
@@ -966,184 +1289,170 @@
     ) -> str | list[str]:
         if not isinstance(dir_path, str):
             raise TypeError("'dir_path' must be string")
 
         if not isinstance(list_deleted_only, bool):
             raise TypeError("'list_deleted_only' can only be bool")
         
-        self.cursor.execute("""
-            SELECT user_id FROM users WHERE username=?
-        """, [username])
-        user_data: tuple[str] = self.cursor.fetchone()
-
-        if not user_data:
+        user_id: str = self._get_userid(username)
+        if not user_id:
             return "NO_USER"
         
-        user_id: str = user_data[0]
-        self.cursor.execute("""
-            SELECT dir_id FROM directories
-            WHERE dir_name=? AND user_id=?
-        """, [dir_path, user_id])
-
-        found_dir: tuple[str] = self.cursor.fetchone()
-        if not found_dir:
+        dir_id: str = self._get_dirid(dir_path, user_id)
+        if not dir_id:
             return "NO_DIR_EXISTS"
         
         dirs: list[str] = dir_path.split("/")
         for i, dir_name in enumerate(dirs):
             if i == 0:
                 continue
             elif dir_path == "/":
                 break
 
             if not dir_name:
                 return "INVALID_DIR_PATH"
 
-        dir_id: str = found_dir[0]
-        self.cursor.execute("""
-            SELECT filename, data_id FROM files
-            WHERE dir_id=? AND user_id=?
-        """, [dir_id, user_id])
-        dir_listing: list[tuple[str, str]] = self.cursor.fetchall()
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT filename, data_id FROM files
+                WHERE dir_id=? AND user_id=?
+            """, [dir_id, user_id])
+            dir_listing: list[tuple[str, str]] = cursor.fetchall()
 
         def is_deleted(file_id):
-            self.cursor.execute("""
-                SELECT data_id FROM deleted_files
-                WHERE data_id=?
-            """, [file_id])
-            delete_data: tuple[str] | None = self.cursor.fetchone()
+            with transaction(self.db) as cursor:
+                cursor.execute("""
+                    SELECT data_id FROM deleted_files
+                    WHERE data_id=?
+                """, [file_id])
+                delete_data: tuple[str] | None = cursor.fetchone()
+            
             return bool(delete_data) 
         
         if list_deleted_only:
             files: list[str] = [i[0] for i in dir_listing if is_deleted(i[1])]
         else:
             files: list[str] = [i[0] for i in dir_listing if not is_deleted(i[1])]
         
         return files
     
     def get_dir_paths(self, username: str) -> str | list[str]:
-        self.cursor.execute("""
-            SELECT user_id FROM users WHERE username=?
-        """, [username])
-        user_data: tuple[str] = self.cursor.fetchone()
-
-        if not user_data:
+        user_id: str = self._get_userid(username)
+        if not user_id:
             return "NO_USER"
         
-        user_id: str = user_data[0]
-        self.cursor.execute("""
-            SELECT dir_name FROM directories
-            WHERE user_id=?
-        """, [user_id])
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT dir_name FROM directories
+                WHERE user_id=?
+            """, [user_id])
 
-        dirs: list[tuple[str]] = self.cursor.fetchall()
+            dirs: list[tuple[str]] = cursor.fetchall()
+        
         if not dirs:
             return "NO_DIRS"  # This means even the root directory (/) is missing
         
         return [pathlist[0] for pathlist in dirs]
 
 
 class DeletedFiles:
     def __init__(self, parent: FileDatabase) -> None:
         self.db: sqlite3.Connection = parent.db
-        self.cursor: sqlite3.Cursor = parent.cursor
 
         self.pw_hasher: argon2.PasswordHasher = parent.pw_hasher
-        self.cipher_mgr: CipherManager = parent.cipher_mgr
+        self.cipher: SimpleCipher = parent.cipher
 
         self.conf_secrets: dict = parent.conf_secrets
         self.conf_vars: dict = parent.conf_vars
 
-        self._cipher_key: bytes | str = parent._cipher_key
         self.cipher_conf: dict = self.conf_secrets['encryption_config']
-
         self.dir_checker = parent.dir_checker
+
+        self._get_userid = parent._get_userid
     
     def list_deleted(
             self, username: str,
             file_path: str
     ) -> str | list[str] | dict:
         if not isinstance(file_path, str):
             raise TypeError("'file_path' must be string")
 
-        self.cursor.execute("""
-            SELECT user_id FROM users WHERE username=?
-        """, [username])
-        user_data: tuple[str] = self.cursor.fetchone()
-
-        if not user_data:
+        user_id: str = self._get_userid(username)
+        if not user_id:
             return "NO_USER"
 
-        user_id: str = user_data[0]
-
         if file_path == ":all:":
-            self.cursor.execute("""
-                SELECT filename, data_id FROM files
-                WHERE user_id=?
-            """, [user_id])
-            file_ids = self.cursor.fetchall()
+            with transaction(self.db) as cursor:
+                cursor.execute("""
+                    SELECT filename, data_id FROM files
+                    WHERE user_id=?
+                """, [user_id])
+                file_ids: list[tuple[str, str]] = cursor.fetchall()
 
             grouped_data: dict[str, list] = {}
             for item in file_ids:
                 filename, data_id = item
                 if filename in grouped_data:
                     grouped_data[filename].append(data_id)
                 else:
                     grouped_data[filename] = [data_id]
 
             # Convert dictionary values to lists of tuples
             result: list = [[(key, val) for val in grouped_data[key]] for key in grouped_data]
             all_results: dict = {}
 
-            for path_and_id_tuple in result:
-                for file_path, file_id in path_and_id_tuple:
-                    if file_path not in all_results:
-                        all_results[file_path] = []
+            with transaction(self.db) as cursor:
+                for path_and_id_tuple in result:
+                    for file_path, file_id in path_and_id_tuple:
+                        if file_path not in all_results:
+                            all_results[file_path] = []
+                        
+                        cursor.execute("""
+                            SELECT delete_date FROM deleted_files
+                            WHERE data_id=?
+                            ORDER BY delete_date DESC
+                        """, [file_id])
+                        tmp_del_date: tuple[str] = cursor.fetchone()
+
+                        if tmp_del_date:
+                            all_results[file_path].append(tmp_del_date[0])
                     
-                    self.cursor.execute("""
-                        SELECT delete_date FROM deleted_files
-                        WHERE data_id=?
-                        ORDER BY delete_date DESC
-                    """, [file_id])
-                    tmp_del_date = self.cursor.fetchone()
-                    if tmp_del_date:
-                        all_results[file_path].append(tmp_del_date[0])
+                    file_path = path_and_id_tuple[0][0]
+                    all_results[file_path] = sorted(all_results[file_path], reverse=True)
                 
-                file_path = path_and_id_tuple[0][0]
-                all_results[file_path] = sorted(all_results[file_path], reverse=True)
-            
             return all_results
 
-        dir_exists: tuple[str] = self.dir_checker(file_path, user_id)
-        if not dir_exists:
+        dir_id: str = self.dir_checker(username, file_path)
+        if not dir_id:
             return "NO_DIR_EXISTS"
 
-        dir_id: str = dir_exists[0]
-        self.cursor.execute("""
-            SELECT data_id FROM files
-            WHERE filename=? AND user_id=? AND dir_id=?
-        """, [file_path, user_id, dir_id])
-
-        file_data: list[tuple[str]] = self.cursor.fetchall()
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT data_id FROM files
+                WHERE filename=? AND user_id=? AND dir_id=?
+            """, [file_path, user_id, dir_id])
+            file_data: list[tuple[str]] = cursor.fetchall()
+        
         if not file_data:
             return "NO_MATCHING_FILES"
 
         delete_data: list = []
-        for file_tuple in file_data:
-            file_id: str = file_tuple[0]
-            self.cursor.execute("""
-                SELECT delete_date FROM deleted_files
-                WHERE data_id=?
-                ORDER BY delete_date DESC;
-            """, [file_id])
+        with transaction(self.db) as cursor:
+            for file_tuple in file_data:
+                file_id: str = file_tuple[0]
+                cursor.execute("""
+                    SELECT delete_date FROM deleted_files
+                    WHERE data_id=?
+                    ORDER BY delete_date DESC;
+                """, [file_id])
 
-            tmp_delete_data: tuple[str] = self.cursor.fetchone()
-            if tmp_delete_data:
-                delete_data.append(tmp_delete_data[0])
-                continue
+                tmp_delete_data: tuple[str] = cursor.fetchone()
+                if tmp_delete_data:
+                    delete_data.append(tmp_delete_data[0])
+                    continue
 
         if not delete_data:
             return "NO_MATCHING_FILES"
 
         return sorted(delete_data, reverse=True)
 
     def restore_file(
@@ -1154,57 +1463,53 @@
         if not isinstance(file_path, str):
             raise TypeError("'file_path' must be string")
 
         if not isinstance(restore_which, int):
             # Removed implicit restore
             raise TypeError("'restore_which' must be an int")
         
-        self.cursor.execute("""
-            SELECT user_id FROM users WHERE username=?
-        """, [username])
-        user_data: tuple[str] = self.cursor.fetchone()
-
-        if not user_data:
+        user_id: str = self._get_userid(username)
+        if not user_id:
             return "NO_USER"
-
-        user_id: str = user_data[0]
-
-        dir_exists: tuple[str] = self.dir_checker(file_path, user_id)
-        if not dir_exists:
+        
+        dir_id: str = self.dir_checker(username, file_path)
+        if not dir_id:
             return "NO_DIR_EXISTS"
 
-        dir_id: str = dir_exists[0]
-        self.cursor.execute("""
-            SELECT data_id FROM files
-            WHERE filename=? AND user_id=? AND dir_id=?
-        """, [file_path, user_id, dir_id])
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT data_id FROM files
+                WHERE filename=? AND user_id=? AND dir_id=?
+            """, [file_path, user_id, dir_id])
 
-        file_data: list[tuple[str]] = self.cursor.fetchall()
+            file_data: list[tuple[str]] = cursor.fetchall()
+        
         if not file_data:
             return "NO_FILE_EXISTS"
 
         delete_data: list = []
-        for file_tuple in file_data:
-            file_id: str = file_tuple[0]
-            self.cursor.execute("""
-                SELECT data_id FROM deleted_files
-                WHERE data_id=?
-                ORDER BY delete_date DESC
-            """, [file_id])
-
-            tmp_delete_data: tuple[str] = self.cursor.fetchone()
-            if tmp_delete_data:
-                del_data_id = tmp_delete_data[0]
-                delete_data.append(del_data_id)
-
-                continue
+        with transaction(self.db) as cursor:
+            for file_tuple in file_data:
+                file_id: str = file_tuple[0]
+                cursor.execute("""
+                    SELECT data_id FROM deleted_files
+                    WHERE data_id=?
+                    ORDER BY delete_date DESC
+                """, [file_id])
 
-            # Assume all IDs are in the deleted_files table, if not
-            # then assume there is one file that is not marked deleted
-            return "FILE_CONFLICT"
+                tmp_delete_data: tuple[str] = cursor.fetchone()
+                if tmp_delete_data:
+                    del_data_id = tmp_delete_data[0]
+                    delete_data.append(del_data_id)
+
+                    continue
+
+                # Assume all IDs are in the deleted_files table, if not
+                # then assume there is one file that is not marked deleted
+                return "FILE_CONFLICT"
 
         if not delete_data:
             return "FILE_NOT_DELETED"
         
         # If the value of restore_which is bigger than the length of deleted file ids
         # minus one (since we index starting from zero), then assume out of bounds
         def in_bounds():
@@ -1218,20 +1523,20 @@
         
         if not in_bounds():
             return "OUT_OF_BOUNDS"
 
         # SQLite3 returns the whole list oldest -> latest so we reverse it
         delete_data: list = list(reversed(delete_data))
 
-        with self.db:
+        with transaction(self.db) as cursor:
             # Fetch the list with the data ids and then get the data id
             # [ ('data-id') ] -> delete_data[restore_which]
 
             data_id: str = delete_data[restore_which]
-            self.cursor.execute("""
+            cursor.execute("""
                 DELETE FROM deleted_files
                 WHERE data_id=?
             """, [data_id])
 
         return 0
     
     def true_delete(
@@ -1241,52 +1546,49 @@
     ) -> str | int:
         if not isinstance(file_path, str):
             raise TypeError("'file_path' must be string")
 
         if not (delete_which == ":all:" or isinstance(delete_which, int)):
             raise TypeError("'delete_which' can only be an int or ':all:'")
         
-        self.cursor.execute("""
-            SELECT user_id FROM users WHERE username=?
-        """, [username])
-        user_data: tuple[str] = self.cursor.fetchone()
-
-        if not user_data:
+        user_id: str = self._get_userid(username)
+        if not user_id:
             return "NO_USER"
-
-        user_id: str = user_data[0]
-        dir_exists: tuple[str] = self.dir_checker(file_path, user_id)
-        if not dir_exists:
+        
+        dir_id: str = self.dir_checker(username, file_path)
+        if not dir_id:
             return "NO_DIR_EXISTS"
 
-        dir_id: str = dir_exists[0]
-        self.cursor.execute("""
-            SELECT data_id FROM files
-            WHERE filename=? AND user_id=? AND dir_id=?
-        """, [file_path, user_id, dir_id])
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT data_id FROM files
+                WHERE filename=? AND user_id=? AND dir_id=?
+            """, [file_path, user_id, dir_id])
 
-        file_data: list[tuple[str]] = self.cursor.fetchall()
+            file_data: list[tuple[str]] = cursor.fetchall()
+        
         if not file_data:
             return "NO_MATCHING_FILES"
 
         delete_data: list = []
-        for file_tuple in file_data:
-            file_id: str = file_tuple[0]
-            self.cursor.execute("""
-                SELECT data_id FROM deleted_files
-                WHERE data_id=?
-                ORDER BY delete_date DESC
-            """, [file_id])
+        with transaction(self.db) as cursor:
+            for file_tuple in file_data:
+                file_id: str = file_tuple[0]
+                cursor.execute("""
+                    SELECT data_id FROM deleted_files
+                    WHERE data_id=?
+                    ORDER BY delete_date DESC
+                """, [file_id])
 
-            tmp_delete_data: tuple[str] = self.cursor.fetchone()
-            if tmp_delete_data:
-                del_data_id: str = tmp_delete_data[0]
-                delete_data.append(del_data_id)
+                tmp_delete_data: tuple[str] = cursor.fetchone()
+                if tmp_delete_data:
+                    del_data_id: str = tmp_delete_data[0]
+                    delete_data.append(del_data_id)
 
-                continue
+                    continue
         
         if not delete_data:
             return "NO_MATCHING_FILES"
 
         # If the value of delete_which is bigger than the length of deleted file ids
         # minus one (since we index starting from zero), then assume out of bounds
         def in_bounds() -> bool:
@@ -1303,88 +1605,82 @@
         
         if not in_bounds():
             return "OUT_OF_BOUNDS"
 
         # SQLite3 returns the whole list oldest -> latest so we reverse it
         delete_data: list[str] = list(reversed(delete_data))
 
-        if delete_which == ":all:":
-            with self.db:
+        with transaction(self.db) as cursor:
+            if delete_which == ":all:":            
                 for file_id_to_delete in delete_data:
-                    self.cursor.execute("""
+                    cursor.execute("""
                         DELETE FROM files
                         WHERE data_id=?
                     """, [file_id_to_delete])
-        else:
-            with self.db:
+            else:
                 delete_which_id: str = delete_data[delete_which]
-                self.cursor.execute("""
+                cursor.execute("""
                     DELETE FROM files
                     WHERE data_id=?
                 """, [delete_which_id])
-        
+            
         return 0
 
 
 class APIKeyInterface:
     def __init__(self, parent: FileDatabase) -> None:
         self.db: sqlite3.Connection = parent.db
-        self.cursor: sqlite3.Cursor = parent.cursor
 
         self.pw_hasher: argon2.PasswordHasher = parent.pw_hasher
-        self.cipher_mgr: CipherManager = parent.cipher_mgr
+        self.cipher: SimpleCipher = parent.cipher
 
         self.conf_secrets: dict = parent.conf_secrets
         self.conf_vars: dict = parent.conf_vars
 
-        self._cipher_key: bytes | str = parent._cipher_key
         self.cipher_conf: dict = self.conf_secrets['encryption_config']
 
         self.perms_list: list[str] = ['create', 'read', 'update', 'delete', 'all']
+        self._get_userid = parent._get_userid
     
     def _hash_key(self, api_key: str) -> str:
         if not isinstance(api_key, str):
             raise TypeError("'api_key' must be string")
         
-        match api_key:
-            case bytes():
-                pass
-            case str():
-                api_key = api_key.encode('utf-8')
+        api_key: bytes = api_key.encode('utf-8')
         
         hash_pepper: bytes = self.cipher_conf.get('hash_pepper', b'')
-        hashed_apikey: str = self.cipher_mgr.hash_string(hash_pepper + api_key)
+        hashed_apikey: str = self.cipher.hash_data(api_key + hash_pepper)
 
         return hashed_apikey
     
-    def get_key_owner(
-        self, api_key: str
-    ) -> str:
+    def get_key_owner(self, api_key: str) -> str:
         if not isinstance(api_key, str):
             raise TypeError("'api_key' must be a string")
 
         hashed_apikey: str = self._hash_key(api_key)
-        self.cursor.execute("""
-            SELECT user_id, key_id FROM user_apikeys
-            WHERE api_key=?
-        """, [hashed_apikey])
-        key_data: tuple[str] = self.cursor.fetchone()
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT user_id, key_id FROM user_apikeys
+                WHERE api_key=?
+            """, [hashed_apikey])
+            key_data: tuple[str] = cursor.fetchone()
         
         if not key_data:
             return "INVALID_APIKEY"
         
         user_id: str = key_data[0]
         key_id: str = key_data[1]
 
-        self.cursor.execute("""
-            SELECT username FROM users
-            WHERE user_id=?
-        """, [user_id])
-        user_data: tuple[str] = self.cursor.fetchone()
-        
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT username FROM users
+                WHERE user_id=?
+            """, [user_id])
+            user_data: tuple[str] = cursor.fetchone()
+            
         if not user_data:
             logging.warning(
                 "[APIKeyInterface-keyWithoutOwner]: An key was found in "
                 "the database, but has no owner. Key ID: [%s]",
                 key_id
             )
             return "INVALID_APIKEY"  # key has no owner but exists in the database
@@ -1401,20 +1697,21 @@
         if not isinstance(permission_type, str):
             raise TypeError("'permission_type' must be a string")
         
         if permission_type not in self.perms_list:
             return "INVALID_PERMISSION"
         
         hashed_apikey: str = self._hash_key(api_key)
-        self.cursor.execute("""
-            SELECT user_id, key_perms FROM user_apikeys
-            WHERE api_key=?
-        """, [hashed_apikey])
-        perms_data: tuple[str] = self.cursor.fetchone()
-        
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT user_id, key_perms FROM user_apikeys
+                WHERE api_key=?
+            """, [hashed_apikey])
+            perms_data: tuple[str] = cursor.fetchone()
+            
         if not perms_data:
             return "INVALID_APIKEY"
 
         encoded_key_perms: bytes = perms_data[1]
         key_perms: list[str] = msgpack.unpackb(encoded_key_perms)
 
         if permission_type not in key_perms:
@@ -1449,47 +1746,42 @@
             return "INVALID_DATETIME"
 
         date_today: datetime = datetime.now()
         if date_today > expiry_date:
             # Prevent creating an already expired API key
             return "DATE_EXPIRED"
         
-        self.cursor.execute("""
-            SELECT user_id FROM users WHERE username=?
-        """, [username])
-        user_data: tuple[str] = self.cursor.fetchone()
-
-        if not user_data:
+        user_id: str = self._get_userid(username)
+        if not user_id:
             return "NO_USER"
         
-        user_id: str = user_data[0]
-        
-        self.cursor.execute("""
-            SELECT key_id FROM user_apikeys
-            WHERE key_name=? AND user_id=?
-        """, [key_name, user_id])
-        key_data: tuple[str] = self.cursor.fetchone()
-
-        if key_data:
-            return "APIKEY_EXISTS"
-        
         salt: bytes = secrets.token_hex(32)
-        hashed_userid: str = self.cipher_mgr.hash_string(user_id + salt)
+        hashed_userid: str = self.cipher.hash_data(user_id + salt)
 
         api_key: str = f"syncServer-{hashed_userid}"
         hashed_apikey: str = self._hash_key(api_key)
-        with self.db:
-            key_id: str = str(uuid.uuid4())
-            encoded_key_perms: bytes = msgpack.packb(key_perms)
-
-            insert_data: list[str] = [
-                key_id, user_id, key_name,
-                hashed_apikey, encoded_key_perms, expires_on
-            ]
-            self.cursor.execute("""
+
+        key_id: str = str(uuid.uuid4())
+        encoded_key_perms: bytes = msgpack.packb(key_perms)
+
+        insert_data: list[str] = [
+            key_id, user_id, key_name,
+            hashed_apikey, encoded_key_perms, expires_on
+        ]
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT key_id FROM user_apikeys
+                WHERE key_name=? AND user_id=?
+            """, [key_name, user_id])
+            key_data: tuple[str] = cursor.fetchone()
+
+            if key_data:
+                return "APIKEY_EXISTS"
+            
+            cursor.execute("""
                 INSERT INTO user_apikeys (
                     key_id, user_id, key_name,
                     api_key, key_perms, expiry_date
                 ) VALUES (?, ?, ?, ?, ?, ?)
             """, insert_data)
         
         return api_key
@@ -1500,75 +1792,67 @@
     ) -> int | str:
         if not isinstance(username, str):
             raise TypeError("'username' must be a string")
         
         if not isinstance(key_name, str):
             raise TypeError("'key_name' must be a string")
         
-        self.cursor.execute("""
-            SELECT user_id FROM users WHERE username=?
-        """, [username])
-        user_data: tuple[str] = self.cursor.fetchone()
-        
-        if not user_data:
+        user_id: str = self._get_userid(username)
+        if not user_id:
             return "NO_USER"
-        
-        user_id: str = user_data[0]
-        self.cursor.execute("""
-            SELECT key_id FROM user_apikeys
-            WHERE user_id=? AND key_name=?
-        """, [user_id, key_name])
-        key_data: tuple[str] = self.cursor.fetchone()
-        
-        if not key_data:
-            return "INVALID_APIKEY"
-        
-        key_id: str = key_data[0]
-        with self.db:
-            self.cursor.execute("""
+                
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT key_id FROM user_apikeys
+                WHERE key_name=? AND user_id=?
+            """, [key_name, user_id])
+            key_data: tuple[str] = cursor.fetchone()
+
+            if not key_data:
+                return "INVALID_APIKEY"
+            
+            key_id: str = key_data[0]
+            cursor.execute("""
                 DELETE FROM user_apikeys
                 WHERE key_id=? AND user_id=?
             """, [key_id, user_id])
         
         return 0
 
     def list_keys(self, username: str) -> str | list[str]:
         if not isinstance(username, str):
             raise TypeError("'username' must be a string")
         
-        self.cursor.execute("""
-            SELECT user_id FROM users WHERE username=?
-        """, [username])
-        user_data: tuple[str] = self.cursor.fetchone()
-        
-        if not user_data:
+        user_id: str = self._get_userid(username)
+        if not user_id:
             return "NO_USER"
         
-        user_id: str = user_data[0]
-        self.cursor.execute("""
-            SELECT key_name FROM user_apikeys
-            WHERE user_id=?
-        """, [user_id])
-        key_data: tuple[str] = self.cursor.fetchall()
-        
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT key_name FROM user_apikeys
+                WHERE user_id=?
+            """, [user_id])
+            key_data: tuple[str] = cursor.fetchall()
+            
         if not key_data:
             return []
 
         return [key_tuple[0] for key_tuple in key_data]
     
     def apikey_get_data(self, api_key: str) -> list[list[str], str] | str:
         if not isinstance(api_key, str):
             raise TypeError("'api_key' must be a string")
         
         hashed_apikey: str = self._hash_key(api_key)
-        self.cursor.execute("""
-            SELECT key_perms, expiry_date FROM user_apikeys
-            WHERE api_key=?
-        """, [hashed_apikey])
-        key_data: tuple[bytes, str] = self.cursor.fetchone()
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT key_perms, expiry_date FROM user_apikeys
+                WHERE api_key=?
+            """, [hashed_apikey])
+            key_data: tuple[bytes, str] = cursor.fetchone()
 
         if not key_data:
             return "INVALID_APIKEY"
 
         key_perms: list[str] = msgpack.unpackb(key_data[0])
         expiry_date: str = key_data[1]
         
@@ -1577,29 +1861,25 @@
     def keyname_get_data(self, username: str, key_name: str) -> list[list[str], str] | str:
         if not isinstance(username, str):
             raise TypeError("'username' must be a string")
         
         if not isinstance(key_name, str):
             raise TypeError("'key_name' must be a string")
         
-        self.cursor.execute("""
-            SELECT user_id FROM users WHERE username=?
-        """, [username])
-        user_data: tuple[str] = self.cursor.fetchone()
-        
-        if not user_data:
+        user_id: str = self._get_userid(username)
+        if not user_id:
             return "NO_USER"
         
-        user_id: str = user_data[0]
-        self.cursor.execute("""
-            SELECT key_perms, expiry_date FROM user_apikeys
-            WHERE user_id=? AND key_name=?
-        """, [user_id, key_name])
-        key_data: tuple[bytes, str] = self.cursor.fetchone()
-        
+        with transaction(self.db) as cursor:
+            cursor.execute("""
+                SELECT key_perms, expiry_date FROM user_apikeys
+                WHERE user_id=? AND key_name=?
+            """, [user_id, key_name])
+            key_data: tuple[bytes, str] = cursor.fetchone()
+
         if not key_data:
             return "INVALID_APIKEY"
         
         key_perms: list[str] = msgpack.unpackb(key_data[0])
         expiry_date: str = key_data[1]
         
         return [key_perms, expiry_date]
@@ -1623,37 +1903,33 @@
         
         if not isinstance(key_name, str):
             raise TypeError("'key_name' must be a string")
         
         if not isinstance(username, str):
             raise TypeError("'username' is not a string")
         
-        if api_key:
-            hashed_apikey: str = self._hash_key(api_key)
-            self.cursor.execute("""
-                SELECT expiry_date FROM user_apikeys
-                WHERE api_key=?
-            """, [hashed_apikey])
-            expiry_data: tuple[str] = self.cursor.fetchone()
-        else:
-            self.cursor.execute("""
-                SELECT user_id FROM users WHERE username=?
-            """, [username])
-            user_data: tuple[str] = self.cursor.fetchone()
-            
-            if not user_data:
-                return "NO_USER"
+        with transaction(self.db) as cursor:
+            if api_key:
+                hashed_apikey: str = self._hash_key(api_key)
+                cursor.execute("""
+                    SELECT expiry_date FROM user_apikeys
+                    WHERE api_key=?
+                """, [hashed_apikey])
+                expiry_data: tuple[str] = cursor.fetchone()
+            else:
+                user_id: str = self._get_userid(username)
+                if not user_id:
+                    return "NO_USER"
+        
+                cursor.execute("""
+                    SELECT expiry_date FROM user_apikeys
+                    WHERE key_name=? AND user_id=?
+                """, [key_name, user_id])
+                expiry_data: tuple[str] = cursor.fetchone()
             
-            user_id: str = user_data[0]
-            self.cursor.execute("""
-                SELECT expiry_date FROM user_apikeys
-                WHERE key_name=? AND user_id=?
-            """, [key_name, user_id])
-            expiry_data: tuple[str] = self.cursor.fetchone()
-        
         if not expiry_data:
             return "INVALID_APIKEY"
         
         expiry_date: datetime = datetime.strptime(expiry_data[0], "%Y-%m-%d %H:%M:%S")
         current_time: datetime = datetime.now()
 
         expired: bool = current_time > expiry_date
@@ -1677,19 +1953,14 @@
             '--database-path', '-db',
             action='store', 
             nargs='?',
             metavar='db-path',
             help="Path to syncServer database."
         )
         self.parser.add_argument(
-            '--database-protected', '-dp',
-            action='store_true',
-            help="Prompt to enter the database password."
-        )
-        self.parser.add_argument(
             '--recover-key', '-rk',
             action='store_true',
             help="Recover the original encryption key with the key password."
         )
         self.parser.add_argument(
             '--edit-vars', '-ev',
             action='store_true',
@@ -1773,154 +2044,143 @@
             temp_file.seek(0)
             edited_conf_data: str = temp_file.read()
         
         return edited_conf_data
     
     def parse_args(self) -> None:
         args = self.parser.parse_args()
-        if args.database_protected:
-            db_password: str = getpass.getpass("Enter the database password: ")
-        else:
-            db_password: str = ''
+        if not args.database_path:
+            args.database_path = ''
         
+        recov_mode_db: FileDatabase = FileDatabase(
+            db_path=args.database_path,
+            recovery_mode=True
+        )
         if args.recover_key:
-            self.db: FileDatabase = FileDatabase(
-                db_path=args.database_path,
-                recovery_mode=True
-            )
-            conf_data: dict = self.db.conf_vars
-            recovery_key: bytes = conf_data.get('syncServer-recoveryKey')
+            recov_key: str = getpass.getpass("Enter the exported recovery key: ")
+            key: int | bytes = recov_mode_db.db_admin.key_recovery(recov_key)
 
-            if not recovery_key:
-                self.parser.exit(
-                    1, "Could not find recovery key entry in config variables, is encryption enabled?\n"
-                )
-
-            key_password: str = getpass.getpass("Enter the recovery key: ")            
-            try:
-                original_key: bytes = self.db.cipher_mgr.fernet.decrypt_data(
-                    recovery_key, password=key_password
-                )
-            except cryptography.fernet.InvalidToken:  # type: ignore
-                self.parser.exit(1, "Decrypting recovery key failed!\n")
+            if key == 1:
+                self.parser.exit(1, "Key decryption failed! Wrong recovery key?")
             
-            self.parser.exit(0, f"Found original key: {original_key}\n")
-
+            self.parser.exit(0, f"Found original password: {key}\n")
+        
         if args.edit_vars:
-            self.db: FileDatabase = FileDatabase(
-                db_path=args.database_path,
-                recovery_mode=True
-            )
-            formatted_data: str = self._fmt_data(self.db.conf_vars, indent=4)
+            formatted_data: str = self._fmt_data(recov_mode_db.conf_vars, indent=4)
             edited_conf_data: str = self.display_conf(formatted_data)
 
             try:
                 edited_conf: dict = ast.literal_eval(edited_conf_data)
             except SyntaxError:
                 self.parser.exit(1, "Invalid configuration syntax, is the syntax in Python?\n")
 
-            self.db.save_conf(None, edited_conf)
-            if edited_conf == self.db.conf_vars:
+            recov_mode_db.db_admin.save_conf(None, edited_conf)
+            if edited_conf == recov_mode_db.conf_vars:
                 self.parser.exit(0, "No modifications to configuration variables.\n")
             
             self.parser.exit(0, "Saved configuration variables successfully!\n")
         
-        # Reach this point only if not recovering database
-        self.db: FileDatabase = FileDatabase(
-            db_path=args.database_path,
-            db_password=db_password
+        if recov_mode_db.conf_vars.get('syncServer-protected'):
+            db_password: str = getpass.getpass("Enter database password: ")
+        else:
+            db_password: str = ''
+        
+        normal_db: FileDatabase = FileDatabase(
+            args.database_path,
+            db_password
         )
 
+        normal_conf_secrets: dict = normal_db.conf_secrets
+        normal_conf_vars: dict = normal_db.conf_vars
+
         if args.edit_config:
-            conf_data = {
-                'secrets': self.db.conf_secrets, 
-                'vars': self.db.conf_vars
+            conf_data: dict = {
+                'secrets': normal_conf_secrets, 
+                'vars': normal_conf_vars
             }
             formatted_data: str = self._fmt_data(conf_data, indent=4)
             edited_conf_data: str = self.display_conf(formatted_data)
             
             try:
                 edited_conf: dict = ast.literal_eval(edited_conf_data)
             except SyntaxError:
                 self.parser.exit(1, "Invalid configuration syntax, is the syntax in Python?\n")
             
             if 'secrets' not in edited_conf or 'vars' not in edited_conf:
-                self.parser.exit(1, "'secrets' or 'vars' configuration is missing!\n")
+                self.parser.exit(2, "'secrets' or 'vars' configuration is missing!\n")
             
-            secrets_is_same: bool = self.db.conf_secrets == edited_conf['secrets']
-            vars_is_same: bool = self.db.conf_vars == edited_conf['vars']
+            secrets_is_same: bool = normal_conf_secrets == edited_conf['secrets']
+            vars_is_same: bool = normal_conf_vars == edited_conf['vars']
             if secrets_is_same and vars_is_same:
                 self.parser.exit(0, "No modifications to configuration settings.\n")
             
-            self.db.save_conf(edited_conf['secrets'], edited_conf['vars'])
+            normal_db.db_admin.save_conf(edited_conf['secrets'], edited_conf['vars'])
             self.parser.exit(0, 'Saved configuration successfully!\n')
         
         if args.set_protection:
-            conf_data: dict = {
-                'cipher_key': b""
-            }
+            conf_data: dict = {'cipher_key': b"", 'recovery_key_path': ''}
             formatted_data: str = self._fmt_data(conf_data, indent=4)
             edited_conf_data: str = self.display_conf(formatted_data)
             
-            if os.path.isfile("./syncServer-recoveryKey.key"):
-                emsg: str = (
-                    "Warning: Recovery key file exists in current directory, "
-                    "delete or move this file before changing encryption key\n"
-                )
-                self.parser.exit(0, emsg)
-            
             try:
                 edited_conf: dict = ast.literal_eval(edited_conf_data)
             except SyntaxError:
                 self.parser.exit(1, "Invalid configuration syntax, is the syntax in Python?\n")
 
-            if 'cipher_key' not in edited_conf:
-                self.parser.exit(1, "'cipher_key' configuration is missing!\n")
-            
-            cipher_key: bytes | str = edited_conf['cipher_key']
-            if not isinstance(cipher_key, (bytes, str)) and cipher_key is not None:
-                self.parser.exit(1, "Cipher key is not bytes or string!\n")
-            
-            if not cipher_key and cipher_key is not None:
-                self.parser.exit(1, "Set 'cipher_key' to None to disable protection!\n")
-            
-            if self.db.conf_vars['syncServer-encryptionEnabled']:
-                print("Warning: This will not re-encrypt existing data.")
-                warning_input: str = input(
-                    "Files and data were previously encrypted in this database "
-                    "with a different key. Proceed anyway? [Y/N]: "
+            cipher_key: bytes | str = edited_conf.get('cipher_key', -1)
+            recovery_key_path: bytes | str = edited_conf.get('recovery_key_path')
+
+            if cipher_key == -1:
+                self.parser.exit(2, "'cipher_key' value is missing!\n")
+            if not recovery_key_path and cipher_key:
+                self.parser.exit(2, "'recovery_key_path' value is missing!\n")
+
+            if not isinstance(cipher_key, (bytes, str)):
+                self.parser.exit(3, "Cipher key is not bytes or string!\n")
+            if not isinstance(recovery_key_path, (bytes, str)):
+                self.parser.exit(3, "Recovery key path is not bytes or string!\n")
+            
+            with transaction(normal_db.db) as cursor:
+                cursor.execute("SELECT data_id FROM files")
+                file_data: tuple[str] = cursor.fetchone()
+
+            if file_data:
+                print(
+                    "Files detected! The program will attempt to re-encrypt their contents. "
+                    "This may take a while.\n"
                 )
-                if warning_input.lower() != "y":
+                continue_input: str = input("Continue? [y/N]: ")
+                if continue_input.lower() != 'y':
                     self.parser.exit(0, "Aborted.\n")
-            
-            set_protection: bool = bool(cipher_key)
-            self.db.set_protection(set_protection, cipher_key)
-            
-            self.parser.exit(0, "Saved database protection status!\n")
+                
+            normal_db.db_admin.update_encryption(db_password, cipher_key)
+            normal_db.db_admin.set_protection(cipher_key, recovery_key_path)
 
+            self.parser.exit(0, "Updated encryption key!\n")
+        
         if args.add_user:
             print("Now starting new user configuration!\n")
             username: str = input("Enter a username: ")
             password: str = getpass.getpass("Enter a password: ")
 
             if not username or not password:
-                self.parser.exit(1, "Username or password is empty!\n")
+                self.parser.exit(2, "Username or password is empty!\n")
 
-            result: str | int = self.db.add_user(username, password)
+            result: str | int = normal_db.add_user(username, password)
             if result == "USER_EXISTS":
                 self.parser.exit(1, f"User '{username}' already exists!\n")
             
             self.parser.exit(0, f"Added new user '{username}'!\n")
 
         if args.remove_user:
             username: str = input("Enter the username to delete: ")
             if not username:
-                self.parser.exit(1, "No username was provided!\n")
+                self.parser.exit(2, "No username was provided!\n")
             
-            result: int | str = self.db.remove_user(username)
+            result: int | str = normal_db.remove_user(username)
             if result == "NO_USER":
                 self.parser.exit(1, "User does not exist!\n")
 
             self.parser.exit(0, f"Removed user '{username}' and their data successfully!\n")
 
 
 def run_cli():
```

### Comparing `newguy103-syncserver-1.2.0/syncserver/server/_server.py` & `newguy103_syncserver-1.3.0/syncserver/server/_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,82 @@
 import logging
 import getpass
+import atexit
 
 import secrets
 import types
 import os
+
 from typing import Generator
 
 import flask
-
-from flask import Flask, request
+from flask import Flask, request, g
 
 # from ._db import FileDatabase 
 from ._db import FileDatabase  # use the above import once making setup.py
 
-__version__: str = "1.2.0"
+__version__: str = "1.3.0"
 APP: flask.Flask = Flask(__name__)
 
-database: FileDatabase | None = None
-
-
-def SERVER_ERROR() -> flask.Response:
-    return flask.make_response({
-        'error': "Internal Server Error",
-        'ecode': "SERVER_ERROR"
-    }, 500)
-
 
 def NOT_JSON_ERROR() -> flask.Response:
     return flask.make_response({
         'error': "Provided request must be in a JSON format",
         'ecode': "415"
     }, 415)
 
 
+def create_app():
+    db_password: str = os.environ.get("SYNCSERVER_DBPASSWORD", '')
+    if not db_password:
+        db_password: str = getpass.getpass("Enter database password [or empty if not protected]: ")
+    
+    use_cache: str = os.environ.get("SYNCSERVER_CACHE_ENABLED", '')
+    file_db: FileDatabase = FileDatabase(
+        db_password=db_password, 
+        dict_cache=bool(use_cache)
+    )
+    with APP.app_context():
+        APP.config['SYNCSERVER-DATABASE'] = file_db
+
+    logging.basicConfig(
+        level=logging.DEBUG,
+        format='[%(asctime)s] - [%(levelname)s] - %(message)s',
+        datefmt='%Y-%m-%d %H:%M:%S',
+        handlers=[
+            logging.StreamHandler(),
+            logging.FileHandler('syncServer-serverApp.log')
+        ]
+    )
+    return APP
+
+
+@atexit.register
+def teardown_app():
+    logging.info("Shutting down syncServer. . .")
+
+    with APP.app_context():
+        db: FileDatabase = APP.config.pop('SYNCSERVER-DATABASE', None)
+        if db is not None:
+            db.close()
+            logging.info("Closed database connection!")
+
+
 def _verify(headers: dict, _api_permission_type: str = '') -> flask.Response | int:
     """
     Return response depending on token verification status,
     can either be using username/password or API key.
     """
 
-    global database
-
+    if not flask.has_app_context():
+        raise RuntimeError("using _verify without flask app context")
+    
+    database = APP.config.get('SYNCSERVER-DATABASE')
     api_key: str = headers.get('Authorization', '')
+
     if not isinstance(api_key, str):
         return flask.make_response({
             'error': "Provided API key is not a string",
             'ecode': "INVALID_TYPE"
         }, 400)
 
     if api_key:
@@ -66,15 +97,15 @@
                     'ecode': result
                 }, 401)
             case _:
                 logging.error(
                     "[FLASK-API-VERIFY]: API Key verifier function returned unexpected data: '%s'",
                     result
                 )
-                return SERVER_ERROR()
+                return flask.abort(500)
         
         is_expired: bool = database.api_keys.check_expired(api_key=api_key)
         if isinstance(is_expired, bool) and is_expired:
             return flask.make_response({
                 'error': "API key has expired",
                 'ecode': "EXPIRED_APIKEY"
             }, 401)
@@ -106,25 +137,40 @@
             'error': "User credentials are invalid.",
             'ecode': "INVALID_CREDENTIALS"
         }, 401)
         return err_response
             
     if isinstance(token_verified_result, Exception):
         logging.error("[FLASK-VERIFY-USER]: Refer to [Database.verify_user] error logs for information")
-        return SERVER_ERROR()
+        return flask.abort(500)
 
     return 0
 
 
+@APP.errorhandler(500)
+def return_servererror(e):
+    logging.error("Internal server error raised: %s", e)
+    return flask.make_response({
+        'error': "Internal Server Error",
+        'ecode': "SERVER_ERROR"
+    }, 500)
+
+
+@APP.before_request
+def init_request():
+    g.db = APP.config.get('SYNCSERVER-DATABASE')
+
+
 @APP.get('/auth/check')
 def check_creds():
-    global database
     headers = request.headers
 
-    verify_result = _verify(headers, _api_permission_type='all')
+    with APP.app_context():
+        verify_result = _verify(headers, _api_permission_type='all')
+    
     if verify_result != 0:
         return verify_result
     
     username: str = headers.get('syncServer-Username')
     password: str = headers.get('syncServer-Password')
 
     api_key: str = headers.get('Authorization')
@@ -136,27 +182,28 @@
     elif username and password:
         return flask.make_response({
             'auth-type': 'password', 
             'success': True
         }, 200)
     
     # If both are blank
-    logging.error("[/auth/check]: API key and username/password credentials are blank")
-    return SERVER_ERROR()
+    logging.error("[/auth/check]: Reached unreachable point in function")
+    return flask.abort(500)
 
 
 @APP.post('/api/files/upload')
-@APP.post("/upload")
 def file_uploads():
-    global database
+    database = g.db
 
     files = request.files
     headers = request.headers
 
-    verify_result = _verify(headers, _api_permission_type='create')
+    with APP.app_context():
+        verify_result = _verify(headers, _api_permission_type='create')
+    
     if verify_result != 0:
         return verify_result
 
     if len(files) == 0:
         return flask.make_response({
             'error': 'No files provided to upload',
             'ecode': 'MISSING_FILES'
@@ -227,15 +274,15 @@
             case 0:
                 successful_runs.append(file.name)
             case _:
                 logging.error(
                     "[/upload]: add_file function returned unexpected data: '%s'",
                     result
                 )
-                return SERVER_ERROR()
+                return flask.abort(500)
             
     response = None
     match len(files):
         case 1 if failed_runs.keys():
             first_key: str = list(failed_runs.keys())[0]
             response = failed_runs[first_key]
         case 1 if successful_runs:
@@ -251,22 +298,23 @@
             }
             response_code = 200
 
     return flask.make_response(response, response_code)
 
 
 @APP.post("/api/files/modify")
-@APP.post("/modify")
 def file_updates():
-    global database
+    database = g.db
 
     files = request.files
     headers = request.headers
 
-    verify_result = _verify(headers, _api_permission_type='update')
+    with APP.app_context():
+        verify_result = _verify(headers, _api_permission_type='update')
+    
     if verify_result != 0:
         return verify_result
 
     if len(files) == 0:
         return flask.make_response({
             'error': 'No files provided to upload',
             'ecode': 'MISSING_FILES'
@@ -338,15 +386,15 @@
             case 0:
                 successful_runs.append(file.name)
             case _:
                 logging.error(
                     "[/modify]: modify_file function returned unexpected data: '%s'",
                     result
                 )
-                return SERVER_ERROR()
+                return flask.abort(500)
             
     response: dict = None
     match len(files):
         case 1 if failed_runs.keys():
             first_key: str = list(failed_runs.keys())[0]
             response: dict[str, str] = failed_runs[first_key]
         case 1 if successful_runs:
@@ -362,25 +410,26 @@
             }
             response_code: int = 200
     
     return flask.make_response(response, response_code)
 
 
 @APP.post("/api/files/delete")
-@APP.post("/delete")
 def file_deletes():
-    global database
+    database = g.db
 
     if not request.is_json:
         return NOT_JSON_ERROR()
             
     data = request.json
     headers = request.headers
 
-    verify_result = _verify(headers, _api_permission_type='delete')
+    with APP.app_context():
+        verify_result = _verify(headers, _api_permission_type='delete')
+    
     if verify_result != 0:
         return verify_result
             
     username: str = database.api_keys.get_key_owner(headers.get('Authorization', ""))
     if username == "INVALID_APIKEY":
         username: str = headers.get('syncServer-Username', '')
             
@@ -446,15 +495,15 @@
             case 0:
                 successful_runs.append(file)
             case _:
                 logging.error(
                     "[/delete]: remove_file function returned unexpected data: '%s'",
                     result
                 )
-                return SERVER_ERROR()
+                return flask.abort(500)
             
     response: dict = None
     match len(filenames):
         case 1 if failed_runs.keys():
             first_key: str = list(failed_runs.keys())[0]
             response: dict[str, str] = failed_runs[first_key]
         case 1 if successful_runs:
@@ -476,25 +525,26 @@
             }
             response_code = 200
                 
     return flask.make_response(response, response_code)
 
 
 @APP.post("/api/files/restore")
-@APP.post("/restore")
 def file_restores():
-    global database
+    database = g.db
 
     if not request.is_json:
         return NOT_JSON_ERROR()
             
     data = request.json
     headers = request.headers
 
-    verify_result = _verify(headers, _api_permission_type='update')
+    with APP.app_context():
+        verify_result = _verify(headers, _api_permission_type='update')
+    
     if verify_result != 0:
         return verify_result
             
     username: str = database.api_keys.get_key_owner(headers.get('Authorization', ""))
     if username == "INVALID_APIKEY":
         username: str = headers.get('syncServer-Username', '')
             
@@ -568,31 +618,32 @@
             }
             response_code = 400
         case _:
             logging.error(
                 "[/restore]: deleted_files.restore_file function returned unexpected data: '%s'",
                 result
             )
-            return SERVER_ERROR()
+            return flask.abort(500)
                 
     return flask.make_response(response, response_code)
 
 
 @APP.post("/api/files/list-deleted")
-@APP.post('/list-deleted')
 def list_deleted():
-    global database
+    database = g.db
 
     if not request.is_json:
         return NOT_JSON_ERROR()
             
     data = request.json
     headers = request.headers
 
-    verify_result = _verify(headers, _api_permission_type='read')
+    with APP.app_context():
+        verify_result = _verify(headers, _api_permission_type='read')
+    
     if verify_result != 0:
         return verify_result
             
     username: str = database.api_keys.get_key_owner(headers.get('Authorization', ""))
     if username == "INVALID_APIKEY":
         username: str = headers.get('syncServer-Username', '')
     
@@ -639,31 +690,32 @@
             }
             response_code = 404
         case _:
             logging.error(
                 "[/list-deleted]: deleted_files.list_deleted function returned unexpected data: '%s'",
                 result
             )
-            return SERVER_ERROR()
+            return flask.abort(500)
             
     return flask.make_response(response, response_code)
 
 
 @APP.post("/api/files/remove-deleted")
-@APP.post('/remove-deleted')
 def remove_deleted():
-    global database
+    database = g.db
 
     if not request.is_json:
         return NOT_JSON_ERROR()
             
     data = request.json
     headers = request.headers
 
-    verify_result = _verify(headers, _api_permission_type='delete')
+    with APP.app_context():
+        verify_result = _verify(headers, _api_permission_type='delete')
+    
     if verify_result != 0:
         return verify_result
             
     username: str = database.api_keys.get_key_owner(headers.get('Authorization', ""))
     if username == "INVALID_APIKEY":
         username: str = headers.get('syncServer-Username', '')
             
@@ -734,31 +786,32 @@
             }
             response_code = 400
         case _:
             logging.error(
                 "[/remove-deleted]: deleted_files.true_delete function returned unexpected data: '%s'",
                 result
             )
-            return SERVER_ERROR()
+            return flask.abort(500)
             
     return flask.make_response(response, response_code)
 
 
 @APP.post("/api/files/read")
-@APP.post('/read')
 def file_reads():
-    global database
+    database = g.db
 
     if not request.is_json:
         return NOT_JSON_ERROR()
             
     data = request.json
     headers = request.headers
 
-    verify_result = _verify(headers, _api_permission_type='read')
+    with APP.app_context():
+        verify_result = _verify(headers, _api_permission_type='read')
+    
     if verify_result != 0:
         return verify_result
             
     username: str = database.api_keys.get_key_owner(headers.get('Authorization', ""))
     if username == "INVALID_APIKEY":
         username: str = headers.get('syncServer-Username', '')
             
@@ -807,31 +860,32 @@
             filename = ''.join(dirs[-1])
             response.headers['Content-Disposition'] = f'attachment; filename={filename}'
         case _:
             logging.error(
                 "[/read]: read_file function returned unexpected data: '%s'",
                 result
             )
-            return SERVER_ERROR()
+            return flask.abort(500)
             
     return response or flask.make_response(flask.jsonify(err_response), response_code)
         
 
 @APP.post("/api/dirs/create")
-@APP.post('/create-dir')
 def dir_creations():
-    global database
+    database = g.db
 
     if not request.is_json:
         return NOT_JSON_ERROR()
             
     data = request.json
     headers = request.headers
 
-    verify_result = _verify(headers, _api_permission_type='create')
+    with APP.app_context():
+        verify_result = _verify(headers, _api_permission_type='create')
+    
     if verify_result != 0:
         return verify_result
             
     username: str = database.api_keys.get_key_owner(headers.get('Authorization', ""))
     if username == "INVALID_APIKEY":
         username: str = headers.get('syncServer-Username', '')
             
@@ -876,31 +930,32 @@
         case 0:
             response = {'success': True}
         case _:
             logging.error(
                 "[/create-dir]: make_dir function returned unexpected data: '%s'",
                 result
             )
-            return SERVER_ERROR()
+            return flask.abort(500)
                 
     return flask.make_response(response, response_code)
 
 
 @APP.post("/api/dirs/remove")
-@APP.post('/remove-dir')
 def dir_deletions():
-    global database
+    database = g.db
 
     if not request.is_json:
         return NOT_JSON_ERROR()
             
     data = request.json
     headers = request.headers
 
-    verify_result = _verify(headers, _api_permission_type='delete')
+    with APP.app_context():
+        verify_result = _verify(headers, _api_permission_type='delete')
+    
     if verify_result != 0:
         return verify_result
             
     username: str = database.api_keys.get_key_owner(headers.get('Authorization', ""))
     if username == "INVALID_APIKEY":
         username: str = headers.get('syncServer-Username', '')
             
@@ -945,31 +1000,32 @@
         case 0:
             response = {'success': True}
         case _:
             logging.error(
                 "[/remove-dir]: remove_dir function returned unexpected data: '%s'",
                 result
             )
-            return SERVER_ERROR()
+            return flask.abort(500)
 
     return flask.make_response(response, response_code)
 
 
 @APP.post("/api/dirs/list")
-@APP.post('/list-dir')
 def dir_listing():
-    global database
+    database = g.db
 
     if not request.is_json:
         return NOT_JSON_ERROR()
             
     data = request.json
     headers = request.headers
 
-    verify_result = _verify(headers, _api_permission_type='read')
+    with APP.app_context():
+        verify_result = _verify(headers, _api_permission_type='read')
+    
     if verify_result != 0:
         return verify_result
             
     username: str = database.api_keys.get_key_owner(headers.get('Authorization', ""))
     if username == "INVALID_APIKEY":
         username: str = headers.get('syncServer-Username', '')
             
@@ -1016,25 +1072,27 @@
                 'success': True
             }
         case _:
             logging.error(
                 "[/list-dir]: list_dir function returned unexpected data: '%s'",
                 result
             )
-            return SERVER_ERROR()
+            return flask.abort(500)
 
     return flask.make_response(flask.jsonify(response), response_code)
 
 
 @APP.get('/api/dirs/get-paths')
 def get_dir_paths():
-    global database
+    database = g.db
     headers = request.headers
 
-    verify_result = _verify(headers, _api_permission_type='read')
+    with APP.app_context():
+        verify_result = _verify(headers, _api_permission_type='read')
+    
     if verify_result != 0:
         return verify_result
             
     username: str = database.api_keys.get_key_owner(headers.get('Authorization', ""))
     if username == "INVALID_APIKEY":
         username: str = headers.get('syncServer-Username', '')
     
@@ -1049,31 +1107,32 @@
                 'dir-paths': result
             }
         case _:
             logging.error(
                 "[/api/dirs/get-paths]: dirs.get_dir_paths returned unexpected data: '%s'",
                 result
             )
-            return SERVER_ERROR()
+            return flask.abort(500)
     
     return flask.make_response(response, response_code)
 
 
 @APP.post("/api/create-key")
-@APP.post('/api/keys/create')
 def create_api_key():
-    global database
+    database = g.db
 
     if not request.is_json:
         return NOT_JSON_ERROR()
             
     data = request.json
     headers = request.headers
     
-    verify_result = _verify(headers, _api_permission_type='create')
+    with APP.app_context():
+        verify_result = _verify(headers, _api_permission_type='create')
+    
     if verify_result != 0:
         return verify_result
             
     username: str = database.api_keys.get_key_owner(headers.get('Authorization', ""))
     if username == "INVALID_APIKEY":
         username: str = headers.get('syncServer-Username', '')
     
@@ -1150,29 +1209,31 @@
                 'api-key': result
             }
         case _:
             logging.error(
                 "[/api/create-key]: api_keys.create_key returned unexpected data: '%s'",
                 result
             )
-            return SERVER_ERROR()
+            return flask.abort(500)
             
     return flask.make_response(response, response_code)
 
 
 @APP.post('/api/keys/delete')
-@APP.post('/api/delete-key')
 def delete_api_key():
+    database = g.db
     if not request.is_json:
         return NOT_JSON_ERROR()
             
     data = request.json
     headers = request.headers
 
-    verify_result = _verify(headers, _api_permission_type='delete')
+    with APP.app_context():
+        verify_result = _verify(headers, _api_permission_type='delete')
+    
     if verify_result != 0:
         return verify_result
             
     username: str = database.api_keys.get_key_owner(headers.get('Authorization', ""))
     if username == "INVALID_APIKEY":
         username: str = headers.get('syncServer-Username', '')
             
@@ -1202,27 +1263,29 @@
         case 0:
             response = {'success': True}
         case _:
             logging.error(
                 "[/api/delete-key]: api_keys.delete_key returned unexpected data: '%s'",
                 result
             )
-            return SERVER_ERROR()
+            return flask.abort(500)
 
     return flask.make_response(response, response_code)
 
 
 @APP.post('/api/keys/list-all')
-@APP.post('/api/list-keys')
 def list_api_keys():
+    database = g.db
+
     if not request.is_json:
         return NOT_JSON_ERROR()
     
     headers = request.headers
-    verify_result = _verify(headers, _api_permission_type='read')
+    with APP.app_context():
+        verify_result = _verify(headers, _api_permission_type='read')
 
     if verify_result != 0:
         return verify_result
             
     username: str = database.api_keys.get_key_owner(headers.get('Authorization', ""))
     if username == "INVALID_APIKEY":
         username: str = headers.get('syncServer-Username', '')
@@ -1238,28 +1301,31 @@
                 'key-names': result
             }
         case _:
             logging.error(
                 "[/api/list-keys]: api_keys.list_keys returned unexpected data: '%s'",
                 result
             )
-            return SERVER_ERROR()
+            return flask.abort(500)
             
     return flask.make_response(response, response_code)
 
 
 @APP.post('/api/keys/get-data')
 def get_key_perms():
+    database = g.db
     if not request.is_json:
         return NOT_JSON_ERROR()
     
     headers = request.headers
     data = request.json
 
-    verify_result = _verify(headers, _api_permission_type='all')
+    with APP.app_context():
+        verify_result = _verify(headers, _api_permission_type='all')
+    
     if verify_result != 0:
         return verify_result
     
     username: str = database.api_keys.get_key_owner(headers.get('Authorization', ""))
     if username == "INVALID_APIKEY":
         username: str = headers.get('syncServer-Username', '')
     
@@ -1311,15 +1377,15 @@
                 'key-data': result
             }
         case _:
             logging.error(
                 "[/api/keys/get-data]: api_keys.%s_get_data returned unexpected data: '%s'",
                 f"{'apikey' if api_key else 'keyname'}", result
             )
-            return SERVER_ERROR()
+            return flask.abort(500)
     
     key_owner: str = database.api_keys.get_key_owner(api_key)
     if api_key and key_owner != username:
         # Prevent using an API key that might not belong to that user
         response: dict = {
             'error': "API key provided is invalid.",
             'ecode': "INVALID_APIKEY"
@@ -1339,33 +1405,16 @@
 
 @APP.get('/')
 @APP.get('/api')
 def api_route():
     return flask.jsonify({'alive': True})
 
 
-def config_app(provided_db: FileDatabase = None) -> flask.Flask:
-    global database
-    if not isinstance(provided_db, FileDatabase):
-        raise TypeError("Provided database is not an instance of _db.FileDatabase")
+def run_simple():
+    _app: flask.Flask = create_app()
+    flask_route_port: int = int(os.environ.get('SYNCSERVER_PORT', 8561))
     
-    logging.basicConfig(
-        level=logging.DEBUG,
-        format='[%(asctime)s] - [%(levelname)s] - %(message)s',
-        datefmt='%Y-%m-%d %H:%M:%S',
-        handlers=[
-            logging.StreamHandler(),
-            logging.FileHandler('app.log')
-        ]
-    )
-    return APP
+    _app.run(debug=False, port=flask_route_port)
 
 
 if __name__ == '__main__':
-    db_password: str = getpass.getpass(
-        "Enter database password [or empty if not protected]: ")
-    database: FileDatabase = FileDatabase(db_password=db_password)
-
-    _app: flask.Flask = config_app(database)
-    flask_route_port: int = int(os.environ.get('SYNCSERVER_PORT', 8561))
-
-    _app.run(debug=False, port=flask_route_port)
+    run_simple()
```

