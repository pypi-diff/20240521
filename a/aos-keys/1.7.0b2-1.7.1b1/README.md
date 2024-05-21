# Comparing `tmp/aos_keys-1.7.0b2-py3-none-any.whl.zip` & `tmp/aos_keys-1.7.1b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,19 @@
-Zip file size: 17740 bytes, number of entries: 16
+Zip file size: 18211 bytes, number of entries: 17
 -rw-rw-r--  2.0 unx      117 b- defN 22-Jun-30 08:41 aos_keys/__init__.py
 -rw-rw-r--  2.0 unx     6720 b- defN 24-Feb-02 11:35 aos_keys/actions.py
--rw-rw-r--  2.0 unx    11336 b- defN 24-Feb-02 11:35 aos_keys/certificate_manager.py
+-rw-rw-r--  2.0 unx    11910 b- defN 24-May-20 12:59 aos_keys/certificate_manager.py
 -rw-rw-r--  2.0 unx     3239 b- defN 24-Feb-02 11:35 aos_keys/cloud_api.py
 -rw-rw-r--  2.0 unx     4323 b- defN 24-Feb-02 11:35 aos_keys/common.py
 -rw-rw-r--  2.0 unx     4959 b- defN 24-Mar-05 13:59 aos_keys/crypto_container.py
--rw-rw-r--  2.0 unx     6194 b- defN 24-Mar-08 10:19 aos_keys/key_manager.py
+-rw-rw-r--  2.0 unx     6194 b- defN 24-Mar-19 07:55 aos_keys/key_manager.py
 -rw-rw-r--  2.0 unx     8451 b- defN 24-Feb-02 11:35 aos_keys/main.py
 -rw-rw-r--  2.0 unx     1452 b- defN 22-Sep-23 09:10 aos_keys/files/1rootCA.crt
 -rw-rw-r--  2.0 unx      113 b- defN 22-Jun-30 08:41 aos_keys/files/__init__.py
--rw-rw-r--  2.0 unx     2597 b- defN 24-Mar-08 10:24 aos_keys-1.7.0b2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-08 10:24 aos_keys-1.7.0b2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       48 b- defN 24-Mar-08 10:24 aos_keys-1.7.0b2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 24-Mar-08 10:24 aos_keys-1.7.0b2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-May-23 08:16 aos_keys-1.7.0b2.dist-info/zip-safe
-?rw-rw-r--  2.0 unx     1293 b- defN 24-Mar-08 10:24 aos_keys-1.7.0b2.dist-info/RECORD
-16 files, 50944 bytes uncompressed, 15610 bytes compressed:  69.4%
+-rw-rw-r--  2.0 unx      193 b- defN 24-May-20 09:21 aos_keys/files/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--  2.0 unx     2597 b- defN 24-May-20 12:59 aos_keys-1.7.1b1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-20 12:59 aos_keys-1.7.1b1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       48 b- defN 24-May-20 12:59 aos_keys-1.7.1b1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 24-May-20 12:59 aos_keys-1.7.1b1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-23 08:16 aos_keys-1.7.1b1.dist-info/zip-safe
+?rw-rw-r--  2.0 unx     1400 b- defN 24-May-20 12:59 aos_keys-1.7.1b1.dist-info/RECORD
+17 files, 51818 bytes uncompressed, 15903 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -24,26 +24,29 @@
 
 Filename: aos_keys/files/1rootCA.crt
 Comment: 
 
 Filename: aos_keys/files/__init__.py
 Comment: 
 
-Filename: aos_keys-1.7.0b2.dist-info/METADATA
+Filename: aos_keys/files/__pycache__/__init__.cpython-310.pyc
 Comment: 
 
-Filename: aos_keys-1.7.0b2.dist-info/WHEEL
+Filename: aos_keys-1.7.1b1.dist-info/METADATA
 Comment: 
 
-Filename: aos_keys-1.7.0b2.dist-info/entry_points.txt
+Filename: aos_keys-1.7.1b1.dist-info/WHEEL
 Comment: 
 
-Filename: aos_keys-1.7.0b2.dist-info/top_level.txt
+Filename: aos_keys-1.7.1b1.dist-info/entry_points.txt
 Comment: 
 
-Filename: aos_keys-1.7.0b2.dist-info/zip-safe
+Filename: aos_keys-1.7.1b1.dist-info/top_level.txt
 Comment: 
 
-Filename: aos_keys-1.7.0b2.dist-info/RECORD
+Filename: aos_keys-1.7.1b1.dist-info/zip-safe
+Comment: 
+
+Filename: aos_keys-1.7.1b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aos_keys/certificate_manager.py

```diff
@@ -66,14 +66,24 @@
 
     raise AosKeysError(
         'Failed to install certificate. "update-ca-certificates" package is missing',
         'Install update-ca-certificates with command: sudo apt install ca-certificates',
     )
 
 
+def check_root_certificate_linux() -> bool:
+    home_str = str(Path.home())
+    nssdb_dir = f'{home_str}/.pki/nssdb'
+    if not os.path.exists(nssdb_dir):
+        return False
+    command = ['certutil', '-d', nssdb_dir, '-L']
+    completed_process = subprocess.run(command, capture_output=True, check=False)
+    return completed_process.returncode == 0
+
+
 def install_root_certificate_macos():
     """Install root certificate on current user's Trusted Root CA."""
     with ca_certificate() as server_certificate_path:
         print_message('We are going to add Aos Root certificate as trusted certificate.')
         print_message('The OS will ask your password to proceed with operation.')
         command = [
             'security',
@@ -258,16 +268,22 @@
 
 
 def install_user_certificate_linux(certificate_path: Path):
     """Install client certificate to the Windows Personal store.
 
     Args:
         certificate_path: path to certificate which will be installed.
+
+    Raises:
+        AosKeysError: Failed to install User's certificate.
     """
     print_message('We are going to import your private key and certificate to browsers databases.')
+    if not check_root_certificate_linux():
+        raise AosKeysError('Failed to install certificate:\n Aos root certificate is not installed.')
+
     password_protected_filename = str(certificate_path) + '.pswd'
     add_password_to_pkcs12(str(certificate_path), password_protected_filename, b'1234', None)
 
     firefox_profiles = find_firefox_profile_locations()
     home_str = str(Path.home())
     all_profiles = [f'sql:{home_str}/.pki/nssdb']
     all_profiles.extend(firefox_profiles)
```

## Comparing `aos_keys-1.7.0b2.dist-info/METADATA` & `aos_keys-1.7.1b1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aos-keys
-Version: 1.7.0b2
+Version: 1.7.1b1
 Summary: AosEdge private keys and certificate manager
 Author: EPAM Systems
 Author-email: support@aoscloud.io
 License: Apache License 2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

## Comparing `aos_keys-1.7.0b2.dist-info/RECORD` & `aos_keys-1.7.1b1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 aos_keys/__init__.py,sha256=uvRZHZ9NW2hkD1OdQb_DWAxB-NpqhCYWJyMKF3XP1Xg,117
 aos_keys/actions.py,sha256=fiUcpGgLQ8IBpNzW1zAsXNYJBNf3_kAYPvaSIpkmVIs,6720
-aos_keys/certificate_manager.py,sha256=M2UzrKUF7MXtGKhug84SESmwuqrEDKM-7gN9yxAGm9E,11336
+aos_keys/certificate_manager.py,sha256=kIutQMvP6XL1LuNFZF0gYl_i05RkxBbgDdZwGUFssPY,11910
 aos_keys/cloud_api.py,sha256=OrkbpciDzZXVn592HIWsHQ9GcBkyFRB6Qapi63stzj4,3239
 aos_keys/common.py,sha256=IU6JpwEWXvv-Qz49O0sRjbEKGtx9J-Y8z0nUYqOq-1M,4323
 aos_keys/crypto_container.py,sha256=8EvPQ1Vaom_0GfKn0Dw88AWtfzSeDAdxWrSF07DRmKg,4959
 aos_keys/key_manager.py,sha256=nnPtsFgCCVoXEAHZJ61X23Cn8zfv4R5_UpEZl7-x6GI,6194
 aos_keys/main.py,sha256=v7OLfFPzjj_-1qWTxFZRjgN0BP_WlcDtXE5RNyG2lFg,8451
 aos_keys/files/1rootCA.crt,sha256=F1BzQ7LOEmNEi2Nl-QJ7s8xRIFLxWlFypOtRSwr84Yg,1452
 aos_keys/files/__init__.py,sha256=RugobKGxKbmCthe2-PYP85pYv7Gfzikpl_SQZ0vFfw8,113
-aos_keys-1.7.0b2.dist-info/METADATA,sha256=DKORRYYmUmmEQ3Mr2YMnKA9dSPhTIRksiIQbOz8mhTc,2597
-aos_keys-1.7.0b2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-aos_keys-1.7.0b2.dist-info/entry_points.txt,sha256=sDI5cvPlgS-4UUF6Kc7ke2gk8wYpeyfr8SbVuNQvG-g,48
-aos_keys-1.7.0b2.dist-info/top_level.txt,sha256=IoCBFe4GEf-X3P8RfB0WvObZxCVLDWbTjgIKMaLo1jY,9
-aos_keys-1.7.0b2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-aos_keys-1.7.0b2.dist-info/RECORD,,
+aos_keys/files/__pycache__/__init__.cpython-310.pyc,sha256=0ZlUW8FaqrCna6bwfWzI4OT7kjjn8hH03QAkDJsyY0A,193
+aos_keys-1.7.1b1.dist-info/METADATA,sha256=o4D_mGtlLXbjKqYA3I8nFlqyNw4PmEKWS2K0Y5o1NBs,2597
+aos_keys-1.7.1b1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+aos_keys-1.7.1b1.dist-info/entry_points.txt,sha256=sDI5cvPlgS-4UUF6Kc7ke2gk8wYpeyfr8SbVuNQvG-g,48
+aos_keys-1.7.1b1.dist-info/top_level.txt,sha256=IoCBFe4GEf-X3P8RfB0WvObZxCVLDWbTjgIKMaLo1jY,9
+aos_keys-1.7.1b1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+aos_keys-1.7.1b1.dist-info/RECORD,,
```

