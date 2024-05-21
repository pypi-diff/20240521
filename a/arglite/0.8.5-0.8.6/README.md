# Comparing `tmp/arglite-0.8.5-py3-none-any.whl.zip` & `tmp/arglite-0.8.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5628 bytes, number of entries: 9
+Zip file size: 5622 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       43 b- defN 24-May-13 20:56 arglite/__init__.py
--rw-r--r--  2.0 unx     5145 b- defN 24-May-15 12:50 arglite/arglite.py
+-rw-r--r--  2.0 unx     5124 b- defN 24-May-21 02:09 arglite/arglite.py
 -rw-r--r--  2.0 unx      824 b- defN 24-May-13 20:56 arglite/argument.py
 -rw-r--r--  2.0 unx     1037 b- defN 24-May-13 20:56 arglite/code.py
--rw-r--r--  2.0 unx     1211 b- defN 24-May-15 13:00 arglite-0.8.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      785 b- defN 24-May-15 13:00 arglite-0.8.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-15 13:00 arglite-0.8.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-15 13:00 arglite-0.8.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      680 b- defN 24-May-15 13:00 arglite-0.8.5.dist-info/RECORD
-9 files, 9825 bytes uncompressed, 4462 bytes compressed:  54.6%
+-rw-r--r--  2.0 unx     1211 b- defN 24-May-21 02:10 arglite-0.8.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      785 b- defN 24-May-21 02:10 arglite-0.8.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-21 02:10 arglite-0.8.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-21 02:10 arglite-0.8.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      680 b- defN 24-May-21 02:10 arglite-0.8.6.dist-info/RECORD
+9 files, 9804 bytes uncompressed, 4456 bytes compressed:  54.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: arglite/argument.py
 Comment: 
 
 Filename: arglite/code.py
 Comment: 
 
-Filename: arglite-0.8.5.dist-info/LICENSE
+Filename: arglite-0.8.6.dist-info/LICENSE
 Comment: 
 
-Filename: arglite-0.8.5.dist-info/METADATA
+Filename: arglite-0.8.6.dist-info/METADATA
 Comment: 
 
-Filename: arglite-0.8.5.dist-info/WHEEL
+Filename: arglite-0.8.6.dist-info/WHEEL
 Comment: 
 
-Filename: arglite-0.8.5.dist-info/top_level.txt
+Filename: arglite-0.8.6.dist-info/top_level.txt
 Comment: 
 
-Filename: arglite-0.8.5.dist-info/RECORD
+Filename: arglite-0.8.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## arglite/arglite.py

```diff
@@ -22,15 +22,14 @@
 
   def __init__(self):
     """ Entry point. """
     self.file = self.caller()
     self.h, self.help = None, None
     arg_str = self.flatten(sys.argv[1:])
     self.args = self.pairs(arg_str)
-    print(self.args)
     self.required = Required()
     self.optional = Optional()
     self.set_vars()
     self.get_errors()
 
     for error in self.errors:
       print(f"✗ ERROR: A value was expected for {error}, but not was provided as a flag")
```

## Comparing `arglite-0.8.5.dist-info/LICENSE` & `arglite-0.8.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `arglite-0.8.5.dist-info/METADATA` & `arglite-0.8.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arglite
-Version: 0.8.5
+Version: 0.8.6
 Summary: A lightweight, dynamic arg parser for fun, but not profit.
 Home-page: https://github.com/dluman/arglite
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: rich
```

## Comparing `arglite-0.8.5.dist-info/RECORD` & `arglite-0.8.6.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 arglite/__init__.py,sha256=qYy3XGLguBP5P03kIROVRrkp83p54SyB6mFd-3hMvpE,43
-arglite/arglite.py,sha256=bPXaEaSrzCtUlfnz44Eg4OkDdgfjlhftN9NO3oDeT0k,5145
+arglite/arglite.py,sha256=eCxarBdnD-q8gBA0A3OenGiT4gWguyJTF9EsvwOWl58,5124
 arglite/argument.py,sha256=-tGlU-8eD21NWBOlgfYI4VmFOXXbDT_kbq6D7zXXkTQ,824
 arglite/code.py,sha256=3zYimm_Q4fRIcILrgTfT9gOWAu82pQdFQKO4mWE03kU,1037
-arglite-0.8.5.dist-info/LICENSE,sha256=fhLl30uuEsshWBuhV87SDhmGoFCN0Q0Oikq5pM-U6Fw,1211
-arglite-0.8.5.dist-info/METADATA,sha256=hT9Gb1j23xspHiWnaEwjCLUHe9uKrnXeKHgvgv5gov4,785
-arglite-0.8.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-arglite-0.8.5.dist-info/top_level.txt,sha256=arzqHSIoCtyjfK5QmzSD--Cxr2BO3A2zFy50JEko6iA,8
-arglite-0.8.5.dist-info/RECORD,,
+arglite-0.8.6.dist-info/LICENSE,sha256=fhLl30uuEsshWBuhV87SDhmGoFCN0Q0Oikq5pM-U6Fw,1211
+arglite-0.8.6.dist-info/METADATA,sha256=EXaG9cTaH2deNREug6yq4SrSZCnsSF5fRcPFSJvnAms,785
+arglite-0.8.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+arglite-0.8.6.dist-info/top_level.txt,sha256=arzqHSIoCtyjfK5QmzSD--Cxr2BO3A2zFy50JEko6iA,8
+arglite-0.8.6.dist-info/RECORD,,
```

