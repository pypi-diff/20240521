# Comparing `tmp/biliass-1.3.7.dev3.tar.gz` & `tmp/biliass-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biliass-1.3.7.dev3.tar", max compression
+gzip compressed data, was "biliass-1.3.8.tar", max compression
```

## Comparing `biliass-1.3.7.dev3.tar` & `biliass-1.3.8.tar`

### file list

```diff
@@ -1,77 +1,10 @@
--rw-r--r--   0        0        0    15137 2022-11-03 07:43:50.204846 biliass-1.3.7.dev3/.venv/lib/python3.10/site-packages/attr/__init__.pyi
--rw-r--r--   0        0        0      357 2022-11-03 07:43:50.205083 biliass-1.3.7.dev3/.venv/lib/python3.10/site-packages/attr/_cmp.pyi
--rw-r--r--   0        0        0      209 2022-11-03 07:43:50.206248 biliass-1.3.7.dev3/.venv/lib/python3.10/site-packages/attr/_version_info.pyi
--rw-r--r--   0        0        0      416 2022-11-03 07:43:50.206485 biliass-1.3.7.dev3/.venv/lib/python3.10/site-packages/attr/converters.pyi
--rw-r--r--   0        0        0      539 2022-11-03 07:43:50.206677 biliass-1.3.7.dev3/.venv/lib/python3.10/site-packages/attr/exceptions.pyi
--rw-r--r--   0        0        0      215 2022-11-03 07:43:50.206874 biliass-1.3.7.dev3/.venv/lib/python3.10/site-packages/attr/filters.pyi
--rw-r--r--   0        0        0      573 2022-11-03 07:43:50.208040 biliass-1.3.7.dev3/.venv/lib/python3.10/site-packages/attr/setters.pyi
--rw-r--r--   0        0        0     2355 2022-11-03 07:43:50.208727 biliass-1.3.7.dev3/.venv/lib/python3.10/site-packages/attr/validators.pyi
--rw-r--r--   0        0        0     2100 2022-11-03 07:43:50.209350 biliass-1.3.7.dev3/.venv/lib/python3.10/site-packages/attrs/__init__.pyi
--rw-r--r--   0        0        0     1205 2022-11-03 07:43:50.232102 biliass-1.3.7.dev3/.venv/lib/python3.10/site-packages/iniconfig/__init__.pyi
--rw-r--r--   0        0        0    35147 2022-02-26 20:10:19.113000 biliass-1.3.7.dev3/LICENSE
--rw-r--r--   0        0        0     2213 2022-02-26 20:17:44.022805 biliass-1.3.7.dev3/README.md
--rw-r--r--   0        0        0       88 2022-11-03 08:56:22.010324 biliass-1.3.7.dev3/biliass/__init__.py
--rw-r--r--   0        0        0     3399 2022-11-03 08:31:05.573857 biliass-1.3.7.dev3/biliass/__main__.py
--rwxr-xr-x   0        0        0    24992 2022-11-03 08:01:28.519050 biliass-1.3.7.dev3/biliass/biliass.py
--rw-r--r--   0        0        0        0 2022-02-26 20:10:04.520481 biliass-1.3.7.dev3/biliass/protobuf/__init__.py
--rw-r--r--   0        0        0     2191 2022-11-03 08:01:28.522467 biliass-1.3.7.dev3/biliass/protobuf/danmaku_pb2.py
--rw-r--r--   0        0        0      111 2022-11-03 08:01:28.523262 biliass-1.3.7.dev3/biliass/protobuf/danmaku_pb2.pyi
--rw-r--r--   0        0        0        0 2022-11-03 08:56:27.649331 biliass-1.3.7.dev3/biliass/py.typed
--rw-r--r--   0        0        0    15137 2022-11-03 07:43:50.204846 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/__init__.pyi
--rw-r--r--   0        0        0      357 2022-11-03 07:43:50.205083 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/_cmp.pyi
--rw-r--r--   0        0        0      209 2022-11-03 07:43:50.206248 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/_version_info.pyi
--rw-r--r--   0        0        0      416 2022-11-03 07:43:50.206485 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/converters.pyi
--rw-r--r--   0        0        0      539 2022-11-03 07:43:50.206677 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/exceptions.pyi
--rw-r--r--   0        0        0      215 2022-11-03 07:43:50.206874 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/filters.pyi
--rw-r--r--   0        0        0      573 2022-11-03 07:43:50.208040 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/setters.pyi
--rw-r--r--   0        0        0     2355 2022-11-03 07:43:50.208727 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/validators.pyi
--rw-r--r--   0        0        0     2100 2022-11-03 07:43:50.209350 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attrs/__init__.pyi
--rw-r--r--   0        0        0     1205 2022-11-03 07:43:50.232102 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/iniconfig/__init__.pyi
--rw-r--r--   0        0        0      111 2022-11-03 08:01:28.523262 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/biliass/protobuf/danmaku_pb2.pyi
--rw-r--r--   0        0        0    15137 2022-11-03 07:43:50.204846 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/__init__.pyi
--rw-r--r--   0        0        0      357 2022-11-03 07:43:50.205083 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/_cmp.pyi
--rw-r--r--   0        0        0      209 2022-11-03 07:43:50.206248 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/_version_info.pyi
--rw-r--r--   0        0        0      416 2022-11-03 07:43:50.206485 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/converters.pyi
--rw-r--r--   0        0        0      539 2022-11-03 07:43:50.206677 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/exceptions.pyi
--rw-r--r--   0        0        0      215 2022-11-03 07:43:50.206874 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/filters.pyi
--rw-r--r--   0        0        0      573 2022-11-03 07:43:50.208040 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/setters.pyi
--rw-r--r--   0        0        0     2355 2022-11-03 07:43:50.208727 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/validators.pyi
--rw-r--r--   0        0        0     2100 2022-11-03 07:43:50.209350 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attrs/__init__.pyi
--rw-r--r--   0        0        0     1205 2022-11-03 07:43:50.232102 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/iniconfig/__init__.pyi
--rw-r--r--   0        0        0      111 2022-11-03 08:01:28.523262 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/biliass/protobuf/danmaku_pb2.pyi
--rw-r--r--   0        0        0    15137 2022-11-03 07:43:50.204846 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/.venv/lib/python3.10/site-packages/attr/__init__.pyi
--rw-r--r--   0        0        0      357 2022-11-03 07:43:50.205083 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/.venv/lib/python3.10/site-packages/attr/_cmp.pyi
--rw-r--r--   0        0        0      209 2022-11-03 07:43:50.206248 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/.venv/lib/python3.10/site-packages/attr/_version_info.pyi
--rw-r--r--   0        0        0      416 2022-11-03 07:43:50.206485 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/.venv/lib/python3.10/site-packages/attr/converters.pyi
--rw-r--r--   0        0        0      539 2022-11-03 07:43:50.206677 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/.venv/lib/python3.10/site-packages/attr/exceptions.pyi
--rw-r--r--   0        0        0      215 2022-11-03 07:43:50.206874 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/.venv/lib/python3.10/site-packages/attr/filters.pyi
--rw-r--r--   0        0        0      573 2022-11-03 07:43:50.208040 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/.venv/lib/python3.10/site-packages/attr/setters.pyi
--rw-r--r--   0        0        0     2355 2022-11-03 07:43:50.208727 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/.venv/lib/python3.10/site-packages/attr/validators.pyi
--rw-r--r--   0        0        0     2100 2022-11-03 07:43:50.209350 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/.venv/lib/python3.10/site-packages/attrs/__init__.pyi
--rw-r--r--   0        0        0     1205 2022-11-03 07:43:50.232102 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/.venv/lib/python3.10/site-packages/iniconfig/__init__.pyi
--rw-r--r--   0        0        0      111 2022-11-03 08:01:28.523262 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/biliass/protobuf/danmaku_pb2.pyi
--rw-r--r--   0        0        0    15137 2022-11-03 07:43:50.204846 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/__init__.pyi
--rw-r--r--   0        0        0      357 2022-11-03 07:43:50.205083 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/_cmp.pyi
--rw-r--r--   0        0        0      209 2022-11-03 07:43:50.206248 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/_version_info.pyi
--rw-r--r--   0        0        0      416 2022-11-03 07:43:50.206485 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/converters.pyi
--rw-r--r--   0        0        0      539 2022-11-03 07:43:50.206677 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/exceptions.pyi
--rw-r--r--   0        0        0      215 2022-11-03 07:43:50.206874 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/filters.pyi
--rw-r--r--   0        0        0      573 2022-11-03 07:43:50.208040 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/setters.pyi
--rw-r--r--   0        0        0     2355 2022-11-03 07:43:50.208727 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/validators.pyi
--rw-r--r--   0        0        0     2100 2022-11-03 07:43:50.209350 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attrs/__init__.pyi
--rw-r--r--   0        0        0     1205 2022-11-03 07:43:50.232102 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/iniconfig/__init__.pyi
--rw-r--r--   0        0        0      111 2022-11-03 08:01:28.523262 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/biliass/protobuf/danmaku_pb2.pyi
--rw-r--r--   0        0        0    15137 2022-11-03 07:43:50.204846 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/__init__.pyi
--rw-r--r--   0        0        0      357 2022-11-03 07:43:50.205083 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/_cmp.pyi
--rw-r--r--   0        0        0      209 2022-11-03 07:43:50.206248 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/_version_info.pyi
--rw-r--r--   0        0        0      416 2022-11-03 07:43:50.206485 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/converters.pyi
--rw-r--r--   0        0        0      539 2022-11-03 07:43:50.206677 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/exceptions.pyi
--rw-r--r--   0        0        0      215 2022-11-03 07:43:50.206874 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/filters.pyi
--rw-r--r--   0        0        0      573 2022-11-03 07:43:50.208040 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/setters.pyi
--rw-r--r--   0        0        0     2355 2022-11-03 07:43:50.208727 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attr/validators.pyi
--rw-r--r--   0        0        0     2100 2022-11-03 07:43:50.209350 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/attrs/__init__.pyi
--rw-r--r--   0        0        0     1205 2022-11-03 07:43:50.232102 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/.venv/lib/python3.10/site-packages/iniconfig/__init__.pyi
--rw-r--r--   0        0        0      111 2022-11-03 08:01:28.523262 biliass-1.3.7.dev3/dist/biliass-1.3.7.dev2 2/dist/biliass-1.3.7.dev2/dist/biliass-1.3.7.dev2/biliass/protobuf/danmaku_pb2.pyi
--rw-r--r--   0        0        0     1407 2022-11-03 08:56:21.952347 biliass-1.3.7.dev3/pyproject.toml
--rw-r--r--   0        0        0     3061 1970-01-01 00:00:00.000000 biliass-1.3.7.dev3/setup.py
--rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 biliass-1.3.7.dev3/PKG-INFO
+-rw-r--r--   0        0        0    35125 2024-05-21 15:21:58.055116 biliass-1.3.8/LICENSE
+-rw-r--r--   0        0        0     2213 2024-05-21 15:21:58.055116 biliass-1.3.8/README.md
+-rw-r--r--   0        0        0      164 2024-05-21 15:21:58.055116 biliass-1.3.8/biliass/__init__.py
+-rw-r--r--   0        0        0     3381 2024-05-21 15:21:58.055116 biliass-1.3.8/biliass/__main__.py
+-rwxr-xr-x   0        0        0    24891 2024-05-21 15:21:58.055116 biliass-1.3.8/biliass/biliass.py
+-rw-r--r--   0        0        0        0 2024-05-21 15:21:58.055116 biliass-1.3.8/biliass/protobuf/__init__.py
+-rw-r--r--   0        0        0     2191 2024-05-21 15:21:58.055116 biliass-1.3.8/biliass/protobuf/danmaku_pb2.py
+-rw-r--r--   0        0        0       75 2024-05-21 15:21:58.055116 biliass-1.3.8/biliass/protobuf/danmaku_pb2.pyi
+-rw-r--r--   0        0        0     1897 2024-05-21 15:21:58.055116 biliass-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0     3192 1970-01-01 00:00:00.000000 biliass-1.3.8/PKG-INFO
```

### Comparing `biliass-1.3.7.dev3/LICENSE` & `biliass-1.3.8/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -627,16 +627,16 @@
 free software which everyone can redistribute and change under these terms.
 
   To do so, attach the following notices to the program.  It is safest
 to attach them to the start of each source file to most effectively
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
+    biliass, convert bilibili XML and protobuf danmaku into ASS
+    Copyright (C) 2024  Nyakku Shigure
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
@@ -648,15 +648,15 @@
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
   If the program does terminal interaction, make it output a short
 notice like this when it starts in an interactive mode:
 
-    <program>  Copyright (C) <year>  <name of author>
+    biliass  Copyright (C) 2024  Nyakku Shigure
     This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
     This is free software, and you are welcome to redistribute it
     under certain conditions; type `show c' for details.
 
 The hypothetical commands `show w' and `show c' should show the appropriate
 parts of the General Public License.  Of course, your program's commands
 might be different; for a GUI interface, you would use an "about box".
```

### Comparing `biliass-1.3.7.dev3/README.md` & `biliass-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `biliass-1.3.7.dev3/biliass/__main__.py` & `biliass-1.3.8/biliass/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,66 +9,68 @@
 
 
 def main():
     logging.basicConfig(format="%(levelname)s: %(message)s")
     if len(sys.argv) == 1:
         sys.argv.append("--help")
     parser = argparse.ArgumentParser(description="bilibili ASS Danmaku converter", prog="biliass")
-    parser.add_argument("-v", "--version", action="version", version="%(prog)s {}".format(biliass_version))
+    parser.add_argument("-v", "--version", action="version", version=f"%(prog)s {biliass_version}")
     parser.add_argument("-o", "--output", metavar="OUTPUT", help="Output file")
     parser.add_argument("-s", "--size", metavar="WIDTHxHEIGHT", required=True, help="Stage size in pixels")
     parser.add_argument(
         "-fn",
         "--font",
         metavar="FONT",
-        help="Specify font face [default: %s]" % "sans-serif",
+        help="Specify font face [default: sans-serif]",
         default="sans-serif",
     )
     parser.add_argument(
         "-fs",
         "--fontsize",
         metavar="SIZE",
-        help=("Default font size [default: %s]" % 25),
+        help="Default font size [default: 25]",
         type=float,
         default=25.0,
     )
     parser.add_argument("-a", "--alpha", metavar="ALPHA", help="Text opacity", type=float, default=1.0)
     parser.add_argument(
         "-dm",
         "--duration-marquee",
         metavar="SECONDS",
-        help="Duration of scrolling comment display [default: %s]" % 5,
+        help="Duration of scrolling comment display [default: 5]",
         type=float,
         default=5.0,
     )
     parser.add_argument(
         "-ds",
         "--duration-still",
         metavar="SECONDS",
-        help="Duration of still comment display [default: %s]" % 5,
+        help="Duration of still comment display [default: 5]",
         type=float,
         default=5.0,
     )
     parser.add_argument("-fl", "--filter", help="Regular expression to filter comments")
     parser.add_argument(
         "-flf", "--filter-file", help="Regular expressions from file (one line one regex) to filter comments"
     )
     parser.add_argument(
         "-p", "--protect", metavar="HEIGHT", help="Reserve blank on the bottom of the stage", type=int, default=0
     )
     parser.add_argument("-r", "--reduce", action="store_true", help="Reduce the amount of comments if stage is full")
-    parser.add_argument("-f", "--format", choices=["xml", "protobuf"], default="xml", help="Input danmaku format (xml or protobuf)")
+    parser.add_argument(
+        "-f", "--format", choices=["xml", "protobuf"], default="xml", help="Input danmaku format (xml or protobuf)"
+    )
     parser.add_argument("file", metavar="FILE", nargs="+", help="Comment file to be processed")
     args = parser.parse_args()
     try:
         width, height = str(args.size).split("x", 1)
         width = int(width)
         height = int(height)
     except ValueError:
-        raise ValueError("Invalid stage size: %r" % args.size)
+        raise ValueError(f"Invalid stage size: {args.size!r}")
 
     inputs = []
     for file in args.file:
         try:
             with open(file, "r" if args.format == "xml" else "rb") as f:
                 inputs.append(f.read())
         except UnicodeDecodeError:
```

### Comparing `biliass-1.3.7.dev3/biliass/biliass.py` & `biliass-1.3.8/biliass/biliass.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 import json
 import logging
 import math
 import random
 import re
 import xml.dom.minidom
-from typing import Callable, Generator, List, Optional, Tuple, Union
+from collections.abc import Generator
+from typing import Callable, Tuple, TypeVar, Union
 
 from biliass.protobuf.danmaku_pb2 import DanmakuEvent
 
 #
 # ReadComments**** protocol
 #
 # Input:
@@ -36,34 +37,25 @@
 #     height:    The estimated height in pixels
 #                i.e. (comment.count('\n')+1)*size
 #     width:     The estimated width in pixels
 #                i.e. CalculateLength(comment)*size
 #
 
 
-def export(func):
-    global __all__
-    try:
-        __all__.append(func.__name__)
-    except NameError:
-        __all__ = [func.__name__]
-    return func
-
-
+T = TypeVar("T")
 Comment = Tuple[float, float, int, str, Union[int, str], int, float, float, float]
 
 
-@export
-def ReadCommentsBilibiliXml(text: Union[str, bytes], fontsize: float) -> Generator[Comment, None, None]:
+def ReadCommentsBilibiliXml(text: str | bytes, fontsize: float) -> Generator[Comment, None, None]:
     if isinstance(text, bytes):
         text = text.decode()
     text = FilterBadChars(text)
     dom = xml.dom.minidom.parseString(text)
     version = dom.version
-    assert version in ["1.0", "2.0"], "未知的 XML 版本号 {}".format(version)
+    assert version in ["1.0", "2.0"], f"未知的 XML 版本号 {version}"
     if version == "1.0":
         return ReadCommentsBilibiliXmlV1(text, fontsize)
     else:
         return ReadCommentsBilibiliXmlV2(text, fontsize)
 
 
 def ReadCommentsBilibiliXmlV1(text: str, fontsize: float) -> Generator[Comment, None, None]:
@@ -91,15 +83,15 @@
                     )
                 elif p[1] == "7":  # positioned comment
                     c = str(comment.childNodes[0].wholeText)
                     yield (float(p[0]), int(p[4]), i, c, "bilipos", int(p[3]), int(p[2]), 0, 0)
                 elif p[1] == "8":
                     pass  # ignore scripted comment
         except (AssertionError, AttributeError, IndexError, TypeError, ValueError):
-            logging.warning("Invalid comment: %s" % comment.toxml())
+            logging.warning(f"Invalid comment: {comment.toxml()}")
             continue
 
 
 def ReadCommentsBilibiliXmlV2(text: str, fontsize: float) -> Generator[Comment, None, None]:
     dom = xml.dom.minidom.parseString(text)
     comment_element = dom.getElementsByTagName("d")
     for i, comment in enumerate(comment_element):
@@ -125,20 +117,19 @@
                     )
                 elif p[3] == "7":  # positioned comment
                     c = str(comment.childNodes[0].wholeText)
                     yield (time, int(p[6]), i, c, "bilipos", int(p[5]), int(p[4]), 0, 0)
                 elif p[3] == "8":
                     pass  # ignore scripted comment
         except (AssertionError, AttributeError, IndexError, TypeError, ValueError):
-            logging.warning("Invalid comment: %s" % comment.toxml())
+            logging.warning(f"Invalid comment: {comment.toxml()}")
             continue
 
 
-@export
-def ReadCommentsBilibiliProtobuf(protobuf: Union[bytes, str], fontsize: float) -> Generator[Comment, None, None]:
+def ReadCommentsBilibiliProtobuf(protobuf: bytes | str, fontsize: float) -> Generator[Comment, None, None]:
     assert isinstance(protobuf, bytes), "protobuf 仅支持使用 bytes 转换"
     target = DanmakuEvent()
     target.ParseFromString(protobuf)
     for i, elem in enumerate(target.elems):
         try:
             assert elem.mode in (1, 4, 5, 6, 7, 8)
             if elem.mode in (1, 4, 5, 6):
@@ -157,15 +148,15 @@
                 )
             elif elem.mode == 7:  # positioned comment
                 c = elem.content
                 yield (elem.progress / 1000, elem.ctime, i, c, "bilipos", elem.color, elem.fontsize, 0, 0)
             elif elem.mode == 8:
                 pass  # ignore scripted comment
         except (AssertionError, AttributeError, IndexError, TypeError, ValueError):
-            logging.warning("Invalid comment: %s" % elem.content)
+            logging.warning(f"Invalid comment: {elem.content}")
             continue
 
 
 class AssText:
     def __init__(self):
         self._text = ""
 
@@ -206,66 +197,66 @@
             alpha = safe_list(str(comment_args.get(2, "1")).split("-"))
             from_alpha = float(alpha.get(0, 1))
             to_alpha = float(alpha.get(1, from_alpha))
             from_alpha = 255 - round(from_alpha * 255)
             to_alpha = 255 - round(to_alpha * 255)
             rotate_z = int(comment_args.get(5, 0))
             rotate_y = int(comment_args.get(6, 0))
-            lifetime = float(comment_args.get(3, 4500))
+            lifetime = float(wrap_default(comment_args.get(3, 4500), 4500))
             duration = int(comment_args.get(9, lifetime * 1000))
             delay = int(comment_args.get(10, 0))
             fontface = comment_args.get(12)
             isborder = comment_args.get(11, "true")
             from_rotarg = ConvertFlashRotation(rotate_y, rotate_z, from_x, from_y, width, height)
             to_rotarg = ConvertFlashRotation(rotate_y, rotate_z, to_x, to_y, width, height)
             styles = ["\\org(%d, %d)" % (width / 2, height / 2)]
             if from_rotarg[0:2] == to_rotarg[0:2]:
-                styles.append("\\pos(%.0f, %.0f)" % (from_rotarg[0:2]))
+                styles.append("\\pos({:.0f}, {:.0f})".format(*from_rotarg[0:2]))
             else:
                 styles.append(
-                    "\\move(%.0f, %.0f, %.0f, %.0f, %.0f, %.0f)"
-                    % (from_rotarg[0:2] + to_rotarg[0:2] + (delay, delay + duration))
+                    "\\move({:.0f}, {:.0f}, {:.0f}, {:.0f}, {:.0f}, {:.0f})".format(
+                        *(from_rotarg[0:2] + to_rotarg[0:2] + (delay, delay + duration))
+                    )
                 )
-            styles.append("\\frx%.0f\\fry%.0f\\frz%.0f\\fscx%.0f\\fscy%.0f" % (from_rotarg[2:7]))
+            styles.append("\\frx{:.0f}\\fry{:.0f}\\frz{:.0f}\\fscx{:.0f}\\fscy{:.0f}".format(*from_rotarg[2:7]))
             if (from_x, from_y) != (to_x, to_y):
-                styles.append("\\t(%d, %d, " % (delay, delay + duration))
-                styles.append("\\frx%.0f\\fry%.0f\\frz%.0f\\fscx%.0f\\fscy%.0f" % (to_rotarg[2:7]))
+                styles.append(f"\\t({delay:d}, {delay + duration:d}, ")
+                styles.append("\\frx{:.0f}\\fry{:.0f}\\frz{:.0f}\\fscx{:.0f}\\fscy{:.0f}".format(*to_rotarg[2:7]))
                 styles.append(")")
             if fontface:
-                styles.append("\\fn%s" % ASSEscape(fontface))
+                styles.append(f"\\fn{ASSEscape(fontface)}")
             styles.append("\\fs%.0f" % (c[6] * ZoomFactor[0]))
             if c[5] != 0xFFFFFF:
-                styles.append("\\c&H%s&" % ConvertColor(c[5]))
+                styles.append(f"\\c&H{ConvertColor(c[5])}&")
                 if c[5] == 0x000000:
                     styles.append("\\3c&HFFFFFF&")
             if from_alpha == to_alpha:
-                styles.append("\\alpha&H%02X" % from_alpha)
+                styles.append(f"\\alpha&H{from_alpha:02X}")
             elif (from_alpha, to_alpha) == (255, 0):
-                styles.append("\\fad(%.0f,0)" % (lifetime * 1000))
+                styles.append(f"\\fad({lifetime * 1000:.0f},0)")
             elif (from_alpha, to_alpha) == (0, 255):
-                styles.append("\\fad(0, %.0f)" % (lifetime * 1000))
+                styles.append(f"\\fad(0, {lifetime * 1000:.0f})")
             else:
                 styles.append(
-                    "\\fade(%(from_alpha)d, %(to_alpha)d, %(to_alpha)d, 0, %(end_time).0f, %(end_time).0f, %(end_time).0f)"
-                    % {"from_alpha": from_alpha, "to_alpha": to_alpha, "end_time": lifetime * 1000}
+                    f"\\fade({from_alpha:d}, {to_alpha:d}, {to_alpha:d}, 0, {lifetime * 1000:.0f}, {lifetime * 1000:.0f}, {lifetime * 1000:.0f})"
                 )
             if isborder == "false":
                 styles.append("\\bord0")
-            self._text += "Dialogue: -1,%(start)s,%(end)s,%(styleid)s,,0,0,0,,{%(styles)s}%(text)s\n" % {
-                "start": ConvertTimestamp(c[0]),
-                "end": ConvertTimestamp(c[0] + lifetime),
-                "styles": "".join(styles),
-                "text": text,
-                "styleid": styleid,
-            }
-        except (IndexError, ValueError) as e:
+            self._text += "Dialogue: -1,{start},{end},{styleid},,0,0,0,,{{{styles}}}{text}\n".format(
+                start=ConvertTimestamp(c[0]),
+                end=ConvertTimestamp(c[0] + lifetime),
+                styles="".join(styles),
+                text=text,
+                styleid=styleid,
+            )
+        except (IndexError, ValueError):
             try:
-                logging.warning("Invalid comment: %r" % c[3])
+                logging.warning(f"Invalid comment: {c[3]:r}")
             except IndexError:
-                logging.warning("Invalid comment: %r" % c)
+                logging.warning(f"Invalid comment: {c:r}")
 
     def WriteASSHead(self, width, height, fontface, fontsize, alpha, styleid):
         self._text += """[Script Info]
 ; Script generated by biliass (based on Danmaku2ASS)
 ; https://github.com/yutto-dev/biliass
 Script Updated By: biliass (https://github.com/yutto-dev/biliass)
 ScriptType: v4.00+
@@ -314,26 +305,26 @@
         else:
             styles.append(
                 "\\move(%(width)d, %(row)d, %(neglen)d, %(row)d)"
                 % {"width": width, "row": row, "neglen": -math.ceil(c[8])}
             )
             duration = duration_marquee
         if not (-1 < c[6] - fontsize < 1):
-            styles.append("\\fs%.0f" % c[6])
+            styles.append(f"\\fs{c[6]:.0f}")
         if c[5] != 0xFFFFFF:
-            styles.append("\\c&H%s&" % ConvertColor(c[5]))
+            styles.append(f"\\c&H{ConvertColor(c[5])}&")
             if c[5] == 0x000000:
                 styles.append("\\3c&HFFFFFF&")
-        self._text += "Dialogue: 2,%(start)s,%(end)s,%(styleid)s,,0000,0000,0000,,{%(styles)s}%(text)s\n" % {
-            "start": ConvertTimestamp(c[0]),
-            "end": ConvertTimestamp(c[0] + duration),
-            "styles": "".join(styles),
-            "text": text,
-            "styleid": styleid,
-        }
+        self._text += "Dialogue: 2,{start},{end},{styleid},,0000,0000,0000,,{{{styles}}}{text}\n".format(
+            start=ConvertTimestamp(c[0]),
+            end=ConvertTimestamp(c[0] + duration),
+            styles="".join(styles),
+            text=text,
+            styleid=styleid,
+        )
 
     def to_file(self, f):
         f.write(self._text)
 
     def to_string(self):
         return self._text
 
@@ -396,23 +387,23 @@
     )
     trY = Y * math.cos(rotZ) - X * math.sin(rotZ) + math.sin(rotZ) * width / 2 + (1 - math.cos(rotZ)) * height / 2
     trZ = (trX - width / 2) * math.sin(rotY)
     FOV = width * math.tan(2 * math.pi / 9.0) / 2
     try:
         scaleXY = FOV / (FOV + trZ)
     except ZeroDivisionError:
-        logging.error("Rotation makes object behind the camera: trZ == %.0f" % trZ)
+        logging.error(f"Rotation makes object behind the camera: trZ == {trZ:.0f}")
         scaleXY = 1
     trX = (trX - width / 2) * scaleXY + width / 2
     trY = (trY - height / 2) * scaleXY + height / 2
     if scaleXY < 0:
         scaleXY = -scaleXY
         outX += 180
         outY += 180
-        logging.error("Rotation makes object behind the camera: trZ == %.0f < %.0f" % (trZ, FOV))
+        logging.error(f"Rotation makes object behind the camera: trZ == {trZ:.0f} < {FOV:.0f}")
     return (trX, trY, WrapAngle(outX), WrapAngle(outY), WrapAngle(outZ), scaleXY * 100, scaleXY * 100)
 
 
 def ProcessComments(
     comments,
     width,
     height,
@@ -422,15 +413,15 @@
     alpha,
     duration_marquee,
     duration_still,
     filters_regex,
     reduced,
     progress_callback,
 ):
-    styleid = "biliass_%04x" % random.randint(0, 0xFFFF)
+    styleid = f"biliass_{random.randint(0, 0xFFFF):04x}"
     ass = AssText()
     ass.WriteASSHead(width, height, fontface, fontsize, alpha, styleid)
     rows = [[None] * (height - bottomReserved + 1) for i in range(4)]
     for idx, i in enumerate(comments):
         if progress_callback and idx % 1000 == 0:
             progress_callback(idx, len(comments))
         if isinstance(i[4], int):
@@ -459,15 +450,15 @@
                     MarkCommentRow(rows, i, row)
                     ass.WriteComment(
                         i, row, width, height, bottomReserved, fontsize, duration_marquee, duration_still, styleid
                     )
         elif i[4] == "bilipos":
             ass.WriteCommentBilibiliPositioned(i, width, height, styleid)
         else:
-            logging.warning("Invalid comment: %r" % i[3])
+            logging.warning(f"Invalid comment: {i[3]!r}")
     if progress_callback:
         progress_callback(len(comments), len(comments))
     return ass.to_string()
 
 
 def TestFreeRows(rows, c, row, width, height, bottomReserved, duration_marquee, duration_still):
     res = 0
@@ -528,18 +519,16 @@
             return s
         else:
             llen = slen - len(s.lstrip(" "))
             rlen = slen - len(s.rstrip(" "))
             return "".join(("\u2007" * llen, sstrip, "\u2007" * rlen))
 
     return "\\N".join(
-        (
-            ReplaceLeadingSpace(i) or " "
-            for i in str(s).replace("\\", "\\\\").replace("{", "\\{").replace("}", "\\}").split("\n")
-        )
+        ReplaceLeadingSpace(i) or " "
+        for i in str(s).replace("\\", "\\\\").replace("{", "\\{").replace("}", "\\}").split("\n")
     )
 
 
 def CalculateLength(s):
     return max(map(len, s.split("\n")))  # May not be accurate
 
 
@@ -556,18 +545,21 @@
         return "000000"
     elif RGB == 0xFFFFFF:
         return "FFFFFF"
     R = (RGB >> 16) & 0xFF
     G = (RGB >> 8) & 0xFF
     B = RGB & 0xFF
     if width < 1280 and height < 576:
-        return "%02X%02X%02X" % (B, G, R)
+        return f"{B:02X}{G:02X}{R:02X}"
     else:  # VobSub always uses BT.601 colorspace, convert to BT.709
-        ClipByte = lambda x: 255 if x > 255 else 0 if x < 0 else round(x)
-        return "%02X%02X%02X" % (
+
+        def ClipByte(x):
+            return 255 if x > 255 else 0 if x < 0 else round(x)
+
+        return "{:02X}{:02X}{:02X}".format(  # noqa: UP032
             ClipByte(R * 0.00956384088080656 + G * 0.03217254540203729 + B * 0.95826361371715607),
             ClipByte(R * -0.10493933142075390 + G * 1.17231478191855154 + B * -0.06737545049779757),
             ClipByte(R * 0.91348912373987645 + G * 0.07858536372532510 + B * 0.00792551253479842),
         )
 
 
 def ConvertType2(row, height, bottomReserved):
@@ -582,40 +574,43 @@
     def get(self, index, default=None):
         try:
             return self[index]
         except IndexError:
             return default
 
 
-@export
+def wrap_default(value: T | None, default: T) -> T:
+    return default if value is None else value
+
+
 def Danmaku2ASS(
-    inputs: Union[List[Union[str, bytes]], Union[str, bytes]],
+    inputs: list[str | bytes] | str | bytes,
     stage_width: int,
     stage_height: int,
     input_format: str = "xml",
     reserve_blank: float = 0,
     font_face: str = "sans-serif",
     font_size: float = 25.0,
     text_opacity: float = 1.0,
     duration_marquee: float = 5.0,
     duration_still: float = 5.0,
-    comment_filter: Optional[str] = None,
+    comment_filter: str | None = None,
     is_reduce_comments: bool = False,
-    progress_callback: Optional[Callable[..., None]] = None,
+    progress_callback: Callable[..., None] | None = None,
 ) -> str:
-    comment_filters: List[str] = [comment_filter] if comment_filter is not None else []
+    comment_filters: list[str] = [comment_filter] if comment_filter is not None else []
     filters_regex = []
     for comment_filter in comment_filters:
         try:
             if comment_filter:
                 filters_regex.append(re.compile(comment_filter))
-        except:
-            raise ValueError("Invalid regular expression: %s" % comment_filter)
+        except:  # noqa: E722
+            raise ValueError(f"Invalid regular expression: {comment_filter}")
 
-    comments: List[Comment] = []
+    comments: list[Comment] = []
     if not isinstance(inputs, list):
         inputs = [inputs]
     for input in inputs:
         if input_format == "xml":
             comments.extend(ReadCommentsBilibiliXml(input, font_size))
         else:
             if isinstance(input, str):
```

### Comparing `biliass-1.3.7.dev3/biliass/protobuf/danmaku_pb2.py` & `biliass-1.3.8/biliass/protobuf/danmaku_pb2.py`

 * *Files identical despite different names*

### Comparing `biliass-1.3.7.dev3/pyproject.toml` & `biliass-1.3.8/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,75 @@
 [tool.poetry]
 name = "biliass"
-version = "1.3.7-dev.3"
+version = "1.3.8"
 description = "将 B 站 XML 弹幕转换为 ASS 弹幕"
 authors = ["m13253", "Nyakku Shigure <sigure.qaq@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/yutto-dev/biliass"
 repository = "https://github.com/yutto-dev/biliass"
 keywords = ["bilibili", "yutto", "Danmaku2ASS"]
 include = ["biliass/py.typed", "*.pyi", "**/*.pyi"]
 classifiers = [
   "Operating System :: OS Independent",
-  "License :: OSI Approved :: MIT License",
+  "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 protobuf = "^4.21.9"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.0"
-black = "^22.1"
+pytest = "^7.2.2"
 tomli = { version = "^2.0.1", python = "<3.11" }
 pytest-rerunfailures = "^10.2"
-requests = "^2.28.1"
+requests = "^2.32.1"
+ruff = "^0.4.4"
 
 [tool.poetry.scripts]
 biliass = "biliass.__main__:main"
 
-[tool.black]
+[tool.ruff]
 line-length = 120
+target-version = "py38"
+exclude = ["*_pb2.py"]
 
-[tool.isort]
-profile = "black"
-add_imports = ["from __future__ import annotations"]
-skip = ["setup.py", ".venv"]
+[tool.ruff.lint]
+select = [
+  # Pyflakes
+  "F",
+  # Pycodestyle
+  "E",
+  "W",
+  # Isort
+  "I",
+  # Pyupgrade
+  "UP",
+  # Flake8-pyi
+  "PYI",
+  # Yesqa
+  "RUF100",
+]
+ignore = [
+  "E501", # line too long, duplicate with ruff fmt
+  "F401", # imported but unused, duplicate with pyright
+  "F841", # local variable is assigned to but never used, duplicate with pyright
+]
+
+[tool.ruff.lint.isort]
+required-imports = ["from __future__ import annotations"]
+known-first-party = ["biliass"]
+
+[tool.ruff.lint.per-file-ignores]
+"setup.py" = ["I"]
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `biliass-1.3.7.dev3/PKG-INFO` & `biliass-1.3.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 Metadata-Version: 2.1
 Name: biliass
-Version: 1.3.7.dev3
+Version: 1.3.8
 Summary: 将 B 站 XML 弹幕转换为 ASS 弹幕
 Home-page: https://github.com/yutto-dev/biliass
 License: GPLv3
 Keywords: bilibili,yutto,Danmaku2ASS
 Author: m13253
-Requires-Python: >=3.7,<4.0
-Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: protobuf (>=4.21.9,<5.0.0)
 Project-URL: Repository, https://github.com/yutto-dev/biliass
 Description-Content-Type: text/markdown
 
 # biliass
```

#### html2text {}

```diff
@@ -1,24 +1,20 @@
-Metadata-Version: 2.1 Name: biliass Version: 1.3.7.dev3 Summary: å° B ç« XML
+Metadata-Version: 2.1 Name: biliass Version: 1.3.8 Summary: å° B ç« XML
 å¼¹å¹è½¬æ¢ä¸º ASS å¼¹å¹ Home-page: https://github.com/yutto-dev/biliass
 License: GPLv3 Keywords: bilibili,yutto,Danmaku2ASS Author: m13253 Requires-
-Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: MIT License
-Classifier: License :: Other/Proprietary License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: Implementation :: CPython Requires-Dist:
-protobuf (>=4.21.9,<5.0.0) Project-URL: Repository, https://github.com/yutto-
-dev/biliass Description-Content-Type: text/markdown # biliass
+Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: GNU General Public
+License v3 (GPLv3) Classifier: License :: Other/Proprietary License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Dist: protobuf (>=4.21.9,<5.0.0) Project-URL: Repository, https://
+github.com/yutto-dev/biliass Description-Content-Type: text/markdown # biliass
 _[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_p_y_p_i_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_L_I_C_E_N_S_E_]_[_G_i_t_m_o_j_i_]
 biliassï¼åªæ¯ Danmaku2ASS ç bilili ä¸ yutto ééç åçï¼
 github.com/m13253/danmaku2ass> ä»æ¯æ bilibili å¼¹å¹ï¼æ¯æ XML å¼¹å¹å
 Protobuf å¼¹å¹ ## Install ```bash pip install biliass ``` ## Usage ```bash #
 XML å¼¹å¹ biliass danmaku.xml -s 1920x1080 -o danmaku.ass # protobuf å¼¹å¹
 biliass danmaku.pb -s 1920x1080 -f protobuf -o danmaku.ass ``` ```python from
 biliass import Danmaku2ASS # xml Danmaku2ASS( xml_text_or_bytes, width, height,
```

