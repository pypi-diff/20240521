# Comparing `tmp/dataextractoroeg-0.5.1.tar.gz` & `tmp/dataextractoroeg-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dataextractoroeg-0.5.1.tar", last modified: Tue May 14 11:01:07 2024, max compression
+gzip compressed data, was "dist\dataextractoroeg-0.5.2.tar", last modified: Tue May 21 08:43:08 2024, max compression
```

## Comparing `dataextractoroeg-0.5.1.tar` & `dataextractoroeg-0.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 11:01:07.522965 dataextractoroeg-0.5.1/
--rw-rw-rw-   0        0        0      277 2024-05-14 11:00:46.000000 dataextractoroeg-0.5.1/.gitignore
-drwxrwxrwx   0        0        0        0 2024-05-14 11:01:07.521372 dataextractoroeg-0.5.1/DataExtractorOEG.egg-info/
--rw-rw-rw-   0        0        0     4299 2024-05-14 11:01:07.000000 dataextractoroeg-0.5.1/DataExtractorOEG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2024-05-14 11:01:07.000000 dataextractoroeg-0.5.1/DataExtractorOEG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 11:01:07.000000 dataextractoroeg-0.5.1/DataExtractorOEG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-14 11:01:07.000000 dataextractoroeg-0.5.1/DataExtractorOEG.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-05-14 11:01:07.000000 dataextractoroeg-0.5.1/DataExtractorOEG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-14 11:01:07.000000 dataextractoroeg-0.5.1/DataExtractorOEG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.5.1/LICENSE.txt
--rw-rw-rw-   0        0        0     4299 2024-05-14 11:01:07.522965 dataextractoroeg-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     4030 2024-05-14 08:44:15.000000 dataextractoroeg-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 11:01:07.509512 dataextractoroeg-0.5.1/doiExtractor/
-drwxrwxrwx   0        0        0        0 2024-05-14 11:01:07.517518 dataextractoroeg-0.5.1/doiExtractor/ExistingPapers/
--rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.5.1/doiExtractor/ExistingPapers/Papers.csv
--rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.5.1/doiExtractor/ExistingPapers/name_doi_papers.csv
--rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.5.1/doiExtractor/__init__.py
--rw-rw-rw-   0        0        0     8437 2024-05-14 11:00:05.000000 dataextractoroeg-0.5.1/doiExtractor/doiExtractor.py
--rw-rw-rw-   0        0        0     2497 2024-05-14 10:51:29.000000 dataextractoroeg-0.5.1/doiExtractor/main.py
--rw-rw-rw-   0        0        0     4116 2024-05-09 10:14:04.000000 dataextractoroeg-0.5.1/doiExtractor/openAlex.py
--rw-rw-rw-   0        0        0       42 2024-05-14 11:01:07.522965 dataextractoroeg-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      633 2024-05-14 11:00:58.000000 dataextractoroeg-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:43:08.546008 dataextractoroeg-0.5.2/
+-rw-rw-rw-   0        0        0      277 2024-05-20 16:51:52.000000 dataextractoroeg-0.5.2/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-21 08:43:08.539156 dataextractoroeg-0.5.2/DataExtractorOEG.egg-info/
+-rw-rw-rw-   0        0        0     4299 2024-05-21 08:43:08.000000 dataextractoroeg-0.5.2/DataExtractorOEG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2024-05-21 08:43:08.000000 dataextractoroeg-0.5.2/DataExtractorOEG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 08:43:08.000000 dataextractoroeg-0.5.2/DataExtractorOEG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-21 08:43:08.000000 dataextractoroeg-0.5.2/DataExtractorOEG.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-05-21 08:43:08.000000 dataextractoroeg-0.5.2/DataExtractorOEG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-21 08:43:08.000000 dataextractoroeg-0.5.2/DataExtractorOEG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.5.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     4299 2024-05-21 08:43:08.539156 dataextractoroeg-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4030 2024-05-14 08:44:15.000000 dataextractoroeg-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 08:43:08.505751 dataextractoroeg-0.5.2/doiExtractor/
+drwxrwxrwx   0        0        0        0 2024-05-21 08:43:08.529154 dataextractoroeg-0.5.2/doiExtractor/ExistingPapers/
+-rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.5.2/doiExtractor/ExistingPapers/Papers.csv
+-rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.5.2/doiExtractor/ExistingPapers/name_doi_papers.csv
+-rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.5.2/doiExtractor/__init__.py
+-rw-rw-rw-   0        0        0     8437 2024-05-14 11:00:05.000000 dataextractoroeg-0.5.2/doiExtractor/doiExtractor.py
+-rw-rw-rw-   0        0        0     2497 2024-05-20 16:51:26.000000 dataextractoroeg-0.5.2/doiExtractor/main.py
+-rw-rw-rw-   0        0        0     5254 2024-05-20 17:16:21.000000 dataextractoroeg-0.5.2/doiExtractor/openAlex.py
+-rw-rw-rw-   0        0        0       42 2024-05-21 08:43:08.546008 dataextractoroeg-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      633 2024-05-21 08:42:22.000000 dataextractoroeg-0.5.2/setup.py
```

### Comparing `dataextractoroeg-0.5.1/DataExtractorOEG.egg-info/PKG-INFO` & `dataextractoroeg-0.5.2/DataExtractorOEG.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.5.1
+Version: 0.5.2
 Author: Pablo Torija Martínez
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.5.1/LICENSE.txt` & `dataextractoroeg-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.5.1/PKG-INFO` & `dataextractoroeg-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.5.1
+Version: 0.5.2
 Author: Pablo Torija Martínez
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.5.1/README.md` & `dataextractoroeg-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.5.1/doiExtractor/ExistingPapers/Papers.csv` & `dataextractoroeg-0.5.2/doiExtractor/ExistingPapers/Papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.5.1/doiExtractor/ExistingPapers/name_doi_papers.csv` & `dataextractoroeg-0.5.2/doiExtractor/ExistingPapers/name_doi_papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.5.1/doiExtractor/doiExtractor.py` & `dataextractoroeg-0.5.2/doiExtractor/doiExtractor.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.5.1/doiExtractor/main.py` & `dataextractoroeg-0.5.2/doiExtractor/main.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.5.1/doiExtractor/openAlex.py` & `dataextractoroeg-0.5.2/doiExtractor/openAlex.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,21 +10,30 @@
         data = response.json()
         if data.get("id"):
             primary_location = data.get("primary_location")
             if primary_location:
                 landing_page_url = primary_location.get("landing_page_url")
                 pdf_url = primary_location.get("pdf_url")
                 
-                # Check if either landing_page_url or pdf_url ends with ".pdf"
-                if landing_page_url and landing_page_url.endswith(".pdf"):
-                    return landing_page_url, doi
-                elif pdf_url is not None:
-                    return pdf_url, doi
-                elif landing_page_url:
-                    return landing_page_url, doi
+                # Check both URLs for 'application/pdf' content type
+                if landing_page_url:
+                    checked_landing_page_url = check_pdf(landing_page_url)
+                    if checked_landing_page_url:
+                        print(f"Found PDF for {doi}: {checked_landing_page_url}")
+                        return checked_landing_page_url, doi
+
+                if pdf_url:
+                    checked_pdf_url = check_pdf(pdf_url)
+                    if checked_pdf_url:
+                        print(f"Found PDF for {doi}: {checked_pdf_url}")
+                        return checked_pdf_url, doi
+                    
+                else: 
+                    print(f"No PDF found for {doi}")
+                    return None ,doi
     else:
         return get_primary_location_by_title(name, doi)
 
 
 
 def get_primary_location_by_title(name, doi, include_doi=False):
     search_url = "https://api.openalex.org/works?filter=title.search:"
@@ -48,21 +57,29 @@
                         else:
                             doi = None
                     else:
                         doi = None
                 else:
                     doi = None
                 
-                # Check if either landing_page_url or pdf_url ends with ".pdf"
-                if landing_page_url and landing_page_url.endswith(".pdf"):
-                    return landing_page_url, doi
-                elif pdf_url is not None:
-                    return pdf_url, doi
-                elif landing_page_url:
-                    return landing_page_url, doi
+                # Check both URLs for 'application/pdf' content type
+                if landing_page_url:
+                    checked_landing_page_url = check_pdf(landing_page_url)
+                    if checked_landing_page_url:
+                        print(f"Found PDF for {name}: {checked_landing_page_url}")
+                        return checked_landing_page_url, doi
+
+                if pdf_url:
+                    checked_pdf_url = check_pdf(pdf_url)
+                    if checked_pdf_url:
+                        print(f"Found PDF for {name}: {checked_pdf_url}")
+                        return checked_pdf_url, doi
+                     
+                print(f"No PDF found for {name}")
+                return None ,doi
     return None, None
 
 
 def add_primary_location_to_csv(csv_filename):
     with open(csv_filename, mode='r', newline='', encoding='utf-8') as file:
         reader = csv.DictReader(file)
         rows = list(reader)
@@ -72,27 +89,41 @@
         doi = row["doi"] 
 
         # If doi is None, add the doi founded in OpenAlex
         if doi == "":
             page_url = get_primary_location_by_title(name, doi, include_doi=True)
             if page_url[1] is not None:
                 row["doi"] = page_url[1]
-                print(f"Searching in OpenAlex for DOI of {name}: {page_url[1]}")
         else:
             page_url = get_primary_location_by_doi(name, doi)
         
-        if page_url[0] is not None:
+        if page_url and page_url[0] is not None:
             row["primary_location"] = page_url[0]
-            print(f"Searching in OpenAlex for {name} \nFounded link:{page_url[0]}")
         else:
             row["primary_location"] = ""
-            print(f"Searching in OpenAlex for {name}: No primary location")
+            if doi:
+                print(f"No primary location for {doi}")
+            else:
+                if name:
+                    print(f"No primary location for {name}")  
         print("-----------------------------------------------------------------")
 
     new_columns = list(rows[0].keys())  
     if "primary_location" not in new_columns: 
         new_columns.append("primary_location")
 
     with open(csv_filename, mode='w', newline='', encoding='utf-8') as file:
         writer = csv.DictWriter(file, quoting=csv.QUOTE_ALL, fieldnames=new_columns)
         writer.writeheader()
-        writer.writerows(rows)
+        writer.writerows(rows)
+
+
+def check_pdf(url):
+        try:
+            response = requests.head(url, allow_redirects=True)
+            response.raise_for_status()
+            content_type = response.headers.get('Content-Type')
+            if content_type == 'application/pdf':
+                return url
+        except requests.exceptions.RequestException as e:
+            print(f"Error checking URL {url}: {e}")
+        return None
```

### Comparing `dataextractoroeg-0.5.1/setup.py` & `dataextractoroeg-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="DataExtractorOEG",
-    version="0.5.1",
+    version="0.5.2",
     author =  "Pablo Torija Martínez",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "beautifulsoup4",
         "selenium",
         "requests",
```

