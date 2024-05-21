# Comparing `tmp/fasttrackpy-0.4.4.tar.gz` & `tmp/fasttrackpy-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttrackpy-0.4.4.tar", max compression
+gzip compressed data, was "fasttrackpy-0.4.5.tar", max compression
```

## Comparing `fasttrackpy-0.4.4.tar` & `fasttrackpy-0.4.5.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     1072 2023-11-15 22:25:59.747254 fasttrackpy-0.4.4/LICENSE
--rw-r--r--   0        0        0      889 2024-03-14 21:53:55.296369 fasttrackpy-0.4.4/README.md
--rw-r--r--   0        0        0     1746 2024-04-25 20:32:54.435824 fasttrackpy-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      629 2023-11-28 04:58:49.197727 fasttrackpy-0.4.4/src/fasttrackpy/__init__.py
--rw-r--r--   0        0        0    17458 2024-04-25 20:32:54.436009 fasttrackpy-0.4.4/src/fasttrackpy/cli.py
--rw-r--r--   0        0        0        0 2023-11-15 22:25:59.749448 fasttrackpy-0.4.4/src/fasttrackpy/patterns/__init__.py
--rw-r--r--   0        0        0     6223 2024-03-22 21:32:36.644068 fasttrackpy-0.4.4/src/fasttrackpy/patterns/audio_textgrid.py
--rw-r--r--   0        0        0     7550 2024-03-22 21:32:36.644304 fasttrackpy-0.4.4/src/fasttrackpy/patterns/corpus.py
--rw-r--r--   0        0        0     7249 2024-03-22 21:32:36.644532 fasttrackpy-0.4.4/src/fasttrackpy/patterns/just_audio.py
--rw-r--r--   0        0        0        0 2023-11-15 22:11:10.457070 fasttrackpy-0.4.4/src/fasttrackpy/processors/__init__.py
--rw-r--r--   0        0        0      844 2023-11-15 22:25:59.749799 fasttrackpy-0.4.4/src/fasttrackpy/processors/aggs.py
--rw-r--r--   0        0        0     1753 2023-11-15 22:25:59.749908 fasttrackpy-0.4.4/src/fasttrackpy/processors/losses.py
--rw-r--r--   0        0        0    13195 2024-04-25 20:32:54.436214 fasttrackpy-0.4.4/src/fasttrackpy/processors/outputs.py
--rw-r--r--   0        0        0     3285 2024-04-15 14:21:09.838641 fasttrackpy-0.4.4/src/fasttrackpy/processors/smoothers.py
--rw-r--r--   0        0        0        0 2023-11-27 01:47:20.549781 fasttrackpy-0.4.4/src/fasttrackpy/resources/config.yml
--rw-r--r--   0        0        0    20530 2024-04-25 20:32:54.436369 fasttrackpy-0.4.4/src/fasttrackpy/tracks.py
--rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 fasttrackpy-0.4.4/setup.py
--rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 fasttrackpy-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-11-15 22:25:59.747254 fasttrackpy-0.4.5/LICENSE
+-rw-r--r--   0        0        0     1617 2024-05-21 16:47:49.547057 fasttrackpy-0.4.5/README.md
+-rw-r--r--   0        0        0     1746 2024-05-21 16:47:49.548166 fasttrackpy-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0      629 2023-11-28 04:58:49.197727 fasttrackpy-0.4.5/src/fasttrackpy/__init__.py
+-rw-r--r--   0        0        0    17458 2024-04-25 20:32:54.436009 fasttrackpy-0.4.5/src/fasttrackpy/cli.py
+-rw-r--r--   0        0        0        0 2023-11-15 22:25:59.749448 fasttrackpy-0.4.5/src/fasttrackpy/patterns/__init__.py
+-rw-r--r--   0        0        0     6455 2024-05-21 16:47:49.548507 fasttrackpy-0.4.5/src/fasttrackpy/patterns/audio_textgrid.py
+-rw-r--r--   0        0        0     8109 2024-05-21 16:47:49.548720 fasttrackpy-0.4.5/src/fasttrackpy/patterns/corpus.py
+-rw-r--r--   0        0        0     7464 2024-05-21 16:47:49.548926 fasttrackpy-0.4.5/src/fasttrackpy/patterns/just_audio.py
+-rw-r--r--   0        0        0        0 2023-11-15 22:11:10.457070 fasttrackpy-0.4.5/src/fasttrackpy/processors/__init__.py
+-rw-r--r--   0        0        0      844 2023-11-15 22:25:59.749799 fasttrackpy-0.4.5/src/fasttrackpy/processors/aggs.py
+-rw-r--r--   0        0        0     1753 2023-11-15 22:25:59.749908 fasttrackpy-0.4.5/src/fasttrackpy/processors/losses.py
+-rw-r--r--   0        0        0    13195 2024-05-21 16:47:49.549143 fasttrackpy-0.4.5/src/fasttrackpy/processors/outputs.py
+-rw-r--r--   0        0        0     3285 2024-05-13 16:24:10.932141 fasttrackpy-0.4.5/src/fasttrackpy/processors/smoothers.py
+-rw-r--r--   0        0        0        0 2023-11-27 01:47:20.549781 fasttrackpy-0.4.5/src/fasttrackpy/resources/config.yml
+-rw-r--r--   0        0        0    20530 2024-05-21 15:07:51.285028 fasttrackpy-0.4.5/src/fasttrackpy/tracks.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:47:49.549179 fasttrackpy-0.4.5/src/fasttrackpy/utils/__init__.py
+-rw-r--r--   0        0        0     1751 2024-05-21 16:47:49.549349 fasttrackpy-0.4.5/src/fasttrackpy/utils/safely.py
+-rw-r--r--   0        0        0     3252 1970-01-01 00:00:00.000000 fasttrackpy-0.4.5/setup.py
+-rw-r--r--   0        0        0     2978 1970-01-01 00:00:00.000000 fasttrackpy-0.4.5/PKG-INFO
```

### Comparing `fasttrackpy-0.4.4/LICENSE` & `fasttrackpy-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.4/README.md` & `fasttrackpy-0.4.5/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,48 @@
 # FastTrackPy
 [![PyPI](https://img.shields.io/pypi/v/fasttrackpy)](https://pypi.org/project/fasttrackpy/)
 [![Python CI](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [![codecov](https://codecov.io/gh/FastTrackiverse/fasttrackpy/graph/badge.svg?token=GOAWY4B5C8)](https://codecov.io/gh/FastTrackiverse/fasttrackpy) <a href="https://codeclimate.com/github/JoFrhwld/fasttrackpy/maintainability"><img src="https://api.codeclimate.com/v1/badges/6725fded174b21a3c59f/maintainability" /></a> [![DOI](https://zenodo.org/badge/580169086.svg)](https://zenodo.org/badge/latestdoi/580169086)
 
 
-Goal: A FastTrack python implementation with importable modules
+A python implementation of the FastTrack method
 
 ## Installation
 
 ```bash
 pip install fasttrackpy
 ```
 
+This will make the command line executable `fasttrack` available, along with its subcommands:
+
+- `audio`
+- `audio-textgrid`
+- `corpus`
+
+## Getting help
+
+For any of the fasttrack subcommands, add the `--help` flag to
+print the help info. You can also visit [the docs](https://fasttrackiverse.github.io/fasttrackpy/usage/getting_started.html).
+
 ## Usage
 
+For a single audio file containing a vowel-like sound:
+
+```bash
+fasttrack audio --file audio.wav \
+    --output formants.csv
+```
+
+For a paired audio file and textgrid with intervals defining
+target audio to process:
+
 ```bash
-fasttrack --file audio.wav --output formants.csv
+fasttrack audio-textgrid --audio audio.wav \
+    --textgrid audio.TextGrid \
+    --output formants.csv
 ```
+
+For a corpus directory of paired audio files and textgrid
+
+```bash
+fasttrack corpus --corpus dir/ \
+    --output formants.csv
+```
```

#### html2text {}

```diff
@@ -2,10 +2,19 @@
 pypi.org/project/fasttrackpy/) [![Python CI](https://github.com/JoFrhwld/
 fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/
 JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [![codecov](https://
 codecov.io/gh/FastTrackiverse/fasttrackpy/graph/badge.svg?token=GOAWY4B5C8)]
 (https://codecov.io/gh/FastTrackiverse/fasttrackpy) _[_h_t_t_p_s_:_/_/
 _a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_6_7_2_5_f_d_e_d_1_7_4_b_2_1_a_3_c_5_9_f_/_m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_][![DOI]
 (https://zenodo.org/badge/580169086.svg)](https://zenodo.org/badge/latestdoi/
-580169086) Goal: A FastTrack python implementation with importable modules ##
-Installation ```bash pip install fasttrackpy ``` ## Usage ```bash fasttrack --
-file audio.wav --output formants.csv ```
+580169086) A python implementation of the FastTrack method ## Installation
+```bash pip install fasttrackpy ``` This will make the command line executable
+`fasttrack` available, along with its subcommands: - `audio` - `audio-textgrid`
+- `corpus` ## Getting help For any of the fasttrack subcommands, add the `--
+help` flag to print the help info. You can also visit [the docs](https://
+fasttrackiverse.github.io/fasttrackpy/usage/getting_started.html). ## Usage For
+a single audio file containing a vowel-like sound: ```bash fasttrack audio --
+file audio.wav \ --output formants.csv ``` For a paired audio file and textgrid
+with intervals defining target audio to process: ```bash fasttrack audio-
+textgrid --audio audio.wav \ --textgrid audio.TextGrid \ --output formants.csv
+``` For a corpus directory of paired audio files and textgrid ```bash fasttrack
+corpus --corpus dir/ \ --output formants.csv ```
```

### Comparing `fasttrackpy-0.4.4/pyproject.toml` & `fasttrackpy-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fasttrackpy"
-version = "0.4.4"
+version = "0.4.5"
 description = "A python implementation of FastTrack"
 authors = [
     "JoFrhwld <JoFrhwld@gmail.com>",
     "santiagobarreda <sbarreda@ucdavis.edu>"
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `fasttrackpy-0.4.4/src/fasttrackpy/__init__.py` & `fasttrackpy-0.4.5/src/fasttrackpy/__init__.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.4/src/fasttrackpy/cli.py` & `fasttrackpy-0.4.5/src/fasttrackpy/cli.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.4/src/fasttrackpy/patterns/audio_textgrid.py` & `fasttrackpy-0.4.5/src/fasttrackpy/patterns/audio_textgrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import parselmouth as pm
 from aligned_textgrid import AlignedTextGrid, Word, Phone, SequenceInterval, SequenceTier
 import aligned_textgrid
 from fasttrackpy import CandidateTracks, Smoother, Loss, Agg
 from fasttrackpy.patterns.just_audio import create_audio_checker
+from fasttrackpy.utils.safely import safely, filter_nones
 import re
 
 from pathlib import Path
 from tqdm import tqdm
 from joblib import Parallel, cpu_count, delayed
 import warnings
 
@@ -61,14 +62,15 @@
         if re.match(target_labels, interval.label) and
         (interval.end - interval.start) > min_duration
     ]
 
     return intervals
 
 @delayed
+@safely(message="There was a problem getting some candidate tracks.")
 def get_candidates(args_dict):
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         candidates =  CandidateTracks(**args_dict)
     if candidates.winner.formants.shape[1] == 1:
         warnings.warn("formant tracking error")
     return candidates
@@ -166,14 +168,15 @@
         } for x, interval in zip(sound_parts, target_intervals)
     ]
     
     n_jobs = cpu_count()
     candidate_list = Parallel(n_jobs=n_jobs)(
         get_candidates(args_dict=arg) for arg in tqdm(arg_list)
         )
+    candidate_list, target_intervals = filter_nones(candidate_list, [candidate_list, target_intervals])
     for cand, interval in zip(candidate_list, target_intervals):
         cand.interval = interval
         cand.file_name = Path(str(audio_path)).stem
 
     return candidate_list
```

### Comparing `fasttrackpy-0.4.4/src/fasttrackpy/patterns/corpus.py` & `fasttrackpy-0.4.5/src/fasttrackpy/patterns/corpus.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import parselmouth as pm
 from aligned_textgrid import AlignedTextGrid, Word, Phone, SequenceInterval, SequenceTier
 import aligned_textgrid
 from fasttrackpy import CandidateTracks, Smoother, Loss, Agg
 from fasttrackpy.patterns.just_audio import create_audio_checker
 from fasttrackpy.patterns.audio_textgrid import get_interval_classes
+from fasttrackpy.utils.safely import safely, filter_nones
 import re
 from collections import namedtuple
 from pathlib import Path
 from tqdm import tqdm
 from functools import reduce
 from operator import add
 from joblib import Parallel, cpu_count, delayed
@@ -82,27 +83,42 @@
     
     raise Exception(f"Could not {target_tier} target tier in textgrid")
 
 def get_target_intervals(
         target_tiers: list[SequenceTier],
         target_labels:str = "[AEIOU]",
         min_duration = 0.05
-        ):
+        )->list[SequenceInterval]:
     intervals = [
         interval 
         for tier in target_tiers 
         for interval in tier
         if re.match(target_labels, interval.label) and
         (interval.end - interval.start) > min_duration
     ]
     [setattr(interval, "wav", interval.intier.wav) for interval in intervals]
 
     return intervals
 
+@safely(message = "There was a problem extracting some sounds.")
+def get_sound_parts(
+        intervals: list[SequenceInterval],
+        window_length: float
+):
+    sound = pm.Sound(str(intervals[0].wav))
+    sound_parts = [
+        sound.extract_part(from_time = interval.start-(window_length/2), 
+        to_time = interval.end+(window_length/2))
+        for interval in intervals
+    ]
+
+    return sound_parts
+
 @delayed
+@safely(message = "There was a problem getting some candidate tracks.")
 def get_candidates(args_dict):
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         candidates =  CandidateTracks(**args_dict)
     if candidates.winner.formants.shape[1] == 1:
         warnings.warn("formant tracking error")
     return candidates
@@ -172,20 +188,16 @@
                              target_labels=target_labels, 
                              min_duration=min_duration
                              )
             for tiers in all_tiers
         ]
     all_candidates = []
     for intervals in all_intervals:
-        sound = pm.Sound(str(intervals[0].wav))
-        sound_parts = [
-            sound.extract_part(from_time = interval.start-(window_length/2), 
-            to_time = interval.end+(window_length/2))
-            for interval in intervals
-        ]
+        sound_parts = get_sound_parts(intervals, window_length)
+        sound_parts, intervals = filter_nones(sound_parts, [sound_parts, intervals])
 
         arg_list = [
             {
                 "samples": x.values,
                 "sampling_frequency": x.sampling_frequency,
                 "xmin": x.xmin,
                 #"interval": interval,
@@ -203,13 +215,14 @@
         ]
 
         n_jobs = cpu_count()
         candidate_list = Parallel(n_jobs=n_jobs)(
             get_candidates(args_dict=arg) for arg in tqdm(arg_list)
             )
 
+        candidate_list, intervals = filter_nones(candidate_list, [candidate_list, intervals])
         for cand, interval in zip(candidate_list, intervals):
             cand.interval = interval
             cand.file_name = Path(str(interval.wav)).stem
         all_candidates += candidate_list
     
     return all_candidates
```

### Comparing `fasttrackpy-0.4.4/src/fasttrackpy/patterns/just_audio.py` & `fasttrackpy-0.4.5/src/fasttrackpy/patterns/just_audio.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Union
 from collections.abc import Callable
 import parselmouth as pm
 from fasttrackpy import CandidateTracks,\
                         Smoother,\
                         Loss,\
                         Agg
+from fasttrackpy.utils.safely import safely, filter_nones
 
 from tqdm import tqdm
 from joblib import Parallel, cpu_count, delayed
 
 try:
     import magic
     no_magic = False
@@ -132,14 +133,15 @@
         loss_fun=loss_fun,
         agg_fun=agg_fun
     )
     candidates.file_name = Path(str(path)).name
     return candidates
 
 @delayed
+@safely(message = "There was a problem processing an audio file.")
 def wrapped_audio(args_dict):
     return process_audio_file(**args_dict)
 
 def process_directory(
         path: str|Path,
         min_max_formant:float = 4000,
         max_max_formant:float = 7000,
@@ -201,12 +203,13 @@
             for x in all_audio
     ]
     n_jobs = cpu_count()
 
     all_candidates = Parallel(n_jobs=n_jobs)(
         wrapped_audio(args_dict=arg) for arg in tqdm(arg_list)
         )
+    all_candidates, all_audio = filter_nones(all_candidates, [all_candidates, all_audio])
     for x, path in zip(all_candidates, all_audio):
         x.file_name = Path(str(path)).name
 
     return all_candidates
```

### Comparing `fasttrackpy-0.4.4/src/fasttrackpy/processors/aggs.py` & `fasttrackpy-0.4.5/src/fasttrackpy/processors/aggs.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.4/src/fasttrackpy/processors/losses.py` & `fasttrackpy-0.4.5/src/fasttrackpy/processors/losses.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.4/src/fasttrackpy/processors/outputs.py` & `fasttrackpy-0.4.5/src/fasttrackpy/processors/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     ]
     param_df = pl.DataFrame(
         data = self.parameters,schema=schema
     )
 
     param_df = param_df.with_columns(
         error = pl.lit(self.smooth_error)
-    ).with_row_count(name = "param")
+    ).with_row_index(name = "param")
 
     param_df = add_metadata(self, param_df)
 
     return param_df
 
 def log_param_to_dataframe(self):
     """Return data as a data frame
@@ -113,15 +113,15 @@
     ]
     param_df = pl.DataFrame(
         data = self.log_parameters,schema=schema
     )
 
     param_df = param_df.with_columns(
         error = pl.lit(self.smooth_error)
-    ).with_row_count(name = "param")
+    ).with_row_index(name = "param")
 
     param_df = add_metadata(self, param_df)
 
     return param_df
 
 def get_big_df(self, output):
         all_df = [x.to_df(output = output) for x in self.candidates]
```

### Comparing `fasttrackpy-0.4.4/src/fasttrackpy/processors/smoothers.py` & `fasttrackpy-0.4.5/src/fasttrackpy/processors/smoothers.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.4/src/fasttrackpy/tracks.py` & `fasttrackpy-0.4.5/src/fasttrackpy/tracks.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.4/setup.py` & `fasttrackpy-0.4.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
-['fasttrackpy', 'fasttrackpy.patterns', 'fasttrackpy.processors']
+['fasttrackpy',
+ 'fasttrackpy.patterns',
+ 'fasttrackpy.processors',
+ 'fasttrackpy.utils']
 
 package_data = \
 {'': ['*'], 'fasttrackpy': ['resources/*']}
 
 install_requires = \
 ['aligned-textgrid>=0.6.2,<0.7.0',
  'click>=8.1.7,<9.0.0',
@@ -30,17 +33,17 @@
  ':sys_platform == "win32"': ['python-magic-bin>=0.4.14,<0.5.0']}
 
 entry_points = \
 {'console_scripts': ['fasttrack = fasttrackpy.cli:fasttrack']}
 
 setup_kwargs = {
     'name': 'fasttrackpy',
-    'version': '0.4.4',
+    'version': '0.4.5',
     'description': 'A python implementation of FastTrack',
-    'long_description': '# FastTrackPy\n[![PyPI](https://img.shields.io/pypi/v/fasttrackpy)](https://pypi.org/project/fasttrackpy/)\n[![Python CI](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [![codecov](https://codecov.io/gh/FastTrackiverse/fasttrackpy/graph/badge.svg?token=GOAWY4B5C8)](https://codecov.io/gh/FastTrackiverse/fasttrackpy) <a href="https://codeclimate.com/github/JoFrhwld/fasttrackpy/maintainability"><img src="https://api.codeclimate.com/v1/badges/6725fded174b21a3c59f/maintainability" /></a> [![DOI](https://zenodo.org/badge/580169086.svg)](https://zenodo.org/badge/latestdoi/580169086)\n\n\nGoal: A FastTrack python implementation with importable modules\n\n## Installation\n\n```bash\npip install fasttrackpy\n```\n\n## Usage\n\n```bash\nfasttrack --file audio.wav --output formants.csv\n```\n',
+    'long_description': '# FastTrackPy\n[![PyPI](https://img.shields.io/pypi/v/fasttrackpy)](https://pypi.org/project/fasttrackpy/)\n[![Python CI](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [![codecov](https://codecov.io/gh/FastTrackiverse/fasttrackpy/graph/badge.svg?token=GOAWY4B5C8)](https://codecov.io/gh/FastTrackiverse/fasttrackpy) <a href="https://codeclimate.com/github/JoFrhwld/fasttrackpy/maintainability"><img src="https://api.codeclimate.com/v1/badges/6725fded174b21a3c59f/maintainability" /></a> [![DOI](https://zenodo.org/badge/580169086.svg)](https://zenodo.org/badge/latestdoi/580169086)\n\n\nA python implementation of the FastTrack method\n\n## Installation\n\n```bash\npip install fasttrackpy\n```\n\nThis will make the command line executable `fasttrack` available, along with its subcommands:\n\n- `audio`\n- `audio-textgrid`\n- `corpus`\n\n## Getting help\n\nFor any of the fasttrack subcommands, add the `--help` flag to\nprint the help info. You can also visit [the docs](https://fasttrackiverse.github.io/fasttrackpy/usage/getting_started.html).\n\n## Usage\n\nFor a single audio file containing a vowel-like sound:\n\n```bash\nfasttrack audio --file audio.wav \\\n    --output formants.csv\n```\n\nFor a paired audio file and textgrid with intervals defining\ntarget audio to process:\n\n```bash\nfasttrack audio-textgrid --audio audio.wav \\\n    --textgrid audio.TextGrid \\\n    --output formants.csv\n```\n\nFor a corpus directory of paired audio files and textgrid\n\n```bash\nfasttrack corpus --corpus dir/ \\\n    --output formants.csv\n```',
     'author': 'JoFrhwld',
     'author_email': 'JoFrhwld@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://fasttrackiverse.github.io/fasttrackpy/',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,31 +1,41 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['fasttrackpy', 'fasttrackpy.patterns',
-'fasttrackpy.processors'] package_data = \ {'': ['*'], 'fasttrackpy':
-['resources/*']} install_requires = \ ['aligned-textgrid>=0.6.2,<0.7.0',
-'click>=8.1.7,<9.0.0', 'cloup>=3.0.3,<4.0.0', 'joblib>=1.3.2,<2.0.0',
-'matplotlib>=3.8.2,<4.0.0', 'polars>=0.20.18,<0.21.0', 'praat-
-parselmouth>=0.4.3,<0.5.0', 'pytest-cov>=4.1.0,<5.0.0', 'pytest>=7.4.3,<8.0.0',
-'pyyaml>=6.0.1,<7.0.0', 'tqdm>=4.66.1,<5.0.0'] extras_require = \ {':
-python_version >= "3.10" and python_version < "3.12"': ['scipy>=1.11.3,<2.0.0',
-'numpy>=1.26.1,<2.0.0'], ':sys_platform != "win32"': ['python-
-magic>=0.4.27,<0.5.0'], ':sys_platform == "win32"': ['python-magic-
+'fasttrackpy.processors', 'fasttrackpy.utils'] package_data = \ {'': ['*'],
+'fasttrackpy': ['resources/*']} install_requires = \ ['aligned-
+textgrid>=0.6.2,<0.7.0', 'click>=8.1.7,<9.0.0', 'cloup>=3.0.3,<4.0.0',
+'joblib>=1.3.2,<2.0.0', 'matplotlib>=3.8.2,<4.0.0', 'polars>=0.20.18,<0.21.0',
+'praat-parselmouth>=0.4.3,<0.5.0', 'pytest-cov>=4.1.0,<5.0.0',
+'pytest>=7.4.3,<8.0.0', 'pyyaml>=6.0.1,<7.0.0', 'tqdm>=4.66.1,<5.0.0']
+extras_require = \ {':python_version >= "3.10" and python_version < "3.12"':
+['scipy>=1.11.3,<2.0.0', 'numpy>=1.26.1,<2.0.0'], ':sys_platform != "win32"':
+['python-magic>=0.4.27,<0.5.0'], ':sys_platform == "win32"': ['python-magic-
 bin>=0.4.14,<0.5.0']} entry_points = \ {'console_scripts': ['fasttrack =
 fasttrackpy.cli:fasttrack']} setup_kwargs = { 'name': 'fasttrackpy', 'version':
-'0.4.4', 'description': 'A python implementation of FastTrack',
+'0.4.5', 'description': 'A python implementation of FastTrack',
 'long_description': '# FastTrackPy\n[![PyPI](https://img.shields.io/pypi/v/
 fasttrackpy)](https://pypi.org/project/fasttrackpy/)\n[![Python CI](https://
 github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)]
 (https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [!
 [codecov](https://codecov.io/gh/FastTrackiverse/fasttrackpy/graph/
 badge.svg?token=GOAWY4B5C8)](https://codecov.io/gh/FastTrackiverse/fasttrackpy)
 _[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_6_7_2_5_f_d_e_d_1_7_4_b_2_1_a_3_c_5_9_f_/_m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_][!
 [DOI](https://zenodo.org/badge/580169086.svg)](https://zenodo.org/badge/
-latestdoi/580169086)\n\n\nGoal: A FastTrack python implementation with
-importable modules\n\n## Installation\n\n```bash\npip install
-fasttrackpy\n```\n\n## Usage\n\n```bash\nfasttrack --file audio.wav --output
-formants.csv\n```\n', 'author': 'JoFrhwld', 'author_email':
-'JoFrhwld@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
-'https://fasttrackiverse.github.io/fasttrackpy/', 'package_dir': package_dir,
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'extras_require': extras_require, 'entry_points':
-entry_points, 'python_requires': '>=3.10,<3.12', } setup(**setup_kwargs)
+latestdoi/580169086)\n\n\nA python implementation of the FastTrack method\n\n##
+Installation\n\n```bash\npip install fasttrackpy\n```\n\nThis will make the
+command line executable `fasttrack` available, along with its subcommands:\n\n-
+`audio`\n- `audio-textgrid`\n- `corpus`\n\n## Getting help\n\nFor any of the
+fasttrack subcommands, add the `--help` flag to\nprint the help info. You can
+also visit [the docs](https://fasttrackiverse.github.io/fasttrackpy/usage/
+getting_started.html).\n\n## Usage\n\nFor a single audio file containing a
+vowel-like sound:\n\n```bash\nfasttrack audio --file audio.wav \\\n --output
+formants.csv\n```\n\nFor a paired audio file and textgrid with intervals
+defining\ntarget audio to process:\n\n```bash\nfasttrack audio-textgrid --audio
+audio.wav \\\n --textgrid audio.TextGrid \\\n --output formants.csv\n```\n\nFor
+a corpus directory of paired audio files and textgrid\n\n```bash\nfasttrack
+corpus --corpus dir/ \\\n --output formants.csv\n```', 'author': 'JoFrhwld',
+'author_email': 'JoFrhwld@gmail.com', 'maintainer': 'None', 'maintainer_email':
+'None', 'url': 'https://fasttrackiverse.github.io/fasttrackpy/', 'package_dir':
+package_dir, 'packages': packages, 'package_data': package_data,
+'install_requires': install_requires, 'extras_require': extras_require,
+'entry_points': entry_points, 'python_requires': '>=3.10,<3.12', } setup
+(**setup_kwargs)
```

