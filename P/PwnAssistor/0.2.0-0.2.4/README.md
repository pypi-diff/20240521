# Comparing `tmp/PwnAssistor-0.2.0.tar.gz` & `tmp/pwnassistor-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PwnAssistor-0.2.0.tar", last modified: Mon Nov  6 06:51:38 2023, max compression
+gzip compressed data, was "pwnassistor-0.2.4.tar", last modified: Tue May 21 17:07:00 2024, max compression
```

## Comparing `PwnAssistor-0.2.0.tar` & `pwnassistor-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 06:51:38.613234 PwnAssistor-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-06 06:51:23.000000 PwnAssistor-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2023-11-06 06:51:38.609234 PwnAssistor-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 06:51:38.609234 PwnAssistor-0.2.0/PwnAssistor/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-06 06:51:23.000000 PwnAssistor-0.2.0/PwnAssistor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 06:51:38.609234 PwnAssistor-0.2.0/PwnAssistor/attacker/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-11-06 06:51:23.000000 PwnAssistor-0.2.0/PwnAssistor/attacker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2023-11-06 06:51:23.000000 PwnAssistor-0.2.0/PwnAssistor/attacker/fmt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2023-11-06 06:51:23.000000 PwnAssistor-0.2.0/PwnAssistor/attacker/gadget.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-11-06 06:51:23.000000 PwnAssistor-0.2.0/PwnAssistor/attacker/heap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2023-11-06 06:51:23.000000 PwnAssistor-0.2.0/PwnAssistor/attacker/io.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-11-06 06:51:23.000000 PwnAssistor-0.2.0/PwnAssistor/attacker/pwnvar.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 06:51:23.000000 PwnAssistor-0.2.0/PwnAssistor/attacker/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 06:51:38.609234 PwnAssistor-0.2.0/PwnAssistor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2023-11-06 06:51:38.000000 PwnAssistor-0.2.0/PwnAssistor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2023-11-06 06:51:38.000000 PwnAssistor-0.2.0/PwnAssistor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 06:51:38.000000 PwnAssistor-0.2.0/PwnAssistor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-06 06:51:38.000000 PwnAssistor-0.2.0/PwnAssistor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-11-06 06:51:23.000000 PwnAssistor-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-06 06:51:38.613234 PwnAssistor-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-11-06 06:51:23.000000 PwnAssistor-0.2.0/setup.py
+drwxr-xr-x   0 nemo      (1000) nemo      (1000)        0 2024-05-21 17:07:00.822105 pwnassistor-0.2.4/
+-rw-r--r--   0 nemo      (1000) nemo      (1000)     1064 2023-08-08 05:16:12.000000 pwnassistor-0.2.4/LICENSE
+-rw-r--r--   0 nemo      (1000) nemo      (1000)     1235 2024-05-21 17:07:00.821105 pwnassistor-0.2.4/PKG-INFO
+drwxr-xr-x   0 nemo      (1000) nemo      (1000)        0 2024-05-21 17:07:00.813105 pwnassistor-0.2.4/PwnAssistor/
+-rw-r--r--   0 nemo      (1000) nemo      (1000)       28 2023-08-08 09:00:05.000000 pwnassistor-0.2.4/PwnAssistor/__init__.py
+drwxr-xr-x   0 nemo      (1000) nemo      (1000)        0 2024-05-21 17:07:00.819105 pwnassistor-0.2.4/PwnAssistor/attacker/
+-rw-r--r--   0 nemo      (1000) nemo      (1000)       86 2023-08-23 01:45:31.000000 pwnassistor-0.2.4/PwnAssistor/attacker/__init__.py
+-rw-r--r--   0 nemo      (1000) nemo      (1000)     5083 2023-10-10 08:16:14.000000 pwnassistor-0.2.4/PwnAssistor/attacker/fmt.py
+-rw-r--r--   0 nemo      (1000) nemo      (1000)     1278 2023-10-10 04:18:49.000000 pwnassistor-0.2.4/PwnAssistor/attacker/gadget.py
+-rw-r--r--   0 nemo      (1000) nemo      (1000)      502 2024-05-21 16:45:53.000000 pwnassistor-0.2.4/PwnAssistor/attacker/heap.py
+-rw-r--r--   0 nemo      (1000) nemo      (1000)     6395 2024-05-21 17:04:04.000000 pwnassistor-0.2.4/PwnAssistor/attacker/io.py
+-rw-r--r--   0 nemo      (1000) nemo      (1000)       42 2023-08-08 11:19:59.000000 pwnassistor-0.2.4/PwnAssistor/attacker/pwnvar.py
+-rw-r--r--   0 nemo      (1000) nemo      (1000)        0 2023-08-23 02:11:19.000000 pwnassistor-0.2.4/PwnAssistor/attacker/stack.py
+drwxr-xr-x   0 nemo      (1000) nemo      (1000)        0 2024-05-21 17:07:00.820105 pwnassistor-0.2.4/PwnAssistor.egg-info/
+-rw-r--r--   0 nemo      (1000) nemo      (1000)     1235 2024-05-21 17:07:00.000000 pwnassistor-0.2.4/PwnAssistor.egg-info/PKG-INFO
+-rw-r--r--   0 nemo      (1000) nemo      (1000)      399 2024-05-21 17:07:00.000000 pwnassistor-0.2.4/PwnAssistor.egg-info/SOURCES.txt
+-rw-r--r--   0 nemo      (1000) nemo      (1000)        1 2024-05-21 17:07:00.000000 pwnassistor-0.2.4/PwnAssistor.egg-info/dependency_links.txt
+-rw-r--r--   0 nemo      (1000) nemo      (1000)       12 2024-05-21 17:07:00.000000 pwnassistor-0.2.4/PwnAssistor.egg-info/top_level.txt
+-rw-r--r--   0 nemo      (1000) nemo      (1000)      900 2023-11-12 06:23:51.000000 pwnassistor-0.2.4/README.md
+-rw-r--r--   0 nemo      (1000) nemo      (1000)       38 2024-05-21 17:07:00.822105 pwnassistor-0.2.4/setup.cfg
+-rw-r--r--   0 nemo      (1000) nemo      (1000)      495 2024-05-21 17:04:10.000000 pwnassistor-0.2.4/setup.py
```

### Comparing `PwnAssistor-0.2.0/LICENSE` & `pwnassistor-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PwnAssistor-0.2.0/PKG-INFO` & `pwnassistor-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PwnAssistor
-Version: 0.2.0
+Version: 0.2.4
 Summary: Atool for pwn
 Author: V3rdant
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires: pwntools
```

### Comparing `PwnAssistor-0.2.0/PwnAssistor/attacker/fmt.py` & `pwnassistor-0.2.4/PwnAssistor/attacker/fmt.py`

 * *Files identical despite different names*

### Comparing `PwnAssistor-0.2.0/PwnAssistor/attacker/gadget.py` & `pwnassistor-0.2.4/PwnAssistor/attacker/gadget.py`

 * *Files identical despite different names*

### Comparing `PwnAssistor-0.2.0/PwnAssistor/attacker/io.py` & `pwnassistor-0.2.4/PwnAssistor/attacker/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,17 @@
                 0x40: rop_payload
             }
         },
         filler='\x00'
     )
     return payload
 
+def house_of_lys_orw_by_shellcode(target_addr: int):
+    pass
+
 
 def get_IO_obstack_jumps():
     for i in pwnvar.pwnlibc.sections:
         if i.name == "__libc_IO_vtables":
             mem = pwnvar.pwnlibc.mmap
             pos = i.header.sh_offset
             with mem:
```

### Comparing `PwnAssistor-0.2.0/PwnAssistor.egg-info/PKG-INFO` & `pwnassistor-0.2.4/PwnAssistor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PwnAssistor
-Version: 0.2.0
+Version: 0.2.4
 Summary: Atool for pwn
 Author: V3rdant
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires: pwntools
```

### Comparing `PwnAssistor-0.2.0/README.md` & `pwnassistor-0.2.4/README.md`

 * *Files identical despite different names*

