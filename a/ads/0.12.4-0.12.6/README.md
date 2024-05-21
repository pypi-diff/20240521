# Comparing `tmp/ads-0.12.4.tar.gz` & `tmp/ads-0.12.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ads-0.12.4.tar", last modified: Sun Jan 28 22:37:03 2024, max compression
+gzip compressed data, was "ads-0.12.6.tar", last modified: Tue May 21 12:28:42 2024, max compression
```

## Comparing `ads-0.12.4.tar` & `ads-0.12.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 andycasey   (501) staff       (20)        0 2024-01-28 22:37:03.243330 ads-0.12.4/
--rw-r--r--   0 andycasey   (501) staff       (20)     1078 2024-01-28 22:28:47.000000 ads-0.12.4/LICENSE
--rw-r--r--   0 andycasey   (501) staff       (20)       54 2024-01-28 22:28:47.000000 ads-0.12.4/MANIFEST.in
--rw-r--r--   0 andycasey   (501) staff       (20)     1809 2024-01-28 22:37:03.242944 ads-0.12.4/PKG-INFO
--rw-r--r--   0 andycasey   (501) staff       (20)     1440 2024-01-28 22:28:47.000000 ads-0.12.4/README.rst
-drwxr-xr-x   0 andycasey   (501) staff       (20)        0 2024-01-28 22:37:03.237447 ads-0.12.4/ads/
--rw-r--r--   0 andycasey   (501) staff       (20)      283 2024-01-28 22:33:01.000000 ads-0.12.4/ads/__init__.py
--rw-r--r--   0 andycasey   (501) staff       (20)     4575 2024-01-28 22:28:47.000000 ads-0.12.4/ads/base.py
--rw-r--r--   0 andycasey   (501) staff       (20)      534 2024-01-28 22:28:47.000000 ads-0.12.4/ads/config.py
--rw-r--r--   0 andycasey   (501) staff       (20)      453 2024-01-28 22:28:47.000000 ads-0.12.4/ads/exceptions.py
--rw-r--r--   0 andycasey   (501) staff       (20)     1830 2024-01-28 22:28:47.000000 ads-0.12.4/ads/export.py
--rw-r--r--   0 andycasey   (501) staff       (20)     9687 2024-01-28 22:28:47.000000 ads-0.12.4/ads/libraries.py
--rw-r--r--   0 andycasey   (501) staff       (20)     1411 2024-01-28 22:28:47.000000 ads-0.12.4/ads/metrics.py
--rw-r--r--   0 andycasey   (501) staff       (20)     1473 2024-01-28 22:28:47.000000 ads-0.12.4/ads/sandbox.py
--rw-r--r--   0 andycasey   (501) staff       (20)    19009 2024-01-28 22:28:47.000000 ads-0.12.4/ads/search.py
-drwxr-xr-x   0 andycasey   (501) staff       (20)        0 2024-01-28 22:37:03.241182 ads-0.12.4/ads/tests/
--rw-r--r--   0 andycasey   (501) staff       (20)        0 2024-01-28 22:28:47.000000 ads-0.12.4/ads/tests/__init__.py
--rw-r--r--   0 andycasey   (501) staff       (20)     4440 2024-01-28 22:28:47.000000 ads-0.12.4/ads/tests/mocks.py
-drwxr-xr-x   0 andycasey   (501) staff       (20)        0 2024-01-28 22:37:03.242347 ads-0.12.4/ads/tests/stubdata/
--rw-r--r--   0 andycasey   (501) staff       (20)        0 2024-01-28 22:28:47.000000 ads-0.12.4/ads/tests/stubdata/__init__.py
--rw-r--r--   0 andycasey   (501) staff       (20)     1020 2024-01-28 22:28:47.000000 ads-0.12.4/ads/tests/stubdata/export.py
--rw-r--r--   0 andycasey   (501) staff       (20)    18919 2024-01-28 22:28:47.000000 ads-0.12.4/ads/tests/stubdata/metrics.py
--rw-r--r--   0 andycasey   (501) staff       (20)    74823 2024-01-28 22:28:47.000000 ads-0.12.4/ads/tests/stubdata/solr.py
--rw-r--r--   0 andycasey   (501) staff       (20)     5799 2024-01-28 22:28:47.000000 ads-0.12.4/ads/tests/test_base.py
--rw-r--r--   0 andycasey   (501) staff       (20)     1552 2024-01-28 22:28:47.000000 ads-0.12.4/ads/tests/test_export.py
--rw-r--r--   0 andycasey   (501) staff       (20)     1527 2024-01-28 22:28:47.000000 ads-0.12.4/ads/tests/test_metrics.py
--rw-r--r--   0 andycasey   (501) staff       (20)     2077 2024-01-28 22:28:47.000000 ads-0.12.4/ads/tests/test_sandbox.py
--rw-r--r--   0 andycasey   (501) staff       (20)    15478 2024-01-28 22:28:47.000000 ads-0.12.4/ads/tests/test_search.py
--rw-r--r--   0 andycasey   (501) staff       (20)     1110 2024-01-28 22:28:47.000000 ads-0.12.4/ads/tests/test_utils.py
--rw-r--r--   0 andycasey   (501) staff       (20)     1150 2024-01-28 22:29:30.000000 ads-0.12.4/ads/utils.py
-drwxr-xr-x   0 andycasey   (501) staff       (20)        0 2024-01-28 22:37:03.238964 ads-0.12.4/ads.egg-info/
--rw-r--r--   0 andycasey   (501) staff       (20)     1809 2024-01-28 22:37:02.000000 ads-0.12.4/ads.egg-info/PKG-INFO
--rw-r--r--   0 andycasey   (501) staff       (20)      645 2024-01-28 22:37:02.000000 ads-0.12.4/ads.egg-info/SOURCES.txt
--rw-r--r--   0 andycasey   (501) staff       (20)        1 2024-01-28 22:37:02.000000 ads-0.12.4/ads.egg-info/dependency_links.txt
--rw-r--r--   0 andycasey   (501) staff       (20)       45 2024-01-28 22:37:02.000000 ads-0.12.4/ads.egg-info/requires.txt
--rw-r--r--   0 andycasey   (501) staff       (20)        4 2024-01-28 22:37:02.000000 ads-0.12.4/ads.egg-info/top_level.txt
--rw-r--r--   0 andycasey   (501) staff       (20)       45 2024-01-28 22:28:47.000000 ads-0.12.4/requirements.txt
--rw-r--r--   0 andycasey   (501) staff       (20)       38 2024-01-28 22:37:03.243420 ads-0.12.4/setup.cfg
--rw-r--r--   0 andycasey   (501) staff       (20)     1219 2024-01-28 22:33:48.000000 ads-0.12.4/setup.py
+drwxr-xr-x   0 andycasey   (501) staff       (20)        0 2024-05-21 12:28:42.683902 ads-0.12.6/
+-rw-r--r--   0 andycasey   (501) staff       (20)     1078 2022-10-14 01:29:43.000000 ads-0.12.6/LICENSE
+-rw-r--r--   0 andycasey   (501) staff       (20)       54 2022-10-14 01:29:43.000000 ads-0.12.6/MANIFEST.in
+-rw-r--r--   0 andycasey   (501) staff       (20)     1832 2024-05-21 12:28:42.683496 ads-0.12.6/PKG-INFO
+-rw-r--r--   0 andycasey   (501) staff       (20)     1383 2024-05-21 12:19:33.000000 ads-0.12.6/README.md
+drwxr-xr-x   0 andycasey   (501) staff       (20)        0 2024-05-21 12:28:42.678111 ads-0.12.6/ads/
+-rw-r--r--   0 andycasey   (501) staff       (20)      283 2024-05-21 12:24:10.000000 ads-0.12.6/ads/__init__.py
+-rw-r--r--   0 andycasey   (501) staff       (20)     4575 2024-05-21 12:06:26.000000 ads-0.12.6/ads/base.py
+-rw-r--r--   0 andycasey   (501) staff       (20)      534 2024-05-21 12:06:26.000000 ads-0.12.6/ads/config.py
+-rw-r--r--   0 andycasey   (501) staff       (20)      453 2024-05-21 12:06:26.000000 ads-0.12.6/ads/exceptions.py
+-rw-r--r--   0 andycasey   (501) staff       (20)     1830 2024-05-21 12:06:26.000000 ads-0.12.6/ads/export.py
+-rw-r--r--   0 andycasey   (501) staff       (20)     9687 2024-05-21 12:06:28.000000 ads-0.12.6/ads/libraries.py
+-rw-r--r--   0 andycasey   (501) staff       (20)     1411 2024-05-21 12:06:26.000000 ads-0.12.6/ads/metrics.py
+-rw-r--r--   0 andycasey   (501) staff       (20)     1473 2024-05-21 12:06:26.000000 ads-0.12.6/ads/sandbox.py
+-rw-r--r--   0 andycasey   (501) staff       (20)    19009 2024-05-21 12:06:28.000000 ads-0.12.6/ads/search.py
+drwxr-xr-x   0 andycasey   (501) staff       (20)        0 2024-05-21 12:28:42.681534 ads-0.12.6/ads/tests/
+-rw-r--r--   0 andycasey   (501) staff       (20)        0 2024-05-21 12:06:26.000000 ads-0.12.6/ads/tests/__init__.py
+-rw-r--r--   0 andycasey   (501) staff       (20)     4440 2024-05-21 12:06:26.000000 ads-0.12.6/ads/tests/mocks.py
+drwxr-xr-x   0 andycasey   (501) staff       (20)        0 2024-05-21 12:28:42.682489 ads-0.12.6/ads/tests/stubdata/
+-rw-r--r--   0 andycasey   (501) staff       (20)        0 2022-10-14 01:29:43.000000 ads-0.12.6/ads/tests/stubdata/__init__.py
+-rw-r--r--   0 andycasey   (501) staff       (20)     1020 2022-10-14 01:29:43.000000 ads-0.12.6/ads/tests/stubdata/export.py
+-rw-r--r--   0 andycasey   (501) staff       (20)    18919 2022-10-14 01:29:43.000000 ads-0.12.6/ads/tests/stubdata/metrics.py
+-rw-r--r--   0 andycasey   (501) staff       (20)    74823 2022-10-14 01:29:43.000000 ads-0.12.6/ads/tests/stubdata/solr.py
+-rw-r--r--   0 andycasey   (501) staff       (20)     5799 2024-05-21 12:06:26.000000 ads-0.12.6/ads/tests/test_base.py
+-rw-r--r--   0 andycasey   (501) staff       (20)     1552 2024-05-21 12:06:26.000000 ads-0.12.6/ads/tests/test_export.py
+-rw-r--r--   0 andycasey   (501) staff       (20)     1527 2024-05-21 12:06:26.000000 ads-0.12.6/ads/tests/test_metrics.py
+-rw-r--r--   0 andycasey   (501) staff       (20)     2077 2024-05-21 12:06:26.000000 ads-0.12.6/ads/tests/test_sandbox.py
+-rw-r--r--   0 andycasey   (501) staff       (20)    15478 2024-05-21 12:06:26.000000 ads-0.12.6/ads/tests/test_search.py
+-rw-r--r--   0 andycasey   (501) staff       (20)     1110 2024-05-21 12:06:26.000000 ads-0.12.6/ads/tests/test_utils.py
+-rw-r--r--   0 andycasey   (501) staff       (20)     1150 2024-05-21 12:06:28.000000 ads-0.12.6/ads/utils.py
+drwxr-xr-x   0 andycasey   (501) staff       (20)        0 2024-05-21 12:28:42.682922 ads-0.12.6/ads.egg-info/
+-rw-r--r--   0 andycasey   (501) staff       (20)     1832 2024-05-21 12:28:42.000000 ads-0.12.6/ads.egg-info/PKG-INFO
+-rw-r--r--   0 andycasey   (501) staff       (20)      644 2024-05-21 12:28:42.000000 ads-0.12.6/ads.egg-info/SOURCES.txt
+-rw-r--r--   0 andycasey   (501) staff       (20)        1 2024-05-21 12:28:42.000000 ads-0.12.6/ads.egg-info/dependency_links.txt
+-rw-r--r--   0 andycasey   (501) staff       (20)       54 2024-05-21 12:28:42.000000 ads-0.12.6/ads.egg-info/requires.txt
+-rw-r--r--   0 andycasey   (501) staff       (20)        4 2024-05-21 12:28:42.000000 ads-0.12.6/ads.egg-info/top_level.txt
+-rw-r--r--   0 andycasey   (501) staff       (20)       27 2024-05-21 12:07:49.000000 ads-0.12.6/requirements.txt
+-rw-r--r--   0 andycasey   (501) staff       (20)       38 2024-05-21 12:28:42.683968 ads-0.12.6/setup.cfg
+-rw-r--r--   0 andycasey   (501) staff       (20)     1369 2024-05-21 12:28:21.000000 ads-0.12.6/setup.py
```

### Comparing `ads-0.12.4/LICENSE` & `ads-0.12.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/PKG-INFO` & `ads-0.12.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 Metadata-Version: 2.1
 Name: ads
-Version: 0.12.4
+Version: 0.12.6
 Summary: A Python module for NASA's ADS that doesn't suck.
 Home-page: http://www.github.com/andycasey/ads/
 Author: Andrew R. Casey
 Author-email: andy@astrowizici.st
 License: MIT
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: six
 Requires-Dist: requests
-Requires-Dist: httpretty>=0.8.10
 Requires-Dist: werkzeug
 Requires-Dist: mock
+Provides-Extra: tests
+Requires-Dist: httpretty>=0.8.10; extra == "tests"
 
-A Python Module to Interact with NASA's ADS that Doesn't Suck™
-==============================================================
+# A Python Module to Interact with NASA's ADS that Doesn't Suck™
 
-If you're in astro research, then you pretty much *need* NASA's ADS.
-It's tried, true, and people go crazy on the rare occasions when it goes down.
+If you're in astro research, then you pretty much *need* NASA's ADS. It's tried, true, and people go crazy on the rare occasions when it goes down.
 
 * Docs: https://ads.readthedocs.io/
 * Repo: https://github.com/andycasey/ads
 * PyPI: https://pypi.python.org/pypi/ads
 
-.. image:: https://travis-ci.org/andycasey/ads.svg?branch=master
-    :target: https://travis-ci.org/andycasey/ads
+[![Build Status](https://travis-ci.org/andycasey/ads.svg?branch=master)](https://travis-ci.org/andycasey/ads)
+[![Coverage Status](https://coveralls.io/repos/github/andycasey/ads/badge.svg?branch=master)](https://coveralls.io/github/andycasey/ads?branch=master)
 
-.. image:: https://coveralls.io/repos/github/andycasey/ads/badge.svg?branch=master
-    :target: https://coveralls.io/github/andycasey/ads?branch=master
+## Quickstart
 
-
-Quickstart
-==========
-
-   >>> import ads
-   >>> ads.config.token = 'secret token'
-   >>> papers = ads.SearchQuery(q="supernova", sort="citation_count")
-   >>> for paper in papers:
-   >>>    print(paper.title)
-   [u'Maps of Dust Infrared Emission for Use in Estimation of Reddening and Cosmic Microwave Background Radiation Foregrounds']
-   [u'Measurements of Omega and Lambda from 42 High-Redshift Supernovae']
-   [u'Observational Evidence from Supernovae for an Accelerating Universe and a Cosmological Constant']
-   [u'First-Year Wilkinson Microwave Anisotropy Probe (WMAP) Observations: Determination of Cosmological Parameters']
-   [u'Abundances of the elements: Meteoritic and solar']
-
-Running Tests
-=============
-
-   > cd /path/to/ads
-   > python -m unittest discover
+```python
+import ads
+ads.config.token = 'secret token'
+
+papers = ads.SearchQuery(q="supernova", sort="citation_count")
+for paper in papers:
+    print(paper.title[0])
+```
+
+You can expect to see some titles like this:
+```
+Maps of Dust Infrared Emission for Use in Estimation of Reddening and Cosmic Microwave Background Radiation Foregrounds
+Measurements of Omega and Lambda from 42 High-Redshift Supernovae
+Observational Evidence from Supernovae for an Accelerating Universe and a Cosmological Constant
+First-Year Wilkinson Microwave Anisotropy Probe (WMAP) Observations: Determination of Cosmological Parameters
+Abundances of the elements: Meteoritic and solar
+```
+
+## Running tests
+
+```bash
+cd /path/to/ads
+pip install -e . "ads[tests]"
+python -m unittest discover
+```
```

### Comparing `ads-0.12.4/ads/base.py` & `ads-0.12.6/ads/base.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads/config.py` & `ads-0.12.6/ads/config.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads/export.py` & `ads-0.12.6/ads/export.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads/libraries.py` & `ads-0.12.6/ads/libraries.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads/metrics.py` & `ads-0.12.6/ads/metrics.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads/sandbox.py` & `ads-0.12.6/ads/sandbox.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads/search.py` & `ads-0.12.6/ads/search.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads/tests/mocks.py` & `ads-0.12.6/ads/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads/tests/stubdata/export.py` & `ads-0.12.6/ads/tests/stubdata/export.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads/tests/stubdata/metrics.py` & `ads-0.12.6/ads/tests/stubdata/metrics.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads/tests/stubdata/solr.py` & `ads-0.12.6/ads/tests/stubdata/solr.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads/tests/test_base.py` & `ads-0.12.6/ads/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads/tests/test_export.py` & `ads-0.12.6/ads/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads/tests/test_metrics.py` & `ads-0.12.6/ads/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads/tests/test_sandbox.py` & `ads-0.12.6/ads/tests/test_sandbox.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads/tests/test_search.py` & `ads-0.12.6/ads/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads/tests/test_utils.py` & `ads-0.12.6/ads/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads/utils.py` & `ads-0.12.6/ads/utils.py`

 * *Files identical despite different names*

### Comparing `ads-0.12.4/ads.egg-info/PKG-INFO` & `ads-0.12.6/ads.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 Metadata-Version: 2.1
 Name: ads
-Version: 0.12.4
+Version: 0.12.6
 Summary: A Python module for NASA's ADS that doesn't suck.
 Home-page: http://www.github.com/andycasey/ads/
 Author: Andrew R. Casey
 Author-email: andy@astrowizici.st
 License: MIT
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: six
 Requires-Dist: requests
-Requires-Dist: httpretty>=0.8.10
 Requires-Dist: werkzeug
 Requires-Dist: mock
+Provides-Extra: tests
+Requires-Dist: httpretty>=0.8.10; extra == "tests"
 
-A Python Module to Interact with NASA's ADS that Doesn't Suck™
-==============================================================
+# A Python Module to Interact with NASA's ADS that Doesn't Suck™
 
-If you're in astro research, then you pretty much *need* NASA's ADS.
-It's tried, true, and people go crazy on the rare occasions when it goes down.
+If you're in astro research, then you pretty much *need* NASA's ADS. It's tried, true, and people go crazy on the rare occasions when it goes down.
 
 * Docs: https://ads.readthedocs.io/
 * Repo: https://github.com/andycasey/ads
 * PyPI: https://pypi.python.org/pypi/ads
 
-.. image:: https://travis-ci.org/andycasey/ads.svg?branch=master
-    :target: https://travis-ci.org/andycasey/ads
+[![Build Status](https://travis-ci.org/andycasey/ads.svg?branch=master)](https://travis-ci.org/andycasey/ads)
+[![Coverage Status](https://coveralls.io/repos/github/andycasey/ads/badge.svg?branch=master)](https://coveralls.io/github/andycasey/ads?branch=master)
 
-.. image:: https://coveralls.io/repos/github/andycasey/ads/badge.svg?branch=master
-    :target: https://coveralls.io/github/andycasey/ads?branch=master
+## Quickstart
 
-
-Quickstart
-==========
-
-   >>> import ads
-   >>> ads.config.token = 'secret token'
-   >>> papers = ads.SearchQuery(q="supernova", sort="citation_count")
-   >>> for paper in papers:
-   >>>    print(paper.title)
-   [u'Maps of Dust Infrared Emission for Use in Estimation of Reddening and Cosmic Microwave Background Radiation Foregrounds']
-   [u'Measurements of Omega and Lambda from 42 High-Redshift Supernovae']
-   [u'Observational Evidence from Supernovae for an Accelerating Universe and a Cosmological Constant']
-   [u'First-Year Wilkinson Microwave Anisotropy Probe (WMAP) Observations: Determination of Cosmological Parameters']
-   [u'Abundances of the elements: Meteoritic and solar']
-
-Running Tests
-=============
-
-   > cd /path/to/ads
-   > python -m unittest discover
+```python
+import ads
+ads.config.token = 'secret token'
+
+papers = ads.SearchQuery(q="supernova", sort="citation_count")
+for paper in papers:
+    print(paper.title[0])
+```
+
+You can expect to see some titles like this:
+```
+Maps of Dust Infrared Emission for Use in Estimation of Reddening and Cosmic Microwave Background Radiation Foregrounds
+Measurements of Omega and Lambda from 42 High-Redshift Supernovae
+Observational Evidence from Supernovae for an Accelerating Universe and a Cosmological Constant
+First-Year Wilkinson Microwave Anisotropy Probe (WMAP) Observations: Determination of Cosmological Parameters
+Abundances of the elements: Meteoritic and solar
+```
+
+## Running tests
+
+```bash
+cd /path/to/ads
+pip install -e . "ads[tests]"
+python -m unittest discover
+```
```

### Comparing `ads-0.12.4/ads.egg-info/SOURCES.txt` & `ads-0.12.6/ads.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 requirements.txt
 setup.py
 ads/__init__.py
 ads/base.py
 ads/config.py
 ads/exceptions.py
 ads/export.py
```

### Comparing `ads-0.12.4/setup.py` & `ads-0.12.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,11 +35,17 @@
       author="Andrew R. Casey",
       author_email="andy@astrowizici.st",
       packages=["ads", "ads.tests", "ads.tests.stubdata"],
       url="http://www.github.com/andycasey/ads/",
       license="MIT",
       description="A Python module for NASA's ADS that doesn't suck.",
       long_description=\
-          readfile(os.path.join(os.path.dirname(__file__), "README.rst")),
+          readfile(os.path.join(os.path.dirname(__file__), "README.md")),
       install_requires=\
-          readfile(os.path.join(os.path.dirname(__file__), "requirements.txt"))
+          readfile(os.path.join(os.path.dirname(__file__), "requirements.txt")),
+      long_description_content_type="text/markdown",
+      extras_require={
+          "tests": [
+            "httpretty>=0.8.10",
+          ]
+      }
      )
```

