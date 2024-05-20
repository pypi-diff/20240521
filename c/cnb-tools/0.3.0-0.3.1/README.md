# Comparing `tmp/cnb_tools-0.3.0.tar.gz` & `tmp/cnb_tools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnb_tools-0.3.0.tar", max compression
+gzip compressed data, was "cnb_tools-0.3.1.tar", max compression
```

## Comparing `cnb_tools-0.3.0.tar` & `cnb_tools-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-03-22 21:14:14.440131 cnb_tools-0.3.0/LICENSE
--rw-r--r--   0        0        0     3419 2024-03-22 21:14:14.440280 cnb_tools-0.3.0/README.md
--rw-r--r--   0        0        0       81 2024-05-02 23:43:17.720382 cnb_tools-0.3.0/cnb_tools/__init__.py
--rw-r--r--   0        0        0       54 2024-03-22 21:14:14.440603 cnb_tools-0.3.0/cnb_tools/__main__.py
--rw-r--r--   0        0        0     2586 2024-05-16 23:29:46.060950 cnb_tools-0.3.0/cnb_tools/classes/annotation.py
--rw-r--r--   0        0        0     1366 2024-05-16 23:29:46.061910 cnb_tools-0.3.0/cnb_tools/classes/base.py
--rw-r--r--   0        0        0     1119 2024-05-16 23:29:46.063286 cnb_tools-0.3.0/cnb_tools/classes/participant.py
--rw-r--r--   0        0        0      994 2024-05-16 23:29:46.064287 cnb_tools-0.3.0/cnb_tools/classes/queue.py
--rw-r--r--   0        0        0     2341 2024-05-16 23:29:46.065040 cnb_tools-0.3.0/cnb_tools/classes/submission.py
--rw-r--r--   0        0        0     4753 2024-05-16 23:29:46.067072 cnb_tools-0.3.0/cnb_tools/commands/submission_cli.py
--rw-r--r--   0        0        0     1183 2024-04-04 22:34:42.552921 cnb_tools-0.3.0/cnb_tools/main_cli.py
--rw-r--r--   0        0        0     4055 2024-05-18 00:02:25.655870 cnb_tools-0.3.0/cnb_tools/validation_toolkit.py
--rw-r--r--   0        0        0     1688 2024-05-17 23:32:45.644846 cnb_tools-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4890 1970-01-01 00:00:00.000000 cnb_tools-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-22 21:14:14.440131 cnb_tools-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3419 2024-03-22 21:14:14.440280 cnb_tools-0.3.1/README.md
+-rw-r--r--   0        0        0       81 2024-05-02 23:43:17.720382 cnb_tools-0.3.1/cnb_tools/__init__.py
+-rw-r--r--   0        0        0       54 2024-03-22 21:14:14.440603 cnb_tools-0.3.1/cnb_tools/__main__.py
+-rw-r--r--   0        0        0     2586 2024-05-16 23:29:46.060950 cnb_tools-0.3.1/cnb_tools/classes/annotation.py
+-rw-r--r--   0        0        0     1366 2024-05-16 23:29:46.061910 cnb_tools-0.3.1/cnb_tools/classes/base.py
+-rw-r--r--   0        0        0     1119 2024-05-16 23:29:46.063286 cnb_tools-0.3.1/cnb_tools/classes/participant.py
+-rw-r--r--   0        0        0      994 2024-05-16 23:29:46.064287 cnb_tools-0.3.1/cnb_tools/classes/queue.py
+-rw-r--r--   0        0        0     2341 2024-05-16 23:29:46.065040 cnb_tools-0.3.1/cnb_tools/classes/submission.py
+-rw-r--r--   0        0        0     4753 2024-05-16 23:29:46.067072 cnb_tools-0.3.1/cnb_tools/commands/submission_cli.py
+-rw-r--r--   0        0        0     1183 2024-04-04 22:34:42.552921 cnb_tools-0.3.1/cnb_tools/main_cli.py
+-rw-r--r--   0        0        0     4055 2024-05-18 00:10:17.867431 cnb_tools-0.3.1/cnb_tools/validation_toolkit.py
+-rw-r--r--   0        0        0     1688 2024-05-20 23:53:07.395813 cnb_tools-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4890 1970-01-01 00:00:00.000000 cnb_tools-0.3.1/PKG-INFO
```

### Comparing `cnb_tools-0.3.0/LICENSE` & `cnb_tools-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cnb_tools-0.3.0/README.md` & `cnb_tools-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cnb_tools-0.3.0/cnb_tools/classes/annotation.py` & `cnb_tools-0.3.1/cnb_tools/classes/annotation.py`

 * *Files identical despite different names*

### Comparing `cnb_tools-0.3.0/cnb_tools/classes/base.py` & `cnb_tools-0.3.1/cnb_tools/classes/base.py`

 * *Files identical despite different names*

### Comparing `cnb_tools-0.3.0/cnb_tools/classes/participant.py` & `cnb_tools-0.3.1/cnb_tools/classes/participant.py`

 * *Files identical despite different names*

### Comparing `cnb_tools-0.3.0/cnb_tools/classes/queue.py` & `cnb_tools-0.3.1/cnb_tools/classes/queue.py`

 * *Files identical despite different names*

### Comparing `cnb_tools-0.3.0/cnb_tools/classes/submission.py` & `cnb_tools-0.3.1/cnb_tools/classes/submission.py`

 * *Files identical despite different names*

### Comparing `cnb_tools-0.3.0/cnb_tools/commands/submission_cli.py` & `cnb_tools-0.3.1/cnb_tools/commands/submission_cli.py`

 * *Files identical despite different names*

### Comparing `cnb_tools-0.3.0/cnb_tools/main_cli.py` & `cnb_tools-0.3.1/cnb_tools/main_cli.py`

 * *Files identical despite different names*

### Comparing `cnb_tools-0.3.0/cnb_tools/validation_toolkit.py` & `cnb_tools-0.3.1/cnb_tools/validation_toolkit.py`

 * *Files identical despite different names*

### Comparing `cnb_tools-0.3.0/pyproject.toml` & `cnb_tools-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cnb-tools"
-version = "0.3.0"
+version = "0.3.1"
 description = "Convenience tools/functions for challenges and benchmarking on Synapse.org"
 license = "Apache-2.0"
 authors = ["Sage CNB Team <cnb@sagebase.org>"]
 maintainers = [
     "Verena Chung <verena.chung@sagebase.org>",
 ]
 readme = "README.md"
```

### Comparing `cnb_tools-0.3.0/PKG-INFO` & `cnb_tools-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnb-tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: Convenience tools/functions for challenges and benchmarking on Synapse.org
 Home-page: https://github.com/Sage-Bionetworks-Challenges/cnb-tools
 License: Apache-2.0
 Author: Sage CNB Team
 Author-email: cnb@sagebase.org
 Maintainer: Verena Chung
 Maintainer-email: verena.chung@sagebase.org
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cnb-tools Version: 0.3.0 Summary: Convenience
+Metadata-Version: 2.1 Name: cnb-tools Version: 0.3.1 Summary: Convenience
 tools/functions for challenges and benchmarking on Synapse.org Home-page:
 https://github.com/Sage-Bionetworks-Challenges/cnb-tools License: Apache-2.0
 Author: Sage CNB Team Author-email: cnb@sagebase.org Maintainer: Verena Chung
 Maintainer-email: verena.chung@sagebase.org Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

