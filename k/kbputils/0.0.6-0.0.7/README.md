# Comparing `tmp/kbputils-0.0.6.tar.gz` & `tmp/kbputils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbputils-0.0.6.tar", last modified: Fri May 10 15:51:21 2024, max compression
+gzip compressed data, was "kbputils-0.0.7.tar", last modified: Tue May 21 03:18:16 2024, max compression
```

## Comparing `kbputils-0.0.6.tar` & `kbputils-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-10 15:51:21.464118 kbputils-0.0.6/
--rw-r--r--   0 matt      (1000) matt      (1000)     1305 2024-04-16 18:40:43.000000 kbputils-0.0.6/LICENSE
--rw-r--r--   0 matt      (1000) matt      (1000)     2718 2024-05-10 15:51:21.464118 kbputils-0.0.6/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)     2363 2024-05-10 15:51:04.000000 kbputils-0.0.6/README.md
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-10 15:51:21.464118 kbputils-0.0.6/kbputils/
--rw-r--r--   0 matt      (1000) matt      (1000)      154 2024-05-10 15:51:04.000000 kbputils-0.0.6/kbputils/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-16 18:40:43.000000 kbputils-0.0.6/kbputils/__main__.py
--rw-r--r--   0 matt      (1000) matt      (1000)     2563 2024-05-03 18:34:35.000000 kbputils-0.0.6/kbputils/cli.py
--rw-r--r--   0 matt      (1000) matt      (1000)    14246 2024-05-10 15:51:04.000000 kbputils-0.0.6/kbputils/converters.py
--rw-r--r--   0 matt      (1000) matt      (1000)    18656 2024-05-10 15:51:04.000000 kbputils-0.0.6/kbputils/kbp.py
--rw-r--r--   0 matt      (1000) matt      (1000)      773 2024-04-16 18:40:43.000000 kbputils-0.0.6/kbputils/kbs.py
--rw-r--r--   0 matt      (1000) matt      (1000)     6745 2024-04-16 18:40:43.000000 kbputils-0.0.6/kbputils/validators.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-10 15:51:21.464118 kbputils-0.0.6/kbputils.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)     2718 2024-05-10 15:51:21.000000 kbputils-0.0.6/kbputils.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      362 2024-05-10 15:51:21.000000 kbputils-0.0.6/kbputils.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-05-10 15:51:21.000000 kbputils-0.0.6/kbputils.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       55 2024-05-10 15:51:21.000000 kbputils-0.0.6/kbputils.egg-info/entry_points.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        4 2024-05-10 15:51:21.000000 kbputils-0.0.6/kbputils.egg-info/requires.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        9 2024-05-10 15:51:21.000000 kbputils-0.0.6/kbputils.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      627 2024-05-03 18:34:35.000000 kbputils-0.0.6/pyproject.toml
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-05-10 15:51:21.464118 kbputils-0.0.6/setup.cfg
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-21 03:18:16.678255 kbputils-0.0.7/
+-rw-r--r--   0 matt      (1000) matt      (1000)     1305 2024-04-16 18:40:43.000000 kbputils-0.0.7/LICENSE
+-rw-r--r--   0 matt      (1000) matt      (1000)     2718 2024-05-21 03:18:16.678255 kbputils-0.0.7/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)     2363 2024-05-10 15:51:04.000000 kbputils-0.0.7/README.md
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-21 03:18:16.674921 kbputils-0.0.7/kbputils/
+-rw-r--r--   0 matt      (1000) matt      (1000)      154 2024-05-21 03:17:09.000000 kbputils-0.0.7/kbputils/__init__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-16 18:40:43.000000 kbputils-0.0.7/kbputils/__main__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     2563 2024-05-03 18:34:35.000000 kbputils-0.0.7/kbputils/cli.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    14842 2024-05-21 03:17:09.000000 kbputils-0.0.7/kbputils/converters.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    18907 2024-05-21 03:17:09.000000 kbputils-0.0.7/kbputils/kbp.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      773 2024-04-16 18:40:43.000000 kbputils-0.0.7/kbputils/kbs.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     6745 2024-04-16 18:40:43.000000 kbputils-0.0.7/kbputils/validators.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-21 03:18:16.678255 kbputils-0.0.7/kbputils.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)     2718 2024-05-21 03:18:16.000000 kbputils-0.0.7/kbputils.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      362 2024-05-21 03:18:16.000000 kbputils-0.0.7/kbputils.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-05-21 03:18:16.000000 kbputils-0.0.7/kbputils.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       55 2024-05-21 03:18:16.000000 kbputils-0.0.7/kbputils.egg-info/entry_points.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        4 2024-05-21 03:18:16.000000 kbputils-0.0.7/kbputils.egg-info/requires.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        9 2024-05-21 03:18:16.000000 kbputils-0.0.7/kbputils.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      627 2024-05-03 18:34:35.000000 kbputils-0.0.7/pyproject.toml
+-rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-05-21 03:18:16.678255 kbputils-0.0.7/setup.cfg
```

### Comparing `kbputils-0.0.6/LICENSE` & `kbputils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kbputils-0.0.6/PKG-INFO` & `kbputils-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbputils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Utilities to handle .kbp files created with Karaoke Builder Studio.
 Author-email: Matt M <code@itmightbekaraoke.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ass
```

### Comparing `kbputils-0.0.6/README.md` & `kbputils-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `kbputils-0.0.6/kbputils/cli.py` & `kbputils-0.0.7/kbputils/cli.py`

 * *Files identical despite different names*

### Comparing `kbputils-0.0.6/kbputils/converters.py` & `kbputils-0.0.7/kbputils/converters.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     target_x: int = 300 # Output resolution
     target_y: int = 216
     fade_in: int = 300 # Fade duration for line display/remove
     fade_out: int = 200
     transparency: bool = True
     offset: int | bool = True # False = disable offset (same as 0), True = pull from KBS config, int is offset in ms
     overflow: AssOverflow = AssOverflow.EVEN_SPLIT
+    allow_kt: bool = False # Use \kt if there are overlapping wipes on the same line (not supported by all ass implementations)
     #overflow_spacing: float # TODO? spacing value in styles that will apply for overflow (default 0). Multiplied by font height or based on default style?
 
     @validators.validated_types
     @staticmethod
     def __assert_valid(key: str, value):
         if key in AssOptions._fields:
             if not isinstance(value, (t := AssOptions._fields[key].type)):
@@ -212,25 +213,31 @@
             delay = s.start - cur
             dur = s.end - s.start
 
             if delay > 0:
                 # Gap between current position and start of next syllable
                 result += r"{\k%d}" % delay
             elif delay < 0:
-                # Playing catchup - could potentially use \kt to reset time
-                # here but it has limited support
-                dur += delay
+                # Playing catchup
+                if self.allow_kt:
+                    # Reset time so wipes can overlap (\kt takes a time in centiseconds from line start)
+                    result += r"{\kt%d}" % (s.start - line.start)
+                else:
+                    # Shorten syllable to compensate for missing time (keep in mind delay is negative)
+                    dur += delay
 
             # By default a syllable ends 1 centisecond before the next, so
             # special casing so we don't need a bunch of \k1 and the slight
             # errors don't catch up with us on a long line
             if len(line.syllables) > n+1 and line.syllables[n+1].start - s.end == 1:
                 dur += 1
 
-            wipe = "\kf" if s.wipe < 5 else "\k"
+            # Using == False explicitly because it's technically a tri-state with None meaning undefined
+            # Though that scenario shouldn't come up since we are allowing KBPFile to resolve wipedetail
+            wipe = "\k" if s.isprogressive() == False else "\kf"
 
             result += r"{%s%d}%s" % (wipe, dur, s.syllable)
             cur = s.start + dur
         return result
 
     @validators.validated_types
     @staticmethod
```

### Comparing `kbputils-0.0.6/kbputils/kbp.py` & `kbputils-0.0.7/kbputils/kbp.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,14 +166,19 @@
     start: int
     end: int
     wipe: int
 
     def isempty(self):
         return self.syllable == ""
 
+    def isprogressive(self):
+        # Zero means unresolved default wipe, so result is undefined. Otherwise
+        # everything less than 5 is progressive with varying level of wipe detail
+        return None if self.wipe == 0 else (self.wipe < 5)
+
 class KBPLine(typing.NamedTuple):
     header: KBPLineHeader
     syllables: list
 
     # There's only one header, so may as well pass anything unresolved down to it
     def __getattr__(self, attr):
         return getattr(self.header, attr)
```

### Comparing `kbputils-0.0.6/kbputils/kbs.py` & `kbputils-0.0.7/kbputils/kbs.py`

 * *Files identical despite different names*

### Comparing `kbputils-0.0.6/kbputils/validators.py` & `kbputils-0.0.7/kbputils/validators.py`

 * *Files identical despite different names*

### Comparing `kbputils-0.0.6/kbputils.egg-info/PKG-INFO` & `kbputils-0.0.7/kbputils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbputils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Utilities to handle .kbp files created with Karaoke Builder Studio.
 Author-email: Matt M <code@itmightbekaraoke.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ass
```

### Comparing `kbputils-0.0.6/pyproject.toml` & `kbputils-0.0.7/pyproject.toml`

 * *Files identical despite different names*

