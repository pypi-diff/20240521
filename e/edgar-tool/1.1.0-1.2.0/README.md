# Comparing `tmp/edgar_tool-1.1.0.tar.gz` & `tmp/edgar_tool-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgar_tool-1.1.0.tar", max compression
+gzip compressed data, was "edgar_tool-1.2.0.tar", max compression
```

## Comparing `edgar_tool-1.1.0.tar` & `edgar_tool-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2024-03-26 19:21:50.347158 edgar_tool-1.1.0/LICENSE
--rw-r--r--   0        0        0     9304 2024-03-26 19:21:50.347158 edgar_tool-1.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-26 19:21:50.347158 edgar_tool-1.1.0/edgar_tool/__init__.py
--rw-r--r--   0        0        0     6262 2024-03-26 19:21:50.351158 edgar_tool-1.1.0/edgar_tool/cli.py
--rw-r--r--   0        0        0    62521 2024-03-26 19:21:50.351158 edgar_tool-1.1.0/edgar_tool/constants.py
--rw-r--r--   0        0        0     3322 2024-03-26 19:21:50.351158 edgar_tool-1.1.0/edgar_tool/io.py
--rw-r--r--   0        0        0      168 2024-03-26 19:21:50.351158 edgar_tool-1.1.0/edgar_tool/main.py
--rw-r--r--   0        0        0     2212 2024-03-26 19:21:50.351158 edgar_tool-1.1.0/edgar_tool/page_fetcher.py
--rw-r--r--   0        0        0     9271 2024-03-26 19:21:50.351158 edgar_tool-1.1.0/edgar_tool/rss.py
--rw-r--r--   0        0        0    19806 2024-03-26 19:21:50.351158 edgar_tool-1.1.0/edgar_tool/text_search.py
--rw-r--r--   0        0        0     1099 2024-03-26 19:21:50.351158 edgar_tool-1.1.0/edgar_tool/utils.py
--rw-r--r--   0        0        0     1092 2024-03-26 19:21:50.351158 edgar_tool-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    10581 1970-01-01 00:00:00.000000 edgar_tool-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-21 16:41:20.221519 edgar_tool-1.2.0/LICENSE
+-rw-r--r--   0        0        0     9477 2024-05-21 16:41:20.221519 edgar_tool-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 16:41:20.221519 edgar_tool-1.2.0/edgar_tool/__init__.py
+-rw-r--r--   0        0        0     7015 2024-05-21 16:41:20.221519 edgar_tool-1.2.0/edgar_tool/cli.py
+-rw-r--r--   0        0        0    63254 2024-05-21 16:41:20.221519 edgar_tool-1.2.0/edgar_tool/constants.py
+-rw-r--r--   0        0        0     3322 2024-05-21 16:41:20.221519 edgar_tool-1.2.0/edgar_tool/io.py
+-rw-r--r--   0        0        0      168 2024-05-21 16:41:20.221519 edgar_tool-1.2.0/edgar_tool/main.py
+-rw-r--r--   0        0        0     2212 2024-05-21 16:41:20.221519 edgar_tool-1.2.0/edgar_tool/page_fetcher.py
+-rw-r--r--   0        0        0     9271 2024-05-21 16:41:20.221519 edgar_tool-1.2.0/edgar_tool/rss.py
+-rw-r--r--   0        0        0    20605 2024-05-21 16:41:20.221519 edgar_tool-1.2.0/edgar_tool/text_search.py
+-rw-r--r--   0        0        0     1099 2024-05-21 16:41:20.221519 edgar_tool-1.2.0/edgar_tool/utils.py
+-rw-r--r--   0        0        0     1092 2024-05-21 16:41:20.221519 edgar_tool-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10754 1970-01-01 00:00:00.000000 edgar_tool-1.2.0/PKG-INFO
```

### Comparing `edgar_tool-1.1.0/LICENSE` & `edgar_tool-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgar_tool-1.1.0/README.md` & `edgar_tool-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 
 # Basic usage with a combination of exact and partial search parameters
 edgar-tool text_search \"John Doe\" Pharmaceuticals Chemicals
 
 # Usage with date range and export to custom CSV file
 edgar-tool text_search Tsunami Hazards --start_date "2021-01-01" --end_date "2021-12-31" --output "results.csv"
 
+# Usage with a partial set of filing forms + single forms 
+edgar-tool text_search Hurricane Damage --filing_form "registration_statements" --single_forms "['1-K', '1-SA']"
+
 # More advanced usage specifying more arguments, with export to JSON
 edgar-tool text_search Volcano Monitoring --start_date "2021-01-01" --end_date "2021-12-31" --output "results.json"\
           --filing_type "all_annual_quarterly_and_current_reports" --entity_id "0001030717" \
           --min_wait 5.0 --max_wait 7.0 --retries 3
           
 # Using aliases where supported and exporting to JSONLines
 edgar-tool text_search Calabarzon -s "2021-01-01" -o "results.jsonl" -f "all_annual_quarterly_and_current_reports" -r 3 -h
```

### Comparing `edgar_tool-1.1.0/edgar_tool/cli.py` & `edgar_tool-1.2.0/edgar_tool/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import sys
 import time
 from datetime import date, timedelta, datetime
 from typing import List, Optional
 from warnings import warn
 from edgar_tool.constants import (
     SUPPORTED_OUTPUT_EXTENSIONS,
-    TEXT_SEARCH_FILING_CATEGORIES_MAPPING,
+    TEXT_SEARCH_CATEGORY_FORM_GROUPINGS,
+    TEXT_SEARCH_FILING_VS_MAPPING_CATEGORIES_MAPPING,
 )
 from edgar_tool.rss import fetch_rss_feed
 from edgar_tool.text_search import EdgarTextSearcher
 from edgar_tool.page_fetcher import NoResultsFoundError
 
 
 def _validate_text_search_args(
     search_keywords: List[str],
     start_date: date,
     end_date: date,
-    filing_type: Optional[str],
+    filing_form: Optional[str],
+    single_forms: Optional[List[str]],
     min_wait_secs: float,
     max_wait_secs: float,
     retries: int,
     browser_name: Optional[str],
     headless: Optional[bool],
     destination: str,
 ) -> None:
@@ -42,33 +44,42 @@
         warn("browser argument is deprecated and is ignored")
     if headless is not None:
         warn("headless argument is deprecated and is ignored")
     if not any(
         destination.lower().endswith(ext) for ext in SUPPORTED_OUTPUT_EXTENSIONS
     ):
         raise ValueError(
-            f"Destination file must have one of the following extensions: {', '.join(SUPPORTED_OUTPUT_EXTENSIONS)}"
+            f"Destination file must have one of the following extensions: {'; '.join(SUPPORTED_OUTPUT_EXTENSIONS)}"
         )
     if (
-        filing_type
-        and filing_type.lower() not in TEXT_SEARCH_FILING_CATEGORIES_MAPPING.keys()
+        filing_form
+        and filing_form not in TEXT_SEARCH_FILING_VS_MAPPING_CATEGORIES_MAPPING.keys()
     ):
         raise ValueError(
-            f"Filing type must be one of: {', '.join(TEXT_SEARCH_FILING_CATEGORIES_MAPPING.keys())}"
-        )
+            f"Filing form group must be one of: {'; '.join(TEXT_SEARCH_FILING_VS_MAPPING_CATEGORIES_MAPPING.keys())}"
+    )
+    if single_forms:
+        single_list = [item for sublist in TEXT_SEARCH_CATEGORY_FORM_GROUPINGS.values() for item in
+                       sublist]
+        invalid_forms = [form for form in single_forms if form not in single_list]
+        if invalid_forms:
+            raise ValueError(
+                f"Single forms must be one or more of: {single_list}"
+            )
 
 
 class SecEdgarScraperCli:
 
     @staticmethod
     def text_search(
         *keywords: str,
         output: str = f"edgar_search_results_{datetime.now().strftime('%Y%m%d_%H%M%S')}.csv",
         entity_id: Optional[str] = None,
-        filing_type: Optional[str] = None,
+        filing_form: Optional[str] = None,
+        single_forms: Optional[List[str]] = None,
         start_date: str = (date.today() - timedelta(days=365 * 5)).strftime("%Y-%m-%d"),
         end_date: str = date.today().strftime("%Y-%m-%d"),
         # todo: deprecate min_wait and max_wait
         min_wait: float = 0.1,
         max_wait: float = 0.15,
         retries: int = 3,
         browser: Optional[str] = None,
@@ -77,15 +88,16 @@
         """
         Perform a custom text search on the SEC EDGAR website and save the results to either a CSV, JSON,
         or JSONLines file.
 
         :param keywords: List of keywords to search for
         :param output: Name of the output file to save the results to
         :param entity_id: CIK or name or ticker of the company to search for
-        :param filing_type: Type of filing to search for
+        :param filing_form: Form group to search for
+        :param single_forms: List of single forms to search for (e.g. ['10-K', '10-Q'])
         :param start_date: Start date of the search
         :param end_date: End date of the search
         :param min_wait: Minimum wait time for the request to complete before checking the page or retrying a request
         :param max_wait: Maximum wait time for the request to complete before checking the page or retrying a request
         :param retries: How many times to retry requests before failing
         :param browser: Deprecated and not used
         :param headless: Deprecated and not used
@@ -99,28 +111,30 @@
             retries = int(retries)
         except Exception as e:
             raise ValueError(f"Invalid argument type or format: {e}")
         _validate_text_search_args(
             search_keywords=keywords,
             start_date=start_date,
             end_date=end_date,
-            filing_type=filing_type,
+            filing_form=filing_form,
+            single_forms=single_forms,
             min_wait_secs=min_wait,
             max_wait_secs=max_wait,
             retries=retries,
             browser_name=browser,
             headless=headless,
             destination=output,
         )
         scraper = EdgarTextSearcher()
         try:
             scraper.text_search(
                 keywords=keywords,
                 entity_id=entity_id,
-                filing_type=filing_type,
+                filing_form=TEXT_SEARCH_FILING_VS_MAPPING_CATEGORIES_MAPPING.get(filing_form),
+                single_forms=single_forms,
                 start_date=start_date,
                 end_date=end_date,
                 min_wait_seconds=min_wait,
                 max_wait_seconds=max_wait,
                 retries=retries,
                 destination=output,
             )
```

### Comparing `edgar_tool-1.1.0/edgar_tool/constants.py` & `edgar_tool-1.2.0/edgar_tool/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     "sec_orders_and_notices": "form-cat7",
     "proxy_materials": "form-cat8",
     "tender_offers_and_going_private_tx": "form-cat9",
     "trust_indentures": "form-cat10",
 }
 TEXT_SEARCH_SPLIT_BATCHES_NUMBER = 2
 TEXT_SEARCH_CSV_FIELDS_NAMES = [
-    "filing_type",
     "root_form",
     "form_name",
     "filed_at",
     "reporting_for",
     "entity_name",
     "ticker",
     "company_cik",
@@ -1386,15 +1385,14 @@
     },
     "N-VPFS": {
         "description": "",
         "title": "Financial statements for certain variable contracts",
     },
 }
 
-# These groupings are not yet used, but are included for completeness
 TEXT_SEARCH_CATEGORY_FORM_GROUPINGS = {
     #    "Exclude insider equity awards, transactions, and ownership (Section 16 Reports)": ["-3","-4","-5"], # todo: work out how to exclude these
     "All annual, quarterly, and current reports": [
         "1-K",
         "1-SA",
         "1-U",
         "1-Z",
@@ -1604,7 +1602,21 @@
         "SC TO-T",
         "SC13E4F",
         "SC14D9C",
         "SC14D9F",
     ],
     "Trust indenture filings": ["305B2", "T-3"],
 }
+
+# These are the verbose descriptions of the categories that are used in the CLI,
+TEXT_SEARCH_FILING_VS_MAPPING_CATEGORIES_MAPPING = {
+    "all_annual_quarterly_and_current_reports": "All annual, quarterly, and current reports",
+    "all_section_16": "Insider equity awards, transactions, and ownership (Section 16 Reports)",
+    "beneficial_ownership_reports": "Beneficial ownership reports",
+    "exempt_offerings": "Exempt offerings",
+    "registration_statements": "Registration statements and prospectuses",
+    "filing_review_correspondence": "Filing review correspondence",
+    "sec_orders_and_notices": "SEC orders and notices",
+    "proxy_materials": "Proxy materials",
+    "tender_offers_and_going_private_tx": "Tender offers and going private transactions",
+    "trust_indentures": "Trust indenture filings",
+}
```

### Comparing `edgar_tool-1.1.0/edgar_tool/io.py` & `edgar_tool-1.2.0/edgar_tool/io.py`

 * *Files identical despite different names*

### Comparing `edgar_tool-1.1.0/edgar_tool/page_fetcher.py` & `edgar_tool-1.2.0/edgar_tool/page_fetcher.py`

 * *Files identical despite different names*

### Comparing `edgar_tool-1.1.0/edgar_tool/rss.py` & `edgar_tool-1.2.0/edgar_tool/rss.py`

 * *Files identical despite different names*

### Comparing `edgar_tool-1.1.0/edgar_tool/text_search.py` & `edgar_tool-1.2.0/edgar_tool/text_search.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     fetch_page,
     PageCheckFailedError,
     ResultsTableNotFoundError,
     NoResultsFoundError
 )
 from edgar_tool.constants import (
     TEXT_SEARCH_BASE_URL,
-    TEXT_SEARCH_FILING_CATEGORIES_MAPPING,
+    TEXT_SEARCH_CATEGORY_FORM_GROUPINGS,
     TEXT_SEARCH_SPLIT_BATCHES_NUMBER,
     TEXT_SEARCH_CSV_FIELDS_NAMES,
     TEXT_SEARCH_FORM_MAPPING,
     TEXT_SEARCH_LOCATIONS_MAPPING,
 )
 from edgar_tool.io import write_results_to_file
 from edgar_tool.utils import split_date_range_in_n, unpack_singleton_list
@@ -74,17 +74,14 @@
         # Fetching film numbers
         film_nums = _source.get("film_num")
 
         # Fetching and cleaning CIKs
         ciks = _source.get("ciks")
         ciks_trimmed: List[str] = [c.strip("0") for c in ciks]
 
-        # Fetching filing type
-        filing_type = _source.get("file_type")
-
         # Get form and human readable name
         root_form = _source.get("root_form")
         form_name = TEXT_SEARCH_FORM_MAPPING.get(root_form, {}).get("title", "")
 
         # Build adsh for url
         data_adsh = _source.get("adsh", "")
         data_adsh_no_dash = data_adsh.replace("-", "")
@@ -137,15 +134,14 @@
         incorporated_locations = _source.get("inc_states")
         incorporated_locations = [
             TEXT_SEARCH_LOCATIONS_MAPPING.get(inc_loc)
             for inc_loc in incorporated_locations
         ]
 
         parsed = {
-            "filing_type": filing_type,
             "root_form": root_form,
             "form_name": form_name,
             "filed_at": filed_at,
             "reporting_for": end_date,
             "entity_name": unpack_singleton_list(entity_names),
             "ticker": unpack_singleton_list(tickers),
             "company_cik": unpack_singleton_list(ciks),
@@ -183,25 +179,27 @@
                 continue
         return parsed_rows
 
     @staticmethod
     def _generate_request_args(
         keywords: List[str],
         entity_id: Optional[str],
-        filing_type: Optional[str],
+        filing_form: Optional[str],
+        single_forms: Optional[List[str]],
         start_date: date,
         end_date: date,
         page_number: int,
     ) -> str:
         """
         Generates the request arguments for the SEC website based on the given parameters.
 
         :param keywords: Search keywords to input in the "Document word or phrase" field
         :param entity_id: Entity/Person name, ticker, or CIK number to input in the "Company name, ticker, or CIK" field
-        :param filing_type: Filing category to select from the dropdown menu, defaults to None
+        :param filing_form: Group to select within the filing category dropdown menu, defaults to None
+        :param single_forms: List of single forms to search for (e.g. ['10-K', '10-Q']), defaults to None
         :param start_date: Start date for the custom date range, defaults to 5 years ago to replicate the default behavior of the SEC website
         :param end_date: End date for the custom date range, defaults to current date in order to replicate the default behavior of the SEC website
         :param page_number: Page number to request, defaults to 1
 
         :return: URL-encoded request arguments string to concatenate to the SEC website URL
         """
 
@@ -220,19 +218,24 @@
             "enddt": end_date.strftime("%Y-%m-%d"),
             "page": page_number,
         }
 
         # Add optional parameters
         if entity_id:
             request_args["entityName"] = entity_id
-        if filing_type:
-            request_args["category"] = TEXT_SEARCH_FILING_CATEGORIES_MAPPING[
-                filing_type
-            ]
 
+        # Handle forms and single forms
+        part_filing_form = [] if filing_form is None else TEXT_SEARCH_CATEGORY_FORM_GROUPINGS[filing_form]
+        part_single_forms = [] if single_forms is None else single_forms
+
+        # Join the filing_forms and single forms and remove duplicates
+        forms = ",".join(list(set(part_filing_form + part_single_forms)))
+        if forms != "":
+            request_args["forms"] = forms
+ 
         # URL-encode the request arguments
         request_args = urllib.parse.urlencode(request_args)
 
         return request_args
 
     def _fetch_search_request_results(
         self,
@@ -296,40 +299,43 @@
                 )
                 continue
 
     def _generate_search_requests(
         self,
         keywords: List[str],
         entity_id: Optional[str],
-        filing_type: Optional[str],
+        filing_form: Optional[str],
+        single_forms: Optional[List[str]],
         start_date: date,
         end_date: date,
         min_wait_seconds: float,
         max_wait_seconds: float,
         retries: int,
     ) -> None:
         """
         Generates search requests for the given parameters and date range,
         recursively splitting the date range in two if the number of results is 10000 or more.
 
         :param keywords: Search keywords to input in the "Document word or phrase" field
         :param entity_id: Entity/Person name, ticker, or CIK number to input in the "Company name, ticker, or CIK" field
-        :param filing_type: Filing category to select from the dropdown menu
+        :param filing_form: Group to select within the filing category dropdown menu, defaults to None
+        :param single_forms: List of single forms to search for (e.g. ['10-K', '10-Q']), defaults to None
         :param start_date: Start date for the custom date range
         :param end_date: End date for the custom date range
         :param min_wait_seconds: Minimum number of seconds to wait for the request to complete
         :param max_wait_seconds: Maximum number of seconds to wait for the request to complete
         :param retries: Number of times to retry the request before failing
         """
 
         # Fetch first page, verify that the request was successful by checking the result count value on the page
         request_args = self._generate_request_args(
             keywords=keywords,
             entity_id=entity_id,
-            filing_type=filing_type,
+            filing_form=filing_form,
+            single_forms=single_forms,
             start_date=start_date,
             end_date=end_date,
             page_number=1,
         )
         url = f"{TEXT_SEARCH_BASE_URL}{request_args}"
 
         # Try to fetch the first page and parse the number of results
@@ -345,15 +351,15 @@
                 f"while parsing result number for seemingly non-empty results: {ve}"
             )
             num_results = 10000
 
         # If we have 10000 results, split date range in two separate requests and fetch first page again, do so until
         # we have a set of date ranges for which none of the requests have 10000 results
         if num_results == 0:
-            print(f"No results found for query in date range {start_date} -> {end_date}.")      
+            print(f"No results found for query in date range {start_date} -> {end_date}.")
         elif num_results < 10000:
             print(
                 f"Less than 10000 ({num_results}) results found for range {start_date} -> {end_date}, "
                 f"returning search request string..."
             )
             self.search_requests.append(request_args)
         else:
@@ -370,54 +376,58 @@
                     end = dates[i + 1]
                     print(
                         f"Trying to generate search requests for date range {start} -> {end} ..."
                     )
                     self._generate_search_requests(
                         keywords=keywords,
                         entity_id=entity_id,
-                        filing_type=filing_type,
+                        filing_form=filing_form,
+                        single_forms=single_forms,
                         start_date=start,
                         end_date=end,
                         min_wait_seconds=min_wait_seconds,
                         max_wait_seconds=max_wait_seconds,
                         retries=retries,
                     )
                 except IndexError:
                     pass
 
     def text_search(
         self,
         keywords: List[str],
         entity_id: Optional[str],
-        filing_type: Optional[str],
+        filing_form: Optional[str],
+        single_forms: Optional[List[str]],
         start_date: date,
         end_date: date,
         min_wait_seconds: float,
         max_wait_seconds: float,
         retries: int,
         destination: str,
     ) -> None:
         """
         Searches the SEC website for filings based on the given parameters.
 
         :param keywords: Search keywords to input in the "Document word or phrase" field
         :param entity_id: Entity/Person name, ticker, or CIK number to input in the "Company name, ticker, or CIK" field
-        :param filing_type: Filing category to select from the dropdown menu
+        :param filing_form: Group to select within the filing category dropdown menu, defaults to None
+        :param single_forms: List of single forms to search for (e.g. ['10-K', '10-Q']), defaults to None
         :param start_date: Start date for the custom date range
         :param end_date: End date for the custom date range
         :param min_wait_seconds: Minimum number of seconds to wait for the request to complete
         :param max_wait_seconds: Maximum number of seconds to wait for the request to complete
         :param retries: Number of times to retry the request before failing
         :param destination: Name of the CSV file to write the results to
         """
 
         self._generate_search_requests(
             keywords=keywords,
             entity_id=entity_id,
-            filing_type=filing_type,
+            filing_form=filing_form,
+            single_forms=single_forms,
             start_date=start_date,
             end_date=end_date,
             min_wait_seconds=min_wait_seconds,
             max_wait_seconds=max_wait_seconds,
             retries=retries,
         )
```

### Comparing `edgar_tool-1.1.0/edgar_tool/utils.py` & `edgar_tool-1.2.0/edgar_tool/utils.py`

 * *Files identical despite different names*

### Comparing `edgar_tool-1.1.0/pyproject.toml` & `edgar_tool-1.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgar-tool"
-version = "1.1.0"
+version = "1.2.0"
 description = "Search and retrieve corporate and financial data from the United States Securities and Exchange Commission (SEC)."
 authors = ["Bellingcat"]
 license = "GNU General Public License v3 (GPLv3)"
 readme = "README.md"
 repository = "https://github.com/bellingcat/EDGAR"
 classifiers = [
   "Intended Audience :: Developers",
```

### Comparing `edgar_tool-1.1.0/PKG-INFO` & `edgar_tool-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgar-tool
-Version: 1.1.0
+Version: 1.2.0
 Summary: Search and retrieve corporate and financial data from the United States Securities and Exchange Commission (SEC).
 Home-page: https://github.com/bellingcat/EDGAR
 License: GNU General Public License v3 (GPLv3)
 Keywords: scraper,edgar,finance,sec
 Author: Bellingcat
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -71,14 +71,17 @@
 
 # Basic usage with a combination of exact and partial search parameters
 edgar-tool text_search \"John Doe\" Pharmaceuticals Chemicals
 
 # Usage with date range and export to custom CSV file
 edgar-tool text_search Tsunami Hazards --start_date "2021-01-01" --end_date "2021-12-31" --output "results.csv"
 
+# Usage with a partial set of filing forms + single forms 
+edgar-tool text_search Hurricane Damage --filing_form "registration_statements" --single_forms "['1-K', '1-SA']"
+
 # More advanced usage specifying more arguments, with export to JSON
 edgar-tool text_search Volcano Monitoring --start_date "2021-01-01" --end_date "2021-12-31" --output "results.json"\
           --filing_type "all_annual_quarterly_and_current_reports" --entity_id "0001030717" \
           --min_wait 5.0 --max_wait 7.0 --retries 3
           
 # Using aliases where supported and exporting to JSONLines
 edgar-tool text_search Calabarzon -s "2021-01-01" -o "results.jsonl" -f "all_annual_quarterly_and_current_reports" -r 3 -h
```

