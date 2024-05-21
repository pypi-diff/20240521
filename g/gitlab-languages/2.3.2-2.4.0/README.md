# Comparing `tmp/gitlab_languages-2.3.2.tar.gz` & `tmp/gitlab_languages-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_languages-2.3.2.tar", max compression
+gzip compressed data, was "gitlab_languages-2.4.0.tar", max compression
```

## Comparing `gitlab_languages-2.3.2.tar` & `gitlab_languages-2.4.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1073 2022-12-20 10:29:21.753122 gitlab_languages-2.3.2/LICENSE
--rw-r--r--   0        0        0     4783 2022-12-20 10:29:21.753122 gitlab_languages-2.3.2/README.md
--rw-r--r--   0        0        0      128 2022-12-20 10:29:21.753122 gitlab_languages-2.3.2/gitlab_languages/__main__.py
--rw-r--r--   0        0        0    14209 2022-12-20 10:29:21.753122 gitlab_languages-2.3.2/gitlab_languages/gitlab_languages.py
--rw-r--r--   0        0        0     1187 2022-12-20 10:29:21.753122 gitlab_languages-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     5930 1970-01-01 00:00:00.000000 gitlab_languages-2.3.2/setup.py
--rw-r--r--   0        0        0     5890 1970-01-01 00:00:00.000000 gitlab_languages-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-21 08:57:43.254256 gitlab_languages-2.4.0/LICENSE
+-rw-r--r--   0        0        0     4783 2024-05-21 08:57:43.254256 gitlab_languages-2.4.0/README.md
+-rw-r--r--   0        0        0      128 2024-05-21 08:57:43.254256 gitlab_languages-2.4.0/gitlab_languages/__main__.py
+-rw-r--r--   0        0        0    14209 2024-05-21 08:57:43.254256 gitlab_languages-2.4.0/gitlab_languages/gitlab_languages.py
+-rw-r--r--   0        0        0     1283 2024-05-21 08:57:43.254256 gitlab_languages-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5889 1970-01-01 00:00:00.000000 gitlab_languages-2.4.0/PKG-INFO
```

### Comparing `gitlab_languages-2.3.2/LICENSE` & `gitlab_languages-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_languages-2.3.2/README.md` & `gitlab_languages-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gitlab_languages-2.3.2/gitlab_languages/gitlab_languages.py` & `gitlab_languages-2.4.0/gitlab_languages/gitlab_languages.py`

 * *Files identical despite different names*

### Comparing `gitlab_languages-2.3.2/pyproject.toml` & `gitlab_languages-2.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 [tool.poetry]
 name = "gitlab-languages"
-version = "2.3.2"
+version = "2.4.0"
 description = "Utility to generate a Prometheus data source from programming languages inside GitLab repositores"
 authors = ["Max Wittig"]
 readme = "README.md"
 repository = "https://github.com/max-wittig/gitlab-languages"
 keywords = ["gitlab", "languages", "api", "python-gitlab", "prometheus", "metrics"]
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development",
     "Topic :: Utilities"
 ]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 prometheus-client = "^0.15.0"
 maya = "^0.6.1"
-python-gitlab = "^3.12.0"
+python-gitlab = "^4.5.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.scripts]
 gitlab-languages = "gitlab_languages.__main__:main"
 gitlab_languages = "gitlab_languages.__main__:main"
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.12.0"
+black = ">=22.12,<25.0"
 isort = "^5.11.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gitlab_languages-2.3.2/PKG-INFO` & `gitlab_languages-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: gitlab-languages
-Version: 2.3.2
+Version: 2.4.0
 Summary: Utility to generate a Prometheus data source from programming languages inside GitLab repositores
 Home-page: https://github.com/max-wittig/gitlab-languages
 License: MIT
 Keywords: gitlab,languages,api,python-gitlab,prometheus,metrics
 Author: Max Wittig
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Dist: maya (>=0.6.1,<0.7.0)
 Requires-Dist: prometheus-client (>=0.15.0,<0.16.0)
-Requires-Dist: python-gitlab (>=3.12.0,<4.0.0)
+Requires-Dist: python-gitlab (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/max-wittig/gitlab-languages
 Description-Content-Type: text/markdown
 
 # gitlab-languages
 
 [![PyPI - License](https://img.shields.io/pypi/l/gitlab-languages.svg)](https://github.com/max-wittig/gitlab-languages/blob/master/LICENSE)
```

