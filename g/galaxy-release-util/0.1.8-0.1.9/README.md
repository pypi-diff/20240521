# Comparing `tmp/galaxy_release_util-0.1.8.tar.gz` & `tmp/galaxy_release_util-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy_release_util-0.1.8.tar", last modified: Thu May  2 09:54:22 2024, max compression
+gzip compressed data, was "galaxy_release_util-0.1.9.tar", last modified: Thu May  2 12:13:37 2024, max compression
```

## Comparing `galaxy_release_util-0.1.8.tar` & `galaxy_release_util-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:54:22.553325 galaxy_release_util-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-02 09:54:22.553325 galaxy_release_util-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:54:22.553325 galaxy_release_util-0.1.8/galaxy_release_util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22296 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/bootstrap_history.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:54:22.553325 galaxy_release_util-0.1.8/galaxy_release_util/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/cli/release_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/github_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    28017 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/point_release.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:54:22.553325 galaxy_release_util-0.1.8/galaxy_release_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-02 09:54:22.000000 galaxy_release_util-0.1.8/galaxy_release_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-02 09:54:22.000000 galaxy_release_util-0.1.8/galaxy_release_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 09:54:22.000000 galaxy_release_util-0.1.8/galaxy_release_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 09:54:22.000000 galaxy_release_util-0.1.8/galaxy_release_util.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 09:54:22.000000 galaxy_release_util-0.1.8/galaxy_release_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 09:54:22.000000 galaxy_release_util-0.1.8/galaxy_release_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-02 09:54:22.553325 galaxy_release_util-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:54:22.553325 galaxy_release_util-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/tests/test_release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:37.732448 galaxy_release_util-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-02 12:13:29.000000 galaxy_release_util-0.1.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-02 12:13:29.000000 galaxy_release_util-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 12:13:29.000000 galaxy_release_util-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-02 12:13:37.732448 galaxy_release_util-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-02 12:13:29.000000 galaxy_release_util-0.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 12:13:29.000000 galaxy_release_util-0.1.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:37.732448 galaxy_release_util-0.1.9/galaxy_release_util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:29.000000 galaxy_release_util-0.1.9/galaxy_release_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22296 2024-05-02 12:13:29.000000 galaxy_release_util-0.1.9/galaxy_release_util/bootstrap_history.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:37.732448 galaxy_release_util-0.1.9/galaxy_release_util/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:29.000000 galaxy_release_util-0.1.9/galaxy_release_util/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-02 12:13:29.000000 galaxy_release_util-0.1.9/galaxy_release_util/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-02 12:13:29.000000 galaxy_release_util-0.1.9/galaxy_release_util/cli/release_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-02 12:13:29.000000 galaxy_release_util-0.1.9/galaxy_release_util/github_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-02 12:13:29.000000 galaxy_release_util-0.1.9/galaxy_release_util/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28326 2024-05-02 12:13:29.000000 galaxy_release_util-0.1.9/galaxy_release_util/point_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:29.000000 galaxy_release_util-0.1.9/galaxy_release_util/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:37.732448 galaxy_release_util-0.1.9/galaxy_release_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-02 12:13:37.000000 galaxy_release_util-0.1.9/galaxy_release_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-02 12:13:37.000000 galaxy_release_util-0.1.9/galaxy_release_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:13:37.000000 galaxy_release_util-0.1.9/galaxy_release_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 12:13:37.000000 galaxy_release_util-0.1.9/galaxy_release_util.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 12:13:37.000000 galaxy_release_util-0.1.9/galaxy_release_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 12:13:37.000000 galaxy_release_util-0.1.9/galaxy_release_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-02 12:13:29.000000 galaxy_release_util-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-02 12:13:37.732448 galaxy_release_util-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 12:13:29.000000 galaxy_release_util-0.1.9/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:13:37.732448 galaxy_release_util-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-02 12:13:29.000000 galaxy_release_util-0.1.9/tests/test_release.py
```

### Comparing `galaxy_release_util-0.1.8/HISTORY.rst` & `galaxy_release_util-0.1.9/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 History
 -------
 
 .. to_doc
 
 
 ------------------
+0.1.9 (02-05-2024)
+------------------
+* Fix release script if multiple bug fixes subheadings in changelog by @mvdbeek in https://github.com/galaxyproject/galaxy-release-util/pull/15
+
+------------------
 0.1.8 (02-05-2024)
 ------------------
 * Add mypy to CI under python 3.8 by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/11
 * Misc. updates  by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/12
 * Misc. updates to script generating the release publication issue by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/13
 * Fix link to docs on point releases by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/14
```

### Comparing `galaxy_release_util-0.1.8/LICENSE.txt` & `galaxy_release_util-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galaxy_release_util-0.1.8/PKG-INFO` & `galaxy_release_util-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-release-util
-Version: 0.1.8
+Version: 0.1.9
 Summary: Utlity for various tasks around creating Galaxy releases
 Home-page: https://github.com/galaxyproject/galaxy-release-util
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -63,14 +63,19 @@
 History
 -------
 
 .. to_doc
 
 
 ------------------
+0.1.9 (02-05-2024)
+------------------
+* Fix release script if multiple bug fixes subheadings in changelog by @mvdbeek in https://github.com/galaxyproject/galaxy-release-util/pull/15
+
+------------------
 0.1.8 (02-05-2024)
 ------------------
 * Add mypy to CI under python 3.8 by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/11
 * Misc. updates  by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/12
 * Misc. updates to script generating the release publication issue by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/13
 * Fix link to docs on point releases by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/14
```

### Comparing `galaxy_release_util-0.1.8/README.rst` & `galaxy_release_util-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `galaxy_release_util-0.1.8/galaxy_release_util/bootstrap_history.py` & `galaxy_release_util-0.1.9/galaxy_release_util/bootstrap_history.py`

 * *Files identical despite different names*

### Comparing `galaxy_release_util-0.1.8/galaxy_release_util/cli/options.py` & `galaxy_release_util-0.1.9/galaxy_release_util/cli/options.py`

 * *Files identical despite different names*

### Comparing `galaxy_release_util-0.1.8/galaxy_release_util/github_client.py` & `galaxy_release_util-0.1.9/galaxy_release_util/github_client.py`

 * *Files identical despite different names*

### Comparing `galaxy_release_util-0.1.8/galaxy_release_util/metadata.py` & `galaxy_release_util-0.1.9/galaxy_release_util/metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy_release_util-0.1.8/galaxy_release_util/point_release.py` & `galaxy_release_util-0.1.9/galaxy_release_util/point_release.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,20 @@
                 elif isinstance(changelog_item, docutils.nodes.paragraph):
                     changes = changelog_item.rawsource.splitlines()
                 elif isinstance(changelog_item, docutils.nodes.section):
                     kind = changelog_item[0].astext()
                     section_delimiter = "=" * len(kind)
                     changes.append(f"\n{section_delimiter}\n{kind}\n{section_delimiter}\n")
                     for section_changelog_item in changelog_item[1:]:
-                        assert isinstance(section_changelog_item, docutils.nodes.bullet_list)
+                        if isinstance(section_changelog_item, docutils.nodes.system_message):
+                            # Likely a warning that subsection (e.g. Bug fixes) is not unique
+                            continue
+                        assert isinstance(section_changelog_item, docutils.nodes.bullet_list), type(
+                            section_changelog_item
+                        )
                         for child in section_changelog_item:
                             add_changelog_item(changes, child)
             changelog_items.append(ChangelogItem(version=current_version, date=current_date, changes=changes))
 
     # Filter out dev release versions without changelog,
     # we're going to add these back after committing the release version
     clean_changelog_items: List[ChangelogItem] = []
```

### Comparing `galaxy_release_util-0.1.8/galaxy_release_util.egg-info/PKG-INFO` & `galaxy_release_util-0.1.9/galaxy_release_util.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-release-util
-Version: 0.1.8
+Version: 0.1.9
 Summary: Utlity for various tasks around creating Galaxy releases
 Home-page: https://github.com/galaxyproject/galaxy-release-util
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -63,14 +63,19 @@
 History
 -------
 
 .. to_doc
 
 
 ------------------
+0.1.9 (02-05-2024)
+------------------
+* Fix release script if multiple bug fixes subheadings in changelog by @mvdbeek in https://github.com/galaxyproject/galaxy-release-util/pull/15
+
+------------------
 0.1.8 (02-05-2024)
 ------------------
 * Add mypy to CI under python 3.8 by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/11
 * Misc. updates  by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/12
 * Misc. updates to script generating the release publication issue by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/13
 * Fix link to docs on point releases by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/14
```

### Comparing `galaxy_release_util-0.1.8/galaxy_release_util.egg-info/SOURCES.txt` & `galaxy_release_util-0.1.9/galaxy_release_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy_release_util-0.1.8/setup.cfg` & `galaxy_release_util-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-release-util
 url = https://github.com/galaxyproject/galaxy-release-util
-version = 0.1.8
+version = 0.1.9
 
 [options]
 include_package_data = True
 install_requires = 
 	build
 	click
 	docutils
```

### Comparing `galaxy_release_util-0.1.8/tests/test_release.py` & `galaxy_release_util-0.1.9/tests/test_release.py`

 * *Files identical despite different names*

