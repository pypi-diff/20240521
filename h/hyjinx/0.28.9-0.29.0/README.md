# Comparing `tmp/hyjinx-0.28.9.tar.gz` & `tmp/hyjinx-0.29.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyjinx-0.28.9.tar", last modified: Fri Feb  9 13:37:05 2024, max compression
+gzip compressed data, was "hyjinx-0.29.0.tar", last modified: Tue May 21 09:08:02 2024, max compression
```

## Comparing `hyjinx-0.28.9.tar` & `hyjinx-0.29.0.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 user      (1001) users      (100)        0 2024-02-09 13:37:05.745863 hyjinx-0.28.9/
--rw-r--r--   0 user      (1001) users      (100)     1070 2024-02-06 14:37:46.000000 hyjinx-0.28.9/LICENSE
--rw-r--r--   0 user      (1001) users      (100)     1420 2024-02-09 13:37:05.729863 hyjinx-0.28.9/PKG-INFO
--rw-r--r--   0 user      (1001) users      (100)      739 2024-02-09 11:34:31.000000 hyjinx-0.28.9/README.md
-drwxr-xr-x   0 user      (1001) users      (100)        0 2024-02-09 13:37:05.470863 hyjinx-0.28.9/hyjinx/
--rw-r--r--   0 user      (1001) users      (100)       23 2024-02-09 13:36:01.000000 hyjinx-0.28.9/hyjinx/__init__.py
--rw-r--r--   0 user      (1001) users      (100)     2294 2024-02-05 12:57:36.000000 hyjinx-0.28.9/hyjinx/crypto.hy
--rw-r--r--   0 user      (1001) users      (100)     3062 2024-02-06 15:19:32.000000 hyjinx-0.28.9/hyjinx/datatypes.hy
--rw-r--r--   0 user      (1001) users      (100)     2385 2024-02-09 12:34:36.000000 hyjinx-0.28.9/hyjinx/docs.hy
--rw-r--r--   0 user      (1001) users      (100)     1623 2024-02-09 13:11:43.000000 hyjinx-0.28.9/hyjinx/hyrc.hy
--rw-r--r--   0 user      (1001) users      (100)     6001 2024-02-07 17:42:03.000000 hyjinx-0.28.9/hyjinx/lib.hy
--rw-r--r--   0 user      (1001) users      (100)      744 2024-02-09 11:51:20.000000 hyjinx-0.28.9/hyjinx/macros.hy
--rw-r--r--   0 user      (1001) users      (100)     1798 2024-02-09 11:56:41.000000 hyjinx-0.28.9/hyjinx/mat.hy
--rw-r--r--   0 user      (1001) users      (100)     3077 2024-02-05 23:16:16.000000 hyjinx-0.28.9/hyjinx/screen.hy
--rw-r--r--   0 user      (1001) users      (100)     7558 2024-02-09 13:34:36.000000 hyjinx-0.28.9/hyjinx/source.hy
--rw-r--r--   0 user      (1001) users      (100)       32 2024-02-07 16:18:14.000000 hyjinx-0.28.9/hyjinx/visual.hy
--rw-r--r--   0 user      (1001) users      (100)     1152 2024-02-06 15:19:05.000000 hyjinx-0.28.9/hyjinx/wire.hy
--rw-r--r--   0 user      (1001) users      (100)     1172 2024-02-09 11:38:27.000000 hyjinx-0.28.9/hyjinx/zmq_client.hy
--rw-r--r--   0 user      (1001) users      (100)     1948 2024-02-09 11:38:18.000000 hyjinx-0.28.9/hyjinx/zmq_server.hy
-drwxr-xr-x   0 user      (1001) users      (100)        0 2024-02-09 13:37:05.678863 hyjinx-0.28.9/hyjinx.egg-info/
--rw-r--r--   0 user      (1001) users      (100)     1420 2024-02-09 13:37:04.000000 hyjinx-0.28.9/hyjinx.egg-info/PKG-INFO
--rw-r--r--   0 user      (1001) users      (100)      447 2024-02-09 13:37:04.000000 hyjinx-0.28.9/hyjinx.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1001) users      (100)        1 2024-02-09 13:37:04.000000 hyjinx-0.28.9/hyjinx.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1001) users      (100)      111 2024-02-09 13:37:04.000000 hyjinx-0.28.9/hyjinx.egg-info/requires.txt
--rw-r--r--   0 user      (1001) users      (100)        7 2024-02-09 13:37:04.000000 hyjinx-0.28.9/hyjinx.egg-info/top_level.txt
--rw-r--r--   0 user      (1001) users      (100)      102 2024-02-06 14:53:46.000000 hyjinx-0.28.9/pyproject.toml
--rw-r--r--   0 user      (1001) users      (100)       88 2024-02-09 11:55:11.000000 hyjinx-0.28.9/requirements.txt
--rw-r--r--   0 user      (1001) users      (100)      705 2024-02-09 13:37:05.762863 hyjinx-0.28.9/setup.cfg
+drwxr-xr-x   0 user      (1001) users      (100)        0 2024-05-21 09:08:02.069175 hyjinx-0.29.0/
+-rw-r--r--   0 user      (1001) users      (100)       38 2024-02-06 15:19:38.000000 hyjinx-0.29.0/AUTHORS
+-rw-r--r--   0 user      (1001) users      (100)     1070 2024-02-06 14:37:46.000000 hyjinx-0.29.0/LICENSE
+-rw-r--r--   0 user      (1001) users      (100)     4622 2024-05-21 09:08:02.045175 hyjinx-0.29.0/PKG-INFO
+-rw-r--r--   0 user      (1001) users      (100)     1957 2024-05-08 11:47:39.000000 hyjinx-0.29.0/README.md
+drwxr-xr-x   0 user      (1001) users      (100)        0 2024-05-21 09:08:01.750175 hyjinx-0.29.0/hyjinx/
+-rw-r--r--   0 user      (1001) users      (100)     2179 2024-05-21 09:06:03.000000 hyjinx-0.29.0/hyjinx/__init__.py
+-rw-r--r--   0 user      (1001) users      (100)    16082 2024-05-08 14:16:43.000000 hyjinx-0.29.0/hyjinx/beautify.hy
+-rw-r--r--   0 user      (1001) users      (100)     2294 2024-02-05 12:57:36.000000 hyjinx-0.29.0/hyjinx/crypto.hy
+-rw-r--r--   0 user      (1001) users      (100)     2538 2024-05-08 11:51:44.000000 hyjinx-0.29.0/hyjinx/docs.hy
+-rw-r--r--   0 user      (1001) users      (100)     2738 2024-05-04 00:22:53.000000 hyjinx-0.29.0/hyjinx/hyrc.hy
+-rw-r--r--   0 user      (1001) users      (100)    11310 2024-05-06 19:45:02.000000 hyjinx-0.29.0/hyjinx/inspect.py
+-rw-r--r--   0 user      (1001) users      (100)    10309 2024-04-30 10:37:49.000000 hyjinx-0.29.0/hyjinx/lib.hy
+-rw-r--r--   0 user      (1001) users      (100)    15848 2024-05-04 19:06:11.000000 hyjinx-0.29.0/hyjinx/llm.hy
+-rw-r--r--   0 user      (1001) users      (100)     3829 2024-04-29 10:47:04.000000 hyjinx-0.29.0/hyjinx/macros.hy
+-rw-r--r--   0 user      (1001) users      (100)      888 2024-04-09 13:50:23.000000 hyjinx-0.29.0/hyjinx/mail.hy
+-rw-r--r--   0 user      (1001) users      (100)     3979 2024-04-29 10:55:33.000000 hyjinx-0.29.0/hyjinx/mat.hy
+-rw-r--r--   0 user      (1001) users      (100)    16648 2024-05-07 21:18:58.000000 hyjinx-0.29.0/hyjinx/reader.py
+-rw-r--r--   0 user      (1001) users      (100)     3026 2024-04-02 12:27:35.000000 hyjinx-0.29.0/hyjinx/screen.hy
+-rw-r--r--   0 user      (1001) users      (100)     8926 2024-05-07 14:02:21.000000 hyjinx-0.29.0/hyjinx/source.hy
+-rw-r--r--   0 user      (1001) users      (100)     1168 2024-02-18 19:01:10.000000 hyjinx-0.29.0/hyjinx/wire.hy
+-rw-r--r--   0 user      (1001) users      (100)     1178 2024-02-18 19:01:43.000000 hyjinx-0.29.0/hyjinx/zmq_client.hy
+-rw-r--r--   0 user      (1001) users      (100)     1960 2024-05-21 09:03:49.000000 hyjinx-0.29.0/hyjinx/zmq_server.hy
+drwxr-xr-x   0 user      (1001) users      (100)        0 2024-05-21 09:08:01.993175 hyjinx-0.29.0/hyjinx.egg-info/
+-rw-r--r--   0 user      (1001) users      (100)     4622 2024-05-21 09:08:00.000000 hyjinx-0.29.0/hyjinx.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1001) users      (100)      507 2024-05-21 09:08:00.000000 hyjinx-0.29.0/hyjinx.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1001) users      (100)        1 2024-05-21 09:08:00.000000 hyjinx-0.29.0/hyjinx.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1001) users      (100)       94 2024-05-21 09:08:00.000000 hyjinx-0.29.0/hyjinx.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1001) users      (100)      194 2024-05-21 09:08:00.000000 hyjinx-0.29.0/hyjinx.egg-info/requires.txt
+-rw-r--r--   0 user      (1001) users      (100)        7 2024-05-21 09:08:00.000000 hyjinx-0.29.0/hyjinx.egg-info/top_level.txt
+-rw-r--r--   0 user      (1001) users      (100)     1544 2024-05-06 15:23:59.000000 hyjinx-0.29.0/pyproject.toml
+-rw-r--r--   0 user      (1001) users      (100)       38 2024-05-21 09:08:02.076175 hyjinx-0.29.0/setup.cfg
```

### Comparing `hyjinx-0.28.9/LICENSE` & `hyjinx-0.29.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyjinx-0.28.9/hyjinx/crypto.hy` & `hyjinx-0.29.0/hyjinx/crypto.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.28.9/hyjinx/docs.hy` & `hyjinx-0.29.0/hyjinx/docs.hy`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,66 @@
 "Browse the official Hy / Hyrule docs (with syntax highlighting)."
 
+(require hyrule [defmain])
+
 (import hy hyrule)
 (import os
         tarfile
         shutil
         urllib.request)
 (import pydoc [pager])
 (import platformdirs [user-cache-dir])
 
 (import pygments [highlight])
 (import pygments.lexers [RstLexer])
 (import pygments.formatters [TerminalFormatter])
 
 (import hyjinx.lib [mkdir slurp])
 
+;; TODO search docs for terms
 
-(defn install []
-  "Download a local copy of the Hy documentation."
-  (let [hy-url f"https://github.com/hylang/hy/archive/refs/tags/{hy.__version__}.tar.gz"
-        hyrule-url f"https://github.com/hylang/hyrule/archive/refs/tags/{hyrule.__version__}.tar.gz"
-        cachedir (user-cache-dir __package__ __name__)]
-    (mkdir f"{cachedir}/docs/hy")
+
+(defn _install_docs [tarball-url package * [extension ".rst"]]
+  "Download a local copy of some specific documentation."
+  (let [cachedir (user-cache-dir __package__ __name__)
+        tarball f"{cachedir}/{package}.tar.gz"]
+    (mkdir f"{cachedir}/docs/{package}")
     ;; download docs to cache
-    (urllib.request.urlretrieve hy-url :filename f"{cachedir}/{hy.__version__}.tar.gz")
-    (with [tf (tarfile.open f"{cachedir}/{hy.__version__}.tar.gz" "r")]
+    (urllib.request.urlretrieve tarball-url :filename tarball) 
+    (with [tf (tarfile.open tarball "r")]
       (for [f (tf.getmembers)]
-        (when (f.path.endswith ".rst")
+        (when (f.path.endswith extension)
           (setv f.name (os.path.basename f.name))
-          ;; unpack and copy docs/*.rst to cache (incl. version name)
-          (tf.extract :member f :path f"{cachedir}/docs/hy"))))
-    (mkdir f"{cachedir}/docs/hyrule")
-    (urllib.request.urlretrieve hyrule-url :filename f"{cachedir}/{hyrule.__version__}.tar.gz")
-    (with [tf (tarfile.open f"{cachedir}/{hyrule.__version__}.tar.gz" "r")]
-      (for [f (tf.getmembers)]
-        (when (f.path.endswith ".rst")
-          (setv f.name (os.path.basename f.name))
-          (tf.extract :member f :path f"{cachedir}/docs/hyrule"))))))
+          ;; unpack and copy docs/*.rst to cache
+          (tf.extract :member f :path f"{cachedir}/docs/{package}"))))
+    (os.remove tarball)))
 
+(defn install []
+  "Download a local copy of the Hy and Hyrule documentation."
+  (_install-docs f"https://github.com/hylang/hy/archive/refs/tags/{hy.__version__}.tar.gz" f"hy_{hy.__version__}")
+  (_install-docs f"https://github.com/hylang/hyrule/archive/refs/tags/{hyrule.__version__}.tar.gz" f"hyrule_{hyrule.__version__}"))
 
-(defn hy-doc [[page "index"] * [package "hy"] [use-pager True] [bg "dark"]]
-  "Show hy docs (or another package). For example, `(hy-doc \"whyhy\")` or `(hy-doc \"NEWS\")."
+(defn _show-doc [[page "index"] * package [use-pager True] [bg "dark"]]
+  "Show a package's documentation. For example, (hy-doc \"whyhy\") or (hy-doc \"NEWS\")."
   (try
     (let [formatter (TerminalFormatter :bg bg :stripall True)
           term (shutil.get-terminal-size)
           cachedir (user-cache-dir __package__ __name__)
           fname f"{cachedir}/docs/{package}/{page}.rst"
           text (highlight (slurp fname) (RstLexer) formatter)]
       (if use-pager
           (pager text)
           (print text)))
     (except [FileNotFoundError]
-      (raise (FileNotFoundError f"Could not find '{page}' - did you correctly type the page name and install the documentation with (doc.install)?")))))
+      (raise (FileNotFoundError f"Could not find '{page}' - did you correctly type the page name and install the documentation with (hyjinx.docs.install)?")))))
 
 (defn hyrule-doc [#* args #** kwargs]
-  "Show hyrule docs."
-  (hy-docs #* args #** kwargs :package "hyrule"))
+  "Show hyrule's docs."
+  (_show-doc #* args #** kwargs :package f"hyrule_{hyrule.__version__}"))
+
+(defn hy-doc [#* args #** kwargs]
+  "Show Hy's documentation. For example, (hy-doc \"whyhy\") or (hy-doc \"NEWS\")."
+  (_show-doc #* args #** kwargs :package f"hy_{hy.__version__}"))
+
+(defmain []
+  "If running from the command line, install the docs."
+  (install))
```

### Comparing `hyjinx-0.28.9/hyjinx/screen.hy` & `hyjinx-0.29.0/hyjinx/screen.hy`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-"""
-A simple curses display class with context manager.
-You'll need to start the main using (.wrapper curses ...).
-"""
+"A simple curses display class with context manager.
+You'll need to start the main using (.wrapper curses ...)."
+
+(require hyrule [unless -> ->>])
 
 (import curses)
 (import logging)
 
 
 (defclass Screen []
   "Manage a display."
@@ -77,16 +77,15 @@
   (defn input [self [prompt ""]]
     "Get input in a text box."
     (let [y (- curses.LINES 2)
           x (+ 1 (len prompt))
           tw (.newwin curses 1 (- curses.COLS 1) y 1)]
       (.put self y 1 prompt) 
       (.refresh self.window)
-      (.bkgdset tw (or (.color_pair curses 191) curses.A_REVERSE))
-      ;; FIXME : earlier efforts explicitly did (del tb) - check if necessary
+      (.bkgdset tw (| (.color_pair curses 191) curses.A_REVERSE))
       (let [tb (.Textbox curses.textpad tw :insert-mode True)]
         (.edit tb)
         (setv instr (.strip (tb.gather)))
         (.clear tw)
         instr)))
 
   (defn centre [self s]
```

### Comparing `hyjinx-0.28.9/hyjinx/source.hy` & `hyjinx-0.29.0/hyjinx/source.hy`

 * *Files 15% similar despite different names*

```diff
@@ -1,169 +1,191 @@
-"Utilities for code inspection and presentation."
+"
+Utilities for code inspection and presentation.
+"
 
 (require hyrule [-> ->> unless])
 
+(require hyjinx.macros [defmethod lmap])
+
 (import hyrule [inc dec pformat])
-(import hy.compiler [hy-compile])
+(import hyjinx.lib [first second last])
 (import hy.repl [REPL])
 
+(import multimethod [multimethod])
 (import functools [partial])
 
 (import sys os traceback subprocess shutil)
 
 (import pygments [highlight])
 (import pygments.lexers [get-lexer-by-name HyLexer PythonLexer PythonTracebackLexer])
 (import pygments.formatters [TerminalFormatter])
-(import pansi [ansi])
+(import pansi [ansi :as _ansi])
 
-(import inspect [ismodule getsource getsourcefile])
+(import hyjinx.inspect [currentframe stack
+                        ismodule findsource
+                        getmodule getcomments getsource getsourcefile])
+(import hyjinx.beautify [grind])
 
 (import hyjinx.lib [slurp])
 
 
-(defn get-hy-tree [x]
-  "Returns the AST of a hy module, function, class etc."
-  (let [file (getsourcefile x)
-        hy-source (slurp file)
-        module (cond (ismodule x) x.__name__
-                     :else x.__module__)]
-    (hy-compile hy-source module)))
-
-(defn edit-source [x]
-  "Quick and dirty edit of source file. Uses the system editor.
-You could also call emacsclient or similar."
-  (let [line (:line (get-source-details x))
-        editor (os.getenv "HYJINX_EDITOR" (os.getenv "EDITOR" f"vi +{line}"))]
+(defn edit-source [obj * [editor None]]
+  "Quick and dirty edit of source file.
+  You could also call emacsclient or similar.
+  Uses, in order of preference:
+      - the editor command passed as an argument
+      - the editor command set by $HYJINX_EDITOR
+      - the system editor set by $EDITOR
+      - vi +{line}
+  It will replace any mention of '{line}' in the editor string with
+  the line number associated with `obj`."
+  ;; TODO : arguments to emacsclient are not handled
+  (let [line (:line (get-source-details obj))
+        editor (os.getenv "HYJINX_EDITOR" (os.getenv "EDITOR" f"vi +{line}"))
+        editor_args (os.getenv "HYJINX_EDITOR_ARGS" "")]
     (try
-      (subprocess.run [editor (getsourcefile x)] :check True))))
+      (subprocess.run [(.replace editor "{line}" (str line)) #* editor_args (getsourcefile obj)] :check True))))
 
-(defn get-source-details [x]
-  "Get line number, source file of x."
-  (let [file (getsourcefile x)
-        module (cond (ismodule x) x.__name__
-                     :else x.__module__)
-        ext (cut file -3 None)
-        lang (match ext
-                    ".py" "python"
-                    ".hy" "hylang"
-                    ".pytb" "pytb"
-                    ".py3tb" "py3tb")
+(defn _get-lang-from-filename [filename]
+  "Guess the language from the filename extension."
+  (match (last (.split filename "."))
+    "py" "python"
+    "hy" "hylang"
+    "pytb" "pytb"
+    "py3tb" "py3tb"))
+
+(defn get-source-details [obj]
+  "Get line number, source file of obj."
+  (let [file (getsourcefile obj)
+        module (cond (ismodule obj) obj.__name__
+                     :else obj.__module__)
+        ext (last (.split file "."))
+        lang (_get-lang-from-filename file)
         ;; TODO : handle classes
-        lnum (if (and (hasattr x "__code__")
-                      (hasattr x.__code__ "co_firstlineno"))
-                 (- x.__code__.co-firstlineno 1)
-                 0)]
-      {"line" lnum
+        lineno (if (and (hasattr obj "__code__")
+                        (hasattr obj.__code__ "co_firstlineno"))
+                   (- obj.__code__.co-firstlineno 1)
+                   (second (findsource obj)))]
+      {"line" lineno
        "module" module
        "file" file
        "language" lang
        "extension" ext}))
 
-(defn get-lines [fname line-number]
-  (let [source (slurp fname)
-        lines (.split source "\n")
-        rest-lines (cut lines line-number None)
-        defn-lines []
-        paren-excess 0]
-    (for [l rest-lines]
-      (.append defn-lines l)
-      (+= paren-excess (l.count "("))
-      (-= paren-excess (l.count ")"))
-      (unless (or paren-excess
-                  (not (.count l ")")))
-              (break)))
-    (.join "\n" defn-lines)))  
-           
-(defn get-hy-source [x]
-  "Returns the source code of a hy module or the module of a hy function, class etc."
-  (let [details (get-source-details x)
-        file (:file details)
-        module (:module details)
-        lnum (:line details)]
-    ;; TODO : handle classes
-    (if lnum
-        (get-lines file lnum)
-        (slurp file))))
-
-(defn get-source [x]
-  "Get the source for a python or hy function, module or other object."
-  (let [details (get-source-details x)
-        lang (:language details)]
-    (cond (= lang "python") (getsource x)
-          (= lang "hylang") (get-hy-source x)
-          :else (raise (NotImplementedError f"Filetype {(:extension details)} is unknown.")))))
-
-(defn print-source [x * [bg "dark"] [linenos False]]
-  "Pretty-print the source code of a module or function, with syntax highlighting."
-  (let [details (get-source-details x)
+(defmethod print-source [#^ multimethod obj #** kwargs]
+  "Pretty-print the source code of a multimethod, with syntax highlighting."
+  (for [f (obj.values)]
+    (print-source f #** kwargs)))
+
+(defmethod print-source [#^ partial obj * [linenos False] #** kwargs]
+  "Pretty-print the source code of a partial, with syntax highlighting."
+  (let [padding (if linenos "      " "")]
+    (print)
+    (print f"{padding}{obj}")
+    (print)
+    (print "Resolves to:")
+    (print-source obj.func #** kwargs)
+    (print f"args: {obj.args}")
+    (print f"keyword args: {obj.keywords}")
+    (print)))
+
+(defmethod print-source [obj * [bg "light"] [linenos False] [details None]]
+  "Pretty-print the source code of module or function obj, with syntax highlighting.
+  Keyword `bg` is \"dark\" or \"light\"."
+  (let [details (get-source-details obj)
         padding (if linenos "      " "")
-        header f"{padding}{x}, module {(:module details)}\n{padding}File {(:file details)}, line {(:line details)}"
-        lexer (get-lexer-by-name (:language details))
+        language (:language details)
+        header f"{padding}{obj}, module {(:module details)}\n{padding}File {_ansi.b}{(:file details)}{_ansi._b}, line {(:line details)}"
+        lexer (get-lexer-by-name language)
         formatter (TerminalFormatter :linenos linenos
                                      :bg bg
-                                     :stripall True)]
+                                     :stripall True)
+        source (if (= language "hylang")
+                   (grind (getsource obj) :filename (:file details))
+                   (getsource obj))]
+    ;; modify formatter so that line numbers correspond to the source
     (setv formatter._lineno (:line details))
     (print)
     (print header)
     (unless linenos (print))
-    (print (highlight (get-source x) lexer formatter))))
+    (print (highlight source lexer formatter))))
 
 (defn interact []
-  "Interact with code from called point."
-  (let [repl (REPL :locals (| (globals) (locals)))]
+  "Interact with code from called point by starting a nested REPL
+  with the same local variables as the calling scope.
+
+  This is useful for debugging by running within the context of a calling
+  function. The local variables can be used in the REPL and the behaviour
+  of the code can be observed and modified as needed.
+
+  This is only expected to work in CPython."
+  (let [caller-frame (. (currentframe) f-back)
+        caller caller-frame.f-code.co-name
+        lineno (- caller-frame.f-lineno 1)
+        filename caller-frame.f-code.co-filename
+        lang (_get-lang-from-filename filename)
+        module (get caller-frame.f-globals "__name__")
+        repl (REPL :locals caller-frame.f-locals)]
+    ;; give the nested REPL an extended prompt by setting sys.ps*
     (setv old-ps1 sys.ps1
           old-ps2 sys.ps2
-          sys.ps1 (+ "=" sys.ps1)
-          sys.ps2 (+ "." sys.ps2))
-    (.interact repl f"{ansi.GREEN}nested REPL - ctrl-D to exit.{ansi.reset}")
-    (setv sys.ps1 old-ps1
-          sys.ps2 old-ps2)))
+          sys.ps1 (+ _ansi.GREEN module "." caller " " sys.ps1 _ansi.reset)
+          sys.ps2 (+ _ansi.RED module "." caller "." sys.ps2 _ansi.reset))
+    (try
+      (.interact repl f"{_ansi.GREEN}nested REPL {caller} - ctrl-D to exit.
+File {_ansi.b}{filename}{_ansi._b}, line {lineno}{_ansi.reset}")
+      (finally
+        (del caller-frame)
+        (setv sys.ps1 old-ps1
+              sys.ps2 old-ps2)))))
     
-(defn hylight [s * [bg "dark"] [language "hylang"]]
-  "Syntax highlight a Hy (or other language) string. This is nice for use in the repl - put
-`(import hyjinx.source [hylight])
-(setv repl-output-fn hylight)`
-in your .hyrc."
+(defn hylight [s * [bg "light"] [language "hylang"]]
+  "Syntax highlight a Hy (or other language) string.
+  Keyword `bg` is \"dark\" or \"light\".
+
+  This is nice for use in the repl - put
+  (import hyjinx.source [hylight])
+  (setv repl-output-fn hylight)
+  in your .hyrc."
   (let [formatter (TerminalFormatter :bg bg :stripall True)
         term (shutil.get-terminal-size)
         lexer (get-lexer-by-name language)]
     (highlight (pformat s :indent 2 :width (- term.columns 5))
                (HyLexer)
                formatter)))
 
 (defn _exception-hook [exc-type exc-value tb *
                        [bg "dark"]
                        [limit 4]
                        [lines-around 2]
                        [linenos True]
                        [ignore ["hy/repl.py"]]]
-  "Exception hook for syntax highlighted traceback. Install using (for example)
-`(setv sys.excepthook (partial exception-hook :lines-around 3 :ignore [\"hy/repl.py\"]`
-(note the use of `partial` to set options) or simply
-`(setv sys.excepthook exception-hook)`
-if you're happy with the defaults."
+  "Exception hook for syntax highlighted traceback.
+  Install using inject-exception-hook, or with
+    (setv sys.excepthook (partial exception-hook :lines-around 3 :ignore [\"hy/repl.py\"]
+  (note the use of partial to set options) or simply with
+    (setv sys.excepthook exception-hook)
+  if you're happy with the defaults."
   (setv _tb tb
         lang None
         filename "")
   (while _tb
     (setv filename _tb.tb_frame.f_code.co_filename
-          ext (cut filename -3 None)
-          lang (match ext
-                      ".py" "python"
-                      ".hy" "hylang"
-                      _ None))
+          ext (last (.split filename "."))
+          lang (_get-lang-from-filename filename))
     ;; code for top frame
-    (if (and lang (not (any (map filename.endswith ignore))))
+    (if (and lang
+             (not (any (map filename.endswith ignore))))
       (let [source (slurp filename)
             lineno _tb.tb-lineno
             lines (cut (.split source "\n") (- lineno lines-around) (+ lineno lines-around))
             code-lexer (get-lexer-by-name lang)
             code-formatter (TerminalFormatter :bg bg :stripall True :linenos linenos)]
         (setv code-formatter._lineno (- lineno lines-around))
-        (sys.stderr.write f"  File {ansi.b}{filename}{ansi._b}, line {lineno}\n")
+        (sys.stderr.write f"  File {_ansi.b}{filename}{_ansi._b}, line {lineno}\n")
         (-> (.join "\n" lines)
             (highlight code-lexer code-formatter)
             (sys.stderr.write))
         (sys.stderr.write "\n")
         (break))
       (setv _tb _tb.tb-next)))
   ;; the traceback
@@ -171,15 +193,17 @@
         exc-formatter (TerminalFormatter :bg bg :stripall True)
         term (shutil.get-terminal-size)]
     (-> (.join "" fexc)
         (highlight (PythonTracebackLexer) exc-formatter)
         (sys.stderr.write))))
 
 (defn inject-exception-hook [#** kwargs]
-  "Inject the new exception hook."
+  "Inject (install) a new exception hook, for syntax highlighted traceback.
+  Install using (for example)
+  (inject-exception-hook :lines-around 3 :ignore [\"hy/repl.py\"])"
   (try
     _hy_repl
     ;; if it didn't raise an exception, we're already running in a repl
     ;; so we can just replace the global exception handler
     (setv sys.excepthook (partial _exception-hook #** kwargs))
 
     (except [NameError]
@@ -192,8 +216,7 @@
             (setv sys.last_type (self.locals.get "_hy_last_type" sys.last_type))
             (setv sys.last_value (self.locals.get "_hy_last_value" sys.last_value))
             (setv sys.last_traceback (self.locals.get "_hy_last_traceback" sys.last_traceback)))
         ((partial _exception-hook #** kwargs) sys.last_type sys.last_value sys.last_traceback)
         (setv (get self.locals (hy.mangle "*e")) sys.last_value))
 
       (setv hy.repl.REPL._error_wrap _error_wrap))))
-
```

### Comparing `hyjinx-0.28.9/hyjinx/wire.hy` & `hyjinx-0.29.0/hyjinx/wire.hy`

 * *Files 20% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 (import zmq)
 (import json)
 (import time [time])
 (import uuid [uuid1])
 (import zstandard [compress decompress])
 
-(import crypto)
-(import lib [config hash-id])
+(import hyjinx [crypto])
+(import hyjinx.lib [config hash-id])
 
 
 (setv sender-id (. (uuid1) hex))
 
 (setv HYJINX_PROTOCOL_VERSION "0.0.2")
 
 (setv keys (crypto.keys (config "passphrase"))
```

### Comparing `hyjinx-0.28.9/hyjinx/zmq_client.hy` & `hyjinx-0.29.0/hyjinx/zmq_client.hy`

 * *Files 21% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 (import json)
 (import zmq)
 
 (import hyjinx.wire [wrap unwrap zerror])
 (import hyjinx.lib [config])
 
 
-(setv context (zmq.Context))
+(setv _context (zmq.Context))
 
-(setv conf (config "client.toml")
+(setv _conf (config "client.toml")
       REQUEST_TIMEOUT_S 20
-      context (zmq.Context))
+      _context (zmq.Context))
 
 (defn start-socket []
-  (setv socket (.socket context zmq.REQ))
+  (setv socket (.socket _context zmq.REQ))
   ; see https://stackoverflow.com/questions/26915347/zeromq-reset-req-rep-socket-state
   (.setsockopt socket zmq.RCVTIMEO (* REQUEST_TIMEOUT_S 1000))
   (.setsockopt socket zmq.REQ_CORRELATE 1)
   (.setsockopt socket zmq.REQ_RELAXED 1)
   (.setsockopt socket zmq.LINGER 1000)
-  (.connect socket f"tcp://{(:server conf)}:{(:port conf)}")
+  (.connect socket f"tcp://{(:server _conf)}:{(:port _conf)}")
   socket)
 
 (setv socket (start-socket))
 
 (defn rpc [method #* args #** kwargs]
   "Call a method on the server. Return None for timeout."
   (try
```

### Comparing `hyjinx-0.28.9/hyjinx/zmq_server.hy` & `hyjinx-0.29.0/hyjinx/zmq_server.hy`

 * *Files 3% similar despite different names*

```diff
@@ -18,47 +18,47 @@
 
 (setv SendError (Exception "Message (reply) send failed.")
       ServerError (Exception))
 
 (setv N_CONCURRENT_CLIENTS 1000
       BACKGROUND_TICK 1)
 
-(setv conf (config "server.toml")
+(setv _conf (config "server.toml")
       context (zmq.asyncio.Context)
       socket (.socket context zmq.ROUTER))
 
 (defn start-router-socket [address]
   (setv socket (.socket context zmq.ROUTER))
   ; see https://stackoverflow.com/questions/26915347/zeromq-reset-req-rep-socket-state
   ; server will tick every 2s
   (.setsockopt socket zmq.RCVTIMEO 2000)
   (.setsockopt socket zmq.SNDTIMEO 1000)
   (.setsockopt socket zmq.LINGER 2000)
   (.bind socket address)
   socket)
 
-(setv frontend (start-router-socket (:listen conf)))
+(setv frontend (start-router-socket (:listen _conf)))
 
 
-(defn/a send [zmsg]
+(defn :async send [zmsg]
   "Send a reply to a client."
   (try
     (await (.send-multipart frontend zmsg))
     (except [zmq.EAGAIN]
       (raise SendError))))
   
 (defn verify [pub-key msg]
   "Check the message against its signature."
   (let [payload (:payload msg {})
         signature (:signature msg "")
         client-time (:sender-time msg Inf)
         expected-hash (hash-id (+ client-time (json.dumps payload)))]
     (crypto.verify pub-key signature expected-hash)))
 
-(defn/a server-loop [f [id 0]]
+(defn :async server-loop [f [id 0]]
   "Wait for a message, then call (f msg).
 For example, f may verify signature, then call a method, then send the reply (verified rpc)."
   (while True
     (try
       (await (f (await (.recv-multipart frontend))))
       (except [zmq.Again])
       (except [KeyboardInterrupt]
```

