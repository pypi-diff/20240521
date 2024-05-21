# Comparing `tmp/clickhouse-connect-0.7.8.tar.gz` & `tmp/clickhouse_connect-0.7.9-cp312-cp312-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse-connect-0.7.8.tar", last modified: Sun Apr 14 23:04:37 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

