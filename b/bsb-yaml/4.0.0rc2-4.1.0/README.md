# Comparing `tmp/bsb_yaml-4.0.0rc2.tar.gz` & `tmp/bsb_yaml-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsb_yaml-4.0.0rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bsb_yaml-4.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bsb_yaml-4.0.0rc2.tar` & `bsb_yaml-4.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0    33041 2024-02-08 13:34:52.206837 bsb_yaml-4.0.0rc2/LICENSE
--rwxr-xr-x   0        0        0       12 2024-01-05 17:03:10.175209 bsb_yaml-4.0.0rc2/README.md
--rwxr-xr-x   0        0        0      121 2024-03-28 20:48:32.606832 bsb_yaml-4.0.0rc2/bsb_yaml/__init__.py
--rwxr-xr-x   0        0        0      409 2024-03-28 13:47:14.627608 bsb_yaml-4.0.0rc2/bsb_yaml/components.py
--rwxr-xr-x   0        0        0      755 2024-03-28 13:39:55.315004 bsb_yaml-4.0.0rc2/bsb_yaml/parser.py
--rwxr-xr-x   0        0        0      176 2024-01-05 17:03:10.174209 bsb_yaml-4.0.0rc2/bsb_yaml/templates/__init__.py
--rwxr-xr-x   0        0        0      258 2024-01-05 17:03:10.174209 bsb_yaml-4.0.0rc2/bsb_yaml/templates/skeleton.yaml
--rwxr-xr-x   0        0        0      540 2024-01-05 17:03:10.175209 bsb_yaml-4.0.0rc2/bsb_yaml/templates/starting_example.yaml
--rwxr-xr-x   0        0        0     1901 2024-03-28 20:48:22.959865 bsb_yaml-4.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 bsb_yaml-4.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    33041 2024-03-19 12:14:21.193690 bsb_yaml-4.1.0/LICENSE
+-rw-r--r--   0        0        0       11 2024-03-19 12:14:21.193690 bsb_yaml-4.1.0/README.md
+-rw-r--r--   0        0        0      117 2024-05-21 15:01:56.302114 bsb_yaml-4.1.0/bsb_yaml/__init__.py
+-rw-r--r--   0        0        0      409 2024-03-28 16:16:10.923609 bsb_yaml-4.1.0/bsb_yaml/components.py
+-rw-r--r--   0        0        0      775 2024-05-21 15:01:25.182180 bsb_yaml-4.1.0/bsb_yaml/parser.py
+-rw-r--r--   0        0        0      169 2024-03-19 12:14:21.193690 bsb_yaml-4.1.0/bsb_yaml/templates/__init__.py
+-rw-r--r--   0        0        0      242 2024-03-19 12:14:21.193690 bsb_yaml-4.1.0/bsb_yaml/templates/skeleton.yaml
+-rw-r--r--   0        0        0      510 2024-03-19 12:14:21.193690 bsb_yaml-4.1.0/bsb_yaml/templates/starting_example.yaml
+-rw-r--r--   0        0        0     1504 2024-05-21 15:01:56.310114 bsb_yaml-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 bsb_yaml-4.1.0/PKG-INFO
```

### Comparing `bsb_yaml-4.0.0rc2/LICENSE` & `bsb_yaml-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bsb_yaml-4.0.0rc2/pyproject.toml` & `bsb_yaml-4.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -5,53 +5,41 @@
 [project]
 name = "bsb-yaml"
 authors = [{name = "Robin De Schepper", email = "robingilbert.deschepper@unipv.it"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"]
 dynamic = ["version", "description"]
-dependencies = ["bsb-core==4.0.0rc2", "PyYAML~=6.0"]
+dependencies = ["bsb-core~=4.1", "PyYAML~=6.0"]
 
 [project.entry-points."bsb.config.parsers"]
 yaml = "bsb_yaml.parser"
 
 [project.entry-points."bsb.config.templates"]
 yaml_templates = "bsb_yaml.templates"
 
 [tool.flit.module]
 name = "bsb_yaml"
 
 [project.optional-dependencies]
-test = ["bsb-core[parallel]", "bsb-test==4.0.0rc2", "coverage~=7.0"]
+test = ["bsb-core[parallel]", "bsb-test~=4.0", "coverage~=7.0"]
 dev = [
     "pre-commit~=3.5",
-    "black~=23.11",
+    "black~=24.0",
     "isort~=5.12",
     "bump-my-version~=0.18"
 ]
 
 [tool.isort]
 profile = "black"
 
 [tool.bumpversion]
-current_version = "4.0.0-rc2"
-parse = """(?x)
-    (?P<major>0|[1-9]\\d*)\\.
-    (?P<minor>0|[1-9]\\d*)\\.
-    (?P<patch>0|[1-9]\\d*)
-    (?:
-        -                             # dash seperator for pre-release section
-        (?P<pre_l>[a-zA-Z-]+)         # pre-release label
-        (?P<pre_n>0|[1-9]\\d*)        # pre-release version number
-    )?                                # pre-release section is optional
-"""
-serialize = [
-    "{major}.{minor}.{patch}-{pre_l}{pre_n}",
-    "{major}.{minor}.{patch}",
-]
+current_version = "4.1.0"
+parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
+serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = true
 sign_tags = false
 tag_name = "v{new_version}"
```

### Comparing `bsb_yaml-4.0.0rc2/PKG-INFO` & `bsb_yaml-4.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: bsb-yaml
-Version: 4.0.0rc2
+Version: 4.1.0
 Summary: YAML parser for the BSB framework.
 Author-email: Robin De Schepper <robingilbert.deschepper@unipv.it>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Dist: bsb-core==4.0.0rc2
+Requires-Dist: bsb-core~=4.1
 Requires-Dist: PyYAML~=6.0
 Requires-Dist: pre-commit~=3.5 ; extra == "dev"
-Requires-Dist: black~=23.11 ; extra == "dev"
+Requires-Dist: black~=24.0 ; extra == "dev"
 Requires-Dist: isort~=5.12 ; extra == "dev"
 Requires-Dist: bump-my-version~=0.18 ; extra == "dev"
 Requires-Dist: bsb-core[parallel] ; extra == "test"
-Requires-Dist: bsb-test==4.0.0rc2 ; extra == "test"
+Requires-Dist: bsb-test~=4.0 ; extra == "test"
 Requires-Dist: coverage~=7.0 ; extra == "test"
 Provides-Extra: dev
 Provides-Extra: test
 
 # bsb-yaml
```

