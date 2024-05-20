# Comparing `tmp/deezer_python-6.1.1.tar.gz` & `tmp/deezer_python-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deezer_python-6.1.1.tar", max compression
+gzip compressed data, was "deezer_python-6.2.0.tar", max compression
```

## Comparing `deezer_python-6.1.1.tar` & `deezer_python-6.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1054 2023-10-18 10:49:08.531660 deezer_python-6.1.1/LICENSE.txt
--rw-r--r--   0        0        0    13246 2023-10-18 10:49:08.531660 deezer_python-6.1.1/README.md
--rw-r--r--   0        0        0     3319 2023-10-18 10:49:10.239643 deezer_python-6.1.1/pyproject.toml
--rw-r--r--   0        0        0      556 2023-10-18 10:49:10.239643 deezer_python-6.1.1/src/deezer/__init__.py
--rw-r--r--   0        0        0    24896 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/client.py
--rw-r--r--   0        0        0      648 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/dates.py
--rw-r--r--   0        0        0     2003 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/exceptions.py
--rw-r--r--   0        0        0     4057 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/pagination.py
--rw-r--r--   0        0        0      549 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/resources/__init__.py
--rw-r--r--   0        0        0     1734 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/resources/album.py
--rw-r--r--   0        0        0     2150 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/resources/artist.py
--rw-r--r--   0        0        0     2193 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/resources/chart.py
--rw-r--r--   0        0        0     1413 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/resources/editorial.py
--rw-r--r--   0        0        0     1762 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/resources/episode.py
--rw-r--r--   0        0        0     1355 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/resources/genre.py
--rw-r--r--   0        0        0     3325 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/resources/playlist.py
--rw-r--r--   0        0        0      915 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/resources/podcast.py
--rw-r--r--   0        0        0      805 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/resources/radio.py
--rw-r--r--   0        0        0     4978 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/resources/resource.py
--rw-r--r--   0        0        0     1546 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/resources/track.py
--rw-r--r--   0        0        0     6752 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/resources/user.py
--rw-r--r--   0        0        0      583 2023-10-18 10:49:08.531660 deezer_python-6.1.1/src/deezer/utils.py
--rw-r--r--   0        0        0    14630 1970-01-01 00:00:00.000000 deezer_python-6.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-05-20 22:49:17.423074 deezer_python-6.2.0/LICENSE.txt
+-rw-r--r--   0        0        0    13245 2024-05-20 22:49:17.423074 deezer_python-6.2.0/README.md
+-rw-r--r--   0        0        0     3668 2024-05-20 22:49:28.635103 deezer_python-6.2.0/pyproject.toml
+-rw-r--r--   0        0        0      556 2024-05-20 22:49:28.635103 deezer_python-6.2.0/src/deezer/__init__.py
+-rw-r--r--   0        0        0    25651 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/client.py
+-rw-r--r--   0        0        0      648 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/dates.py
+-rw-r--r--   0        0        0     2003 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/exceptions.py
+-rw-r--r--   0        0        0     4041 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/pagination.py
+-rw-r--r--   0        0        0      549 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/resources/__init__.py
+-rw-r--r--   0        0        0     1734 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/resources/album.py
+-rw-r--r--   0        0        0     2150 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/resources/artist.py
+-rw-r--r--   0        0        0     2193 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/resources/chart.py
+-rw-r--r--   0        0        0     1413 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/resources/editorial.py
+-rw-r--r--   0        0        0     1762 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/resources/episode.py
+-rw-r--r--   0        0        0     1355 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/resources/genre.py
+-rw-r--r--   0        0        0     3325 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/resources/playlist.py
+-rw-r--r--   0        0        0      915 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/resources/podcast.py
+-rw-r--r--   0        0        0      805 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/resources/radio.py
+-rw-r--r--   0        0        0     4978 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/resources/resource.py
+-rw-r--r--   0        0        0     1546 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/resources/track.py
+-rw-r--r--   0        0        0     6752 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/resources/user.py
+-rw-r--r--   0        0        0      583 2024-05-20 22:49:17.427074 deezer_python-6.2.0/src/deezer/utils.py
+-rw-r--r--   0        0        0    14629 1970-01-01 00:00:00.000000 deezer_python-6.2.0/PKG-INFO
```

### Comparing `deezer_python-6.1.1/LICENSE.txt` & `deezer_python-6.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deezer_python-6.1.1/README.md` & `deezer_python-6.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     pip install deezer-python
 
 ## Basic Use
 
 Easily query the Deezer API from you Python code. The data returned by the Deezer
 API is mapped to python resources:
 
-```python
+```pycon
 >>> client = deezer.Client()
 >>> client.get_album(680407).title
 'Monkey Business'
 ```
 
 Ready for more? Look at our whole [documentation](http://deezer-python.readthedocs.io/)
 on Read The Docs or have a play in pre-populated Jupyter notebook
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
         _[_L_a_u_n_c_h_ _d_e_m_o_ _o_n_ _B_i_n_d_e_r_]_[_P_y_P_i_ _S_t_a_t_u_s_][pyversions][license]_[_L_o_C_]
 --- **Documentation**: _h_t_t_p_s_:_/_/_d_e_e_z_e_r_-_p_y_t_h_o_n_._r_e_a_d_t_h_e_d_o_c_s_._i_o **Source Code**:
 _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_b_r_o_w_n_i_e_b_r_o_k_e_/_d_e_e_z_e_r_-_p_y_t_h_o_n_ --- A friendly Python wrapper
 around the [Deezer API](https://developers.deezer.com/api). ## Installation The
 package is published on [PyPI](https://pypi.org/project/deezer-python/) and can
 be installed by running: pip install deezer-python ## Basic Use Easily query
 the Deezer API from you Python code. The data returned by the Deezer API is
-mapped to python resources: ```python >>> client = deezer.Client() >>>
+mapped to python resources: ```pycon >>> client = deezer.Client() >>>
 client.get_album(680407).title 'Monkey Business' ``` Ready for more? Look at
 our whole [documentation](http://deezer-python.readthedocs.io/) on Read The
 Docs or have a play in pre-populated Jupyter notebook [on Binder](https://
 mybinder.org/v2/gh/browniebroke/deezer-python/main?filepath=demo.ipynb). ##
 Contributors
  _[_B_r_u_n_o     _[_m_i_s_u_z_u_]         _[_P_a_s_c_a_l_]    _[_k_h_a_m_a_i_l_e_o_n_]  _[_N_i_k_o_l_a_y   _[_M_a_t_h_e_u_s  _[_K_i_e_r_a_n
   _A_l_l_a_]      _mm_ii_ss_uu_zz_uu           _PP_aa_ss_cc_aa_ll      _kk_hh_aa_mm_aa_ii_ll_ee_oo_nn  _S_h_e_r_e_g_e_d_a_] _H_o_r_s_t_m_a_n_n_]  _W_y_n_n_e_]
```

### Comparing `deezer_python-6.1.1/pyproject.toml` & `deezer_python-6.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deezer-python"
-version = "6.1.1"
+version = "6.2.0"
 description = "A friendly wrapper library for the Deezer API"
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["deezer", "sdk", "client", "requests"]
 repository = "https://github.com/browniebroke/deezer-python"
 documentation = "https://deezer-python.readthedocs.io"
@@ -30,46 +30,55 @@
 python = "^3.8"
 requests = ">=2.18"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-myst-parser = ">=0.16"
-sphinx = ">=4.0"
-sphinx-autobuild = ">=2021.0"
-furo = ">=2023.5.20"
+myst-parser = { version = ">=0.16", python = ">=3.11" }
+sphinx = { version = ">=4.0", python = ">=3.11" }
+furo = { version = ">=2023.5.20", python = ">=3.11" }
+sphinx-autobuild = { version = ">=2024.0.0", python = ">=3.11" }
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.0"
-environs = "^9.3"
-pytest = "^7.0"
-pytest-cov = "^4.0"
+environs = "^11.0.0"
+pytest = "^8.0.0"
+pytest-cov = "^5.0.0"
 pytest-mock = "^3.6"
 pytest-vcr = "^1.0"
-vcrpy = "^5.0.0"
+vcrpy = "^6.0.0"
 deezer-oauth-cli = "^1.0.0"
 
 [tool.semantic_release]
 version_toml = ["pyproject.toml:tool.poetry.version"]
 version_variables = [
     "src/deezer/__init__.py:__version__",
 ]
-branch = "main"
 build_command = "pip install poetry && poetry build"
 
 [tool.semantic_release.changelog]
 exclude_commit_patterns = [
     "chore*",
     "ci*",
 ]
 
 [tool.semantic_release.changelog.environment]
 keep_trailing_newline = true
 
+[tool.semantic_release.branches.main]
+match = "main"
+
+[tool.semantic_release.branches.stable]
+match = "(?!stable/*$)"
+
+[tool.semantic_release.branches.noop]
+match = "(?!main$)"
+prerelease = true
+
 [tool.pytest.ini_options]
 addopts = "-v -Wdefault --cov=deezer"
 pythonpath = ["src"]
 
 [tool.coverage.run]
 branch = true
 source = ["deezer"]
@@ -82,14 +91,16 @@
     "if TYPE_CHECKING",
     "raise NotImplementedError",
 ]
 
 [tool.ruff]
 target-version = "py38"
 line-length = 120
+
+[tool.ruff.lint]
 ignore = [
     "D203", # 1 blank line required before class docstring
     "D212", # Multi-line docstring summary should start at the first line
     "D100", # Missing docstring in public module
     "D104", # Missing docstring in public package
     "D107", # Missing docstring in `__init__`
     "D401", # First line of docstring should be in imperative mood
@@ -103,28 +114,28 @@
     "E",   # pycodestyle
     "W",   # pycodestyle
     "UP",  # pyupgrade
     "I",   # isort
     "RUF", # ruff specific
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/**/*" = [
     "D100",
     "D101",
     "D102",
     "D103",
     "D104",
     "S101",
 ]
 "setup.py" = ["D100"]
 "conftest.py" = ["D100"]
 "docs/conf.py" = ["D100"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["deezer"]
 
 [tool.mypy]
 # suppress errors about unsatisfied imports
 ignore_missing_imports = true
 
 no_implicit_optional = true
```

### Comparing `deezer_python-6.1.1/src/deezer/__init__.py` & `deezer_python-6.2.0/src/deezer/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Podcast,
     Radio,
     Resource,
     Track,
     User,
 )
 
-__version__ = "6.1.1"
+__version__ = "6.2.0"
 __all__ = [
     "Album",
     "Artist",
     "Chart",
     "Client",
     "Editorial",
     "Episode",
```

### Comparing `deezer_python-6.1.1/src/deezer/client.py` & `deezer_python-6.2.0/src/deezer/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import warnings
 from typing import Any, ClassVar
 
 import requests
 
 from deezer.exceptions import (
     DeezerErrorResponse,
     DeezerHTTPError,
@@ -21,38 +22,47 @@
     Podcast,
     Radio,
     Resource,
     Track,
     User,
 )
 
+_UNSET = object()
+
 
 class Client:
     """
     A client to retrieve some basic infos about Deezer resources.
 
     Create a client instance with the given options. Options should
     be passed in to the constructor as kwargs.
 
         >>> import deezer
-        >>> client = deezer.Client(app_id='foo', app_secret='bar')
+        >>> client = deezer.Client()
 
     This client provides several methods to retrieve the content most
     kinds of Deezer objects, based on their json structure.
 
     Headers can be forced by using the ``headers`` kwarg.
     For example, use ``Accept-Language`` header to force the output language.
 
         >>> import deezer
         >>> client = deezer.Client(headers={'Accept-Language': 'fr'})
 
-    :param app_id: application ID.
-    :param app_secret: application secret.
     :param access_token: user access token.
     :param headers: a dictionary of headers to be used.
+
+    .. deprecated:: 6.2.0
+
+        The following parameters will be removed in the next major version:
+
+            * **app_id**
+            * **app_secret**
+
+        They were never actively used by the package.
     """
 
     objects_types: ClassVar[dict[str, type[Resource] | None]] = {
         "album": Album,
         "artist": Artist,
         "chart": Chart,
         "editorial": Editorial,
@@ -65,18 +75,37 @@
         "search": None,
         "track": Track,
         "user": User,
     }
     base_url = "https://api.deezer.com"
 
     def __init__(
-        self, app_id=None, app_secret=None, access_token=None, headers=None, **kwargs
+        self,
+        app_id=_UNSET,
+        app_secret=_UNSET,
+        access_token=None,
+        headers=None,
+        **kwargs,
     ):
-        self.app_id = app_id
-        self.app_secret = app_secret
+        if app_id is not _UNSET:
+            warnings.warn(
+                "The 'app_id' parameter is not actually used and is deprecated. "
+                "It will be removed in the next major release.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+            self.app_id = app_id
+        if app_secret is not _UNSET:
+            warnings.warn(
+                "The 'app_secret' parameter is not actually used and is deprecated. "
+                "It will be removed in the next major release.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+            self.app_secret = app_secret
         self.access_token = access_token
         self.session = requests.Session()
 
         headers = headers or {}
         self.session.headers.update(headers)
 
     def _process_json(
@@ -162,15 +191,15 @@
         try:
             response.raise_for_status()
         except requests.HTTPError as exc:
             raise DeezerHTTPError.from_http_error(exc) from exc
         json_data = response.json()
         if not isinstance(json_data, dict):
             return json_data
-        if "error" in json_data and json_data["error"]:
+        if json_data.get("error"):
             raise DeezerErrorResponse(json_data)
         return self._process_json(
             json_data,
             parent=parent,
             resource_type=resource_type,
             resource_id=resource_id,
             paginate_list=paginate_list,
```

### Comparing `deezer_python-6.1.1/src/deezer/dates.py` & `deezer_python-6.2.0/src/deezer/dates.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.1.1/src/deezer/exceptions.py` & `deezer_python-6.2.0/src/deezer/exceptions.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.1.1/src/deezer/pagination.py` & `deezer_python-6.2.0/src/deezer/pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,20 +37,18 @@
         repr_size = 5
         data: list[ResourceType | str] = list(self[: repr_size + 1])
         if len(data) > repr_size:
             data[-1] = "..."
         return f"<{self.__class__.__name__} {data!r}>"
 
     @overload
-    def __getitem__(self, index: int) -> ResourceType:
-        ...
+    def __getitem__(self, index: int) -> ResourceType: ...
 
     @overload
-    def __getitem__(self, index: slice) -> list[ResourceType]:
-        ...
+    def __getitem__(self, index: slice) -> list[ResourceType]: ...
 
     def __getitem__(
         self,
         index: int | slice,
     ) -> ResourceType | list[ResourceType]:
         """Get an item or a slice of items from the list."""
         if isinstance(index, int):
```

### Comparing `deezer_python-6.1.1/src/deezer/resources/__init__.py` & `deezer_python-6.2.0/src/deezer/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.1.1/src/deezer/resources/album.py` & `deezer_python-6.2.0/src/deezer/resources/album.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.1.1/src/deezer/resources/artist.py` & `deezer_python-6.2.0/src/deezer/resources/artist.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.1.1/src/deezer/resources/chart.py` & `deezer_python-6.2.0/src/deezer/resources/chart.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.1.1/src/deezer/resources/editorial.py` & `deezer_python-6.2.0/src/deezer/resources/editorial.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.1.1/src/deezer/resources/episode.py` & `deezer_python-6.2.0/src/deezer/resources/episode.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.1.1/src/deezer/resources/genre.py` & `deezer_python-6.2.0/src/deezer/resources/genre.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.1.1/src/deezer/resources/playlist.py` & `deezer_python-6.2.0/src/deezer/resources/playlist.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.1.1/src/deezer/resources/podcast.py` & `deezer_python-6.2.0/src/deezer/resources/podcast.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.1.1/src/deezer/resources/radio.py` & `deezer_python-6.2.0/src/deezer/resources/radio.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.1.1/src/deezer/resources/resource.py` & `deezer_python-6.2.0/src/deezer/resources/resource.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.1.1/src/deezer/resources/track.py` & `deezer_python-6.2.0/src/deezer/resources/track.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.1.1/src/deezer/resources/user.py` & `deezer_python-6.2.0/src/deezer/resources/user.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.1.1/src/deezer/utils.py` & `deezer_python-6.2.0/src/deezer/utils.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.1.1/PKG-INFO` & `deezer_python-6.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deezer-python
-Version: 6.1.1
+Version: 6.2.0
 Summary: A friendly wrapper library for the Deezer API
 Home-page: https://github.com/browniebroke/deezer-python
 License: MIT
 Keywords: deezer,sdk,client,requests
 Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -85,15 +85,15 @@
     pip install deezer-python
 
 ## Basic Use
 
 Easily query the Deezer API from you Python code. The data returned by the Deezer
 API is mapped to python resources:
 
-```python
+```pycon
 >>> client = deezer.Client()
 >>> client.get_album(680407).title
 'Monkey Business'
 ```
 
 Ready for more? Look at our whole [documentation](http://deezer-python.readthedocs.io/)
 on Read The Docs or have a play in pre-populated Jupyter notebook
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deezer-python Version: 6.1.1 Summary: A friendly
+Metadata-Version: 2.1 Name: deezer-python Version: 6.2.0 Summary: A friendly
 wrapper library for the Deezer API Home-page: https://github.com/browniebroke/
 deezer-python License: MIT Keywords: deezer,sdk,client,requests Author: Bruno
 Alla Author-email: alla.brunoo@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
@@ -22,15 +22,15 @@
         _[_L_a_u_n_c_h_ _d_e_m_o_ _o_n_ _B_i_n_d_e_r_]_[_P_y_P_i_ _S_t_a_t_u_s_][pyversions][license]_[_L_o_C_]
 --- **Documentation**: _h_t_t_p_s_:_/_/_d_e_e_z_e_r_-_p_y_t_h_o_n_._r_e_a_d_t_h_e_d_o_c_s_._i_o **Source Code**:
 _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_b_r_o_w_n_i_e_b_r_o_k_e_/_d_e_e_z_e_r_-_p_y_t_h_o_n_ --- A friendly Python wrapper
 around the [Deezer API](https://developers.deezer.com/api). ## Installation The
 package is published on [PyPI](https://pypi.org/project/deezer-python/) and can
 be installed by running: pip install deezer-python ## Basic Use Easily query
 the Deezer API from you Python code. The data returned by the Deezer API is
-mapped to python resources: ```python >>> client = deezer.Client() >>>
+mapped to python resources: ```pycon >>> client = deezer.Client() >>>
 client.get_album(680407).title 'Monkey Business' ``` Ready for more? Look at
 our whole [documentation](http://deezer-python.readthedocs.io/) on Read The
 Docs or have a play in pre-populated Jupyter notebook [on Binder](https://
 mybinder.org/v2/gh/browniebroke/deezer-python/main?filepath=demo.ipynb). ##
 Contributors
  _[_B_r_u_n_o     _[_m_i_s_u_z_u_]         _[_P_a_s_c_a_l_]    _[_k_h_a_m_a_i_l_e_o_n_]  _[_N_i_k_o_l_a_y   _[_M_a_t_h_e_u_s  _[_K_i_e_r_a_n
   _A_l_l_a_]      _mm_ii_ss_uu_zz_uu           _PP_aa_ss_cc_aa_ll      _kk_hh_aa_mm_aa_ii_ll_ee_oo_nn  _S_h_e_r_e_g_e_d_a_] _H_o_r_s_t_m_a_n_n_]  _W_y_n_n_e_]
```

