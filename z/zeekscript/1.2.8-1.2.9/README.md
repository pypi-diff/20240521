# Comparing `tmp/zeekscript-1.2.8.tar.gz` & `tmp/zeekscript-1.2.9-cp312-cp312-musllinux_1_1_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeekscript-1.2.8.tar", last modified: Fri Dec  1 10:29:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

