# Comparing `tmp/starrydata-1.0.2.tar.gz` & `tmp/starrydata-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrydata-1.0.2.tar", last modified: Thu May 16 03:42:29 2024, max compression
+gzip compressed data, was "starrydata-1.1.0.tar", last modified: Tue May 21 07:54:05 2024, max compression
```

## Comparing `starrydata-1.0.2.tar` & `starrydata-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-16 03:42:29.254779 starrydata-1.0.2/
--rw-r--r--   0 matotomoya   (501) staff       (20)     1073 2023-12-12 10:27:13.000000 starrydata-1.0.2/LICENSE
--rw-r--r--   0 matotomoya   (501) staff       (20)     2202 2024-05-16 03:42:29.254488 starrydata-1.0.2/PKG-INFO
--rw-r--r--   0 matotomoya   (501) staff       (20)     1610 2024-05-16 03:42:03.000000 starrydata-1.0.2/README.md
--rw-r--r--   0 matotomoya   (501) staff       (20)      576 2024-05-16 03:42:27.000000 starrydata-1.0.2/pyproject.toml
--rw-r--r--   0 matotomoya   (501) staff       (20)       38 2024-05-16 03:42:29.254848 starrydata-1.0.2/setup.cfg
-drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-16 03:42:29.252181 starrydata-1.0.2/src/
-drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-16 03:42:29.253161 starrydata-1.0.2/src/starrydata/
--rw-r--r--   0 matotomoya   (501) staff       (20)        0 2024-05-15 03:36:37.000000 starrydata-1.0.2/src/starrydata/__init__.py
--rw-r--r--   0 matotomoya   (501) staff       (20)     5740 2024-05-15 06:22:44.000000 starrydata-1.0.2/src/starrydata/dataset.py
--rw-r--r--   0 matotomoya   (501) staff       (20)     4914 2024-05-12 10:10:09.000000 starrydata-1.0.2/src/starrydata/test_dataset.py
-drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-16 03:42:29.254218 starrydata-1.0.2/src/starrydata.egg-info/
--rw-r--r--   0 matotomoya   (501) staff       (20)     2202 2024-05-16 03:42:29.000000 starrydata-1.0.2/src/starrydata.egg-info/PKG-INFO
--rw-r--r--   0 matotomoya   (501) staff       (20)      305 2024-05-16 03:42:29.000000 starrydata-1.0.2/src/starrydata.egg-info/SOURCES.txt
--rw-r--r--   0 matotomoya   (501) staff       (20)        1 2024-05-16 03:42:29.000000 starrydata-1.0.2/src/starrydata.egg-info/dependency_links.txt
--rw-r--r--   0 matotomoya   (501) staff       (20)       21 2024-05-16 03:42:29.000000 starrydata-1.0.2/src/starrydata.egg-info/requires.txt
--rw-r--r--   0 matotomoya   (501) staff       (20)       11 2024-05-16 03:42:29.000000 starrydata-1.0.2/src/starrydata.egg-info/top_level.txt
+drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 07:54:05.075660 starrydata-1.1.0/
+-rw-r--r--   0 matotomoya   (501) staff       (20)     1073 2023-12-12 10:27:13.000000 starrydata-1.1.0/LICENSE
+-rw-r--r--   0 matotomoya   (501) staff       (20)     2724 2024-05-21 07:54:05.075344 starrydata-1.1.0/PKG-INFO
+-rw-r--r--   0 matotomoya   (501) staff       (20)     2132 2024-05-21 07:17:33.000000 starrydata-1.1.0/README.md
+-rw-r--r--   0 matotomoya   (501) staff       (20)      576 2024-05-21 07:54:02.000000 starrydata-1.1.0/pyproject.toml
+-rw-r--r--   0 matotomoya   (501) staff       (20)       38 2024-05-21 07:54:05.075737 starrydata-1.1.0/setup.cfg
+drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 07:54:05.072834 starrydata-1.1.0/src/
+drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 07:54:05.073886 starrydata-1.1.0/src/starrydata/
+-rw-r--r--   0 matotomoya   (501) staff       (20)      183 2024-05-21 06:08:13.000000 starrydata-1.1.0/src/starrydata/__init__.py
+-rw-r--r--   0 matotomoya   (501) staff       (20)     6532 2024-05-21 07:16:15.000000 starrydata-1.1.0/src/starrydata/dataset.py
+-rw-r--r--   0 matotomoya   (501) staff       (20)     4914 2024-05-12 10:10:09.000000 starrydata-1.1.0/src/starrydata/test_dataset.py
+drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-21 07:54:05.075038 starrydata-1.1.0/src/starrydata.egg-info/
+-rw-r--r--   0 matotomoya   (501) staff       (20)     2724 2024-05-21 07:54:05.000000 starrydata-1.1.0/src/starrydata.egg-info/PKG-INFO
+-rw-r--r--   0 matotomoya   (501) staff       (20)      305 2024-05-21 07:54:05.000000 starrydata-1.1.0/src/starrydata.egg-info/SOURCES.txt
+-rw-r--r--   0 matotomoya   (501) staff       (20)        1 2024-05-21 07:54:05.000000 starrydata-1.1.0/src/starrydata.egg-info/dependency_links.txt
+-rw-r--r--   0 matotomoya   (501) staff       (20)       21 2024-05-21 07:54:05.000000 starrydata-1.1.0/src/starrydata.egg-info/requires.txt
+-rw-r--r--   0 matotomoya   (501) staff       (20)       11 2024-05-21 07:54:05.000000 starrydata-1.1.0/src/starrydata.egg-info/top_level.txt
```

### Comparing `starrydata-1.0.2/LICENSE` & `starrydata-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starrydata-1.0.2/PKG-INFO` & `starrydata-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrydata
-Version: 1.0.2
+Version: 1.1.0
 Summary: Starrydata Python useful tools 
 Author-email: MATO Tomoya <tomoya.matou@gmail.com>
 Project-URL: Homepage, https://github.com/starrydata/starrydata-python-library
 Project-URL: Issues, https://github.com/starrydata/starrydata-python-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,27 +31,35 @@
 Below is an example of how to use Starrydata.
 
 ### Downloading a Dataset
 
 To download a specific dataset, use the `Dataset` class. Here is an example of how to download and load a dataset into a pandas DataFrame:
 
 ```python
-from starrydata import Dataset
-import pandas as pd
+import starrydata as sd  # Import the Starrydata library
+import pandas as pd  # Import the pandas library
 
-# Initialize the Dataset object with a specific date
-dataset = Dataset(date="20240515")
+# Load the dataset for the specified date
+sd_dataset = sd.load_dataset(date="20240521")
 
-# Load the dataset into a pandas DataFrame
-df = pd.read_csv(dataset.all_curves)
+# Print the dataset timestamp to confirm the download date
+print(sd_dataset.dataset_timestamp)
 
-# Display the DataFrame
-print(df)
+# Read the 'all_curves.csv' file from the dataset and convert it to a pandas DataFrame
+df_curves = pd.read_csv(sd_dataset.curves_csv)
+
+# Read the 'all_samples.csv' file from the dataset and convert it to a pandas DataFrame
+df_samples = pd.read_csv(sd_dataset.samples_csv)
+
+# Read the 'all_papers.json' file from the dataset and convert it to a pandas DataFrame
+df_papers = pd.read_json(sd_dataset.papers_json)
 ```
 
+More details is [1_how_to_use.ipynb](example_notebooks/1_how_to_use.ipynb)
+
 ## Documentation
 
 For more detailed documentation and usage examples, please refer to the [official documentation](https://pypi.org/project/starrydata/).
 
 ## Contributing
 
 Bug reports and feature requests are welcome at the [GitHub repository](https://github.com/starrydata/starrydata-python-library/). Contributions to the codebase are also appreciated. Follow these steps to contribute:
```

### Comparing `starrydata-1.0.2/README.md` & `starrydata-1.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -15,27 +15,35 @@
 Below is an example of how to use Starrydata.
 
 ### Downloading a Dataset
 
 To download a specific dataset, use the `Dataset` class. Here is an example of how to download and load a dataset into a pandas DataFrame:
 
 ```python
-from starrydata import Dataset
-import pandas as pd
+import starrydata as sd  # Import the Starrydata library
+import pandas as pd  # Import the pandas library
 
-# Initialize the Dataset object with a specific date
-dataset = Dataset(date="20240515")
+# Load the dataset for the specified date
+sd_dataset = sd.load_dataset(date="20240521")
 
-# Load the dataset into a pandas DataFrame
-df = pd.read_csv(dataset.all_curves)
+# Print the dataset timestamp to confirm the download date
+print(sd_dataset.dataset_timestamp)
 
-# Display the DataFrame
-print(df)
+# Read the 'all_curves.csv' file from the dataset and convert it to a pandas DataFrame
+df_curves = pd.read_csv(sd_dataset.curves_csv)
+
+# Read the 'all_samples.csv' file from the dataset and convert it to a pandas DataFrame
+df_samples = pd.read_csv(sd_dataset.samples_csv)
+
+# Read the 'all_papers.json' file from the dataset and convert it to a pandas DataFrame
+df_papers = pd.read_json(sd_dataset.papers_json)
 ```
 
+More details is [1_how_to_use.ipynb](example_notebooks/1_how_to_use.ipynb)
+
 ## Documentation
 
 For more detailed documentation and usage examples, please refer to the [official documentation](https://pypi.org/project/starrydata/).
 
 ## Contributing
 
 Bug reports and feature requests are welcome at the [GitHub repository](https://github.com/starrydata/starrydata-python-library/). Contributions to the codebase are also appreciated. Follow these steps to contribute:
```

### Comparing `starrydata-1.0.2/pyproject.toml` & `starrydata-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "starrydata"
-version = "1.0.2"
+version = "1.1.0"
 authors = [
   { name="MATO Tomoya", email="tomoya.matou@gmail.com" },
 ]
 description = "Starrydata Python useful tools "
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `starrydata-1.0.2/src/starrydata/dataset.py` & `starrydata-1.1.0/src/starrydata/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,39 +17,50 @@
         :param api_url: The base URL of the Figshare API.
         :param date: The date of the dataset to load in 'YYYY-MM-DD' format. If None, the latest dataset is loaded.
         """
         self.project_id = project_id
         self.api_url = api_url
         self.date = date
         self.zip_data = self._download_zip()
+        self._print_dataset_timestamp()
 
     def _fetch_article(self) -> dict:
         logging.info("Fetching dataset information.")
         if self.date:
             search_for = f"{self.date.replace('-', '')}_starrydata2"
             search_url = f"{self.api_url}/articles/search"
-            headers = {"Content-Type": "application/json"}
+            headers = {"Content-Type": "application/json", "User-Agent": "Starrydata"}
             search_body = {"project_id": self.project_id, "search_for": search_for}
             response = requests.post(search_url, headers=headers, data=json.dumps(search_body))
-            articles = response.json()
-            if not articles:
-                logging.error(
-                    f"No datasets found for the specified date: {self.date}. "
-                    "Please check the valid dates at https://figshare.com/projects/Starrydata_datasets/155129"
-                )
+
+            if response.status_code == 200:
+                articles = response.json()
+                if not articles:
+                    logging.error(
+                        f"No datasets found for the specified date: {self.date}. "
+                        "Please check the valid dates at https://figshare.com/projects/Starrydata_datasets/155129"
+                    )
+                    return None
+                logging.info(f"Found dataset for date {self.date}: {articles[0]['title']}")
+                return articles[0]
+            else:
+                logging.error(f"Failed to fetch articles. Status code: {response.status_code}, Response: {response.text}")
                 return None
-            logging.info(f"Found dataset for date {self.date}: {articles[0]['title']}")
-            return articles[0]
 
         logging.info("No specific date provided. Fetching the latest dataset.")
-        articles = requests.get(f"{self.api_url}/projects/{self.project_id}/articles").json()
-        latest_article = max(articles, key=lambda x: x['published_date'])
-        logging.info(f"Found latest dataset: {latest_article['title']}")
-        return latest_article
+        response = requests.get(f"{self.api_url}/projects/{self.project_id}/articles")
 
+        if response.status_code == 200:
+            articles = response.json()
+            latest_article = max(articles, key=lambda x: x['published_date'])
+            logging.info(f"Found latest dataset: {latest_article['title']}")
+            return latest_article
+        else:
+            logging.error(f"Failed to fetch articles. Status code: {response.status_code}, Response: {response.text}")
+            return None
 
     def _download_zip(self) -> io.BytesIO:
         logging.info("Starting the download of the ZIP file.")
         article = self._fetch_article()
         if not article:
             logging.error("Article fetch failed. Exiting download process.")
             return None
@@ -79,56 +90,63 @@
                     buffer.write(chunk)
                     progress_bar.update(len(chunk))
                     logging.debug(f"Downloaded chunk of size: {len(chunk)} bytes")
         buffer.seek(0)  # Reset buffer position to the beginning
         logging.info(f"Download complete. ZIP file '{file_name}' loaded into memory.")
         return buffer
 
-
     def _extract_file_from_zip(self, filename: str) -> io.BytesIO:
         with zipfile.ZipFile(self.zip_data, 'r') as zip_ref:
             with zip_ref.open(filename) as file:
                 return io.BytesIO(file.read())
 
     @property
-    def all_samples(self) -> io.BytesIO:
+    def samples_csv(self) -> io.BytesIO:
         """
         Extract and load the 'all_samples.csv' file from the downloaded ZIP file into a pandas DataFrame.
 
         :return: A pandas DataFrame containing the data from 'all_samples.csv'.
         """
         filename = "all_samples.csv"
         file_data = self._extract_file_from_zip(filename)
         return file_data
 
     @property
-    def all_papers(self) -> io.BytesIO:
+    def papers_json(self) -> io.BytesIO:
         """
         Extract and load the 'all_papers.json' file from the downloaded ZIP file into a pandas DataFrame.
 
         :return: A pandas DataFrame containing the data from 'all_papers.json'.
         """
         filename = "all_papers.json"
         file_data = self._extract_file_from_zip(filename)
         return file_data
 
     @property
-    def all_curves(self) -> io.BytesIO:
+    def curves_csv(self) -> io.BytesIO:
         """
         Extract and load the 'all_curves.csv' file from the downloaded ZIP file into a pandas DataFrame.
 
         :return: A pandas DataFrame containing the data from 'all_curves.csv'.
         """
         filename = "all_curves.csv"
         file_data = self._extract_file_from_zip(filename)
         return file_data
 
     @property
-    def database_snapshot(self) -> str:
+    def dataset_timestamp(self) -> str:
         """
         Extract and return the contents of the 'db_snapshot.txt' file from the downloaded ZIP file as a string.
 
         :return: A string containing the contents of 'db_snapshot.txt'.
         """
         filename = "db_snapshot.txt"
         file_data = self._extract_file_from_zip(filename)
-        return file_data.getvalue().decode('utf-8')
+        return file_data.getvalue().decode('utf-8').strip()
+
+    def _print_dataset_timestamp(self):
+        """
+        Print the dataset timestamp after downloading the dataset.
+        """
+        timestamp = self.dataset_timestamp
+        print(f"Dataset timestamp: {timestamp}")
+
```

### Comparing `starrydata-1.0.2/src/starrydata/test_dataset.py` & `starrydata-1.1.0/src/starrydata/test_dataset.py`

 * *Files identical despite different names*

### Comparing `starrydata-1.0.2/src/starrydata.egg-info/PKG-INFO` & `starrydata-1.1.0/src/starrydata.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrydata
-Version: 1.0.2
+Version: 1.1.0
 Summary: Starrydata Python useful tools 
 Author-email: MATO Tomoya <tomoya.matou@gmail.com>
 Project-URL: Homepage, https://github.com/starrydata/starrydata-python-library
 Project-URL: Issues, https://github.com/starrydata/starrydata-python-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,27 +31,35 @@
 Below is an example of how to use Starrydata.
 
 ### Downloading a Dataset
 
 To download a specific dataset, use the `Dataset` class. Here is an example of how to download and load a dataset into a pandas DataFrame:
 
 ```python
-from starrydata import Dataset
-import pandas as pd
+import starrydata as sd  # Import the Starrydata library
+import pandas as pd  # Import the pandas library
 
-# Initialize the Dataset object with a specific date
-dataset = Dataset(date="20240515")
+# Load the dataset for the specified date
+sd_dataset = sd.load_dataset(date="20240521")
 
-# Load the dataset into a pandas DataFrame
-df = pd.read_csv(dataset.all_curves)
+# Print the dataset timestamp to confirm the download date
+print(sd_dataset.dataset_timestamp)
 
-# Display the DataFrame
-print(df)
+# Read the 'all_curves.csv' file from the dataset and convert it to a pandas DataFrame
+df_curves = pd.read_csv(sd_dataset.curves_csv)
+
+# Read the 'all_samples.csv' file from the dataset and convert it to a pandas DataFrame
+df_samples = pd.read_csv(sd_dataset.samples_csv)
+
+# Read the 'all_papers.json' file from the dataset and convert it to a pandas DataFrame
+df_papers = pd.read_json(sd_dataset.papers_json)
 ```
 
+More details is [1_how_to_use.ipynb](example_notebooks/1_how_to_use.ipynb)
+
 ## Documentation
 
 For more detailed documentation and usage examples, please refer to the [official documentation](https://pypi.org/project/starrydata/).
 
 ## Contributing
 
 Bug reports and feature requests are welcome at the [GitHub repository](https://github.com/starrydata/starrydata-python-library/). Contributions to the codebase are also appreciated. Follow these steps to contribute:
```

