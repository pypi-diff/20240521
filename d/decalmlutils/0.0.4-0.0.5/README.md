# Comparing `tmp/decalmlutils-0.0.4.tar.gz` & `tmp/decalmlutils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decalmlutils-0.0.4.tar", last modified: Fri May 10 21:31:10 2024, max compression
+gzip compressed data, was "decalmlutils-0.0.5.tar", last modified: Tue May 21 21:21:22 2024, max compression
```

## Comparing `decalmlutils-0.0.4.tar` & `decalmlutils-0.0.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-10 21:31:10.478621 decalmlutils-0.0.4/
--rw-rw-r--   0 richard   (1000) richard   (1000)    11358 2024-02-14 15:27:04.000000 decalmlutils-0.0.4/LICENSE
--rw-r--r--   0 richard   (1000) richard   (1000)     6350 2024-05-10 21:31:10.478621 decalmlutils-0.0.4/PKG-INFO
--rw-rw-r--   0 richard   (1000) richard   (1000)     2117 2024-05-10 21:20:37.000000 decalmlutils-0.0.4/README.md
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-10 21:31:10.474621 decalmlutils-0.0.4/decalmlutils/
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-10 21:31:10.478621 decalmlutils-0.0.4/decalmlutils/decalmlutils.egg-info/
--rw-r--r--   0 richard   (1000) richard   (1000)     6350 2024-05-10 21:31:10.000000 decalmlutils-0.0.4/decalmlutils/decalmlutils.egg-info/PKG-INFO
--rw-rw-r--   0 richard   (1000) richard   (1000)     1300 2024-05-10 21:31:10.000000 decalmlutils-0.0.4/decalmlutils/decalmlutils.egg-info/SOURCES.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)        1 2024-05-10 21:31:10.000000 decalmlutils-0.0.4/decalmlutils/decalmlutils.egg-info/dependency_links.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)      846 2024-05-10 21:31:10.000000 decalmlutils-0.0.4/decalmlutils/decalmlutils.egg-info/requires.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)       11 2024-05-10 21:31:10.000000 decalmlutils-0.0.4/decalmlutils/decalmlutils.egg-info/top_level.txt
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-10 21:31:10.474621 decalmlutils-0.0.4/decalmlutils/io/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 14:10:58.000000 decalmlutils-0.0.4/decalmlutils/io/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     4668 2024-05-10 21:01:49.000000 decalmlutils-0.0.4/decalmlutils/io/context.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-10 21:31:10.474621 decalmlutils-0.0.4/decalmlutils/io/disk/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 20:50:13.000000 decalmlutils-0.0.4/decalmlutils/io/disk/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1699 2024-05-04 09:54:41.000000 decalmlutils-0.0.4/decalmlutils/io/disk/compressed_writer.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1327 2024-05-10 21:05:06.000000 decalmlutils-0.0.4/decalmlutils/io/disk/geojson.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     3437 2024-05-10 21:05:06.000000 decalmlutils-0.0.4/decalmlutils/io/disk/img.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      682 2024-05-10 21:05:06.000000 decalmlutils-0.0.4/decalmlutils/io/disk/json.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2191 2024-05-10 21:05:06.000000 decalmlutils-0.0.4/decalmlutils/io/disk/misc.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     5220 2024-05-10 21:01:49.000000 decalmlutils-0.0.4/decalmlutils/io/disk/parquet.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      196 2024-02-14 20:50:13.000000 decalmlutils-0.0.4/decalmlutils/io/disk/yaml.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      966 2024-02-14 21:13:54.000000 decalmlutils-0.0.4/decalmlutils/io/git_.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2767 2024-05-10 21:05:05.000000 decalmlutils-0.0.4/decalmlutils/io/jira_.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-10 21:31:10.478621 decalmlutils-0.0.4/decalmlutils/io/mflow/
--rw-rw-r--   0 richard   (1000) richard   (1000)      469 2024-05-10 21:05:06.000000 decalmlutils-0.0.4/decalmlutils/io/mflow/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    19247 2024-05-10 21:05:06.000000 decalmlutils-0.0.4/decalmlutils/io/mflow/artifacts.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2845 2024-05-10 21:22:50.000000 decalmlutils-0.0.4/decalmlutils/io/mflow/cloudwatch_logs.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     4238 2024-02-15 15:48:28.000000 decalmlutils-0.0.4/decalmlutils/io/mflow/decorators.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     4077 2024-05-10 21:05:06.000000 decalmlutils-0.0.4/decalmlutils/io/mflow/deps.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1029 2024-02-14 22:19:06.000000 decalmlutils-0.0.4/decalmlutils/io/mflow/flows.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     7696 2024-05-10 21:05:06.000000 decalmlutils-0.0.4/decalmlutils/io/mflow/lineage.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    15127 2024-02-15 15:50:10.000000 decalmlutils-0.0.4/decalmlutils/io/mflow/runs.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1786 2024-02-15 15:48:28.000000 decalmlutils-0.0.4/decalmlutils/io/mflow/tasks.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2890 2024-05-10 21:05:06.000000 decalmlutils-0.0.4/decalmlutils/io/mflow/workflows.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     6975 2024-05-10 21:26:05.000000 decalmlutils-0.0.4/decalmlutils/io/misc.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     6697 2024-05-10 21:05:05.000000 decalmlutils-0.0.4/decalmlutils/io/slack.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1284 2024-02-14 21:25:06.000000 decalmlutils-0.0.4/decalmlutils/io/sort.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-10 21:31:10.478621 decalmlutils-0.0.4/decalmlutils/metrics/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 14:13:02.000000 decalmlutils-0.0.4/decalmlutils/metrics/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    12437 2024-05-10 21:05:06.000000 decalmlutils-0.0.4/decalmlutils/metrics/misc.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    17049 2024-05-10 21:05:07.000000 decalmlutils-0.0.4/decalmlutils/metrics/prg.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2143 2024-03-04 16:56:09.000000 decalmlutils-0.0.4/decalmlutils/metrics/rankme.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      993 2024-05-10 21:05:05.000000 decalmlutils-0.0.4/pyproject.toml
--rw-rw-r--   0 richard   (1000) richard   (1000)       38 2024-05-10 21:31:10.478621 decalmlutils-0.0.4/setup.cfg
--rw-rw-r--   0 richard   (1000) richard   (1000)     3930 2024-05-10 21:29:16.000000 decalmlutils-0.0.4/setup.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-10 21:31:10.478621 decalmlutils-0.0.4/tests/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 21:27:17.000000 decalmlutils-0.0.4/tests/test_plotting.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1586 2024-05-10 21:05:07.000000 decalmlutils-0.0.4/tests/test_tensors.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      233 2024-05-10 21:05:07.000000 decalmlutils-0.0.4/tests/test_testing.py
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 21:25:36.000000 decalmlutils-0.0.4/tests/test_text.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      416 2024-05-10 21:05:06.000000 decalmlutils-0.0.4/tests/test_training.py
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 17:31:23.000000 decalmlutils-0.0.4/tests/test_web.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-21 21:21:22.436585 decalmlutils-0.0.5/
+-rw-rw-r--   0 richard   (1000) richard   (1000)    11358 2024-02-14 15:27:04.000000 decalmlutils-0.0.5/LICENSE
+-rw-r--r--   0 richard   (1000) richard   (1000)     6350 2024-05-21 21:21:22.436585 decalmlutils-0.0.5/PKG-INFO
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2117 2024-05-10 21:20:37.000000 decalmlutils-0.0.5/README.md
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-21 21:21:22.432584 decalmlutils-0.0.5/decalmlutils/
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-21 21:21:22.432584 decalmlutils-0.0.5/decalmlutils/decalmlutils.egg-info/
+-rw-r--r--   0 richard   (1000) richard   (1000)     6350 2024-05-21 21:21:22.000000 decalmlutils-0.0.5/decalmlutils/decalmlutils.egg-info/PKG-INFO
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1300 2024-05-21 21:21:22.000000 decalmlutils-0.0.5/decalmlutils/decalmlutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)        1 2024-05-21 21:21:22.000000 decalmlutils-0.0.5/decalmlutils/decalmlutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)      846 2024-05-21 21:21:22.000000 decalmlutils-0.0.5/decalmlutils/decalmlutils.egg-info/requires.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)       11 2024-05-21 21:21:22.000000 decalmlutils-0.0.5/decalmlutils/decalmlutils.egg-info/top_level.txt
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-21 21:21:22.432584 decalmlutils-0.0.5/decalmlutils/io/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 14:10:58.000000 decalmlutils-0.0.5/decalmlutils/io/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     4668 2024-05-10 21:01:49.000000 decalmlutils-0.0.5/decalmlutils/io/context.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-21 21:21:22.432584 decalmlutils-0.0.5/decalmlutils/io/disk/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 20:50:13.000000 decalmlutils-0.0.5/decalmlutils/io/disk/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1699 2024-05-04 09:54:41.000000 decalmlutils-0.0.5/decalmlutils/io/disk/compressed_writer.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1327 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/disk/geojson.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     3437 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/disk/img.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      682 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/disk/json.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2191 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/disk/misc.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     5220 2024-05-10 21:01:49.000000 decalmlutils-0.0.5/decalmlutils/io/disk/parquet.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      196 2024-02-14 20:50:13.000000 decalmlutils-0.0.5/decalmlutils/io/disk/yaml.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      966 2024-02-14 21:13:54.000000 decalmlutils-0.0.5/decalmlutils/io/git_.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2767 2024-05-10 21:05:05.000000 decalmlutils-0.0.5/decalmlutils/io/jira_.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-21 21:21:22.432584 decalmlutils-0.0.5/decalmlutils/io/mflow/
+-rw-rw-r--   0 richard   (1000) richard   (1000)      469 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    19247 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/artifacts.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2845 2024-05-10 21:22:50.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/cloudwatch_logs.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     4238 2024-02-15 15:48:28.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/decorators.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     4077 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/deps.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1029 2024-02-14 22:19:06.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/flows.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     7696 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/lineage.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    15127 2024-02-15 15:50:10.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/runs.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1786 2024-02-15 15:48:28.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/tasks.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2890 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/workflows.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     7067 2024-05-21 21:12:36.000000 decalmlutils-0.0.5/decalmlutils/io/misc.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     6697 2024-05-10 21:05:05.000000 decalmlutils-0.0.5/decalmlutils/io/slack.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1284 2024-02-14 21:25:06.000000 decalmlutils-0.0.5/decalmlutils/io/sort.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-21 21:21:22.432584 decalmlutils-0.0.5/decalmlutils/metrics/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 14:13:02.000000 decalmlutils-0.0.5/decalmlutils/metrics/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    12437 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/metrics/misc.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    17049 2024-05-10 21:05:07.000000 decalmlutils-0.0.5/decalmlutils/metrics/prg.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2143 2024-03-04 16:56:09.000000 decalmlutils-0.0.5/decalmlutils/metrics/rankme.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      993 2024-05-10 21:05:05.000000 decalmlutils-0.0.5/pyproject.toml
+-rw-rw-r--   0 richard   (1000) richard   (1000)       38 2024-05-21 21:21:22.436585 decalmlutils-0.0.5/setup.cfg
+-rw-rw-r--   0 richard   (1000) richard   (1000)     3930 2024-05-21 21:16:30.000000 decalmlutils-0.0.5/setup.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-21 21:21:22.432584 decalmlutils-0.0.5/tests/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 21:27:17.000000 decalmlutils-0.0.5/tests/test_plotting.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1586 2024-05-10 21:05:07.000000 decalmlutils-0.0.5/tests/test_tensors.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      233 2024-05-10 21:05:07.000000 decalmlutils-0.0.5/tests/test_testing.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 21:25:36.000000 decalmlutils-0.0.5/tests/test_text.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      416 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/tests/test_training.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 17:31:23.000000 decalmlutils-0.0.5/tests/test_web.py
```

### Comparing `decalmlutils-0.0.4/LICENSE` & `decalmlutils-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/PKG-INFO` & `decalmlutils-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decalmlutils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Useful functions when working with Machine Learning in Python
 Home-page: https://github.com/crypdick/decalmlutils
 Author: Richard Decal
 Author-email: public@richarddecal.com
 License: Apache
 Keywords: deep learning pytorch numpy
 Classifier: Development Status :: 5 - Production/Stable
@@ -72,49 +72,49 @@
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-env; extra == "tests"
 Requires-Dist: pytest-xdist; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Provides-Extra: all
-Requires-Dist: slack_sdk; extra == "all"
-Requires-Dist: pytest-xdist; extra == "all"
-Requires-Dist: metaflow; extra == "all"
+Requires-Dist: boto3; extra == "all"
+Requires-Dist: numpy; extra == "all"
+Requires-Dist: pyarrow; extra == "all"
+Requires-Dist: bump2version; extra == "all"
 Requires-Dist: isort; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: geojson; extra == "all"
-Requires-Dist: ray; extra == "all"
-Requires-Dist: tenacity; extra == "all"
-Requires-Dist: build; extra == "all"
-Requires-Dist: torch; extra == "all"
-Requires-Dist: pre-commit; extra == "all"
-Requires-Dist: requests; extra == "all"
-Requires-Dist: jinja2; extra == "all"
+Requires-Dist: hypothesis; extra == "all"
 Requires-Dist: pytest-env; extra == "all"
 Requires-Dist: scikit-learn; extra == "all"
-Requires-Dist: bump2version; extra == "all"
+Requires-Dist: torchvision; extra == "all"
 Requires-Dist: ruff; extra == "all"
-Requires-Dist: pandas; extra == "all"
-Requires-Dist: boto3; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: geojson; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: tenacity; extra == "all"
+Requires-Dist: slack_sdk; extra == "all"
+Requires-Dist: build; extra == "all"
+Requires-Dist: jira; extra == "all"
+Requires-Dist: pytest-mock; extra == "all"
+Requires-Dist: pytest-xdist; extra == "all"
+Requires-Dist: pytest-cov; extra == "all"
+Requires-Dist: twine; extra == "all"
 Requires-Dist: ipython; extra == "all"
+Requires-Dist: pandas; extra == "all"
+Requires-Dist: pytest; extra == "all"
 Requires-Dist: graphviz; extra == "all"
+Requires-Dist: jinja2; extra == "all"
+Requires-Dist: matplotlib>=3.4.0; extra == "all"
 Requires-Dist: click; extra == "all"
-Requires-Dist: hypothesis; extra == "all"
-Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: numpy; extra == "all"
+Requires-Dist: metaflow; extra == "all"
+Requires-Dist: ray; extra == "all"
 Requires-Dist: pyinstrument; extra == "all"
-Requires-Dist: pytest-mock; extra == "all"
-Requires-Dist: torchvision; extra == "all"
-Requires-Dist: pytest; extra == "all"
+Requires-Dist: requests; extra == "all"
+Requires-Dist: pre-commit; extra == "all"
+Requires-Dist: torch; extra == "all"
 Requires-Dist: watchtower; extra == "all"
-Requires-Dist: jira; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: matplotlib>=3.4.0; extra == "all"
-Requires-Dist: twine; extra == "all"
-Requires-Dist: pyarrow; extra == "all"
 
 # decalmlutils
 
 [![Build status](https://github.com/crypdick/decalmlutils/actions/workflows/python-app.yml/badge.svg)](https://github.com/crypdick/decalmlutils/actions/workflows/python-app.yml)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
```

### Comparing `decalmlutils-0.0.4/README.md` & `decalmlutils-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/decalmlutils.egg-info/PKG-INFO` & `decalmlutils-0.0.5/decalmlutils/decalmlutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decalmlutils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Useful functions when working with Machine Learning in Python
 Home-page: https://github.com/crypdick/decalmlutils
 Author: Richard Decal
 Author-email: public@richarddecal.com
 License: Apache
 Keywords: deep learning pytorch numpy
 Classifier: Development Status :: 5 - Production/Stable
@@ -72,49 +72,49 @@
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-env; extra == "tests"
 Requires-Dist: pytest-xdist; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Provides-Extra: all
-Requires-Dist: slack_sdk; extra == "all"
-Requires-Dist: pytest-xdist; extra == "all"
-Requires-Dist: metaflow; extra == "all"
+Requires-Dist: boto3; extra == "all"
+Requires-Dist: numpy; extra == "all"
+Requires-Dist: pyarrow; extra == "all"
+Requires-Dist: bump2version; extra == "all"
 Requires-Dist: isort; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: geojson; extra == "all"
-Requires-Dist: ray; extra == "all"
-Requires-Dist: tenacity; extra == "all"
-Requires-Dist: build; extra == "all"
-Requires-Dist: torch; extra == "all"
-Requires-Dist: pre-commit; extra == "all"
-Requires-Dist: requests; extra == "all"
-Requires-Dist: jinja2; extra == "all"
+Requires-Dist: hypothesis; extra == "all"
 Requires-Dist: pytest-env; extra == "all"
 Requires-Dist: scikit-learn; extra == "all"
-Requires-Dist: bump2version; extra == "all"
+Requires-Dist: torchvision; extra == "all"
 Requires-Dist: ruff; extra == "all"
-Requires-Dist: pandas; extra == "all"
-Requires-Dist: boto3; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: geojson; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: tenacity; extra == "all"
+Requires-Dist: slack_sdk; extra == "all"
+Requires-Dist: build; extra == "all"
+Requires-Dist: jira; extra == "all"
+Requires-Dist: pytest-mock; extra == "all"
+Requires-Dist: pytest-xdist; extra == "all"
+Requires-Dist: pytest-cov; extra == "all"
+Requires-Dist: twine; extra == "all"
 Requires-Dist: ipython; extra == "all"
+Requires-Dist: pandas; extra == "all"
+Requires-Dist: pytest; extra == "all"
 Requires-Dist: graphviz; extra == "all"
+Requires-Dist: jinja2; extra == "all"
+Requires-Dist: matplotlib>=3.4.0; extra == "all"
 Requires-Dist: click; extra == "all"
-Requires-Dist: hypothesis; extra == "all"
-Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: numpy; extra == "all"
+Requires-Dist: metaflow; extra == "all"
+Requires-Dist: ray; extra == "all"
 Requires-Dist: pyinstrument; extra == "all"
-Requires-Dist: pytest-mock; extra == "all"
-Requires-Dist: torchvision; extra == "all"
-Requires-Dist: pytest; extra == "all"
+Requires-Dist: requests; extra == "all"
+Requires-Dist: pre-commit; extra == "all"
+Requires-Dist: torch; extra == "all"
 Requires-Dist: watchtower; extra == "all"
-Requires-Dist: jira; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: matplotlib>=3.4.0; extra == "all"
-Requires-Dist: twine; extra == "all"
-Requires-Dist: pyarrow; extra == "all"
 
 # decalmlutils
 
 [![Build status](https://github.com/crypdick/decalmlutils/actions/workflows/python-app.yml/badge.svg)](https://github.com/crypdick/decalmlutils/actions/workflows/python-app.yml)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
```

### Comparing `decalmlutils-0.0.4/decalmlutils/decalmlutils.egg-info/SOURCES.txt` & `decalmlutils-0.0.5/decalmlutils/decalmlutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/context.py` & `decalmlutils-0.0.5/decalmlutils/io/context.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/disk/compressed_writer.py` & `decalmlutils-0.0.5/decalmlutils/io/disk/compressed_writer.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/disk/geojson.py` & `decalmlutils-0.0.5/decalmlutils/io/disk/geojson.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/disk/img.py` & `decalmlutils-0.0.5/decalmlutils/io/disk/img.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/disk/json.py` & `decalmlutils-0.0.5/decalmlutils/io/disk/json.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/disk/misc.py` & `decalmlutils-0.0.5/decalmlutils/io/disk/misc.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/disk/parquet.py` & `decalmlutils-0.0.5/decalmlutils/io/disk/parquet.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/git_.py` & `decalmlutils-0.0.5/decalmlutils/io/git_.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/jira_.py` & `decalmlutils-0.0.5/decalmlutils/io/jira_.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/mflow/artifacts.py` & `decalmlutils-0.0.5/decalmlutils/io/mflow/artifacts.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/mflow/cloudwatch_logs.py` & `decalmlutils-0.0.5/decalmlutils/io/mflow/cloudwatch_logs.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/mflow/decorators.py` & `decalmlutils-0.0.5/decalmlutils/io/mflow/decorators.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/mflow/deps.py` & `decalmlutils-0.0.5/decalmlutils/io/mflow/deps.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/mflow/flows.py` & `decalmlutils-0.0.5/decalmlutils/io/mflow/flows.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/mflow/lineage.py` & `decalmlutils-0.0.5/decalmlutils/io/mflow/lineage.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/mflow/runs.py` & `decalmlutils-0.0.5/decalmlutils/io/mflow/runs.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/mflow/tasks.py` & `decalmlutils-0.0.5/decalmlutils/io/mflow/tasks.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/mflow/workflows.py` & `decalmlutils-0.0.5/decalmlutils/io/mflow/workflows.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/misc.py` & `decalmlutils-0.0.5/decalmlutils/io/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,14 +155,15 @@
     return pprint.pformat(natural_sort(items))
 
 
 @beartype
 def kwargs_to_filename(
     date: DateType = None,
     ext="",
+    prefix: Optional[str] = None,
     suffix: Optional[str] = None,
     key_only: Optional[list[str]] = None,
     **kwargs,
 ) -> str:
     """
     Generates a nice filename from a dictionary of kwargs.
 
@@ -225,14 +226,16 @@
     # clean up ++
     filename = filename.replace("++", "+")
 
     # remove leading and trailing spaces or +
     filename = filename.strip()
     filename = filename.strip("+")
 
+    if prefix:
+        filename = f"{prefix}__{filename}"
     if suffix:
         filename = f"{filename}__{suffix}"
     if ext:
         filename = f"{filename}.{ext}"
 
     return filename
```

### Comparing `decalmlutils-0.0.4/decalmlutils/io/slack.py` & `decalmlutils-0.0.5/decalmlutils/io/slack.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/io/sort.py` & `decalmlutils-0.0.5/decalmlutils/io/sort.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/metrics/misc.py` & `decalmlutils-0.0.5/decalmlutils/metrics/misc.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/metrics/prg.py` & `decalmlutils-0.0.5/decalmlutils/metrics/prg.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/decalmlutils/metrics/rankme.py` & `decalmlutils-0.0.5/decalmlutils/metrics/rankme.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/pyproject.toml` & `decalmlutils-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.4/setup.py` & `decalmlutils-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 extras = {
     **_extras,
     "all": list({dep for deps in _extras.values() for dep in deps}),
 }
 
 setup(
     name="decalmlutils",
-    version="0.0.4",
+    version="0.0.5",
     author="Richard Decal",
     author_email="public@richarddecal.com",
     description="Useful functions when working with Machine Learning in Python",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning pytorch numpy",
     license="Apache",
```

### Comparing `decalmlutils-0.0.4/tests/test_tensors.py` & `decalmlutils-0.0.5/tests/test_tensors.py`

 * *Files identical despite different names*

