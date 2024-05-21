# Comparing `tmp/pdf2anki-0.1.1.tar.gz` & `tmp/pdf2anki-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf2anki-0.1.1.tar", last modified: Thu Jun  1 18:33:49 2023, max compression
+gzip compressed data, was "pdf2anki-0.1.2.tar", last modified: Tue May 21 19:50:17 2024, max compression
```

## Comparing `pdf2anki-0.1.1.tar` & `pdf2anki-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 fcarva844   (501) staff       (20)        0 2023-06-01 18:33:49.762233 pdf2anki-0.1.1/
--rw-r--r--   0 fcarva844   (501) staff       (20)     1062 2023-06-01 18:28:39.000000 pdf2anki-0.1.1/LICENSE
--rw-r--r--   0 fcarva844   (501) staff       (20)     2359 2023-06-01 18:33:49.759541 pdf2anki-0.1.1/PKG-INFO
--rw-r--r--   0 fcarva844   (501) staff       (20)     1877 2023-06-01 18:28:52.000000 pdf2anki-0.1.1/README.md
-drwxr-xr-x   0 fcarva844   (501) staff       (20)        0 2023-06-01 18:33:49.722526 pdf2anki-0.1.1/pdf2anki/
--rw-r--r--   0 fcarva844   (501) staff       (20)        0 2023-06-01 18:28:52.000000 pdf2anki-0.1.1/pdf2anki/__init__.py
--rw-r--r--   0 fcarva844   (501) staff       (20)     6121 2023-06-01 18:28:52.000000 pdf2anki-0.1.1/pdf2anki/main.py
-drwxr-xr-x   0 fcarva844   (501) staff       (20)        0 2023-06-01 18:33:49.754373 pdf2anki-0.1.1/pdf2anki.egg-info/
--rw-r--r--   0 fcarva844   (501) staff       (20)     2359 2023-06-01 18:33:49.000000 pdf2anki-0.1.1/pdf2anki.egg-info/PKG-INFO
--rw-r--r--   0 fcarva844   (501) staff       (20)      258 2023-06-01 18:33:49.000000 pdf2anki-0.1.1/pdf2anki.egg-info/SOURCES.txt
--rw-r--r--   0 fcarva844   (501) staff       (20)        1 2023-06-01 18:33:49.000000 pdf2anki-0.1.1/pdf2anki.egg-info/dependency_links.txt
--rw-r--r--   0 fcarva844   (501) staff       (20)       48 2023-06-01 18:33:49.000000 pdf2anki-0.1.1/pdf2anki.egg-info/entry_points.txt
--rw-r--r--   0 fcarva844   (501) staff       (20)       30 2023-06-01 18:33:49.000000 pdf2anki-0.1.1/pdf2anki.egg-info/requires.txt
--rw-r--r--   0 fcarva844   (501) staff       (20)        9 2023-06-01 18:33:49.000000 pdf2anki-0.1.1/pdf2anki.egg-info/top_level.txt
--rw-r--r--   0 fcarva844   (501) staff       (20)       38 2023-06-01 18:33:49.762486 pdf2anki-0.1.1/setup.cfg
--rw-r--r--   0 fcarva844   (501) staff       (20)      844 2023-06-01 18:28:52.000000 pdf2anki-0.1.1/setup.py
+drwxr-xr-x   0 fcarva844   (502) staff       (20)        0 2024-05-21 19:50:17.084801 pdf2anki-0.1.2/
+-rw-r--r--   0 fcarva844   (502) staff       (20)     1062 2023-09-12 01:54:37.000000 pdf2anki-0.1.2/LICENSE
+-rw-r--r--   0 fcarva844   (502) staff       (20)     2498 2024-05-21 19:50:17.083968 pdf2anki-0.1.2/PKG-INFO
+-rw-r--r--   0 fcarva844   (502) staff       (20)     2016 2023-09-12 01:54:37.000000 pdf2anki-0.1.2/README.md
+drwxr-xr-x   0 fcarva844   (502) staff       (20)        0 2024-05-21 19:50:17.049469 pdf2anki-0.1.2/pdf2anki/
+-rw-r--r--   0 fcarva844   (502) staff       (20)        0 2023-09-12 01:54:37.000000 pdf2anki-0.1.2/pdf2anki/__init__.py
+-rw-r--r--   0 fcarva844   (502) staff       (20)     6248 2024-05-21 19:41:14.000000 pdf2anki-0.1.2/pdf2anki/main.py
+drwxr-xr-x   0 fcarva844   (502) staff       (20)        0 2024-05-21 19:50:17.083252 pdf2anki-0.1.2/pdf2anki.egg-info/
+-rw-r--r--   0 fcarva844   (502) staff       (20)     2498 2024-05-21 19:50:17.000000 pdf2anki-0.1.2/pdf2anki.egg-info/PKG-INFO
+-rw-r--r--   0 fcarva844   (502) staff       (20)      258 2024-05-21 19:50:17.000000 pdf2anki-0.1.2/pdf2anki.egg-info/SOURCES.txt
+-rw-r--r--   0 fcarva844   (502) staff       (20)        1 2024-05-21 19:50:17.000000 pdf2anki-0.1.2/pdf2anki.egg-info/dependency_links.txt
+-rw-r--r--   0 fcarva844   (502) staff       (20)       48 2024-05-21 19:50:17.000000 pdf2anki-0.1.2/pdf2anki.egg-info/entry_points.txt
+-rw-r--r--   0 fcarva844   (502) staff       (20)       30 2024-05-21 19:50:17.000000 pdf2anki-0.1.2/pdf2anki.egg-info/requires.txt
+-rw-r--r--   0 fcarva844   (502) staff       (20)        9 2024-05-21 19:50:17.000000 pdf2anki-0.1.2/pdf2anki.egg-info/top_level.txt
+-rw-r--r--   0 fcarva844   (502) staff       (20)       38 2024-05-21 19:50:17.084873 pdf2anki-0.1.2/setup.cfg
+-rw-r--r--   0 fcarva844   (502) staff       (20)      844 2023-09-12 01:54:37.000000 pdf2anki-0.1.2/setup.py
```

### Comparing `pdf2anki-0.1.1/LICENSE` & `pdf2anki-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdf2anki-0.1.1/PKG-INFO` & `pdf2anki-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,10 @@
-Metadata-Version: 2.1
-Name: pdf2anki
-Version: 0.1.1
-Summary: A Python package to create Anki cards from PDFs using OpenAI.
-Home-page: https://github.com/hipnologo/pdf2anki
-Author: Fabio Carvalho
-Author-email: hipnologo@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pdf2anki
 
-`pdf2anki` is a Python application that enables you to generate Anki flashcards from PDF files utilizing the power of OpenAI.
+`pdf2anki` is a Python application that enables you to generate Anki flashcards questions from PDF files utilizing the power of OpenAI ChatGPT.
 
 ## Prerequisites
 
 - Python 3.6 or higher
 - Access to OpenAI API (ensure to set your API key as an environment variable named 'OPENAI_API_KEY')
 
 ## Installation
@@ -36,30 +22,30 @@
 ```bash
 pdf2anki --source-dir SOURCE_DIR --output-dir OUTPUT_DIR --model MODEL --temperature TEMPERATURE --max-tokens MAX_TOKENS
 ```
 
 For example:
 
 ```bash
-pdf2anki --source-dir ./pdfs --output-dir ./anki-cards --model gpt-3.5-turbo --temperature 0.5 --max-tokens 1000
+pdf2anki --source-dir ./pdfs --output-dir ./anki-cards --model gpt-4 --temperature 0.5 --max-tokens 1000
 ```
 
 ## For Developers
 Developers can also use pdf2anki in their Python scripts as follows:
 
 ```bash
 import os
 from pdf2anki.main import read_pdf, create_anki_cards
 
 #### Define the source PDF folder and the output folder for the Anki cards
 source_dir = "path/to/pdf_folder"
 output_dir = "path/to/output_folder"
 
 #### Define the parameters for the OpenAI model
-model = "gpt-3.5-turbo"
+model = "gpt-4"
 temperature = 0.5
 max_tokens = 1000
 
 #### Iterate over the PDF files in the source directory
 for file_name in os.listdir(source_dir):
     if file_name.endswith(".pdf"):
         # Get the full path to the source PDF
@@ -73,7 +59,11 @@
 
         # Create Anki cards from the PDF text
         create_anki_cards(pdf_text, output_file, model, temperature, max_tokens)
 ```
 
 ## License
 This project is licensed under the terms of the MIT license. For more details, see the LICENSE file.
+
+## References
+- [pdf2anki package](https://pypi.org/project/pdf2anki/)
+- [OpenAI API key](https://platform.openai.com/account/api-keys)
```

### Comparing `pdf2anki-0.1.1/pdf2anki/main.py` & `pdf2anki-0.1.2/pdf2anki/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,12 @@
+# File: main.py
+# PDF2Anki: A Python library for generating AI-generated Anki flashcards from PDFs
+# Author: Fabio Carvalho
 import os
+import sys
 import argparse
 import PyPDF2
 import openai
 import logging
 from joblib import load
 from typing import List
 
@@ -130,15 +134,15 @@
             output_file = os.path.join(output_dir, file_name.rsplit(".", 1)[0] + ".txt")
             create_anki_cards(pdf_text, output_file, model, temperature, max_tokens, api_key)
 
 def main():
     parser = argparse.ArgumentParser(description='Generate Anki flashcards from PDFs')
     parser.add_argument('--source-dir', type=str, required=True, help='Directory containing source PDFs')
     parser.add_argument('--output-dir', type=str, required=True, help='Directory for output files')
-    parser.add_argument('--model', type=str, required=False, default='gpt-3.5-turbo', help='The OpenAI model to use for generation')
+    parser.add_argument('--model', type=str, required=False, default='gpt-4', help='The OpenAI model to use for generation')
     parser.add_argument('--temperature', type=float, required=False, default='0.3', help='The OpenAI temperature setting')
     parser.add_argument('--max-tokens', type=int, required=False, default='2048', help='The maximum number of tokens for the OpenAI model')
     parser.add_argument('--api-key', type=str, required=False, help='The OpenAI API key')
     parser.add_argument('--section-size', type=int, default=1000, help='Section size for dividing text')
     args = parser.parse_args()
     
     api_key = args.api_key if args.api_key else os.getenv('OPENAI_API_KEY')
```

### Comparing `pdf2anki-0.1.1/pdf2anki.egg-info/PKG-INFO` & `pdf2anki-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pdf2anki
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package to create Anki cards from PDFs using OpenAI.
 Home-page: https://github.com/hipnologo/pdf2anki
 Author: Fabio Carvalho
 Author-email: hipnologo@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pdf2anki
 
-`pdf2anki` is a Python application that enables you to generate Anki flashcards from PDF files utilizing the power of OpenAI.
+`pdf2anki` is a Python application that enables you to generate Anki flashcards questions from PDF files utilizing the power of OpenAI ChatGPT.
 
 ## Prerequisites
 
 - Python 3.6 or higher
 - Access to OpenAI API (ensure to set your API key as an environment variable named 'OPENAI_API_KEY')
 
 ## Installation
@@ -36,30 +36,30 @@
 ```bash
 pdf2anki --source-dir SOURCE_DIR --output-dir OUTPUT_DIR --model MODEL --temperature TEMPERATURE --max-tokens MAX_TOKENS
 ```
 
 For example:
 
 ```bash
-pdf2anki --source-dir ./pdfs --output-dir ./anki-cards --model gpt-3.5-turbo --temperature 0.5 --max-tokens 1000
+pdf2anki --source-dir ./pdfs --output-dir ./anki-cards --model gpt-4 --temperature 0.5 --max-tokens 1000
 ```
 
 ## For Developers
 Developers can also use pdf2anki in their Python scripts as follows:
 
 ```bash
 import os
 from pdf2anki.main import read_pdf, create_anki_cards
 
 #### Define the source PDF folder and the output folder for the Anki cards
 source_dir = "path/to/pdf_folder"
 output_dir = "path/to/output_folder"
 
 #### Define the parameters for the OpenAI model
-model = "gpt-3.5-turbo"
+model = "gpt-4"
 temperature = 0.5
 max_tokens = 1000
 
 #### Iterate over the PDF files in the source directory
 for file_name in os.listdir(source_dir):
     if file_name.endswith(".pdf"):
         # Get the full path to the source PDF
@@ -73,7 +73,11 @@
 
         # Create Anki cards from the PDF text
         create_anki_cards(pdf_text, output_file, model, temperature, max_tokens)
 ```
 
 ## License
 This project is licensed under the terms of the MIT license. For more details, see the LICENSE file.
+
+## References
+- [pdf2anki package](https://pypi.org/project/pdf2anki/)
+- [OpenAI API key](https://platform.openai.com/account/api-keys)
```

### Comparing `pdf2anki-0.1.1/setup.py` & `pdf2anki-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pdf2anki',
-    version='0.1.1',
+    version='0.1.2',
     description='A Python package to create Anki cards from PDFs using OpenAI.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Fabio Carvalho',
     author_email='hipnologo@gmail.com',
     url='https://github.com/hipnologo/pdf2anki',
     packages=find_packages(exclude=['pdftoanki']),
```

