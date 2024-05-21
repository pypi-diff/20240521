# Comparing `tmp/calculate_savings-0.0.7.tar.gz` & `tmp/calculate_savings-0.0.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculate_savings-0.0.7.tar", last modified: Tue May 21 11:27:16 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

