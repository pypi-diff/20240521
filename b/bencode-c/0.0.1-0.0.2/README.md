# Comparing `tmp/bencode_c-0.0.1.tar.gz` & `tmp/bencode_c-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bencode_c-0.0.1.tar", last modified: Mon May 20 22:37:58 2024, max compression
+gzip compressed data, was "bencode_c-0.0.2.tar", last modified: Mon May 20 22:42:18 2024, max compression
```

## Comparing `bencode_c-0.0.1.tar` & `bencode_c-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:37:58.768165 bencode_c-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 22:37:58.768165 bencode_c-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-20 22:37:52.000000 bencode_c-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-20 22:37:52.000000 bencode_c-0.0.1/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 22:37:58.768165 bencode_c-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-20 22:37:52.000000 bencode_c-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:37:58.764165 bencode_c-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:37:58.764165 bencode_c-0.0.1/src/bencode_c/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 22:37:52.000000 bencode_c-0.0.1/src/bencode_c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-20 22:37:52.000000 bencode_c-0.0.1/src/bencode_c/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-20 22:37:52.000000 bencode_c-0.0.1/src/bencode_c/bencode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:37:58.768165 bencode_c-0.0.1/src/bencode_c.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 22:37:58.000000 bencode_c-0.0.1/src/bencode_c.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 22:37:58.000000 bencode_c-0.0.1/src/bencode_c.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:37:58.000000 bencode_c-0.0.1/src/bencode_c.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-20 22:37:58.000000 bencode_c-0.0.1/src/bencode_c.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 22:37:58.000000 bencode_c-0.0.1/src/bencode_c.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:37:58.768165 bencode_c-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-20 22:37:52.000000 bencode_c-0.0.1/tests/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-20 22:37:52.000000 bencode_c-0.0.1/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-20 22:37:52.000000 bencode_c-0.0.1/tests/test_torrent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:42:18.296928 bencode_c-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 22:42:18.296928 bencode_c-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-20 22:42:15.000000 bencode_c-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-20 22:42:15.000000 bencode_c-0.0.2/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 22:42:18.296928 bencode_c-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-20 22:42:15.000000 bencode_c-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:42:18.292928 bencode_c-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:42:18.292928 bencode_c-0.0.2/src/bencode_c/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 22:42:15.000000 bencode_c-0.0.2/src/bencode_c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-20 22:42:15.000000 bencode_c-0.0.2/src/bencode_c/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-20 22:42:15.000000 bencode_c-0.0.2/src/bencode_c/bencode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:42:18.292928 bencode_c-0.0.2/src/bencode_c.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 22:42:18.000000 bencode_c-0.0.2/src/bencode_c.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 22:42:18.000000 bencode_c-0.0.2/src/bencode_c.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:42:18.000000 bencode_c-0.0.2/src/bencode_c.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-20 22:42:18.000000 bencode_c-0.0.2/src/bencode_c.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 22:42:18.000000 bencode_c-0.0.2/src/bencode_c.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:42:18.292928 bencode_c-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-20 22:42:15.000000 bencode_c-0.0.2/tests/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-20 22:42:15.000000 bencode_c-0.0.2/tests/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-20 22:42:15.000000 bencode_c-0.0.2/tests/test_torrent.py
```

### Comparing `bencode_c-0.0.1/PKG-INFO` & `bencode_c-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bencode-c
-Version: 0.0.1
+Version: 0.0.2
 Summary: A fast and correct bencode serialize/deserialize library
 Author-email: trim21 <trim21me@gmail.com>
 License: MIT
 Keywords: bencode,bittorrent,bit-torrent,serialize,deserialize,p2p
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bencode_c-0.0.1/pyproject.toml` & `bencode_c-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pyproject.toml
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bencode-c"
-version = "0.0.1"
+version = "0.0.2"
 description = "A fast and correct bencode serialize/deserialize library"
 license = { text = "MIT" }
 requires-python = ">=3.8,<4.0"
 authors = [
     { name = "trim21", email = "trim21me@gmail.com" },
 ]
 readme = 'readme.md'
```

### Comparing `bencode_c-0.0.1/src/bencode_c/bencode.c` & `bencode_c-0.0.2/src/bencode_c/bencode.c`

 * *Files identical despite different names*

### Comparing `bencode_c-0.0.1/src/bencode_c.egg-info/PKG-INFO` & `bencode_c-0.0.2/src/bencode_c.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bencode-c
-Version: 0.0.1
+Version: 0.0.2
 Summary: A fast and correct bencode serialize/deserialize library
 Author-email: trim21 <trim21me@gmail.com>
 License: MIT
 Keywords: bencode,bittorrent,bit-torrent,serialize,deserialize,p2p
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bencode_c-0.0.1/tests/test_decode.py` & `bencode_c-0.0.2/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `bencode_c-0.0.1/tests/test_encode.py` & `bencode_c-0.0.2/tests/test_encode.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,21 +79,21 @@
                 {"id": 0, "name": "Colon Salazar"},
                 {"id": 1, "name": "French Mcneil"},
                 {"id": 2, "name": "Carol Martin"},
             ],
             "favoriteFruit": "banana",
         }
     ) == (
-               b"d3:_id24:5973782bdb9a930533b05cb23:agei32e7:balance9"
-               b":$1,446.357:company5:ARTIQ5:email21:logankeller@artiq.c"
-               b"om8:eyeColor5:green13:favoriteFruit6:banana7:friendsld2"
-               b":idi0e4:name13:Colon Salazared2:idi1e4:name13:French Mc"
-               b"neiled2:idi2e4:name12:Carol Martinee6:gender4:male8:isA"
-               b"ctivei1e4:name12:Logan Keller5:phone17:+1 (952) 533-2258e"
-           )
+        b"d3:_id24:5973782bdb9a930533b05cb23:agei32e7:balance9"
+        b":$1,446.357:company5:ARTIQ5:email21:logankeller@artiq.c"
+        b"om8:eyeColor5:green13:favoriteFruit6:banana7:friendsld2"
+        b":idi0e4:name13:Colon Salazared2:idi1e4:name13:French Mc"
+        b"neiled2:idi2e4:name12:Carol Martinee6:gender4:male8:isA"
+        b"ctivei1e4:name12:Logan Keller5:phone17:+1 (952) 533-2258e"
+    )
 
 
 def test_duplicated_type_keys():
     with pytest.raises(BencodeEncodeError):
         bencode({"string_key": 1, b"string_key": 2, "1": 2})
 
 
@@ -112,14 +112,16 @@
         (False, b"i0e"),
         (-3, b"i-3e"),
         (4927586304, b"i4927586304e"),
         ([b"spam", b"eggs"], b"l4:spam4:eggse"),
         ({b"cow": b"moo", b"spam": b"eggs"}, b"d3:cow3:moo4:spam4:eggse"),
         ({b"spam": [b"a", b"b"]}, b"d4:spaml1:a1:bee"),
         ({}, b"de"),
+        ((1, 2), b"li1ei2ee"),
+        ([1, 2], b"li1ei2ee"),
     ],
 )
 def test_basic(raw: Any, expected: bytes):
     assert bencode(raw) == expected
 
 
 def test_overflow():
```

