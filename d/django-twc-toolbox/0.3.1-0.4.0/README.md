# Comparing `tmp/django_twc_toolbox-0.3.1.tar.gz` & `tmp/django_twc_toolbox-0.4.0.tar.gz`

## Comparing `django_twc_toolbox-0.3.1.tar` & `django_twc_toolbox-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/RELEASING.md
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/noxfile.py
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/docs/conf.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/docs/index.md
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/docs/_static/css/custom.css
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/docs/development/just.md
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/src/django_twc_toolbox/__init__.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/src/django_twc_toolbox/apps.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/src/django_twc_toolbox/models.py
--rw-r--r--   0        0        0    10715 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/src/django_twc_toolbox/paginator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/src/django_twc_toolbox/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/tests/settings.py
--rw-r--r--   0        0        0    30152 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/tests/test_paginator.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/tests/dummy/__init__.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/tests/dummy/models.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/.gitignore
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/AUTHORS.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/LICENSE
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/README.md
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/RELEASING.md
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/noxfile.py
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/docs/conf.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/docs/index.md
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/docs/development/just.md
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/src/django_twc_toolbox/__init__.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/src/django_twc_toolbox/apps.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/src/django_twc_toolbox/fields.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/src/django_twc_toolbox/models.py
+-rw-r--r--   0        0        0    10715 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/src/django_twc_toolbox/paginator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/src/django_twc_toolbox/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/tests/settings.py
+-rw-r--r--   0        0        0    30152 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/tests/test_paginator.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/tests/dummy/__init__.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/tests/dummy/models.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/.gitignore
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/AUTHORS.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/LICENSE
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/README.md
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 django_twc_toolbox-0.4.0/PKG-INFO
```

### Comparing `django_twc_toolbox-0.3.1/CHANGELOG.md` & `django_twc_toolbox-0.4.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,24 @@
 ### Fixed - for any bug fixes
 ### Security - in case of vulnerabilities
 [${version}]: https://github.com/westerveltco/django-twc-toolbox/releases/tag/v${version}
 -->
 
 ## [Unreleased]
 
+## [0.4.0]
+
+### Added
+
+-   Added a `CuidField` and extra dependencies needed to use it. Install the package with `django-twc-toolbox[cuid]` in order to use it.
+
+### Removed
+
+-   Dropped support for Django 3.2 (EOL April 2024).
+
 ## [0.3.1]
 
 ### Added
 
 -   `py.typed` added to the project.
 
 ### Changed
@@ -72,13 +82,14 @@
 -   Initial CI/CD (GitHub Actions).
 -   A `TimeStamped` abstract model for adding `created_at` and `updated_at` fields to models.
 
 ### New Contributors
 
 -   Josh Thomas <josh@joshthomas.dev> (maintainer)
 
-[unreleased]: https://github.com/westerveltco/django-twc-toolbox/compare/v0.3.1...HEAD
+[unreleased]: https://github.com/westerveltco/django-twc-toolbox/compare/v0.4.0...HEAD
 [0.2.1]: https://github.com/westerveltco/django-twc-toolbox/releases/tag/v0.2.1
 [0.2.0]: https://github.com/westerveltco/django-twc-toolbox/releases/tag/v0.2.0
 [0.1.1]: https://github.com/westerveltco/django-twc-toolbox/releases/tag/v0.1.1
 [0.3.0]: https://github.com/westerveltco/django-twc-toolbox.git/releases/tag/v0.3.0
 [0.3.1]: https://github.com/westerveltco/django-twc-toolbox/releases/tag/v0.3.1
+[0.4.0]: https://github.com/westerveltco/django-twc-toolbox/releases/tag/v0.4.0
```

### Comparing `django_twc_toolbox-0.3.1/CONTRIBUTING.md` & `django_twc_toolbox-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.1/RELEASING.md` & `django_twc_toolbox-0.4.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.1/noxfile.py` & `django_twc_toolbox-0.4.0/noxfile.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,21 +13,20 @@
 PY310 = "3.10"
 PY311 = "3.11"
 PY312 = "3.12"
 PY_VERSIONS = [PY38, PY39, PY310, PY311, PY312]
 PY_DEFAULT = PY_VERSIONS[0]
 PY_LATEST = PY_VERSIONS[-1]
 
-DJ32 = "3.2"
 DJ42 = "4.2"
 DJ50 = "5.0"
 DJMAIN = "main"
 DJMAIN_MIN_PY = PY310
-DJ_VERSIONS = [DJ32, DJ42, DJ50, DJMAIN]
-DJ_LTS = [DJ32, DJ42]
+DJ_VERSIONS = [DJ42, DJ50, DJMAIN]
+DJ_LTS = [DJ42]
 DJ_DEFAULT = DJ_LTS[0]
 DJ_LATEST = DJ_VERSIONS[-2]
 
 
 def version(ver: str) -> tuple[int, ...]:
     """Convert a string version to a tuple of ints, e.g. "3.10" -> (3, 10)"""
     return tuple(map(int, ver.split(".")))
@@ -36,18 +35,14 @@
 def should_skip(python: str, django: str) -> bool:
     """Return True if the test should be skipped"""
 
     if django == DJMAIN and version(python) < version(DJMAIN_MIN_PY):
         # Django main requires Python 3.10+
         return True
 
-    if django == DJ32 and version(python) >= version(PY312):
-        # Django 3.2 requires Python < 3.12
-        return True
-
     if django == DJ50 and version(python) < version(PY310):
         # Django 5.0 requires Python 3.10+
         return True
 
     return False
```

### Comparing `django_twc_toolbox-0.3.1/docs/conf.py` & `django_twc_toolbox-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.1/docs/development/just.md` & `django_twc_toolbox-0.4.0/docs/development/just.md`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.1/src/django_twc_toolbox/models.py` & `django_twc_toolbox-0.4.0/src/django_twc_toolbox/models.py`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.1/src/django_twc_toolbox/paginator.py` & `django_twc_toolbox-0.4.0/src/django_twc_toolbox/paginator.py`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.1/tests/settings.py` & `django_twc_toolbox-0.4.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.1/tests/test_paginator.py` & `django_twc_toolbox-0.4.0/tests/test_paginator.py`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.1/.gitignore` & `django_twc_toolbox-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.1/LICENSE` & `django_twc_toolbox-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.1/README.md` & `django_twc_toolbox-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # django-twc-toolbox
 
 [![PyPI](https://img.shields.io/pypi/v/django-twc-toolbox)](https://pypi.org/project/django-twc-toolbox/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-twc-toolbox)
-![Django Version](https://img.shields.io/badge/django-3.2%20%7C%204.2%20%7C%205.0-%2344B78B?labelColor=%23092E20)
+![Django Version](https://img.shields.io/badge/django-4.2%20%7C%205.0-%2344B78B?labelColor=%23092E20)
 <!-- https://shields.io/badges -->
-<!-- django-3.2 | 4.2 | 5.0-#44B78B -->
+<!-- django-4.2 | 5.0-#44B78B -->
 <!-- labelColor=%23092E20 -->
 
 ## Requirements
 
 - Python 3.8, 3.9, 3.10, 3.11, 3.12
-- Django 3.2, 4.2, 5.0
+- Django 4.2, 5.0
 
 ## Getting Started
 
 1. Install the package from PyPI:
 
 ```bash
 python -m pip install django-twc-toolbox
```

### Comparing `django_twc_toolbox-0.3.1/pyproject.toml` & `django_twc_toolbox-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
-authors = [
-  {name = "Josh Thomas", email = "josh@joshthomas.dev"}
-]
+authors = [{name = "Josh Thomas", email = "josh@joshthomas.dev"}]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Framework :: Django",
-  "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.2",
   "Framework :: Django :: 5.0",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython"
 ]
-dependencies = [
-  "django>=3.2"
-]
+dependencies = ["django>=4.2"]
 description = "Various tools for Django projects at The Westervelt Company."
 dynamic = ["version"]
 keywords = []
 license = {file = "LICENSE"}
 name = "django-twc-toolbox"
 readme = "README.md"
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
+cuid = ["cuid", "django-charid-field"]
 dev = [
   "bumpver",
   "copier",
   "copier-templates-extensions",
   "coverage[toml]",
   "django-stubs",
   "django-stubs-ext",
@@ -70,29 +66,23 @@
 Documentation = "https://django-twc-toolbox.westervelt.dev/"
 Issues = "https://github.com/westerveltco/django-twc-toolbox/issues"
 Source = "https://github.com/westerveltco/django-twc-toolbox"
 
 [tool.bumpver]
 commit = true
 commit_message = ":bookmark: bump version {old_version} -> {new_version}"
-current_version = "0.3.1"
+current_version = "0.4.0"
 push = false  # set to false for CI
 tag = false
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 
 [tool.bumpver.file_patterns]
-".copier/package.yml" = [
-  'current_version: {version}'
-]
-"src/django_twc_toolbox/__init__.py" = [
-  '__version__ = "{version}"'
-]
-"tests/test_version.py" = [
-  'assert __version__ == "{version}"'
-]
+".copier/package.yml" = ['current_version: {version}']
+"src/django_twc_toolbox/__init__.py" = ['__version__ = "{version}"']
+"tests/test_version.py" = ['assert __version__ == "{version}"']
 
 [tool.coverage.paths]
 source = ["src"]
 
 [tool.coverage.report]
 exclude_lines = [
   "pragma: no cover",
@@ -101,58 +91,51 @@
   "if settings.DEBUG:",
   "if TYPE_CHECKING:",
   'def __str__\(self\)\s?\-?\>?\s?\w*\:'
 ]
 fail_under = 75
 
 [tool.coverage.run]
-omit = [
-  "src/django_twc_toolbox/migrations/*",
-  "tests/*"
-]
+omit = ["src/django_twc_toolbox/migrations/*", "tests/*"]
 source = ["django_twc_toolbox"]
 
 [tool.django-stubs]
 django_settings_module = "tests.settings"
 strict_settings = false
 
 [tool.djlint]
 indent = 2
 
 [tool.hatch.build]
-exclude = [
-  ".*",
-  "Justfile"
-]
+exclude = [".*", "Justfile"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/django_twc_toolbox"]
 
 [tool.hatch.version]
 path = "src/django_twc_toolbox/__init__.py"
 
 [tool.mypy]
 check_untyped_defs = true
 exclude = "docs/.*\\.py$"
 mypy_path = "src/"
 no_implicit_optional = true
-plugins = [
-  "mypy_django_plugin.main"
-]
+plugins = ["mypy_django_plugin.main"]
 warn_redundant_casts = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
 ignore_errors = true
 ignore_missing_imports = true
-module = [
-  "django_twc_toolbox.*.migrations.*",
-  "tests.*"
-]
+module = ["django_twc_toolbox.*.migrations.*", "tests.*"]
+
+[[tool.mypy.overrides]]
+ignore_missing_imports = true
+module = ["charidfield.*", "cuid.*"]
 
 [tool.mypy_django_plugin]
 ignore_missing_model_attributes = true
 
 [tool.pytest.ini_options]
 addopts = "--create-db -n auto --dist loadfile --doctest-modules"
 django_find_project = false
```

### Comparing `django_twc_toolbox-0.3.1/PKG-INFO` & `django_twc_toolbox-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-twc-toolbox
-Version: 0.3.1
+Version: 0.4.0
 Summary: Various tools for Django projects at The Westervelt Company.
 Project-URL: Documentation, https://django-twc-toolbox.westervelt.dev/
 Project-URL: Issues, https://github.com/westerveltco/django-twc-toolbox/issues
 Project-URL: Source, https://github.com/westerveltco/django-twc-toolbox
 Author-email: Josh Thomas <josh@joshthomas.dev>
 License: MIT License
         
@@ -15,30 +15,32 @@
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 License-File: AUTHORS.md
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
-Requires-Dist: django>=3.2
+Requires-Dist: django>=4.2
+Provides-Extra: cuid
+Requires-Dist: cuid; extra == 'cuid'
+Requires-Dist: django-charid-field; extra == 'cuid'
 Provides-Extra: dev
 Requires-Dist: bumpver; extra == 'dev'
 Requires-Dist: copier; extra == 'dev'
 Requires-Dist: copier-templates-extensions; extra == 'dev'
 Requires-Dist: coverage[toml]; extra == 'dev'
 Requires-Dist: django-stubs; extra == 'dev'
 Requires-Dist: django-stubs-ext; extra == 'dev'
@@ -65,23 +67,23 @@
 Requires-Dist: pre-commit; extra == 'lint'
 Description-Content-Type: text/markdown
 
 # django-twc-toolbox
 
 [![PyPI](https://img.shields.io/pypi/v/django-twc-toolbox)](https://pypi.org/project/django-twc-toolbox/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-twc-toolbox)
-![Django Version](https://img.shields.io/badge/django-3.2%20%7C%204.2%20%7C%205.0-%2344B78B?labelColor=%23092E20)
+![Django Version](https://img.shields.io/badge/django-4.2%20%7C%205.0-%2344B78B?labelColor=%23092E20)
 <!-- https://shields.io/badges -->
-<!-- django-3.2 | 4.2 | 5.0-#44B78B -->
+<!-- django-4.2 | 5.0-#44B78B -->
 <!-- labelColor=%23092E20 -->
 
 ## Requirements
 
 - Python 3.8, 3.9, 3.10, 3.11, 3.12
-- Django 3.2, 4.2, 5.0
+- Django 4.2, 5.0
 
 ## Getting Started
 
 1. Install the package from PyPI:
 
 ```bash
 python -m pip install django-twc-toolbox
```

