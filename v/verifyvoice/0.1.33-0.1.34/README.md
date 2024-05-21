# Comparing `tmp/verifyvoice-0.1.33.tar.gz` & `tmp/verifyvoice-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verifyvoice-0.1.33.tar", last modified: Mon May 20 18:36:12 2024, max compression
+gzip compressed data, was "verifyvoice-0.1.34.tar", last modified: Tue May 21 02:48:27 2024, max compression
```

## Comparing `verifyvoice-0.1.33.tar` & `verifyvoice-0.1.34.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 thejan    (1000) thejan    (1000)        0 2024-05-20 18:36:12.816205 verifyvoice-0.1.33/
--rw-r--r--   0 thejan    (1000) thejan    (1000)     3752 2024-05-20 18:36:12.816205 verifyvoice-0.1.33/PKG-INFO
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     2901 2024-05-20 18:35:17.000000 verifyvoice-0.1.33/README.md
--rw-rw-r--   0 thejan    (1000) thejan    (1000)       38 2024-05-20 18:36:12.816205 verifyvoice-0.1.33/setup.cfg
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     1369 2024-05-20 18:35:35.000000 verifyvoice-0.1.33/setup.py
-drwxrwxr-x   0 thejan    (1000) thejan    (1000)        0 2024-05-20 18:36:12.812205 verifyvoice-0.1.33/verifyvoice/
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     3667 2024-05-20 18:35:17.000000 verifyvoice-0.1.33/verifyvoice/DataLoader.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     4943 2024-05-20 18:35:17.000000 verifyvoice-0.1.33/verifyvoice/ModelLoader.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)      719 2024-05-20 18:35:17.000000 verifyvoice-0.1.33/verifyvoice/Similarity.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     2765 2024-05-20 18:35:17.000000 verifyvoice-0.1.33/verifyvoice/SpeakerNet.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     3656 2024-05-20 18:35:17.000000 verifyvoice-0.1.33/verifyvoice/Spk_Encoder.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)    28893 2024-05-20 18:35:17.000000 verifyvoice-0.1.33/verifyvoice/WavLM.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)      106 2024-05-20 18:35:17.000000 verifyvoice-0.1.33/verifyvoice/__init__.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     2082 2024-05-20 18:35:17.000000 verifyvoice-0.1.33/verifyvoice/aamsoftmax.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     1330 2024-05-20 18:35:17.000000 verifyvoice-0.1.33/verifyvoice/deepInfoMaxLoss.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     1935 2024-05-20 18:35:17.000000 verifyvoice-0.1.33/verifyvoice/mine.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     2760 2024-05-20 18:35:17.000000 verifyvoice-0.1.33/verifyvoice/model_args.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)    31946 2024-05-20 18:35:17.000000 verifyvoice-0.1.33/verifyvoice/modules.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     1285 2024-05-20 18:35:17.000000 verifyvoice-0.1.33/verifyvoice/utils.py
-drwxrwxr-x   0 thejan    (1000) thejan    (1000)        0 2024-05-20 18:36:12.816205 verifyvoice-0.1.33/verifyvoice.egg-info/
--rw-r--r--   0 thejan    (1000) thejan    (1000)     3752 2024-05-20 18:36:12.000000 verifyvoice-0.1.33/verifyvoice.egg-info/PKG-INFO
--rw-rw-r--   0 thejan    (1000) thejan    (1000)      516 2024-05-20 18:36:12.000000 verifyvoice-0.1.33/verifyvoice.egg-info/SOURCES.txt
--rw-rw-r--   0 thejan    (1000) thejan    (1000)        1 2024-05-20 18:36:12.000000 verifyvoice-0.1.33/verifyvoice.egg-info/dependency_links.txt
--rw-rw-r--   0 thejan    (1000) thejan    (1000)       55 2024-05-20 18:36:12.000000 verifyvoice-0.1.33/verifyvoice.egg-info/requires.txt
--rw-rw-r--   0 thejan    (1000) thejan    (1000)       12 2024-05-20 18:36:12.000000 verifyvoice-0.1.33/verifyvoice.egg-info/top_level.txt
+drwxrwxr-x   0 thejan    (1000) thejan    (1000)        0 2024-05-21 02:48:27.226250 verifyvoice-0.1.34/
+-rw-r--r--   0 thejan    (1000) thejan    (1000)     3752 2024-05-21 02:48:27.226250 verifyvoice-0.1.34/PKG-INFO
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     2901 2024-05-20 18:35:17.000000 verifyvoice-0.1.34/README.md
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)       38 2024-05-21 02:48:27.226250 verifyvoice-0.1.34/setup.cfg
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     1369 2024-05-21 02:47:43.000000 verifyvoice-0.1.34/setup.py
+drwxrwxr-x   0 thejan    (1000) thejan    (1000)        0 2024-05-21 02:48:27.222250 verifyvoice-0.1.34/verifyvoice/
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     3667 2024-05-21 02:47:58.000000 verifyvoice-0.1.34/verifyvoice/DataLoader.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     4942 2024-05-21 02:47:27.000000 verifyvoice-0.1.34/verifyvoice/ModelLoader.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)      719 2024-05-20 18:35:17.000000 verifyvoice-0.1.34/verifyvoice/Similarity.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     2765 2024-05-20 18:35:17.000000 verifyvoice-0.1.34/verifyvoice/SpeakerNet.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     3656 2024-05-20 18:35:17.000000 verifyvoice-0.1.34/verifyvoice/Spk_Encoder.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)    28893 2024-05-20 18:35:17.000000 verifyvoice-0.1.34/verifyvoice/WavLM.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)      106 2024-05-20 18:35:17.000000 verifyvoice-0.1.34/verifyvoice/__init__.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     2082 2024-05-20 18:35:17.000000 verifyvoice-0.1.34/verifyvoice/aamsoftmax.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     1330 2024-05-20 18:35:17.000000 verifyvoice-0.1.34/verifyvoice/deepInfoMaxLoss.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     1935 2024-05-20 18:35:17.000000 verifyvoice-0.1.34/verifyvoice/mine.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     2760 2024-05-20 18:35:17.000000 verifyvoice-0.1.34/verifyvoice/model_args.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)    31946 2024-05-20 18:35:17.000000 verifyvoice-0.1.34/verifyvoice/modules.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     1285 2024-05-20 18:35:17.000000 verifyvoice-0.1.34/verifyvoice/utils.py
+drwxrwxr-x   0 thejan    (1000) thejan    (1000)        0 2024-05-21 02:48:27.226250 verifyvoice-0.1.34/verifyvoice.egg-info/
+-rw-r--r--   0 thejan    (1000) thejan    (1000)     3752 2024-05-21 02:48:27.000000 verifyvoice-0.1.34/verifyvoice.egg-info/PKG-INFO
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)      516 2024-05-21 02:48:27.000000 verifyvoice-0.1.34/verifyvoice.egg-info/SOURCES.txt
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)        1 2024-05-21 02:48:27.000000 verifyvoice-0.1.34/verifyvoice.egg-info/dependency_links.txt
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)       55 2024-05-21 02:48:27.000000 verifyvoice-0.1.34/verifyvoice.egg-info/requires.txt
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)       12 2024-05-21 02:48:27.000000 verifyvoice-0.1.34/verifyvoice.egg-info/top_level.txt
```

### Comparing `verifyvoice-0.1.33/PKG-INFO` & `verifyvoice-0.1.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifyvoice
-Version: 0.1.33
+Version: 0.1.34
 Summary: A package for verifying the voice of a person
 Home-page: https://github.com/NirmalSankalana/VerifiVoice
 Author: Nirmal Sankalana, Nipun Thejan
 Author-email: sankalana.nirmal@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `verifyvoice-0.1.33/README.md` & `verifyvoice-0.1.34/README.md`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.33/setup.py` & `verifyvoice-0.1.34/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="verifyvoice",
-    version="0.1.33",
+    version="0.1.34",
     description="A package for verifying the voice of a person",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/NirmalSankalana/VerifiVoice",
     author="Nirmal Sankalana, Nipun Thejan",
     author_email="sankalana.nirmal@gmail.com",
     license="MIT",
```

### Comparing `verifyvoice-0.1.33/verifyvoice/DataLoader.py` & `verifyvoice-0.1.34/verifyvoice/DataLoader.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.33/verifyvoice/ModelLoader.py` & `verifyvoice-0.1.34/verifyvoice/ModelLoader.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 model_name_download_mapping = {
     "model_h4_dim.model": "https://huggingface.co/thejan-fonseka/DeepSpeakerVerifier/blob/main/model_h4_dim.model",
     "model_h8_dim.model": "https://huggingface.co/thejan-fonseka/DeepSpeakerVerifier/blob/main/model_h8_dim.model",
     "model_h16_dim.model": "https://huggingface.co/thejan-fonseka/DeepSpeakerVerifier/blob/main/model_h16_dim.model",
 }
 
 model_threshold = {
-    4: 0.24,
-    8: 0.23,
-    16: 0.21
+    4: 0.4,
+    8: 0.39,
+    16: 0.37
 }
 
 
 class ModelLoader:
     """
     ModelLoader class for loading and working with deep learning models.
```

### Comparing `verifyvoice-0.1.33/verifyvoice/Similarity.py` & `verifyvoice-0.1.34/verifyvoice/Similarity.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.33/verifyvoice/SpeakerNet.py` & `verifyvoice-0.1.34/verifyvoice/SpeakerNet.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.33/verifyvoice/Spk_Encoder.py` & `verifyvoice-0.1.34/verifyvoice/Spk_Encoder.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.33/verifyvoice/WavLM.py` & `verifyvoice-0.1.34/verifyvoice/WavLM.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.33/verifyvoice/aamsoftmax.py` & `verifyvoice-0.1.34/verifyvoice/aamsoftmax.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.33/verifyvoice/deepInfoMaxLoss.py` & `verifyvoice-0.1.34/verifyvoice/deepInfoMaxLoss.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.33/verifyvoice/mine.py` & `verifyvoice-0.1.34/verifyvoice/mine.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.33/verifyvoice/model_args.py` & `verifyvoice-0.1.34/verifyvoice/model_args.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.33/verifyvoice/modules.py` & `verifyvoice-0.1.34/verifyvoice/modules.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.33/verifyvoice/utils.py` & `verifyvoice-0.1.34/verifyvoice/utils.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.33/verifyvoice.egg-info/PKG-INFO` & `verifyvoice-0.1.34/verifyvoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifyvoice
-Version: 0.1.33
+Version: 0.1.34
 Summary: A package for verifying the voice of a person
 Home-page: https://github.com/NirmalSankalana/VerifiVoice
 Author: Nirmal Sankalana, Nipun Thejan
 Author-email: sankalana.nirmal@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `verifyvoice-0.1.33/verifyvoice.egg-info/SOURCES.txt` & `verifyvoice-0.1.34/verifyvoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

