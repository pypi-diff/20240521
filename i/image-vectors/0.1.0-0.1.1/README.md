# Comparing `tmp/image_vectors-0.1.0.tar.gz` & `tmp/image_vectors-0.1.1.tar.gz`

## Comparing `image_vectors-0.1.0.tar` & `image_vectors-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 image_vectors-0.1.0/src/image_vectors/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 image_vectors-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 image_vectors-0.1.0/.gitignore
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 image_vectors-0.1.0/README.md
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 image_vectors-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 image_vectors-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    75986 2020-02-02 00:00:00.000000 image_vectors-0.1.1/pdm.lock
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 image_vectors-0.1.1/src/image_vectors/__init__.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 image_vectors-0.1.1/src/image_vectors/embedder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 image_vectors-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 image_vectors-0.1.1/tests/test_embedder.py
+-rw-r--r--   0        0        0   104626 2020-02-02 00:00:00.000000 image_vectors-0.1.1/tests/assets/example-image.jpg
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 image_vectors-0.1.1/.gitignore
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 image_vectors-0.1.1/README.md
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 image_vectors-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 image_vectors-0.1.1/PKG-INFO
```

### Comparing `image_vectors-0.1.0/.gitignore` & `image_vectors-0.1.1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -156,7 +156,10 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+# Apple
+.DS_Store
```

