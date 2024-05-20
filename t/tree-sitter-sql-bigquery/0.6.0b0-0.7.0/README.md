# Comparing `tmp/tree-sitter-sql-bigquery-0.6.0b0.tar.gz` & `tmp/tree-sitter-sql-bigquery-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-sitter-sql-bigquery-0.6.0b0.tar", last modified: Sun May 12 10:59:12 2024, max compression
+gzip compressed data, was "tree-sitter-sql-bigquery-0.7.0.tar", last modified: Mon May 20 21:38:40 2024, max compression
```

## Comparing `tree-sitter-sql-bigquery-0.6.0b0.tar` & `tree-sitter-sql-bigquery-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pisces    (1000) pisces    (1000)        0 2024-05-12 10:59:12.247061 tree-sitter-sql-bigquery-0.6.0b0/
--rw-r--r--   0 pisces    (1000) pisces    (1000)     1064 2022-08-14 12:36:03.000000 tree-sitter-sql-bigquery-0.6.0b0/LICENSE
--rw-r--r--   0 pisces    (1000) pisces    (1000)     1502 2024-05-12 10:59:12.247061 tree-sitter-sql-bigquery-0.6.0b0/PKG-INFO
--rw-r--r--   0 pisces    (1000) pisces    (1000)      904 2024-04-07 10:51:56.000000 tree-sitter-sql-bigquery-0.6.0b0/README.md
-drwxr-xr-x   0 pisces    (1000) pisces    (1000)        0 2024-05-12 10:59:12.227060 tree-sitter-sql-bigquery-0.6.0b0/bindings/
-drwxr-xr-x   0 pisces    (1000) pisces    (1000)        0 2024-05-12 10:59:12.227060 tree-sitter-sql-bigquery-0.6.0b0/bindings/python/
-drwxr-xr-x   0 pisces    (1000) pisces    (1000)        0 2024-05-12 10:59:12.227060 tree-sitter-sql-bigquery-0.6.0b0/bindings/python/tree_sitter_sql_bigquery/
--rw-r--r--   0 pisces    (1000) pisces    (1000)       94 2024-05-12 05:25:15.000000 tree-sitter-sql-bigquery-0.6.0b0/bindings/python/tree_sitter_sql_bigquery/__init__.py
--rw-r--r--   0 pisces    (1000) pisces    (1000)       27 2024-05-12 05:25:15.000000 tree-sitter-sql-bigquery-0.6.0b0/bindings/python/tree_sitter_sql_bigquery/__init__.pyi
--rw-r--r--   0 pisces    (1000) pisces    (1000)      648 2024-05-12 05:25:15.000000 tree-sitter-sql-bigquery-0.6.0b0/bindings/python/tree_sitter_sql_bigquery/binding.c
--rw-r--r--   0 pisces    (1000) pisces    (1000)        0 2024-05-12 05:25:15.000000 tree-sitter-sql-bigquery-0.6.0b0/bindings/python/tree_sitter_sql_bigquery/py.typed
-drwxr-xr-x   0 pisces    (1000) pisces    (1000)        0 2024-05-12 10:59:12.227060 tree-sitter-sql-bigquery-0.6.0b0/bindings/python/tree_sitter_sql_bigquery.egg-info/
--rw-r--r--   0 pisces    (1000) pisces    (1000)     1502 2024-05-12 10:59:12.000000 tree-sitter-sql-bigquery-0.6.0b0/bindings/python/tree_sitter_sql_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 pisces    (1000) pisces    (1000)      658 2024-05-12 10:59:12.000000 tree-sitter-sql-bigquery-0.6.0b0/bindings/python/tree_sitter_sql_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 pisces    (1000) pisces    (1000)        1 2024-05-12 10:59:12.000000 tree-sitter-sql-bigquery-0.6.0b0/bindings/python/tree_sitter_sql_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 pisces    (1000) pisces    (1000)        1 2024-05-12 05:43:31.000000 tree-sitter-sql-bigquery-0.6.0b0/bindings/python/tree_sitter_sql_bigquery.egg-info/not-zip-safe
--rw-r--r--   0 pisces    (1000) pisces    (1000)       26 2024-05-12 10:59:12.000000 tree-sitter-sql-bigquery-0.6.0b0/bindings/python/tree_sitter_sql_bigquery.egg-info/requires.txt
--rw-r--r--   0 pisces    (1000) pisces    (1000)       34 2024-05-12 10:59:12.000000 tree-sitter-sql-bigquery-0.6.0b0/bindings/python/tree_sitter_sql_bigquery.egg-info/top_level.txt
--rw-r--r--   0 pisces    (1000) pisces    (1000)      774 2024-05-12 10:32:34.000000 tree-sitter-sql-bigquery-0.6.0b0/pyproject.toml
--rw-r--r--   0 pisces    (1000) pisces    (1000)       38 2024-05-12 10:59:12.247061 tree-sitter-sql-bigquery-0.6.0b0/setup.cfg
--rw-r--r--   0 pisces    (1000) pisces    (1000)     1536 2024-05-12 04:01:23.000000 tree-sitter-sql-bigquery-0.6.0b0/setup.py
-drwxr-xr-x   0 pisces    (1000) pisces    (1000)        0 2024-05-12 10:59:12.247061 tree-sitter-sql-bigquery-0.6.0b0/src/
--rw-r--r--   0 pisces    (1000) pisces    (1000) 33276574 2024-05-12 06:41:43.000000 tree-sitter-sql-bigquery-0.6.0b0/src/parser.c
--rw-r--r--   0 pisces    (1000) pisces    (1000)     8498 2024-05-12 06:06:34.000000 tree-sitter-sql-bigquery-0.6.0b0/src/scanner.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:38:40.770637 tree-sitter-sql-bigquery-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-20 21:38:37.000000 tree-sitter-sql-bigquery-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-20 21:38:40.770637 tree-sitter-sql-bigquery-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-20 21:38:37.000000 tree-sitter-sql-bigquery-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:38:40.726637 tree-sitter-sql-bigquery-0.7.0/bindings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:38:40.726637 tree-sitter-sql-bigquery-0.7.0/bindings/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:38:40.730637 tree-sitter-sql-bigquery-0.7.0/bindings/python/tree_sitter_sql_bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-20 21:38:37.000000 tree-sitter-sql-bigquery-0.7.0/bindings/python/tree_sitter_sql_bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 21:38:37.000000 tree-sitter-sql-bigquery-0.7.0/bindings/python/tree_sitter_sql_bigquery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-20 21:38:37.000000 tree-sitter-sql-bigquery-0.7.0/bindings/python/tree_sitter_sql_bigquery/binding.c
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:38:37.000000 tree-sitter-sql-bigquery-0.7.0/bindings/python/tree_sitter_sql_bigquery/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:38:40.730637 tree-sitter-sql-bigquery-0.7.0/bindings/python/tree_sitter_sql_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-20 21:38:40.000000 tree-sitter-sql-bigquery-0.7.0/bindings/python/tree_sitter_sql_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-20 21:38:40.000000 tree-sitter-sql-bigquery-0.7.0/bindings/python/tree_sitter_sql_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:38:40.000000 tree-sitter-sql-bigquery-0.7.0/bindings/python/tree_sitter_sql_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:38:40.000000 tree-sitter-sql-bigquery-0.7.0/bindings/python/tree_sitter_sql_bigquery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 21:38:40.000000 tree-sitter-sql-bigquery-0.7.0/bindings/python/tree_sitter_sql_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-20 21:38:40.000000 tree-sitter-sql-bigquery-0.7.0/bindings/python/tree_sitter_sql_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-20 21:38:37.000000 tree-sitter-sql-bigquery-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:38:40.770637 tree-sitter-sql-bigquery-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-20 21:38:37.000000 tree-sitter-sql-bigquery-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:38:40.770637 tree-sitter-sql-bigquery-0.7.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127) 33276574 2024-05-20 21:38:37.000000 tree-sitter-sql-bigquery-0.7.0/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-20 21:38:37.000000 tree-sitter-sql-bigquery-0.7.0/src/scanner.c
```

### Comparing `tree-sitter-sql-bigquery-0.6.0b0/LICENSE` & `tree-sitter-sql-bigquery-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-sitter-sql-bigquery-0.6.0b0/PKG-INFO` & `tree-sitter-sql-bigquery-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-sitter-sql-bigquery
-Version: 0.6.0b0
+Version: 0.7.0
 Summary: SqlBigquery grammar for tree-sitter
 License: MIT
 Project-URL: Homepage, https://github.com/tree-sitter/tree-sitter-sql-bigquery
 Keywords: incremental,parsing,tree-sitter,sql-bigquery
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
```

### Comparing `tree-sitter-sql-bigquery-0.6.0b0/README.md` & `tree-sitter-sql-bigquery-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tree-sitter-sql-bigquery-0.6.0b0/bindings/python/tree_sitter_sql_bigquery/binding.c` & `tree-sitter-sql-bigquery-0.7.0/bindings/python/tree_sitter_sql_bigquery/binding.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-sql-bigquery-0.6.0b0/bindings/python/tree_sitter_sql_bigquery.egg-info/PKG-INFO` & `tree-sitter-sql-bigquery-0.7.0/bindings/python/tree_sitter_sql_bigquery.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-sitter-sql-bigquery
-Version: 0.6.0b0
+Version: 0.7.0
 Summary: SqlBigquery grammar for tree-sitter
 License: MIT
 Project-URL: Homepage, https://github.com/tree-sitter/tree-sitter-sql-bigquery
 Keywords: incremental,parsing,tree-sitter,sql-bigquery
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
```

### Comparing `tree-sitter-sql-bigquery-0.6.0b0/bindings/python/tree_sitter_sql_bigquery.egg-info/SOURCES.txt` & `tree-sitter-sql-bigquery-0.7.0/bindings/python/tree_sitter_sql_bigquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tree-sitter-sql-bigquery-0.6.0b0/pyproject.toml` & `tree-sitter-sql-bigquery-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tree-sitter-sql-bigquery"
 description = "SqlBigquery grammar for tree-sitter"
-version = "0.6.0-beta00"
+version = "0.7.0"
 keywords = ["incremental", "parsing", "tree-sitter", "sql-bigquery"]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Topic :: Software Development :: Compilers",
   "Topic :: Text Processing :: Linguistic",
   "Typing :: Typed"
@@ -18,12 +18,12 @@
 license.text = "MIT"
 readme = "README.md"
 
 [project.urls]
 Homepage = "https://github.com/tree-sitter/tree-sitter-sql-bigquery"
 
 [project.optional-dependencies]
-core = ["tree-sitter~=0.22"]
+core = ["tree-sitter~=0.21"]
 
 [tool.cibuildwheel]
 build = "cp38-*"
 build-frontend = "build"
```

### Comparing `tree-sitter-sql-bigquery-0.6.0b0/setup.py` & `tree-sitter-sql-bigquery-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `tree-sitter-sql-bigquery-0.6.0b0/src/parser.c` & `tree-sitter-sql-bigquery-0.7.0/src/parser.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-sql-bigquery-0.6.0b0/src/scanner.c` & `tree-sitter-sql-bigquery-0.7.0/src/scanner.c`

 * *Files 4% similar despite different names*

```diff
@@ -22,26 +22,18 @@
 
 typedef struct {
     char flags;
 } Delimiter;
 
 static inline Delimiter new_delimiter() { return (Delimiter){0}; }
 
-static inline bool is_raw(Delimiter *delimiter) {
-    return delimiter->flags & Raw;
-}
-
 static inline bool is_triple(Delimiter *delimiter) {
     return delimiter->flags & Triple;
 }
 
-static inline bool is_bytes(Delimiter *delimiter) {
-    return delimiter->flags & Bytes;
-}
-
 static inline int32_t end_character(Delimiter *delimiter) {
     if (delimiter->flags & SingleQuote)
         return '\'';
     if (delimiter->flags & DoubleQuote)
         return '"';
     return 0;
 }
@@ -247,35 +239,29 @@
     return size;
 }
 
 void tree_sitter_sql_bigquery_external_scanner_deserialize(void *payload,
                                                            const char *buffer,
                                                            unsigned length) {
     Scanner *scanner = (Scanner *)payload;
+    array_clear(&scanner->delimiters);
+    if(length == 0) return;
 
-    array_delete(&scanner->delimiters);
-
-    if (length > 0) {
-        size_t size = 0;
-
-        size_t delimiter_count = (uint8_t)buffer[size++];
-        if (delimiter_count > 0) {
-            array_reserve(&scanner->delimiters, delimiter_count);
-            scanner->delimiters.size = delimiter_count;
-            memcpy(scanner->delimiters.contents, &buffer[size],
-                   delimiter_count);
-            size += delimiter_count;
-        }
+    size_t size = 0;
+    size_t delimiter_count = (uint8_t)buffer[size++];
+    if (delimiter_count > 0) {
+        array_reserve(&scanner->delimiters, delimiter_count);
+        scanner->delimiters.size = delimiter_count;
+        memcpy(scanner->delimiters.contents, &buffer[size], delimiter_count);
     }
 }
 
 void *tree_sitter_sql_bigquery_external_scanner_create() {
     Scanner *scanner = (Scanner *)ts_calloc(1, sizeof(Scanner));
-
-    array_init(&scanner->delimiters);
-    tree_sitter_sql_bigquery_external_scanner_deserialize(scanner, NULL, 0);
     return scanner;
 }
 
 void tree_sitter_sql_bigquery_external_scanner_destroy(void *payload) {
-    ts_free((Scanner *)payload);
+    Scanner *scanner = (Scanner *)payload;
+    array_delete(&scanner->delimiters);
+    ts_free(scanner);
 }
```

