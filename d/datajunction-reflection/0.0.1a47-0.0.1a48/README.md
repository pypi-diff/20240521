# Comparing `tmp/datajunction_reflection-0.0.1a47.tar.gz` & `tmp/datajunction_reflection-0.0.1a48.tar.gz`

## Comparing `datajunction_reflection-0.0.1a47.tar` & `datajunction_reflection-0.0.1a48.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/.coveragerc
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/.flake8
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/.isort.cfg
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/.pre-commit-config.yaml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/.pylintrc
--rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/Dockerfile
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/Makefile
--rw-r--r--   0        0        0    95757 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/pdm.lock
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/setup.cfg
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/tox.ini
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/datajunction_reflection/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/datajunction_reflection/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/datajunction_reflection/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/datajunction_reflection/worker/__init__.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/datajunction_reflection/worker/app.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/datajunction_reflection/worker/tasks.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/datajunction_reflection/worker/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/tests/__init__.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/tests/conftest.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/tests/test_tasks.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/LICENSE
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/README.md
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/pyproject.toml
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a47/PKG-INFO
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/.coveragerc
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/.flake8
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/.isort.cfg
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/.pylintrc
+-rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/Dockerfile
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/Makefile
+-rw-r--r--   0        0        0    95757 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/pdm.lock
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/setup.cfg
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/tox.ini
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/datajunction_reflection/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/datajunction_reflection/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/datajunction_reflection/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/datajunction_reflection/worker/__init__.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/datajunction_reflection/worker/app.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/datajunction_reflection/worker/tasks.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/datajunction_reflection/worker/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/tests/__init__.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/tests/conftest.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/tests/test_tasks.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/LICENSE
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/README.md
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/pyproject.toml
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 datajunction_reflection-0.0.1a48/PKG-INFO
```

### Comparing `datajunction_reflection-0.0.1a47/.coveragerc` & `datajunction_reflection-0.0.1a48/.coveragerc`

 * *Files identical despite different names*

### Comparing `datajunction_reflection-0.0.1a47/.pre-commit-config.yaml` & `datajunction_reflection-0.0.1a48/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `datajunction_reflection-0.0.1a47/CODE_OF_CONDUCT.md` & `datajunction_reflection-0.0.1a48/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `datajunction_reflection-0.0.1a47/Makefile` & `datajunction_reflection-0.0.1a48/Makefile`

 * *Files identical despite different names*

### Comparing `datajunction_reflection-0.0.1a47/pdm.lock` & `datajunction_reflection-0.0.1a48/pdm.lock`

 * *Files identical despite different names*

### Comparing `datajunction_reflection-0.0.1a47/setup.cfg` & `datajunction_reflection-0.0.1a48/setup.cfg`

 * *Files identical despite different names*

### Comparing `datajunction_reflection-0.0.1a47/datajunction_reflection/config.py` & `datajunction_reflection-0.0.1a48/datajunction_reflection/config.py`

 * *Files identical despite different names*

### Comparing `datajunction_reflection-0.0.1a47/datajunction_reflection/worker/tasks.py` & `datajunction_reflection-0.0.1a48/datajunction_reflection/worker/tasks.py`

 * *Files identical despite different names*

### Comparing `datajunction_reflection-0.0.1a47/datajunction_reflection/worker/utils.py` & `datajunction_reflection-0.0.1a48/datajunction_reflection/worker/utils.py`

 * *Files identical despite different names*

### Comparing `datajunction_reflection-0.0.1a47/tests/conftest.py` & `datajunction_reflection-0.0.1a48/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datajunction_reflection-0.0.1a47/tests/test_tasks.py` & `datajunction_reflection-0.0.1a48/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `datajunction_reflection-0.0.1a47/.gitignore` & `datajunction_reflection-0.0.1a48/.gitignore`

 * *Files identical despite different names*

### Comparing `datajunction_reflection-0.0.1a47/LICENSE` & `datajunction_reflection-0.0.1a48/LICENSE`

 * *Files identical despite different names*

### Comparing `datajunction_reflection-0.0.1a47/README.md` & `datajunction_reflection-0.0.1a48/README.md`

 * *Files identical despite different names*

### Comparing `datajunction_reflection-0.0.1a47/pyproject.toml` & `datajunction_reflection-0.0.1a48/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datajunction_reflection-0.0.1a47/PKG-INFO` & `datajunction_reflection-0.0.1a48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: datajunction-reflection
-Version: 0.0.1a47
+Version: 0.0.1a48
 Summary: OSS Implementation of a DataJunction Reflection Service
 Project-URL: repository, https://github.com/DataJunction/dj
 Author-email: DataJunction Authors <roberto@dealmeida.net>
 License: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```
