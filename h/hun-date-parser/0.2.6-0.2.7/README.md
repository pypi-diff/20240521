# Comparing `tmp/hun-date-parser-0.2.6.tar.gz` & `tmp/hun-date-parser-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hun-date-parser-0.2.6.tar", last modified: Thu Apr 25 09:22:34 2024, max compression
+gzip compressed data, was "hun-date-parser-0.2.7.tar", last modified: Tue May 21 18:48:26 2024, max compression
```

## Comparing `hun-date-parser-0.2.6.tar` & `hun-date-parser-0.2.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 soma       (501) staff       (20)        0 2024-04-25 09:22:34.392316 hun-date-parser-0.2.6/
--rw-r--r--   0 soma       (501) staff       (20)     1035 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/LICENSE
--rw-r--r--   0 soma       (501) staff       (20)     8019 2024-04-25 09:22:34.392068 hun-date-parser-0.2.6/PKG-INFO
--rw-r--r--   0 soma       (501) staff       (20)     7888 2024-04-25 08:49:49.000000 hun-date-parser-0.2.6/README.md
-drwxr-xr-x   0 soma       (501) staff       (20)        0 2024-04-25 09:22:34.385663 hun-date-parser-0.2.6/hun_date_parser/
--rw-r--r--   0 soma       (501) staff       (20)      354 2024-04-25 09:07:55.000000 hun-date-parser-0.2.6/hun_date_parser/__init__.py
-drwxr-xr-x   0 soma       (501) staff       (20)        0 2024-04-25 09:22:34.387427 hun-date-parser-0.2.6/hun_date_parser/date_parser/
--rw-r--r--   0 soma       (501) staff       (20)        0 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/hun_date_parser/date_parser/__init__.py
--rw-r--r--   0 soma       (501) staff       (20)    20502 2024-04-25 08:41:37.000000 hun-date-parser-0.2.6/hun_date_parser/date_parser/date_parsers.py
--rw-r--r--   0 soma       (501) staff       (20)    18810 2024-04-25 09:18:43.000000 hun-date-parser-0.2.6/hun_date_parser/date_parser/datetime_extractor.py
-drwxr-xr-x   0 soma       (501) staff       (20)        0 2024-04-25 09:22:34.387999 hun-date-parser-0.2.6/hun_date_parser/date_parser/interval_restriction/
--rw-r--r--   0 soma       (501) staff       (20)      223 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/hun_date_parser/date_parser/interval_restriction/__init__.py
--rw-r--r--   0 soma       (501) staff       (20)     5805 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/hun_date_parser/date_parser/interval_restriction/restricted_parsing.py
--rw-r--r--   0 soma       (501) staff       (20)     5371 2024-04-25 08:31:35.000000 hun-date-parser-0.2.6/hun_date_parser/date_parser/patterns.py
--rw-r--r--   0 soma       (501) staff       (20)     2643 2024-04-25 06:59:36.000000 hun-date-parser-0.2.6/hun_date_parser/date_parser/structure_parsers.py
--rw-r--r--   0 soma       (501) staff       (20)     8862 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/hun_date_parser/date_parser/time_parsers.py
-drwxr-xr-x   0 soma       (501) staff       (20)        0 2024-04-25 09:22:34.388947 hun-date-parser-0.2.6/hun_date_parser/date_textualizer/
--rw-r--r--   0 soma       (501) staff       (20)        0 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/hun_date_parser/date_textualizer/__init__.py
--rw-r--r--   0 soma       (501) staff       (20)     1439 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/hun_date_parser/date_textualizer/date2text.py
--rw-r--r--   0 soma       (501) staff       (20)     2161 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/hun_date_parser/date_textualizer/datetime_textualizer.py
--rw-r--r--   0 soma       (501) staff       (20)     4182 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/hun_date_parser/date_textualizer/time2text.py
-drwxr-xr-x   0 soma       (501) staff       (20)        0 2024-04-25 09:22:34.389910 hun-date-parser-0.2.6/hun_date_parser/utils/
--rw-r--r--   0 soma       (501) staff       (20)     1049 2024-04-20 14:55:34.000000 hun-date-parser-0.2.6/hun_date_parser/utils/__init__.py
--rw-r--r--   0 soma       (501) staff       (20)     3105 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/hun_date_parser/utils/duration_utils.py
--rw-r--r--   0 soma       (501) staff       (20)     5364 2024-04-25 07:49:55.000000 hun-date-parser-0.2.6/hun_date_parser/utils/general_utils.py
-drwxr-xr-x   0 soma       (501) staff       (20)        0 2024-04-25 09:22:34.386196 hun-date-parser-0.2.6/hun_date_parser.egg-info/
--rw-r--r--   0 soma       (501) staff       (20)     8019 2024-04-25 09:22:34.000000 hun-date-parser-0.2.6/hun_date_parser.egg-info/PKG-INFO
--rw-r--r--   0 soma       (501) staff       (20)     1185 2024-04-25 09:22:34.000000 hun-date-parser-0.2.6/hun_date_parser.egg-info/SOURCES.txt
--rw-r--r--   0 soma       (501) staff       (20)        1 2024-04-25 09:22:34.000000 hun-date-parser-0.2.6/hun_date_parser.egg-info/dependency_links.txt
--rw-r--r--   0 soma       (501) staff       (20)       16 2024-04-25 09:22:34.000000 hun-date-parser-0.2.6/hun_date_parser.egg-info/requires.txt
--rw-r--r--   0 soma       (501) staff       (20)       21 2024-04-25 09:22:34.000000 hun-date-parser-0.2.6/hun_date_parser.egg-info/top_level.txt
--rw-r--r--   0 soma       (501) staff       (20)       38 2024-04-25 09:22:34.392358 hun-date-parser-0.2.6/setup.cfg
--rw-r--r--   0 soma       (501) staff       (20)     1185 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/setup.py
-drwxr-xr-x   0 soma       (501) staff       (20)        0 2024-04-25 09:22:34.391831 hun-date-parser-0.2.6/test/
--rw-r--r--   0 soma       (501) staff       (20)        0 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/test/__init__.py
--rw-r--r--   0 soma       (501) staff       (20)    18074 2024-04-25 08:38:56.000000 hun-date-parser-0.2.6/test/test_date_parsers.py
--rw-r--r--   0 soma       (501) staff       (20)     2869 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/test/test_datetime2text.py
--rw-r--r--   0 soma       (501) staff       (20)    16978 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/test/test_datetime_extractor.py
--rw-r--r--   0 soma       (501) staff       (20)     3804 2024-04-25 09:05:51.000000 hun-date-parser-0.2.6/test/test_exposed.py
--rw-r--r--   0 soma       (501) staff       (20)     4168 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/test/test_restricted_parsing.py
--rw-r--r--   0 soma       (501) staff       (20)     1471 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/test/test_structure_parsers.py
--rw-r--r--   0 soma       (501) staff       (20)     4315 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/test/test_time_parsers.py
--rw-r--r--   0 soma       (501) staff       (20)     1181 2024-04-20 12:28:29.000000 hun-date-parser-0.2.6/test/test_utils.py
+drwxr-xr-x   0 soma       (501) staff       (20)        0 2024-05-21 18:48:26.447106 hun-date-parser-0.2.7/
+-rw-r--r--   0 soma       (501) staff       (20)     1035 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/LICENSE
+-rw-r--r--   0 soma       (501) staff       (20)     8019 2024-05-21 18:48:26.446859 hun-date-parser-0.2.7/PKG-INFO
+-rw-r--r--   0 soma       (501) staff       (20)     7888 2024-04-25 08:49:49.000000 hun-date-parser-0.2.7/README.md
+drwxr-xr-x   0 soma       (501) staff       (20)        0 2024-05-21 18:48:26.439819 hun-date-parser-0.2.7/hun_date_parser/
+-rw-r--r--   0 soma       (501) staff       (20)      354 2024-05-21 06:10:13.000000 hun-date-parser-0.2.7/hun_date_parser/__init__.py
+drwxr-xr-x   0 soma       (501) staff       (20)        0 2024-05-21 18:48:26.442396 hun-date-parser-0.2.7/hun_date_parser/date_parser/
+-rw-r--r--   0 soma       (501) staff       (20)        0 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/hun_date_parser/date_parser/__init__.py
+-rw-r--r--   0 soma       (501) staff       (20)    20554 2024-05-21 04:53:07.000000 hun-date-parser-0.2.7/hun_date_parser/date_parser/date_parsers.py
+-rw-r--r--   0 soma       (501) staff       (20)    19217 2024-05-21 18:21:51.000000 hun-date-parser-0.2.7/hun_date_parser/date_parser/datetime_extractor.py
+drwxr-xr-x   0 soma       (501) staff       (20)        0 2024-05-21 18:48:26.442873 hun-date-parser-0.2.7/hun_date_parser/date_parser/interval_restriction/
+-rw-r--r--   0 soma       (501) staff       (20)      223 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/hun_date_parser/date_parser/interval_restriction/__init__.py
+-rw-r--r--   0 soma       (501) staff       (20)     5805 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/hun_date_parser/date_parser/interval_restriction/restricted_parsing.py
+-rw-r--r--   0 soma       (501) staff       (20)     5371 2024-04-25 08:31:35.000000 hun-date-parser-0.2.7/hun_date_parser/date_parser/patterns.py
+-rw-r--r--   0 soma       (501) staff       (20)     2643 2024-04-25 06:59:36.000000 hun-date-parser-0.2.7/hun_date_parser/date_parser/structure_parsers.py
+-rw-r--r--   0 soma       (501) staff       (20)     8862 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/hun_date_parser/date_parser/time_parsers.py
+drwxr-xr-x   0 soma       (501) staff       (20)        0 2024-05-21 18:48:26.443593 hun-date-parser-0.2.7/hun_date_parser/date_textualizer/
+-rw-r--r--   0 soma       (501) staff       (20)        0 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/hun_date_parser/date_textualizer/__init__.py
+-rw-r--r--   0 soma       (501) staff       (20)     1439 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/hun_date_parser/date_textualizer/date2text.py
+-rw-r--r--   0 soma       (501) staff       (20)     2161 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/hun_date_parser/date_textualizer/datetime_textualizer.py
+-rw-r--r--   0 soma       (501) staff       (20)     4182 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/hun_date_parser/date_textualizer/time2text.py
+drwxr-xr-x   0 soma       (501) staff       (20)        0 2024-05-21 18:48:26.444457 hun-date-parser-0.2.7/hun_date_parser/utils/
+-rw-r--r--   0 soma       (501) staff       (20)     1049 2024-04-20 14:55:34.000000 hun-date-parser-0.2.7/hun_date_parser/utils/__init__.py
+-rw-r--r--   0 soma       (501) staff       (20)     3105 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/hun_date_parser/utils/duration_utils.py
+-rw-r--r--   0 soma       (501) staff       (20)     5364 2024-04-25 07:49:55.000000 hun-date-parser-0.2.7/hun_date_parser/utils/general_utils.py
+drwxr-xr-x   0 soma       (501) staff       (20)        0 2024-05-21 18:48:26.440442 hun-date-parser-0.2.7/hun_date_parser.egg-info/
+-rw-r--r--   0 soma       (501) staff       (20)     8019 2024-05-21 18:48:26.000000 hun-date-parser-0.2.7/hun_date_parser.egg-info/PKG-INFO
+-rw-r--r--   0 soma       (501) staff       (20)     1185 2024-05-21 18:48:26.000000 hun-date-parser-0.2.7/hun_date_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 soma       (501) staff       (20)        1 2024-05-21 18:48:26.000000 hun-date-parser-0.2.7/hun_date_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 soma       (501) staff       (20)       16 2024-05-21 18:48:26.000000 hun-date-parser-0.2.7/hun_date_parser.egg-info/requires.txt
+-rw-r--r--   0 soma       (501) staff       (20)       21 2024-05-21 18:48:26.000000 hun-date-parser-0.2.7/hun_date_parser.egg-info/top_level.txt
+-rw-r--r--   0 soma       (501) staff       (20)       38 2024-05-21 18:48:26.447147 hun-date-parser-0.2.7/setup.cfg
+-rw-r--r--   0 soma       (501) staff       (20)     1185 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/setup.py
+drwxr-xr-x   0 soma       (501) staff       (20)        0 2024-05-21 18:48:26.446624 hun-date-parser-0.2.7/test/
+-rw-r--r--   0 soma       (501) staff       (20)        0 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/test/__init__.py
+-rw-r--r--   0 soma       (501) staff       (20)    18181 2024-05-21 04:52:27.000000 hun-date-parser-0.2.7/test/test_date_parsers.py
+-rw-r--r--   0 soma       (501) staff       (20)     2869 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/test/test_datetime2text.py
+-rw-r--r--   0 soma       (501) staff       (20)    16978 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/test/test_datetime_extractor.py
+-rw-r--r--   0 soma       (501) staff       (20)     3804 2024-04-25 09:05:51.000000 hun-date-parser-0.2.7/test/test_exposed.py
+-rw-r--r--   0 soma       (501) staff       (20)     4168 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/test/test_restricted_parsing.py
+-rw-r--r--   0 soma       (501) staff       (20)     1471 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/test/test_structure_parsers.py
+-rw-r--r--   0 soma       (501) staff       (20)     4315 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/test/test_time_parsers.py
+-rw-r--r--   0 soma       (501) staff       (20)     1181 2024-04-20 12:28:29.000000 hun-date-parser-0.2.7/test/test_utils.py
```

### Comparing `hun-date-parser-0.2.6/LICENSE` & `hun-date-parser-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/PKG-INFO` & `hun-date-parser-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hun-date-parser
-Version: 0.2.6
+Version: 0.2.7
 Summary: A tool for extracting datetime intervals from Hungarian sentences and turning datetime objects into Hungarian text.
 Home-page: https://github.com/szegedai/hun-date-parser
 Author: Soma Nagy
 Author-email: nagysomabalint@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hun-date-parser Version: 0.2.6 Summary: A tool for
+Metadata-Version: 2.1 Name: hun-date-parser Version: 0.2.7 Summary: A tool for
 extracting datetime intervals from Hungarian sentences and turning datetime
 objects into Hungarian text. Home-page: https://github.com/szegedai/hun-date-
 parser Author: Soma Nagy Author-email: nagysomabalint@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 python-dateutil
```

### Comparing `hun-date-parser-0.2.6/README.md` & `hun-date-parser-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/hun_date_parser/date_parser/date_parsers.py` & `hun-date-parser-0.2.7/hun_date_parser/date_parser/date_parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,17 @@
                         'date_parts': [Year(group[2], 'match_iso_date'),
                                        Month(group[1], 'match_iso_date'),
                                        Day(group[0], 'match_iso_date')]})
     elif match:
         for group in match:
             group = [int(m.lstrip('0')) for m in group if m.lstrip('0')]
 
+            if not group:
+                continue
+
             if realistic_year_restriction and not is_year_realistic(group[0]):
                 continue
 
             if len(group) == 1:
                 res.append({'match': group, 'date_parts': [Year(group[0], 'match_iso_date')]})
             elif len(group) == 2:
                 res.append({'match': group,
```

### Comparing `hun-date-parser-0.2.6/hun_date_parser/date_parser/datetime_extractor.py` & `hun-date-parser-0.2.7/hun_date_parser/date_parser/datetime_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,16 @@
     :param input_sentence: Input sentence string.
     :param now: Current timestamp to calculate relative dates.
     :param search_scope: Defines whether the timeframe should be restricted to past or future.
     :param realistic_year_required: Defines whether to restrict year candidates to be between 1900 and 2100.
     :return: list of date interval dictionaries
     """
     datetime_extractor = DatetimeExtractor(now=now, output_container='date',
-                                           search_scope=search_scope, realistic_year_required=realistic_year_required)
+                                           search_scope=search_scope,
+                                           realistic_year_required=realistic_year_required)
     return datetime_extractor.parse_datetime(sentence=input_sentence)
 
 
 def text2time(input_sentence: str, now: datetime = datetime.now(),
               search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED,
               realistic_year_required: bool = True) -> List[Dict[str, datelike]]:
     """
@@ -73,15 +74,16 @@
     :param input_sentence: Input sentence string.
     :param now: Current timestamp to calculate relative dates.
     :param search_scope: Defines whether the timeframe should be restricted to past or future.
     :param realistic_year_required: Defines whether to restrict year candidates to be between 1900 and 2100.
     :return: list of time interval dictionaries
     """
     datetime_extractor = DatetimeExtractor(now=now, output_container='time',
-                                           search_scope=search_scope, realistic_year_required=realistic_year_required)
+                                           search_scope=search_scope,
+                                           realistic_year_required=realistic_year_required)
     return datetime_extractor.parse_datetime(sentence=input_sentence)
 
 
 def match_rules(now: datetime, sentence: str,
                 search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED,
                 realistic_year_required: bool = True) -> List:
     """
@@ -342,14 +344,23 @@
             else:
                 return None
         else:
             return None
 
     def parse_datetime(self, sentence: str) -> List[Dict[str, datelike]]:
         """
+        Fail-safe wrapper around _parse_datetime. All possible exceptions will be caught and an empty list is returned.
+        """
+        try:
+            return self._parse_datetime(sentence)
+        except:
+            return []
+
+    def _parse_datetime(self, sentence: str) -> List[Dict[str, datelike]]:
+        """
         Extracts list of datetime intervals from input sentence.
         :param sentence: Input sentence string.
         :return: list of datetime interval dictionaries
         """
         sentence = sentence.lower()
         sentence_parts = match_multi_match(sentence)
         parsed_dates = []
```

### Comparing `hun-date-parser-0.2.6/hun_date_parser/date_parser/interval_restriction/restricted_parsing.py` & `hun-date-parser-0.2.7/hun_date_parser/date_parser/interval_restriction/restricted_parsing.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/hun_date_parser/date_parser/patterns.py` & `hun-date-parser-0.2.7/hun_date_parser/date_parser/patterns.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/hun_date_parser/date_parser/structure_parsers.py` & `hun-date-parser-0.2.7/hun_date_parser/date_parser/structure_parsers.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/hun_date_parser/date_parser/time_parsers.py` & `hun-date-parser-0.2.7/hun_date_parser/date_parser/time_parsers.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/hun_date_parser/date_textualizer/date2text.py` & `hun-date-parser-0.2.7/hun_date_parser/date_textualizer/date2text.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/hun_date_parser/date_textualizer/datetime_textualizer.py` & `hun-date-parser-0.2.7/hun_date_parser/date_textualizer/datetime_textualizer.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/hun_date_parser/date_textualizer/time2text.py` & `hun-date-parser-0.2.7/hun_date_parser/date_textualizer/time2text.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/hun_date_parser/utils/__init__.py` & `hun-date-parser-0.2.7/hun_date_parser/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/hun_date_parser/utils/duration_utils.py` & `hun-date-parser-0.2.7/hun_date_parser/utils/duration_utils.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/hun_date_parser/utils/general_utils.py` & `hun-date-parser-0.2.7/hun_date_parser/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/hun_date_parser.egg-info/PKG-INFO` & `hun-date-parser-0.2.7/hun_date_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hun-date-parser
-Version: 0.2.6
+Version: 0.2.7
 Summary: A tool for extracting datetime intervals from Hungarian sentences and turning datetime objects into Hungarian text.
 Home-page: https://github.com/szegedai/hun-date-parser
 Author: Soma Nagy
 Author-email: nagysomabalint@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hun-date-parser Version: 0.2.6 Summary: A tool for
+Metadata-Version: 2.1 Name: hun-date-parser Version: 0.2.7 Summary: A tool for
 extracting datetime intervals from Hungarian sentences and turning datetime
 objects into Hungarian text. Home-page: https://github.com/szegedai/hun-date-
 parser Author: Soma Nagy Author-email: nagysomabalint@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 python-dateutil
```

### Comparing `hun-date-parser-0.2.6/hun_date_parser.egg-info/SOURCES.txt` & `hun-date-parser-0.2.7/hun_date_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/setup.py` & `hun-date-parser-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/test/test_date_parsers.py` & `hun-date-parser-0.2.7/test/test_date_parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,16 @@
     ('1923 július', [[Year(1923, 'match_iso_date')]], SearchScopes.NOT_RESTRICTED, None),
     ('1923 július', [[Year(1923, 'match_iso_date')]], SearchScopes.NOT_RESTRICTED, True),
     ('1889 július', [], SearchScopes.NOT_RESTRICTED, True),
     ('1901 július', [[Year(1901, 'match_iso_date')]], SearchScopes.NOT_RESTRICTED, True),
     ('8000 forint', [], SearchScopes.NOT_RESTRICTED, True),
     ('8000', [[Year(8000, 'match_iso_date')]], SearchScopes.PAST_SEARCH, False),
     ('8000 forint', [], SearchScopes.PAST_SEARCH, False),
+    ('0000', [], SearchScopes.NOT_RESTRICTED, False),
+    ('0000', [], SearchScopes.NOT_RESTRICTED, True),
 ]
 
 tf_weekday = [
     ('múlt vasárnap', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(6, 'weekday')]], SearchScopes.NOT_RESTRICTED),
     ('ezen a heten hetfon', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(7, 'weekday')]], SearchScopes.NOT_RESTRICTED),
     ('jövő kedden', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(15, 'weekday')]], SearchScopes.NOT_RESTRICTED),
     ('előző szombaton ', [[Year(2020, 'weekday'), Month(12, 'weekday'), Day(5, 'weekday')]], SearchScopes.NOT_RESTRICTED),
```

### Comparing `hun-date-parser-0.2.6/test/test_datetime2text.py` & `hun-date-parser-0.2.7/test/test_datetime2text.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/test/test_datetime_extractor.py` & `hun-date-parser-0.2.7/test/test_datetime_extractor.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/test/test_exposed.py` & `hun-date-parser-0.2.7/test/test_exposed.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/test/test_restricted_parsing.py` & `hun-date-parser-0.2.7/test/test_restricted_parsing.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/test/test_structure_parsers.py` & `hun-date-parser-0.2.7/test/test_structure_parsers.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/test/test_time_parsers.py` & `hun-date-parser-0.2.7/test/test_time_parsers.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.2.6/test/test_utils.py` & `hun-date-parser-0.2.7/test/test_utils.py`

 * *Files identical despite different names*

