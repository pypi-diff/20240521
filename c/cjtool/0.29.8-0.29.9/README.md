# Comparing `tmp/cjtool-0.29.8-py2.py3-none-any.whl.zip` & `tmp/cjtool-0.29.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 21832 bytes, number of entries: 19
+Zip file size: 22217 bytes, number of entries: 19
 -rw-rw-rw-  2.0 fat       76 b- defN 22-Oct-06 08:53 cjtool/__init__.py
 -rw-rw-rw-  2.0 fat      404 b- defN 24-May-13 08:53 cjtool/addconsole.py
 -rw-rw-rw-  2.0 fat     3501 b- defN 24-May-12 10:07 cjtool/cdbtool.py
--rw-rw-rw-  2.0 fat    12182 b- defN 24-May-13 08:51 cjtool/common.py
+-rw-rw-rw-  2.0 fat    12171 b- defN 24-May-18 06:26 cjtool/common.py
 -rw-rw-rw-  2.0 fat    15195 b- defN 24-May-12 10:07 cjtool/debuger.py
 -rw-rw-rw-  2.0 fat     1938 b- defN 24-May-12 10:07 cjtool/indent.py
 -rw-rw-rw-  2.0 fat     2408 b- defN 24-May-12 10:07 cjtool/monitor.py
 -rw-rw-rw-  2.0 fat     2044 b- defN 24-May-13 08:51 cjtool/search.py
 -rw-rw-rw-  2.0 fat     5826 b- defN 22-Oct-06 08:27 cjtool/stl.py
 -rw-rw-rw-  2.0 fat     7180 b- defN 22-Oct-04 06:17 cjtool/stringtool.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-12 10:07 cjtool/gfy/__init__.py
--rw-rw-rw-  2.0 fat     2280 b- defN 24-May-13 13:36 cjtool/gfy/edoinfo.py
+-rw-rw-rw-  2.0 fat     3349 b- defN 24-May-19 06:01 cjtool/gfy/edoinfo.py
 -rw-rw-rw-  2.0 fat     2226 b- defN 24-May-12 02:17 cjtool/gfy/print.py
 -rw-rw-rw-  2.0 fat     2309 b- defN 24-May-12 10:07 cjtool/gfy/printedo.py
--rw-rw-rw-  2.0 fat     1935 b- defN 24-May-13 13:37 cjtool-0.29.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 24-May-13 13:37 cjtool-0.29.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      221 b- defN 24-May-13 13:37 cjtool-0.29.8.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        7 b- defN 24-May-13 13:37 cjtool-0.29.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1442 b- defN 24-May-13 13:37 cjtool-0.29.8.dist-info/RECORD
-19 files, 61284 bytes uncompressed, 19522 bytes compressed:  68.1%
+-rw-rw-rw-  2.0 fat     1935 b- defN 24-May-21 02:20 cjtool-0.29.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 24-May-21 02:20 cjtool-0.29.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      221 b- defN 24-May-21 02:20 cjtool-0.29.9.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 24-May-21 02:20 cjtool-0.29.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1442 b- defN 24-May-21 02:20 cjtool-0.29.9.dist-info/RECORD
+19 files, 62342 bytes uncompressed, 19907 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: cjtool/gfy/print.py
 Comment: 
 
 Filename: cjtool/gfy/printedo.py
 Comment: 
 
-Filename: cjtool-0.29.8.dist-info/METADATA
+Filename: cjtool-0.29.9.dist-info/METADATA
 Comment: 
 
-Filename: cjtool-0.29.8.dist-info/WHEEL
+Filename: cjtool-0.29.9.dist-info/WHEEL
 Comment: 
 
-Filename: cjtool-0.29.8.dist-info/entry_points.txt
+Filename: cjtool-0.29.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: cjtool-0.29.8.dist-info/top_level.txt
+Filename: cjtool-0.29.9.dist-info/top_level.txt
 Comment: 
 
-Filename: cjtool-0.29.8.dist-info/RECORD
+Filename: cjtool-0.29.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cjtool/common.py

```diff
@@ -15,15 +15,15 @@
     FAIL = '\033[91m'
     ENDC = '\033[0m'
     BOLD = '\033[1m'
     UNDERLINE = '\033[4m'
 
 
 def print_warning(msg):
-    print("{0}WARNING: {2}{1}".format(bcolors.WARNING, bcolors.ENDC, msg))
+    print(f"{bcolors.WARNING}WARNING: {msg}{bcolors.ENDC}")
 
 
 # cache
 cache_dword_size = None
 
 
 def get_arch():
@@ -330,24 +330,26 @@
     freopen = pykd.typedVar(freopen_Type, pykd.getOffset("ucrtbase!freopen"))
     param = pykd.stackAlloc(100)
     pykd.writeCStr(param, "CON")
     pykd.writeCStr(param + 8, "w")
     freopen(param, param + 8, stdout)
     pykd.stackFree(100)
 
+
 def attach_process(process_name: str):
     pykd.initialize()
     pid = getProcessByName(process_name)
     if pid == 0:
         print(f"The app: {process_name} is not found")
         exit()
 
     print(f"Attaching to process: pid {pid}")
     pykd.attachProcess(pid)
 
+
 def natvis(moduleName, var, depth=1):
     # Need copy the stl.natvis to the site-packages\pykd\Visualizers
     typename = var.type().name()
     addr = var.getAddress()
     desc = pykd.dbgCommand("dx -r{} (*(({}!{} *){:#x}))".format(
         depth, moduleName, typename, addr))
     return desc
```

## cjtool/gfy/edoinfo.py

```diff
@@ -1,27 +1,39 @@
 ﻿import pykd
 from cjtool.stl import *
 from cjtool.common import *
 import pyperclip as pc
 import argparse
+import json
+import time
 
+def print_edo(msg):
+    print(f"{bcolors.OKBLUE}{msg}{bcolors.ENDC}")
+
+def print_shape(msg):
+    print(f"{bcolors.OKGREEN}{msg}{bcolors.ENDC}")
 
 def getEdoInfo(edoId) -> str:
-    stringVar = malloc_wstring("")
+    stringVar = malloc_string("")
     Void = pykd.typeInfo("Void")
     functype = pykd.defineFunction(Void, pykd.callingConvention.NearC)
     functype.append("argret", pykd.baseTypes.VoidPtr)
     functype.append("id", pykd.baseTypes.Int8B)
-    printEdoWPtr = pykd.typedVar("GFCCommon!getEdoW")
+    printEdoPtr = pykd.typedVar("GFCCommon!getEdo")
     pykd.callFunctionByAddr(
-        functype, printEdoWPtr.getAddress(), stringVar.getAddress(), edoId)
-    value = wstring(stringVar.getAddress())
+        functype, printEdoPtr.getAddress(), stringVar.getAddress(), edoId)
+    value = string(stringVar.getAddress())
     return str(value)
 
 
+def getEdoInfoJson(edoId) -> json:
+    jsonStr = getEdoInfo(edoId)
+    return json.loads(jsonStr)
+
+
 def getShape(edoId) -> str:
     stringVar = malloc_string("")
     Void = pykd.typeInfo("Void")
     functype = pykd.defineFunction(Void, pykd.callingConvention.NearC)
     functype.append("argret", pykd.baseTypes.VoidPtr)
     functype.append("id", pykd.baseTypes.Int8B)
     printEdoWPtr = pykd.typedVar("GFCCommon!getShape")
@@ -30,41 +42,55 @@
     value = string(stringVar.getAddress())
     return str(value)
 
 
 def main():
     parser = argparse.ArgumentParser(description="Input the edoid")
     parser.add_argument("edoid", type=int, help="The GFY Edo Id")
+    parser.add_argument("--gfy4", "-4", action="store_true",
+                        help="Set the process to be GFY4")
     args = parser.parse_args()
     edoid = args.edoid
 
+    process_name = "GFY4" if args.gfy4 else "GFYDeepen"
+
     ext = pykd.isWindbgExt()
     try:
         if not ext:
             pykd.initialize()
-            pid = getProcessByName("gfy4.exe")
+            pid = getProcessByName(f"{process_name}.exe")
             if pid == 0:
-                print("The app: {} is not found".format("gfy4.exe"))
+                print(f"The app {process_name}.exe is not found")
                 exit()
 
             pykd.attachProcess(pid)
 
         # 下行的代码，bp不能省去，否则pykd.go就不返回了
-        bp = pykd.setBp(pykd.getOffset('GFY4!GMPMainForm::eventFilter'))
+        bp = pykd.setBp(pykd.getOffset(
+            f'{process_name}!GMPMainForm::eventFilter'))
         ret = pykd.go()
         if ret == pykd.executionStatus.Break:
-            edoInfo = getEdoInfo(edoid)
-            print(edoInfo)
+            edoInfo = getEdoInfoJson(edoid)
+            print(f"{edoInfo['description']} {edoInfo['typeName']}({edoInfo['elementType']}) {edoInfo['subTypeName']}({edoInfo['elementSubType']})\n")
 
-        ret = pykd.go()
-        if ret == pykd.executionStatus.Break:
-            szShape = getShape(edoid)
-            print(szShape)
+            sorted_properties = sorted(edoInfo['properties'], key=lambda x: x['orderNum'])
+            for index, prop in enumerate(sorted_properties):
+                prn = print if prop['publicFlag'] == 1 else print_edo
+                prn(f"{index:02}. {prop['description']}({prop['code']}, {prop['dataType']})\t{prop['value']}")
+
+            szShape = edoInfo["shape"]
+            print_shape(f"\n{szShape}")
             pc.copy(szShape)
 
+            time.sleep(0.1)
+            szBody = edoInfo["body"]
+            if szBody:
+                print_shape(f"\n{szShape}")
+                pc.copy(szBody)
+
     except Exception as errtxt:
         print(errtxt)
     finally:
         if not ext:
             pykd.detachAllProcesses()
```

## Comparing `cjtool-0.29.8.dist-info/METADATA` & `cjtool-0.29.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjtool
-Version: 0.29.8
+Version: 0.29.9
 Summary: Provide some tools in C++ development
 Home-page: http://github.com/Junch/cjtool
 Author: Jun Chen
 Author-email: junc76@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: colorama
```

## Comparing `cjtool-0.29.8.dist-info/RECORD` & `cjtool-0.29.9.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 cjtool/__init__.py,sha256=Lh7NOd9-n-o-7iRw3-RIoQCF_F57zhZQktJjCkSYOgA,76
 cjtool/addconsole.py,sha256=K9sOmpNh0pqSghnqGOyRwgshJAfgfnIcjyqCVcmNs9I,404
 cjtool/cdbtool.py,sha256=gKc-NzgsDwCg6yBHOTmQG4IEC0jRtIK1jEmoIbB2PWw,3501
-cjtool/common.py,sha256=djGMFHGFc8758wQDe9Y8bMlxEsCGZK-Fz2fPBOTRjuo,12182
+cjtool/common.py,sha256=NP9y8QieD5DZYope8sVIGq4FWcClr_F883cKQSZ_fJY,12171
 cjtool/debuger.py,sha256=3V3YkWiKpTlm70TQIoJXRi6tka21AZRmtKXVFwF30Zw,15195
 cjtool/indent.py,sha256=o8nzbYzfXviUn4f7JayUAtCc5o2c_SZp5PTr1MK8sRg,1938
 cjtool/monitor.py,sha256=qE1sLXBOhcI_AgbdbwOzKqTPqLGsyOKLsjkewuPciWE,2408
 cjtool/search.py,sha256=bbz_gpxrlEfDATWv26MbsfN1Pm6yEB-1zoTAZL10kaw,2044
 cjtool/stl.py,sha256=SeNfQubgArMRtByamEIjdn5fuvEKDhhaIeKBeo6cSdM,5826
 cjtool/stringtool.py,sha256=84VYHVPyIPSO51IXxrhDjJdGE-11NJsdCD-EcI7eL0w,7180
 cjtool/gfy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cjtool/gfy/edoinfo.py,sha256=f2-FVzs6INSWm_EOIhtMjSaBK_VRlhS1RQhSvpzcW04,2280
+cjtool/gfy/edoinfo.py,sha256=tjplRM6geyWeTIFldACqRBALEJ8Jl4XYSNHj7UFWdJ8,3349
 cjtool/gfy/print.py,sha256=O5VyI3XC2EXjs-HhR2Dv2kA_uEpfeHoIhIJOYaZkaeI,2226
 cjtool/gfy/printedo.py,sha256=E8a_4GG_PBTEdw_9NGqhZTMXIAQlR5t3P7ilKJ8Dtw4,2309
-cjtool-0.29.8.dist-info/METADATA,sha256=NR-qtlYARNDc98_YvNWzzSgDE_YB2THMjuFtAmAWKjA,1935
-cjtool-0.29.8.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-cjtool-0.29.8.dist-info/entry_points.txt,sha256=AWsqHhznLRvyrE6X5j68-B3xsMz7SRbx6glhSxb36qI,221
-cjtool-0.29.8.dist-info/top_level.txt,sha256=xT9DqEuxuB3mnAq-fVy_mWHaaTT3M-S7J_93pQnE7W8,7
-cjtool-0.29.8.dist-info/RECORD,,
+cjtool-0.29.9.dist-info/METADATA,sha256=RrdwlIJiOqK-kZxU-wilB4qDY4WoGwA6rtQx8ftzrzI,1935
+cjtool-0.29.9.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+cjtool-0.29.9.dist-info/entry_points.txt,sha256=AWsqHhznLRvyrE6X5j68-B3xsMz7SRbx6glhSxb36qI,221
+cjtool-0.29.9.dist-info/top_level.txt,sha256=xT9DqEuxuB3mnAq-fVy_mWHaaTT3M-S7J_93pQnE7W8,7
+cjtool-0.29.9.dist-info/RECORD,,
```

