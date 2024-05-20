# Comparing `tmp/dolomite-base-0.2.2.tar.gz` & `tmp/dolomite_base-0.2.3-cp38-cp38-macosx_13_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolomite-base-0.2.2.tar", last modified: Thu Feb  8 14:43:07 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

