# Comparing `tmp/sphinx_notfound_page-1.0.0.tar.gz` & `tmp/sphinx_notfound_page-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_notfound_page-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_notfound_page-1.0.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_notfound_page-1.0.0.tar` & `sphinx_notfound_page-1.0.0rc1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.0/.eslintrc -> common/eslintrc
-lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.254299 sphinx_notfound_page-1.0.0/.flake8 -> common/flake8
--rw-r--r--   0        0        0       81 2019-07-30 11:28:47.437314 sphinx_notfound_page-1.0.0/.gitmodules
-lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.0/.isort.cfg -> common/isort.cfg
-lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.0/.pep8 -> common/pep8
-lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.0/.pre-commit-config.yaml -> common/pre-commit-config.yaml
--rw-r--r--   0        0        0    11109 2023-08-30 11:31:20.498545 sphinx_notfound_page-1.0.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1072 2019-01-19 11:32:01.424634 sphinx_notfound_page-1.0.0/LICENSE
--rw-r--r--   0        0        0     1362 2021-04-25 19:00:36.924124 sphinx_notfound_page-1.0.0/README.rst
--rw-r--r--   0        0        0    34339 2022-08-29 15:03:35.625028 sphinx_notfound_page-1.0.0/docs/404-using-this-extension.png
--rw-r--r--   0        0        0    38048 2022-08-29 15:00:24.433754 sphinx_notfound_page-1.0.0/docs/404-without-this-extension.png
--rw-r--r--   0        0        0      216 2021-04-25 19:00:36.924124 sphinx_notfound_page-1.0.0/docs/404.rst
--rw-r--r--   0        0        0      580 2019-05-25 10:54:48.008540 sphinx_notfound_page-1.0.0/docs/Makefile
--rw-r--r--   0        0        0    68168 2022-07-18 16:56:36.852748 sphinx_notfound_page-1.0.0/docs/_static/who-is-using-it/docs.carpentries.org.png
--rw-r--r--   0        0        0    64437 2022-07-18 17:13:57.944284 sphinx_notfound_page-1.0.0/docs/_static/who-is-using-it/docs.jina.ai.png
--rw-r--r--   0        0        0    24679 2022-07-18 16:53:01.545428 sphinx_notfound_page-1.0.0/docs/_static/who-is-using-it/docs.pyvista.org.png
--rw-r--r--   0        0        0    87647 2022-07-18 16:50:44.183555 sphinx_notfound_page-1.0.0/docs/_static/who-is-using-it/docs.readthedocs.io.png
--rw-r--r--   0        0        0    55341 2022-07-18 16:58:38.521142 sphinx_notfound_page-1.0.0/docs/_static/who-is-using-it/www.attrs.org.png
--rw-r--r--   0        0        0    59498 2022-07-18 17:20:20.270689 sphinx_notfound_page-1.0.0/docs/_static/who-is-using-it/www.nengo.ai.png
--rw-r--r--   0        0        0    74477 2022-07-18 16:55:10.520497 sphinx_notfound_page-1.0.0/docs/_static/who-is-using-it/www.writethedocs.org.png
--rw-r--r--   0        0        0     5483 2023-08-24 13:36:06.694482 sphinx_notfound_page-1.0.0/docs/conf.py
--rw-r--r--   0        0        0     1941 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.0/docs/configuration.rst
--rw-r--r--   0        0        0     2135 2022-06-29 10:10:02.805104 sphinx_notfound_page-1.0.0/docs/faq.rst
--rw-r--r--   0        0        0      495 2019-07-30 11:28:47.437314 sphinx_notfound_page-1.0.0/docs/get-involved.rst
--rw-r--r--   0        0        0     2010 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.0/docs/how-it-works.rst
--rw-r--r--   0        0        0     2663 2023-08-23 13:37:32.431949 sphinx_notfound_page-1.0.0/docs/index.rst
--rw-r--r--   0        0        0     1450 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.0/docs/installation.rst
--rw-r--r--   0        0        0    13265 2019-06-11 09:36:10.430735 sphinx_notfound_page-1.0.0/docs/loudly-crying-face.png
--rw-r--r--   0        0        0     1964 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.0/docs/requirements.txt
--rw-r--r--   0        0        0     2715 2022-07-18 17:25:35.491222 sphinx_notfound_page-1.0.0/docs/who-is-using-it.rst
--rw-r--r--   0        0        0       22 2023-08-30 11:32:45.698000 sphinx_notfound_page-1.0.0/notfound/__init__.py
--rw-r--r--   0        0        0    12078 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.0/notfound/extension.py
--rw-r--r--   0        0        0     3028 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.0/notfound/utils.py
-lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.0/prospector.yml -> common/prospector.yml
--rw-r--r--   0        0        0     2011 2023-08-30 11:32:45.688000 sphinx_notfound_page-1.0.0/pyproject.toml
-lrwxr-xr-x   0        0        0        0 2023-08-24 09:58:45.126657 sphinx_notfound_page-1.0.0/tasks.py -> common/tasks.py
--rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 sphinx_notfound_page-1.0.0/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.0rc1/.eslintrc -> common/eslintrc
+lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.254299 sphinx_notfound_page-1.0.0rc1/.flake8 -> common/flake8
+-rw-r--r--   0        0        0       81 2019-07-30 11:28:47.437314 sphinx_notfound_page-1.0.0rc1/.gitmodules
+lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.0rc1/.isort.cfg -> common/isort.cfg
+lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.0rc1/.pep8 -> common/pep8
+lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.0rc1/.pre-commit-config.yaml -> common/pre-commit-config.yaml
+-rw-r--r--   0        0        0    11055 2023-08-24 13:54:09.793288 sphinx_notfound_page-1.0.0rc1/CHANGELOG.rst
+-rw-r--r--   0        0        0     1072 2019-01-19 11:32:01.424634 sphinx_notfound_page-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     1362 2021-04-25 19:00:36.924124 sphinx_notfound_page-1.0.0rc1/README.rst
+-rw-r--r--   0        0        0    34339 2022-08-29 15:03:35.625028 sphinx_notfound_page-1.0.0rc1/docs/404-using-this-extension.png
+-rw-r--r--   0        0        0    38048 2022-08-29 15:00:24.433754 sphinx_notfound_page-1.0.0rc1/docs/404-without-this-extension.png
+-rw-r--r--   0        0        0      216 2021-04-25 19:00:36.924124 sphinx_notfound_page-1.0.0rc1/docs/404.rst
+-rw-r--r--   0        0        0      580 2019-05-25 10:54:48.008540 sphinx_notfound_page-1.0.0rc1/docs/Makefile
+-rw-r--r--   0        0        0    68168 2022-07-18 16:56:36.852748 sphinx_notfound_page-1.0.0rc1/docs/_static/who-is-using-it/docs.carpentries.org.png
+-rw-r--r--   0        0        0    64437 2022-07-18 17:13:57.944284 sphinx_notfound_page-1.0.0rc1/docs/_static/who-is-using-it/docs.jina.ai.png
+-rw-r--r--   0        0        0    24679 2022-07-18 16:53:01.545428 sphinx_notfound_page-1.0.0rc1/docs/_static/who-is-using-it/docs.pyvista.org.png
+-rw-r--r--   0        0        0    87647 2022-07-18 16:50:44.183555 sphinx_notfound_page-1.0.0rc1/docs/_static/who-is-using-it/docs.readthedocs.io.png
+-rw-r--r--   0        0        0    55341 2022-07-18 16:58:38.521142 sphinx_notfound_page-1.0.0rc1/docs/_static/who-is-using-it/www.attrs.org.png
+-rw-r--r--   0        0        0    59498 2022-07-18 17:20:20.270689 sphinx_notfound_page-1.0.0rc1/docs/_static/who-is-using-it/www.nengo.ai.png
+-rw-r--r--   0        0        0    74477 2022-07-18 16:55:10.520497 sphinx_notfound_page-1.0.0rc1/docs/_static/who-is-using-it/www.writethedocs.org.png
+-rw-r--r--   0        0        0     5483 2023-08-24 13:36:06.694482 sphinx_notfound_page-1.0.0rc1/docs/conf.py
+-rw-r--r--   0        0        0     1941 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.0rc1/docs/configuration.rst
+-rw-r--r--   0        0        0     2135 2022-06-29 10:10:02.805104 sphinx_notfound_page-1.0.0rc1/docs/faq.rst
+-rw-r--r--   0        0        0      495 2019-07-30 11:28:47.437314 sphinx_notfound_page-1.0.0rc1/docs/get-involved.rst
+-rw-r--r--   0        0        0     2010 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.0rc1/docs/how-it-works.rst
+-rw-r--r--   0        0        0     2663 2023-08-23 13:37:32.431949 sphinx_notfound_page-1.0.0rc1/docs/index.rst
+-rw-r--r--   0        0        0     1450 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.0rc1/docs/installation.rst
+-rw-r--r--   0        0        0    13265 2019-06-11 09:36:10.430735 sphinx_notfound_page-1.0.0rc1/docs/loudly-crying-face.png
+-rw-r--r--   0        0        0     1964 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.0rc1/docs/requirements.txt
+-rw-r--r--   0        0        0     2715 2022-07-18 17:25:35.491222 sphinx_notfound_page-1.0.0rc1/docs/who-is-using-it.rst
+-rw-r--r--   0        0        0       25 2023-08-24 13:59:53.207841 sphinx_notfound_page-1.0.0rc1/notfound/__init__.py
+-rw-r--r--   0        0        0    12078 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.0rc1/notfound/extension.py
+-rw-r--r--   0        0        0     3028 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.0rc1/notfound/utils.py
+lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.0rc1/prospector.yml -> common/prospector.yml
+-rw-r--r--   0        0        0     2017 2023-08-24 13:59:53.207841 sphinx_notfound_page-1.0.0rc1/pyproject.toml
+lrwxr-xr-x   0        0        0        0 2023-08-24 09:58:45.126657 sphinx_notfound_page-1.0.0rc1/tasks.py -> common/tasks.py
+-rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 sphinx_notfound_page-1.0.0rc1/PKG-INFO
```

### Comparing `sphinx_notfound_page-1.0.0/CHANGELOG.rst` & `sphinx_notfound_page-1.0.0rc1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 Changelog
 =========
 
 
-Version 1.0.0
--------------
-
-:Date: August 30, 2023
-
-
 Version 1.0.0rc0
 ----------------
 
 :Date: August 24, 2023
 
 * Add support for Sphinx 7.x
 * Drop support for older versions of Sphinx. Currently, only Sphinx>=5 is tested and supported.
```

### Comparing `sphinx_notfound_page-1.0.0/LICENSE` & `sphinx_notfound_page-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/README.rst` & `sphinx_notfound_page-1.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/404-using-this-extension.png` & `sphinx_notfound_page-1.0.0rc1/docs/404-using-this-extension.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/404-without-this-extension.png` & `sphinx_notfound_page-1.0.0rc1/docs/404-without-this-extension.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/Makefile` & `sphinx_notfound_page-1.0.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/_static/who-is-using-it/docs.carpentries.org.png` & `sphinx_notfound_page-1.0.0rc1/docs/_static/who-is-using-it/docs.carpentries.org.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/_static/who-is-using-it/docs.jina.ai.png` & `sphinx_notfound_page-1.0.0rc1/docs/_static/who-is-using-it/docs.jina.ai.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/_static/who-is-using-it/docs.pyvista.org.png` & `sphinx_notfound_page-1.0.0rc1/docs/_static/who-is-using-it/docs.pyvista.org.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/_static/who-is-using-it/docs.readthedocs.io.png` & `sphinx_notfound_page-1.0.0rc1/docs/_static/who-is-using-it/docs.readthedocs.io.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/_static/who-is-using-it/www.attrs.org.png` & `sphinx_notfound_page-1.0.0rc1/docs/_static/who-is-using-it/www.attrs.org.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/_static/who-is-using-it/www.nengo.ai.png` & `sphinx_notfound_page-1.0.0rc1/docs/_static/who-is-using-it/www.nengo.ai.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/_static/who-is-using-it/www.writethedocs.org.png` & `sphinx_notfound_page-1.0.0rc1/docs/_static/who-is-using-it/www.writethedocs.org.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/conf.py` & `sphinx_notfound_page-1.0.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/configuration.rst` & `sphinx_notfound_page-1.0.0rc1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/faq.rst` & `sphinx_notfound_page-1.0.0rc1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/how-it-works.rst` & `sphinx_notfound_page-1.0.0rc1/docs/how-it-works.rst`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/index.rst` & `sphinx_notfound_page-1.0.0rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/installation.rst` & `sphinx_notfound_page-1.0.0rc1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/loudly-crying-face.png` & `sphinx_notfound_page-1.0.0rc1/docs/loudly-crying-face.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/requirements.txt` & `sphinx_notfound_page-1.0.0rc1/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/docs/who-is-using-it.rst` & `sphinx_notfound_page-1.0.0rc1/docs/who-is-using-it.rst`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/notfound/extension.py` & `sphinx_notfound_page-1.0.0rc1/notfound/extension.py`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/notfound/utils.py` & `sphinx_notfound_page-1.0.0rc1/notfound/utils.py`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.0/pyproject.toml` & `sphinx_notfound_page-1.0.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "page",
     "sphinx",
     "documentation",
 ]
 dependencies = [
     "sphinx>=5",
 ]
-version = "1.0.0"
+version = "1.0.0rc1"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Sphinx",
     "Framework :: Sphinx :: Extension",
@@ -69,15 +69,15 @@
   ".readthedocs.yml",
   "pytest.ini",
   "conftest.py",
   "tox.ini",
 ]
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.0.0rc1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Release {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `sphinx_notfound_page-1.0.0/PKG-INFO` & `sphinx_notfound_page-1.0.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-notfound-page
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Sphinx extension to build a 404 page with absolute URLs
 Keywords: notfound,404,page,sphinx,documentation
 Author-email: Manuel Kaufmann <humitos@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Sphinx
```

