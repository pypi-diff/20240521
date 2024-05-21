# Comparing `tmp/africanwhisper-0.9.3.tar.gz` & `tmp/africanwhisper-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "africanwhisper-0.9.3.tar", max compression
+gzip compressed data, was "africanwhisper-0.9.4.tar", last modified: Tue May 21 09:45:51 2024, max compression
```

## Comparing `africanwhisper-0.9.3.tar` & `africanwhisper-0.9.4.tar`

### file list

```diff
@@ -1,38 +1,55 @@
--rw-r--r--   0        0        0     1067 2024-05-02 20:37:57.515738 africanwhisper-0.9.3/LICENSE
--rw-r--r--   0        0        0    11066 2024-05-02 20:37:57.515738 africanwhisper-0.9.3/README.md
--rw-r--r--   0        0        0     1248 2024-05-02 20:37:57.523738 africanwhisper-0.9.3/pyproject.toml
--rw-r--r--   0        0        0       60 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/.dockerignore
--rw-r--r--   0        0        0      361 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/Dockerfile
--rw-r--r--   0        0        0        0 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/__init__.py
--rw-r--r--   0        0        0     7479 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/app.py
--rw-r--r--   0        0        0      538 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/docker-compose.yaml
--rw-r--r--   0        0        0        0 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/__init__.py
--rw-r--r--   0        0        0    18321 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/alignment.py
--rw-r--r--   0        0        0    11001 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/asr.py
--rw-r--r--   0        0        0     4894 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/audio.py
--rw-r--r--   0        0        0     3276 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/diarize.py
--rw-r--r--   0        0        0     3759 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/load_asr_model.py
--rw-r--r--   0        0        0     4271 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/mel_filters.npz
--rw-r--r--   0        0        0     9103 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/subtitles_processor.py
--rw-r--r--   0        0        0     1126 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/types.py
--rw-r--r--   0        0        0    14411 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/utils.py
--rw-r--r--   0        0        0    11354 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/vad.py
--rw-r--r--   0        0        0     2847 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/main.py
--rw-r--r--   0        0        0     3537 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/peft_speech_inference.py
--rw-r--r--   0        0        0     1064 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/deployment/peft_speech_inference_cli.py
--rw-r--r--   0        0        0      136 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/deployment/prometheus.yml
--rw-r--r--   0        0        0      231 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/deployment/requirements.txt
--rw-r--r--   0        0        0     7667 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/deployment/speech_inference.py
--rw-r--r--   0        0        0     2451 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/deployment/speech_inference_cli.py
--rw-r--r--   0        0        0     2027 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/deployment/transcription_model.py
--rw-r--r--   0        0        0        0 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/__init__.py
--rw-r--r--   0        0        0     1910 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/audio_data_processor.py
--rw-r--r--   0        0        0     1986 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/collator.py
--rw-r--r--   0        0        0     4959 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/data_prep.py
--rw-r--r--   0        0        0     1806 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/evaluation.py
--rw-r--r--   0        0        0     2660 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/load_data.py
--rw-r--r--   0        0        0     2592 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/main.py
--rw-r--r--   0        0        0    11165 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/model_trainer.py
--rw-r--r--   0        0        0     7952 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/wandb_callback.py
--rw-r--r--   0        0        0     4336 2024-05-02 20:37:57.539738 africanwhisper-0.9.3/src/training/whisper_model_prep.py
--rw-r--r--   0        0        0    12823 1970-01-01 00:00:00.000000 africanwhisper-0.9.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:45:51.031928 africanwhisper-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-21 09:45:51.031928 africanwhisper-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:45:51.031928 africanwhisper-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:45:51.015928 africanwhisper-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:45:51.023928 africanwhisper-0.9.4/src/africanwhisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-21 09:45:50.000000 africanwhisper-0.9.4/src/africanwhisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-21 09:45:51.000000 africanwhisper-0.9.4/src/africanwhisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:45:50.000000 africanwhisper-0.9.4/src/africanwhisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-21 09:45:51.000000 africanwhisper-0.9.4/src/africanwhisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 09:45:51.000000 africanwhisper-0.9.4/src/africanwhisper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:45:51.015928 africanwhisper-0.9.4/src/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:45:51.019928 africanwhisper-0.9.4/src/deployment/faster_whisper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/faster_whisper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18321 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/faster_whisper/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/faster_whisper/asr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/faster_whisper/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/faster_whisper/diarize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/faster_whisper/load_asr_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/faster_whisper/mel_filters.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/faster_whisper/subtitles_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/faster_whisper/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14411 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/faster_whisper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/faster_whisper/vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/peft_speech_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/peft_speech_inference_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/speech_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/speech_inference_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/deployment/transcription_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:45:51.019928 africanwhisper-0.9.4/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/tests/test_audio_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/tests/test_data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/tests/test_load_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/tests/test_model_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/tests/test_model_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/tests/test_model_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/tests/test_peft_speech_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/tests/test_transcription_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:45:51.023928 africanwhisper-0.9.4/src/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/training/audio_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/training/collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/training/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/training/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/training/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/training/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11166 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/training/model_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/training/wandb_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-21 09:45:47.000000 africanwhisper-0.9.4/src/training/whisper_model_prep.py
```

### Comparing `africanwhisper-0.9.3/LICENSE` & `africanwhisper-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/deployment/app.py` & `africanwhisper-0.9.4/src/deployment/app.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/deployment/faster_whisper/alignment.py` & `africanwhisper-0.9.4/src/deployment/faster_whisper/alignment.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/deployment/faster_whisper/asr.py` & `africanwhisper-0.9.4/src/deployment/faster_whisper/asr.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/deployment/faster_whisper/audio.py` & `africanwhisper-0.9.4/src/deployment/faster_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/deployment/faster_whisper/diarize.py` & `africanwhisper-0.9.4/src/deployment/faster_whisper/diarize.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/deployment/faster_whisper/load_asr_model.py` & `africanwhisper-0.9.4/src/deployment/faster_whisper/load_asr_model.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/deployment/faster_whisper/mel_filters.npz` & `africanwhisper-0.9.4/src/deployment/faster_whisper/mel_filters.npz`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/deployment/faster_whisper/subtitles_processor.py` & `africanwhisper-0.9.4/src/deployment/faster_whisper/subtitles_processor.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/deployment/faster_whisper/types.py` & `africanwhisper-0.9.4/src/deployment/faster_whisper/types.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/deployment/faster_whisper/utils.py` & `africanwhisper-0.9.4/src/deployment/faster_whisper/utils.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/deployment/faster_whisper/vad.py` & `africanwhisper-0.9.4/src/deployment/faster_whisper/vad.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/deployment/main.py` & `africanwhisper-0.9.4/src/deployment/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 from fastapi import FastAPI, UploadFile, HTTPException, Response
 from pydantic import BaseModel
-import tempfile
 from deployment.peft_speech_inference import SpeechInference
 import logging
 from dotenv import load_dotenv
 import uvicorn
 import time
 import prometheus_client
 from prometheus_client import Histogram, Counter
@@ -35,33 +34,22 @@
     logger = logging.getLogger(__name__)
     logging.basicConfig(format='%(asctime)s %(levelname)-8s %(message)s', filename='app.log', level=logging.INFO, datefmt='%Y-%m-%d %H:%M:%S')
     if file is None:
         logger.error("No file provided")
         raise HTTPException(status_code=400, detail="No file provided")
 
     try:
-        with tempfile.NamedTemporaryFile(suffix=".tmp", delete=False) as tmp_file:
-            tmp_file.write(await file.read())
-            tmp_file_path = tmp_file.name
-
-        if file.filename.endswith(".mp3"):
-            logger.info("Processing mp3 file")
-            start_time = time.time()
-            result = inference.output(pipeline, tmp_file_path, task)
-            end_time = time.time()
-            duration = end_time - start_time
-            request_time.observe(duration)
-            logger.info(f"Time taken for inference: {duration} seconds")
-        elif file.filename.endswith(".wav"):
-            logger.info("Processing wav file")
-            pass
-        else:
-            logger.error("Unsupported file format")
-            raise HTTPException(status_code=400, detail="Unsupported file format")
-
+       
+        audio_data = await file.read()
+        logger.info("Processing mp3 file")
+        start_time = time.time()
+        result = inference.output(pipeline, audio_data, task)
+        end_time = time.time()
+        duration = end_time - start_time
+        request_time.observe(duration)
         logger.info("File processed successfully")
         successful_requests_counter.inc()
         return result
     except Exception as e:
         logger.error(f"Error processing file: {str(e)}")
         errors_counter.inc()
         raise HTTPException(status_code=500, detail=f"Error processing file: {str(e)}")
```

### Comparing `africanwhisper-0.9.3/src/deployment/peft_speech_inference.py` & `africanwhisper-0.9.4/src/deployment/peft_speech_inference.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/deployment/peft_speech_inference_cli.py` & `africanwhisper-0.9.4/src/deployment/peft_speech_inference_cli.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/deployment/speech_inference.py` & `africanwhisper-0.9.4/src/deployment/speech_inference.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/deployment/speech_inference_cli.py` & `africanwhisper-0.9.4/src/deployment/speech_inference_cli.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/deployment/transcription_model.py` & `africanwhisper-0.9.4/src/deployment/transcription_model.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/training/audio_data_processor.py` & `africanwhisper-0.9.4/src/training/audio_data_processor.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/training/collator.py` & `africanwhisper-0.9.4/src/training/collator.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/training/data_prep.py` & `africanwhisper-0.9.4/src/training/data_prep.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/training/evaluation.py` & `africanwhisper-0.9.4/src/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/training/load_data.py` & `africanwhisper-0.9.4/src/training/load_data.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/training/main.py` & `africanwhisper-0.9.4/src/training/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,14 +24,26 @@
     parser.add_argument(
         "--dataset_name",
         type=str,
         default="mozilla-foundation/common_voice_16_1",
         help="Name of the dataset to be downloaded from Hugging Face.",
     )
     parser.add_argument(
+        "--train_num_samples",
+        type=int,
+        default=None,
+        help="Number of training samples in the dataset",
+    )
+    parser.add_argument(
+        "--test_num_samples",
+        type=int,
+        default=None,
+        help="Number of testing samples in the dataset",
+    )
+    parser.add_argument(
         "--language_abbr",
         nargs='+',
         required=True,
         help="Abbreviation(s) of the language(s) for the dataset.",
     )
     parser.add_argument(
         "--model_id",
@@ -67,15 +79,19 @@
         language_abbr=args.language_abbr,
         model_id=args.model_id,
         processing_task=args.processing_task,
         use_peft=args.use_peft,
     )
     tokenizer, feature_extractor, feature_processor, model = process.prepare_model()
 
-    dataset = process.load_dataset(feature_extractor, tokenizer, feature_processor)
+    dataset = process.load_dataset(feature_extractor, 
+                                   tokenizer, 
+                                   feature_processor, 
+                                   train_num_samples = args.train_num_samples,
+                                   test_num_samples = args.test_num_samples)
     trainer = Trainer(
         huggingface_write_token=args.huggingface_write_token,
         model_id=args.model_id,
         dataset=dataset,
         model=model,
         feature_processor=feature_processor,
         feature_extractor=feature_extractor,
```

### Comparing `africanwhisper-0.9.3/src/training/model_trainer.py` & `africanwhisper-0.9.4/src/training/model_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
             remove_unused_columns (bool, optional): Whether to remove columns not required by the model when using a dataset. Defaults to False.
             ignore_data_skip (bool, optional): Whether to skip data loading issues when the dataset is being created. Defaults to True.
             **kwargs: Additional keyword arguments to be passed to the `Seq2SeqTrainingArguments` constructor https://huggingface.co/docs/transformers/main_classes/trainer#transformers.Seq2SeqTrainingArguments.
         """
         data_collator = DataCollatorSpeechSeq2SeqWithPadding(
             processor=self.feature_processor
         )
-        output_dir = "../{self.model_id}-finetuned"
+        output_dir = f"../{self.model_id}-finetuned"
         training_args = Seq2SeqTrainingArguments(
             output_dir=output_dir,
             per_device_train_batch_size=per_device_train_batch_size,
             gradient_accumulation_steps=gradient_accumulation_steps,
             learning_rate=learning_rate,
             max_steps=max_steps,
             gradient_checkpointing=gradient_checkpointing,
```

### Comparing `africanwhisper-0.9.3/src/training/wandb_callback.py` & `africanwhisper-0.9.4/src/training/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.3/src/training/whisper_model_prep.py` & `africanwhisper-0.9.4/src/training/whisper_model_prep.py`

 * *Files identical despite different names*

