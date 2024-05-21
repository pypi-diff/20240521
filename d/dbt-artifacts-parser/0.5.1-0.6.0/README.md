# Comparing `tmp/dbt_artifacts_parser-0.5.1.tar.gz` & `tmp/dbt_artifacts_parser-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_artifacts_parser-0.5.1.tar", last modified: Thu Jan  4 01:13:31 2024, max compression
+gzip compressed data, was "dbt_artifacts_parser-0.6.0.tar", last modified: Tue May 21 09:33:13 2024, max compression
```

## Comparing `dbt_artifacts_parser-0.5.1.tar` & `dbt_artifacts_parser-0.6.0.tar`

### file list

```diff
@@ -1,56 +1,60 @@
--rw-r--r--   0        0        0    11357 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/LICENSE
--rw-r--r--   0        0        0    10251 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/README.md
--rw-r--r--   0        0        0      859 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/__init__.py
--rw-r--r--   0        0        0    13216 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parser.py
--rw-r--r--   0        0        0      796 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/__init__.py
--rw-r--r--   0        0        0      977 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/base.py
--rw-r--r--   0        0        0      796 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/catalog/__init__.py
--rw-r--r--   0        0        0     1887 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/catalog/catalog_v1.py
--rw-r--r--   0        0        0      796 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/__init__.py
--rw-r--r--   0        0        0    39709 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v1.py
--rw-r--r--   0        0        0    47940 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v10.py
--rw-r--r--   0        0        0    44178 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v11.py
--rw-r--r--   0        0        0    40546 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v2.py
--rw-r--r--   0        0        0    41294 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v3.py
--rw-r--r--   0        0        0    46633 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v4.py
--rw-r--r--   0        0        0    47752 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v5.py
--rw-r--r--   0        0        0    48520 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v6.py
--rw-r--r--   0        0        0    52862 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v7.py
--rw-r--r--   0        0        0    35032 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v8.py
--rw-r--r--   0        0        0    39343 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v9.py
--rw-r--r--   0        0        0      796 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/run_results/__init__.py
--rw-r--r--   0        0        0     1719 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/run_results/run_results_v1.py
--rw-r--r--   0        0        0     1755 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/run_results/run_results_v2.py
--rw-r--r--   0        0        0     3346 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/run_results/run_results_v3.py
--rw-r--r--   0        0        0     3458 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/run_results/run_results_v4.py
--rw-r--r--   0        0        0     1839 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/run_results/run_results_v5.py
--rw-r--r--   0        0        0      796 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/sources/__init__.py
--rw-r--r--   0        0        0     2044 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/sources/sources_v1.py
--rw-r--r--   0        0        0     2327 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/sources/sources_v2.py
--rw-r--r--   0        0        0     2441 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/sources/sources_v3.py
--rw-r--r--   0        0        0     2348 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/utils.py
--rw-r--r--   0        0        0     4845 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/version_map.py
--rw-r--r--   0        0        0     5968 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/catalog/catalog_v1.json
--rw-r--r--   0        0        0   129577 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v1.json
--rw-r--r--   0        0        0   148278 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v10.json
--rw-r--r--   0        0        0   130575 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v11.json
--rw-r--r--   0        0        0   135379 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v2.json
--rw-r--r--   0        0        0   138302 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v3.json
--rw-r--r--   0        0        0   157235 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v4.json
--rw-r--r--   0        0        0   159203 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v5.json
--rw-r--r--   0        0        0   163791 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v6.json
--rw-r--r--   0        0        0   174833 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v7.json
--rw-r--r--   0        0        0   115570 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v8.json
--rw-r--r--   0        0        0   129190 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v9.json
--rw-r--r--   0        0        0     4622 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/run-results/run-results_v1.json
--rw-r--r--   0        0        0     4777 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/run-results/run-results_v2.json
--rw-r--r--   0        0        0     9817 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/run-results/run-results_v3.json
--rw-r--r--   0        0        0    10272 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/run-results/run-results_v4.json
--rw-r--r--   0        0        0     4690 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/run-results/run-results_v5.json
--rw-r--r--   0        0        0     5568 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/sources/sources_v1.json
--rw-r--r--   0        0        0     6790 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/sources/sources_v2.json
--rw-r--r--   0        0        0     7249 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/sources/sources_v3.json
--rw-r--r--   0        0        0     1017 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/utils.py
--rw-r--r--   0        0        0     1828 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      830 2024-01-04 01:13:31.000000 dbt_artifacts_parser-0.5.1/setup.py
--rw-r--r--   0        0        0    12111 1970-01-01 00:00:00.000000 dbt_artifacts_parser-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/LICENSE
+-rw-r--r--   0        0        0    10523 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/README.md
+-rw-r--r--   0        0        0      859 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/__init__.py
+-rw-r--r--   0        0        0    14365 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parser.py
+-rw-r--r--   0        0        0      796 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/__init__.py
+-rw-r--r--   0        0        0      977 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/base.py
+-rw-r--r--   0        0        0      796 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/catalog/__init__.py
+-rw-r--r--   0        0        0     1887 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/catalog/catalog_v1.py
+-rw-r--r--   0        0        0      796 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/__init__.py
+-rw-r--r--   0        0        0    39709 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v1.py
+-rw-r--r--   0        0        0    47940 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v10.py
+-rw-r--r--   0        0        0    44179 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v11.py
+-rw-r--r--   0        0        0   162546 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v12.py
+-rw-r--r--   0        0        0    40546 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v2.py
+-rw-r--r--   0        0        0    41294 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v3.py
+-rw-r--r--   0        0        0    46633 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v4.py
+-rw-r--r--   0        0        0    47752 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v5.py
+-rw-r--r--   0        0        0    48520 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v6.py
+-rw-r--r--   0        0        0    52862 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v7.py
+-rw-r--r--   0        0        0    35032 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v8.py
+-rw-r--r--   0        0        0    39343 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v9.py
+-rw-r--r--   0        0        0      796 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/__init__.py
+-rw-r--r--   0        0        0     1719 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v1.py
+-rw-r--r--   0        0        0     1755 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v2.py
+-rw-r--r--   0        0        0     3346 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v3.py
+-rw-r--r--   0        0        0     3458 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v4.py
+-rw-r--r--   0        0        0     1839 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v5.py
+-rw-r--r--   0        0        0     1759 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v6.py
+-rw-r--r--   0        0        0      796 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/sources/__init__.py
+-rw-r--r--   0        0        0     2044 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/sources/sources_v1.py
+-rw-r--r--   0        0        0     2327 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/sources/sources_v2.py
+-rw-r--r--   0        0        0     2441 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/sources/sources_v3.py
+-rw-r--r--   0        0        0     2348 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/utils.py
+-rw-r--r--   0        0        0     5202 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/version_map.py
+-rw-r--r--   0        0        0     5968 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/catalog/catalog_v1.json
+-rw-r--r--   0        0        0   129577 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v1.json
+-rw-r--r--   0        0        0   148278 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v10.json
+-rw-r--r--   0        0        0   130575 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v11.json
+-rw-r--r--   0        0        0   724056 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v12.json
+-rw-r--r--   0        0        0   135379 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v2.json
+-rw-r--r--   0        0        0   138302 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v3.json
+-rw-r--r--   0        0        0   157235 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v4.json
+-rw-r--r--   0        0        0   159203 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v5.json
+-rw-r--r--   0        0        0   163791 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v6.json
+-rw-r--r--   0        0        0   174833 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v7.json
+-rw-r--r--   0        0        0   115570 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v8.json
+-rw-r--r--   0        0        0   129190 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v9.json
+-rw-r--r--   0        0        0     4622 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v1.json
+-rw-r--r--   0        0        0     4777 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v2.json
+-rw-r--r--   0        0        0     9817 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v3.json
+-rw-r--r--   0        0        0    10272 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v4.json
+-rw-r--r--   0        0        0     4690 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v5.json
+-rw-r--r--   0        0        0     4820 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v6.json
+-rw-r--r--   0        0        0     5568 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/sources/sources_v1.json
+-rw-r--r--   0        0        0     6790 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/sources/sources_v2.json
+-rw-r--r--   0        0        0     7249 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/sources/sources_v3.json
+-rw-r--r--   0        0        0     1017 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/utils.py
+-rw-r--r--   0        0        0     1828 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      830 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/setup.py
+-rw-r--r--   0        0        0    12383 1970-01-01 00:00:00.000000 dbt_artifacts_parser-0.6.0/PKG-INFO
```

### Comparing `dbt_artifacts_parser-0.5.1/LICENSE` & `dbt_artifacts_parser-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/README.md` & `dbt_artifacts_parser-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -277,14 +277,22 @@
         <a href="https://github.com/nabilm">
             <img src="https://avatars.githubusercontent.com/u/987369?v=4" width="100;" alt="nabilm"/>
             <br />
             <sub><b>Mohamed Nabil Mahmoud Hafez</b></sub>
         </a>
     </td>
     <td align="center">
+        <a href="https://github.com/OnkarVO7">
+            <img src="https://avatars.githubusercontent.com/u/28966081?v=4" width="100;" alt="OnkarVO7"/>
+            <br />
+            <sub><b>Onkar Ravgan</b></sub>
+        </a>
+    </td></tr>
+<tr>
+    <td align="center">
         <a href="https://github.com/meyer-glean">
             <img src="https://avatars.githubusercontent.com/u/134302890?v=4" width="100;" alt="meyer-glean"/>
             <br />
             <sub><b>Null</b></sub>
         </a>
     </td></tr>
 </table>
```

#### html2text {}

```diff
@@ -104,10 +104,12 @@
 sources_obj = parse_sources_v1(sources=sources_dict) # parse sources.json v2
 from dbt_artifacts_parser.parser import parse_sources_v2 with open("path/to/
 sources.json", "r") as fp: sources_dict = json.load(fp) sources_obj =
 parse_sources_v2(sources=sources_dict) # parse sources.json v3 from
 dbt_artifacts_parser.parser import parse_sources_v3 with open("path/to/
 sources.json", "r") as fp: sources_dict = json.load(fp) sources_obj =
 parse_sources_v3(sources=sources_dict) ``` ## Contributors
- _[_y_u_-_i_s_k_w_]  _[_d_l_a_w_i_n_]  _[_b_b_r_e_w_i_n_g_t_o_n_]   _[_j_u_d_a_h_r_a_n_d_]   _[_n_a_b_i_l_m_]    _[_m_e_y_e_r_-_g_l_e_a_n_]
-_YY_uu_ _II_ss_hh_ii_kk_aa_ww_aa   _NN_uu_ll_ll   _BB_rr_ee_nn_tt_ _BB_rr_ee_ww_ii_nn_gg_tt_oo_nn _JJ_uu_dd_aa_hh_ _RR_aa_nn_dd  _MM_oo_hh_aa_mm_ee_dd_ _NN_aa_bb_ii_ll     _NN_uu_ll_ll
-                                                  _MM_aa_hh_mm_oo_uu_dd_ _HH_aa_ff_ee_zz
+  _[_y_u_-_i_s_k_w_]   _[_d_l_a_w_i_n_]  _[_b_b_r_e_w_i_n_g_t_o_n_]   _[_j_u_d_a_h_r_a_n_d_]   _[_n_a_b_i_l_m_]     _[_O_n_k_a_r_V_O_7_]
+ _YY_uu_ _II_ss_hh_ii_kk_aa_ww_aa    _NN_uu_ll_ll   _BB_rr_ee_nn_tt_ _BB_rr_ee_ww_ii_nn_gg_tt_oo_nn _JJ_uu_dd_aa_hh_ _RR_aa_nn_dd  _MM_oo_hh_aa_mm_ee_dd_ _NN_aa_bb_ii_ll _OO_nn_kk_aa_rr_ _RR_aa_vv_gg_aa_nn
+                                                    _MM_aa_hh_mm_oo_uu_dd_ _HH_aa_ff_ee_zz
+_[_m_e_y_e_r_-_g_l_e_a_n_]
+    _NN_uu_ll_ll
```

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/__init__.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 """
 A dbt artifacts parser in python
 """
-__version__ = "0.5.1"
+__version__ = "0.6.0"
```

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parser.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,21 @@
 from dbt_artifacts_parser.parsers.manifest.manifest_v5 import ManifestV5
 from dbt_artifacts_parser.parsers.manifest.manifest_v6 import ManifestV6
 from dbt_artifacts_parser.parsers.manifest.manifest_v7 import ManifestV7
 from dbt_artifacts_parser.parsers.manifest.manifest_v8 import ManifestV8
 from dbt_artifacts_parser.parsers.manifest.manifest_v9 import ManifestV9
 from dbt_artifacts_parser.parsers.manifest.manifest_v10 import ManifestV10
 from dbt_artifacts_parser.parsers.manifest.manifest_v11 import ManifestV11
+from dbt_artifacts_parser.parsers.manifest.manifest_v12 import ManifestV12
 from dbt_artifacts_parser.parsers.run_results.run_results_v1 import RunResultsV1
 from dbt_artifacts_parser.parsers.run_results.run_results_v2 import RunResultsV2
 from dbt_artifacts_parser.parsers.run_results.run_results_v3 import RunResultsV3
 from dbt_artifacts_parser.parsers.run_results.run_results_v4 import RunResultsV4
 from dbt_artifacts_parser.parsers.run_results.run_results_v5 import RunResultsV5
+from dbt_artifacts_parser.parsers.run_results.run_results_v6 import RunResultsV6
 from dbt_artifacts_parser.parsers.sources.sources_v1 import SourcesV1
 from dbt_artifacts_parser.parsers.sources.sources_v2 import SourcesV2
 from dbt_artifacts_parser.parsers.sources.sources_v3 import SourcesV3
 from dbt_artifacts_parser.parsers.utils import get_dbt_schema_version
 from dbt_artifacts_parser.parsers.version_map import ArtifactTypes
 
 
@@ -78,14 +80,16 @@
         ManifestV4,
         ManifestV5,
         ManifestV6,
         ManifestV7,
         ManifestV8,
         ManifestV9,
         ManifestV10,
+        ManifestV11,
+        ManifestV12,
 ]:
     """Parse manifest.json
 
     Args:
         manifest: A dict of manifest.json
 
     Returns:
@@ -110,14 +114,16 @@
         return ManifestV8(**manifest)
     elif dbt_schema_version == ArtifactTypes.MANIFEST_V9.value.dbt_schema_version:
         return ManifestV9(**manifest)
     elif dbt_schema_version == ArtifactTypes.MANIFEST_V10.value.dbt_schema_version:
         return ManifestV10(**manifest)
     elif dbt_schema_version == ArtifactTypes.MANIFEST_V11.value.dbt_schema_version:
         return ManifestV11(**manifest)
+    elif dbt_schema_version == ArtifactTypes.MANIFEST_V12.value.dbt_schema_version:
+        return ManifestV12(**manifest)
     raise ValueError("Not a manifest.json")
 
 
 def parse_manifest_v1(manifest: dict) -> ManifestV1:
     """Parse manifest.json ver.1"""
     dbt_schema_version = get_dbt_schema_version(artifact_json=manifest)
     if dbt_schema_version == ArtifactTypes.MANIFEST_V1.value.dbt_schema_version:
@@ -200,21 +206,29 @@
     """Parse manifest.json ver.11"""
     dbt_schema_version = get_dbt_schema_version(artifact_json=manifest)
     if dbt_schema_version == ArtifactTypes.MANIFEST_V11.value.dbt_schema_version:
         return ManifestV11(**manifest)
     raise ValueError("Not a manifest.json v11")
 
 
+def parse_manifest_v12(manifest: dict) -> ManifestV12:
+    """Parse manifest.json ver.12"""
+    dbt_schema_version = get_dbt_schema_version(artifact_json=manifest)
+    if dbt_schema_version == ArtifactTypes.MANIFEST_V12.value.dbt_schema_version:
+        return ManifestV12(**manifest)
+    raise ValueError("Not a manifest.json v12")
+
+
 #
 # run-results
 #
 def parse_run_results(
     run_results: dict,
 ) -> Union[RunResultsV1, RunResultsV2, RunResultsV3, RunResultsV4,
-           RunResultsV5]:
+           RunResultsV5, RunResultsV6]:
     """Parse run-results.json
 
     Args:
         run_results: A dict of run-results.json
 
     Returns:
         Union[RunResultsV1, RunResultsV2, RunResultsV3, RunResultsV4]:
@@ -226,14 +240,16 @@
         return RunResultsV2(**run_results)
     elif dbt_schema_version == ArtifactTypes.RUN_RESULTS_V3.value.dbt_schema_version:
         return RunResultsV3(**run_results)
     elif dbt_schema_version == ArtifactTypes.RUN_RESULTS_V4.value.dbt_schema_version:
         return RunResultsV4(**run_results)
     elif dbt_schema_version == ArtifactTypes.RUN_RESULTS_V5.value.dbt_schema_version:
         return RunResultsV5(**run_results)
+    elif dbt_schema_version == ArtifactTypes.RUN_RESULTS_V6.value.dbt_schema_version:
+        return RunResultsV6(**run_results)
     raise ValueError("Not a manifest.json")
 
 
 def parse_run_results_v1(run_results: dict) -> RunResultsV1:
     """Parse run-results.json v1"""
     dbt_schema_version = get_dbt_schema_version(artifact_json=run_results)
     if dbt_schema_version == ArtifactTypes.RUN_RESULTS_V1.value.dbt_schema_version:
@@ -268,14 +284,21 @@
     """Parse run-results.json v5"""
     dbt_schema_version = get_dbt_schema_version(artifact_json=run_results)
     if dbt_schema_version == ArtifactTypes.RUN_RESULTS_V5.value.dbt_schema_version:
         return RunResultsV5(**run_results)
     raise ValueError("Not a run-results.json v5")
 
 
+def parse_run_results_v6(run_results: dict) -> RunResultsV6:
+    """Parse run-results.json v6"""
+    dbt_schema_version = get_dbt_schema_version(artifact_json=run_results)
+    if dbt_schema_version == ArtifactTypes.RUN_RESULTS_V6.value.dbt_schema_version:
+        return RunResultsV6(**run_results)
+    raise ValueError("Not a run-results.json v6")
+
 #
 # sources
 #
 def parse_sources(sources: dict) -> Union[SourcesV1, SourcesV2, SourcesV3]:
     """Parse sources.json
 
     Args:
```

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/__init__.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/base.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/base.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/catalog/__init__.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/catalog/catalog_v1.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/catalog/catalog_v1.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/__init__.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v1.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v1.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v10.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v10.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v11.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v11.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
 
 from pydantic import Extra, Field, constr
 
 from dbt_artifacts_parser.parsers.base import BaseParserModel
 
+
 class ResourceType11(Enum):
     doc = 'doc'
 class Documentation(BaseParserModel):
     class Config:
         extra = Extra.forbid
 
     name: str
```

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v2.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v2.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v3.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v3.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v4.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v4.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v5.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v5.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v6.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v6.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v7.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v7.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v8.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v8.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/manifest/manifest_v9.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v9.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/run_results/__init__.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/run_results/run_results_v1.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v1.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/run_results/run_results_v2.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v2.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/run_results/run_results_v3.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v3.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/run_results/run_results_v4.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v4.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/run_results/run_results_v5.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v5.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/sources/__init__.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/sources/sources_v1.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/sources/sources_v1.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/sources/sources_v2.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/sources/sources_v2.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/sources/sources_v3.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/sources/sources_v3.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/utils.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/parsers/version_map.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/version_map.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,19 +27,21 @@
 from dbt_artifacts_parser.parsers.manifest.manifest_v5 import ManifestV5
 from dbt_artifacts_parser.parsers.manifest.manifest_v6 import ManifestV6
 from dbt_artifacts_parser.parsers.manifest.manifest_v7 import ManifestV7
 from dbt_artifacts_parser.parsers.manifest.manifest_v8 import ManifestV8
 from dbt_artifacts_parser.parsers.manifest.manifest_v9 import ManifestV9
 from dbt_artifacts_parser.parsers.manifest.manifest_v10 import ManifestV10
 from dbt_artifacts_parser.parsers.manifest.manifest_v11 import ManifestV11
+from dbt_artifacts_parser.parsers.manifest.manifest_v12 import ManifestV12
 from dbt_artifacts_parser.parsers.run_results.run_results_v1 import RunResultsV1
 from dbt_artifacts_parser.parsers.run_results.run_results_v2 import RunResultsV2
 from dbt_artifacts_parser.parsers.run_results.run_results_v3 import RunResultsV3
 from dbt_artifacts_parser.parsers.run_results.run_results_v4 import RunResultsV4
 from dbt_artifacts_parser.parsers.run_results.run_results_v5 import RunResultsV5
+from dbt_artifacts_parser.parsers.run_results.run_results_v6 import RunResultsV6
 from dbt_artifacts_parser.parsers.sources.sources_v1 import SourcesV1
 from dbt_artifacts_parser.parsers.sources.sources_v2 import SourcesV2
 from dbt_artifacts_parser.parsers.sources.sources_v3 import SourcesV3
 
 
 @dataclass
 class ArtifactType:
@@ -47,70 +49,54 @@
     model_class: Type[BaseParserModel]
 
 
 class ArtifactTypes(Enum):
     """Dbt artifacts types"""
 
     # Catalog
-    CATALOG_V1 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/catalog/v1.json", CatalogV1
-    )
+    CATALOG_V1 = ArtifactType("https://schemas.getdbt.com/dbt/catalog/v1.json",
+                              CatalogV1)
     # Manifest
     MANIFEST_V1 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/manifest/v1.json", ManifestV1
-    )
+        "https://schemas.getdbt.com/dbt/manifest/v1.json", ManifestV1)
     MANIFEST_V2 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/manifest/v2.json", ManifestV2
-    )
+        "https://schemas.getdbt.com/dbt/manifest/v2.json", ManifestV2)
     MANIFEST_V3 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/manifest/v3.json", ManifestV3
-    )
+        "https://schemas.getdbt.com/dbt/manifest/v3.json", ManifestV3)
     MANIFEST_V4 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/manifest/v4.json", ManifestV4
-    )
+        "https://schemas.getdbt.com/dbt/manifest/v4.json", ManifestV4)
     MANIFEST_V5 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/manifest/v5.json", ManifestV5
-    )
+        "https://schemas.getdbt.com/dbt/manifest/v5.json", ManifestV5)
     MANIFEST_V6 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/manifest/v6.json", ManifestV6
-    )
+        "https://schemas.getdbt.com/dbt/manifest/v6.json", ManifestV6)
     MANIFEST_V7 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/manifest/v7.json", ManifestV7
-    )
+        "https://schemas.getdbt.com/dbt/manifest/v7.json", ManifestV7)
     MANIFEST_V8 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/manifest/v8.json", ManifestV8
-    )
+        "https://schemas.getdbt.com/dbt/manifest/v8.json", ManifestV8)
     MANIFEST_V9 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/manifest/v9.json", ManifestV9
-    )
+        "https://schemas.getdbt.com/dbt/manifest/v9.json", ManifestV9)
     MANIFEST_V10 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/manifest/v10.json", ManifestV10
-    )
+        "https://schemas.getdbt.com/dbt/manifest/v10.json", ManifestV10)
     MANIFEST_V11 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/manifest/v11.json", ManifestV11
-    )
+        "https://schemas.getdbt.com/dbt/manifest/v11.json", ManifestV11)
+    MANIFEST_V12 = ArtifactType(
+        "https://schemas.getdbt.com/dbt/manifest/v12.json", ManifestV12)
     # RunResults
     RUN_RESULTS_V1 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/run-results/v1.json", RunResultsV1
-    )
+        "https://schemas.getdbt.com/dbt/run-results/v1.json", RunResultsV1)
     RUN_RESULTS_V2 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/run-results/v2.json", RunResultsV2
-    )
+        "https://schemas.getdbt.com/dbt/run-results/v2.json", RunResultsV2)
     RUN_RESULTS_V3 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/run-results/v3.json", RunResultsV3
-    )
+        "https://schemas.getdbt.com/dbt/run-results/v3.json", RunResultsV3)
     RUN_RESULTS_V4 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/run-results/v4.json", RunResultsV4
-    )
+        "https://schemas.getdbt.com/dbt/run-results/v4.json", RunResultsV4)
     RUN_RESULTS_V5 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/run-results/v5.json", RunResultsV5
-    )
+        "https://schemas.getdbt.com/dbt/run-results/v5.json", RunResultsV5)
+    RUN_RESULTS_V6 = ArtifactType(
+        "https://schemas.getdbt.com/dbt/run-results/v6.json", RunResultsV6)
     # Sources
-    SOURCES_V1 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/sources/v1.json", SourcesV1
-    )
-    SOURCES_V2 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/sources/v2.json", SourcesV2
-    )
-    SOURCES_V3 = ArtifactType(
-        "https://schemas.getdbt.com/dbt/sources/v3.json", SourcesV3
-    )
+    SOURCES_V1 = ArtifactType("https://schemas.getdbt.com/dbt/sources/v1.json",
+                              SourcesV1)
+    SOURCES_V2 = ArtifactType("https://schemas.getdbt.com/dbt/sources/v2.json",
+                              SourcesV2)
+    SOURCES_V3 = ArtifactType("https://schemas.getdbt.com/dbt/sources/v3.json",
+                              SourcesV3)
```

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/catalog/catalog_v1.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/catalog/catalog_v1.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v1.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v1.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v10.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v10.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v11.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v11.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v2.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v2.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v3.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v3.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v4.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v4.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v5.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v5.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v6.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v6.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v7.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v7.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v8.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v8.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/manifest/manifest_v9.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v9.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/run-results/run-results_v1.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v1.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/run-results/run-results_v2.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v2.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/run-results/run-results_v3.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v3.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/run-results/run-results_v4.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v4.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/run-results/run-results_v5.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v5.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/sources/sources_v1.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/sources/sources_v1.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/sources/sources_v2.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/sources/sources_v2.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/resources/sources/sources_v3.json` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/sources/sources_v3.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/dbt_artifacts_parser/utils.py` & `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/pyproject.toml` & `dbt_artifacts_parser-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/setup.py` & `dbt_artifacts_parser-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.5.1/PKG-INFO` & `dbt_artifacts_parser-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-artifacts-parser
-Version: 0.5.1
+Version: 0.6.0
 Summary: A dbt artifacts parser in python
 Author: yu-iskw
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -319,14 +319,22 @@
         <a href="https://github.com/nabilm">
             <img src="https://avatars.githubusercontent.com/u/987369?v=4" width="100;" alt="nabilm"/>
             <br />
             <sub><b>Mohamed Nabil Mahmoud Hafez</b></sub>
         </a>
     </td>
     <td align="center">
+        <a href="https://github.com/OnkarVO7">
+            <img src="https://avatars.githubusercontent.com/u/28966081?v=4" width="100;" alt="OnkarVO7"/>
+            <br />
+            <sub><b>Onkar Ravgan</b></sub>
+        </a>
+    </td></tr>
+<tr>
+    <td align="center">
         <a href="https://github.com/meyer-glean">
             <img src="https://avatars.githubusercontent.com/u/134302890?v=4" width="100;" alt="meyer-glean"/>
             <br />
             <sub><b>Null</b></sub>
         </a>
     </td></tr>
 </table>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-artifacts-parser Version: 0.5.1 Summary: A dbt
+Metadata-Version: 2.1 Name: dbt-artifacts-parser Version: 0.6.0 Summary: A dbt
 artifacts parser in python Author: yu-iskw Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: Operating System :: OS
 Independent Classifier: Topic :: Software Development :: Libraries Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
@@ -128,10 +128,12 @@
 sources_obj = parse_sources_v1(sources=sources_dict) # parse sources.json v2
 from dbt_artifacts_parser.parser import parse_sources_v2 with open("path/to/
 sources.json", "r") as fp: sources_dict = json.load(fp) sources_obj =
 parse_sources_v2(sources=sources_dict) # parse sources.json v3 from
 dbt_artifacts_parser.parser import parse_sources_v3 with open("path/to/
 sources.json", "r") as fp: sources_dict = json.load(fp) sources_obj =
 parse_sources_v3(sources=sources_dict) ``` ## Contributors
- _[_y_u_-_i_s_k_w_]  _[_d_l_a_w_i_n_]  _[_b_b_r_e_w_i_n_g_t_o_n_]   _[_j_u_d_a_h_r_a_n_d_]   _[_n_a_b_i_l_m_]    _[_m_e_y_e_r_-_g_l_e_a_n_]
-_YY_uu_ _II_ss_hh_ii_kk_aa_ww_aa   _NN_uu_ll_ll   _BB_rr_ee_nn_tt_ _BB_rr_ee_ww_ii_nn_gg_tt_oo_nn _JJ_uu_dd_aa_hh_ _RR_aa_nn_dd  _MM_oo_hh_aa_mm_ee_dd_ _NN_aa_bb_ii_ll     _NN_uu_ll_ll
-                                                  _MM_aa_hh_mm_oo_uu_dd_ _HH_aa_ff_ee_zz
+  _[_y_u_-_i_s_k_w_]   _[_d_l_a_w_i_n_]  _[_b_b_r_e_w_i_n_g_t_o_n_]   _[_j_u_d_a_h_r_a_n_d_]   _[_n_a_b_i_l_m_]     _[_O_n_k_a_r_V_O_7_]
+ _YY_uu_ _II_ss_hh_ii_kk_aa_ww_aa    _NN_uu_ll_ll   _BB_rr_ee_nn_tt_ _BB_rr_ee_ww_ii_nn_gg_tt_oo_nn _JJ_uu_dd_aa_hh_ _RR_aa_nn_dd  _MM_oo_hh_aa_mm_ee_dd_ _NN_aa_bb_ii_ll _OO_nn_kk_aa_rr_ _RR_aa_vv_gg_aa_nn
+                                                    _MM_aa_hh_mm_oo_uu_dd_ _HH_aa_ff_ee_zz
+_[_m_e_y_e_r_-_g_l_e_a_n_]
+    _NN_uu_ll_ll
```

