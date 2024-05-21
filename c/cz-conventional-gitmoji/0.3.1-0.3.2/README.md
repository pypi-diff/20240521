# Comparing `tmp/cz_conventional_gitmoji-0.3.1.tar.gz` & `tmp/cz_conventional_gitmoji-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cz_conventional_gitmoji-0.3.1.tar", max compression
+gzip compressed data, was "cz_conventional_gitmoji-0.3.2.tar", max compression
```

## Comparing `cz_conventional_gitmoji-0.3.1.tar` & `cz_conventional_gitmoji-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2625 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/README.md
--rw-r--r--   0        0        0     2554 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/cz_gitmoji/__init__.py
--rw-r--r--   0        0        0     1285 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/cz_gitmoji/conventional_gitmojis_info.txt
--rw-r--r--   0        0        0    13467 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/cz_gitmoji/main.py
--rw-r--r--   0        0        0        0 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/cz_gitmoji/py.typed
--rw-r--r--   0        0        0        0 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/gitmojify/__init__.py
--rw-r--r--   0        0        0     1687 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/gitmojify/mojify.py
--rw-r--r--   0        0        0        0 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/gitmojify/py.typed
--rw-r--r--   0        0        0        0 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/shared/__init__.py
--rw-r--r--   0        0        0     2701 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/shared/gitmojis.py
--rw-r--r--   0        0        0      406 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/shared/model.py
--rw-r--r--   0        0        0        0 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/shared/py.typed
--rw-r--r--   0        0        0    10765 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/shared/spec.py
--rw-r--r--   0        0        0      817 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/shared/utils.py
--rw-r--r--   0        0        0     3569 1970-01-01 00:00:00.000000 cz_conventional_gitmoji-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2625 2024-05-21 19:17:19.423428 cz_conventional_gitmoji-0.3.2/README.md
+-rw-r--r--   0        0        0     2554 2024-05-21 19:17:19.423428 cz_conventional_gitmoji-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-21 19:17:19.423428 cz_conventional_gitmoji-0.3.2/src/cz_gitmoji/__init__.py
+-rw-r--r--   0        0        0     1285 2024-05-21 19:17:19.423428 cz_conventional_gitmoji-0.3.2/src/cz_gitmoji/conventional_gitmojis_info.txt
+-rw-r--r--   0        0        0    13892 2024-05-21 19:17:19.423428 cz_conventional_gitmoji-0.3.2/src/cz_gitmoji/main.py
+-rw-r--r--   0        0        0        0 2024-05-21 19:17:19.423428 cz_conventional_gitmoji-0.3.2/src/cz_gitmoji/py.typed
+-rw-r--r--   0        0        0        0 2024-05-21 19:17:19.423428 cz_conventional_gitmoji-0.3.2/src/gitmojify/__init__.py
+-rw-r--r--   0        0        0     1687 2024-05-21 19:17:19.423428 cz_conventional_gitmoji-0.3.2/src/gitmojify/mojify.py
+-rw-r--r--   0        0        0        0 2024-05-21 19:17:19.423428 cz_conventional_gitmoji-0.3.2/src/gitmojify/py.typed
+-rw-r--r--   0        0        0        0 2024-05-21 19:17:19.423428 cz_conventional_gitmoji-0.3.2/src/shared/__init__.py
+-rw-r--r--   0        0        0     2701 2024-05-21 19:17:19.423428 cz_conventional_gitmoji-0.3.2/src/shared/gitmojis.py
+-rw-r--r--   0        0        0      406 2024-05-21 19:17:19.423428 cz_conventional_gitmoji-0.3.2/src/shared/model.py
+-rw-r--r--   0        0        0        0 2024-05-21 19:17:19.423428 cz_conventional_gitmoji-0.3.2/src/shared/py.typed
+-rw-r--r--   0        0        0    10765 2024-05-21 19:17:19.423428 cz_conventional_gitmoji-0.3.2/src/shared/spec.py
+-rw-r--r--   0        0        0      817 2024-05-21 19:17:19.423428 cz_conventional_gitmoji-0.3.2/src/shared/utils.py
+-rw-r--r--   0        0        0     3569 1970-01-01 00:00:00.000000 cz_conventional_gitmoji-0.3.2/PKG-INFO
```

### Comparing `cz_conventional_gitmoji-0.3.1/README.md` & `cz_conventional_gitmoji-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.3.1/pyproject.toml` & `cz_conventional_gitmoji-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cz-conventional-gitmoji"
-version = "0.3.1"
+version = "0.3.2"
 description = "A commitizen plugin that combines gitmoji and conventional."
 authors = ["ljnsn <82611987+ljnsn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "shared", from = "src" },
   { include = "cz_gitmoji", from = "src" },
@@ -30,15 +30,15 @@
 coverage = { extras = ["toml"], version = ">=7.0.1" }
 ruff = ">=0.3.7"
 mypy = ">=1.3.0"
 pre-commit = ">=2.0"
 
 [tool.commitizen]
 name = "cz_gitmoji"
-version = "0.3.1"
+version = "0.3.2"
 bump_message = "🔖 bump(release): v$current_version → v$new_version"
 tag_format = "v$version"
 version_files = ["pyproject.toml:^version"]
 update_changelog_on_bump = true
 
 [tool.ruff]
 fix = true
```

### Comparing `cz_conventional_gitmoji-0.3.1/src/cz_gitmoji/conventional_gitmojis_info.txt` & `cz_conventional_gitmoji-0.3.2/src/cz_gitmoji/conventional_gitmojis_info.txt`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.3.1/src/cz_gitmoji/main.py` & `cz_conventional_gitmoji-0.3.2/src/cz_gitmoji/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,26 @@
             (rf"^{GJ_FEAT}? ?feat", MINOR),
             (rf"^{GJ_FIX}? ?fix", PATCH),
             (rf"^{GJ_HOTFIX}? ?hotfix", PATCH),
             (rf"^{GJ_REFACTOR}? ?refactor", PATCH),
             (rf"^{GJ_PERF}? ?perf", PATCH),
         )
     )
+    bump_map_major_version_zero = OrderedDict(
+        (
+            (r"^.+!$", MINOR),
+            (r"^BREAKING[\-\ ]CHANGE", MINOR),
+            (rf"^{GJ_BOOM}? ?boom", MINOR),
+            (rf"^{GJ_FEAT}? ?feat", MINOR),
+            (rf"^{GJ_FIX}? ?fix", PATCH),
+            (rf"^{GJ_HOTFIX}? ?hotfix", PATCH),
+            (rf"^{GJ_REFACTOR}? ?refactor", PATCH),
+            (rf"^{GJ_PERF}? ?perf", PATCH),
+        )
+    )
     # parse information for generating the change log
     commit_parser = (
         rf"^(?P<change_type>{utils.get_type_group_pattern()}|BREAKING CHANGE)"
         r"(?:\((?P<scope>[^()\r\n]*)\)|\()?(?P<breaking>!)?:\s(?P<message>.*)?"
     )
     # exclude from changelog
     changelog_pattern = (
```

### Comparing `cz_conventional_gitmoji-0.3.1/src/gitmojify/mojify.py` & `cz_conventional_gitmoji-0.3.2/src/gitmojify/mojify.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.3.1/src/shared/gitmojis.py` & `cz_conventional_gitmoji-0.3.2/src/shared/gitmojis.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.3.1/src/shared/spec.py` & `cz_conventional_gitmoji-0.3.2/src/shared/spec.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.3.1/src/shared/utils.py` & `cz_conventional_gitmoji-0.3.2/src/shared/utils.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.3.1/PKG-INFO` & `cz_conventional_gitmoji-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cz-conventional-gitmoji
-Version: 0.3.1
+Version: 0.3.2
 Summary: A commitizen plugin that combines gitmoji and conventional.
 Home-page: https://github.com/ljnsn/cz-conventional-gitmoji
 License: MIT
 Author: ljnsn
 Author-email: 82611987+ljnsn@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

