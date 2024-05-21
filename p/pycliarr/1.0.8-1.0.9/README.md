# Comparing `tmp/pycliarr-1.0.8.tar.gz` & `tmp/pycliarr-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycliarr-1.0.8.tar", last modified: Sun May  9 12:17:32 2021, max compression
+gzip compressed data, was "pycliarr-1.0.9.tar", last modified: Thu May 13 21:06:14 2021, max compression
```

## Comparing `pycliarr-1.0.8.tar` & `pycliarr-1.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2021-05-09 12:17:32.510031 pycliarr-1.0.8/
--rw-r--r--   0 viv        (501) staff       (20)     1077 2020-08-21 15:10:33.000000 pycliarr-1.0.8/LICENSE
--rw-r--r--   0 viv        (501) staff       (20)     7514 2021-05-09 12:17:32.510521 pycliarr-1.0.8/PKG-INFO
--rw-r--r--   0 viv        (501) staff       (20)     5578 2021-05-09 10:43:52.000000 pycliarr-1.0.8/README.md
--rw-r--r--   0 viv        (501) staff       (20)      930 2021-05-09 12:17:32.512452 pycliarr-1.0.8/setup.cfg
--rwxr-xr-x   0 viv        (501) staff       (20)     1031 2020-08-21 23:12:48.000000 pycliarr-1.0.8/setup.py
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2021-05-09 12:17:32.480961 pycliarr-1.0.8/src/
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2021-05-09 12:17:32.489406 pycliarr-1.0.8/src/pycliarr/
--rw-r--r--   0 viv        (501) staff       (20)       22 2021-05-09 11:29:51.000000 pycliarr-1.0.8/src/pycliarr/__init__.py
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2021-05-09 12:17:32.503277 pycliarr-1.0.8/src/pycliarr/api/
--rw-r--r--   0 viv        (501) staff       (20)      194 2020-12-18 19:35:06.000000 pycliarr-1.0.8/src/pycliarr/api/__init__.py
--rw-r--r--   0 viv        (501) staff       (20)     6884 2021-05-09 11:55:23.000000 pycliarr-1.0.8/src/pycliarr/api/base_api.py
--rw-r--r--   0 viv        (501) staff       (20)     8423 2021-05-09 10:01:40.000000 pycliarr-1.0.8/src/pycliarr/api/base_media.py
--rw-r--r--   0 viv        (501) staff       (20)      391 2020-12-18 18:59:41.000000 pycliarr-1.0.8/src/pycliarr/api/exceptions.py
--rw-r--r--   0 viv        (501) staff       (20)     7430 2020-12-18 22:05:34.000000 pycliarr-1.0.8/src/pycliarr/api/radarr.py
--rw-r--r--   0 viv        (501) staff       (20)     9954 2021-05-09 10:36:00.000000 pycliarr-1.0.8/src/pycliarr/api/sonarr.py
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2021-05-09 12:17:32.508839 pycliarr-1.0.8/src/pycliarr/cli/
--rw-r--r--   0 viv        (501) staff       (20)        0 2020-08-21 19:18:00.000000 pycliarr-1.0.8/src/pycliarr/cli/__init__.py
--rw-r--r--   0 viv        (501) staff       (20)     2698 2021-05-09 11:25:45.000000 pycliarr-1.0.8/src/pycliarr/cli/cli.py
--rw-r--r--   0 viv        (501) staff       (20)    19607 2021-05-09 11:52:46.000000 pycliarr-1.0.8/src/pycliarr/cli/cli_cmd.py
--rw-r--r--   0 viv        (501) staff       (20)      312 2020-08-21 21:35:22.000000 pycliarr-1.0.8/src/pycliarr/cli/utils.py
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2021-05-09 12:17:32.496409 pycliarr-1.0.8/src/pycliarr.egg-info/
--rw-r--r--   0 viv        (501) staff       (20)     7514 2021-05-09 12:17:32.000000 pycliarr-1.0.8/src/pycliarr.egg-info/PKG-INFO
--rw-r--r--   0 viv        (501) staff       (20)      595 2021-05-09 12:17:32.000000 pycliarr-1.0.8/src/pycliarr.egg-info/SOURCES.txt
--rw-r--r--   0 viv        (501) staff       (20)        1 2021-05-09 12:17:32.000000 pycliarr-1.0.8/src/pycliarr.egg-info/dependency_links.txt
--rw-r--r--   0 viv        (501) staff       (20)       52 2021-05-09 12:17:32.000000 pycliarr-1.0.8/src/pycliarr.egg-info/entry_points.txt
--rw-r--r--   0 viv        (501) staff       (20)        1 2020-08-21 16:38:32.000000 pycliarr-1.0.8/src/pycliarr.egg-info/not-zip-safe
--rw-r--r--   0 viv        (501) staff       (20)       13 2021-05-09 12:17:32.000000 pycliarr-1.0.8/src/pycliarr.egg-info/requires.txt
--rw-r--r--   0 viv        (501) staff       (20)        9 2021-05-09 12:17:32.000000 pycliarr-1.0.8/src/pycliarr.egg-info/top_level.txt
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2021-05-13 21:06:14.529004 pycliarr-1.0.9/
+-rw-r--r--   0 viv        (501) staff       (20)     1077 2020-08-21 15:10:33.000000 pycliarr-1.0.9/LICENSE
+-rw-r--r--   0 viv        (501) staff       (20)     7514 2021-05-13 21:06:14.529395 pycliarr-1.0.9/PKG-INFO
+-rw-r--r--   0 viv        (501) staff       (20)     5578 2021-05-09 10:43:52.000000 pycliarr-1.0.9/README.md
+-rw-r--r--   0 viv        (501) staff       (20)      930 2021-05-13 21:06:14.530532 pycliarr-1.0.9/setup.cfg
+-rwxr-xr-x   0 viv        (501) staff       (20)     1031 2020-08-21 23:12:48.000000 pycliarr-1.0.9/setup.py
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2021-05-13 21:06:14.510748 pycliarr-1.0.9/src/
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2021-05-13 21:06:14.514519 pycliarr-1.0.9/src/pycliarr/
+-rw-r--r--   0 viv        (501) staff       (20)       22 2021-05-13 21:02:05.000000 pycliarr-1.0.9/src/pycliarr/__init__.py
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2021-05-13 21:06:14.524788 pycliarr-1.0.9/src/pycliarr/api/
+-rw-r--r--   0 viv        (501) staff       (20)      194 2020-12-18 19:35:06.000000 pycliarr-1.0.9/src/pycliarr/api/__init__.py
+-rw-r--r--   0 viv        (501) staff       (20)     6884 2021-05-09 11:55:23.000000 pycliarr-1.0.9/src/pycliarr/api/base_api.py
+-rw-r--r--   0 viv        (501) staff       (20)     8423 2021-05-09 10:01:40.000000 pycliarr-1.0.9/src/pycliarr/api/base_media.py
+-rw-r--r--   0 viv        (501) staff       (20)      391 2020-12-18 18:59:41.000000 pycliarr-1.0.9/src/pycliarr/api/exceptions.py
+-rw-r--r--   0 viv        (501) staff       (20)     7796 2021-05-13 20:54:41.000000 pycliarr-1.0.9/src/pycliarr/api/radarr.py
+-rw-r--r--   0 viv        (501) staff       (20)     9973 2021-05-09 12:40:48.000000 pycliarr-1.0.9/src/pycliarr/api/sonarr.py
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2021-05-13 21:06:14.527961 pycliarr-1.0.9/src/pycliarr/cli/
+-rw-r--r--   0 viv        (501) staff       (20)        0 2020-08-21 19:18:00.000000 pycliarr-1.0.9/src/pycliarr/cli/__init__.py
+-rw-r--r--   0 viv        (501) staff       (20)     2698 2021-05-09 11:25:45.000000 pycliarr-1.0.9/src/pycliarr/cli/cli.py
+-rw-r--r--   0 viv        (501) staff       (20)    19806 2021-05-09 13:14:23.000000 pycliarr-1.0.9/src/pycliarr/cli/cli_cmd.py
+-rw-r--r--   0 viv        (501) staff       (20)      312 2020-08-21 21:35:22.000000 pycliarr-1.0.9/src/pycliarr/cli/utils.py
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2021-05-13 21:06:14.519103 pycliarr-1.0.9/src/pycliarr.egg-info/
+-rw-r--r--   0 viv        (501) staff       (20)     7514 2021-05-13 21:06:14.000000 pycliarr-1.0.9/src/pycliarr.egg-info/PKG-INFO
+-rw-r--r--   0 viv        (501) staff       (20)      595 2021-05-13 21:06:14.000000 pycliarr-1.0.9/src/pycliarr.egg-info/SOURCES.txt
+-rw-r--r--   0 viv        (501) staff       (20)        1 2021-05-13 21:06:14.000000 pycliarr-1.0.9/src/pycliarr.egg-info/dependency_links.txt
+-rw-r--r--   0 viv        (501) staff       (20)       52 2021-05-13 21:06:14.000000 pycliarr-1.0.9/src/pycliarr.egg-info/entry_points.txt
+-rw-r--r--   0 viv        (501) staff       (20)        1 2020-08-21 16:38:32.000000 pycliarr-1.0.9/src/pycliarr.egg-info/not-zip-safe
+-rw-r--r--   0 viv        (501) staff       (20)       13 2021-05-13 21:06:14.000000 pycliarr-1.0.9/src/pycliarr.egg-info/requires.txt
+-rw-r--r--   0 viv        (501) staff       (20)        9 2021-05-13 21:06:14.000000 pycliarr-1.0.9/src/pycliarr.egg-info/top_level.txt
```

### Comparing `pycliarr-1.0.8/LICENSE` & `pycliarr-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pycliarr-1.0.8/PKG-INFO` & `pycliarr-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycliarr
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python client for radarr and sonarr
 Home-page: https://github.com/vche/pycliarr
 Author: Vivien Chene
 Author-email: viv@vivc.org
 License: UNKNOWN
 Description: ![GitHub](https://img.shields.io/github/license/vche/pycliarr) [![Codecov](https://img.shields.io/codecov/c/github/vche/pycliarr)](https://codecov.io/gh/vche/pycliarr) [![Read the Docs](https://img.shields.io/readthedocs/pycliarr)](https://pycliarr.readthedocs.io/en/latest/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/vche/pycliarr)](https://github.com/vche/pycliarr/releases) [![PyPI](https://img.shields.io/pypi/v/pycliarr)](https://pypi.org/project/pycliarr/) [![Downloads](https://pepy.tech/badge/pycliarr)](https://pepy.tech/project/pycliarr)
```

### Comparing `pycliarr-1.0.8/README.md` & `pycliarr-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pycliarr-1.0.8/setup.cfg` & `pycliarr-1.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycliarr-1.0.8/setup.py` & `pycliarr-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pycliarr-1.0.8/src/pycliarr/api/base_api.py` & `pycliarr-1.0.9/src/pycliarr/api/base_api.py`

 * *Files identical despite different names*

### Comparing `pycliarr-1.0.8/src/pycliarr/api/base_media.py` & `pycliarr-1.0.9/src/pycliarr/api/base_media.py`

 * *Files identical despite different names*

### Comparing `pycliarr-1.0.8/src/pycliarr/api/radarr.py` & `pycliarr-1.0.9/src/pycliarr/api/radarr.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,31 +10,43 @@
 
     def _model(self) -> Dict[Any, Any]:
         """Define the model of items represented by this class."""
         return {
             "title": "",
             "sortTitle": "",
             "sizeOnDisk": 0,
+            "overview": "",
+            "inCinemas": "",
+            "physicalRelease": "",
             "status": "",
             "images": [],
+            "website": "",
             "downloaded": False,
             "year": 0,
             "hasFile": False,
+            "youTubeTrailerId": "",
+            "studio": "",
             "path": "",
+            "rootFolderPath": "",
             "profileId": 0,
             "monitored": True,
             "minimumAvailability": "",
+            "isAvailable": "",
+            "folderName": "",
             "runtime": 0,
             "cleanTitle": "",
             "imdbId": "",
             "tmdbId": 0,
             "titleSlug": "",
+            "certification": "",
             "genres": [],
             "tags": [],
             "added": "",
+            "ratings": {},
+            "collection": {},
             "alternativeTitles": [],
             "qualityProfileId": 0,
             "id": 0,
         }
 
 
 class RadarrCli(BaseCliMediaApi):
```

### Comparing `pycliarr-1.0.8/src/pycliarr/api/sonarr.py` & `pycliarr-1.0.9/src/pycliarr/api/sonarr.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,15 @@
         """
         if tvdb_id:
             term = "tvdb:" + str(tvdb_id)
         elif not term:
             raise SonarrCliError("Error invalid parameters")
 
         res = self.lookup_item(str(term))
+        print(res)
         if not res:
             return None
         elif isinstance(res, list):
             if len(res) > 1:
                 return [SonarrSerieItem.from_dict(serie) for serie in res]
             else:
                 res = res[0]
```

### Comparing `pycliarr-1.0.8/src/pycliarr/cli/cli.py` & `pycliarr-1.0.9/src/pycliarr/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pycliarr-1.0.8/src/pycliarr/cli/cli_cmd.py` & `pycliarr-1.0.9/src/pycliarr/cli/cli_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 import json
 from argparse import ArgumentParser, Namespace, _SubParsersAction
 from pprint import pformat
 from typing import Any, List, Optional, Union
 
-from pycliarr.api import base_media, radarr, sonarr
+from pycliarr.api import base_api, base_media, radarr, sonarr
 
 
 class CliCommand:
     """Base command, all command should extend this class."""
 
     name = ""
     description = ""
@@ -71,16 +71,19 @@
     else:
         raise Exception("Invalid profile selection: {}")
 
 
 def select_item(
     terms: str, choices: List[Union[radarr.RadarrMovieItem, sonarr.SonarrSerieItem]]
 ) -> Union[radarr.RadarrMovieItem, sonarr.SonarrSerieItem]:
-    if len(choices) == 0:
+    if not choices or (isinstance(choices, list) and len(choices) == 0):
         raise Exception(f"No match found for terms {terms}")
+    elif issubclass(choices.__class__, base_api.BaseCliApiItem):
+        # Only one result is returned
+        return choices  # type: ignore
     for item in choices:
         print(f"[{choices.index(item)+1}]: {item.title} ({item.year})")
     item_id = input(f"Select the item to add (1-{len(choices)}):")
     if item_id.isdigit() and int(item_id) <= len(choices):
         return choices[int(item_id) - 1]
     else:
         raise Exception("Invalid selection: {}")
```

### Comparing `pycliarr-1.0.8/src/pycliarr.egg-info/PKG-INFO` & `pycliarr-1.0.9/src/pycliarr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycliarr
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python client for radarr and sonarr
 Home-page: https://github.com/vche/pycliarr
 Author: Vivien Chene
 Author-email: viv@vivc.org
 License: UNKNOWN
 Description: ![GitHub](https://img.shields.io/github/license/vche/pycliarr) [![Codecov](https://img.shields.io/codecov/c/github/vche/pycliarr)](https://codecov.io/gh/vche/pycliarr) [![Read the Docs](https://img.shields.io/readthedocs/pycliarr)](https://pycliarr.readthedocs.io/en/latest/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/vche/pycliarr)](https://github.com/vche/pycliarr/releases) [![PyPI](https://img.shields.io/pypi/v/pycliarr)](https://pypi.org/project/pycliarr/) [![Downloads](https://pepy.tech/badge/pycliarr)](https://pepy.tech/project/pycliarr)
```

### Comparing `pycliarr-1.0.8/src/pycliarr.egg-info/SOURCES.txt` & `pycliarr-1.0.9/src/pycliarr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

