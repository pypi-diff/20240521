# Comparing `tmp/leitmotif-0.0.1.tar.gz` & `tmp/leitmotif-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leitmotif-0.0.1.tar", last modified: Tue Dec 19 09:39:49 2023, max compression
+gzip compressed data, was "leitmotif-0.1.0.tar", last modified: Tue May 21 09:52:47 2024, max compression
```

## Comparing `leitmotif-0.0.1.tar` & `leitmotif-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-12-19 09:39:49.445852 leitmotif-0.0.1/
--rw-r--r--   0 bzcschae   (501) staff       (20)    35149 2022-12-30 10:49:29.000000 leitmotif-0.0.1/LICENSE
--rw-r--r--   0 bzcschae   (501) staff       (20)    43233 2023-12-19 09:39:49.446004 leitmotif-0.0.1/PKG-INFO
--rw-r--r--   0 bzcschae   (501) staff       (20)     1420 2023-12-19 09:38:52.000000 leitmotif-0.0.1/README.md
-drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-12-19 09:39:49.444313 leitmotif-0.0.1/leitmotif.egg-info/
--rw-r--r--   0 bzcschae   (501) staff       (20)    43233 2023-12-19 09:39:49.000000 leitmotif-0.0.1/leitmotif.egg-info/PKG-INFO
--rw-r--r--   0 bzcschae   (501) staff       (20)      364 2023-12-19 09:39:49.000000 leitmotif-0.0.1/leitmotif.egg-info/SOURCES.txt
--rw-r--r--   0 bzcschae   (501) staff       (20)        1 2023-12-19 09:39:49.000000 leitmotif-0.0.1/leitmotif.egg-info/dependency_links.txt
--rw-r--r--   0 bzcschae   (501) staff       (20)        1 2023-12-19 09:39:49.000000 leitmotif-0.0.1/leitmotif.egg-info/not-zip-safe
--rw-r--r--   0 bzcschae   (501) staff       (20)      136 2023-12-19 09:39:49.000000 leitmotif-0.0.1/leitmotif.egg-info/requires.txt
--rw-r--r--   0 bzcschae   (501) staff       (20)       10 2023-12-19 09:39:49.000000 leitmotif-0.0.1/leitmotif.egg-info/top_level.txt
-drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-12-19 09:39:49.445254 leitmotif-0.0.1/motiflets/
--rw-r--r--   0 bzcschae   (501) staff       (20)        0 2022-03-22 11:19:31.000000 leitmotif-0.0.1/motiflets/__init__.py
--rw-r--r--   0 bzcschae   (501) staff       (20)        0 2023-12-19 09:30:28.000000 leitmotif-0.0.1/motiflets/competitors.py
--rw-r--r--   0 bzcschae   (501) staff       (20)    40444 2023-12-18 16:23:52.000000 leitmotif-0.0.1/motiflets/motiflets.py
--rw-r--r--   0 bzcschae   (501) staff       (20)    28661 2023-12-19 08:46:36.000000 leitmotif-0.0.1/motiflets/plotting.py
--rw-r--r--   0 bzcschae   (501) staff       (20)     1789 2023-12-19 09:33:03.000000 leitmotif-0.0.1/pyproject.toml
--rw-r--r--   0 bzcschae   (501) staff       (20)       79 2023-12-19 09:39:49.446222 leitmotif-0.0.1/setup.cfg
--rw-r--r--   0 bzcschae   (501) staff       (20)     1455 2022-12-31 13:49:27.000000 leitmotif-0.0.1/setup.py
-drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2023-12-19 09:39:49.445588 leitmotif-0.0.1/tests/
--rw-r--r--   0 bzcschae   (501) staff       (20)      675 2023-12-19 09:05:05.000000 leitmotif-0.0.1/tests/test_univariate.py
+drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2024-05-21 09:52:47.001646 leitmotif-0.1.0/
+-rw-r--r--   0 bzcschae   (501) staff       (20)    35149 2024-05-21 09:46:19.000000 leitmotif-0.1.0/LICENSE
+-rw-r--r--   0 bzcschae   (501) staff       (20)    46178 2024-05-21 09:52:47.001938 leitmotif-0.1.0/PKG-INFO
+-rw-r--r--   0 bzcschae   (501) staff       (20)     4347 2024-05-21 09:46:19.000000 leitmotif-0.1.0/README.md
+drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2024-05-21 09:52:46.999669 leitmotif-0.1.0/leitmotif.egg-info/
+-rw-r--r--   0 bzcschae   (501) staff       (20)    46178 2024-05-21 09:52:46.000000 leitmotif-0.1.0/leitmotif.egg-info/PKG-INFO
+-rw-r--r--   0 bzcschae   (501) staff       (20)      416 2024-05-21 09:52:46.000000 leitmotif-0.1.0/leitmotif.egg-info/SOURCES.txt
+-rw-r--r--   0 bzcschae   (501) staff       (20)        1 2024-05-21 09:52:46.000000 leitmotif-0.1.0/leitmotif.egg-info/dependency_links.txt
+-rw-r--r--   0 bzcschae   (501) staff       (20)        1 2024-05-21 09:49:36.000000 leitmotif-0.1.0/leitmotif.egg-info/not-zip-safe
+-rw-r--r--   0 bzcschae   (501) staff       (20)      136 2024-05-21 09:52:46.000000 leitmotif-0.1.0/leitmotif.egg-info/requires.txt
+-rw-r--r--   0 bzcschae   (501) staff       (20)       11 2024-05-21 09:52:46.000000 leitmotif-0.1.0/leitmotif.egg-info/top_level.txt
+drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2024-05-21 09:52:47.000598 leitmotif-0.1.0/leitmotifs/
+-rw-r--r--   0 bzcschae   (501) staff       (20)        0 2024-05-21 09:46:19.000000 leitmotif-0.1.0/leitmotifs/__init__.py
+-rw-r--r--   0 bzcschae   (501) staff       (20)     4682 2024-05-21 09:46:19.000000 leitmotif-0.1.0/leitmotifs/competitors.py
+-rw-r--r--   0 bzcschae   (501) staff       (20)    43024 2024-05-21 09:46:19.000000 leitmotif-0.1.0/leitmotifs/lama.py
+-rw-r--r--   0 bzcschae   (501) staff       (20)    31377 2024-05-21 09:46:19.000000 leitmotif-0.1.0/leitmotifs/plotting.py
+-rw-r--r--   0 bzcschae   (501) staff       (20)     1806 2024-05-21 09:52:39.000000 leitmotif-0.1.0/pyproject.toml
+-rw-r--r--   0 bzcschae   (501) staff       (20)       79 2024-05-21 09:52:47.002321 leitmotif-0.1.0/setup.cfg
+-rw-r--r--   0 bzcschae   (501) staff       (20)     1455 2024-05-21 09:46:19.000000 leitmotif-0.1.0/setup.py
+drwxr-xr-x   0 bzcschae   (501) staff       (20)        0 2024-05-21 09:52:47.001327 leitmotif-0.1.0/tests/
+-rw-r--r--   0 bzcschae   (501) staff       (20)     2150 2024-05-21 09:46:19.000000 leitmotif-0.1.0/tests/test_scalability.py
+-rw-r--r--   0 bzcschae   (501) staff       (20)     1398 2024-05-21 09:46:19.000000 leitmotif-0.1.0/tests/test_segmentation.py
+-rw-r--r--   0 bzcschae   (501) staff       (20)      653 2024-05-21 09:46:19.000000 leitmotif-0.1.0/tests/test_univariate.py
```

### Comparing `leitmotif-0.0.1/LICENSE` & `leitmotif-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `leitmotif-0.0.1/PKG-INFO` & `leitmotif-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: leitmotif
-Version: 0.0.1
+Version: 0.1.0
 Summary: Discovering Leitmotifs in Multidimensional Time Series
-Home-page: https://github.com/patrickzib/motiflets
+Home-page: https://github.com/patrickzib/leitmotifs
 Author: patrickzib
-Author-email: patrickzib <void@void.com>
+Author-email: patrickzib <patrick.schaefer@hu-berlin.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -676,15 +676,15 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: repository, https://github.com/patrickzib/motiflets
+Project-URL: repository, https://github.com/patrickzib/leitmotifs
 Keywords: multidimensional,sub-dimensional,multivariate,time-series,motif,motif-set,leitmotif,machine-learning,motif-discovery,unsupervised
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -698,72 +698,124 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Motiflets
+# Discovering Leitmotifs in Multidimensional Time Series
 
 This page was built in support of our paper "Discovering Leitmotifs in Multidimensional 
 Time Series" by Patrick Schäfer and Ulf Leser.
 
 Supporting Material
 - `tests`: Please see the python tests for use cases
 - `notebooks`: Please see the Jupyter Notebooks for use cases
 - `csvs`: The results of the scalability experiments
-- `motiflets`: Code implementing multidimensonal k-Motiflet
+- `leitmotifs`: Code implementing multidimensonal leitmotif discovery using LAMA
 - `datasets`: Use cases in the paper
 
-# k-Motiflets
+# Leitmotif Use Case
 
-TODO 
+<img src="images/leitmotifs.png" width="500">
 
-# Showcase
-
-TODO 
+A **leitmotif** (*leading motif*) is a recurring theme or motif that carries 
+symbolic significance in various forms of art, particularly literature, movies, 
+and music. The distinct feature of any leitmotif is that humans associate them to 
+meaning, which enhances narrative cohesion and establishes emotional connections 
+with the audience. The use of (leit)motifs thus eases perception, interpretation, 
+and identification with the underlying narrative. 
+A genre that often uses leitmotifs are soundtracks, for instance in the compositions of 
+Hans Zimmer or Howard Shore. The above figure shows a suite from *The Shire* with 14 
+channels arranged by Howard Shore for Lord of the Rings. The suite opens and ends with 
+the Hobbits' leitmotif, which is played by a solo tin whistle, and manifests in a 
+distinct pattern in several, but not all channels of the piece.
+
+Our LAMA (in purple) is the only method to correctly identify **4** 
+occurrences within the leitmotif using a distinctive subset of channels. 
+Other than EMD*, LAMA's occurrences show high pairwise similarity, too.
 
 # Installation
 
-The easiest is to use pip to install motiflets.
+The easiest is to use pip to install leitmotif.
 
 ## a) Install using pip
 ```
 pip install leitmotif
 ```
 
 You can also install the project from source.
 
 ## b) Build from Source
 
 First, download the repository.
 ```
-git clone https://github.com/patrickzib/motiflets.git
+git clone https://github.com/patrickzib/leitmotif.git
 ```
 
 Change into the directory and build the package from source.
 ```
 pip install .
 ```
 
 # Usage
 
-Here we illustrate how to use k-Motiflets.
+The parameters of LAMA are:
 
+- *n_dims* : Number of subdimensions to use
+- *k_max* : The largest expected number of repeats. LAMA will search from  to  for motif sets
+- *motif_length_range*
+
+LAMA has a simple OO-API.
+
+    ml = LAMA(
+        ds_name,     # Name of the dataset
+        series,      # Multidimensional time series
+        n_dims,      # Number of sub-dimensions to use
+        n_jobs,      # number of parallel jobs
+    )
+  
+LAMA has a unique feature to automatically find suitable values for the motif length  and set size  so, that meaningful Leitmotifs of an input TS can be found without domain knowledge. The methods for determining values for  and  are based on an analysis of the extent function for different .
+
+## Learning the Leitmotif length 
+
+To learn the motif length, we may simply call:
+
+    ml.fit_motif_length(
+        k_max,               # expected number of repeats
+        motif_length_range,  # motif length range
+        plot,                # Plot the results
+        plot_elbows,         # Create an elbow plot 
+        plot_motifsets,      # Plot the found motif sets
+        plot_best_only       # Plot only the motif sets of the optimal length. Otherwise plot all local optima in lengths
+    )    
+To do variable length motif discovery simply set plot_best_only=False
+
+## Learning the number of repeats
+
+To do an elbow plot, and learn the number of repeats of the motif, we may simply call:
+
+    ml.fit_k_elbow(
+        k_max,                # expected number of repeats
+        motif_length,         # motif length to use
+        plot_elbows,          # Plot the elbow plot
+        plot_motifsets        # Plot the found motif sets
+    )
+    
 # Use Cases
 
 Data Sets: We collected challenging real-life data sets to assess the quality and 
-scalability of MD algorithms. An overview of datasets can be found in Table 2 
+scalability of the algorithm. An overview of datasets can be found in Table 2 
 of our paper. 
 
-TODO
+- Jupyter-Notebooks for finding subdimensional Leitmotif in multidimensional time series
+<a href="notebooks/use_cases_paper.ipynb">Multivariate Use Case</a>:
+highlights a use case used in the paper, and shows the unique ability 
+to learn its parameters from the data and find interesting motif sets.
 
-- Jupyter-Notebook 
-<a href="notebooks/use_cases_paper.ipynb">Univariate Use Cases for k-Motiflets</a>:
-highlights all use cases used in the paper and shows the unique ability of k-Motiflets 
-to learn its parameters from the data and find itneresting motif sets.
+- All other use cases can be found in the <a href="tests">test folder</a>
 
 
 ## Citation
 If you use this work, please cite as:
 
 TODO
```

### Comparing `leitmotif-0.0.1/leitmotif.egg-info/PKG-INFO` & `leitmotif-0.1.0/leitmotif.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: leitmotif
-Version: 0.0.1
+Version: 0.1.0
 Summary: Discovering Leitmotifs in Multidimensional Time Series
-Home-page: https://github.com/patrickzib/motiflets
+Home-page: https://github.com/patrickzib/leitmotifs
 Author: patrickzib
-Author-email: patrickzib <void@void.com>
+Author-email: patrickzib <patrick.schaefer@hu-berlin.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -676,15 +676,15 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: repository, https://github.com/patrickzib/motiflets
+Project-URL: repository, https://github.com/patrickzib/leitmotifs
 Keywords: multidimensional,sub-dimensional,multivariate,time-series,motif,motif-set,leitmotif,machine-learning,motif-discovery,unsupervised
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -698,72 +698,124 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Motiflets
+# Discovering Leitmotifs in Multidimensional Time Series
 
 This page was built in support of our paper "Discovering Leitmotifs in Multidimensional 
 Time Series" by Patrick Schäfer and Ulf Leser.
 
 Supporting Material
 - `tests`: Please see the python tests for use cases
 - `notebooks`: Please see the Jupyter Notebooks for use cases
 - `csvs`: The results of the scalability experiments
-- `motiflets`: Code implementing multidimensonal k-Motiflet
+- `leitmotifs`: Code implementing multidimensonal leitmotif discovery using LAMA
 - `datasets`: Use cases in the paper
 
-# k-Motiflets
+# Leitmotif Use Case
 
-TODO 
+<img src="images/leitmotifs.png" width="500">
 
-# Showcase
-
-TODO 
+A **leitmotif** (*leading motif*) is a recurring theme or motif that carries 
+symbolic significance in various forms of art, particularly literature, movies, 
+and music. The distinct feature of any leitmotif is that humans associate them to 
+meaning, which enhances narrative cohesion and establishes emotional connections 
+with the audience. The use of (leit)motifs thus eases perception, interpretation, 
+and identification with the underlying narrative. 
+A genre that often uses leitmotifs are soundtracks, for instance in the compositions of 
+Hans Zimmer or Howard Shore. The above figure shows a suite from *The Shire* with 14 
+channels arranged by Howard Shore for Lord of the Rings. The suite opens and ends with 
+the Hobbits' leitmotif, which is played by a solo tin whistle, and manifests in a 
+distinct pattern in several, but not all channels of the piece.
+
+Our LAMA (in purple) is the only method to correctly identify **4** 
+occurrences within the leitmotif using a distinctive subset of channels. 
+Other than EMD*, LAMA's occurrences show high pairwise similarity, too.
 
 # Installation
 
-The easiest is to use pip to install motiflets.
+The easiest is to use pip to install leitmotif.
 
 ## a) Install using pip
 ```
 pip install leitmotif
 ```
 
 You can also install the project from source.
 
 ## b) Build from Source
 
 First, download the repository.
 ```
-git clone https://github.com/patrickzib/motiflets.git
+git clone https://github.com/patrickzib/leitmotif.git
 ```
 
 Change into the directory and build the package from source.
 ```
 pip install .
 ```
 
 # Usage
 
-Here we illustrate how to use k-Motiflets.
+The parameters of LAMA are:
 
+- *n_dims* : Number of subdimensions to use
+- *k_max* : The largest expected number of repeats. LAMA will search from  to  for motif sets
+- *motif_length_range*
+
+LAMA has a simple OO-API.
+
+    ml = LAMA(
+        ds_name,     # Name of the dataset
+        series,      # Multidimensional time series
+        n_dims,      # Number of sub-dimensions to use
+        n_jobs,      # number of parallel jobs
+    )
+  
+LAMA has a unique feature to automatically find suitable values for the motif length  and set size  so, that meaningful Leitmotifs of an input TS can be found without domain knowledge. The methods for determining values for  and  are based on an analysis of the extent function for different .
+
+## Learning the Leitmotif length 
+
+To learn the motif length, we may simply call:
+
+    ml.fit_motif_length(
+        k_max,               # expected number of repeats
+        motif_length_range,  # motif length range
+        plot,                # Plot the results
+        plot_elbows,         # Create an elbow plot 
+        plot_motifsets,      # Plot the found motif sets
+        plot_best_only       # Plot only the motif sets of the optimal length. Otherwise plot all local optima in lengths
+    )    
+To do variable length motif discovery simply set plot_best_only=False
+
+## Learning the number of repeats
+
+To do an elbow plot, and learn the number of repeats of the motif, we may simply call:
+
+    ml.fit_k_elbow(
+        k_max,                # expected number of repeats
+        motif_length,         # motif length to use
+        plot_elbows,          # Plot the elbow plot
+        plot_motifsets        # Plot the found motif sets
+    )
+    
 # Use Cases
 
 Data Sets: We collected challenging real-life data sets to assess the quality and 
-scalability of MD algorithms. An overview of datasets can be found in Table 2 
+scalability of the algorithm. An overview of datasets can be found in Table 2 
 of our paper. 
 
-TODO
+- Jupyter-Notebooks for finding subdimensional Leitmotif in multidimensional time series
+<a href="notebooks/use_cases_paper.ipynb">Multivariate Use Case</a>:
+highlights a use case used in the paper, and shows the unique ability 
+to learn its parameters from the data and find interesting motif sets.
 
-- Jupyter-Notebook 
-<a href="notebooks/use_cases_paper.ipynb">Univariate Use Cases for k-Motiflets</a>:
-highlights all use cases used in the paper and shows the unique ability of k-Motiflets 
-to learn its parameters from the data and find itneresting motif sets.
+- All other use cases can be found in the <a href="tests">test folder</a>
 
 
 ## Citation
 If you use this work, please cite as:
 
 TODO
```

### Comparing `leitmotif-0.0.1/motiflets/motiflets.py` & `leitmotif-0.1.0/leitmotifs/lama.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
-"""Compute k-Motiflets.
+"""Compute leitmotifs using LAMA.
 
 
 """
 
 __author__ = ["patrickzib"]
 
 from ast import literal_eval
 from os.path import exists
+import os
 
 import numpy as np
 import numpy.fft as fft
 import pandas as pd
 from numba import njit, prange, objmode, types
 from numba.typed import Dict, List
 from scipy.signal import argrelextrema
@@ -60,26 +61,40 @@
 
     Returns
     -------
     Series : pd.Series
         A series of ground-truth data
 
     """
-    file = '../datasets/ground_truth/' + dataset.split(".")[0] + "_gt.csv"
+    file = os.path.splitext(dataset)[0] + "_gt.csv"
     if exists(file):
         print(file)
         series = pd.read_csv(file, index_col=0)
 
         for i in range(0, series.shape[0]):
             series.iloc[i] = series.iloc[i].apply(literal_eval)
 
         return series
     return None
 
 
+def read_audio_from_dataframe(pandas_file_url, channels=None):
+    """Reads a time series with an index (e.g. time) from a CSV with MFCC features."""
+
+    df = pd.read_csv(pandas_file_url, index_col=0, compression='gzip')
+    audio_length_seconds = 2 * float(df.columns[-1]) - float(df.columns[-2])
+
+    if channels:
+        df = df.loc[channels]
+
+    ground_truth = read_ground_truth(pandas_file_url)
+
+    return audio_length_seconds, df, np.float64(df.columns), ground_truth
+
+
 def read_dataset_with_index(dataset, sampling_factor=10000):
     """Reads a time series with an index (e.g. time) and resamples.
 
     Parameters
     ----------
     dataset : String
         File location.
@@ -138,15 +153,15 @@
         data_index = data.index
     elif isinstance(data, pd.DataFrame):
         data_raw = data.values
         data_index = data.columns
     else:
         data_raw = data
         data_index = np.arange(data.shape[-1])
-    return data_index, data_raw.astype(np.float64, copy=False)
+    return data_index.astype(np.float64), data_raw.astype(np.float64, copy=False)
 
 
 def read_dataset(dataset, sampling_factor=10000):
     """ Reads a dataset and resamples.
 
     Parameters
     ----------
@@ -255,14 +270,15 @@
 
 
 @njit(fastmath=True, cache=True, parallel=True)
 def compute_distance_matrix(time_series,
                             m,
                             k,
                             exclude_trivial_match=True,
+                            compute_knns=True,
                             n_jobs=4,
                             slack=0.5,
                             sum_dims=True):
     """ Compute the full Distance Matrix between all pairs of subsequences of a
         multivariate time series.
 
         Computes pairwise distances between n-m+1 subsequences, of length, extracted
@@ -304,18 +320,25 @@
     halve_m = 0
     if exclude_trivial_match:
         halve_m = int(m * slack)
 
     # Sum all dimensions into one row
     if sum_dims:
         D_all = np.zeros((1, n, n), dtype=np.float32)
-        knns = np.zeros((1, n, k), dtype=np.int32)
+        if compute_knns:
+            knns = np.zeros((1, n, k), dtype=np.int32)
+        else:
+            knns = np.zeros((dims, 1, 1), dtype=np.int32)
     else:
         D_all = np.zeros((dims, n, n), dtype=np.float32)
-        knns = np.zeros((dims, n, k), dtype=np.int32)
+
+        if compute_knns:
+            knns = np.zeros((dims, n, k), dtype=np.int32)
+        else:
+            knns = np.zeros((dims, 1, 1), dtype=np.int32)
 
     bin_size = time_series.shape[-1] // n_jobs
     # lower_bounds = np.zeros(n_jobs)
     # lower_bounds[:] = np.inf
 
     for idx in prange(n_jobs):
         start = idx * bin_size
@@ -341,26 +364,30 @@
                 dist = distance(dot_rolled, n, m, means, stds, order, halve_m)
                 if sum_dims:
                     D_all[0, order] += dist
                 else:
                     D_all[d, order] = dist
                 dot_prev = dot_rolled
 
-        # do not merge with previous loop, as we are adding distances
-        # over dimensions, first
-        for d in np.arange(D_all.shape[0]):
-            for order in np.arange(start, end):
-                knn = _argknn(D_all[d, order], k, m, slack=slack)
-
-                knns[d, order, :len(knn)] = knn
-                knns[d, order, len(knn):] = -1
+        if sum_dims:
+            D_all = D_all / dims
 
-                # if len(knn) == k:
-                #    lower_bounds[idx] = min(lower_bounds[idx],
-                #                            4 * D_all[d, order, knn[-1]])
+        if compute_knns:
+            # do not merge with previous loop, as we are adding distances
+            # over dimensions, first
+            for d in np.arange(D_all.shape[0]):
+                for order in np.arange(start, end):
+                    knn = _argknn(D_all[d, order], k, m, slack=slack)
+
+                    knns[d, order, :len(knn)] = knn
+                    knns[d, order, len(knn):] = -1
+
+                    # if len(knn) == k:
+                    #    lower_bounds[idx] = min(lower_bounds[idx],
+                    #                            4 * D_all[d, order, knn[-1]])
 
     return D_all, knns
 
 
 @njit(fastmath=True, cache=True, parallel=True)
 def compute_distance_matrix_sparse(time_series,
                                    m,
@@ -463,14 +490,15 @@
     #        for i in range(len(dist_knn)):
     #            lowest_distance[i] = min(lowest_distance[i], dist_knn[i])
 
     # 2*r is the maximal distance between two subsequences
     # lowest_distance = 4 * lowest_distance * dims  # FIXME: depends on worst dimension
 
     # Parallelizm does not work, as Dict is not thread safe :(
+    # FIXME : given a large number of dimensions, the memory usage explodes
     for d in np.arange(dims):
         for order in np.arange(0, n):
             for ks in knns[d, order]:  # needed to compute the k-nn distances
                 D_bool[order][ks] = True
 
         for order in np.arange(0, n):
             # all pairs only needed when lower bound is given
@@ -528,40 +556,40 @@
     dist[order] = 0
 
     return dist
 
 
 @njit(fastmath=True, cache=True)
 def get_radius(D_full, motifset_pos):
-    """Computes the radius of the passed motif set (motiflet).
+    """Computes the radius of the passed motif set (leitmotif).
 
     Parameters
     ----------
     D_full : 2d array-like
         The distance matrix
     motifset_pos : array-like
         The motif set start-offsets
 
     Returns
     -------
-    motiflet_radius : float
+    leitmotif_radius : float
         The radius of the motif set
     """
-    motiflet_radius = np.inf
+    leitmotif_radius = np.inf
 
     for ii in range(len(motifset_pos) - 1):
         i = motifset_pos[ii]
         current = np.float32(0.0)
         for jj in range(1, len(motifset_pos)):
             if (i != jj):
                 j = motifset_pos[jj]
                 current = max(current, D_full[i, j])
-        motiflet_radius = min(current, motiflet_radius)
+        leitmotif_radius = min(current, leitmotif_radius)
 
-    return motiflet_radius
+    return leitmotif_radius
 
 
 @njit(fastmath=True, cache=True)
 def get_pairwise_extent(D_full, motifset_pos, dim_index, upperbound=np.inf):
     """Computes the extent of the motifset.
 
     Parameters
@@ -667,73 +695,78 @@
         else:
             break
 
     return np.array(idx, dtype=np.int32)
 
 
 @njit(fastmath=True, cache=True)
-def get_approximate_k_motiflet(
+def run_LAMA(
         ts, m, k, D, knns, dim_index, upper_bound=np.inf
 ):
-    """Compute the approximate k-Motiflets.
+    """Compute the approximate leitmotif using LAMA.
 
-    Details are given within the paper Section 4.2 Approximate k-Motiflet Algorithm.
+    Details are given within the paper Section 3.3
+    LAtent leitMotif discovery Algorithm (LAMA).
 
     Parameters
     ----------
     ts : array-like
         The raw time seres
     m : int
         The motif length
     k : int
-        The k in k-Motiflets
+        The size k of the leitmotif
     D : 2d array-like
         The distance matrix
     upper_bound : float
         Used for admissible pruning
 
     Returns
     -------
     Tuple
-        motiflet_candidate : np.array
-            The (approximate) best motiflet found
-        motiflet_dist:
-            The extent of the motiflet found
+        leitmotif_candidate : np.array
+            The (approximate) best leitmotif found
+        leitmotif_dist:
+            The extent of the leitmotif found
     """
     n = ts.shape[-1] - m + 1
-    motiflet_dist = upper_bound
-    motiflet_dims = None
-    motiflet_candidate = None
+    leitmotif_dist = upper_bound
+    leitmotif_dims = None
+    leitmotif_candidate = None
 
     for order in np.arange(n, dtype=np.int32):
+        # for dim in np.arange(ts.shape[0], dtype=np.int32):
+        # knn_idx = knns[dim_index[order, dim], order]
+
         # Use the first (best) dimension for ordering of k-NNs
         knn_idx = knns[dim_index[order, 0], order]
         if np.any(knn_idx[:k] == -1):
             continue
 
         # sum over the knns from the best dimensions
+        # TODO
         knn_distance = 0.0
         for a in np.arange(dim_index.shape[-1]):  # dimensions
             knn_distance += D[dim_index[order, a]][order][knn_idx[k - 1]]
 
         if len(knn_idx) >= k and knn_idx[k - 1] >= 0:
-            if knn_distance <= motiflet_dist:
-                motiflet_extent = get_pairwise_extent(
+            if knn_distance <= leitmotif_dist:
+                extent = get_pairwise_extent(
                     D,
                     knn_idx[:k],
                     dim_index,
-                    motiflet_dist
+                    leitmotif_dist
                 )
-                if motiflet_extent <= motiflet_dist:
-                    motiflet_dist = motiflet_extent
-                    motiflet_candidate = knn_idx[:k]
-                    motiflet_dims = dim_index[order]
+                if extent <= leitmotif_dist:
+                    leitmotif_dist = extent
+                    leitmotif_candidate = knn_idx[:k]
+                    leitmotif_dims = dim_index[order]
 
-    # print("best dims", m, k, motiflet_dims)
-    return motiflet_candidate, motiflet_dist, motiflet_dims
+    # print("best dims", m, k, leitmotif_dims)
+    return leitmotif_candidate, leitmotif_dist, leitmotif_dims
 
 
 @njit(fastmath=True, cache=True)
 def _check_unique(motifset_1, motifset_2, motif_length):
     """Check for overlaps between two motif sets.
 
     Two motif sets overlapp, if more than m/2 subsequences overlap from motifset 1.
@@ -748,16 +781,16 @@
         The length of the motif. Overlap exists, if 25% of two subsequences overlap.
 
     Returns
     -------
     True, if there are at least m/2 subsequences with an overlap of 25%, else False.
     """
     count = 0
-    for a in motifset_1:  # smaller motiflet
-        for b in motifset_2:  # larger motiflet
+    for a in motifset_1:  # smaller leitmotif
+        for b in motifset_2:  # larger leitmotif
             if abs(a - b) < (motif_length / 4):
                 count = count + 1
                 break
 
         if count >= len(motifset_1) / 2:
             return False
     return True
@@ -858,14 +891,15 @@
 
 
 def select_subdimensions(
         data,
         k_max,
         motif_length,
         dim_range,
+        minimize_pairwise_dist=False,
         n_jobs=4,
         elbow_deviation=1.00,
         slack=0.5):
     """Findes the optimal number of dimensions
 
     Parameters
     ----------
@@ -894,37 +928,38 @@
             The minumum found
         all_minima : array-like
             All local minima found
         au_efs : array-like
             For each length in the interval, the AU_EF.
         elbows :
             Largest k (largest elbow) found
-        top_motiflets :
-            The motiflet for the largest k for each length.
+        top_leitmotifs :
+            The leitmotif for the largest k for each length.
 
     """
     # in reverse order
     all_dist = np.zeros(len(dim_range), dtype=object)
     all_candidates = np.zeros(len(dim_range), dtype=object)
     all_candidate_dims = np.zeros(len(dim_range), dtype=object)
     all_elbow_points = np.zeros(len(dim_range), dtype=object)
 
     D_full = None
     knns = None
     for i, n_dims in enumerate(dim_range):
         if n_dims <= data.shape[0]:
             dist, candidates, candidate_dims, elbow_points, D_full, knns \
-                = search_k_motiflets_elbow(
+                = search_leitmotifs_elbow(
                 k_max,
                 data,
                 motif_length,
                 n_dims=n_dims,
                 elbow_deviation=elbow_deviation,
                 slack=slack,
                 return_distances=True,
+                minimize_pairwise_dist=minimize_pairwise_dist,
                 D_full=D_full,
                 knns=knns,  # reuse distances from last runs
                 n_jobs=n_jobs
             )
 
             elbow_points = _filter_unique(elbow_points, candidates, motif_length)
 
@@ -940,14 +975,15 @@
 
 
 def find_au_ef_motif_length(
         data,
         k_max,
         motif_length_range,
         n_dims=None,
+        minimize_pairwise_dist=False,
         n_jobs=4,
         elbow_deviation=1.00,
         slack=0.5,
         subsample=2):
     """Computes the Area under the Elbow-Function within an of motif lengths.
 
     Parameters
@@ -977,43 +1013,44 @@
             The minumum found
         all_minima : array-like
             All local minima found
         au_efs : array-like
             For each length in the interval, the AU_EF.
         elbows :
             Largest k (largest elbow) found
-        top_motiflets :
-            The motiflet for the largest k for each length.
+        top_leitmotifs :
+            The leitmotif for the largest k for each length.
 
     """
     # apply sampling for speedup only
     if subsample > 1:
         if data.ndim >= 2:
             data = data[:, ::subsample]
         else:
             data = data[::subsample]
 
     # in reverse order
     au_efs = np.zeros(len(motif_length_range), dtype=object)
     au_efs.fill(np.inf)
     elbows = np.zeros(len(motif_length_range), dtype=object)
-    top_motiflets = np.zeros(len(motif_length_range), dtype=object)
-    top_motiflets_dims = np.zeros(len(motif_length_range), dtype=object)
+    top_leitmotifs = np.zeros(len(motif_length_range), dtype=object)
+    top_leitmotifs_dims = np.zeros(len(motif_length_range), dtype=object)
     dists = np.zeros(len(motif_length_range), dtype=object)
 
     # TODO parallelize?
     for i, m in enumerate(motif_length_range[::-1]):
         if m // subsample < data.shape[-1]:
-            dist, candidates, candidate_dims, elbow_points, _ = search_k_motiflets_elbow(
+            dist, candidates, candidate_dims, elbow_points, _ = search_leitmotifs_elbow(
                 k_max,
                 data,
                 m // subsample,
                 n_dims=n_dims,
                 n_jobs=n_jobs,
                 elbow_deviation=elbow_deviation,
+                minimize_pairwise_dist=minimize_pairwise_dist,
                 slack=slack)
 
             dists_ = dist[(~np.isinf(dist)) & (~np.isnan(dist))]
             # dists_ = dists_[:min(elbow_points[-1] + 1, len(dists_))]
             if dists_.max() - dists_.min() == 0:
                 au_efs[i] = 1.0
             else:
@@ -1021,62 +1058,63 @@
                         dists_.max() - dists_.min())).sum()
                              / len(dists_))
 
             elbow_points = _filter_unique(elbow_points, candidates, m // subsample)
 
             if len(elbow_points > 0):
                 elbows[i] = elbow_points
-                top_motiflets[i] = candidates[elbow_points]
-                top_motiflets_dims[i] = candidate_dims[elbow_points]
+                top_leitmotifs[i] = candidates[elbow_points]
+                top_leitmotifs_dims[i] = candidate_dims[elbow_points]
             else:
                 # we found only the pair motif
                 elbows[i] = [2]
-                top_motiflets[i] = [candidates[2]]
-                top_motiflets_dims[i] = candidate_dims[candidates[2]]
+                top_leitmotifs[i] = [candidates[2]]
+                top_leitmotifs_dims[i] = candidate_dims[candidates[2]]
 
                 # no elbow can be found, ignore this part
                 au_efs[i] = 1.0
 
             dists[i] = dist
 
     # reverse order
     au_efs = np.array(au_efs, dtype=np.float64)[::-1]
     elbows = elbows[::-1]
     dists = dists[::-1]
-    top_motiflets = top_motiflets[::-1] * subsample
-    top_motiflets_dims = top_motiflets_dims[::-1]
+    top_leitmotifs = top_leitmotifs[::-1] * subsample
+    top_leitmotifs_dims = top_leitmotifs_dims[::-1]
 
     # Minima in AU_EF
     minimum = motif_length_range[np.nanargmin(au_efs)]
     au_ef_minima = argrelextrema(au_efs, np.less_equal, order=subsample)
 
     # Maxima in the EF
     return (minimum,
             au_ef_minima, au_efs,
             elbows,
-            top_motiflets, top_motiflets_dims,
+            top_leitmotifs, top_leitmotifs_dims,
             dists)
 
 
-def search_k_motiflets_elbow(
+def search_leitmotifs_elbow(
         k_max,
         data,
         motif_length,
         n_dims=None,
         elbow_deviation=1.00,
         filter=True,
         slack=0.5,
         return_distances=False,
         D_full=None,
         knns=None,
+        minimize_pairwise_dist=False,
         n_jobs=4,
 ):
     """Computes the elbow-function.
 
-    This is the method to find the characteristic k-Motiflets within range
+    This is the method to find the characteristic leitmotifs within range
     [2...k_max] for given a `motif_length` using elbow-plots.
 
     Details are given within the paper Section 5.1 Learning meaningful k.
 
     Parameters
     ----------
     k_max : int
@@ -1088,15 +1126,15 @@
     n_dims : int
         the number of dimensions to use for subdimensional motif discovery
     elbow_deviation : float, default=1.00
         The minimal absolute deviation needed to detect an elbow.
         It measures the absolute change in deviation from k to k+1.
         1.05 corresponds to 5% increase in deviation.
     filter: bool, default=True
-        filters overlapping motiflets from the result,
+        filters overlapping leitmotif from the result,
     slack: float
         Defines an exclusion zone around each subsequence to avoid trivial matches.
         Defined as percentage of m. E.g. 0.5 is equal to half the window length.
     n_jobs : int
         Number of jobs to be used.
 
 
@@ -1125,127 +1163,160 @@
     # Check if use_dim is smaller than all given dimensions
     n_dims = d if n_dims is None else n_dims
     sum_dims = True if n_dims >= d else False
 
     # switch to sparse matrix representation when length is above 30_000
     # sparse matrix is 2x slower but needs less memory
     sparse_gb = ((n ** 2) * d) * 32 / (1024 ** 3) / 8
-    sparse = sparse_gb > 4.0
+    sparse = sparse_gb > 8.0
 
     # compute the distance matrix
     if D_full is None:
-        if sparse:
-            print("sparse")
+        if minimize_pairwise_dist: # FIXME: find better name
+            # this has the drawback, that each pair of subsequences may
+            # have different smallest dimensions
+
+            print("Sort along dimension axis", flush=True)
+            D_full, _ = compute_distance_matrix(
+                data_raw, m, k_max_,
+                compute_knns=False,
+                n_jobs=n_jobs,
+                slack=slack,
+                sum_dims=False)
+
+            D_full = np.sort(D_full, axis=0)[:n_dims].sum(axis=0, dtype=np.float32)
+            knns = _argknns(D_full, k_max_, m, n, slack)
+
+            D_full = D_full.reshape(1, D_full.shape[0], D_full.shape[1])
+            knns = knns.reshape(1, knns.shape[0], knns.shape[1])
+        elif sparse:
+            print("Using Sparse Backend", flush=True)
             D_knns, D_full, knns = compute_distance_matrix_sparse(
                 data_raw, m, k_max_,
                 n_jobs=n_jobs,
                 slack=slack)
         else:
+            print("Using Default Backend", flush=True)
             D_full, knns = compute_distance_matrix(
                 data_raw, m, k_max_,
                 n_jobs=n_jobs,
                 slack=slack,
                 sum_dims=sum_dims)
 
     # non-overlapping motifs only
-    k_motiflet_distances = np.zeros(k_max_ + 1)
-    k_motiflet_candidates = np.empty(k_max_ + 1, dtype=object)
-    k_motiflet_dims = np.empty(k_max_ + 1, dtype=object)
+    k_leitmotif_distances = np.zeros(k_max_ + 1)
+    k_leitmotif_candidates = np.empty(k_max_ + 1, dtype=object)
+    k_leitmotif_dims = np.empty(k_max_ + 1, dtype=object)
 
     # order dimensions by increasing distance
     use_dim = min(n_dims, len(D_full))  # dimensions indexed by 0
 
     upper_bound = np.inf
     for test_k in tqdm(range(k_max_, 1, -1),
                        desc='Compute ks (' + str(k_max_) + ")",
                        position=0, leave=False):
 
-        if not sum_dims:
+        if minimize_pairwise_dist or sum_dims:
+            # Do nothing
+            dim_index = np.zeros((n, 1), dtype=np.int32)
+        elif not sum_dims:
             # k-th NN and it's distance along all dimensions
             knn_idx = knns[:, :, test_k - 1]
             if isinstance(D_full, List) or isinstance(D_full, list):
                 D_knn = take_along_axis(D_full, d, knn_idx, n)
             else:
                 D_knn = np.take_along_axis(
                     D_full,
                     knn_idx.reshape((knn_idx.shape[0], knn_idx.shape[1], 1)),
                     axis=2)[:, :, 0]
 
             dim_index = np.argsort(D_knn, axis=0)[:use_dim]
             dim_index = np.transpose(dim_index, (1, 0))
-        else:
-            dim_index = np.zeros((n, 1), dtype=np.int32)
 
-        candidate, candidate_dist, candidate_dims = get_approximate_k_motiflet(
+        candidate, candidate_dist, candidate_dims = run_LAMA(
             data_raw, m, test_k, D_full, knns, dim_index,
             upper_bound=upper_bound,
         )
 
-        k_motiflet_distances[test_k] = candidate_dist
-        k_motiflet_candidates[test_k] = candidate
+        k_leitmotif_distances[test_k] = candidate_dist
+        k_leitmotif_candidates[test_k] = candidate
 
-        if not sum_dims:
-            k_motiflet_dims[test_k] = candidate_dims
-        else:
-            k_motiflet_dims[test_k] = np.arange(d)
+        if minimize_pairwise_dist or sum_dims:
+            k_leitmotif_dims[test_k] = np.arange(d)
+        elif not sum_dims:
+            k_leitmotif_dims[test_k] = candidate_dims
 
         # compute a new upper bound
-        upper_bound = min(candidate_dist, upper_bound)
+        # if candidate is not None:
+        #    dist_new = get_pairwise_extent(D_full, candidate[:test_k])
+        #    upper_bound = min(upper_bound, dist_new)
+        # FIXME: upper_bound = min(candidate_dist, upper_bound)
 
     # smoothen the line to make it monotonically increasing
-    k_motiflet_distances[0:2] = k_motiflet_distances[2]
-    for i in range(len(k_motiflet_distances), 2):
-        k_motiflet_distances[i - 1] = min(k_motiflet_distances[i],
-                                          k_motiflet_distances[i - 1])
+    k_leitmotif_distances[0:2] = k_leitmotif_distances[2]
+    for i in range(len(k_leitmotif_distances), 2):
+        k_leitmotif_distances[i - 1] = min(k_leitmotif_distances[i],
+                                          k_leitmotif_distances[i - 1])
 
-    elbow_points = find_elbow_points(k_motiflet_distances,
+    elbow_points = find_elbow_points(k_leitmotif_distances,
                                      elbow_deviation=elbow_deviation)
 
     if filter:
         elbow_points = _filter_unique(
-            elbow_points, k_motiflet_candidates, motif_length)
+            elbow_points, k_leitmotif_candidates, motif_length)
 
     if return_distances:
-        return (k_motiflet_distances, k_motiflet_candidates, k_motiflet_dims,
+        return (k_leitmotif_distances, k_leitmotif_candidates, k_leitmotif_dims,
                 elbow_points, D_full, knns)
     else:
-        return (k_motiflet_distances, k_motiflet_candidates, k_motiflet_dims,
+        return (k_leitmotif_distances, k_leitmotif_candidates, k_leitmotif_dims,
                 elbow_points, m)
 
 
+@njit(fastmath=True, cache=True)
+def _argknns(D_full, k_max_, m, n, slack):
+    # compute knns from new distance matrix
+    knns = np.zeros((n, k_max_), dtype=np.int32)
+    for order in range(0, D_full.shape[0]):
+        knn = _argknn(D_full[order], k_max_, m, slack=slack)
+        knns[order, :len(knn)] = knn
+        knns[order, len(knn):] = -1
+
+    return knns
+
+
 @njit(fastmath=True, cache=True, parallel=True)
 def take_along_axis(D_full, d, knn_idx, n):
     D_knn = np.zeros((d, n), dtype=np.float32)
     for i in prange(d):
         for j in prange(n):
             D_knn[i, j] = D_full[i][j][knn_idx[i, j]]
     return D_knn
 
 
 @njit(fastmath=True, cache=True)
 def candidate_dist(D_full, pool, upperbound, m, slack=0.5):
-    motiflet_candidate_dist = 0
+    leitmotif_candidate_dist = 0
     m_half = int(m * slack)
     for i in pool:
         for j in pool:
             if ((i != j and np.abs(i - j) < m_half)
                     or (i != j and D_full[i, j] > upperbound)):
                 return np.inf
 
     for i in pool:
         for j in pool:
-            motiflet_candidate_dist = max(motiflet_candidate_dist, D_full[i, j])
+            leitmotif_candidate_dist = max(leitmotif_candidate_dist, D_full[i, j])
 
-    return motiflet_candidate_dist
+    return leitmotif_candidate_dist
 
 
-@njit(fastmath=True, cache=True, parallel=True)
+# @njit(fastmath=True, cache=True, parallel=True)
 def compute_distances_full_univ(ts, m, exclude_trivial_match=True, n_jobs=4, slack=0.5):
     """Compute the full Distance Matrix between all pairs of subsequences.
-        # TODO only used for backwards compability
 
         Computes pairwise distances between n-m+1 subsequences, of length, extracted
         from the time series, of length n.
 
         Z-normed ED is used for distances.
 
         This implementation is in O(n^2) by using the sliding dot-product.
@@ -1266,15 +1337,15 @@
 
         Returns
         -------
         D : 2d array-like
             The O(n^2) z-normed ED distances between all pairs of subsequences
 
     """
-    D, _ = compute_distance_matrix(ts,
-                                   m,
-                                   1,
-                                   exclude_trivial_match=exclude_trivial_match,
-                                   n_jobs=n_jobs,
-                                   slack=slack,
-                                   sum_dims=True)
-    return D[0]
+    return compute_distance_matrix(
+        ts,
+        m,
+        1,
+        exclude_trivial_match=exclude_trivial_match,
+        n_jobs=n_jobs,
+        slack=slack,
+        sum_dims=True)[0]
```

### Comparing `leitmotif-0.0.1/motiflets/plotting.py` & `leitmotif-0.1.0/leitmotifs/plotting.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,56 +11,58 @@
 import pandas as pd
 import seaborn as sns
 from matplotlib import pyplot as plt
 from matplotlib.patches import Rectangle
 from matplotlib.ticker import MaxNLocator
 from scipy.stats import zscore
 
-import motiflets.motiflets as ml
+import leitmotifs.lama as ml
 
 matplotlib.rcParams['pdf.fonttype'] = 42
 matplotlib.rcParams['ps.fonttype'] = 42
 
 
-class Motiflets:
+class LAMA:
 
     def __init__(
             self,
             ds_name,
             series,
+            minimize_pairwise_dist=False,
             ground_truth=None,
             dimension_labels=None,
             elbow_deviation=1.00,
             n_dims=None,
             n_jobs=4,
             slack=0.5,
     ):
         self.ds_name = ds_name
         self.series = convert_to_2d(series)
 
         self.elbow_deviation = elbow_deviation
         self.slack = slack
         self.dimension_labels = dimension_labels
         self.ground_truth = ground_truth
+        self.minimize_pairwise_dist = minimize_pairwise_dist
 
         self.motif_length_range = None
         self.motif_length = 0
         self.all_extrema = []
         self.all_elbows = []
-        self.all_top_motiflets = []
+        self.all_top_leitmotifs = []
         self.all_dists = []
 
         self.n_dims = n_dims
         self.n_jobs = n_jobs
         self.motif_length = 0
         self.k_max = 0
         self.dists = []
-        self.motiflets = []
+        self.leitmotifs = []
         self.elbow_points = []
-        self.motiflets_dims = []
+        self.leitmotif_dims = []
         self.all_dimensions = []
 
     def fit_motif_length(
             self,
             k_max,
             motif_length_range,
             subsample=1,
@@ -70,84 +72,88 @@
             plot_best_only=True
     ):
         self.motif_length_range = motif_length_range
         self.k_max = k_max
 
         (self.motif_length,
          self.dists,
-         self.motiflets,
-         self.motiflets_dims,
+         self.leitmotifs,
+         self.leitmotif_dims,
          self.elbow_points,
          self.all_elbows,
-         self.all_top_motiflets,
+         self.all_top_leitmotifs,
          self.all_dists,
          self.all_dimensions,
          self.all_extrema) = plot_motif_length_selection(
             k_max,
             self.series,
             motif_length_range,
             self.ds_name,
             n_dims=self.n_dims,
+            minimize_pairwise_dist=self.minimize_pairwise_dist,
             n_jobs=self.n_jobs,
             elbow_deviation=self.elbow_deviation,
             slack=self.slack,
             subsample=subsample,
             plot_elbows=plot_elbows,
-            plot_motifs=plot_motifsets,
+            plot_motif=plot_motifsets,
+            ground_truth=self.ground_truth,
             plot=plot,
             plot_best_only=plot_best_only)
 
         return self.motif_length, self.all_extrema
 
     def fit_k_elbow(
             self,
             k_max,
             motif_length=None,  # if None, use best_motif_length
             filter_duplicates=True,
             plot_elbows=True,
-            plot_motifs_as_grid=True,
+            plot_motifsets=True,
     ):
         self.k_max = k_max
 
         if motif_length is None:
             motif_length = self.motif_length
         else:
             self.motif_length = motif_length
 
-        self.dists, self.motiflets, self.motiflets_dims, self.elbow_points = plot_elbow(
+        self.dists, self.leitmotifs, self.leitmotif_dims, self.elbow_points = plot_elbow(
             k_max,
             self.series,
             n_dims=self.n_dims,
             ds_name=self.ds_name,
             motif_length=motif_length,
             plot_elbows=plot_elbows,
-            plot_grid=plot_motifs_as_grid,
+            plot_motif=plot_motifsets,
             ground_truth=self.ground_truth,
             dimension_labels=self.dimension_labels,
             filter=filter_duplicates,
+            minimize_pairwise_dist=self.minimize_pairwise_dist,
             n_jobs=self.n_jobs,
             elbow_deviation=self.elbow_deviation,
             slack=self.slack
         )
 
-        return self.dists, self.motiflets, self.elbow_points
+        return self.dists, self.leitmotifs, self.elbow_points
 
     def fit_dimensions(
             self,
             k_max,
             motif_length,
             dim_range
     ):
 
         all_dist, all_candidates, all_candidate_dims, all_elbow_points \
             = ml.select_subdimensions(
             self.series,
             k_max=k_max,
             motif_length=motif_length,
             dim_range=dim_range,
+            minimize_pairwise_dist=self.minimize_pairwise_dist,
             n_jobs=self.n_jobs,
             elbow_deviation=self.elbow_deviation,
             slack=self.slack,
         )
 
         fig, ax = plt.subplots(figsize=(10, 4))
         ax.set_title("Dimension Plot")
@@ -164,32 +170,37 @@
 
         if path is not None:
             plt.savefig(path)
             plt.show()
 
         return fig, ax
 
-    def plot_motifset(self, elbow_points=None, path=None):
+    def plot_motifset(self, elbow_points=None, path=None, motifset_name=None):
 
-        if self.dists is None or self.motiflets is None or self.elbow_points is None:
+        if self.dists is None or self.leitmotifs is None or self.elbow_points is None:
             raise Exception("Please call fit_k_elbow first.")
 
         if elbow_points is None:
             elbow_points = self.elbow_points
 
         # TODO
         # if elbow_point is None:
         #    elbow_point = self.elbow_points[-1]
+        motifset_names = None
+        if motifset_name is not None:
+            motifset_names = [motifset_name for _ in range(len(self.elbow_points))]
 
         fig, ax = plot_motifsets(
             self.ds_name,
             self.series,
-            motifsets=self.motiflets[elbow_points],
-            motiflet_dims=self.motiflets_dims[elbow_points],
+            motifsets=self.leitmotifs[elbow_points],
+            leitmotif_dims=self.leitmotif_dims[elbow_points],
+            motifset_names=motifset_names,
             dist=self.dists[elbow_points],
+            ground_truth=self.ground_truth,
             motif_length=self.motif_length,
             show=path is None)
 
         if path is not None:
             plt.savefig(path)
             plt.show()
 
@@ -205,14 +216,15 @@
             series = np.arange(series.shape[-1])
     if series.shape[0] > series.shape[1]:
         raise ('Warning: The input shape is wrong. Dimensions should be on rows. '
                'Try transposing the input.')
 
     return series
 
+
 def as_series(data, index_range, index_name):
     """Coverts a time series to a series with an index.
 
     Parameters
     ----------
     data : array-like
         The time series raw data as numpy array
@@ -256,17 +268,18 @@
 
 def plot_motifsets(
         ds_name,
         data,
         motifsets=None,
         motifset_names=None,
         dist=None,
-        motiflet_dims=None,
+        leitmotif_dims=None,
         motif_length=None,
         ground_truth=None,
+        font_size=26,
         show=True):
     """Plots the data and the found motif sets.
 
     Parameters
     ----------
     ds_name: String,
         The name of the time series
@@ -280,155 +293,228 @@
         The length of the motif
     ground_truth: pd.Series
         Ground-truth information as pd.Series.
     show: boolean
         Outputs the plot
 
     """
+    # set_sns_style(font_size)
+    # sns.set(font_scale=3)
+    sns.set(font="Calibri")
+    sns.set_style("white")
+
     # turn into 2d array
     data = convert_to_2d(data)
 
     if motifsets is not None:
         git_ratio = [4]
         for _ in range(len(motifsets)):
             git_ratio.append(1)
 
         fig, axes = plt.subplots(2, 1 + len(motifsets),
                                  sharey="row",
                                  sharex=False,
                                  figsize=(
-                                     10 + 2 * len(motifsets), 5 + data.shape[0] // 2),
+                                     10 + 2 * len(motifsets),
+                                     5 + (data.shape[0] + len(motifsets)) // 2),
                                  squeeze=False,
                                  gridspec_kw={
                                      'width_ratios': git_ratio,
+                                     'height_ratios': [10, 3]})  # 5 for rolling stone?
+    elif ground_truth is not None:
+        fig, axes = plt.subplots(2, 1,
+                                 sharey="row",
+                                 sharex=False,
+                                 figsize=(20, 5 + data.shape[0] // 2),
+                                 squeeze=False,
+                                 gridspec_kw={
+                                     'width_ratios': [4],
                                      'height_ratios': [10, 1]})
     else:
         fig, axes = plt.subplots(1, 1, squeeze=False,
-                                 figsize=(20, 3 + data.shape[0] // 3))
+                                 figsize=(20, 5 + data.shape[0] // 2))
 
     if ground_truth is None:
         ground_truth = []
 
     data_index, data_raw = ml.pd_series_to_numpy(data)
 
+    color_offset = 1
     offset = 0
     tick_offsets = []
-    axes[0, 0].set_title(ds_name, fontsize=20)
+    axes[0, 0].set_title(ds_name, fontsize=22)
 
     for dim in range(data_raw.shape[0]):
         dim_data_raw = zscore(data_raw[dim])
         offset -= 1.2 * (np.max(dim_data_raw) - np.min(dim_data_raw))
         tick_offsets.append(offset)
 
         _ = sns.lineplot(x=data_index,
                          y=dim_data_raw + offset,
                          ax=axes[0, 0],
-                         linewidth=1,
-                         color=sns.color_palette("tab10")[0],
-                         ci=None,
+                         linewidth=0.5,
+                         # color=sns.color_palette("tab10")[0],
+                         color="gray",
+                         errorbar=("ci", None),
                          estimator=None
                          )
         sns.despine()
 
         if motifsets is not None:
             for i, motifset in enumerate(motifsets):
-                if (motiflet_dims is None or
-                        (motiflet_dims[i] is not None and dim in motiflet_dims[i])):
+                if (leitmotif_dims is None or
+                        (leitmotif_dims[i] is not None and dim in leitmotif_dims[i])):
                     if motifset is not None:
                         for a, pos in enumerate(motifset):
-                            _ = sns.lineplot(ax=axes[0, 0],
-                                             x=data_index[
-                                                 np.arange(pos, pos + motif_length)],
-                                             y=dim_data_raw[
-                                               pos:pos + motif_length] + offset,
-                                             linewidth=2,
-                                             color=sns.color_palette("tab10")[2 + i],
-                                             ci=None,
-                                             estimator=None)
+                            # Do not plot, if all dimensions are covered
+                            if leitmotif_dims is None or leitmotif_dims[i].shape[0] < \
+                                    data.shape[0]:
+                                _ = sns.lineplot(ax=axes[0, 0],
+                                                 x=data_index[
+                                                     np.arange(pos,
+                                                               pos + motif_length)],
+                                                 y=dim_data_raw[
+                                                   pos:pos + motif_length] + offset,
+                                                 linewidth=3,
+                                                 color=sns.color_palette("tab10")[
+                                                     (color_offset + i) % len(
+                                                         sns.color_palette("tab10"))],
+                                                 errorbar=("ci", None),
+                                                 # alpha=0.9,
+                                                 estimator=None)
 
                             axes[0, 1 + i].set_title(
                                 (("Motif Set " + str(i + 1)) if motifset_names is None
-                                 else motifset_names[i]) + "\n" +
+                                 else motifset_names[i%len(motifset_names)]) + "\n" +
                                 "k=" + str(len(motifset)) +
                                 # ", d=" + str(np.round(dist[i], 2)) +
                                 ", l=" + str(motif_length),
-                                fontsize=16)
+                                fontsize=18)
 
                             df = pd.DataFrame()
                             df["time"] = range(0, motif_length)
 
                             for aa, pos in enumerate(motifset):
-                                df[str(aa)] = zscore(
-                                    dim_data_raw[pos:pos + motif_length]) + offset
+                                values = dim_data_raw[pos:pos + motif_length]
+                                df[str(aa)] = (values - values.mean()) / (
+                                            values.std() + 1e-4) + offset
 
                             df_melt = pd.melt(df, id_vars="time")
-                            _ = sns.lineplot(ax=axes[0, 1 + i],
-                                             data=df_melt,
-                                             ci=99,
-                                             n_boot=10,
-                                             lw=1,
-                                             color=sns.color_palette("tab10")[2 + i],
-                                             x="time",
-                                             y="value")
-
-        for aaa, column in enumerate(ground_truth):
-            for offsets in ground_truth[column]:
-                for pos, off in enumerate(offsets):
-                    if pos == 0:
-                        sns.lineplot(x=data_index[off[0]: off[1]],
-                                     y=dim_data_raw[off[0]:off[1]] + offset,
-                                     label=column,
-                                     color=sns.color_palette("tab10")[(aaa + 1) % 10],
-                                     ax=axes[0, 0],
-                                     ci=None, estimator=None
-                                     )
-                    else:
-                        sns.lineplot(x=data_index[off[0]: off[1]],
-                                     y=dim_data_raw[off[0]:off[1]] + offset,
-                                     color=sns.color_palette("tab10")[(aaa + 1) % 10],
-                                     ax=axes[0, 0],
-                                     ci=None, estimator=None
-                                     )
+                            _ = sns.lineplot(
+                                ax=axes[0, 1 + i],
+                                data=df_melt,
+                                errorbar=("ci", 99),
+                                n_boot=10,
+                                lw=1,
+                                color=sns.color_palette("tab10")[
+                                    (color_offset + i) % len(
+                                        sns.color_palette("tab10"))],
+                                x="time",
+                                y="value")
+
+        # for aaa, column in enumerate(ground_truth):
+        #     for offsets in ground_truth[column]:
+        #         for pos, off in enumerate(offsets):
+        #             if pos == 0 and dim == 0:
+        #                 # Plot label only once
+        #                 sns.lineplot(x=data_index[off[0]: off[1]],
+        #                              y=dim_data_raw[off[0]:off[1]] + offset,
+        #                              label=column,
+        #                              alpha=0.5,
+        #                              color=sns.color_palette("tab10")[(aaa-1) % 10],
+        #                              ax=axes[0, 0],
+        #                              errorbar=("ci", None),
+        #                              estimator=None
+        #                              )
+        #             else:
+        #                 sns.lineplot(x=data_index[off[0]: off[1]],
+        #                              y=dim_data_raw[off[0]:off[1]] + offset,
+        #                              color=sns.color_palette("tab10")[(aaa-1) % 10],
+        #                              alpha=0.5,
+        #                              ax=axes[0, 0],
+        #                              errorbar=("ci", None),
+        #                              estimator=None
+        #                              )
+
+    gt_count = 0
+    y_labels = []
+    motif_set_count = 0 if motifsets is None else len(motifsets)
+
+    for aaa, column in enumerate(ground_truth):
+        for offsets in ground_truth[column]:
+            for off in offsets:
+                ratio = 0.8
+                start = off[0]
+                end = off[1]
+                rect = Rectangle(
+                    (data_index[start], 0),
+                    data_index[end - 1] - data_index[start],
+                    ratio,
+                    facecolor=sns.color_palette("tab10")[
+                        (color_offset + motif_set_count + aaa) %
+                        len(sns.color_palette("tab10"))],
+                    alpha=0.7
+                )
+
+                rx, ry = rect.get_xy()
+                cx = rx + rect.get_width() / 2.0
+                cy = ry + rect.get_height() / 2.0
+                axes[1, 0].annotate(column, (cx, cy),
+                                    color='black',
+                                    weight='bold',
+                                    fontsize=12,
+                                    ha='center', va='center')
+
+                axes[1, 0].add_patch(rect)
+    if ground_truth is not None and len(ground_truth) > 0:
+        gt_count = 1
+        y_labels.append("Ground Truth")
 
     if motifsets is not None:
-        y_labels = []
-        for i, motiflet in enumerate(motifsets):
-            if motiflet is not None:
-                for aa, pos in enumerate(motiflet):
+        for i, leitmotif in enumerate(motifsets):
+            if leitmotif is not None:
+                for pos in leitmotif:
                     ratio = 0.8
                     rect = Rectangle(
-                        (data_index[pos], -i),
+                        (data_index[pos], -i - gt_count),
                         data_index[pos + motif_length - 1] - data_index[pos],
                         ratio,
-                        facecolor=sns.color_palette("tab10")[2 + i],
+                        facecolor=sns.color_palette("tab10")[
+                            (color_offset + i) % len(sns.color_palette("tab10"))],
                         alpha=0.7
                     )
                     axes[1, 0].add_patch(rect)
 
-                y_labels.append("Motif Set" + str(i))
-
-        axes[1, 0].set_yticks(-np.arange(len(motifsets)) + 1.5)
-        axes[1, 0].set_yticklabels([], fontsize=12)
-        axes[1, 0].set_ylim([-abs(len(motifsets)) + 1, 1])
+                label = (("Motif Set " + str(i + 1)) if motifset_names is None
+                         else motifset_names[i % len(motifset_names)])
+                y_labels.append(label)
+
+    if len(y_labels) > 0:
+        axes[1, 0].set_yticks(-np.arange(len(y_labels)) + 0.5)
+        axes[1, 0].set_yticklabels(y_labels, fontsize=18)
+        axes[1, 0].set_ylim([-abs(len(y_labels)) + 1, 1])
         axes[1, 0].set_xlim(axes[0, 0].get_xlim())
-        axes[1, 0].set_title("Position of Motifsets", fontsize=20)
+
+        if motifsets is not None:
+            axes[1, 0].set_title("Positions", fontsize=22)
 
         for i in range(1, axes.shape[-1]):
             axes[1, i].remove()
 
     if isinstance(data, pd.DataFrame):
         axes[0, 0].set_yticks(tick_offsets)
-        axes[0, 0].set_yticklabels(data.index, fontsize=12)
+        axes[0, 0].set_yticklabels(data.index, fontsize=18)
 
         if motifsets is not None:
             axes[0, 1].set_yticks(tick_offsets)
-            axes[0, 1].set_yticklabels(data.index, fontsize=12)
+            axes[0, 1].set_yticklabels(data.index, fontsize=18)
 
     sns.despine()
     fig.tight_layout()
+
     if show:
         plt.show()
 
     return fig, axes
 
 
 def _plot_elbow_points(
@@ -468,78 +554,45 @@
     ax.plot(range(2, len(np.sqrt(dists))), dists[2:], "b", label="Extent")
 
     lim1 = plt.ylim()[0]
     lim2 = plt.ylim()[1]
     for elbow in elbow_points:
         ax.vlines(
             elbow, lim1, lim2,
-            linestyles="--", label=str(elbow) + "-Motiflet"
+            linestyles="--", label=str(elbow) + "-Leitmotif"
         )
     ax.set(xlabel='Size (k)', ylabel='Extent')
     ax.xaxis.set_major_locator(MaxNLocator(integer=True))
     plt.scatter(elbow_points, dists[elbow_points], color="red", label="Minima")
 
-    motiflets = motifset_candidates[elbow_points]
-    for i, motiflet in enumerate(motiflets):
-        if motiflet is not None:
-            if elbow_points[i] - 3 < 0:
-                x_pos = 0
-            else:
-                x_pos = (elbow_points[i] - 2) / (len(motifset_candidates))
-
-            scale = max(dists) - min(dists)
-            # y_pos = (dists[elbow_points[i]] - min(dists) + scale * 0.15) / scale
-            axins = ax.inset_axes(
-                [x_pos, 0.1, 0.2, 0.15])
-
-            df = pd.DataFrame()
-            df["time"] = data_index[range(0, motif_length)]
-
-            for dim in range(data_raw.shape[0]):
-                if (motifset_candidates_dims is None or
-                        dim == motifset_candidates_dims[elbow_points][0][0]):
-                    pos = motiflet[0]
-                    normed_data = zscore(data_raw[dim, pos:pos + motif_length])
-                    df["dim_" + str(dim)] = normed_data
-
-            df_melt = pd.melt(df, id_vars="time")
-            _ = sns.lineplot(ax=axins, data=df_melt,
-                             x="time", y="value",
-                             hue="variable",
-                             style="variable",
-                             ci=99,
-                             # alpha=0.8,
-                             n_boot=10, color=sns.color_palette("tab10")[(i + 1) % 10])
-            axins.set_xlabel("")
-            axins.patch.set_alpha(0)
-            axins.set_ylabel("")
-            axins.xaxis.set_major_formatter(plt.NullFormatter())
-            axins.yaxis.set_major_formatter(plt.NullFormatter())
-            axins.legend().set_visible(False)
+    leitmotifs = motifset_candidates[elbow_points]
 
     plt.tight_layout()
+    plt.savefig("lord_of_the_rings_elbow_points.pdf")
     plt.show()
 
 
+
 def plot_elbow(k_max,
                data,
                ds_name,
                motif_length,
                n_dims=2,
                plot_elbows=False,
-               plot_grid=True,
+               plot_motif=True,
                ground_truth=None,
                dimension_labels=None,
+               minimize_pairwise_dist=False,
                filter=True,
                n_jobs=4,
                elbow_deviation=1.00,
                slack=0.5):
-    """Plots the elbow-plot for k-Motiflets.
+    """Plots the elbow-plot for leitmotifs.
 
-    This is the method to find and plot the characteristic k-Motiflets within range
+    This is the method to find and plot the characteristic leitmotifs within range
     [2...k_max] for given a `motif_length` using elbow-plots.
 
     Details are given within the paper Section 5.1 Learning meaningful k.
 
     Parameters
     ----------
     k_max: int
@@ -550,22 +603,22 @@
         the name of the dataset
     motif_length: int
         the length of the motif (user parameter)
     n_dims : int
         the number of dimensions to use for subdimensional motif discovery
     plot_elbows: bool, default=False
         plots the elbow ploints into the plot
-    plot_grid: bool, default=True
+    plot_motif: bool, default=True
         The motifs along the time series
     ground_truth: pd.Series
         Ground-truth information as pd.Series.
     dimension_labels:
         Labels for the dimensions
     filter: bool, default=True
-        filters overlapping motiflets from the result,
+        filters overlapping leitmotifs from the result,
     n_jobs : int
         Number of jobs to be used.
     elbow_deviation : float, default=1.00
         The minimal absolute deviation needed to detect an elbow.
         It measures the absolute change in deviation from k to k+1.
         1.05 corresponds to 5% increase in deviation.
     slack : float
@@ -587,44 +640,45 @@
         elif isinstance(data, (np.ndarray, np.generic)):
             data = np.arange(data.shape[-1])
 
     _, raw_data = ml.pd_series_to_numpy(data)
     print("Data", raw_data.shape)
 
     startTime = time.perf_counter()
-    dists, candidates, candidate_dims, elbow_points, m = ml.search_k_motiflets_elbow(
+    dists, candidates, candidate_dims, elbow_points, m = ml.search_leitmotifs_elbow(
         k_max,
         raw_data,
         motif_length,
         n_dims=n_dims,
         elbow_deviation=elbow_deviation,
         filter=filter,
         n_jobs=n_jobs,
+        minimize_pairwise_dist=minimize_pairwise_dist,
         slack=slack)
     endTime = (time.perf_counter() - startTime)
 
     print("Chosen window-size:", m, "in", np.round(endTime, 1), "s")
     print("Elbow Points", elbow_points)
 
     if plot_elbows:
         _plot_elbow_points(
             ds_name, data, motif_length, elbow_points,
             candidates, dists, motifset_candidates_dims=candidate_dims)
 
-    if plot_grid:
+    if plot_motif:
         plot_motifsets(
             ds_name,
             data,
             motifsets=candidates[elbow_points],
-            motiflet_dims=candidate_dims[elbow_points],
+            leitmotif_dims=candidate_dims[elbow_points],
             dist=dists,
             motif_length=motif_length,
             show=True)
 
-        # plot_grid_motiflets(
+        # plot_grid_leitmotifs(
         #    ds_name, data, candidates, elbow_points,
         #    dists, motif_length, show_elbows=False,
         #    candidates_dims=candidate_dims,
         #    font_size=24,
         #    ground_truth=ground_truth,
         #    dimension_labels=dimension_labels)
 
@@ -634,18 +688,20 @@
 def plot_motif_length_selection(
         k_max, data, motif_length_range, ds_name,
         n_jobs=4,
         elbow_deviation=1.00,
         slack=0.5,
         subsample=2,
         n_dims=2,
+        minimize_pairwise_dist=False,
+        ground_truth=None,
         plot=True,
         plot_best_only=True,
         plot_elbows=True,
-        plot_motifs=True,
+        plot_motif=True,
 ):
     """Computes the AU_EF plot to extract the best motif lengths
 
     This is the method to find and plot the characteristic motif-lengths, for k in
     [2...k_max], using the area AU-EF plot.
 
     Details are given within the paper 5.2 Learning Motif Length l.
@@ -688,84 +744,86 @@
 
     # discretizes ranges
     motif_length_range = np.int32(motif_length_range)
 
     startTime = time.perf_counter()
     (best_motif_length,
      all_minima, au_ef,
-     elbow, top_motiflets,
-     top_motiflets_dims, dists) = \
+     elbow, top_leitmotifs,
+     top_leitmotifs_dims, dists) = \
         ml.find_au_ef_motif_length(
             data_raw, k_max,
             n_dims=n_dims,
             motif_length_range=motif_length_range,
+            minimize_pairwise_dist=minimize_pairwise_dist,
             n_jobs=n_jobs,
             elbow_deviation=elbow_deviation,
             slack=slack,
             subsample=subsample)
     endTime = (time.perf_counter() - startTime)
     print("\tTime", np.round(endTime, 1), "s")
 
     all_minima = _filter_duplicate_window_sizes(au_ef, all_minima)
 
     if plot:
         _plot_window_lengths(
             all_minima, au_ef, data_raw, ds_name, elbow, header, index,
-            motif_length_range, top_motiflets,
-            top_motiflets_dims=top_motiflets_dims)
+            motif_length_range, top_leitmotifs,
+            top_leitmotifs_dims=top_leitmotifs_dims)
 
-        if plot_elbows or plot_motifs:
+        if plot_elbows or plot_motifsets:
             to_plot = all_minima[0]
             if plot_best_only:
                 to_plot = [np.argmin(au_ef)]
 
             for a in to_plot:
                 motif_length = motif_length_range[a]
                 candidates = np.zeros(len(dists[a]), dtype=object)
-                candidates[elbow[a]] = top_motiflets[a]  # need to unpack
+                candidates[elbow[a]] = top_leitmotifs[a]  # need to unpack
 
                 candidate_dims = np.zeros(len(dists[a]), dtype=object)
-                candidate_dims[elbow[a]] = top_motiflets_dims[a]  # need to unpack
+                candidate_dims[elbow[a]] = top_leitmotifs_dims[a]  # need to unpack
 
                 elbow_points = elbow[a]
 
                 if plot_elbows:
                     _plot_elbow_points(
                         ds_name, data, motif_length,
                         elbow_points, candidates, dists[a],
                         motifset_candidates_dims=candidate_dims)
 
-                if plot_motifs:
+                if plot_motif:
                     plot_motifsets(
                         ds_name,
                         data,
-                        motifsets=top_motiflets[a],
-                        motiflet_dims=top_motiflets_dims[a],
+                        motifsets=top_leitmotifs[a],
+                        leitmotif_dims=top_leitmotifs_dims[a],
                         dist=dists[a][elbow_points],
                         motif_length=motif_length,
+                        ground_truth=ground_truth,
                         show=True)
 
     best_pos = np.argmin(au_ef)
     best_elbows = elbow[best_pos]
     best_dist = dists[best_pos]
-    best_motiflets = np.zeros(len(dists[best_pos]), dtype=object)
-    best_motiflets[elbow[best_pos]] = top_motiflets[best_pos]  # need to unpack
-    best_motiflets_dims = np.zeros(len(dists[best_pos]), dtype=object)
-    best_motiflets_dims[elbow[best_pos]] = top_motiflets_dims[
+    best_leitmotifs = np.zeros(len(dists[best_pos]), dtype=object)
+    best_leitmotifs[elbow[best_pos]] = top_leitmotifs[best_pos]  # need to unpack
+    best_leitmotifs_dims = np.zeros(len(dists[best_pos]), dtype=object)
+    best_leitmotifs_dims[elbow[best_pos]] = top_leitmotifs_dims[
         best_pos]  # need to unpack
 
     return (best_motif_length,
             best_dist,
-            best_motiflets,
-            best_motiflets_dims,
+            best_leitmotifs,
+            best_leitmotifs_dims,
             best_elbows,
             elbow,
-            top_motiflets,
+            top_leitmotifs,
             dists,
-            top_motiflets_dims,
+            top_leitmotifs_dims,
             all_minima[0])
 
 
 def _filter_duplicate_window_sizes(au_ef, minima):
     """Filter neighboring window sizes with equal minima
     """
     filtered = []
@@ -781,82 +839,81 @@
     return [np.array(filtered)]
 
 
 def _plot_window_lengths(
         all_minima, au_ef, data_raw, ds_name,
         elbow, header, index,
         motif_length_range,
-        top_motiflets,
-        top_motiflets_dims=None,
-        font_size=20):
-    set_sns_style(font_size)
+        top_leitmotifs,
+        top_leitmotifs_dims=None):
+    # set_sns_style(font_size)
 
     indices = ~np.isinf(au_ef)
-    fig, ax = plt.subplots(figsize=(10, 3),
+    fig, ax = plt.subplots(figsize=(10, 4),
                            constrained_layout=True
                            )
     sns.lineplot(
         # x=index[motif_length_range[indices]],  # TODO!!!
         x=motif_length_range[indices],
         y=au_ef[indices],
         label="AU_EF",
-        ci=None, estimator=None,
+        errorbar=("ci", None), estimator=None,
         ax=ax)
     sns.despine()
-    ax.set_title("Best lengths on " + ds_name, size=20)
+    ax.set_title("Best lengths on " + ds_name, size=14)
     ax.set(xlabel='Motif Length' + header, ylabel='Area under EF\n(lower is better)')
     ax.scatter(  # index[motif_length_range[all_minima]],   # TODO!!!
         motif_length_range[all_minima],
         au_ef[all_minima], color="red",
         label="Minima")
     for item in ([ax.xaxis.label, ax.yaxis.label] +
                  ax.get_xticklabels() + ax.get_yticklabels()):
-        item.set_fontsize(16)
+        item.set_fontsize(12)
     # turn into 2d array
     if data_raw.ndim == 1:
         data_raw = data_raw.reshape((1, -1))
     # iterate all minima
     for i, minimum in enumerate(all_minima[0]):
-        # iterate all motiflets
-        for a, motiflet_pos in enumerate(top_motiflets[minimum]):
+        # iterate all leitmotifs
+        for a, leitmotif_pos in enumerate(top_leitmotifs[minimum]):
             x_pos = minimum / len(motif_length_range)
             scale = max(au_ef) - min(au_ef)
             y_pos = (au_ef[minimum] - min(au_ef) + (1.5 * a + 1) * scale * 0.15) / scale
             axins = ax.inset_axes([x_pos, y_pos, 0.20, 0.15])
 
             motif_length = motif_length_range[minimum]
             df = pd.DataFrame()
             df["time"] = index[range(0, motif_length)]
 
             for dim in range(data_raw.shape[0]):
-                if top_motiflets_dims is None or dim == top_motiflets_dims[minimum][0][
+                if top_leitmotifs_dims is None or dim == top_leitmotifs_dims[minimum][0][
                     0]:
-                    pos = motiflet_pos[0]
+                    pos = leitmotif_pos[0]
                     normed_data = zscore(data_raw[dim, pos:pos + motif_length])
                     df["dim_" + str(dim)] = normed_data
 
             df_melt = pd.melt(df, id_vars="time")
             _ = sns.lineplot(ax=axins, data=df_melt,
                              x="time", y="value",
                              hue="variable",
                              style="variable",
-                             ci=99,
+                             errorbar=("ci", 99),
                              n_boot=10,
                              lw=1,
                              color=sns.color_palette("tab10")[(i + 1) % 10])
             axins.set_xlabel("")
             axins.patch.set_alpha(0)
             axins.set_ylabel("")
             axins.xaxis.set_major_formatter(plt.NullFormatter())
             axins.yaxis.set_major_formatter(plt.NullFormatter())
             axins.legend().set_visible(False)
-    fig.set_figheight(5)
-    fig.set_figwidth(8)
+    # fig.set_figheight(5)
+    # fig.set_figwidth(8)
     plt.tight_layout()
-    # plt.savefig("window_length.pdf")
+    plt.savefig("lord_of_the_rings_window_length.pdf")
     plt.show()
 
 
 def set_sns_style(font_size):
     sns.set(font_scale=2)
     sns.set_style("white")
     sns.set_context("paper",
```

### Comparing `leitmotif-0.0.1/pyproject.toml` & `leitmotif-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "leitmotif"
 
-version = "0.0.1"
+version = "0.1.0"
 
 description = "Discovering Leitmotifs in Multidimensional Time Series"
 readme = "README.md"
 authors = [
-    {name = "patrickzib", email = "void@void.com"}
+    {name = "patrickzib", email = "patrick.schaefer@hu-berlin.de"}
 ]
 keywords = [
     "multidimensional",
     "sub-dimensional",
     "multivariate",
     "time-series",
     "motif",
@@ -48,15 +48,15 @@
     "scipy<2.0.0",
     "seaborn>=0.11.2",
     "tqdm>=4.63.0",
     "matplotlib>=3.5.1",
 ]
 
 [project.urls]
-repository = "https://github.com/patrickzib/motiflets"
+repository = "https://github.com/patrickzib/leitmotifs"
 #documentation = ""
 #download = ""
 
 [project.license]
 file = "LICENSE"
 
 [build-system]
```

### Comparing `leitmotif-0.0.1/setup.py` & `leitmotif-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `leitmotif-0.0.1/tests/test_univariate.py` & `leitmotif-0.1.0/tests/test_univariate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from motiflets.motiflets import *
-from motiflets.plotting import *
+from leitmotifs.lama import *
+from leitmotifs.plotting import *
 
 matplotlib.rcParams['pdf.fonttype'] = 42
 matplotlib.rcParams['ps.fonttype'] = 42
 
 import warnings
 
 warnings.simplefilter("ignore")
@@ -12,17 +12,17 @@
 
 mpl.rcParams['figure.dpi'] = 150
 
 
 def test_univariate():
     file = 'ecg-heartbeat-av.csv'
     ds_name = "ECG Heartbeat"
-    series, df_gt = read_dataset_with_index(file)
+    series = read_dataset_with_index(file)
 
-    ml = Motiflets(ds_name, series, df_gt)
+    ml = LAMA(ds_name, series)
     ml.plot_dataset()
 
     ks = 20
     length_range = np.arange(25, 200, 25)
     ml.fit_motif_length(ks, length_range)
     print("Best motif length", series.index[ml.motif_length], "seconds")
```

