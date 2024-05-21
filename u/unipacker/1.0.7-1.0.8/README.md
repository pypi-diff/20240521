# Comparing `tmp/unipacker-1.0.7-py3-none-any.whl.zip` & `tmp/unipacker-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 3729923 bytes, number of entries: 28
--rw-rw-r--  2.0 unx       22 b- defN 24-Jan-30 13:51 unipacker/__init__.py
+Zip file size: 3729925 bytes, number of entries: 28
+-rw-rw-r--  2.0 unx       22 b- defN 24-May-21 15:46 unipacker/__init__.py
 -rw-rw-r--  2.0 unx    18693 b- defN 24-Jan-30 13:51 unipacker/apicalls.py
 -rw-rw-r--  2.0 unx      381 b- defN 24-Jan-30 13:51 unipacker/banner
--rw-rw-r--  2.0 unx    22616 b- defN 24-Jan-30 13:51 unipacker/core.py
+-rw-rw-r--  2.0 unx    22623 b- defN 24-May-21 15:40 unipacker/core.py
 -rw-rw-r--  2.0 unx     8458 b- defN 24-Jan-30 13:51 unipacker/fortunes
 -rw-rw-r--  2.0 unx    24572 b- defN 24-Jan-30 13:51 unipacker/headers.py
 -rw-rw-r--  2.0 unx    22429 b- defN 24-Jan-30 13:51 unipacker/imagedump.py
 -rw-rw-r--  2.0 unx     1341 b- defN 24-Jan-30 13:51 unipacker/io_handler.py
 -rw-rw-r--  2.0 unx     1960 b- defN 24-Jan-30 13:51 unipacker/kernel_structs.py
 -rw-rw-r--  2.0 unx     4745 b- defN 24-Jan-30 13:51 unipacker/malwrsig.yar
 -rw-rw-r--  2.0 unx     3106 b- defN 24-Jan-30 13:51 unipacker/packer_signatures.yar
@@ -16,15 +16,15 @@
 -rw-rw-r--  2.0 unx     9135 b- defN 24-Jan-30 13:51 unipacker/utils.py
 -rwxrwxr-x  2.0 unx  1981280 b- defN 24-Jan-30 13:51 unipacker/DLLs/KernelBase.dll
 -rw-rw-r--  2.0 unx  1980416 b- defN 24-Jan-30 13:51 unipacker/DLLs/KernelBase.ldll
 -rwxrwxr-x  2.0 unx   607744 b- defN 24-Jan-30 13:51 unipacker/DLLs/kernel32.dll
 -rw-rw-r--  2.0 unx   872448 b- defN 24-Jan-30 13:51 unipacker/DLLs/kernel32.ldll
 -rwxrwxr-x  2.0 unx  1620264 b- defN 24-Jan-30 13:51 unipacker/DLLs/ntdll.dll
 -rw-rw-r--  2.0 unx  1638400 b- defN 24-Jan-30 13:51 unipacker/DLLs/ntdll.ldll
--rw-rw-r--  2.0 unx    18092 b- defN 24-Jan-30 14:19 unipacker-1.0.7.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6840 b- defN 24-Jan-30 14:19 unipacker-1.0.7.dist-info/METADATA
--rw-rw-r--  2.0 unx      111 b- defN 24-Jan-30 14:19 unipacker-1.0.7.dist-info/NOTICE
--rw-rw-r--  2.0 unx       92 b- defN 24-Jan-30 14:19 unipacker-1.0.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       51 b- defN 24-Jan-30 14:19 unipacker-1.0.7.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 24-Jan-30 14:19 unipacker-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2280 b- defN 24-Jan-30 14:19 unipacker-1.0.7.dist-info/RECORD
-28 files, 8897160 bytes uncompressed, 3726323 bytes compressed:  58.1%
+-rw-rw-r--  2.0 unx    18092 b- defN 24-May-21 15:48 unipacker-1.0.8.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6840 b- defN 24-May-21 15:48 unipacker-1.0.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx      111 b- defN 24-May-21 15:48 unipacker-1.0.8.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-21 15:48 unipacker-1.0.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       51 b- defN 24-May-21 15:48 unipacker-1.0.8.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 24-May-21 15:48 unipacker-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2280 b- defN 24-May-21 15:48 unipacker-1.0.8.dist-info/RECORD
+28 files, 8897167 bytes uncompressed, 3726325 bytes compressed:  58.1%
```

## zipnote {}

```diff
@@ -57,29 +57,29 @@
 
 Filename: unipacker/DLLs/ntdll.dll
 Comment: 
 
 Filename: unipacker/DLLs/ntdll.ldll
 Comment: 
 
-Filename: unipacker-1.0.7.dist-info/LICENSE
+Filename: unipacker-1.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: unipacker-1.0.7.dist-info/METADATA
+Filename: unipacker-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: unipacker-1.0.7.dist-info/NOTICE
+Filename: unipacker-1.0.8.dist-info/NOTICE
 Comment: 
 
-Filename: unipacker-1.0.7.dist-info/WHEEL
+Filename: unipacker-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: unipacker-1.0.7.dist-info/entry_points.txt
+Filename: unipacker-1.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: unipacker-1.0.7.dist-info/top_level.txt
+Filename: unipacker-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: unipacker-1.0.7.dist-info/RECORD
+Filename: unipacker-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## unipacker/__init__.py

```diff
@@ -1 +1 @@
-__VERSION__ = "1.0.7"
+__VERSION__ = "1.0.8"
```

## unipacker/core.py

```diff
@@ -434,15 +434,15 @@
         self.sample.unpacker.secs.append(SectionHeader(stack_sec_header))
         self.HOOK_ADDR = STACK_START + 0x3000 + 0x1000
 
         # Start unicorn emulator with x86-32bit architecture
         self.uc = Uc(UC_ARCH_X86, UC_MODE_32)
         if self.sample.unpacker.startaddr is None:
             self.sample.unpacker.startaddr = self.entrypoint(pe)
-        self.sample.loaded_image = pe.get_memory_mapped_image(ImageBase=self.sample.BASE_ADDR)
+        self.sample.loaded_image = bytes(pe.get_memory_mapped_image(ImageBase=self.sample.BASE_ADDR))
         self.sample.virtualmemorysize = align(self.sample.virtualmemorysize + 0x10000,
                                               page_size=4096)  # Space possible IAT rebuilding
         self.sample.unpacker.virtualmemorysize = self.sample.virtualmemorysize
         self.uc.mem_map(self.sample.BASE_ADDR, self.sample.virtualmemorysize)
         self.uc.mem_write(self.sample.BASE_ADDR, self.sample.loaded_image)
 
         self.setup_processinfo()
```

## Comparing `unipacker-1.0.7.dist-info/LICENSE` & `unipacker-1.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `unipacker-1.0.7.dist-info/METADATA` & `unipacker-1.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unipacker
-Version: 1.0.7
+Version: 1.0.8
 Summary: Automatic and platform-independent unpacker for Windows binaries based on emulation
 Home-page: https://github.com/unipacker/unipacker
 Author: Un{i}packer Team
 Author-email: masrepus97@gmail.com
 License: GPL-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

## Comparing `unipacker-1.0.7.dist-info/RECORD` & `unipacker-1.0.8.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-unipacker/__init__.py,sha256=mog5EUIDEeAFCqBo_i4PTmcQrgHzbviDc6G7nEzdeAc,22
+unipacker/__init__.py,sha256=ufFUzigj1g0_KLcf115HW4wQZpnWBtmr7RXsPQFoEoQ,22
 unipacker/apicalls.py,sha256=oOMpU_7lq7TYhzeq9fygnlEIx87s8hVIgj_LeHoVWO8,18693
 unipacker/banner,sha256=MAXro242v5D363ZQriRm_rRjRY5DgoxSGy5GFy8AtUY,381
-unipacker/core.py,sha256=y03Jm6JvdAkLmFaYCoNPdch1D6r1CDTM-G04VmBLUyU,22616
+unipacker/core.py,sha256=aMGrN7X4pMv1JJTlmckhrV55X2xMAdRPYrjxM1m-_E0,22623
 unipacker/fortunes,sha256=wyoZe5eVPGlnZBhT4hrPbT4Cb_RpWY1QDFxcCzFo7nk,8458
 unipacker/headers.py,sha256=NbcUjsgpA1RG_LyPPblSdy5O8FDKli6Q_jIM9dIcZhQ,24572
 unipacker/imagedump.py,sha256=m0b0ZIG_B5AAxiEDk275YfvrnrAr6ihMzvfFFZDbeD4,22429
 unipacker/io_handler.py,sha256=weTHAkjBYu7HrEMCtApMPFRJpxUChw1ApU0THQelUms,1341
 unipacker/kernel_structs.py,sha256=He1yXXbvdLmpq8IhPIwcxoUJpAcgkzve4uBDaHfcQ8w,1960
 unipacker/malwrsig.yar,sha256=C5wnPv_y6oBuPcHzwNM492sKXwv1DPoLFdidGShvHKM,4745
 unipacker/packer_signatures.yar,sha256=97oLuGKlYHvY54dYG9S8CQUKVJtSPfWCN6EDX6-Ii4Y,3106
@@ -15,14 +15,14 @@
 unipacker/utils.py,sha256=mc0EBIDIFg6ukU0FKNmwBzN4c1M0ZyINTgYqeygSp7k,9135
 unipacker/DLLs/KernelBase.dll,sha256=nygEdXaB91xZeCOKKU2OvHPOMvImgl-bMy-OLtA4RCc,1981280
 unipacker/DLLs/KernelBase.ldll,sha256=W2MxGHdE-Uws4SMbFm3GzLhrcR1ZPrJMNlWUAL8X9LU,1980416
 unipacker/DLLs/kernel32.dll,sha256=z2pdrS-KvMHsaMUnQ5U2x1Z7Sp_rtuAIqqu9as-0abc,607744
 unipacker/DLLs/kernel32.ldll,sha256=zMvRQKvN8cosyRzaQ0xSdIwijtAzvu52z0a0fsl0gek,872448
 unipacker/DLLs/ntdll.dll,sha256=uCG2rmf2JYcye2UmX-FFhIthiUEUpbA_8XeaWBuhb1c,1620264
 unipacker/DLLs/ntdll.ldll,sha256=WUay8JHANPqdnI4EVuE5HHmbLQfJ0D94je1EEfuCg18,1638400
-unipacker-1.0.7.dist-info/LICENSE,sha256=gXf5dRMhNSbfLPYYTY_5hsZ1r7UU1OaKQEAQUhuIBkM,18092
-unipacker-1.0.7.dist-info/METADATA,sha256=oSI5lRLReavisgn4nh2I4PV977qYUQPYD_CvcE9KhV4,6840
-unipacker-1.0.7.dist-info/NOTICE,sha256=mjMcv2-3ZrD6wYVNVO4Xf2U_qBqGlKPpEWGcR4Rk0A8,111
-unipacker-1.0.7.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-unipacker-1.0.7.dist-info/entry_points.txt,sha256=vo5S_AzZosmZqX1MW2QrnsrHSUjxwy6DQ0GvQxAwxl4,51
-unipacker-1.0.7.dist-info/top_level.txt,sha256=nZ0NWBWe-6oWXhFVEA2DGzrUqh90U_Vatb0zuGnO4Mk,10
-unipacker-1.0.7.dist-info/RECORD,,
+unipacker-1.0.8.dist-info/LICENSE,sha256=gXf5dRMhNSbfLPYYTY_5hsZ1r7UU1OaKQEAQUhuIBkM,18092
+unipacker-1.0.8.dist-info/METADATA,sha256=D4S6kUAZxRRW4aH-qNATGCf8TzDiTCz20ahN-GckppM,6840
+unipacker-1.0.8.dist-info/NOTICE,sha256=mjMcv2-3ZrD6wYVNVO4Xf2U_qBqGlKPpEWGcR4Rk0A8,111
+unipacker-1.0.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+unipacker-1.0.8.dist-info/entry_points.txt,sha256=vo5S_AzZosmZqX1MW2QrnsrHSUjxwy6DQ0GvQxAwxl4,51
+unipacker-1.0.8.dist-info/top_level.txt,sha256=nZ0NWBWe-6oWXhFVEA2DGzrUqh90U_Vatb0zuGnO4Mk,10
+unipacker-1.0.8.dist-info/RECORD,,
```

