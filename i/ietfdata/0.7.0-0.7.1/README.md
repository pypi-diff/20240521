# Comparing `tmp/ietfdata-0.7.0.tar.gz` & `tmp/ietfdata-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ietfdata-0.7.0.tar", last modified: Fri Apr 19 10:53:13 2024, max compression
+gzip compressed data, was "ietfdata-0.7.1.tar", last modified: Tue May 21 08:14:22 2024, max compression
```

## Comparing `ietfdata-0.7.0.tar` & `ietfdata-0.7.1.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwx---   0 csp        (502) staff       (20)        0 2024-04-19 10:53:13.809322 ietfdata-0.7.0/
--rw-r--r--   0 csp        (502) staff       (20)     1294 2021-04-14 11:17:29.000000 ietfdata-0.7.0/LICENSE
--rw-r--r--   0 csp        (502) staff       (20)     3478 2024-04-19 10:53:13.809139 ietfdata-0.7.0/PKG-INFO
--rw-rw----   0 csp        (502) staff       (20)     2529 2023-06-21 08:17:16.000000 ietfdata-0.7.0/README.md
-drwxrwx---   0 csp        (502) staff       (20)        0 2024-04-19 10:53:13.804970 ietfdata-0.7.0/examples/
--rw-rw----   0 csp        (502) staff       (20)        0 2020-08-04 12:44:47.000000 ietfdata-0.7.0/examples/__init__.py
--rw-rw----   0 csp        (502) staff       (20)     2037 2022-10-28 12:45:40.000000 ietfdata-0.7.0/examples/bluesheets.py
--rw-r--r--   0 csp        (502) staff       (20)     2223 2021-04-14 11:17:29.000000 ietfdata-0.7.0/examples/draft-authors.py
--rw-rw----   0 csp        (502) staff       (20)     2163 2022-10-28 12:50:08.000000 ietfdata-0.7.0/examples/draft-references.py
--rw-rw----   0 csp        (502) staff       (20)     2748 2021-12-02 17:45:56.000000 ietfdata-0.7.0/examples/draft-submissions-by-date.py
--rw-rw----   0 csp        (502) staff       (20)     1756 2023-11-24 13:32:11.000000 ietfdata-0.7.0/examples/draft-submissions.py
--rw-rw----   0 csp        (502) staff       (20)     1814 2022-06-27 14:31:39.000000 ietfdata-0.7.0/examples/drafts-for-person.py
--rw-r--r--   0 csp        (502) staff       (20)     1799 2022-10-28 13:00:03.000000 ietfdata-0.7.0/examples/drafts-for-rfc.py
--rw-r--r--   0 csp        (502) staff       (20)     1981 2021-04-14 11:17:29.000000 ietfdata-0.7.0/examples/drafts-for-wg.py
--rw-rw----   0 csp        (502) staff       (20)     2910 2022-10-28 13:08:25.000000 ietfdata-0.7.0/examples/emails-per-person.py
--rw-rw----   0 csp        (502) staff       (20)     4006 2024-01-20 17:43:00.000000 ietfdata-0.7.0/examples/iesg-processing-time.py
--rw-r--r--   0 csp        (502) staff       (20)     2773 2021-04-14 11:17:29.000000 ietfdata-0.7.0/examples/ietf-leadership.py
--rw-rw----   0 csp        (502) staff       (20)     1842 2022-10-28 12:36:22.000000 ietfdata-0.7.0/examples/non-wg-standards-track-rfcs.py
--rw-r--r--   0 csp        (502) staff       (20)     2214 2023-11-19 18:26:39.000000 ietfdata-0.7.0/examples/org-chart.py
--rw-rw----   0 csp        (502) staff       (20)     1995 2022-12-10 15:03:43.000000 ietfdata-0.7.0/examples/person-attendance.py
--rw-rw----   0 csp        (502) staff       (20)     1776 2022-10-28 15:37:24.000000 ietfdata-0.7.0/examples/person-emails.py
--rw-rw----   0 csp        (502) staff       (20)     7955 2022-10-28 15:48:45.000000 ietfdata-0.7.0/examples/person.py
--rw-r-----   0 csp        (502) staff       (20)     2203 2023-04-19 18:40:26.000000 ietfdata-0.7.0/examples/recent-pubreq.py
--rw-r--r--   0 csp        (502) staff       (20)     5567 2022-10-28 15:51:05.000000 ietfdata-0.7.0/examples/rfc-data.py
--rw-rw----   0 csp        (502) staff       (20)     1911 2023-11-26 14:57:50.000000 ietfdata-0.7.0/examples/rfc-per-year.py
--rw-rw----   0 csp        (502) staff       (20)     2155 2021-08-27 12:26:02.000000 ietfdata-0.7.0/examples/rfc-streams.py
--rw-r--r--   0 csp        (502) staff       (20)     2055 2021-04-14 11:17:29.000000 ietfdata-0.7.0/examples/role-names.py
-drwxrwx---   0 csp        (502) staff       (20)        0 2024-04-19 10:53:13.806656 ietfdata-0.7.0/ietfdata/
--rw-rw----   0 csp        (502) staff       (20)        0 2020-04-11 11:24:32.000000 ietfdata-0.7.0/ietfdata/__init__.py
--rw-rw----   0 csp        (502) staff       (20)   158330 2024-03-17 21:44:16.000000 ietfdata-0.7.0/ietfdata/datatracker.py
--rw-rw----   0 csp        (502) staff       (20)    16790 2023-12-27 18:19:57.000000 ietfdata-0.7.0/ietfdata/datatracker_ext.py
--rw-rw----   0 csp        (502) staff       (20)    38885 2024-04-02 14:53:19.000000 ietfdata-0.7.0/ietfdata/mailarchive2.py
--rw-rw----   0 csp        (502) staff       (20)        0 2020-04-11 11:24:32.000000 ietfdata-0.7.0/ietfdata/py.typed
--rw-rw----   0 csp        (502) staff       (20)    25180 2023-11-23 08:45:26.000000 ietfdata-0.7.0/ietfdata/rfcindex.py
-drwxrwx---   0 csp        (502) staff       (20)        0 2024-04-19 10:53:13.808942 ietfdata-0.7.0/ietfdata.egg-info/
--rw-r--r--   0 csp        (502) staff       (20)     3478 2024-04-19 10:53:13.000000 ietfdata-0.7.0/ietfdata.egg-info/PKG-INFO
--rw-rw----   0 csp        (502) staff       (20)     1045 2024-04-19 10:53:13.000000 ietfdata-0.7.0/ietfdata.egg-info/SOURCES.txt
--rw-rw----   0 csp        (502) staff       (20)        1 2024-04-19 10:53:13.000000 ietfdata-0.7.0/ietfdata.egg-info/dependency_links.txt
--rw-rw----   0 csp        (502) staff       (20)      206 2024-04-19 10:53:13.000000 ietfdata-0.7.0/ietfdata.egg-info/requires.txt
--rw-rw----   0 csp        (502) staff       (20)       18 2024-04-19 10:53:13.000000 ietfdata-0.7.0/ietfdata.egg-info/top_level.txt
--rw-rw----   0 csp        (502) staff       (20)      779 2023-12-27 19:59:03.000000 ietfdata-0.7.0/pyproject.toml
--rw-rw----   0 csp        (502) staff       (20)       38 2024-04-19 10:53:13.809357 ietfdata-0.7.0/setup.cfg
--rw-rw----   0 csp        (502) staff       (20)      806 2023-12-27 19:39:54.000000 ietfdata-0.7.0/setup.py
-drwxrwx---   0 csp        (502) staff       (20)        0 2024-04-19 10:53:13.808754 ietfdata-0.7.0/tests/
--rw-rw----   0 csp        (502) staff       (20)   232033 2024-03-24 20:51:25.000000 ietfdata-0.7.0/tests/test_datatracker.py
--rw-rw----   0 csp        (502) staff       (20)     5952 2023-12-20 17:52:07.000000 ietfdata-0.7.0/tests/test_datatracker_coverage.py
--rw-rw----   0 csp        (502) staff       (20)     2908 2023-11-10 13:10:13.000000 ietfdata-0.7.0/tests/test_mailarchive2.py
--rw-rw----   0 csp        (502) staff       (20)     7034 2022-07-04 08:34:17.000000 ietfdata-0.7.0/tests/test_rfcindex.py
+drwxrwx---   0 csp        (502) staff       (20)        0 2024-05-21 08:14:22.702662 ietfdata-0.7.1/
+-rw-r--r--   0 csp        (502) staff       (20)     1294 2021-04-14 11:17:29.000000 ietfdata-0.7.1/LICENSE
+-rw-r--r--   0 csp        (502) staff       (20)     3478 2024-05-21 08:14:22.702464 ietfdata-0.7.1/PKG-INFO
+-rw-rw----   0 csp        (502) staff       (20)     2529 2023-06-21 08:17:16.000000 ietfdata-0.7.1/README.md
+drwxrwx---   0 csp        (502) staff       (20)        0 2024-05-21 08:14:22.694080 ietfdata-0.7.1/examples/
+-rw-rw----   0 csp        (502) staff       (20)        0 2020-08-04 12:44:47.000000 ietfdata-0.7.1/examples/__init__.py
+-rw-rw----   0 csp        (502) staff       (20)     2037 2022-10-28 12:45:40.000000 ietfdata-0.7.1/examples/bluesheets.py
+-rw-r--r--   0 csp        (502) staff       (20)     2223 2021-04-14 11:17:29.000000 ietfdata-0.7.1/examples/draft-authors.py
+-rw-rw----   0 csp        (502) staff       (20)     2163 2022-10-28 12:50:08.000000 ietfdata-0.7.1/examples/draft-references.py
+-rw-rw----   0 csp        (502) staff       (20)     2748 2021-12-02 17:45:56.000000 ietfdata-0.7.1/examples/draft-submissions-by-date.py
+-rw-rw----   0 csp        (502) staff       (20)     1756 2023-11-24 13:32:11.000000 ietfdata-0.7.1/examples/draft-submissions.py
+-rw-rw----   0 csp        (502) staff       (20)     1814 2022-06-27 14:31:39.000000 ietfdata-0.7.1/examples/drafts-for-person.py
+-rw-r--r--   0 csp        (502) staff       (20)     1799 2022-10-28 13:00:03.000000 ietfdata-0.7.1/examples/drafts-for-rfc.py
+-rw-r--r--   0 csp        (502) staff       (20)     1981 2021-04-14 11:17:29.000000 ietfdata-0.7.1/examples/drafts-for-wg.py
+-rw-rw----   0 csp        (502) staff       (20)     2910 2022-10-28 13:08:25.000000 ietfdata-0.7.1/examples/emails-per-person.py
+-rw-rw----   0 csp        (502) staff       (20)     4006 2024-01-20 17:43:00.000000 ietfdata-0.7.1/examples/iesg-processing-time.py
+-rw-r--r--   0 csp        (502) staff       (20)     2773 2021-04-14 11:17:29.000000 ietfdata-0.7.1/examples/ietf-leadership.py
+-rw-rw----   0 csp        (502) staff       (20)     1842 2022-10-28 12:36:22.000000 ietfdata-0.7.1/examples/non-wg-standards-track-rfcs.py
+-rw-r--r--   0 csp        (502) staff       (20)     2214 2023-11-19 18:26:39.000000 ietfdata-0.7.1/examples/org-chart.py
+-rw-rw----   0 csp        (502) staff       (20)     1995 2022-12-10 15:03:43.000000 ietfdata-0.7.1/examples/person-attendance.py
+-rw-rw----   0 csp        (502) staff       (20)     1776 2022-10-28 15:37:24.000000 ietfdata-0.7.1/examples/person-emails.py
+-rw-rw----   0 csp        (502) staff       (20)     7955 2022-10-28 15:48:45.000000 ietfdata-0.7.1/examples/person.py
+-rw-r-----   0 csp        (502) staff       (20)     2203 2023-04-19 18:40:26.000000 ietfdata-0.7.1/examples/recent-pubreq.py
+-rw-r--r--   0 csp        (502) staff       (20)     5567 2022-10-28 15:51:05.000000 ietfdata-0.7.1/examples/rfc-data.py
+-rw-rw----   0 csp        (502) staff       (20)     2319 2024-05-10 14:51:11.000000 ietfdata-0.7.1/examples/rfc-per-year-ietf.py
+-rw-rw----   0 csp        (502) staff       (20)     1911 2023-11-26 14:57:50.000000 ietfdata-0.7.1/examples/rfc-per-year.py
+-rw-rw----   0 csp        (502) staff       (20)     2155 2021-08-27 12:26:02.000000 ietfdata-0.7.1/examples/rfc-streams.py
+-rw-r--r--   0 csp        (502) staff       (20)     2055 2021-04-14 11:17:29.000000 ietfdata-0.7.1/examples/role-names.py
+drwxrwx---   0 csp        (502) staff       (20)        0 2024-05-21 08:14:22.697922 ietfdata-0.7.1/ietfdata/
+-rw-rw----   0 csp        (502) staff       (20)        0 2020-04-11 11:24:32.000000 ietfdata-0.7.1/ietfdata/__init__.py
+-rw-rw----   0 csp        (502) staff       (20)   158330 2024-05-21 08:01:37.000000 ietfdata-0.7.1/ietfdata/datatracker.py
+-rw-rw----   0 csp        (502) staff       (20)    16790 2024-05-10 19:57:00.000000 ietfdata-0.7.1/ietfdata/datatracker_ext.py
+-rw-rw----   0 csp        (502) staff       (20)    39230 2024-05-06 10:44:17.000000 ietfdata-0.7.1/ietfdata/mailarchive2.py
+-rw-rw----   0 csp        (502) staff       (20)        0 2020-04-11 11:24:32.000000 ietfdata-0.7.1/ietfdata/py.typed
+-rw-rw----   0 csp        (502) staff       (20)    25180 2023-11-23 08:45:26.000000 ietfdata-0.7.1/ietfdata/rfcindex.py
+drwxrwx---   0 csp        (502) staff       (20)        0 2024-05-21 08:14:22.702253 ietfdata-0.7.1/ietfdata.egg-info/
+-rw-r--r--   0 csp        (502) staff       (20)     3478 2024-05-21 08:14:22.000000 ietfdata-0.7.1/ietfdata.egg-info/PKG-INFO
+-rw-rw----   0 csp        (502) staff       (20)     1075 2024-05-21 08:14:22.000000 ietfdata-0.7.1/ietfdata.egg-info/SOURCES.txt
+-rw-rw----   0 csp        (502) staff       (20)        1 2024-05-21 08:14:22.000000 ietfdata-0.7.1/ietfdata.egg-info/dependency_links.txt
+-rw-rw----   0 csp        (502) staff       (20)      206 2024-05-21 08:14:22.000000 ietfdata-0.7.1/ietfdata.egg-info/requires.txt
+-rw-rw----   0 csp        (502) staff       (20)       18 2024-05-21 08:14:22.000000 ietfdata-0.7.1/ietfdata.egg-info/top_level.txt
+-rw-rw----   0 csp        (502) staff       (20)      779 2024-05-21 08:10:30.000000 ietfdata-0.7.1/pyproject.toml
+-rw-rw----   0 csp        (502) staff       (20)       38 2024-05-21 08:14:22.702713 ietfdata-0.7.1/setup.cfg
+-rw-rw----   0 csp        (502) staff       (20)      806 2024-05-21 08:01:23.000000 ietfdata-0.7.1/setup.py
+drwxrwx---   0 csp        (502) staff       (20)        0 2024-05-21 08:14:22.701720 ietfdata-0.7.1/tests/
+-rw-rw----   0 csp        (502) staff       (20)   232033 2024-05-20 08:00:08.000000 ietfdata-0.7.1/tests/test_datatracker.py
+-rw-rw----   0 csp        (502) staff       (20)     5952 2023-12-20 17:52:07.000000 ietfdata-0.7.1/tests/test_datatracker_coverage.py
+-rw-rw----   0 csp        (502) staff       (20)     2908 2023-11-10 13:10:13.000000 ietfdata-0.7.1/tests/test_mailarchive2.py
+-rw-rw----   0 csp        (502) staff       (20)     7034 2022-07-04 08:34:17.000000 ietfdata-0.7.1/tests/test_rfcindex.py
```

### Comparing `ietfdata-0.7.0/LICENSE` & `ietfdata-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/PKG-INFO` & `ietfdata-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ietfdata
-Version: 0.7.0
+Version: 0.7.1
 Summary: Access the IETF Data Tracker and RFC Index
 Home-page: https://github.com/glasgow-ipl/ietfdata
 Author: Colin Perkins
 Author-email: Colin Perkins <csp@csperkins.org>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ietfdata-0.7.0/README.md` & `ietfdata-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/bluesheets.py` & `ietfdata-0.7.1/examples/bluesheets.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/draft-authors.py` & `ietfdata-0.7.1/examples/draft-authors.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/draft-references.py` & `ietfdata-0.7.1/examples/draft-references.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/draft-submissions-by-date.py` & `ietfdata-0.7.1/examples/draft-submissions-by-date.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/draft-submissions.py` & `ietfdata-0.7.1/examples/draft-submissions.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/drafts-for-person.py` & `ietfdata-0.7.1/examples/drafts-for-person.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/drafts-for-rfc.py` & `ietfdata-0.7.1/examples/drafts-for-rfc.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/drafts-for-wg.py` & `ietfdata-0.7.1/examples/drafts-for-wg.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/emails-per-person.py` & `ietfdata-0.7.1/examples/emails-per-person.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/iesg-processing-time.py` & `ietfdata-0.7.1/examples/iesg-processing-time.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/ietf-leadership.py` & `ietfdata-0.7.1/examples/ietf-leadership.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/non-wg-standards-track-rfcs.py` & `ietfdata-0.7.1/examples/non-wg-standards-track-rfcs.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/org-chart.py` & `ietfdata-0.7.1/examples/org-chart.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/person-attendance.py` & `ietfdata-0.7.1/examples/person-attendance.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/person-emails.py` & `ietfdata-0.7.1/examples/person-emails.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/person.py` & `ietfdata-0.7.1/examples/person.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/recent-pubreq.py` & `ietfdata-0.7.1/examples/recent-pubreq.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/rfc-data.py` & `ietfdata-0.7.1/examples/rfc-data.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/rfc-per-year.py` & `ietfdata-0.7.1/examples/rfc-per-year.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/rfc-streams.py` & `ietfdata-0.7.1/examples/rfc-streams.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/examples/role-names.py` & `ietfdata-0.7.1/examples/role-names.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/ietfdata/datatracker.py` & `ietfdata-0.7.1/ietfdata/datatracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1618,15 +1618,15 @@
         logging.getLogger('requests').setLevel('ERROR')
         logging.getLogger('requests_cache').setLevel('ERROR')
         logging.getLogger("urllib3").setLevel('ERROR')
 
         logging.basicConfig(level=os.environ.get("IETFDATA_LOGLEVEL", "INFO"))
         self.log = logging.getLogger("ietfdata")
 
-        self.ua        = "glasgow-ietfdata/0.7.0"          # Update when making a new relaase
+        self.ua        = "glasgow-ietfdata/0.7.1"          # Update when making a new relaase
         self.base_url  = os.environ.get("IETFDATA_DT_URL", "https://datatracker.ietf.org")
         self.get_count = 0
 
         if use_cache:
             self.log.warning(f"mongodb host = {mongodb_host}")
             self.log.warning(f"mongodb port = {mongodb_port}")
             self.log.warning(f"mongodb user = {mongodb_user}")
```

### Comparing `ietfdata-0.7.0/ietfdata/datatracker_ext.py` & `ietfdata-0.7.1/ietfdata/datatracker_ext.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/ietfdata/mailarchive2.py` & `ietfdata-0.7.1/ietfdata/mailarchive2.py`

 * *Files 0% similar despite different names*

```diff
@@ -586,57 +586,58 @@
         If the first message in the thread was only sent to a single mailing
         list, then the message-id for the thread will map onto a list with a
         single Envelope.
         """
         threads = {}
         seen    = {} # type: Dict[str,Envelope]
         for msg in self.messages():
-            msg_id  = msg.header("message-id")[0]
-            seen[msg_id] = msg
-
-            self._log.debug(f"{msg.uid():5} {msg.header('message-id')} {msg.header('subject')}")
-
-            parents = msg.in_reply_to()
-            if len(parents) == 0:
-                # This is the first message in the thread
-                if msg.header("message-id")[0] not in threads:
-                    threads[msg.header("message-id")[0]] = [msg]
-                self._log.debug("      First in thread")
-            elif parents[0].header("message-id")[0] in seen:
-                # This is part of a thread we've already seen
-                self._log.debug(f"      {parents[0].header('message-id')} {parents[0].header('subject')}")
-                self._log.debug(f"      Continues known thread")
-            else:
-                # This is either a new thread that has been copied to this list
-                # where the earlier messages in the thread are on another list,
-                # or this message is part of an existing thread but has arrived
-                # before its parent.
-                curr = []
-                curr.append(msg)
-                while True:
-                    parents = curr[0].in_reply_to()
-
-                    parent_in_this_list = False
-                    for p in parents:
-                        if p.mailing_list() == self.name():
-                            parent_in_this_list = True
-                    if not parent_in_this_list and this_list_only:
-                        self._log.debug(f"      {parents[0].header('message-id')} {parents[0].header('subject')}")
-                        self._log.debug(f"      Not in this list")
-                        if curr[0].header("message-id")[0] not in threads:
-                            threads[curr[0].header("message-id")[0]] = curr
-                        break
-
-                    if len(parents) == 0:
-                        self._log.debug("      First in thread")
-                        if curr[0].header("message-id")[0] not in threads:
-                            threads[curr[0].header("message-id")[0]] = curr
-                        break
-                    curr = parents
-                    self._log.debug(f"      {curr[0].header('message-id')} {curr[0].header('subject')}")
+            if len(msg.header("message-id")) > 0:
+                msg_id  = msg.header("message-id")[0]
+                seen[msg_id] = msg
+    
+                self._log.debug(f"{msg.uid():5} {msg.header('message-id')} {msg.header('subject')}")
+    
+                parents = msg.in_reply_to()
+                if len(parents) == 0:
+                    # This is the first message in the thread
+                    if msg.header("message-id")[0] not in threads:
+                        threads[msg.header("message-id")[0]] = [msg]
+                    self._log.debug("      First in thread")
+                elif parents[0].header("message-id")[0] in seen:
+                    # This is part of a thread we've already seen
+                    self._log.debug(f"      {parents[0].header('message-id')} {parents[0].header('subject')}")
+                    self._log.debug(f"      Continues known thread")
+                else:
+                    # This is either a new thread that has been copied to this list
+                    # where the earlier messages in the thread are on another list,
+                    # or this message is part of an existing thread but has arrived
+                    # before its parent.
+                    curr = []
+                    curr.append(msg)
+                    while True:
+                        parents = curr[0].in_reply_to()
+    
+                        parent_in_this_list = False
+                        for p in parents:
+                            if p.mailing_list() == self.name():
+                                parent_in_this_list = True
+                        if not parent_in_this_list and this_list_only:
+                            self._log.debug(f"      {parents[0].header('message-id')} {parents[0].header('subject')}")
+                            self._log.debug(f"      Not in this list")
+                            if curr[0].header("message-id")[0] not in threads:
+                                threads[curr[0].header("message-id")[0]] = curr
+                            break
+    
+                        if len(parents) == 0:
+                            self._log.debug("      First in thread")
+                            if curr[0].header("message-id")[0] not in threads:
+                                threads[curr[0].header("message-id")[0]] = curr
+                            break
+                        curr = parents
+                        self._log.debug(f"      {curr[0].header('message-id')} {curr[0].header('subject')}")
         return threads
 
 
     def add_metadata(self, project:str, key:str, value):
         """
         Add metadata relating to the list.
 
@@ -755,14 +756,16 @@
                                         ('uidvalidity', ASCENDING), 
                                         ('uid', ASCENDING),
                                         ('project', ASCENDING),
                                         ('key', ASCENDING),
                                        ], unique=False)
         self._db.metadata.create_index([('message_id', ASCENDING)
                                        ], unique=False)
+        self._db.metadata.create_index([('in_reply_to', ASCENDING)
+                                       ], unique=False)
         self._fs = GridFS(self._db)
         # Create other state:
         self._mailing_lists = {}
 
 
     def mailing_list_names(self) -> Iterator[str]:
         """
```

### Comparing `ietfdata-0.7.0/ietfdata/rfcindex.py` & `ietfdata-0.7.1/ietfdata/rfcindex.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/ietfdata.egg-info/PKG-INFO` & `ietfdata-0.7.1/ietfdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ietfdata
-Version: 0.7.0
+Version: 0.7.1
 Summary: Access the IETF Data Tracker and RFC Index
 Home-page: https://github.com/glasgow-ipl/ietfdata
 Author: Colin Perkins
 Author-email: Colin Perkins <csp@csperkins.org>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ietfdata-0.7.0/ietfdata.egg-info/SOURCES.txt` & `ietfdata-0.7.1/ietfdata.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 examples/non-wg-standards-track-rfcs.py
 examples/org-chart.py
 examples/person-attendance.py
 examples/person-emails.py
 examples/person.py
 examples/recent-pubreq.py
 examples/rfc-data.py
+examples/rfc-per-year-ietf.py
 examples/rfc-per-year.py
 examples/rfc-streams.py
 examples/role-names.py
 ietfdata/__init__.py
 ietfdata/datatracker.py
 ietfdata/datatracker_ext.py
 ietfdata/mailarchive2.py
```

### Comparing `ietfdata-0.7.0/pyproject.toml` & `ietfdata-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name    = "ietfdata"
-version = "0.7.0"
+version = "0.7.1"
 authors = [
   {name = "Colin Perkins", email = "csp@csperkins.org"}
 ]
 description = "Access the IETF Data Tracker and RFC Index"
 readme = "README.md"
 requires-python = '>=3.11'
 classifiers = [
```

### Comparing `ietfdata-0.7.0/setup.py` & `ietfdata-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ietfdata",
-    version="0.7.0",
+    version="0.7.1",
     author="Colin Perkins",
     author_email="csp@csperkins.org",
     description="Access the IETF Data Tracker and RFC Index",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/glasgow-ipl/ietfdata",
     packages=setuptools.find_packages(),
```

### Comparing `ietfdata-0.7.0/tests/test_datatracker.py` & `ietfdata-0.7.1/tests/test_datatracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1884,15 +1884,15 @@
     def test_group_role_histories(self) -> None:
         group_role_histories = self.dt.group_role_histories()
         self.assertIsNot(group_role_histories, None)
 
 
     def test_group_role_histories_email(self) -> None:
         group_role_histories = list(self.dt.group_role_histories(email="csp@csperkins.org"))
-        self.assertEqual(len(group_role_histories), 84)
+        self.assertEqual(len(group_role_histories), 87)
 
 
     def test_group_role_histories_group(self) -> None:
         group_role_histories = list(self.dt.group_role_histories(group=self.dt.group_history(GroupHistoryURI(uri="/api/v1/group/grouphistory/256/"))))
         self.assertEqual(len(group_role_histories), 1)
         self.assertEqual(group_role_histories[0].id, 519)
 
@@ -1900,15 +1900,15 @@
     def test_group_role_histories_name(self) -> None:
         group_role_histories = self.dt.group_role_histories(name=self.dt.role_name(RoleNameURI(uri="/api/v1/name/rolename/chair/")))
         self.assertIsNot(group_role_histories, None)
 
 
     def test_group_role_histories_person(self) -> None:
         group_role_histories = list(self.dt.group_role_histories(person=self.dt.person(PersonURI(uri="/api/v1/person/person/20209/"))))
-        self.assertEqual(len(group_role_histories), 84)
+        self.assertEqual(len(group_role_histories), 87)
 
 
     def test_group_state_change_event(self) -> None:
         group_state_change_event = self.dt.group_state_change_event(GroupStateChangeEventURI(uri="/api/v1/group/changestategroupevent/16833/"))
         if group_state_change_event is not None:
             self.assertEqual(group_state_change_event.by,             PersonURI(uri="/api/v1/person/person/106842/"))
             self.assertEqual(group_state_change_event.desc,           "State changed to <b>Proposed</b> from Unknown")
```

### Comparing `ietfdata-0.7.0/tests/test_datatracker_coverage.py` & `ietfdata-0.7.1/tests/test_datatracker_coverage.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/tests/test_mailarchive2.py` & `ietfdata-0.7.1/tests/test_mailarchive2.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.7.0/tests/test_rfcindex.py` & `ietfdata-0.7.1/tests/test_rfcindex.py`

 * *Files identical despite different names*

