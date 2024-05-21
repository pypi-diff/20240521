# Comparing `tmp/pyscal3-3.1.9.tar.gz` & `tmp/pyscal3-3.2.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscal3-3.1.9.tar", last modified: Thu Apr  4 15:34:22 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

