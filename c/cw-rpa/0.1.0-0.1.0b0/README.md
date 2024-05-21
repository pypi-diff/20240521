# Comparing `tmp/cw_rpa-0.1.0-py3-none-any.whl.zip` & `tmp/cw_rpa-0.1.0b0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 8985 bytes, number of entries: 13
--rw-r--r--  2.0 unx       61 b- defN 24-May-07 10:52 cw_rpa/__init__.py
--rw-r--r--  2.0 unx       62 b- defN 24-May-07 10:52 cw_rpa/libraries/__init__.py
--rw-r--r--  2.0 unx      174 b- defN 24-May-07 10:52 cw_rpa/libraries/cloud/__init__.py
--rw-r--r--  2.0 unx     9996 b- defN 24-May-07 10:52 cw_rpa/libraries/cloud/pre_defined_functions.py
--rw-r--r--  2.0 unx       74 b- defN 24-May-07 10:52 cw_rpa/libraries/common/__init__.py
--rw-r--r--  2.0 unx     9914 b- defN 24-May-07 10:52 cw_rpa/libraries/common/common_functions.py
--rw-r--r--  2.0 unx       62 b- defN 24-May-07 10:52 cw_rpa/libraries/device/__init__.py
--rw-r--r--  2.0 unx       87 b- defN 24-May-07 10:52 cw_rpa/libraries/device/execute_powershell_script.py
--rw-rw-rw-  2.0 unx     1074 b- defN 24-May-07 10:53 cw_rpa-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      199 b- defN 24-May-07 10:53 cw_rpa-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-07 10:53 cw_rpa-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-May-07 10:53 cw_rpa-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1116 b- defN 24-May-07 10:53 cw_rpa-0.1.0.dist-info/RECORD
-13 files, 22918 bytes uncompressed, 7083 bytes compressed:  69.1%
+Zip file size: 9010 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       61 b- defN 24-May-21 11:45 cw_rpa/__init__.py
+-rw-r--r--  2.0 unx       62 b- defN 24-May-21 11:45 cw_rpa/libraries/__init__.py
+-rw-r--r--  2.0 unx      174 b- defN 24-May-21 11:45 cw_rpa/libraries/cloud/__init__.py
+-rw-r--r--  2.0 unx     9996 b- defN 24-May-21 11:45 cw_rpa/libraries/cloud/pre_defined_functions.py
+-rw-r--r--  2.0 unx       74 b- defN 24-May-21 11:45 cw_rpa/libraries/common/__init__.py
+-rw-r--r--  2.0 unx     9914 b- defN 24-May-21 11:45 cw_rpa/libraries/common/common_functions.py
+-rw-r--r--  2.0 unx       62 b- defN 24-May-21 11:45 cw_rpa/libraries/device/__init__.py
+-rw-r--r--  2.0 unx       87 b- defN 24-May-21 11:45 cw_rpa/libraries/device/execute_powershell_script.py
+-rw-rw-rw-  2.0 unx     1074 b- defN 24-May-21 11:45 cw_rpa-0.1.0b0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      201 b- defN 24-May-21 11:45 cw_rpa-0.1.0b0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-21 11:45 cw_rpa-0.1.0b0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-May-21 11:45 cw_rpa-0.1.0b0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1126 b- defN 24-May-21 11:45 cw_rpa-0.1.0b0.dist-info/RECORD
+13 files, 22930 bytes uncompressed, 7088 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: cw_rpa/libraries/device/__init__.py
 Comment: 
 
 Filename: cw_rpa/libraries/device/execute_powershell_script.py
 Comment: 
 
-Filename: cw_rpa-0.1.0.dist-info/LICENSE
+Filename: cw_rpa-0.1.0b0.dist-info/LICENSE
 Comment: 
 
-Filename: cw_rpa-0.1.0.dist-info/METADATA
+Filename: cw_rpa-0.1.0b0.dist-info/METADATA
 Comment: 
 
-Filename: cw_rpa-0.1.0.dist-info/WHEEL
+Filename: cw_rpa-0.1.0b0.dist-info/WHEEL
 Comment: 
 
-Filename: cw_rpa-0.1.0.dist-info/top_level.txt
+Filename: cw_rpa-0.1.0b0.dist-info/top_level.txt
 Comment: 
 
-Filename: cw_rpa-0.1.0.dist-info/RECORD
+Filename: cw_rpa-0.1.0b0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cw_rpa-0.1.0.dist-info/LICENSE` & `cw_rpa-0.1.0b0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cw_rpa-0.1.0.dist-info/RECORD` & `cw_rpa-0.1.0b0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 cw_rpa/libraries/__init__.py,sha256=WilrrZVJIhPAqXlr0kjCN-RnLFZqBN-8zqLSVIvKLuQ,62
 cw_rpa/libraries/cloud/__init__.py,sha256=dOtcJwc9ktu5B-L3VWW_e6IXmfgDGAIlU-AFug70_zU,174
 cw_rpa/libraries/cloud/pre_defined_functions.py,sha256=N02BbMXJGO7MqmjhAoJUFDl5OVruzXl6zIYSxy5lXOA,9996
 cw_rpa/libraries/common/__init__.py,sha256=dc9bvhKg2b8JsW0X0zhfR4WQCoiDwXLl1jxYBblq_IE,74
 cw_rpa/libraries/common/common_functions.py,sha256=hsBo5LeQ_rgAg8XbPgFmnv9OqCo0Qg66zh-IAtCtBL0,9914
 cw_rpa/libraries/device/__init__.py,sha256=msCSrRE7wI_1hPOsrg6yJP_fMa2lF8Om93DP4FJnrIU,62
 cw_rpa/libraries/device/execute_powershell_script.py,sha256=bbhMj3XpQga5h7GJnBs1Cb7knNSYhzBLJe83DT8yMkM,87
-cw_rpa-0.1.0.dist-info/LICENSE,sha256=uSjkbZqFg4qLL4jGa9klR5faoQ7dQatDQXG0bpVFAbk,1074
-cw_rpa-0.1.0.dist-info/METADATA,sha256=OeiAk-NpEFcHY_-t3cbeJxAznvgIwjjufWnxkrVNkD0,199
-cw_rpa-0.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-cw_rpa-0.1.0.dist-info/top_level.txt,sha256=eCMQTVi9G0JQTesbEbLv4eeEQZHiGEBnZVWOPriLn3c,7
-cw_rpa-0.1.0.dist-info/RECORD,,
+cw_rpa-0.1.0b0.dist-info/LICENSE,sha256=uSjkbZqFg4qLL4jGa9klR5faoQ7dQatDQXG0bpVFAbk,1074
+cw_rpa-0.1.0b0.dist-info/METADATA,sha256=t7U8RkfhujtCUeUYi4gs3UoSsXiidbWy12eXGAWfoi4,201
+cw_rpa-0.1.0b0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+cw_rpa-0.1.0b0.dist-info/top_level.txt,sha256=eCMQTVi9G0JQTesbEbLv4eeEQZHiGEBnZVWOPriLn3c,7
+cw_rpa-0.1.0b0.dist-info/RECORD,,
```

