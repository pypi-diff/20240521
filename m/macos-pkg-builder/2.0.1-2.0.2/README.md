# Comparing `tmp/macos_pkg_builder-2.0.1-py3-none-any.whl.zip` & `tmp/macos_pkg_builder-2.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 12397 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1155 b- defN 24-Apr-26 17:51 macos_pkg_builder/__init__.py
--rw-r--r--  2.0 unx     8838 b- defN 24-Apr-26 17:51 macos_pkg_builder/core.py
--rw-r--r--  2.0 unx     7922 b- defN 24-Apr-26 17:51 macos_pkg_builder/distribution_pkg.py
--rw-r--r--  2.0 unx     8341 b- defN 24-Apr-26 17:51 macos_pkg_builder/flat_pkg.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 17:51 macos_pkg_builder/utilities/__init__.py
--rw-r--r--  2.0 unx     1866 b- defN 24-Apr-26 17:51 macos_pkg_builder/utilities/signing.py
--rw-r--r--  2.0 unx     2747 b- defN 24-Apr-26 17:51 macos_pkg_builder/utilities/subprocess_wrapper.py
--rw-r--r--  2.0 unx     8475 b- defN 24-Apr-26 17:52 macos_pkg_builder-2.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-26 17:52 macos_pkg_builder-2.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-Apr-26 17:52 macos_pkg_builder-2.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      980 b- defN 24-Apr-26 17:52 macos_pkg_builder-2.0.1.dist-info/RECORD
-11 files, 40434 bytes uncompressed, 10711 bytes compressed:  73.5%
+Zip file size: 12399 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1155 b- defN 24-May-21 16:50 macos_pkg_builder/__init__.py
+-rw-r--r--  2.0 unx     8838 b- defN 24-May-21 16:50 macos_pkg_builder/core.py
+-rw-r--r--  2.0 unx     7922 b- defN 24-May-21 16:50 macos_pkg_builder/distribution_pkg.py
+-rw-r--r--  2.0 unx     8347 b- defN 24-May-21 16:50 macos_pkg_builder/flat_pkg.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-21 16:50 macos_pkg_builder/utilities/__init__.py
+-rw-r--r--  2.0 unx     1866 b- defN 24-May-21 16:50 macos_pkg_builder/utilities/signing.py
+-rw-r--r--  2.0 unx     2747 b- defN 24-May-21 16:50 macos_pkg_builder/utilities/subprocess_wrapper.py
+-rw-r--r--  2.0 unx     8475 b- defN 24-May-21 16:51 macos_pkg_builder-2.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-21 16:51 macos_pkg_builder-2.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-May-21 16:51 macos_pkg_builder-2.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      980 b- defN 24-May-21 16:51 macos_pkg_builder-2.0.2.dist-info/RECORD
+11 files, 40440 bytes uncompressed, 10713 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: macos_pkg_builder/utilities/signing.py
 Comment: 
 
 Filename: macos_pkg_builder/utilities/subprocess_wrapper.py
 Comment: 
 
-Filename: macos_pkg_builder-2.0.1.dist-info/METADATA
+Filename: macos_pkg_builder-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: macos_pkg_builder-2.0.1.dist-info/WHEEL
+Filename: macos_pkg_builder-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: macos_pkg_builder-2.0.1.dist-info/top_level.txt
+Filename: macos_pkg_builder-2.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: macos_pkg_builder-2.0.1.dist-info/RECORD
+Filename: macos_pkg_builder-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## macos_pkg_builder/__init__.py

```diff
@@ -15,15 +15,15 @@
     >>>     },
     >>> )
 
     >>> assert pkg_obj.build() is True
 """
 
 __title__:        str = "macos_pkg_builder"
-__version__:      str = "2.0.1"
+__version__:      str = "2.0.2"
 __description__:  str = "macOS Package Builder Library, wrapping Apple's 'pkgbuild' and 'productbuild' utilities."
 __url__:          str = "https://github.com/ripeda/macOS-Pkg-Builder"
 __author__:       str = "RIPEDA Consulting"
 __author_email__: str = "info@ripeda.com"
 __status__:       str = "Production/Stable"
 __all__:         list = ["Packages"]
```

## macos_pkg_builder/flat_pkg.py

```diff
@@ -142,15 +142,15 @@
             "BundleHasStrictIdentifier": True,
             "BundleIsRelocatable":       self._pkg_allow_relocation,
             "BundleIsVersionChecked":    True,
             "BundleOverwriteAction":     "upgrade",
             "RootRelativeBundlePath":    bundle,
         }]
         file = tempfile.NamedTemporaryFile(delete=False)
-        plistlib.dump(contents, file.name.open("wb"))
+        plistlib.dump(contents, Path(file.name).open("wb"))
 
         return Path(file.name)
 
 
     def _generate_pkg_arguments(self) -> list:
         """
         Generate pkgbuild arguments according to the provided configuration.
```

## Comparing `macos_pkg_builder-2.0.1.dist-info/METADATA` & `macos_pkg_builder-2.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macos_pkg_builder
-Version: 2.0.1
+Version: 2.0.2
 Summary: macOS Package Builder Library, wrapping Apple's 'pkgbuild' and 'productbuild' utilities.
 Home-page: https://github.com/ripeda/macOS-Pkg-Builder
 Author: RIPEDA Consulting
 Author-email: info@ripeda.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: markdown
```

## Comparing `macos_pkg_builder-2.0.1.dist-info/RECORD` & `macos_pkg_builder-2.0.2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-macos_pkg_builder/__init__.py,sha256=BEwWaaYeubT1M5HmyhnRqfyA3R5fweDbR9Xe0GHYbzs,1155
+macos_pkg_builder/__init__.py,sha256=8jMK0FAnjXzXpNhYvL9APgFnQ2p9NI6fSjnGCjRtajI,1155
 macos_pkg_builder/core.py,sha256=m26ykH3_0o3oEn8ZKAqs_iMujEv7LpnaS4P_DwdVENA,8838
 macos_pkg_builder/distribution_pkg.py,sha256=ZyYM_Ul33PyFaO7KCo8Zv1oMWg6bO8sZhYwn8t-UMDs,7922
-macos_pkg_builder/flat_pkg.py,sha256=wOTIL15oKks3OOu5PwpZCgZNllPLSRAwciwgO9BOp4U,8341
+macos_pkg_builder/flat_pkg.py,sha256=SpZ3qYa9Dlk-LFtITSKZ4hABNzAfRTnZ1g-S3_u3H8U,8347
 macos_pkg_builder/utilities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 macos_pkg_builder/utilities/signing.py,sha256=0yX9uR_b4dRhyDg6HX2Dbh2jyvl30Dnv6iOSh0NorPw,1866
 macos_pkg_builder/utilities/subprocess_wrapper.py,sha256=jJyh2D_oTVAWUUBMHPUdF6YYA0vycRZGch3Z3SwCX2A,2747
-macos_pkg_builder-2.0.1.dist-info/METADATA,sha256=CM-9o4MzFSIi7yzYj2dZytYsnp5spvThBQvowUIsJpw,8475
-macos_pkg_builder-2.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-macos_pkg_builder-2.0.1.dist-info/top_level.txt,sha256=bQR8DTKmm4DzHeH3KB62AWXUwQwcWBwyUcn3wmlvOgQ,18
-macos_pkg_builder-2.0.1.dist-info/RECORD,,
+macos_pkg_builder-2.0.2.dist-info/METADATA,sha256=zsPWTwbgddlQtMB-b7JbMHL6_BtcQkW2C0B1vKqnmmY,8475
+macos_pkg_builder-2.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+macos_pkg_builder-2.0.2.dist-info/top_level.txt,sha256=bQR8DTKmm4DzHeH3KB62AWXUwQwcWBwyUcn3wmlvOgQ,18
+macos_pkg_builder-2.0.2.dist-info/RECORD,,
```

