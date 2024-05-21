# Comparing `tmp/idc_index-0.5.6.tar.gz` & `tmp/idc_index-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri May 17 21:32:59 2024, max compression
+gzip compressed data, last modified: Tue May 21 15:49:49 2024, max compression
```

## Comparing `idc_index-0.5.6.tar` & `idc_index-0.5.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      125 2024-05-17 21:32:59.000000 idc_index-0.5.6/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-05-17 21:32:59.000000 idc_index-0.5.6/.gitattributes
--rw-r--r--   0        0        0     2357 2024-05-17 21:32:59.000000 idc_index-0.5.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-05-17 21:32:59.000000 idc_index-0.5.6/.readthedocs.yaml
--rw-r--r--   0        0        0     2742 2024-05-17 21:32:59.000000 idc_index-0.5.6/noxfile.py
--rw-r--r--   0        0        0     2394 2024-05-17 21:32:59.000000 idc_index-0.5.6/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-05-17 21:32:59.000000 idc_index-0.5.6/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-05-17 21:32:59.000000 idc_index-0.5.6/.github/matchers/pylint.json
--rw-r--r--   0        0        0      847 2024-05-17 21:32:59.000000 idc_index-0.5.6/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1585 2024-05-17 21:32:59.000000 idc_index-0.5.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0      355 2024-05-17 21:32:59.000000 idc_index-0.5.6/.github/workflows/keep-alive.yaml
--rw-r--r--   0        0        0      920 2024-05-17 21:32:59.000000 idc_index-0.5.6/docs/conf.py
--rw-r--r--   0        0        0      662 2024-05-17 21:32:59.000000 idc_index-0.5.6/docs/index.md
--rw-r--r--   0        0        0      278 2024-05-17 21:32:59.000000 idc_index-0.5.6/docs/api/idc_index.rst
--rw-r--r--   0        0        0      262 2024-05-17 21:32:59.000000 idc_index-0.5.6/idc_index/__init__.py
--rw-r--r--   0        0        0      411 2024-05-17 21:32:59.000000 idc_index-0.5.6/idc_index/_version.py
--rw-r--r--   0        0        0      118 2024-05-17 21:32:59.000000 idc_index-0.5.6/idc_index/_version.pyi
--rw-r--r--   0        0        0    64739 2024-05-17 21:32:59.000000 idc_index-0.5.6/idc_index/index.py
--rw-r--r--   0        0        0        0 2024-05-17 21:32:59.000000 idc_index-0.5.6/idc_index/py.typed
--rw-r--r--   0        0        0        0 2024-05-17 21:32:59.000000 idc_index-0.5.6/tests/__init__.py
--rw-r--r--   0        0        0    14639 2024-05-17 21:32:59.000000 idc_index-0.5.6/tests/idcindex.py
--rw-r--r--   0        0        0      413 2024-05-17 21:32:59.000000 idc_index-0.5.6/tests/study_manifest_aws.s5cmd
--rw-r--r--   0        0        0      279 2024-05-17 21:32:59.000000 idc_index-0.5.6/tests/study_manifest_bogus.s5cmd
--rw-r--r--   0        0        0      419 2024-05-17 21:32:59.000000 idc_index-0.5.6/tests/study_manifest_gcs.s5cmd
--rw-r--r--   0        0        0      175 2024-05-17 21:32:59.000000 idc_index-0.5.6/tests/test_package.py
--rw-r--r--   0        0        0     2265 2024-05-17 21:32:59.000000 idc_index-0.5.6/.gitignore
--rw-r--r--   0        0        0     1077 2024-05-17 21:32:59.000000 idc_index-0.5.6/LICENSE
--rw-r--r--   0        0        0     4303 2024-05-17 21:32:59.000000 idc_index-0.5.6/README.md
--rw-r--r--   0        0        0     6269 2024-05-17 21:32:59.000000 idc_index-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     7588 2024-05-17 21:32:59.000000 idc_index-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-05-21 15:49:49.000000 idc_index-0.5.7/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-05-21 15:49:49.000000 idc_index-0.5.7/.gitattributes
+-rw-r--r--   0        0        0     2357 2024-05-21 15:49:49.000000 idc_index-0.5.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-05-21 15:49:49.000000 idc_index-0.5.7/.readthedocs.yaml
+-rw-r--r--   0        0        0     2742 2024-05-21 15:49:49.000000 idc_index-0.5.7/noxfile.py
+-rw-r--r--   0        0        0     2394 2024-05-21 15:49:49.000000 idc_index-0.5.7/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-05-21 15:49:49.000000 idc_index-0.5.7/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-05-21 15:49:49.000000 idc_index-0.5.7/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      847 2024-05-21 15:49:49.000000 idc_index-0.5.7/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1585 2024-05-21 15:49:49.000000 idc_index-0.5.7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      355 2024-05-21 15:49:49.000000 idc_index-0.5.7/.github/workflows/keep-alive.yaml
+-rw-r--r--   0        0        0      920 2024-05-21 15:49:49.000000 idc_index-0.5.7/docs/conf.py
+-rw-r--r--   0        0        0      662 2024-05-21 15:49:49.000000 idc_index-0.5.7/docs/index.md
+-rw-r--r--   0        0        0      278 2024-05-21 15:49:49.000000 idc_index-0.5.7/docs/api/idc_index.rst
+-rw-r--r--   0        0        0      262 2024-05-21 15:49:49.000000 idc_index-0.5.7/idc_index/__init__.py
+-rw-r--r--   0        0        0      411 2024-05-21 15:49:49.000000 idc_index-0.5.7/idc_index/_version.py
+-rw-r--r--   0        0        0      118 2024-05-21 15:49:49.000000 idc_index-0.5.7/idc_index/_version.pyi
+-rw-r--r--   0        0        0    66810 2024-05-21 15:49:49.000000 idc_index-0.5.7/idc_index/index.py
+-rw-r--r--   0        0        0        0 2024-05-21 15:49:49.000000 idc_index-0.5.7/idc_index/py.typed
+-rw-r--r--   0        0        0        0 2024-05-21 15:49:49.000000 idc_index-0.5.7/tests/__init__.py
+-rw-r--r--   0        0        0    14766 2024-05-21 15:49:49.000000 idc_index-0.5.7/tests/idcindex.py
+-rw-r--r--   0        0        0      413 2024-05-21 15:49:49.000000 idc_index-0.5.7/tests/study_manifest_aws.s5cmd
+-rw-r--r--   0        0        0      279 2024-05-21 15:49:49.000000 idc_index-0.5.7/tests/study_manifest_bogus.s5cmd
+-rw-r--r--   0        0        0      419 2024-05-21 15:49:49.000000 idc_index-0.5.7/tests/study_manifest_gcs.s5cmd
+-rw-r--r--   0        0        0      175 2024-05-21 15:49:49.000000 idc_index-0.5.7/tests/test_package.py
+-rw-r--r--   0        0        0     2265 2024-05-21 15:49:49.000000 idc_index-0.5.7/.gitignore
+-rw-r--r--   0        0        0     1077 2024-05-21 15:49:49.000000 idc_index-0.5.7/LICENSE
+-rw-r--r--   0        0        0     4303 2024-05-21 15:49:49.000000 idc_index-0.5.7/README.md
+-rw-r--r--   0        0        0     6269 2024-05-21 15:49:49.000000 idc_index-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     7588 2024-05-21 15:49:49.000000 idc_index-0.5.7/PKG-INFO
```

### Comparing `idc_index-0.5.6/.pre-commit-config.yaml` & `idc_index-0.5.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.6/noxfile.py` & `idc_index-0.5.7/noxfile.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.6/.github/CONTRIBUTING.md` & `idc_index-0.5.7/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.6/.github/matchers/pylint.json` & `idc_index-0.5.7/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.6/.github/workflows/cd.yml` & `idc_index-0.5.7/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.6/.github/workflows/ci.yml` & `idc_index-0.5.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.6/docs/conf.py` & `idc_index-0.5.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.6/docs/index.md` & `idc_index-0.5.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.6/idc_index/index.py` & `idc_index-0.5.7/idc_index/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1176,30 +1176,81 @@
             quiet=quiet,
             show_progress_bar=show_progress_bar,
             use_s5cmd_sync=use_s5cmd_sync,
             dirTemplate=dirTemplate,
             list_of_directories=list_of_directories,
         )
 
+    def citations_from_manifest(
+        self,
+        manifestFile: str,
+        citation_format: str = CITATION_FORMAT_APA,
+    ):
+        """Get the list of publications that should be cited/attributed for a cohort defined by a manifest.
+
+        Args:
+            manifestFile (str: string containing the path to the manifest file.
+            format (str): string containing the format of the citation. Must be one of the following: CITATION_FORMAT_APA, CITATION_FORMAT_BIBTEX, CITATION_FORMAT_JSON. Defaults to CITATION_FORMAT_APA. Can be initialized to the alternative formats as allowed by DOI API, see https://citation.crosscite.org/docs.html#sec-4.
+
+        Returns:
+            List of citations in the requested format.
+        """
+
+        manifest_df = pd.read_csv(
+            manifestFile,
+            comment="#",
+            skip_blank_lines=True,
+            header=None,
+            names=["manifest_line"],
+        )
+        uuid_pattern = r"s3://.*/([^/]+)/\*"
+        manifest_df["crdc_series_uuid"] = manifest_df["manifest_line"].str.extract(
+            uuid_pattern, expand=False
+        )
+        index_copy = self.index[["series_aws_url", "SeriesInstanceUID"]].copy()
+        index_copy["crdc_series_uuid"] = index_copy["series_aws_url"].str.extract(
+            uuid_pattern, expand=False
+        )
+        query = """
+        SELECT
+          SeriesInstanceUID
+        FROM
+          index_copy
+        JOIN
+          manifest_df
+        ON
+          index_copy.crdc_series_uuid = manifest_df.crdc_series_uuid
+        """
+
+        result_df = self.sql_query(query)
+
+        return self.citations_from_selection(
+            seriesInstanceUID=result_df["SeriesInstanceUID"].tolist(),
+            citation_format=citation_format,
+        )
+
     def citations_from_selection(
         self,
         collection_id=None,
         patientId=None,
         studyInstanceUID=None,
         seriesInstanceUID=None,
         citation_format=CITATION_FORMAT_APA,
     ):
         """Get the list of publications that should be cited/attributed for the specific collection, patient (case) ID, study or series UID.
 
         Args:
             collection_id: string or list of strings containing the values of collection_id to filter by
             patientId: string or list of strings containing the values of PatientID to filter by
-            studyInstanceUID: string or list of strings containing the values of DICOM StudyInstanceUID to filter by
+            studyInstanceUID (str): string or list of strings containing the values of DICOM StudyInstanceUID to filter by
             seriesInstanceUID: string or list of strings containing the values of DICOM SeriesInstanceUID to filter by
             format: string containing the format of the citation. Must be one of the following: CITATION_FORMAT_APA, CITATION_FORMAT_BIBTEX, CITATION_FORMAT_JSON. Defaults to CITATION_FORMAT_APA. Can be initialized to the alternative formats as allowed by DOI API, see https://citation.crosscite.org/docs.html#sec-4.
+
+        Returns:
+            List of citations in the requested format.
         """
         result_df = self._safe_filter_by_selection(
             self.index,
             collection_id=collection_id,
             patientId=patientId,
             studyInstanceUID=studyInstanceUID,
             seriesInstanceUID=seriesInstanceUID,
@@ -1220,21 +1271,27 @@
 
             headers = {"accept": citation_format}
             timeout = 30
 
             for doi in distinct_dois:
                 url = "https://dx.doi.org/" + doi
 
+                logger.debug(f"Requesting citation for DOI: {doi}")
+
                 response = requests.get(url, headers=headers, timeout=timeout)
 
+                logger.debug("Received response: " + str(response.status_code))
+
                 if response.status_code == 200:
                     if citation_format == self.CITATION_FORMAT_JSON:
                         citations.append(response.json())
                     else:
                         citations.append(response.text)
+                    logger.debug("Received citation: " + citations[-1])
+
                 else:
                     logger.error(f"Failed to get citation for DOI: {url}")
 
         return citations
 
     def download_from_selection(
         self,
```

### Comparing `idc_index-0.5.6/tests/idcindex.py` & `idc_index-0.5.7/tests/idcindex.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,10 +366,13 @@
 
         citations = self.client.citations_from_selection(
             studyInstanceUID="1.2.840.113654.2.55.174144834924218414213677353968537663991",
             citation_format=index.IDCClient.CITATION_FORMAT_BIBTEX,
         )
         self.assertIsNotNone(citations)
 
+        citations = self.client.citations_from_manifest("./study_manifest_aws.s5cmd")
+        self.assertIsNotNone(citations)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `idc_index-0.5.6/.gitignore` & `idc_index-0.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.6/LICENSE` & `idc_index-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.6/README.md` & `idc_index-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.6/pyproject.toml` & `idc_index-0.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.6/PKG-INFO` & `idc_index-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: idc-index
-Version: 0.5.6
+Version: 0.5.7
 Summary: Package to query and download data from an index of ImagingDataCommons
 Project-URL: Homepage, https://github.com/ImagingDataCommons/idc-index
 Project-URL: Bug Tracker, https://github.com/ImagingDataCommons/idc-index/issues
 Project-URL: Discussions, https://discourse.canceridc.dev/
 Project-URL: Changelog, https://github.com/ImagingDataCommons/idc-index/releases
 Author-email: Andrey Fedorov <andrey.fedorov@gmail.com>, Vamsi Thiriveedhi <vthiriveedhi@mgh.harvard.edu>
 License: MIT License
```

