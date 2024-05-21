# Comparing `tmp/django_xlsx_serializer-0.2.0.tar.gz` & `tmp/django_xlsx_serializer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_xlsx_serializer-0.2.0.tar", last modified: Thu May 16 20:33:29 2024, max compression
+gzip compressed data, was "django_xlsx_serializer-0.3.0.tar", last modified: Tue May 21 21:07:21 2024, max compression
```

## Comparing `django_xlsx_serializer-0.2.0.tar` & `django_xlsx_serializer-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:33:29.594145 django_xlsx_serializer-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-16 20:33:20.000000 django_xlsx_serializer-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-16 20:33:29.594145 django_xlsx_serializer-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-16 20:33:20.000000 django_xlsx_serializer-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-16 20:33:20.000000 django_xlsx_serializer-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:33:29.594145 django_xlsx_serializer-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:33:29.590145 django_xlsx_serializer-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:33:29.590145 django_xlsx_serializer-0.2.0/src/django_xlsx_serializer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-16 20:33:29.000000 django_xlsx_serializer-0.2.0/src/django_xlsx_serializer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-16 20:33:29.000000 django_xlsx_serializer-0.2.0/src/django_xlsx_serializer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:33:29.000000 django_xlsx_serializer-0.2.0/src/django_xlsx_serializer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-16 20:33:29.000000 django_xlsx_serializer-0.2.0/src/django_xlsx_serializer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 20:33:29.000000 django_xlsx_serializer-0.2.0/src/django_xlsx_serializer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:33:29.590145 django_xlsx_serializer-0.2.0/src/xlsx_serializer/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 20:33:20.000000 django_xlsx_serializer-0.2.0/src/xlsx_serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:33:20.000000 django_xlsx_serializer-0.2.0/src/xlsx_serializer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:07:21.329388 django_xlsx_serializer-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-21 21:07:07.000000 django_xlsx_serializer-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-05-21 21:07:21.329388 django_xlsx_serializer-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:07:21.325388 django_xlsx_serializer-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-05-21 21:07:07.000000 django_xlsx_serializer-0.3.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-21 21:07:07.000000 django_xlsx_serializer-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 21:07:21.329388 django_xlsx_serializer-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:07:21.325388 django_xlsx_serializer-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:07:21.329388 django_xlsx_serializer-0.3.0/src/django_xlsx_serializer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-05-21 21:07:21.000000 django_xlsx_serializer-0.3.0/src/django_xlsx_serializer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-21 21:07:21.000000 django_xlsx_serializer-0.3.0/src/django_xlsx_serializer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 21:07:21.000000 django_xlsx_serializer-0.3.0/src/django_xlsx_serializer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-21 21:07:21.000000 django_xlsx_serializer-0.3.0/src/django_xlsx_serializer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 21:07:21.000000 django_xlsx_serializer-0.3.0/src/django_xlsx_serializer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:07:21.329388 django_xlsx_serializer-0.3.0/src/xlsx_serializer/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-21 21:07:07.000000 django_xlsx_serializer-0.3.0/src/xlsx_serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-21 21:07:07.000000 django_xlsx_serializer-0.3.0/src/xlsx_serializer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15106 2024-05-21 21:07:07.000000 django_xlsx_serializer-0.3.0/src/xlsx_serializer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 21:07:07.000000 django_xlsx_serializer-0.3.0/src/xlsx_serializer/py.typed
```

### Comparing `django_xlsx_serializer-0.2.0/LICENSE` & `django_xlsx_serializer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_xlsx_serializer-0.2.0/pyproject.toml` & `django_xlsx_serializer-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -5,30 +5,29 @@
 # Project metadata
 # https://packaging.python.org/en/latest/specifications/pyproject-toml/
 
 [project]
 name = "django-xlsx-serializer"
 dependencies = [
   "django >= 3.2, < 5.1",
+  "openpyxl < 4",
   "typing-extensions < 5",
 ]
 requires-python = ">= 3.9"
 authors = [
   { name = "Kamil Paduszyński", email = "92403542+paduszyk@users.noreply.github.com" },
 ]
-description = "Load/dump Django models from/to Excel 2003+ workbooks"
-readme = "README.md"
+description = "Load/dump Django models from/to Excel 2007+ workbooks"
+readme = "docs/README.md"
 keywords = [
   "django",
   "django-application",
   "excel",
   "excel-export",
   "excel-import",
-  "openpyxl",
-  "xlsx",
 ]
 classifiers = [
   "Environment :: Web Environment",
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
@@ -52,62 +51,65 @@
 "Repository" = "https://github.com/paduszyk/django-xlsx-serializer"
 "Documentation" = "https://github.com/paduszyk/django-xlsx-serializer#readme"
 "Issue tracker" = "https://github.com/paduszyk/django-xlsx-serializer/issues"
 
 [project.optional-dependencies]
 dev = [
   "django-stubs[compatible-mypy] < 6",
-  "commitizen < 4",
+  "nox",
   "pre-commit < 4",
   "pytest < 9",
   "pytest-cov < 6",
   "pytest-django < 5",
   "pytest-custom-exit-code < 1",
   "psycopg2-binary < 3",
   "python-dotenv < 2",
   "ruff < 1",
+  "types-openpyxl < 4",
 ]
 
 # Setuptools
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 
 [tool.setuptools.dynamic]
 version = { attr = "xlsx_serializer.__version__" }
 
 # Commitizen
 # https://commitizen-tools.github.io/commitizen/config/
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version_provider = "scm"
-version_scheme = "pep440"
 version_files = [
   "src/xlsx_serializer/__init__.py:__version__",
 ]
+version_provider = "scm"
 tag_format = "v$version"
-annotated_tag = true
-bump_message = "chore(release): $current_version → $new_version"
+bump_message = "chore(release): version $current_version → $new_version [skip ci]"
 
 # Ruff
 # https://docs.astral.sh/ruff/configuration/
 # https://docs.astral.sh/ruff/rules/
 # https://docs.astral.sh/ruff/settings/
 
 [tool.ruff]
 target-version = "py39"
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = ["ANN", "D"]
 
 [tool.ruff.lint.per-file-ignores]
+"scripts/**/*.py" = ["INP"]
 "tests/**/*.py" = ["ARG", "DJ", "E501", "FBT", "PLR2004", "S101"]
 
 [tool.ruff.lint.isort]
 known-first-party = ["xlsx_serializer"]
+required-imports = [
+  "from __future__ import annotations",
+]
 section-order = [
   "future",
   "standard-library",
   "third-party",
   "django",
   "first-party",
   "tests",
@@ -135,20 +137,22 @@
 strict = true
 plugins = [
   "mypy_django_plugin.main",
 ]
 
 [[tool.mypy.overrides]]
 module = [
+  "nox",
   "pytest",
 ]
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = [
+  "noxfile",
   "tests.*",
 ]
 disallow_untyped_decorators = false
 
 # Django-stubs
 # https://github.com/typeddjango/django-stubs
```

