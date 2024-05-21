# Comparing `tmp/scoda-2.1b1.tar.gz` & `tmp/scoda-2.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-2.1b1.tar", last modified: Tue Apr  9 11:36:46 2024, max compression
+gzip compressed data, was "scoda-2.1b2.tar", last modified: Tue May 21 15:01:16 2024, max compression
```

## Comparing `scoda-2.1b1.tar` & `scoda-2.1b2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.694118 scoda-2.1b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 11:36:42.000000 scoda-2.1b1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-09 11:36:46.694118 scoda-2.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-09 11:36:42.000000 scoda-2.1b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-09 11:36:42.000000 scoda-2.1b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.686118 scoda-2.1b1/scoda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.690118 scoda-2.1b1/scoda/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/config/settings.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.690118 scoda-2.1b1/scoda/elements/
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/elements/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/elements/composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/elements/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/elements/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.690118 scoda-2.1b1/scoda/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/exceptions/bar_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/exceptions/sequence_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/exceptions/tokenisation_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/exceptions/track_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.690118 scoda-2.1b1/scoda/midi/
--rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/midi/midi_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/midi/midi_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/midi/midi_track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.690118 scoda-2.1b1/scoda/misc/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/misc/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/misc/enumerations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/misc/music_theory.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/misc/scoda_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/misc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.694118 scoda-2.1b1/scoda/sequences/
--rw-r--r--   0 runner    (1001) docker     (127)    21873 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/sequences/absolute_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/sequences/abstract_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    35040 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/sequences/relative_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    23636 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/sequences/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.694118 scoda-2.1b1/scoda/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/settings/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.694118 scoda-2.1b1/scoda/tokenisation/
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/tokenisation/base_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/tokenisation/gridlike_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/tokenisation/midilike_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    25748 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/tokenisation/notelike_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/tokenisation/transposed_notelike_tokenisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.694118 scoda-2.1b1/scoda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-09 11:36:46.000000 scoda-2.1b1/scoda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-09 11:36:46.000000 scoda-2.1b1/scoda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:36:46.000000 scoda-2.1b1/scoda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 11:36:46.000000 scoda-2.1b1/scoda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 11:36:46.000000 scoda-2.1b1/scoda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:36:46.694118 scoda-2.1b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.382685 scoda-2.1b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-21 15:01:11.000000 scoda-2.1b2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-21 15:01:16.382685 scoda-2.1b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-21 15:01:11.000000 scoda-2.1b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-21 15:01:11.000000 scoda-2.1b2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.374685 scoda-2.1b2/scoda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.378685 scoda-2.1b2/scoda/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/config/settings.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.378685 scoda-2.1b2/scoda/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/elements/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/elements/composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/elements/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/elements/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.378685 scoda-2.1b2/scoda/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/exceptions/bar_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/exceptions/sequence_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/exceptions/tokenisation_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/exceptions/track_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.378685 scoda-2.1b2/scoda/midi/
+-rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/midi/midi_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/midi/midi_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/midi/midi_track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.378685 scoda-2.1b2/scoda/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/misc/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/misc/enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/misc/music_theory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/misc/scoda_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/misc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.382685 scoda-2.1b2/scoda/sequences/
+-rw-r--r--   0 runner    (1001) docker     (127)    21873 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/sequences/absolute_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/sequences/abstract_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35040 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/sequences/relative_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23976 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/sequences/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.382685 scoda-2.1b2/scoda/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/settings/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.382685 scoda-2.1b2/scoda/tokenisation/
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/tokenisation/base_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/tokenisation/gridlike_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/tokenisation/midilike_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25748 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/tokenisation/notelike_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/tokenisation/transposed_notelike_tokenisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.382685 scoda-2.1b2/scoda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-21 15:01:16.000000 scoda-2.1b2/scoda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-21 15:01:16.000000 scoda-2.1b2/scoda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:01:16.000000 scoda-2.1b2/scoda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-21 15:01:16.000000 scoda-2.1b2/scoda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 15:01:16.000000 scoda-2.1b2/scoda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:01:16.382685 scoda-2.1b2/setup.cfg
```

### Comparing `scoda-2.1b1/LICENSE.md` & `scoda-2.1b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/PKG-INFO` & `scoda-2.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda
-Version: 2.1b1
+Version: 2.1b2
 Summary: A MIDI and music data manipulation library
 Author-email: Felix Schön <schoen@kr.tuwien.ac.at>
 License: MIT License
         
         Copyright (c) 2023 Felix Schön
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `scoda-2.1b1/README.md` & `scoda-2.1b2/README.md`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/pyproject.toml` & `scoda-2.1b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "scoda"
-version = "2.1-beta.1"
+version = "2.1-beta.2"
 authors = [{ name = "Felix Schön", email = "schoen@kr.tuwien.ac.at" }]
 description = "A MIDI and music data manipulation library"
 readme = "README.md"
 requires-python = ">= 3.11"
 keywords = ["midi", "music"]
 license = { file = "LICENSE.md" }
 dependencies = [
```

### Comparing `scoda-2.1b1/scoda/config/settings.json` & `scoda-2.1b2/scoda/config/settings.json`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/elements/bar.py` & `scoda-2.1b2/scoda/elements/bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from scoda.misc.enumerations import MessageType
 from scoda.misc.music_theory import Key
 from scoda.sequences.sequence import Sequence
 from scoda.settings.settings import PPQN
 
 
 class Bar:
-    """Class representing a single bar, its length defined by a time signature.
-    """
+    """Class representing a single bar, its length defined by a time signature."""
 
     def __init__(self, sequence: Sequence, numerator: int, denominator: int, key=None) -> None:
         super().__init__()
 
         self.sequence: Sequence = sequence
         self.time_signature_numerator = numerator
         self.time_signature_denominator = denominator
```

### Comparing `scoda-2.1b1/scoda/elements/composition.py` & `scoda-2.1b2/scoda/elements/composition.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,15 @@
         merged_sequences = Sequence.sequences_load(file_path=file_path,
                                                    track_indices=track_indices,
                                                    meta_track_indices=meta_track_indices,
                                                    target_meta_track_index=meta_track_index)
 
         # Quantisation
         for sequence in merged_sequences:
-            sequence.quantise()
-            sequence.quantise_note_lengths()
+            sequence.quantise_and_normalise()
 
         # Load composition from sequence
         return Composition.from_sequences(merged_sequences, meta_track_index)
 
     @staticmethod
     def from_sequences(sequences, meta_track_index: int = 0) -> Composition:
         # Split sequence into bars
@@ -58,7 +57,17 @@
         for track_index in range(0, len(tracks_bars)):
             track = Track(tracks_bars[track_index])
             tracks.append(track)
 
         # Create composition from tracks
         composition = Composition(tracks)
         return composition
+
+    def to_sequences(self):
+        sequences = []
+        for track in self.tracks:
+            sequences.append(track.to_sequence())
+        return sequences
+
+    def save(self, file_path: str):
+        sequences = self.to_sequences()
+        Sequence.sequences_save(sequences, file_path)
```

### Comparing `scoda-2.1b1/scoda/elements/message.py` & `scoda-2.1b2/scoda/elements/message.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/elements/track.py` & `scoda-2.1b2/scoda/elements/track.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/midi/midi_file.py` & `scoda-2.1b2/scoda/midi/midi_file.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/midi/midi_message.py` & `scoda-2.1b2/scoda/midi/midi_message.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/midi/midi_track.py` & `scoda-2.1b2/scoda/midi/midi_track.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/misc/enumerations.py` & `scoda-2.1b2/scoda/misc/enumerations.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/misc/music_theory.py` & `scoda-2.1b2/scoda/misc/music_theory.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/misc/scoda_logging.py` & `scoda-2.1b2/scoda/misc/scoda_logging.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/misc/util.py` & `scoda-2.1b2/scoda/misc/util.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/sequences/absolute_sequence.py` & `scoda-2.1b2/scoda/sequences/absolute_sequence.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/sequences/abstract_sequence.py` & `scoda-2.1b2/scoda/sequences/abstract_sequence.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/sequences/relative_sequence.py` & `scoda-2.1b2/scoda/sequences/relative_sequence.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/sequences/sequence.py` & `scoda-2.1b2/scoda/sequences/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,16 +172,15 @@
 
     def scale(self, factor, meta_sequence=None, quantise_afterwards=True) -> None:
         """See `scoda.sequence.relative_sequence.RelativeSequence.scale`."""
         self.rel.scale(factor, meta_sequence)
         self._abs_stale = True
 
         if quantise_afterwards:
-            self.quantise()
-            self.quantise_note_lengths()
+            self.quantise_and_normalise()
 
     def transpose(self, transpose_by: int) -> bool:
         """See `scoda.sequence.relative_sequence.RelativeSequence.transpose`."""
         self._abs_stale = True
         shifted = self.rel.transpose(transpose_by)
 
         # Possible that notes overlap
@@ -202,14 +201,21 @@
         self._rel_stale = True
 
     def quantise_note_lengths(self, possible_durations=None, standard_length=PPQN, do_not_extend=False) -> None:
         """See `scoda.sequence.absolute_sequence.AbsoluteSequence.quantise_note_lengths`."""
         self.abs.quantise_note_lengths(possible_durations, standard_length=standard_length, do_not_extend=do_not_extend)
         self._rel_stale = True
 
+    def quantise_and_normalise(self, step_sizes: list[int] = None, possible_durations=None, standard_length=PPQN,
+                               do_not_extend=False):
+        """Quantises and normalises the sequence."""
+        self.quantise(step_sizes)
+        self.quantise_note_lengths(possible_durations, standard_length, do_not_extend)
+        self.normalise()
+
     # Misc. Methods
 
     def get_message_timings_of_type(self, message_types: [MessageType]) -> list[tuple[int, Message]]:
         """See `scoda.sequence.absolute_sequence.AbsoluteSequence.get_message_timings_of_type`.
 
         """
         return self.abs.get_message_timings_of_type(message_types)
```

### Comparing `scoda-2.1b1/scoda/settings/settings.py` & `scoda-2.1b2/scoda/settings/settings.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/tokenisation/base_tokenisation.py` & `scoda-2.1b2/scoda/tokenisation/base_tokenisation.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/tokenisation/gridlike_tokenisation.py` & `scoda-2.1b2/scoda/tokenisation/gridlike_tokenisation.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/tokenisation/midilike_tokenisation.py` & `scoda-2.1b2/scoda/tokenisation/midilike_tokenisation.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/tokenisation/notelike_tokenisation.py` & `scoda-2.1b2/scoda/tokenisation/notelike_tokenisation.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda/tokenisation/transposed_notelike_tokenisation.py` & `scoda-2.1b2/scoda/tokenisation/transposed_notelike_tokenisation.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b1/scoda.egg-info/PKG-INFO` & `scoda-2.1b2/scoda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda
-Version: 2.1b1
+Version: 2.1b2
 Summary: A MIDI and music data manipulation library
 Author-email: Felix Schön <schoen@kr.tuwien.ac.at>
 License: MIT License
         
         Copyright (c) 2023 Felix Schön
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `scoda-2.1b1/scoda.egg-info/SOURCES.txt` & `scoda-2.1b2/scoda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

