# Comparing `tmp/munotes-2.0.1.tar.gz` & `tmp/munotes-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "munotes-2.0.1.tar", last modified: Mon Nov 20 09:02:26 2023, max compression
+gzip compressed data, was "munotes-2.0.2.tar", last modified: Tue May 21 13:45:35 2024, max compression
```

## Comparing `munotes-2.0.1.tar` & `munotes-2.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 komiya    (1000) komiya    (1000)        0 2023-11-20 09:02:26.898320 munotes-2.0.1/
--rw-r--r--   0 komiya    (1000) komiya    (1000)     1084 2023-02-05 14:27:23.000000 munotes-2.0.1/LICENSE
--rw-r--r--   0 komiya    (1000) komiya    (1000)     5202 2023-11-20 09:02:26.898320 munotes-2.0.1/PKG-INFO
--rw-r--r--   0 komiya    (1000) komiya    (1000)     4514 2023-11-20 08:59:22.000000 munotes-2.0.1/README.md
-drwxr-xr-x   0 komiya    (1000) komiya    (1000)        0 2023-11-20 09:02:26.898320 munotes-2.0.1/munotes/
--rw-r--r--   0 komiya    (1000) komiya    (1000)      295 2023-11-20 08:59:22.000000 munotes-2.0.1/munotes/__init__.py
--rw-r--r--   0 komiya    (1000) komiya    (1000)     8039 2023-11-20 08:59:22.000000 munotes-2.0.1/munotes/_base.py
--rw-r--r--   0 komiya    (1000) komiya    (1000)     3316 2023-11-20 08:59:22.000000 munotes-2.0.1/munotes/_utils.py
--rw-r--r--   0 komiya    (1000) komiya    (1000)      285 2023-02-16 06:27:08.000000 munotes-2.0.1/munotes/chord_names.py
--rw-r--r--   0 komiya    (1000) komiya    (1000)     4083 2023-11-18 15:49:37.000000 munotes-2.0.1/munotes/envelope.py
--rw-r--r--   0 komiya    (1000) komiya    (1000)    23369 2023-11-20 08:59:22.000000 munotes-2.0.1/munotes/notes.py
--rw-r--r--   0 komiya    (1000) komiya    (1000)     8985 2023-11-20 08:59:22.000000 munotes-2.0.1/munotes/sequence.py
-drwxr-xr-x   0 komiya    (1000) komiya    (1000)        0 2023-11-20 09:02:26.898320 munotes-2.0.1/munotes.egg-info/
--rw-r--r--   0 komiya    (1000) komiya    (1000)     5202 2023-11-20 09:02:26.000000 munotes-2.0.1/munotes.egg-info/PKG-INFO
--rw-r--r--   0 komiya    (1000) komiya    (1000)      325 2023-11-20 09:02:26.000000 munotes-2.0.1/munotes.egg-info/SOURCES.txt
--rw-r--r--   0 komiya    (1000) komiya    (1000)        1 2023-11-20 09:02:26.000000 munotes-2.0.1/munotes.egg-info/dependency_links.txt
--rw-r--r--   0 komiya    (1000) komiya    (1000)       14 2023-11-20 09:02:26.000000 munotes-2.0.1/munotes.egg-info/requires.txt
--rw-r--r--   0 komiya    (1000) komiya    (1000)        8 2023-11-20 09:02:26.000000 munotes-2.0.1/munotes.egg-info/top_level.txt
--rw-r--r--   0 komiya    (1000) komiya    (1000)       86 2023-11-20 09:02:26.898320 munotes-2.0.1/setup.cfg
--rw-r--r--   0 komiya    (1000) komiya    (1000)     1012 2023-07-12 16:36:08.000000 munotes-2.0.1/setup.py
+drwxr-xr-x   0 komiya    (1000) komiya    (1000)        0 2024-05-21 13:45:35.838135 munotes-2.0.2/
+-rw-r--r--   0 komiya    (1000) komiya    (1000)     1084 2023-02-05 14:27:23.000000 munotes-2.0.2/LICENSE
+-rw-r--r--   0 komiya    (1000) komiya    (1000)     5301 2024-05-21 13:45:35.838135 munotes-2.0.2/PKG-INFO
+-rw-r--r--   0 komiya    (1000) komiya    (1000)     4613 2024-05-21 13:44:02.000000 munotes-2.0.2/README.md
+drwxr-xr-x   0 komiya    (1000) komiya    (1000)        0 2024-05-21 13:45:35.838135 munotes-2.0.2/munotes/
+-rw-r--r--   0 komiya    (1000) komiya    (1000)      295 2024-05-21 13:44:02.000000 munotes-2.0.2/munotes/__init__.py
+-rw-r--r--   0 komiya    (1000) komiya    (1000)     7870 2024-05-21 13:44:02.000000 munotes-2.0.2/munotes/_base.py
+-rw-r--r--   0 komiya    (1000) komiya    (1000)     3569 2024-05-21 13:44:02.000000 munotes-2.0.2/munotes/_utils.py
+-rw-r--r--   0 komiya    (1000) komiya    (1000)      285 2023-02-16 06:27:08.000000 munotes-2.0.2/munotes/chord_names.py
+-rw-r--r--   0 komiya    (1000) komiya    (1000)     4083 2023-11-18 15:49:37.000000 munotes-2.0.2/munotes/envelope.py
+-rw-r--r--   0 komiya    (1000) komiya    (1000)    23210 2024-05-21 13:44:02.000000 munotes-2.0.2/munotes/notes.py
+-rw-r--r--   0 komiya    (1000) komiya    (1000)     8501 2024-05-21 13:44:02.000000 munotes-2.0.2/munotes/sequence.py
+drwxr-xr-x   0 komiya    (1000) komiya    (1000)        0 2024-05-21 13:45:35.838135 munotes-2.0.2/munotes.egg-info/
+-rw-r--r--   0 komiya    (1000) komiya    (1000)     5301 2024-05-21 13:45:35.000000 munotes-2.0.2/munotes.egg-info/PKG-INFO
+-rw-r--r--   0 komiya    (1000) komiya    (1000)      325 2024-05-21 13:45:35.000000 munotes-2.0.2/munotes.egg-info/SOURCES.txt
+-rw-r--r--   0 komiya    (1000) komiya    (1000)        1 2024-05-21 13:45:35.000000 munotes-2.0.2/munotes.egg-info/dependency_links.txt
+-rw-r--r--   0 komiya    (1000) komiya    (1000)       14 2024-05-21 13:45:35.000000 munotes-2.0.2/munotes.egg-info/requires.txt
+-rw-r--r--   0 komiya    (1000) komiya    (1000)        8 2024-05-21 13:45:35.000000 munotes-2.0.2/munotes.egg-info/top_level.txt
+-rw-r--r--   0 komiya    (1000) komiya    (1000)       86 2024-05-21 13:45:35.838135 munotes-2.0.2/setup.cfg
+-rw-r--r--   0 komiya    (1000) komiya    (1000)     1012 2023-07-12 16:36:08.000000 munotes-2.0.2/setup.py
```

### Comparing `munotes-2.0.1/LICENSE` & `munotes-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `munotes-2.0.1/PKG-INFO` & `munotes-2.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: munotes
-Version: 2.0.1
+Version: 2.0.2
 Summary: Handle musical notes and their sounds in Python
 Home-page: https://github.com/misya11p/munotes
 Author: misya11p
 License: MIT
 Project-URL: Source, https://github.com/misya11p/munotes
 Project-URL: API Reference, https://misya11p.github.io/munotes/
 Keywords: music note chord sound waveform
@@ -181,52 +181,59 @@
 ```
 
 Methods are the same as other classes.
 
 ## Version History
 
 ### [0.1.0](https://pypi.org/project/munotes/0.1.0/) (2022-11-12, Beta-release)
+
 - Add `Note` class
 - Add `Chord` class
 
 ### [1.0.0](https://pypi.org/project/munotes/1.0.0/) (2023-02-09)
+
 - Add `Notes` class
 - Add `Track` class
 - Add `Stream` class
 - Add `Rest` class
 - Add `sin()`, `square()`, `sawtooth()` methods
 - Add `play()` method
 - Add `render()` method
 
 ### [1.0.1](https://pypi.org/project/munotes/1.0.1/) (2023-02-12)
-- Fix a bug that `Rest` could not be put into `Track`
+
+- Fix a bug that `Rest` could not be put into `Track`.
 
 ### [1.1.0](https://pypi.org/project/munotes/1.1.0/) (2023-02-16)
+
 - Waveform parameters can be specified. Ex: `note.sawtooth(width=0.5)`
 - Support for inputting octave with note names. Ex: `note = mn.Note("A4")`
 - All supported chords can be seen in `mn.chord_names`
 - Arbitrary chords can be added
 
 ### [2.0.0](https://pypi.org/project/munotes/2.0.0/) (2023-11-19)
 
-\*We forgot to update PyPI Homepage in this version
-
 - Add `Envelope` class
-- Modified `sec` argument to `duration`
+- Modify `sec` argument to `duration`
 - Add default parameters for rendering that can be specified in initialization
     - `waveform`
     - `duration`
     - `unit`
     - `bpm`
     - `envelope`
     - `duty`
     - `width`
     - `amp`
 - Remove function that change frequency of `A4` directly
-- Modified input type of `Track` from `Tuple[Note, float]` to `List[Note]`
+- Modify input type of `Track` from `Tuple[Note, float]` to `List[Note]`
     - Note.duration is used to duration when rendering
 - Remove `**kwargs` in `render()` method
 
-### [2.0.1](https://pypi.org/project/munotes/2.0.1/) (2023-11-20, Latest)
+### [2.0.1](https://pypi.org/project/munotes/2.0.1/) (2023-11-20)
+
 - Fix `__add__` method of `Notes` class
 - Fix a bug that `append()` method of `Notes` class does not work
-- Modified `__repr__` method
+- Modify `__repr__` method
+
+### [2.0.2](https://pypi.org/project/munotes/2.0.2/) (2024-05-21, Latest)
+
+- Fix a bug that chord names in `Track` and `Stream` are not update when transposed
```

### Comparing `munotes-2.0.1/README.md` & `munotes-2.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -162,52 +162,59 @@
 ```
 
 Methods are the same as other classes.
 
 ## Version History
 
 ### [0.1.0](https://pypi.org/project/munotes/0.1.0/) (2022-11-12, Beta-release)
+
 - Add `Note` class
 - Add `Chord` class
 
 ### [1.0.0](https://pypi.org/project/munotes/1.0.0/) (2023-02-09)
+
 - Add `Notes` class
 - Add `Track` class
 - Add `Stream` class
 - Add `Rest` class
 - Add `sin()`, `square()`, `sawtooth()` methods
 - Add `play()` method
 - Add `render()` method
 
 ### [1.0.1](https://pypi.org/project/munotes/1.0.1/) (2023-02-12)
-- Fix a bug that `Rest` could not be put into `Track`
+
+- Fix a bug that `Rest` could not be put into `Track`.
 
 ### [1.1.0](https://pypi.org/project/munotes/1.1.0/) (2023-02-16)
+
 - Waveform parameters can be specified. Ex: `note.sawtooth(width=0.5)`
 - Support for inputting octave with note names. Ex: `note = mn.Note("A4")`
 - All supported chords can be seen in `mn.chord_names`
 - Arbitrary chords can be added
 
 ### [2.0.0](https://pypi.org/project/munotes/2.0.0/) (2023-11-19)
 
-\*We forgot to update PyPI Homepage in this version
-
 - Add `Envelope` class
-- Modified `sec` argument to `duration`
+- Modify `sec` argument to `duration`
 - Add default parameters for rendering that can be specified in initialization
     - `waveform`
     - `duration`
     - `unit`
     - `bpm`
     - `envelope`
     - `duty`
     - `width`
     - `amp`
 - Remove function that change frequency of `A4` directly
-- Modified input type of `Track` from `Tuple[Note, float]` to `List[Note]`
+- Modify input type of `Track` from `Tuple[Note, float]` to `List[Note]`
     - Note.duration is used to duration when rendering
 - Remove `**kwargs` in `render()` method
 
-### [2.0.1](https://pypi.org/project/munotes/2.0.1/) (2023-11-20, Latest)
+### [2.0.1](https://pypi.org/project/munotes/2.0.1/) (2023-11-20)
+
 - Fix `__add__` method of `Notes` class
 - Fix a bug that `append()` method of `Notes` class does not work
-- Modified `__repr__` method
+- Modify `__repr__` method
+
+### [2.0.2](https://pypi.org/project/munotes/2.0.2/) (2024-05-21, Latest)
+
+- Fix a bug that chord names in `Track` and `Stream` are not update when transposed
```

### Comparing `munotes-2.0.1/munotes/_base.py` & `munotes-2.0.2/munotes/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,14 @@
 
 import numpy as np
 import IPython.display as ipd
 
 from .envelope import Envelope
 
 
-NUM_C0 = 12 # MIDI note number of C0
-NUM_A4 = 69 # MIDI note number of A4
-KEY_NAMES = ['C', 'C#', 'D', 'D#', 'E', 'F', 'F#', 'G', 'G#', 'A', 'A#', 'B']
-
-
 class BaseNotes:
     def _init_attrs(
         self,
         waveform: Optional[Union[str, Callable]] = 'sin',
         duration: Optional[Union[float, int]] = 1.,
         unit: Optional[str] = "s",
         bpm: Optional[Union[float, int]] = 120,
@@ -22,15 +17,15 @@
         duty: Optional[float] = 0.5,
         width: Optional[float] = 1.,
         amp: Optional[float] = 1.,
         sr: int = 22050,
         A4: float = 440.,
     ):
         """Initialize attributes of notes and sequence."""
-        if not hasattr(self, '_notes'):
+        if not hasattr(self, "_notes"):
             self._notes = [self]
         self.waveform = waveform
         self.duration = duration
         self.unit = unit
         self.bpm = bpm
         self.duty = duty
         self.width = width
@@ -99,15 +94,15 @@
             >>> print(notes.A4)
             >>> note.tuning(450.)
             >>> print(notes.A4)
             440.0
             450.0
         """
         for note in self._notes:
-            note.tuning(freq, stand_A4=True)
+            note.tuning(freq)
 
     def render(self):
         pass
 
     def sin(
         self,
         duration: Optional[float] = None,
@@ -127,15 +122,15 @@
             envelope (Envelope, optional): Envelope.
             amp (float, optional): Amplitude.
 
         Returns:
             np.ndarray: Sin wave of the object.
         """
         return self.render(
-            'sin',
+            "sin",
             duration=duration,
             unit=unit,
             bpm=bpm,
             envelope=envelope,
             amp=amp,
         )
 
@@ -160,15 +155,15 @@
             duty (float, optional): Duty cycle.
             amp (float, optional): Amplitude.
 
         Returns:
             np.ndarray: Square wave of the object.
         """
         return self.render(
-            'square',
+            "square",
             duration=duration,
             unit=unit,
             bpm=bpm,
             envelope=envelope,
             duty=duty,
             amp=amp,
         )
@@ -194,15 +189,15 @@
             width (float, optional): Width of sawtooth.
             amp (float, optional): Amplitude.
 
         Returns:
             np.ndarray: Sawtooth wave of the object.
         """
         return self.render(
-            'sawtooth',
+            "sawtooth",
             duration=duration,
             unit=unit,
             bpm=bpm,
             envelope=envelope,
             width=width,
             amp=amp,
         )
@@ -226,15 +221,15 @@
             envelope (Envelope, optional): Envelope.
             amp (float, optional): Amplitude.
 
         Returns:
             np.ndarray: Triangle wave of the object.
         """
         return self.render(
-            'triangle',
+            "triangle",
             duration=duration,
             unit=unit,
             bpm=bpm,
             envelope=envelope,
             amp=amp,
         )
```

### Comparing `munotes-2.0.1/munotes/_utils.py` & `munotes-2.0.2/munotes/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import re
 from typing import Optional, Tuple
 from .chord_names import chord_names
 
 
+NUM_C0 = 12 # MIDI note number of C0
+NUM_A4 = 69 # MIDI note number of A4
+KEY_NAMES = ["C", "C#", "D", "D#", "E", "F", "F#", "G", "G#", "A", "A#", "B"]
+SUPPORTED_WAVEFORMS = ["sin", "square", "sawtooth", "triangle"]
+SUPPORTED_UNITS = ["s", "ms", "ql"]
+
 NOTE_NAME_PATTERN = "[A-G][#b]?"
 NOTE_PATTERN = f"{NOTE_NAME_PATTERN}\d*"
 VALID_NOTE_PATTERN = r"[A-Ga-g][#♯+b♭-]?\d*"
 LIM_REPR_NOTES = 6
 
 
 def note_name_formatting(
```

### Comparing `munotes-2.0.1/munotes/envelope.py` & `munotes-2.0.2/munotes/envelope.py`

 * *Files identical despite different names*

### Comparing `munotes-2.0.1/munotes/notes.py` & `munotes-2.0.2/munotes/notes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from typing import Optional, Union, List, Callable
 
 import numpy as np
 import scipy as sp
 
 from ._base import BaseNotes
-from ._utils import note_name_formatting, chord_name_formatting, get_repr_notes
+from ._utils import (
+    note_name_formatting,
+    chord_name_formatting,
+    get_repr_notes,
+    NUM_C0,
+    NUM_A4,
+    KEY_NAMES,
+    SUPPORTED_WAVEFORMS,
+    SUPPORTED_UNITS,
+)
 from .chord_names import chord_names
 from .envelope import Envelope
 
 
-NUM_C0 = 12 # MIDI note number of C0
-NUM_A4 = 69 # MIDI note number of A4
-KEY_NAMES = ['C', 'C#', 'D', 'D#', 'E', 'F', 'F#', 'G', 'G#', 'A', 'A#', 'B']
-SUPPORTED_WAVEFORMS = ["sin", "square", "sawtooth", "triangle"]
-SUPPORTED_UNITS = ["s", "ms", "ql"]
-
-
 class Note(BaseNotes):
     def __init__(
         self,
         query: Union[str, int],
         octave: int = 4,
-        waveform: Union[str, Callable] = 'sin',
+        waveform: Union[str, Callable] = "sin",
         duration: Union[float, int] = 1.,
         unit: str = "s",
         bpm: Union[float, int] = 120,
         envelope: Optional[Envelope] = None,
         duty: Optional[float] = 0.5,
         width: Optional[float] = 1.,
         amp: Optional[float] = 1.,
@@ -204,15 +206,15 @@
     @freq.setter
     def freq(self, value):
         raise Exception("freq is read only")
 
     def _return_name_idx(self) -> int:
         """Return index of the note name in KEY_NAMES"""
         idx = KEY_NAMES.index(self.name[0])
-        idx = (idx + ('#' in self.name) - ('b' in self.name)) % 12
+        idx = (idx + ("#" in self.name) - ("b" in self.name)) % 12
         return idx
 
     def _return_time_axis(self, sec: float) -> np.ndarray:
         """
         Generate time axis from duration and sampling rate.
 
         Args:
@@ -239,15 +241,15 @@
             C#4
         """
         for note in self._notes:
             note._idx = (note.idx + n_semitones) % 12
             note._name = KEY_NAMES[note.idx]
             note._num += n_semitones
             note._octave = (note.num - NUM_C0) // 12
-            note._freq = note._A4 * 2** ((note.num - NUM_A4) / 12)
+            note._freq = note._A4 * 2 ** ((note.num - NUM_A4) / 12)
 
     def tuning(self, freq: float = 440., stand_A4: bool = True) -> None:
         """
         Tuning.
 
         Args:
             freq (float, optional):
@@ -359,18 +361,18 @@
         else:
             raise TypeError(
                 "unsupported operand type(s) for +: 'Note' and "
                 f"'{type(other)}'"
             )
 
     def __str__(self):
-        return f'{self.name}{self.octave}'
+        return f"{self.name}{self.octave}"
 
     def __repr__(self):
-        return f'Note {self.name}{self.octave}'
+        return f"Note {self.name}{self.octave}"
 
     def __int__(self):
         return self.num
 
     def __eq__(self, other):
         if isinstance(other, str):
             return str(self) == other
@@ -412,15 +414,15 @@
         rendering.
 
         Examples:
             >>> rest = mn.Rest()
             >>> rest.sin()
             array([0., 0., 0., ..., 0., 0., 0.])
         """
-        self._name = 'Rest'
+        self._name = "Rest"
         self._octave = None
         self._freq = 0.
         self._num = None
         self._idx = None
         self._init_attrs(
             duration=duration,
             unit=unit,
@@ -434,25 +436,25 @@
     def transpose(self, *args, **kwargs):
         pass
 
     def tuning(self, *args, **kwargs):
         pass
 
     def __str__(self):
-        return 'Rest'
+        return "Rest"
 
     def __repr__(self):
-        return 'Rest'
+        return "Rest"
 
 
 class Notes(Note):
     def __init__(
         self,
         notes: List[Union[Note, int, str]],
-        waveform: Union[str, Callable] = 'sin',
+        waveform: Union[str, Callable] = "sin",
         duration: Union[float, int] = 1.,
         unit: str = "s",
         bpm: Union[float, int] = 120,
         envelope: Optional[Envelope] = None,
         duty: Optional[float] = 0.5,
         width: Optional[float] = 1.,
         amp: Optional[float] = 1.,
@@ -551,15 +553,15 @@
 
         Args:
             note (Union[Note, int]):
                 Note (or Notes or Chord) or midi note number
 
         Examples:
             >>> notes = mn.Notes(mn.Note("C4"))
-            >>> notes = notes.append(mn.Note("E4"), mn.Note("G4"))
+            >>> notes.append(mn.Note("E4"), mn.Note("G4"))
             >>> notes
             Notes (notes: Note C4, Note E4, Note G4)
         """
         self._init_notes([*self.notes, *note])
 
     def __len__(self):
         return len(self.notes)
@@ -584,24 +586,24 @@
             A4=self.A4,
         )
 
     def __repr__(self):
         return get_repr_notes(self, name="Notes")
 
     def __str__(self):
-        return ' '.join(self.fullnames)
+        return " ".join(self.fullnames)
 
 
 class Chord(Notes):
     def __init__(
         self,
         chord_name: str,
         type: Optional[str] = None,
         octave: int = 4,
-        waveform: Union[str, Callable] = 'sin',
+        waveform: Union[str, Callable] = "sin",
         duration: Union[float, int] = 1.,
         unit: str = "s",
         bpm: Union[float, int] = 120,
         envelope: Optional[Envelope] = None,
         duty: Optional[float] = 0.5,
         width: Optional[float] = 1.,
         amp: Optional[float] = 1.,
@@ -734,11 +736,11 @@
     def append(self, value) -> None:
         raise Exception("Chord class does not support append()")
 
     def __add__(self, other):
         raise Exception("Chord class does not support + operator")
 
     def __repr__(self):
-        return f'Chord {self.name}'
+        return f"Chord {self.name}"
 
     def __str__(self):
         return self.name
```

### Comparing `munotes-2.0.1/munotes/sequence.py` & `munotes-2.0.2/munotes/sequence.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,31 +4,14 @@
 
 from ._base import BaseNotes
 from ._utils import get_repr_notes
 from .notes import Note
 from .envelope import Envelope
 
 
-def flatten_notes(notes: List[Note]) -> List[Note]:
-    """
-    Flatten notes sequence. Changing the list of notes including Notes
-    class to a single list of notes.
-
-    Args:
-        notes (List[Note]): notes sequence
-
-    Returns:
-        List[Note]: notes sequence as List of a single note
-    """
-    flat_notes = []
-    for notes_ in notes:
-        flat_notes.extend(notes_._notes)
-    return flat_notes
-
-
 class Track(BaseNotes):
     def __init__(
         self,
         sequence: List[Note],
         waveform: Optional[Union[str, Callable]] = None,
         duration: Optional[float] = None,
         unit: Optional[str] = None,
@@ -74,15 +57,15 @@
             Track (notes: Note C4, Note D4, Note E4, Note C4, Note E4, Note G4)
 
             >>> track.sin()
             array([ 0.        ,  0.07448499,  0.14855616, ..., -0.01429455,
                 -0.00726152, -0.        ])
         """
         self.sequence = sequence
-        self._notes = flatten_notes(self.sequence)
+        self._notes = sequence
         self._init_attrs(
             waveform=waveform,
             duration=duration,
             unit=unit,
             bpm=bpm,
             envelope= envelope or Envelope(
                 attack=0.01,
@@ -147,15 +130,15 @@
             >>>     mn.Note("C4", duration=1),
             >>>     mn.Note("D4", duration=1),
             >>> ])
             >>> track.append(mn.Note("E4", duration=1))
             Track (notes: Note C4, Note D4, Note E4)
         """
         self.sequence = [*self.sequence, *notes]
-        self._notes = flatten_notes(self.sequence)
+        self._notes = self.sequence
 
     def __len__(self) -> int:
         return len(self.sequence)
 
     def __iter__(self) -> Iterable:
         return iter(self.sequence)
 
@@ -212,15 +195,15 @@
             >>>     'square',
             >>>     lambda t: np.sin(t) + np.sin(2*t)
             >>> ])
             array([ 1.        ,  1.83660002,  2.64969075, ..., -0.05431521,
                    -0.02542138,  0.        ])
         """
         self.tracks = tracks
-        self._notes = flatten_notes(self.tracks)
+        self._notes = tracks
         self._init_attrs(
             waveform=waveform,
             duration=duration,
             unit=unit,
             bpm=bpm,
             envelope=envelope,
             duty=duty,
@@ -262,15 +245,15 @@
             else:
                 y_track = np.append(y_track, np.zeros(len(y) - len(y_track)))
             y += y_track
         return y
 
     def append(self, *tracks: Track) -> None:
         self.tracks.extend(tracks)
-        self._notes = flatten_notes(self.tracks)
+        self._notes = self.tracks
 
     def __len__(self) -> int:
         return len(self.tracks)
 
     def __iter__(self) -> Iterable:
         return iter(self.tracks)
```

### Comparing `munotes-2.0.1/munotes.egg-info/PKG-INFO` & `munotes-2.0.2/munotes.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: munotes
-Version: 2.0.1
+Version: 2.0.2
 Summary: Handle musical notes and their sounds in Python
 Home-page: https://github.com/misya11p/munotes
 Author: misya11p
 License: MIT
 Project-URL: Source, https://github.com/misya11p/munotes
 Project-URL: API Reference, https://misya11p.github.io/munotes/
 Keywords: music note chord sound waveform
@@ -181,52 +181,59 @@
 ```
 
 Methods are the same as other classes.
 
 ## Version History
 
 ### [0.1.0](https://pypi.org/project/munotes/0.1.0/) (2022-11-12, Beta-release)
+
 - Add `Note` class
 - Add `Chord` class
 
 ### [1.0.0](https://pypi.org/project/munotes/1.0.0/) (2023-02-09)
+
 - Add `Notes` class
 - Add `Track` class
 - Add `Stream` class
 - Add `Rest` class
 - Add `sin()`, `square()`, `sawtooth()` methods
 - Add `play()` method
 - Add `render()` method
 
 ### [1.0.1](https://pypi.org/project/munotes/1.0.1/) (2023-02-12)
-- Fix a bug that `Rest` could not be put into `Track`
+
+- Fix a bug that `Rest` could not be put into `Track`.
 
 ### [1.1.0](https://pypi.org/project/munotes/1.1.0/) (2023-02-16)
+
 - Waveform parameters can be specified. Ex: `note.sawtooth(width=0.5)`
 - Support for inputting octave with note names. Ex: `note = mn.Note("A4")`
 - All supported chords can be seen in `mn.chord_names`
 - Arbitrary chords can be added
 
 ### [2.0.0](https://pypi.org/project/munotes/2.0.0/) (2023-11-19)
 
-\*We forgot to update PyPI Homepage in this version
-
 - Add `Envelope` class
-- Modified `sec` argument to `duration`
+- Modify `sec` argument to `duration`
 - Add default parameters for rendering that can be specified in initialization
     - `waveform`
     - `duration`
     - `unit`
     - `bpm`
     - `envelope`
     - `duty`
     - `width`
     - `amp`
 - Remove function that change frequency of `A4` directly
-- Modified input type of `Track` from `Tuple[Note, float]` to `List[Note]`
+- Modify input type of `Track` from `Tuple[Note, float]` to `List[Note]`
     - Note.duration is used to duration when rendering
 - Remove `**kwargs` in `render()` method
 
-### [2.0.1](https://pypi.org/project/munotes/2.0.1/) (2023-11-20, Latest)
+### [2.0.1](https://pypi.org/project/munotes/2.0.1/) (2023-11-20)
+
 - Fix `__add__` method of `Notes` class
 - Fix a bug that `append()` method of `Notes` class does not work
-- Modified `__repr__` method
+- Modify `__repr__` method
+
+### [2.0.2](https://pypi.org/project/munotes/2.0.2/) (2024-05-21, Latest)
+
+- Fix a bug that chord names in `Track` and `Stream` are not update when transposed
```

### Comparing `munotes-2.0.1/setup.py` & `munotes-2.0.2/setup.py`

 * *Files identical despite different names*

