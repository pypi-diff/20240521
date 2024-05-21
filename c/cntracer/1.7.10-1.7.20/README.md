# Comparing `tmp/cntracer-1.7.10-cp39-cp39-win_amd64.whl.zip` & `tmp/cntracer-1.7.20-cp310-cp310-musllinux_1_1_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,12 @@
-Zip file size: 115659 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   342016 b- defN 24-Apr-11 05:16 cntracer.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2182 b- defN 24-Apr-11 05:16 cntracer-1.7.10.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      234 b- defN 24-Apr-11 05:16 cntracer-1.7.10.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-11 05:16 cntracer-1.7.10.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-11 05:16 cntracer-1.7.10.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      481 b- defN 24-Apr-11 05:16 cntracer-1.7.10.dist-info/RECORD
-6 files, 345022 bytes uncompressed, 114789 bytes compressed:  66.7%
+Zip file size: 660692 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 02:26 cntracer-1.7.20.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 02:26 cntracer.libs/
+-rwxr-xr-x  2.0 unx   533865 b- defN 24-May-21 02:26 cntracer.cpython-310-aarch64-linux-gnu.so
+-rw-r--r--  2.0 unx      223 b- defN 24-May-21 02:26 cntracer-1.7.20.dist-info/METADATA
+-rw-r--r--  2.0 unx     2182 b- defN 24-May-21 02:26 cntracer-1.7.20.dist-info/LICENSE
+-rw-r--r--  2.0 unx      114 b- defN 24-May-21 02:26 cntracer-1.7.20.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-May-21 02:26 cntracer-1.7.20.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      700 b- defN 24-May-21 02:26 cntracer-1.7.20.dist-info/RECORD
+-rwxr-xr-x  2.0 unx  2599041 b- defN 24-May-21 02:26 cntracer.libs/libstdc++-fd9f4683.so.6.0.28
+-rw-r--r--  2.0 unx   134393 b- defN 24-May-21 02:26 cntracer.libs/libgcc_s-4e37474d.so.1
+10 files, 3270527 bytes uncompressed, 659254 bytes compressed:  79.9%
```

## zipnote {}

```diff
@@ -1,19 +1,31 @@
-Filename: cntracer.cp39-win_amd64.pyd
+Filename: cntracer-1.7.20.dist-info/
 Comment: 
 
-Filename: cntracer-1.7.10.dist-info/LICENSE
+Filename: cntracer.libs/
 Comment: 
 
-Filename: cntracer-1.7.10.dist-info/METADATA
+Filename: cntracer.cpython-310-aarch64-linux-gnu.so
 Comment: 
 
-Filename: cntracer-1.7.10.dist-info/WHEEL
+Filename: cntracer-1.7.20.dist-info/METADATA
 Comment: 
 
-Filename: cntracer-1.7.10.dist-info/top_level.txt
+Filename: cntracer-1.7.20.dist-info/LICENSE
 Comment: 
 
-Filename: cntracer-1.7.10.dist-info/RECORD
+Filename: cntracer-1.7.20.dist-info/WHEEL
+Comment: 
+
+Filename: cntracer-1.7.20.dist-info/top_level.txt
+Comment: 
+
+Filename: cntracer-1.7.20.dist-info/RECORD
+Comment: 
+
+Filename: cntracer.libs/libstdc++-fd9f4683.so.6.0.28
+Comment: 
+
+Filename: cntracer.libs/libgcc_s-4e37474d.so.1
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `cntracer-1.7.10.dist-info/LICENSE` & `cntracer-1.7.20.dist-info/LICENSE`

 * *Files identical despite different names*

