# Comparing `tmp/packaged-0.5.1.tar.gz` & `tmp/packaged-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaged-0.5.1.tar", last modified: Mon May 20 20:04:50 2024, max compression
+gzip compressed data, was "packaged-0.5.2.tar", last modified: Tue May 21 21:28:39 2024, max compression
```

## Comparing `packaged-0.5.1.tar` & `packaged-0.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-20 20:04:50.159187 packaged-0.5.1/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)    18089 2024-05-14 12:10:36.000000 packaged-0.5.1/LICENSE
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     5070 2024-05-20 20:04:50.159102 packaged-0.5.1/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3790 2024-05-20 14:37:13.000000 packaged-0.5.1/README.md
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1357 2024-05-20 20:04:50.159771 packaged-0.5.1/setup.cfg
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-09 19:00:34.000000 packaged-0.5.1/setup.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-20 20:04:50.155021 packaged-0.5.1/src/
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-20 20:04:50.157627 packaged-0.5.1/src/packaged/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     7620 2024-05-20 19:53:18.000000 packaged-0.5.1/src/packaged/__init__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.5.1/src/packaged/__main__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2555 2024-05-17 13:49:45.000000 packaged-0.5.1/src/packaged/cli.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1536 2024-05-17 13:49:45.000000 packaged-0.5.1/src/packaged/config.py
--rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    19207 2024-05-14 12:16:01.000000 packaged-0.5.1/src/packaged/makeself-header.sh
--rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    21228 2024-05-13 10:09:30.000000 packaged-0.5.1/src/packaged/makeself.sh
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.5.1/src/packaged/py.typed
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-20 20:04:50.158547 packaged-0.5.1/src/packaged.egg-info/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     5070 2024-05-20 20:04:50.000000 packaged-0.5.1/src/packaged.egg-info/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      426 2024-05-20 20:04:50.000000 packaged-0.5.1/src/packaged.egg-info/SOURCES.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-20 20:04:50.000000 packaged-0.5.1/src/packaged.egg-info/dependency_links.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-20 20:04:50.000000 packaged-0.5.1/src/packaged.egg-info/entry_points.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      119 2024-05-20 20:04:50.000000 packaged-0.5.1/src/packaged.egg-info/requires.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-20 20:04:50.000000 packaged-0.5.1/src/packaged.egg-info/top_level.txt
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-21 21:28:39.452284 packaged-0.5.2/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)    18089 2024-05-14 12:10:36.000000 packaged-0.5.2/LICENSE
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     5129 2024-05-21 21:28:39.452216 packaged-0.5.2/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3849 2024-05-21 17:24:55.000000 packaged-0.5.2/README.md
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1357 2024-05-21 21:28:39.452666 packaged-0.5.2/setup.cfg
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-09 19:00:34.000000 packaged-0.5.2/setup.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-21 21:28:39.447801 packaged-0.5.2/src/
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-21 21:28:39.450467 packaged-0.5.2/src/packaged/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     7863 2024-05-21 20:19:07.000000 packaged-0.5.2/src/packaged/__init__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.5.2/src/packaged/__main__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2722 2024-05-21 20:18:41.000000 packaged-0.5.2/src/packaged/cli.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1610 2024-05-21 20:18:41.000000 packaged-0.5.2/src/packaged/config.py
+-rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    19207 2024-05-14 12:16:01.000000 packaged-0.5.2/src/packaged/makeself-header.sh
+-rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    21228 2024-05-13 10:09:30.000000 packaged-0.5.2/src/packaged/makeself.sh
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.5.2/src/packaged/py.typed
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-21 21:28:39.451614 packaged-0.5.2/src/packaged.egg-info/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     5129 2024-05-21 21:28:39.000000 packaged-0.5.2/src/packaged.egg-info/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      426 2024-05-21 21:28:39.000000 packaged-0.5.2/src/packaged.egg-info/SOURCES.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-21 21:28:39.000000 packaged-0.5.2/src/packaged.egg-info/dependency_links.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-21 21:28:39.000000 packaged-0.5.2/src/packaged.egg-info/entry_points.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      119 2024-05-21 21:28:39.000000 packaged-0.5.2/src/packaged.egg-info/requires.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-21 21:28:39.000000 packaged-0.5.2/src/packaged.egg-info/top_level.txt
```

### Comparing `packaged-0.5.1/LICENSE` & `packaged-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `packaged-0.5.1/PKG-INFO` & `packaged-0.5.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaged
-Version: 0.5.1
+Version: 0.5.2
 Summary: The easiest way to ship python applications.
 Home-page: https://github.com/tusharsadhwani/packaged
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: GPL-2.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -31,14 +31,16 @@
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 
 # packaged
 
 The easiest way to ship python applications.
 
+### Demo apps available on the website: [packaged.live](https://packaged.live)
+
 ![Demo](https://raw.githubusercontent.com/tusharsadhwani/packaged/main/demo.jpg)
 
 `packaged` can take any Python project, and package it into a self contained
 executable, that can run on other machines without needing Python installed.
 
 ## Installation
 
@@ -60,16 +62,15 @@
 
 ## Examples
 
 All examples below create a self contained executable. You can send the produced
 binary file to another machine with the same OS and architecture, and it will
 run the same.
 
-You can also download pre-built binaries for these packages from the
-[Releases page](https://github.com/tusharsadhwani/packaged/releases/latest).
+You can also find the pre-built binaries on the [Releases page](https://github.com/tusharsadhwani/packaged/releases/latest).
 
 ### Mandelbrot (`numpy`, `matplotlib`, GUI)
 
 ```bash
 packaged ./mandelbrot.bin 'pip install -r requirements.txt' 'python mandelbrot.py' ./example/mandelbrot
 ```
```

### Comparing `packaged-0.5.1/README.md` & `packaged-0.5.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # packaged
 
 The easiest way to ship python applications.
 
+### Demo apps available on the website: [packaged.live](https://packaged.live)
+
 ![Demo](https://raw.githubusercontent.com/tusharsadhwani/packaged/main/demo.jpg)
 
 `packaged` can take any Python project, and package it into a self contained
 executable, that can run on other machines without needing Python installed.
 
 ## Installation
 
@@ -27,16 +29,15 @@
 
 ## Examples
 
 All examples below create a self contained executable. You can send the produced
 binary file to another machine with the same OS and architecture, and it will
 run the same.
 
-You can also download pre-built binaries for these packages from the
-[Releases page](https://github.com/tusharsadhwani/packaged/releases/latest).
+You can also find the pre-built binaries on the [Releases page](https://github.com/tusharsadhwani/packaged/releases/latest).
 
 ### Mandelbrot (`numpy`, `matplotlib`, GUI)
 
 ```bash
 packaged ./mandelbrot.bin 'pip install -r requirements.txt' 'python mandelbrot.py' ./example/mandelbrot
 ```
```

### Comparing `packaged-0.5.1/setup.cfg` & `packaged-0.5.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = packaged
-version = 0.5.1
+version = 0.5.2
 description = The easiest way to ship python applications.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tusharsadhwani/packaged
 author = Tushar Sadhwani
 author_email = tushar.sadhwani000@gmail.com
 license = GPL-2.0-or-later
```

### Comparing `packaged-0.5.1/src/packaged/__init__.py` & `packaged-0.5.2/src/packaged/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,23 @@
 from __future__ import annotations
 
 import os.path
 import shutil
 import subprocess
 import sys
 import tempfile
+from typing import cast, TYPE_CHECKING
+from unittest import mock
 
 import yen.github
 from yaspin import yaspin
 
+if TYPE_CHECKING:
+    from yaspin.core import Yaspin
+
 MAKESELF_PATH = os.path.join(os.path.dirname(__file__), "makeself.sh")
 DEFAULT_PYTHON_VERSION = "3.12"
 PACKAGED_PYTHON_FOLDER_NAME = ".packaged_python"
 
 
 class SourceDirectoryNotFound(Exception):
     """Raised when provided directory to package does not exist."""
@@ -34,14 +39,15 @@
 
 def create_package(
     source_directory: str | None,
     output_path: str,
     build_command: str,
     startup_command: str,
     python_version: str,
+    quiet: bool = False,
 ) -> None:
     """Create the makeself executable, with the startup script in it."""
     if source_directory is None:
         source_directory = tempfile.mkdtemp()
 
     if not os.path.isdir(source_directory):
         raise SourceDirectoryNotFound(source_directory)
@@ -66,28 +72,32 @@
         python_bin_folder = os.path.join(
             packaged_python_path, os.path.dirname(yen_python_bin_relpath)
         )
         python_bin_folder_relpath = os.path.relpath(python_bin_folder, source_directory)
 
         # Run the build command in the source directory, while making sure
         # that `python` and related binaries point to the installed python
-        spinner = yaspin(text="Running the build command...")
+        if quiet:
+            spinner = cast("Yaspin", mock.Mock())
+        else:
+            spinner = yaspin(text="Running the build command...")
+
         spinner.start()
         try:
             subprocess.run(
                 [build_command],
                 shell=True,
                 env={
                     "PATH": os.pathsep.join(
                         [python_bin_folder, os.environ.get("PATH", "")]
                     )
                 },
                 cwd=source_directory,
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
+                check=True,
+                capture_output=True,
             )
         except subprocess.CalledProcessError as exc:
             spinner.stop()
             print("*** Build Failed:", file=sys.stderr)
             print("Stdout:\n" + exc.stdout.decode(errors="ignore"), file=sys.stderr)
             print("Stderr:\n" + exc.stdout.decode(errors="ignore"), file=sys.stderr)
             raise
@@ -173,15 +183,17 @@
             print("*** Makeself Failed:", file=sys.stderr)
             print("Stdout:\n" + exc.stdout.decode(errors="ignore"), file=sys.stderr)
             print("Stderr:\n" + exc.stdout.decode(errors="ignore"), file=sys.stderr)
             raise
 
     finally:
         spinner.stop()
-        print(f"Package {output_path!r} built successfully!")
+        if not quiet:
+            print(f"Package {output_path!r} built successfully!")
+
         # Cleanup the packaged python and startup script from source directory
         if os.path.exists(startup_script_path):
             os.remove(startup_script_path)
         if os.path.exists(packaged_python_path):
             shutil.rmtree(packaged_python_path)
```

### Comparing `packaged-0.5.1/src/packaged/cli.py` & `packaged-0.5.2/src/packaged/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """CLI interface for packaged."""
 
 from __future__ import annotations
 
 import argparse
-import dataclasses
 import os.path
 import platform
 import sys
-import typing
 
 from packaged import (
     DEFAULT_PYTHON_VERSION,
     PythonNotAvailable,
     SourceDirectoryNotFound,
     create_package,
 )
@@ -65,24 +63,31 @@
         )
         parser.add_argument(
             "--python-version",
             metavar=DEFAULT_PYTHON_VERSION,
             help="Version of Python to package your project with.",
             default=DEFAULT_PYTHON_VERSION,
         )
+        parser.add_argument(
+            "--quiet",
+            help="Disable all output",
+            action="store_true",
+            default="CI" in os.environ,
+        )
         args = parser.parse_args(argv)
         config = Config(**vars(args))
 
     try:
         create_package(
             config.source_directory,
             config.output_path,
             config.build_command,
             config.startup_command,
             config.python_version,
+            config.quiet,
         )
     except SourceDirectoryNotFound as exc:
         error(f"Folder {exc.directory_path!r} does not exist.")
         return 4
     except PythonNotAvailable as exc:
         error(f"Python {exc.python_version!r} is not available for download.")
         return 5
```

### Comparing `packaged-0.5.1/src/packaged/config.py` & `packaged-0.5.2/src/packaged/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 @dataclass
 class Config:
     source_directory: str | None
     output_path: str
     build_command: str
     startup_command: str
     python_version: str
+    quiet: bool
 
 
 CONFIG_NAME = "./packaged.toml"
 
 
 def config_file_exists(source_directory: str) -> bool:
     """Returns true if `packaged.toml` exists in current directory."""
@@ -50,13 +51,14 @@
     try:
         config = Config(
             os.path.abspath(source_directory),
             config_data["output_path"],
             config_data["build_command"],
             config_data["startup_command"],
             config_data.get("python_version", "3.12"),
+            config_data.get("quiet", "CI" in os.environ),
         )
     except KeyError as exc:
         key = exc.args[0]
         raise ConfigValidationError(key)
 
     return config
```

### Comparing `packaged-0.5.1/src/packaged/makeself-header.sh` & `packaged-0.5.2/src/packaged/makeself-header.sh`

 * *Files identical despite different names*

### Comparing `packaged-0.5.1/src/packaged/makeself.sh` & `packaged-0.5.2/src/packaged/makeself.sh`

 * *Files identical despite different names*

### Comparing `packaged-0.5.1/src/packaged.egg-info/PKG-INFO` & `packaged-0.5.2/src/packaged.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaged
-Version: 0.5.1
+Version: 0.5.2
 Summary: The easiest way to ship python applications.
 Home-page: https://github.com/tusharsadhwani/packaged
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: GPL-2.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -31,14 +31,16 @@
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 
 # packaged
 
 The easiest way to ship python applications.
 
+### Demo apps available on the website: [packaged.live](https://packaged.live)
+
 ![Demo](https://raw.githubusercontent.com/tusharsadhwani/packaged/main/demo.jpg)
 
 `packaged` can take any Python project, and package it into a self contained
 executable, that can run on other machines without needing Python installed.
 
 ## Installation
 
@@ -60,16 +62,15 @@
 
 ## Examples
 
 All examples below create a self contained executable. You can send the produced
 binary file to another machine with the same OS and architecture, and it will
 run the same.
 
-You can also download pre-built binaries for these packages from the
-[Releases page](https://github.com/tusharsadhwani/packaged/releases/latest).
+You can also find the pre-built binaries on the [Releases page](https://github.com/tusharsadhwani/packaged/releases/latest).
 
 ### Mandelbrot (`numpy`, `matplotlib`, GUI)
 
 ```bash
 packaged ./mandelbrot.bin 'pip install -r requirements.txt' 'python mandelbrot.py' ./example/mandelbrot
 ```
```

