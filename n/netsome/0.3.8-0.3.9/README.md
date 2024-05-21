# Comparing `tmp/netsome-0.3.8.tar.gz` & `tmp/netsome-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsome-0.3.8.tar", max compression
+gzip compressed data, was "netsome-0.3.9.tar", max compression
```

## Comparing `netsome-0.3.8.tar` & `netsome-0.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1286 2024-04-11 18:59:46.819718 netsome-0.3.8/LICENSE
--rw-r--r--   0        0        0      355 2024-04-15 07:10:06.582777 netsome-0.3.8/README.md
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820411 netsome-0.3.8/netsome/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820647 netsome-0.3.8/netsome/_converters/__init__.py
--rw-r--r--   0        0        0      967 2024-04-27 12:52:19.064834 netsome-0.3.8/netsome/_converters/bgp.py
--rw-r--r--   0        0        0      343 2024-04-20 09:23:59.213195 netsome-0.3.8/netsome/_converters/ipv4.py
--rw-r--r--   0        0        0     1057 2024-04-27 12:48:27.358013 netsome-0.3.8/netsome/constants.py
--rw-r--r--   0        0        0      324 2024-04-30 07:23:29.209737 netsome-0.3.8/netsome/types/__init__.py
--rw-r--r--   0        0        0     2349 2024-05-02 11:03:45.728278 netsome-0.3.8/netsome/types/bgp.py
--rw-r--r--   0        0        0     6303 2024-05-02 11:03:00.066006 netsome-0.3.8/netsome/types/ipv4.py
--rw-r--r--   0        0        0     3212 2024-04-28 18:56:11.702930 netsome-0.3.8/netsome/types/mac.py
--rw-r--r--   0        0        0      906 2024-04-20 09:23:59.215917 netsome-0.3.8/netsome/types/vlans.py
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.824730 netsome-0.3.8/netsome/validators/__init__.py
--rw-r--r--   0        0        0     2016 2024-04-27 12:48:27.359049 netsome-0.3.8/netsome/validators/bgp.py
--rw-r--r--   0        0        0     2112 2024-04-20 09:23:59.217488 netsome-0.3.8/netsome/validators/ipv4.py
--rw-r--r--   0        0        0      512 2024-04-28 18:55:56.209709 netsome-0.3.8/netsome/validators/mac.py
--rw-r--r--   0        0        0      379 2024-04-27 12:48:27.359608 netsome-0.3.8/netsome/validators/vlans.py
--rw-r--r--   0        0        0     1234 2024-05-02 11:04:09.228242 netsome-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 netsome-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1286 2024-04-11 18:59:46.819718 netsome-0.3.9/LICENSE
+-rw-r--r--   0        0        0      355 2024-04-15 07:10:06.582777 netsome-0.3.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820411 netsome-0.3.9/netsome/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820647 netsome-0.3.9/netsome/_converters/__init__.py
+-rw-r--r--   0        0        0      967 2024-04-27 12:52:19.064834 netsome-0.3.9/netsome/_converters/bgp.py
+-rw-r--r--   0        0        0      343 2024-04-20 09:23:59.213195 netsome-0.3.9/netsome/_converters/ipv4.py
+-rw-r--r--   0        0        0     1057 2024-04-27 12:48:27.358013 netsome-0.3.9/netsome/constants.py
+-rw-r--r--   0        0        0      324 2024-04-30 07:23:29.209737 netsome-0.3.9/netsome/types/__init__.py
+-rw-r--r--   0        0        0     2363 2024-05-03 09:31:18.165465 netsome-0.3.9/netsome/types/bgp.py
+-rw-r--r--   0        0        0     6303 2024-05-02 11:03:00.066006 netsome-0.3.9/netsome/types/ipv4.py
+-rw-r--r--   0        0        0     3196 2024-05-03 09:31:57.576176 netsome-0.3.9/netsome/types/mac.py
+-rw-r--r--   0        0        0      972 2024-05-03 09:33:32.460095 netsome-0.3.9/netsome/types/vlans.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.824730 netsome-0.3.9/netsome/validators/__init__.py
+-rw-r--r--   0        0        0     2016 2024-04-27 12:48:27.359049 netsome-0.3.9/netsome/validators/bgp.py
+-rw-r--r--   0        0        0     2112 2024-04-20 09:23:59.217488 netsome-0.3.9/netsome/validators/ipv4.py
+-rw-r--r--   0        0        0      512 2024-04-28 18:55:56.209709 netsome-0.3.9/netsome/validators/mac.py
+-rw-r--r--   0        0        0      379 2024-04-27 12:48:27.359608 netsome-0.3.9/netsome/validators/vlans.py
+-rw-r--r--   0        0        0     1234 2024-05-03 09:33:56.417004 netsome-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 netsome-0.3.9/PKG-INFO
```

### Comparing `netsome-0.3.8/LICENSE` & `netsome-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netsome-0.3.8/netsome/_converters/bgp.py` & `netsome-0.3.9/netsome/_converters/bgp.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.8/netsome/constants.py` & `netsome-0.3.9/netsome/constants.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.8/netsome/types/bgp.py` & `netsome-0.3.9/netsome/types/bgp.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     ORDER_MAX = c.BGP.ASN_ORDER_MAX
 
     def __init__(self, number: int) -> None:
         valids.validate_asplain(number)
         self._number = number
 
     @property
-    def number(self):
+    def number(self) -> int:
         return self._number
 
     @classmethod
     def from_asdot(cls, string: str) -> "ASN":
         valids.validate_asdot(string)
         return cls(convs.asdot_to_asplain(string))
 
@@ -60,15 +60,15 @@
 
 class Community:
     def __init__(self, number: int) -> None:
         valids.validate_asplain(number)
         self._number = number
 
     @property
-    def number(self):
+    def number(self) -> int:
         return self._number
 
     @classmethod
     def from_str(cls, value: str) -> "Community":
         valids.validate_community(value)
         return cls(convs.community_to_asplain(value))
```

### Comparing `netsome-0.3.8/netsome/types/ipv4.py` & `netsome-0.3.9/netsome/types/ipv4.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.8/netsome/types/mac.py` & `netsome-0.3.9/netsome/types/mac.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,25 +20,25 @@
     OUI_PART_STRING_SIZE = 6
 
     def __init__(self, addr: str) -> None:
         valids.validate_hex_string(addr, self.ADDR_STRING_SIZE)
         self._addr = int(addr, base=c.NUMERALSYSTEMS.HEX)
 
     @functools.cached_property
-    def address(self):
+    def address(self) -> str:
         addr = hex(self._addr)[2:]  # ignore 0x part
         leading_zeros = "0" * (self.ADDR_STRING_SIZE - len(addr))
         return leading_zeros + addr
 
     @functools.cached_property
-    def oui(self):
+    def oui(self) -> str:
         return self.address[: self.OUI_PART_STRING_SIZE]
 
     @functools.cached_property
-    def nic(self):
+    def nic(self) -> str:
         return self.address[self.OUI_PART_STRING_SIZE :]
 
     def is_multicast(self) -> bool:
         # TODO: 40 to const, calculate from cls consts
         return bool(self._addr & 1 << 40)
 
     def is_unicast(self) -> bool:
@@ -72,15 +72,14 @@
     @classmethod
     def parse(cls, addr: str | int) -> "MacAddress":
         # TODO: can collect all this from cls attrs?
         from_fmts = (
             cls.from_dashed,
             cls.from_coloned,
             cls.from_dotted,
-            # cls.from_bit_reversed,
             cls.from_int,
         )
 
         for fmt in from_fmts:
             with contextlib.suppress(Exception):
                 return fmt(addr)
```

### Comparing `netsome-0.3.8/netsome/types/vlans.py` & `netsome-0.3.9/netsome/types/vlans.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 
     RESERVED = {MIN, DEFAULT, MAX}
 
     def __init__(self, vid: int) -> None:
         valids.validate_vid(vid)
         self._vid = vid
 
+    @property
+    def vid(self) -> int:
+        return self._vid
+
     def __eq__(self, other: t.Any) -> bool:
         return isinstance(other, self.__class__) and (self._vid == other._vid)
 
     def __lt__(self, other: t.Any) -> bool:
         return isinstance(other, self.__class__) and (self._vid < other._vid)
 
     def __hash__(self) -> int:
```

### Comparing `netsome-0.3.8/netsome/validators/bgp.py` & `netsome-0.3.9/netsome/validators/bgp.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.8/netsome/validators/ipv4.py` & `netsome-0.3.9/netsome/validators/ipv4.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.8/netsome/validators/mac.py` & `netsome-0.3.9/netsome/validators/mac.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.8/pyproject.toml` & `netsome-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ]
 description = "The one and only library to make your network code handsome"
 keywords = ["library", "network"]
 license = "X11 License Distribution Modification Variant"
 name = "netsome"
 readme = "README.md"
 repository = "https://github.com/kuderr/netsome"
-version = "0.3.8"
+version = "0.3.9"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 poethepoet = "^0.25.0"
 pytest = "^8.1.1"
```

### Comparing `netsome-0.3.8/PKG-INFO` & `netsome-0.3.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsome
-Version: 0.3.8
+Version: 0.3.9
 Summary: The one and only library to make your network code handsome
 Home-page: https://github.com/kuderr/netsome
 License: X11-distribute-modifications-variant
 Keywords: library,network
 Author: kuderr
 Author-email: dakudryavcev@gmail.com
 Requires-Python: >=3.10,<4.0
```

