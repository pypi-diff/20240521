# Comparing `tmp/audiostack-1.3.1.tar.gz` & `tmp/audiostack-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostack-1.3.1.tar", last modified: Mon May 20 08:16:31 2024, max compression
+gzip compressed data, was "audiostack-2.0.0a0.tar", max compression
```

## Comparing `audiostack-1.3.1.tar` & `audiostack-2.0.0a0.tar`

### file list

```diff
@@ -1,49 +1,45 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.350443 audiostack-1.3.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1061 2024-05-20 08:16:07.000000 audiostack-1.3.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5458 2024-05-20 08:16:31.346442 audiostack-1.3.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2024-05-20 08:16:07.000000 audiostack-1.3.1/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.342442 audiostack-1.3.1/audiostack/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-20 08:16:24.000000 audiostack-1.3.1/audiostack/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.342442 audiostack-1.3.1/audiostack/content/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/content/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6077 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/content/file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2270 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/content/media.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2088 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/content/recommend.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      947 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/content/root_functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4183 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/content/script.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.346442 audiostack-1.3.1/audiostack/delivery/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/delivery/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3462 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/delivery/encoder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/delivery/video.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.346442 audiostack-1.3.1/audiostack/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/docs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/docs/docs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.346442 audiostack-1.3.1/audiostack/helpers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/helpers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      715 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/helpers/api_item.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      972 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/helpers/api_list.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4732 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/helpers/request_interface.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/helpers/request_types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      338 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/helpers/response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/helpers/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.346442 audiostack-1.3.1/audiostack/orchestrator/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/orchestrator/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.346442 audiostack-1.3.1/audiostack/production/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      134 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/production/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4801 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/production/mix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4286 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/production/sound.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4265 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/production/suite.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.346442 audiostack-1.3.1/audiostack/speech/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/speech/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2979 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/speech/diction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/speech/predict.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7488 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/speech/tts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2189 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/speech/voice.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.346442 audiostack-1.3.1/audiostack.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5458 2024-05-20 08:16:31.000000 audiostack-1.3.1/audiostack.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1074 2024-05-20 08:16:31.000000 audiostack-1.3.1/audiostack.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-20 08:16:31.000000 audiostack-1.3.1/audiostack.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2024-05-20 08:16:31.000000 audiostack-1.3.1/audiostack.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2024-05-20 08:16:31.000000 audiostack-1.3.1/audiostack.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-20 08:16:31.350443 audiostack-1.3.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1039 2024-05-20 08:16:07.000000 audiostack-1.3.1/setup.py
+-rw-r--r--   0        0        0     1061 2024-05-16 19:16:57.894489 audiostack-2.0.0a0/LICENSE
+-rw-r--r--   0        0        0     4967 2024-05-21 09:54:00.601575 audiostack-2.0.0a0/README.md
+-rw-r--r--   0        0        0      520 2024-05-21 09:54:00.601895 audiostack-2.0.0a0/audiostack/__init__.py
+-rw-r--r--   0        0        0      819 2024-05-21 09:54:00.602382 audiostack-2.0.0a0/audiostack/content/__init__.py
+-rw-r--r--   0        0        0     6199 2024-05-21 09:54:00.602974 audiostack-2.0.0a0/audiostack/content/file.py
+-rw-r--r--   0        0        0     2321 2024-05-21 09:54:00.603553 audiostack-2.0.0a0/audiostack/content/media.py
+-rw-r--r--   0        0        0     2178 2024-05-21 09:54:00.604277 audiostack-2.0.0a0/audiostack/content/recommend.py
+-rw-r--r--   0        0        0     1029 2024-05-21 09:54:00.604729 audiostack-2.0.0a0/audiostack/content/root_functions.py
+-rw-r--r--   0        0        0     4360 2024-05-21 09:54:00.605290 audiostack-2.0.0a0/audiostack/content/script.py
+-rw-r--r--   0        0        0      120 2024-05-21 09:54:00.605797 audiostack-2.0.0a0/audiostack/delivery/__init__.py
+-rw-r--r--   0        0        0     3564 2024-05-21 09:54:00.606302 audiostack-2.0.0a0/audiostack/delivery/encoder.py
+-rw-r--r--   0        0        0     2116 2024-05-21 09:54:00.606819 audiostack-2.0.0a0/audiostack/delivery/video.py
+-rw-r--r--   0        0        0       61 2024-05-21 09:54:00.607276 audiostack-2.0.0a0/audiostack/docs/__init__.py
+-rw-r--r--   0        0        0      602 2024-05-21 09:54:00.607654 audiostack-2.0.0a0/audiostack/docs/docs.py
+-rw-r--r--   0        0        0        0 2024-05-16 19:16:57.895701 audiostack-2.0.0a0/audiostack/helpers/__init__.py
+-rw-r--r--   0        0        0      764 2024-05-21 09:54:00.607893 audiostack-2.0.0a0/audiostack/helpers/api_item.py
+-rw-r--r--   0        0        0     1102 2024-05-21 09:54:00.608269 audiostack-2.0.0a0/audiostack/helpers/api_list.py
+-rw-r--r--   0        0        0     4916 2024-05-21 09:54:00.608702 audiostack-2.0.0a0/audiostack/helpers/request_interface.py
+-rw-r--r--   0        0        0      163 2024-05-16 19:16:57.895951 audiostack-2.0.0a0/audiostack/helpers/request_types.py
+-rw-r--r--   0        0        0      388 2024-05-21 09:54:00.608998 audiostack-2.0.0a0/audiostack/helpers/response.py
+-rw-r--r--   0        0        0      227 2024-05-16 19:16:57.896061 audiostack-2.0.0a0/audiostack/helpers/util.py
+-rw-r--r--   0        0        0       58 2024-05-16 19:16:57.896140 audiostack-2.0.0a0/audiostack/orchestrator/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-21 09:54:00.609336 audiostack-2.0.0a0/audiostack/production/__init__.py
+-rw-r--r--   0        0        0     5096 2024-05-21 09:54:00.609619 audiostack-2.0.0a0/audiostack/production/mix.py
+-rw-r--r--   0        0        0     4542 2024-05-21 09:54:00.609917 audiostack-2.0.0a0/audiostack/production/sound.py
+-rw-r--r--   0        0        0     4630 2024-05-21 09:54:00.610401 audiostack-2.0.0a0/audiostack/production/suite.py
+-rw-r--r--   0        0        0      228 2024-05-21 09:54:00.611925 audiostack-2.0.0a0/audiostack/speech/__init__.py
+-rw-r--r--   0        0        0     3179 2024-05-21 09:54:00.612294 audiostack-2.0.0a0/audiostack/speech/diction.py
+-rw-r--r--   0        0        0     1294 2024-05-21 09:54:00.612830 audiostack-2.0.0a0/audiostack/speech/predict.py
+-rw-r--r--   0        0        0     7903 2024-05-21 09:54:00.613361 audiostack-2.0.0a0/audiostack/speech/tts.py
+-rw-r--r--   0        0        0     2325 2024-05-21 09:54:00.613771 audiostack-2.0.0a0/audiostack/speech/voice.py
+-rw-r--r--   0        0        0     1200 2024-05-21 09:54:00.614173 audiostack-2.0.0a0/audiostack/tests/content/test_file.py
+-rw-r--r--   0        0        0      673 2024-05-21 09:54:00.614999 audiostack-2.0.0a0/audiostack/tests/content/test_folder.py
+-rw-r--r--   0        0        0     3832 2024-05-21 09:54:00.615377 audiostack-2.0.0a0/audiostack/tests/content/test_recommend.py
+-rw-r--r--   0        0        0      906 2024-05-21 09:54:00.615688 audiostack-2.0.0a0/audiostack/tests/content/test_transfer.py
+-rw-r--r--   0        0        0      495 2024-05-21 09:54:00.616144 audiostack-2.0.0a0/audiostack/tests/production/test_aes.py
+-rw-r--r--   0        0        0      364 2024-05-21 09:54:00.616490 audiostack-2.0.0a0/audiostack/tests/production/test_sound.py
+-rw-r--r--   0        0        0      978 2024-05-21 09:54:00.616717 audiostack-2.0.0a0/audiostack/tests/production/test_suite.py
+-rw-r--r--   0        0        0      591 2024-05-21 09:54:00.616966 audiostack-2.0.0a0/audiostack/tests/production/test_video.py
+-rw-r--r--   0        0        0     1292 2024-05-21 09:54:00.617179 audiostack-2.0.0a0/audiostack/tests/test_script.py
+-rw-r--r--   0        0        0     1071 2024-05-21 09:54:00.617459 audiostack-2.0.0a0/audiostack/tests/tts/test_lexi.py
+-rw-r--r--   0        0        0     1427 2024-05-21 09:54:00.617709 audiostack-2.0.0a0/audiostack/tests/tts/test_predict.py
+-rw-r--r--   0        0        0      488 2024-05-21 09:54:00.617968 audiostack-2.0.0a0/audiostack/tests/tts/test_voice.py
+-rw-r--r--   0        0        0     1825 2024-05-21 09:54:00.619085 audiostack-2.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0     5717 1970-01-01 00:00:00.000000 audiostack-2.0.0a0/PKG-INFO
```

### Comparing `audiostack-1.3.1/LICENSE` & `audiostack-2.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.1/PKG-INFO` & `audiostack-2.0.0a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: audiostack
-Version: 1.3.1
+Version: 2.0.0a0
 Summary: Python SDK for Audiostack API
 Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic
-Author-email: sam@aflorithmic.ai
-Classifier: Programming Language :: Python :: 3
+Author-email: support@audiostack.ai
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Repository, https://github.com/aflorithmic/audiostack-python
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.28.1; python_version >= "3.6"
 
 <p align="center">
 <a href="https://www.api.audio/" rel="noopener">
  <img src="https://uploads-ssl.webflow.com/60b89b300a9c71a64936aafd/60c1d07f4fd2c92916129788_logoAudio.svg" alt="api.audio logo"></a>
 </p>
 
 <h3 align="center">Audiostack SDK</h3>
@@ -42,15 +46,15 @@
 
 ```sh
 pip install audiostack -U
 ```
 
 ### Prerequisites <a name = "requirements"></a>
 
-Python 3.6+
+Python `^3.8.1`
 
 ### Authentication
 
 This library needs to be configured with your account's API key which is available in your [Audiostack platform](https://platform.audiostack.ai/audiostackapi). Import the audiostack package and set `audiostack.api_key` with the API key you got from the console:
 
 ```python
 import audiostack
@@ -135,7 +139,8 @@
 
 - https://github.com/Sjhunt93
 
 ## License <a name = "license"> </a>
 
 This project is licensed under the terms of the MIT license.
 
+
```

#### html2text {}

```diff
@@ -1,55 +1,58 @@
-Metadata-Version: 2.1 Name: audiostack Version: 1.3.1 Summary: Python SDK for
+Metadata-Version: 2.1 Name: audiostack Version: 2.0.0a0 Summary: Python SDK for
 Audiostack API Home-page: https://github.com/aflorithmic/audiostack-python
-Author: Aflorithmic Author-email: sam@aflorithmic.ai Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-requests>=2.28.1; python_version >= "3.6"
+Author: Aflorithmic Author-email: support@audiostack.ai Requires-Python:
+>=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Requires-Dist: requests
+(>=2.31.0,<3.0.0) Project-URL: Repository, https://github.com/aflorithmic/
+audiostack-python Description-Content-Type: text/markdown
                                _[_a_p_i_._a_u_d_i_o_ _l_o_g_o_]
                            ******** AAuuddiioossttaacckk SSDDKK ********
 ---
 This is the official _a_u_d_i_o_s_t_a_c_k Python 3 SDK. This SDK provides easy access to
             the Audiostack API for applications written in Python.
 ## ð§ About This repository is actively maintained by [Audiostack](https://
 audiostack.ai/). For examples, recipes and api reference see the [api.audio
 docs](https://docs.audiostack.ai/reference/quick-start). Feel free to get in
 touch with any questions or feedback! ## :book: Changelog You can view [here]
 (https://docs.audiostack.ai/changelog) our updated Changelog. ## ð Getting
 Started ### Installation You don't need this source code unless you want to
 modify it. If you want to use the package, just run: ```sh pip install
-audiostack -U ``` ### Prerequisites Python 3.6+ ### Authentication This library
-needs to be configured with your account's API key which is available in your
-[Audiostack platform](https://platform.audiostack.ai/audiostackapi). Import the
-audiostack package and set `audiostack.api_key` with the API key you got from
-the console: ```python import audiostack audiostack.api_key = "your-key" ``` If
-you belong to multiple organizations, by default the API will use the first
-organization you had access to. You can specify the organization by setting the
-`assume_org_id` attribute: ```python audiostack.assume_org_id = "your-org-id"
-``` ### Create your first audio asset #### âï¸ First, create a Script.
-Audiostack Scripts are the first step in creating audio assets. Not only do
-they contain the text to be spoken, but also determine the final structure of
-our audio asset using the [Script Syntax](https://docs.audiostack.ai/docs/
-script-syntax). It also supports a [unified SSML syntax](https://
-docs.audiostack.ai/docs/ssml-tags), which is a standard way to control speech
-synthesis. ```python script = audiostack.Content.Script.create(scriptText="""
-Hey there, friend! Welcome to Audiostack - the audio creation platform that
-allows you to create high quality audio assets using just a few lines of code.
-Whether it's a podcast, a video, a game, or an app, Audiostack has you covered.
-You can create voiceovers, sound effects, music, and more. We are excited to
-see what you'll create with our product! """) ``` #### ð¤ Now, let's read it
-out load. We integrate all the major TTS voices in the market. You can browse
-them in our [voice library](https://library.audiostack.ai/). Let's use the
-voice "Isaac", substitute the `username` placeholder with `mate` and download
-the produced files. Each section results in a seperate audio file. ```python
-tts = audiostack.Speech.TTS.create(scriptItem=script, voice="isaac", audience=
-{"username": "mate"}) tts.download(fileName="example") ``` When you listen to
-these files, you'll notice each of them has a certain silence padding at the
-end. This might be useful for some use cases, but for this example, let's
-remove it. ```python tts = audiostack.Speech.TTS.remove_padding
+audiostack -U ``` ### Prerequisites Python `^3.8.1` ### Authentication This
+library needs to be configured with your account's API key which is available
+in your [Audiostack platform](https://platform.audiostack.ai/audiostackapi).
+Import the audiostack package and set `audiostack.api_key` with the API key you
+got from the console: ```python import audiostack audiostack.api_key = "your-
+key" ``` If you belong to multiple organizations, by default the API will use
+the first organization you had access to. You can specify the organization by
+setting the `assume_org_id` attribute: ```python audiostack.assume_org_id =
+"your-org-id" ``` ### Create your first audio asset #### âï¸ First, create a
+Script. Audiostack Scripts are the first step in creating audio assets. Not
+only do they contain the text to be spoken, but also determine the final
+structure of our audio asset using the [Script Syntax](https://
+docs.audiostack.ai/docs/script-syntax). It also supports a [unified SSML
+syntax](https://docs.audiostack.ai/docs/ssml-tags), which is a standard way to
+control speech synthesis. ```python script = audiostack.Content.Script.create
+(scriptText=""" Hey there, friend! Welcome to Audiostack - the audio creation
+platform that allows you to create high quality audio assets using just a few
+lines of code. Whether it's a podcast, a video, a game, or an app, Audiostack
+has you covered. You can create voiceovers, sound effects, music, and more. We
+are excited to see what you'll create with our product! """) ``` #### ð¤ Now,
+let's read it out load. We integrate all the major TTS voices in the market.
+You can browse them in our [voice library](https://library.audiostack.ai/).
+Let's use the voice "Isaac", substitute the `username` placeholder with `mate`
+and download the produced files. Each section results in a seperate audio file.
+```python tts = audiostack.Speech.TTS.create(scriptItem=script, voice="isaac",
+audience={"username": "mate"}) tts.download(fileName="example") ``` When you
+listen to these files, you'll notice each of them has a certain silence padding
+at the end. This might be useful for some use cases, but for this example,
+let's remove it. ```python tts = audiostack.Speech.TTS.remove_padding
 (speechId=tts.speechId) ``` #### ðï¸ Now let's mix the speech we just
 created with a [sound template](https://library.audiostack.ai/sound). ```python
 mix = audiostack.Production.Mix.create(speechItem=tts,
 soundTemplate="chill_vibes") ``` Various sound templates consist of various
 segments. In our example, we're using three segments: intro, main and outro.
 You can list all the sound templates to see what segments are available or even
 [create your own](https://docs.audiostack.ai/docs/custom-sound-design-
```

### Comparing `audiostack-1.3.1/README.md` & `audiostack-2.0.0a0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 ```sh
 pip install audiostack -U
 ```
 
 ### Prerequisites <a name = "requirements"></a>
 
-Python 3.6+
+Python `^3.8.1`
 
 ### Authentication
 
 This library needs to be configured with your account's API key which is available in your [Audiostack platform](https://platform.audiostack.ai/audiostackapi). Import the audiostack package and set `audiostack.api_key` with the API key you got from the console:
 
 ```python
 import audiostack
```

#### html2text {}

```diff
@@ -6,43 +6,43 @@
 ## ð§ About This repository is actively maintained by [Audiostack](https://
 audiostack.ai/). For examples, recipes and api reference see the [api.audio
 docs](https://docs.audiostack.ai/reference/quick-start). Feel free to get in
 touch with any questions or feedback! ## :book: Changelog You can view [here]
 (https://docs.audiostack.ai/changelog) our updated Changelog. ## ð Getting
 Started ### Installation You don't need this source code unless you want to
 modify it. If you want to use the package, just run: ```sh pip install
-audiostack -U ``` ### Prerequisites Python 3.6+ ### Authentication This library
-needs to be configured with your account's API key which is available in your
-[Audiostack platform](https://platform.audiostack.ai/audiostackapi). Import the
-audiostack package and set `audiostack.api_key` with the API key you got from
-the console: ```python import audiostack audiostack.api_key = "your-key" ``` If
-you belong to multiple organizations, by default the API will use the first
-organization you had access to. You can specify the organization by setting the
-`assume_org_id` attribute: ```python audiostack.assume_org_id = "your-org-id"
-``` ### Create your first audio asset #### âï¸ First, create a Script.
-Audiostack Scripts are the first step in creating audio assets. Not only do
-they contain the text to be spoken, but also determine the final structure of
-our audio asset using the [Script Syntax](https://docs.audiostack.ai/docs/
-script-syntax). It also supports a [unified SSML syntax](https://
-docs.audiostack.ai/docs/ssml-tags), which is a standard way to control speech
-synthesis. ```python script = audiostack.Content.Script.create(scriptText="""
-Hey there, friend! Welcome to Audiostack - the audio creation platform that
-allows you to create high quality audio assets using just a few lines of code.
-Whether it's a podcast, a video, a game, or an app, Audiostack has you covered.
-You can create voiceovers, sound effects, music, and more. We are excited to
-see what you'll create with our product! """) ``` #### ð¤ Now, let's read it
-out load. We integrate all the major TTS voices in the market. You can browse
-them in our [voice library](https://library.audiostack.ai/). Let's use the
-voice "Isaac", substitute the `username` placeholder with `mate` and download
-the produced files. Each section results in a seperate audio file. ```python
-tts = audiostack.Speech.TTS.create(scriptItem=script, voice="isaac", audience=
-{"username": "mate"}) tts.download(fileName="example") ``` When you listen to
-these files, you'll notice each of them has a certain silence padding at the
-end. This might be useful for some use cases, but for this example, let's
-remove it. ```python tts = audiostack.Speech.TTS.remove_padding
+audiostack -U ``` ### Prerequisites Python `^3.8.1` ### Authentication This
+library needs to be configured with your account's API key which is available
+in your [Audiostack platform](https://platform.audiostack.ai/audiostackapi).
+Import the audiostack package and set `audiostack.api_key` with the API key you
+got from the console: ```python import audiostack audiostack.api_key = "your-
+key" ``` If you belong to multiple organizations, by default the API will use
+the first organization you had access to. You can specify the organization by
+setting the `assume_org_id` attribute: ```python audiostack.assume_org_id =
+"your-org-id" ``` ### Create your first audio asset #### âï¸ First, create a
+Script. Audiostack Scripts are the first step in creating audio assets. Not
+only do they contain the text to be spoken, but also determine the final
+structure of our audio asset using the [Script Syntax](https://
+docs.audiostack.ai/docs/script-syntax). It also supports a [unified SSML
+syntax](https://docs.audiostack.ai/docs/ssml-tags), which is a standard way to
+control speech synthesis. ```python script = audiostack.Content.Script.create
+(scriptText=""" Hey there, friend! Welcome to Audiostack - the audio creation
+platform that allows you to create high quality audio assets using just a few
+lines of code. Whether it's a podcast, a video, a game, or an app, Audiostack
+has you covered. You can create voiceovers, sound effects, music, and more. We
+are excited to see what you'll create with our product! """) ``` #### ð¤ Now,
+let's read it out load. We integrate all the major TTS voices in the market.
+You can browse them in our [voice library](https://library.audiostack.ai/).
+Let's use the voice "Isaac", substitute the `username` placeholder with `mate`
+and download the produced files. Each section results in a seperate audio file.
+```python tts = audiostack.Speech.TTS.create(scriptItem=script, voice="isaac",
+audience={"username": "mate"}) tts.download(fileName="example") ``` When you
+listen to these files, you'll notice each of them has a certain silence padding
+at the end. This might be useful for some use cases, but for this example,
+let's remove it. ```python tts = audiostack.Speech.TTS.remove_padding
 (speechId=tts.speechId) ``` #### ðï¸ Now let's mix the speech we just
 created with a [sound template](https://library.audiostack.ai/sound). ```python
 mix = audiostack.Production.Mix.create(speechItem=tts,
 soundTemplate="chill_vibes") ``` Various sound templates consist of various
 segments. In our example, we're using three segments: intro, main and outro.
 You can list all the sound templates to see what segments are available or even
 [create your own](https://docs.audiostack.ai/docs/custom-sound-design-
```

### Comparing `audiostack-1.3.1/audiostack/content/__init__.py` & `audiostack-2.0.0a0/audiostack/content/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-from audiostack.content.script import Script
-from audiostack.content.media import Media
-from audiostack.content.file import File, Folder
-from audiostack.content.recommend import RecommendTag, RecommendMood, RecommendTone
+from audiostack.content.file import File, Folder  # noqa: F401
+from audiostack.content.media import Media  # noqa: F401
+from audiostack.content.recommend import (  # noqa: F401
+    RecommendMood,
+    RecommendTag,
+    RecommendTone,
+)
+from audiostack.content.script import Script  # noqa: F401
+from audiostack.helpers.api_item import APIResponseItem
 
 
-def list_projects():
+def list_projects() -> APIResponseItem:
     from audiostack.content.root_functions import Root
 
     return Root.list_projects()
 
 
-def list_modules():
+def list_modules(projectName: str) -> APIResponseItem:
     from audiostack.content.root_functions import Root
 
-    return Root.list_modules()
+    return Root.list_modules(projectName=projectName)
 
-def generate(prompt: str, max_length: int = 100):
+
+def generate(prompt: str, max_length: int = 100) -> APIResponseItem:
     from audiostack.content.root_functions import Root
 
-    return Root.generate(prompt, max_length)
+    return Root.generate(prompt, max_length)
```

### Comparing `audiostack-1.3.1/audiostack/content/file.py` & `audiostack-2.0.0a0/audiostack/content/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,53 @@
-from audiostack.helpers.request_interface import RequestInterface
-from audiostack.helpers.request_types import RequestTypes
+import os
+from typing import Any
+
 from audiostack.helpers.api_item import APIResponseItem
 from audiostack.helpers.api_list import APIResponseList
-import os
+from audiostack.helpers.request_interface import RequestInterface
+from audiostack.helpers.request_types import RequestTypes
 
 
 class File:
     FAMILY = "content"
     interface = RequestInterface(family=FAMILY)
 
     class Item(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
             self.fileId = self.data["fileId"]
             self.filePath = self.data["filePath"]
             self.url = self.data.get("url", None)
 
-        def delete(self):
+        def delete(self) -> APIResponseItem:
             return File.delete(self.fileId)
-    
-        def download(self, fileName="", path="./") -> None:
+
+        def download(self, fileName: str = "", path: str = "./") -> None:
             if not fileName:
                 fileName = self.filePath.split("/")[-1]
             RequestInterface.download_url(self.url, destination=path, name=fileName)
 
     class List(APIResponseList):
-        def __init__(self, response, list_type) -> None:
+        def __init__(self, response: dict, list_type: str) -> None:
             super().__init__(response, list_type)
 
-        def resolve_item(self, list_type, item):
+        def resolve_item(self, list_type: str, item: Any) -> "File.Item":
             if list_type == "items" or list_type == "files":
                 return File.Item({"data": item})
             else:
                 raise Exception()
 
     @staticmethod
     def create(
         localPath: str,
         uploadPath: str,
         fileType: str,
         category: str = "",
         tags: list = [],
         metadata: dict = {},
-        filePath: str = None,
     ) -> Item:
         if not os.path.isfile(localPath):
             raise Exception("Supplied file does not eixst")
 
         if not uploadPath or not localPath:
             raise Exception(
                 "Please supply a localPath (path to your local file) and an uploadPath (path to where youd like this to be saved)"
@@ -66,17 +67,15 @@
             route="file/create-upload-url",
             json=data,
         )
         response = APIResponseItem(r)
         url = response.data["fileUploadUrl"]
         fileId = response.data["fileId"]
 
-        status = File.interface.send_upload_request(
-            local_path=localPath, upload_url=url
-        )
+        File.interface.send_upload_request(local_path=localPath, upload_url=url)
         return File.get(fileId)
 
     @staticmethod
     def transfer(
         url: str,
         uploadPath: str,
         category: str = "",
@@ -112,30 +111,30 @@
         data = {
             "filePath": filePath,
             "category": category,
             "tags": tags,
             "metadata": metadata,
         }
 
-        r = File.interface.send_request(
+        File.interface.send_request(
             rtype=RequestTypes.PATCH,
             route=f"file/id/{fileId}",
             json=data,
         )
         return File.get(fileId)
 
     @staticmethod
     def get(fileId: str) -> Item:
         r = File.interface.send_request(
             rtype=RequestTypes.GET, route="file/id", path_parameters=fileId
         )
         return File.Item(r)
 
     @staticmethod
-    def delete(fileId: str) -> str:
+    def delete(fileId: str) -> APIResponseItem:
         r = File.interface.send_request(
             rtype=RequestTypes.DELETE, route="file/id", path_parameters=fileId
         )
         return APIResponseItem(r)
 
     @staticmethod
     def search(
@@ -163,47 +162,47 @@
 
 
 class Folder:
     FAMILY = "content"
     interface = RequestInterface(family=FAMILY)
 
     class Item(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
             self.folders = Folder.List(response, list_type="folders")
             self.files = File.List(response, list_type="files")
 
     class List(APIResponseList):
-        def __init__(self, response, list_type) -> None:
+        def __init__(self, response: dict, list_type: str) -> None:
             super().__init__(response, list_type)
 
-        def resolve_item(self, list_type, item):
+        def resolve_item(self, list_type: str, item: Any) -> dict:
             if list_type == "folders":
                 return {"data": item}
             else:
                 raise Exception()
 
     @staticmethod
-    def create(name) -> Item:
+    def create(name: Any) -> APIResponseItem:
 
         r = File.interface.send_request(
             rtype=RequestTypes.POST,
             route="folder",
             json={"folder": name},
         )
         return APIResponseItem(r)
 
     @staticmethod
-    def list(folder: str) -> Item:
+    def list(folder: str) -> "Folder.Item":
         r = File.interface.send_request(
             rtype=RequestTypes.GET, route="folder", query_parameters={"folder": folder}
         )
         return Folder.Item(r)
 
     @staticmethod
-    def delete(folder: str, delete_files=False) -> str:
+    def delete(folder: str, delete_files: bool = False) -> APIResponseItem:
         r = File.interface.send_request(
             rtype=RequestTypes.DELETE,
             route="folder",
             query_parameters={"folder": folder, "forceDelete": delete_files},
         )
         return APIResponseItem(r)
```

### Comparing `audiostack-1.3.1/audiostack/content/media.py` & `audiostack-2.0.0a0/audiostack/content/media.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-from audiostack.helpers.request_interface import RequestInterface
-from audiostack.helpers.request_types import RequestTypes
+import os
+from typing import Any
+
 from audiostack.helpers.api_item import APIResponseItem
 from audiostack.helpers.api_list import APIResponseList
-import os
-import requests
+from audiostack.helpers.request_interface import RequestInterface
+from audiostack.helpers.request_types import RequestTypes
 
 
 class Media:
     FAMILY = "content"
     interface = RequestInterface(family=FAMILY)
 
     class Item(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
 
             self.mediaId = self.data["mediaId"]
             self.tags = self.data["tags"]
             self.filename = self.data["filename"]
 
-        def delete(self):
+        def delete(self) -> APIResponseItem:
             return Media.delete(self.mediaId)
 
     class List(APIResponseList):
-        def __init__(self, response, list_type) -> None:
+        def __init__(self, response: dict, list_type: str) -> None:
             super().__init__(response, list_type)
 
-        def resolve_item(self, list_type, item):
+        def resolve_item(self, list_type: str, item: Any) -> "Media.Item":
             if list_type == "mediaFiles":
                 return Media.Item({"data": item})
             else:
                 raise Exception()
 
     @staticmethod
     def create(filePath: str) -> Item:
@@ -43,28 +44,26 @@
             route="media/create-upload-url",
             json={"fileName": name},
         )
         response = APIResponseItem(r)
         url = response.data["fileUploadUrl"]
         mediaId = response.data["mediaId"]
 
-        status = Media.interface.send_upload_request(
-            local_path=filePath, upload_url=url
-        )
+        Media.interface.send_upload_request(local_path=filePath, upload_url=url)
         return Media.get(mediaId)
 
     @staticmethod
     def get(mediaId: str) -> Item:
         r = Media.interface.send_request(
             rtype=RequestTypes.GET, route="media", path_parameters=mediaId
         )
         return Media.Item(r)
 
     @staticmethod
-    def delete(mediaId: str) -> str:
+    def delete(mediaId: str) -> APIResponseItem:
         r = Media.interface.send_request(
             rtype=RequestTypes.DELETE, route="media", path_parameters=mediaId
         )
         return APIResponseItem(r)
 
     @staticmethod
     def list() -> List:
```

### Comparing `audiostack-1.3.1/audiostack/content/recommend.py` & `audiostack-2.0.0a0/audiostack/content/recommend.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import List
 
+from audiostack.helpers.api_item import APIResponseItem
 from audiostack.helpers.request_interface import RequestInterface
 from audiostack.helpers.request_types import RequestTypes
-from audiostack.helpers.api_item import APIResponseItem
 
 
 class RecommendTag:
     FAMILY = "content"
     interface = RequestInterface(family=FAMILY)
 
     class Item(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
 
             self.tags = self.data["tags"]
 
     @staticmethod
     def create(
         text: str, category: str, tags: List, number_of_results: int = 1
@@ -22,48 +22,54 @@
         payload = {
             "text": text,
             "category": category,
             "tags": tags,
             "number_of_results": number_of_results,
         }
         r = RecommendTag.interface.send_request(
-            rtype=RequestTypes.POST, route="recommend/tag", json=payload,
+            rtype=RequestTypes.POST,
+            route="recommend/tag",
+            json=payload,
         )
         return RecommendTag.Item(r)
 
 
 class RecommendMood:
     FAMILY = "content"
     interface = RequestInterface(family=FAMILY)
 
     class Item(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
 
             self.moods = self.data["tags"]
 
     @staticmethod
     def create(text: str, number_of_results: int = 1) -> Item:
         payload = {"text": text, "number_of_results": number_of_results}
         r = RecommendMood.interface.send_request(
-            rtype=RequestTypes.POST, route="recommend/mood", json=payload,
+            rtype=RequestTypes.POST,
+            route="recommend/mood",
+            json=payload,
         )
         return RecommendMood.Item(r)
 
 
 class RecommendTone:
     FAMILY = "content"
     interface = RequestInterface(family=FAMILY)
 
     class Item(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
 
             self.tones = self.data["tags"]
 
     @staticmethod
     def create(text: str, number_of_results: int = 1) -> Item:
         payload = {"text": text, "number_of_results": number_of_results}
         r = RecommendTone.interface.send_request(
-            rtype=RequestTypes.POST, route="recommend/tone", json=payload,
+            rtype=RequestTypes.POST,
+            route="recommend/tone",
+            json=payload,
         )
         return RecommendTone.Item(r)
```

### Comparing `audiostack-1.3.1/audiostack/content/root_functions.py` & `audiostack-2.0.0a0/audiostack/content/root_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,30 @@
+from audiostack.helpers.api_item import APIResponseItem
 from audiostack.helpers.request_interface import RequestInterface
 from audiostack.helpers.request_types import RequestTypes
-from audiostack.helpers.api_item import APIResponseItem
 
 
 class Root:
     interface = RequestInterface(family="content")
 
-    def list_projects() -> list:
+    @staticmethod
+    def list_projects() -> APIResponseItem:
         r = Root.interface.send_request(rtype=RequestTypes.GET, route="list_projects")
         return APIResponseItem(r)
 
-    def list_modules(projectName: str) -> list:
+    @staticmethod
+    def list_modules(projectName: str) -> APIResponseItem:
         r = Root.interface.send_request(
             rtype=RequestTypes.GET,
             route="list_projects",
             query_parameters={"projectName": projectName},
         )
         return APIResponseItem(r)
-    
-    def generate(prompt: str, max_length: int = 100) -> list:
+
+    @staticmethod
+    def generate(prompt: str, max_length: int = 100) -> APIResponseItem:
         r = Root.interface.send_request(
             rtype=RequestTypes.POST,
             route="generate",
-            json={"prompt": prompt, "max_length" : max_length},
+            json={"prompt": prompt, "max_length": max_length},
         )
         return APIResponseItem(r)
```

### Comparing `audiostack-1.3.1/audiostack/content/script.py` & `audiostack-2.0.0a0/audiostack/content/script.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-from audiostack.helpers.request_interface import RequestInterface
-from audiostack.helpers.request_types import RequestTypes
+from typing import Any
+
 from audiostack.helpers.api_item import APIResponseItem
 from audiostack.helpers.api_list import APIResponseList
+from audiostack.helpers.request_interface import RequestInterface
+from audiostack.helpers.request_types import RequestTypes
 
 
 class Script:
     FAMILY = "content"
     interface = RequestInterface(family=FAMILY)
 
     class Item(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
 
             self.scriptId = self.data["scriptId"]
             self.projectName = self.data["projectName"]
             self.moduleName = self.data["moduleName"]
             self.scriptName = self.data["scriptName"]
             self.scriptText = self.data["scriptText"]
 
-        def update(self, scriptText):
+        def update(self, scriptText: str) -> "Script.Item":
             return Script.update(scriptId=self.scriptId, scriptText=scriptText)
 
-        def delete(self):
+        def delete(self) -> APIResponseItem:
             return Script.delete(self.scriptId)
 
     class List(APIResponseList):
-        def __init__(self, response, list_type) -> None:
+        def __init__(self, response: dict, list_type: str) -> None:
             super().__init__(response, list_type)
 
-        def resolve_item(self, list_type, item):
+        def resolve_item(self, list_type: str, item: Any) -> "Script.Item":
             if list_type == "scripts":
                 return Script.Item({"data": item})
             else:
                 raise Exception()
 
     @staticmethod
     def create(
@@ -59,15 +61,15 @@
     def generate_advert(
         product_name: str,
         product_description: str,
         mood: str = "",
         tone: str = "",
         thirdPerson: bool = True,
         adLength: int = 30,
-    ):
+    ) -> APIResponseItem:
         body = {
             "productName": product_name,
             "productDescription": product_description,
             "mood": mood,
             "tone": tone,
             "thirdPerson": thirdPerson,
             "adLength": adLength,
@@ -94,32 +96,35 @@
             route="script",
             path_parameters=path_params,
             query_parameters=query_params,
         )
         return Script.Item(r)
 
     @staticmethod
-    def delete(scriptId: str, version: str = "") -> str:
+    def delete(scriptId: str, version: str = "") -> APIResponseItem:
         path_params = f"{scriptId}/{version}" if version else scriptId
         r = Script.interface.send_request(
             rtype=RequestTypes.DELETE, route="script", path_parameters=path_params
         )
         return APIResponseItem(r)
 
     @staticmethod
-    def update(scriptId: str, scriptText, version: str = "") -> Item:
+    def update(scriptId: str, scriptText: str, version: str = "") -> Item:
         body = {"scriptId": scriptId, "scriptText": scriptText, "version": version}
         r = Script.interface.send_request(
             rtype=RequestTypes.PUT, json=body, route="script"
         )
         return Script.Item(r)
 
     @staticmethod
     def list(
-        projectName="", moduleName: str = "", scriptName: str = "", scriptId: str = ""
+        projectName: str = "",
+        moduleName: str = "",
+        scriptName: str = "",
+        scriptId: str = "",
     ) -> List:
         query_params = {
             "projectName": projectName,
             "moduleName": moduleName,
             "scriptName": scriptName,
             "scriptId": scriptId,
         }
```

### Comparing `audiostack-1.3.1/audiostack/delivery/encoder.py` & `audiostack-2.0.0a0/audiostack/delivery/encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,53 @@
-from audiostack.helpers.request_interface import RequestInterface
-from audiostack.helpers.request_types import RequestTypes
+from typing import Any, Optional
+
 from audiostack.helpers.api_item import APIResponseItem
 from audiostack.helpers.api_list import APIResponseList
+from audiostack.helpers.request_interface import RequestInterface
+from audiostack.helpers.request_types import RequestTypes
+
 
 class Encoder:
     interface = RequestInterface(family="delivery")
 
     class Item(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
             self.url = self.data["url"]
             self.format = self.data["format"]
 
-        def download(self, fileName="default", path="./") -> None:
+        def download(self, fileName: str = "default", path: str = "./") -> None:
             full_name = f"{fileName}.{self.format}"
             RequestInterface.download_url(self.url, destination=path, name=full_name)
 
     class List(APIResponseList):
-        def __init__(self, response, list_type) -> None:
+        def __init__(self, response: dict, list_type: str) -> None:
             super().__init__(response, list_type)
 
-        def resolve_item(self, list_type, item):
+        def resolve_item(self, list_type: str, item: Any) -> "Encoder.Item":
             if list_type == "encodedItems":
-                return Encoder.Item({"data": item})            
+                return Encoder.Item({"data": item})
             else:
                 raise Exception()
 
     @staticmethod
     def encode_mix(
-        preset: str ,
+        preset: str,
         productionId: str = "",
-        productionItem: object = None,
+        productionItem: Optional[Any] = None,
         loudnessPreset: str = "",
         public: bool = False,
         bitRateType: str = "",
-        bitRate: int = None,          
-        sampleRate: int = None,
+        bitRate: Optional[int] = None,
+        sampleRate: Optional[int] = None,
         format: str = "",
-        bitDepth: int = None,
-        channels: int = None,
+        bitDepth: Optional[int] = None,
+        channels: Optional[int] = None,
     ) -> Item:
-        
+
         if productionId and productionItem:
             raise Exception(
                 "productionId or productionItem should be supplied not both"
             )
         if not (productionId or productionItem):
             raise Exception("productionId or productionItem should be supplied")
 
@@ -54,42 +57,42 @@
             except Exception:
                 raise Exception(
                     "supplied productionItem is missing an attribute, productionItem should be type object and a response from Production.Mix"
                 )
         elif productionId:
             if not isinstance(productionId, str):
                 raise Exception("supplied productionId should be a uuid string.")
-        
+
         if not preset:
             raise Exception(
                 "Either a an encoding preset (preset) or a loudness preset (loudnessPreset) should be supplied"
-                )
+            )
 
         body = {
             "productionId": productionId,
             "preset": preset,
             "public": public,
             "bitRateType": bitRateType,
             "bitRate": bitRate,
             "sampleRate": sampleRate,
             "format": format,
             "bitDepth": bitDepth,
             "channels": channels,
-            "loudnessPreset": loudnessPreset
+            "loudnessPreset": loudnessPreset,
         }
         r = Encoder.interface.send_request(
             rtype=RequestTypes.POST, route="encoder", json=body
         )
-        
+
         while r["statusCode"] == 202:
             encoderId = r["data"]["encoderId"]
             r = Encoder.interface.send_request(
                 rtype=RequestTypes.GET, route="encoder", path_parameters=encoderId
             )
         return Encoder.Item(r)
 
     @staticmethod
-    def list_presets() -> Item:
+    def list_presets() -> "Encoder.List":
         r = Encoder.interface.send_request(
             rtype=RequestTypes.GET, route="encoder/presets", path_parameters=""
         )
-        return Encoder.List(response=r, list_type="presets")
+        return Encoder.List(response=r, list_type="presets")
```

### Comparing `audiostack-1.3.1/audiostack/delivery/video.py` & `audiostack-2.0.0a0/audiostack/delivery/video.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,34 @@
+from typing import Any, Optional
+
+from audiostack.helpers.api_item import APIResponseItem
 from audiostack.helpers.request_interface import RequestInterface
 from audiostack.helpers.request_types import RequestTypes
-from audiostack.helpers.api_item import APIResponseItem
+
 
 class Video:
     interface = RequestInterface(family="delivery")
 
     class Item(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
             self.url = self.data["url"]
             self.format = self.data["format"]
 
-        def download(self, fileName="default", path="./") -> None:
+        def download(self, fileName: str = "default", path: str = "./") -> None:
             full_name = f"{fileName}.{self.format}"
             RequestInterface.download_url(self.url, destination=path, name=full_name)
 
     @staticmethod
     def create(
         productionId: str = "",
-        productionItem: object = None,
+        productionItem: Optional[Any] = None,
         public: bool = False,
     ) -> Item:
-        
+
         if productionId and productionItem:
             raise Exception(
                 "productionId or productionItem should be supplied not both"
             )
         if not (productionId or productionItem):
             raise Exception("productionId or productionItem should be supplied")
 
@@ -35,23 +38,22 @@
             except Exception:
                 raise Exception(
                     "supplied productionItem is missing an attribute, productionItem should be type object and a response from Production.Mix"
                 )
         elif productionId:
             if not isinstance(productionId, str):
                 raise Exception("supplied productionId should be a uuid string.")
-        
 
         body = {
             "productionId": productionId,
             "public": public,
         }
         r = Video.interface.send_request(
             rtype=RequestTypes.POST, route="video", json=body
         )
-        
+
         while r["statusCode"] == 202:
             videoId = r["data"]["videoId"]
             r = Video.interface.send_request(
                 rtype=RequestTypes.GET, route="video", path_parameters=videoId
             )
-        return Video.Item(r)
+        return Video.Item(r)
```

### Comparing `audiostack-1.3.1/audiostack/docs/docs.py` & `audiostack-2.0.0a0/audiostack/docs/docs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,18 @@
+from audiostack.helpers.api_item import APIResponseItem
 from audiostack.helpers.request_interface import RequestInterface
 from audiostack.helpers.request_types import RequestTypes
-from audiostack.helpers.api_item import APIResponseItem
-from audiostack.helpers.api_list import APIResponseList
 
 
 class Documentation:
     interface = RequestInterface(family="")
 
     @staticmethod
-    def docs_for_service(service: object) -> dict:
-        service = service.__name__.lower()
+    def docs_for_service(service: object) -> APIResponseItem:
+        service = service.__name__.lower()  # type: ignore
 
         r = Documentation.interface.send_request(
             rtype=RequestTypes.GET,
             route="documentation",
             query_parameters={"route": service},
         )
         return APIResponseItem(r)
```

### Comparing `audiostack-1.3.1/audiostack/helpers/api_item.py` & `audiostack-2.0.0a0/audiostack/helpers/api_item.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import json
+from typing import Union
 
 
 class APIResponseItem:
-    def __init__(self, response):
+    def __init__(self, response: dict) -> None:
         self.response = response
-        
+
         # extra specific fields
         self.status_code = response.get("statusCode", 0)
         self.data = response.get("data", {})
         self.message = response.get("message", "")
         self.meta = response.get("meta", {})
         self.bytes = response.get("bytes", None)
-        
 
-    def print_response(self, indent=0):
+    def print_response(self, indent: int = 0) -> Union[dict, str]:
         if indent:
             return json.dumps(self.response, indent=indent)
         else:
             return self.response
 
     def __str__(self) -> str:
         if self.bytes:
```

### Comparing `audiostack-1.3.1/audiostack/helpers/api_list.py` & `audiostack-2.0.0a0/audiostack/helpers/api_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-import json
+from typing import Any
+
 from .api_item import APIResponseItem
 
 
 class APIResponseList(APIResponseItem):
-    def __init__(self, response, list_type):
+    def __init__(self, response: dict, list_type: str) -> None:
         super().__init__(response)
         self.idx = 0
         self.list_type = list_type
         self.items = self.response["data"][list_type]
 
-    def __iter__(self):
+    def __iter__(self) -> "APIResponseList":
         return self
 
-    def __next__(self):
+    def __next__(self) -> Any:
         self.idx += 1
         try:
             item = self.items[self.idx - 1]
             return self.resolve_item(self.list_type, item)
 
         except IndexError:
             self.idx = 0
-            raise StopIteration  
+            raise StopIteration
 
-    def __getitem__(self, x):
+    def __getitem__(self, x: Any) -> Any:
         if isinstance(x, slice):
-            return [self.resolve_item(self.list_type, x) for x in self.items[x.start: x.stop]]
+            return [
+                self.resolve_item(self.list_type, x)
+                for x in self.items[x.start : x.stop]
+            ]
         else:
             return self.resolve_item(self.list_type, x)
-        
 
     # child classes should override this method, failing to do so will raise an exception!
-    def resolve_item(self, list_type):
+    def resolve_item(self, list_type: str, item: Any) -> Any:
         raise Exception()
```

### Comparing `audiostack-1.3.1/audiostack/helpers/request_interface.py` & `audiostack-2.0.0a0/audiostack/helpers/request_interface.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import json
 import shutil
+from typing import Any, Callable, Dict, Optional, Union
 
 import requests
 
-from audiostack.helpers.util import bcolors
-from audiostack.helpers.response import Response
-from audiostack.helpers.request_types import RequestTypes
-
 import audiostack
+from audiostack.helpers.request_types import RequestTypes
 
 
-def remove_empty(data):
+def remove_empty(data: Any) -> Any:
     if not (isinstance(data, dict) or isinstance(data, list)):
         return data
 
     final_dict = {}
-    for key, val in data.items():
+    for key, val in data.items():  # type: ignore
         if val or isinstance(val, int):  # val = int(0) shoud not be removed
             if isinstance(val, dict):
                 final_dict[key] = remove_empty(val)
             elif isinstance(val, list):
                 final_dict[key] = list(filter(None, [remove_empty(i) for i in val]))
             else:
                 final_dict[key] = val
@@ -29,25 +27,24 @@
 class RequestInterface:
     # disable debug print
     DEBUG_PRINT = False
 
     def __init__(self, family: str) -> None:
         self.family = family
 
-    def make_header(self):
+    def make_header(self) -> dict:
         header = {
             "x-api-key": audiostack.api_key,
-            "x-python-sdk-version": audiostack.sdk_version
+            "x-python-sdk-version": audiostack.sdk_version,
         }
         if audiostack.assume_org_id:
             header["x-assume-org"] = audiostack.assume_org_id
         return header
 
-
-    def resolve_response(self, r):
+    def resolve_response(self, r: Any) -> dict:
         if self.DEBUG_PRINT:
             print(json.dumps(r.json(), indent=4))
         if r.status_code >= 500:
             raise Exception("Internal server error - aborting")
 
         if r.status_code == 403:
             exc = r.json().get("message", "Not authorised - check API key is valid")
@@ -72,32 +69,32 @@
         # else:
         if "meta" in r.json():
             if "creditsUsed" in r.json()["meta"]:
                 audiostack.billing_session += r.json()["meta"]["creditsUsed"]
 
         return {**r.json(), **{"statusCode": r.status_code}}
 
-    def send_upload_request(self, local_path, upload_url):
+    def send_upload_request(self, local_path: str, upload_url: str) -> int:
         with open(local_path, "rb") as data:
             r = requests.put(url=upload_url, data=data)
 
             if r.status_code >= 400:
                 raise Exception("Failed to upload file")
 
             return r.status_code
 
     def send_request(
         self,
-        rtype,
-        route,
-        json=None,
-        path_parameters=None,
-        query_parameters=None,
-        overwrite_base_url=None,
-    ):
+        rtype: str,
+        route: str,
+        json: Optional[dict] = None,
+        path_parameters: Optional[Union[dict, str]] = None,
+        query_parameters: Optional[Union[dict, str]] = None,
+        overwrite_base_url: Optional[str] = None,
+    ) -> Any:
         if overwrite_base_url:
             url = overwrite_base_url
         else:
             if self.family:
                 url = f"{audiostack.api_base}/{self.family}"
             else:
                 url = audiostack.api_base
@@ -111,15 +108,15 @@
         if json:
             json = remove_empty(json)
         if query_parameters:
             query_parameters = remove_empty(query_parameters)
 
         # these requests are all the same input parameters.
         if rtype in [RequestTypes.POST, RequestTypes.PUT, RequestTypes.PATCH]:
-            FUNC_MAP = {
+            FUNC_MAP: Dict[str, Callable] = {
                 RequestTypes.POST: requests.post,
                 RequestTypes.PUT: requests.put,
                 RequestTypes.PATCH: requests.patch,
             }
 
             return self.resolve_response(
                 FUNC_MAP[rtype](url=url, json=json, headers=self.make_header())
@@ -140,15 +137,15 @@
             return self.resolve_response(
                 requests.delete(
                     url=url, params=query_parameters, headers=self.make_header()
                 )
             )
 
     @staticmethod
-    def download_url(url, name, destination):
+    def download_url(url: str, name: str, destination: str) -> None:
         r = requests.get(
             url=url, stream=True, headers={"x-api-key": audiostack.api_key}
         )
 
         if r.status_code >= 400:
             raise Exception("Failed to download file")
```

### Comparing `audiostack-1.3.1/audiostack/production/mix.py` & `audiostack-2.0.0a0/audiostack/production/mix.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,141 +1,152 @@
-from audiostack.helpers.request_interface import RequestInterface
-from audiostack.helpers.request_types import RequestTypes
+from typing import Any, Optional, Union
+
 from audiostack.helpers.api_item import APIResponseItem
 from audiostack.helpers.api_list import APIResponseList
+from audiostack.helpers.request_interface import RequestInterface
+from audiostack.helpers.request_types import RequestTypes
 
 
 class Mix:
     interface = RequestInterface(family="production")
 
     class Item(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
             self.productionId = self.data["productionId"]
 
-        def download(self, fileName="", path="./") -> None:
+        def download(self, fileName: str = "", path: str = "./") -> None:
             sections = self.data["files"]
             for i, s in enumerate(sections):
                 format = s["format"]
                 original_name = s["filename"]
 
                 if not fileName:
                     full_name = f"{original_name}.{format}"
                 else:
                     full_name = f"{fileName}_{i}.{format}"
 
                 RequestInterface.download_url(
                     s["url"], destination=path, name=full_name
                 )
 
-        def delete(self):
+        def delete(self) -> APIResponseItem:
             return Mix.delete(self.productionId)
 
     class List(APIResponseList):
-        def __init__(self, response, list_type) -> None:
+        def __init__(self, response: dict, list_type: str) -> None:
             super().__init__(response, list_type)
 
-        def resolve_item(self, list_type, item):
+        def resolve_item(self, list_type: str, item: Any) -> Union["Mix.Item", None]:
             if list_type == "productionIds":
                 return Mix.Item({"data": item})
             elif list_type == "presets":
-                return
-
+                return None
             else:
                 raise Exception()
 
     @staticmethod
     def create(
-        speechId: str="",
-        scriptId: str="",
-        speechItem=None,
+        speechId: str = "",
+        scriptId: str = "",
+        speechItem: Optional[Any] = None,
         soundTemplate: str = "",
         mediaFiles: dict = {},
         fxFiles: dict = {},
         sectionProperties: dict = {},
         timelineProperties: dict = {},
         masteringPreset: str = "",
         public: bool = False,
         exportSettings: dict = {},
         strictValidation: bool = True,
         validate: bool = False,
-        soundLayer: str = "default"
+        soundLayer: str = "default",
     ) -> Item:
         counts = sum([1 for i in [speechId, scriptId, speechItem] if i])
         if counts != 1:
-            raise Exception("only 1 of the following is required; speechId, speechItem, or scriptId")
-        
+            raise Exception(
+                "only 1 of the following is required; speechId, speechItem, or scriptId"
+            )
+
         if speechItem:
             speechId = speechItem.speechId
 
         if not isinstance(soundTemplate, str):
             raise Exception("soundTemplate argument should be a string")
         if not isinstance(masteringPreset, str):
             raise Exception("masteringPreset should be a string")
-        
 
         body = {
             "soundTemplate": soundTemplate,
             "mediaFiles": mediaFiles,
             "fxFiles": fxFiles,
             "sectionProperties": sectionProperties,
             "timelineProperties": timelineProperties,
             "soundLayer": soundLayer,
             "masteringPreset": masteringPreset,
             "public": public,
-            "exportSettings" : exportSettings,
-            "strictValidation" : strictValidation
+            "exportSettings": exportSettings,
+            "strictValidation": strictValidation,
         }
         if speechId:
             body["speechId"] = speechId
         elif scriptId:
             body["scriptId"] = scriptId
 
         if validate:
-            r = Mix.interface.send_request(rtype=RequestTypes.POST, route="validate", json=body)
+            r = Mix.interface.send_request(
+                rtype=RequestTypes.POST, route="validate", json=body
+            )
         else:
-            r = Mix.interface.send_request(rtype=RequestTypes.POST, route="mix", json=body)
-            
+            r = Mix.interface.send_request(
+                rtype=RequestTypes.POST, route="mix", json=body
+            )
+
         while r["statusCode"] == 202:
             print("Response in progress please wait...")
             r = Mix.interface.send_request(
-                rtype=RequestTypes.GET, route="mix", path_parameters=r["data"]["productionId"]
+                rtype=RequestTypes.GET,
+                route="mix",
+                path_parameters=r["data"]["productionId"],
             )
-        
+
         return Mix.Item(r)
 
     @staticmethod
     def get(productionId: str) -> Item:
         r = Mix.interface.send_request(
             rtype=RequestTypes.GET, route="mix", path_parameters=productionId
         )
         return Mix.Item(r)
 
     @staticmethod
-    def delete(productionId: str) -> str:
+    def delete(productionId: str) -> APIResponseItem:
         r = Mix.interface.send_request(
             rtype=RequestTypes.DELETE, route="mix", path_parameters=productionId
         )
         return APIResponseItem(r)
 
     @staticmethod
     def list(
-        projectName="", moduleName: str = "", scriptName: str = "", scriptId: str = ""
-    ) -> list:
+        projectName: str = "",
+        moduleName: str = "",
+        scriptName: str = "",
+        scriptId: str = "",
+    ) -> "Mix.List":
         query_params = {
             "projectName": projectName,
             "moduleName": moduleName,
             "scriptName": scriptName,
             "scriptId": scriptId,
         }
 
         r = Mix.interface.send_request(
             rtype=RequestTypes.GET, route="mixes", query_parameters=query_params
         )
         return Mix.List(r, list_type="productionIds")
 
     @staticmethod
-    def list_presets() -> Item:
+    def list_presets() -> "Mix.List":
         r = Mix.interface.send_request(
             rtype=RequestTypes.GET, route="mix/presets", path_parameters=""
         )
         return Mix.List(response=r, list_type="presets")
```

### Comparing `audiostack-1.3.1/audiostack/production/sound.py` & `audiostack-2.0.0a0/audiostack/production/sound.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from audiostack.helpers.request_interface import RequestInterface
-from audiostack.helpers.request_types import RequestTypes
+from typing import Any, Union
+
 from audiostack.helpers.api_item import APIResponseItem
 from audiostack.helpers.api_list import APIResponseList
-
-from typing import Union
+from audiostack.helpers.request_interface import RequestInterface
+from audiostack.helpers.request_types import RequestTypes
 
 
 class Sound:
     interface = RequestInterface(family="production/sound")
 
     # ----------------------------------------- TEMPLATE -----------------------------------------
     class Template:
         class Item(APIResponseItem):
-            def __init__(self, response) -> None:
+            def __init__(self, response: dict) -> None:
                 super().__init__(response)
 
                 if "template" in self.data:  #
                     self.data = self.data["template"]
 
         class List(APIResponseList):
-            def __init__(self, response, list_type) -> None:
+            def __init__(self, response: dict, list_type: str) -> None:
                 super().__init__(response, list_type)
 
-            def resolve_item(self, list_type, item):
+            def resolve_item(self, list_type: str, item: Any) -> "Sound.Template.Item":
                 if list_type == "templates":
                     return Sound.Template.Item(
                         {"data": item, "statusCode": self.response["statusCode"]}
                     )
                 else:
                     raise Exception()
 
         @staticmethod
         def select_for_script(
-            scriptId="", scriptItem="", mood: str = ""
+            scriptId: str = "", scriptItem: Any = "", mood: str = ""
         ) -> APIResponseItem:
             if scriptId and scriptItem:
                 raise Exception("scriptId or scriptItem should be supplied not both")
             if not (scriptId or scriptItem):
                 raise Exception("scriptId or scriptItem should be supplied")
 
             if scriptItem:
@@ -62,53 +62,58 @@
 
         @staticmethod
         def list(
             collections: Union[str, list] = "",
             genres: Union[str, list] = "",
             instruments: Union[str, list] = "",
             moods: str = "",
-        ) -> list:
+        ) -> "Sound.Template.List":
             query_params = {
                 "moods": moods,
                 "collections": collections,
                 "instruments": instruments,
                 "genres": genres,
             }
             r = Sound.interface.send_request(
                 rtype=RequestTypes.GET, route="template", query_parameters=query_params
             )
             return Sound.Template.List(r, list_type="templates")
 
-        def create(templateName: str, description: str = ""):
+        @staticmethod
+        def create(templateName: str, description: str = "") -> "Sound.Template.Item":
             body = {"templateName": templateName, "description": description}
             r = Sound.interface.send_request(
                 rtype=RequestTypes.POST, route="template", json=body
             )
             return Sound.Template.Item(r)
 
-        def delete(templateName: str):
+        @staticmethod
+        def delete(templateName: str) -> APIResponseItem:
             r = Sound.interface.send_request(
                 rtype=RequestTypes.DELETE,
                 route="template",
                 path_parameters=templateName,
             )
             return APIResponseItem(r)
 
     # ----------------------------------------- TEMPLATE SEGMENT -----------------------------------------
     class Segment:
-        def create(mediaId: str, templateName: str, soundSegmentName: str):
+        @staticmethod
+        def create(
+            mediaId: str, templateName: str, soundSegmentName: str
+        ) -> "Sound.Template.Item":
             segment = {
                 "templateName": templateName,
                 "segmentName": soundSegmentName,
                 "mediaId": mediaId,
             }
             r = Sound.interface.send_request(
                 rtype=RequestTypes.POST, route="segment", json=segment
             )
             return Sound.Template.Item(r)
 
     # ----------------------------------------- TEMPLATE PARAMETERS -----------------------------------------
     class Parameter:
         @staticmethod
-        def get() -> dict:
+        def get() -> APIResponseItem:
             r = Sound.interface.send_request(rtype=RequestTypes.GET, route="parameter")
             return APIResponseItem(r)
```

### Comparing `audiostack-1.3.1/audiostack/production/suite.py` & `audiostack-2.0.0a0/audiostack/production/suite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,116 +1,134 @@
+from typing import Any, List, Optional, Union
+
+from audiostack.content.file import File
+from audiostack.helpers.api_item import APIResponseItem
 from audiostack.helpers.request_interface import RequestInterface
 from audiostack.helpers.request_types import RequestTypes
-from audiostack.helpers.api_item import APIResponseItem
-from audiostack.content.file import File
-from typing import List, Optional
+
 
 class Suite:
     DENOISE_ENDPOINT = "suite/denoise"
+
     class FailedPipeline(Exception):
         pass
-    
+
     interface = RequestInterface(family="production")
 
     class EvaluationItem(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
 
     class PipelineInProgressItem(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
-            
+
             self.pipelineId = self.data["pipelineId"]
 
     class PipelineFinishedItem(PipelineInProgressItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
             self.newFileIds = self.data["results"]["newFileIds"]
             self.inputFileIds = self.data["results"]["inputFileIds"]
             self.replacedFileIds = self.data["results"]["replacedFileIds"]
-        
+
         def convert_new_files_to_items(self) -> List["File.Item"]:
             return [File.get(f["fileId"]) for f in self.newFileIds]
-        
+
         def convert_replaced_files_to_items(self) -> List["File.Item"]:
             return [File.get(f["fileId"]) for f in self.replacedFileIds]
-        
+
     @staticmethod
     def evaluate(
         fileId: str,
         preset: str = "",
         processes: list = [],
         text: str = "",
         scriptId: str = "",
         language: str = "en-US",
     ) -> EvaluationItem:
         if not (fileId):
             raise Exception("fileId should be supplied")
         if text and scriptId:
-            raise Exception("either text or scriptId or none should be supplied not both")
+            raise Exception(
+                "either text or scriptId or none should be supplied not both"
+            )
         if not isinstance(processes, list):
             raise Exception("processes should be a list")
         if not isinstance(preset, str):
             raise Exception("preset should be a string")
 
         body = {
             "fileId": fileId,
             "preset": preset,
             "processes": processes,
-            "language": language
+            "language": language,
         }
         if text:
             body["text"] = text
         elif scriptId:
             body["scriptId"] = scriptId
-        
-        r = Suite.interface.send_request(rtype=RequestTypes.POST, route="suite/evaluate", json=body)
 
-        while r["statusCode"] != 200 and r["statusCode"] !=404:   # TODO REVISE
+        r = Suite.interface.send_request(
+            rtype=RequestTypes.POST, route="suite/evaluate", json=body
+        )
+
+        while r["statusCode"] != 200 and r["statusCode"] != 404:  # TODO REVISE
             print("Response in progress please wait...")
-            r = Suite.interface.send_request(rtype=RequestTypes.POST, route="suite/evaluate", json=body)
-            
+            r = Suite.interface.send_request(
+                rtype=RequestTypes.POST, route="suite/evaluate", json=body
+            )
+
         return Suite.EvaluationItem(r)
-    
+
     @staticmethod
-    def separate(fileId: str, wait=True):
+    def separate(
+        fileId: str, wait: bool = True
+    ) -> Union["Suite.PipelineInProgressItem", "Suite.PipelineFinishedItem"]:
 
         body = {
             "fileId": fileId,
         }
-        r = Suite.interface.send_request(rtype=RequestTypes.POST, route="suite/separate", json=body)
+        r = Suite.interface.send_request(
+            rtype=RequestTypes.POST, route="suite/separate", json=body
+        )
         item = Suite.PipelineInProgressItem(r)
         return Suite._poll(r, item.pipelineId) if wait else item
-    
-    @staticmethod
-    def denoise(fileId: str, level: Optional[int] = None, wait=True):
 
-        body = {
-            "fileId": fileId,
-            "level": level
-        }
-        r = Suite.interface.send_request(rtype=RequestTypes.POST, route=Suite.DENOISE_ENDPOINT, json=body)
+    @staticmethod
+    def denoise(
+        fileId: str, level: Optional[int] = None, wait: bool = True
+    ) -> Union["Suite.PipelineInProgressItem", "Suite.PipelineFinishedItem"]:
+
+        body = {"fileId": fileId, "level": level}
+        r = Suite.interface.send_request(
+            rtype=RequestTypes.POST, route=Suite.DENOISE_ENDPOINT, json=body
+        )
         item = Suite.PipelineInProgressItem(r)
         return Suite._poll(r, item.pipelineId) if wait else item
-        
 
     @staticmethod
-    def _poll(r, pipelineId: str):
+    def _poll(r: Any, pipelineId: str) -> "Suite.PipelineFinishedItem":
         while r["statusCode"] == 202:
             r = Suite.interface.send_request(
-                rtype=RequestTypes.GET, route="suite/pipeline", path_parameters=pipelineId
+                rtype=RequestTypes.GET,
+                route="suite/pipeline",
+                path_parameters=pipelineId,
             )
-        
+
         status = r.get("data", {}).get("status", 200)
         if status > 400:
             msg = r.get("data", {}).get("message")
             errors = r.get("data", {}).get("errors")
-            raise Suite.FailedPipeline("pipeline failed: ", msg, "errors are as follows: ", ','.join(errors))
-        
-        return Suite.PipelineFinishedItem(r)
+            raise Suite.FailedPipeline(
+                "pipeline failed: ", msg, "errors are as follows: ", ",".join(errors)
+            )
 
+        return Suite.PipelineFinishedItem(r)
 
     @staticmethod
-    def get(pipelineId: str):
-        r = Suite.interface.send_request(rtype=RequestTypes.GET, route="suite/pipeline", path_parameters=pipelineId)
-        
-        return Suite._poll(r, pipelineId)
+    def get(pipelineId: str) -> "Suite.PipelineFinishedItem":
+        r = Suite.interface.send_request(
+            rtype=RequestTypes.GET, route="suite/pipeline", path_parameters=pipelineId
+        )
+
+        return Suite._poll(r, pipelineId)
```

### Comparing `audiostack-1.3.1/audiostack/speech/diction.py` & `audiostack-2.0.0a0/audiostack/speech/diction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,89 @@
-from audiostack.helpers.request_interface import RequestInterface
-from audiostack.helpers.request_types import RequestTypes
+from typing import Any, Union
+
 from audiostack.helpers.api_item import APIResponseItem
 from audiostack.helpers.api_list import APIResponseList
+from audiostack.helpers.request_interface import RequestInterface
+from audiostack.helpers.request_types import RequestTypes
 
 
 class Diction:
     interface = RequestInterface(family="speech/diction")
 
     class Item(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
             self.lang = self.data["lang"]
             self.words = self.data["words"]
             self.wordCategory = self.data.get("wordCategory", "")
             self.content = self.data.get("content", "")
 
     class Word(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
             self.inputs = self.data["inputs"]
             self.replacements = self.data["replacements"]
 
     class List(APIResponseList):
-        def __init__(self, response, list_type) -> None:
+        def __init__(self, response: dict, list_type: str) -> None:
             super().__init__(response, list_type)
 
-        def resolve_item(self, list_type, item):
+        def resolve_item(
+            self, list_type: str, item: Any
+        ) -> Union["Diction.Item", "Diction.Word"]:
             if list_type == "dictionaries":
                 return Diction.Item({"data": item})
             elif list_type == "words":
                 return Diction.Word({"data": item})
             else:
                 raise Exception()
 
     @staticmethod
-    def list() -> list:
+    def list() -> "Diction.List":
         r = Diction.interface.send_request(rtype=RequestTypes.GET, route="")
         return Diction.List(r, "dictionaries")
 
     class Custom:
         @staticmethod
-        def list() -> list:
+        def list() -> "Diction.List":
             r = Diction.interface.send_request(rtype=RequestTypes.GET, route="custom")
             return Diction.List(r, "dictionaries")
 
         @staticmethod
         def create_word(
             word: str,
             replacement: str,
             lang: str = "global",
             specialization: str = "default",
             contentType: str = "basic",
-        ) -> dict:
+        ) -> "Diction.Word":
             body = {
                 "word": word,
                 "replacement": replacement,
                 "lang": lang,
                 "specialization": specialization,
                 "contentType": contentType,
             }
 
             r = Diction.interface.send_request(
                 rtype=RequestTypes.PUT, route="custom/item", json=body
             )
             return Diction.Word(r)
 
         @staticmethod
-        def list_words(lang: str) -> list:
+        def list_words(lang: str) -> "Diction.List":
             r = Diction.interface.send_request(
                 rtype=RequestTypes.GET,
                 route="custom/items",
                 query_parameters={"lang": lang},
             )
             return Diction.List(r, "words")
 
         @staticmethod
-        def delete_word(lang: str, word: str, specialization: str = "") -> list:
+        def delete_word(
+            lang: str, word: str, specialization: str = ""
+        ) -> APIResponseItem:
             query = {"lang": lang, "word": word, "specialization": specialization}
             r = Diction.interface.send_request(
                 rtype=RequestTypes.DELETE, route="custom/item", query_parameters=query
             )
             return APIResponseItem(r)
```

### Comparing `audiostack-1.3.1/audiostack/speech/predict.py` & `audiostack-2.0.0a0/audiostack/speech/predict.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,37 @@
-from audiostack.helpers.request_interface import RequestInterface
-from audiostack.helpers.request_types import RequestTypes
+from typing import Any
+
 from audiostack.helpers.api_item import APIResponseItem
 from audiostack.helpers.api_list import APIResponseList
+from audiostack.helpers.request_interface import RequestInterface
+from audiostack.helpers.request_types import RequestTypes
 
 
 class Predict:
     interface = RequestInterface(family="speech/predict")
 
     class Item(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
 
             self.length = self.data["length"]
 
     class List(APIResponseList):
-        def __init__(self, response, list_type) -> None:
+        def __init__(self, response: dict, list_type: str) -> None:
             super().__init__(response, list_type)
 
-        def resolve_item(self, list_type, item):
+        def resolve_item(self, list_type: str, item: Any) -> "Predict.Item":
             if list_type == "voices":
                 return item
             else:
                 raise Exception()
 
     @staticmethod
-    def list() -> list:
+    def list() -> "Predict.List":
         r = Predict.interface.send_request(rtype=RequestTypes.GET, route="voices")
-    #    return #Predict.List(r, list_type="voices")
         return Predict.List(response=r, list_type="voices")
-    
 
     @staticmethod
-    def predict(text: str, voice: str) -> list:
-        body = {
-            "text" : text,
-            "voice" : voice
-        }
+    def predict(text: str, voice: str) -> "Predict.Item":
+        body = {"text": text, "voice": voice}
         r = Predict.interface.send_request(rtype=RequestTypes.POST, route="", json=body)
-        return Predict.Item(r)
+        return Predict.Item(r)
```

### Comparing `audiostack-1.3.1/audiostack/speech/tts.py` & `audiostack-2.0.0a0/audiostack/speech/tts.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-from audiostack.helpers.request_interface import RequestInterface
-from audiostack.helpers.request_types import RequestTypes
+from typing import Any, Optional
+
 from audiostack.helpers.api_item import APIResponseItem
 from audiostack.helpers.api_list import APIResponseList
+from audiostack.helpers.request_interface import RequestInterface
+from audiostack.helpers.request_types import RequestTypes
 
 
 class TTS:
     interface = RequestInterface(family="speech")
 
     class Item(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
             self.speechId = self.data["speechId"]
 
-        def download(self, autoName=False, fileName="", path="./") -> None:
+        def download(
+            self, autoName: bool = False, fileName: str = "", path: str = "./"
+        ) -> None:
             sections = self.data["sections"]
             for i, s in enumerate(sections):
                 if autoName:
                     full_name = ""
                     for k, val in s["audience"].items():
                         full_name += f"{k}={val}~"
 
@@ -26,176 +30,185 @@
                         full_name = s["sectionName"] + ".wav"
                     else:
                         full_name = f"{fileName}_{i+1}_of_{len(sections)}.wav"
                 RequestInterface.download_url(
                     s["url"], destination=path, name=full_name
                 )
 
-        def delete(self):
+        def delete(self) -> APIResponseItem:
             return TTS.delete(self.speechId)
 
     class BytesItem(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
             self.bytes = response["bytes"]
 
         # def download(self, autoName=False, fileName="default", path="./") -> None:
         #     with open("")
 
     class List(APIResponseList):
-        def __init__(self, response, list_type) -> None:
+        def __init__(self, response: dict, list_type: Any) -> None:
             super().__init__(response, list_type)
 
-        def resolve_item(self, list_type, item):
+        def resolve_item(self, list_type: str, item: Any) -> "TTS.Item":
             if list_type == "speechIds":
                 return TTS.Item({"data": item})
             else:
                 raise Exception()
 
     class Section:
         @staticmethod
         def create(
-            sectionToProduce,
-            scriptId="",
-            scriptItem=None,
+            sectionToProduce: Any,
+            scriptId: str = "",
+            scriptItem: Optional[Any] = None,
             voice: str = "",
             speed: float = 1.0,
             silencePadding: str = "",
             audience: dict = {},
             sections: dict = {},
             voiceIntelligence: bool = False,
             public: bool = False,
             sync: bool = True,
-        ):
+        ) -> "TTS.Item":
             # (start) no modify
             route = "tts/section"
             return TTS._create(**locals())
             # (end) modify
 
     @staticmethod
-    def preview(text: str, voice: str):
+    def preview(text: str, voice: str) -> "TTS.BytesItem":
         body = {"text": text, "voice": voice}
         r = TTS.interface.send_request(
             rtype=RequestTypes.POST, route="tts/preview", json=body
         )
         return TTS.BytesItem(r)
 
     @staticmethod
-    def reduce(speechId: str, targetLength: str, sectionId: str = ""):
+    def reduce(speechId: str, targetLength: str, sectionId: str = "") -> "TTS.Item":
         body = {
             "speechId": speechId,
             "targetLength": targetLength,
             "sectionId": sectionId,
         }
         r = TTS.interface.send_request(
             rtype=RequestTypes.POST, route="tts/reduce", json=body
         )
         print(r)
         return TTS.Item(r)
 
+    @staticmethod
     def remove_padding(
         speechId: str,
         minSilenceDuration: float = 1.5,
         silenceThreshold: float = 0.001,
         position: str = "end",
         sectionId: str = "",
-    ):
+    ) -> "TTS.Item":
         body = {
             "speechId": speechId,
             "minSilenceDuration": minSilenceDuration,
             "silenceThreshold": silenceThreshold,
             "position": position,
             "sectionId": sectionId,
         }
         r = TTS.interface.send_request(
             rtype=RequestTypes.POST, route="tts/remove_padding", json=body
         )
         print(r)
         return TTS.Item(r)
 
     @staticmethod
-    def annotate(speechId: str, scriptReference: str = "", languageCode: str ="", continuousRecognition: bool = False):
+    def annotate(
+        speechId: str,
+        scriptReference: str = "",
+        languageCode: str = "",
+        continuousRecognition: bool = False,
+    ) -> dict:
 
         body = {
             "speechId": speechId,
             "scriptReference": scriptReference,
             "language_code": languageCode,
-            "continuous_recognition": continuousRecognition        
+            "continuous_recognition": continuousRecognition,
         }
         r = TTS.interface.send_request(
             rtype=RequestTypes.POST, route="tts/annotate", json=body
         )
         print(r)
-        return (r)
+        return r
 
     @staticmethod
     def create(
-        scriptId="",
-        scriptItem=None,
+        scriptId: str = "",
+        scriptItem: Optional[Any] = None,
         voice: str = "",
         speed: float = 1.0,
         silencePadding: str = "",
         audience: dict = {},
         sections: dict = {},
         voiceIntelligence: bool = False,
         public: bool = False,
         sync: bool = True,
-    ) -> Item:
+    ) -> "TTS.Item":
         # (start) no modify
         route = "tts"
         return TTS._create(**locals())
         # (end) modify
 
     @staticmethod
-    def get(speechId: str, public: bool = False) -> Item:
+    def get(speechId: str, public: bool = False) -> "TTS.Item":
         r = TTS.interface.send_request(
             rtype=RequestTypes.GET,
             route="tts",
             path_parameters=speechId,
             query_parameters={"public": public},
         )
         return TTS.Item(r)
 
     @staticmethod
-    def delete(speechId: str) -> str:
+    def delete(speechId: str) -> APIResponseItem:
         r = TTS.interface.send_request(
             rtype=RequestTypes.DELETE, route="tts", path_parameters=speechId
         )
         return APIResponseItem(r)
 
     @staticmethod
     def list(
-        projectName="", moduleName: str = "", scriptName: str = "", scriptId: str = ""
-    ) -> list:
+        projectName: str = "",
+        moduleName: str = "",
+        scriptName: str = "",
+        scriptId: str = "",
+    ) -> "TTS.List":
         query_params = {
             "projectName": projectName,
             "moduleName": moduleName,
             "scriptName": scriptName,
             "scriptId": scriptId,
         }
         r = TTS.interface.send_request(
             rtype=RequestTypes.GET, route="tts", query_parameters=query_params
         )
         return TTS.List(r, list_type="speechIds")
 
     @staticmethod
     def _create(
         route: str,
-        scriptId="",
-        scriptItem=None,
+        scriptId: str = "",
+        scriptItem: Optional[Any] = None,
         voice: str = "",
         speed: float = 1.0,
         silencePadding: str = "",
         audience: dict = {},
         sections: dict = {},
         voiceIntelligence: bool = False,
         public: bool = False,
         sync: bool = True,
         sectionToProduce: str = "",
-    ):
+    ) -> "TTS.Item":
         if scriptId and scriptItem:
             raise Exception("scriptId or scriptItem should be supplied not both")
         if not (scriptId or scriptItem):
             raise Exception("scriptId or scriptItem should be supplied")
 
         if scriptItem:
             scriptId = scriptItem.scriptId
```

### Comparing `audiostack-1.3.1/audiostack/speech/voice.py` & `audiostack-2.0.0a0/audiostack/speech/voice.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-from audiostack.helpers.request_interface import RequestInterface
-from audiostack.helpers.request_types import RequestTypes
+from typing import Any
+
 from audiostack.helpers.api_item import APIResponseItem
 from audiostack.helpers.api_list import APIResponseList
+from audiostack.helpers.request_interface import RequestInterface
+from audiostack.helpers.request_types import RequestTypes
 
 
 class Voice:
     interface = RequestInterface(family="speech/voice")
 
     class Item(APIResponseItem):
-        def __init__(self, response) -> None:
+        def __init__(self, response: dict) -> None:
             super().__init__(response)
             self.provider = self.data["provider"]
             self.alias = self.data["alias"]
 
     class List(APIResponseList):
-        def __init__(self, response, list_type) -> None:
+        def __init__(self, response: dict, list_type: str) -> None:
             super().__init__(response, list_type)
 
-        def resolve_item(self, list_type, item):
+        def resolve_item(self, list_type: str, item: Any) -> "Voice.Item":
             if list_type == "voices":
                 return Voice.Item({"data": item})
             else:
                 raise Exception()
 
     @staticmethod
     def select_for_script(
-        scriptId: str = "", scriptItem="", tone: str = "", targetLength: int = 20
-    ):
+        scriptId: str = "", scriptItem: Any = "", tone: str = "", targetLength: int = 20
+    ) -> APIResponseItem:
         if scriptId and scriptItem:
             raise Exception("scriptId or scriptItem should be supplied not both")
         if not (scriptId or scriptItem):
             raise Exception("scriptId or scriptItem should be supplied")
 
         if scriptItem:
             scriptId = scriptItem.scriptId
@@ -39,27 +41,27 @@
 
         r = Voice.interface.send_request(
             rtype=RequestTypes.POST, route="select", json=body
         )
         return APIResponseItem(r)
 
     @staticmethod
-    def select_for_content(content, tone: str = ""):
+    def select_for_content(content: str, tone: str = "") -> APIResponseItem:
         body = {"content": content}
         if tone:
             body["tone"] = tone
 
         r = Voice.interface.send_request(
             rtype=RequestTypes.POST, route="select", json=body
         )
         return APIResponseItem(r)
 
     @staticmethod
-    def list() -> list:
+    def list() -> "Voice.List":
         r = Voice.interface.send_request(rtype=RequestTypes.GET, route="")
         return Voice.List(r, list_type="voices")
 
     class Parameter:
         @staticmethod
-        def get() -> dict:
+        def get() -> APIResponseItem:
             r = Voice.interface.send_request(rtype=RequestTypes.GET, route="parameter")
             return APIResponseItem(r)
```

