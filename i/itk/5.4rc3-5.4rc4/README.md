# Comparing `tmp/itk-5.4rc3-cp39-cp39-win_amd64.whl.zip` & `tmp/itk-5.4rc4-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 16964 bytes, number of entries: 7
--rw-rw-r--  2.0 fat    22652 b- defN 24-Apr-07 02:28 itk-5.4rc3.dist-info/METADATA
--rw-rw-r--  2.0 fat      103 b- defN 24-Apr-07 02:28 itk-5.4rc3.dist-info/WHEEL
--rw-rw-r--  2.0 fat        0 b- defN 24-Apr-07 02:28 itk-5.4rc3.dist-info/entry_points.txt
--rw-rw-r--  2.0 fat    11358 b- defN 24-Apr-07 02:28 itk-5.4rc3.dist-info/licenses/LICENSE
--rw-rw-r--  2.0 fat    11360 b- defN 24-Apr-07 02:28 itk-5.4rc3.dist-info/licenses/ITK-source/ITK/LICENSE
--rw-rw-r--  2.0 fat      472 b- defN 24-Apr-07 02:28 itk-5.4rc3.dist-info/licenses/ITK-source/ITK/NOTICE
--rw-rw-r--  2.0 fat      602 b- defN 24-Apr-07 02:28 itk-5.4rc3.dist-info/RECORD
-7 files, 46547 bytes uncompressed, 15892 bytes compressed:  65.9%
+Zip file size: 17020 bytes, number of entries: 7
+-rw-rw-r--  2.0 fat    22876 b- defN 24-Apr-17 14:44 itk-5.4rc4.dist-info/METADATA
+-rw-rw-r--  2.0 fat      103 b- defN 24-Apr-17 14:44 itk-5.4rc4.dist-info/WHEEL
+-rw-rw-r--  2.0 fat        0 b- defN 24-Apr-17 14:44 itk-5.4rc4.dist-info/entry_points.txt
+-rw-rw-r--  2.0 fat    11358 b- defN 24-Apr-17 14:44 itk-5.4rc4.dist-info/licenses/LICENSE
+-rw-rw-r--  2.0 fat    11360 b- defN 24-Apr-17 14:44 itk-5.4rc4.dist-info/licenses/ITK-source/ITK/LICENSE
+-rw-rw-r--  2.0 fat      472 b- defN 24-Apr-17 14:44 itk-5.4rc4.dist-info/licenses/ITK-source/ITK/NOTICE
+-rw-rw-r--  2.0 fat      602 b- defN 24-Apr-17 14:44 itk-5.4rc4.dist-info/RECORD
+7 files, 46771 bytes uncompressed, 15948 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: itk-5.4rc3.dist-info/METADATA
+Filename: itk-5.4rc4.dist-info/METADATA
 Comment: 
 
-Filename: itk-5.4rc3.dist-info/WHEEL
+Filename: itk-5.4rc4.dist-info/WHEEL
 Comment: 
 
-Filename: itk-5.4rc3.dist-info/entry_points.txt
+Filename: itk-5.4rc4.dist-info/entry_points.txt
 Comment: 
 
-Filename: itk-5.4rc3.dist-info/licenses/LICENSE
+Filename: itk-5.4rc4.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: itk-5.4rc3.dist-info/licenses/ITK-source/ITK/LICENSE
+Filename: itk-5.4rc4.dist-info/licenses/ITK-source/ITK/LICENSE
 Comment: 
 
-Filename: itk-5.4rc3.dist-info/licenses/ITK-source/ITK/NOTICE
+Filename: itk-5.4rc4.dist-info/licenses/ITK-source/ITK/NOTICE
 Comment: 
 
-Filename: itk-5.4rc3.dist-info/RECORD
+Filename: itk-5.4rc4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `itk-5.4rc3.dist-info/METADATA` & `itk-5.4rc4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itk
-Version: 5.4rc3
+Version: 5.4rc4
 Summary: ITK is an open-source toolkit for multidimensional image analysis
 Keywords: ITK InsightToolkit scientific medical image imaging
 Author-Email: Insight Software Consortium <community@itk.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -224,20 +224,20 @@
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries
 Project-URL: Download, https://github.com/InsightSoftwareConsortium/ITK/releases
 Project-URL: Home, https://docs.itk.org/
 Project-URL: Issues, https://github.com/InsightSoftwareConsortium/ITK/issues
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/ITK
 Requires-Python: >=3.8
-Requires-Dist: itk-core==5.4rc3
-Requires-Dist: itk-numerics==5.4rc3
-Requires-Dist: itk-io==5.4rc3
-Requires-Dist: itk-filtering==5.4rc3
-Requires-Dist: itk-registration==5.4rc3
-Requires-Dist: itk-segmentation==5.4rc3
+Requires-Dist: itk-core==5.4rc4
+Requires-Dist: itk-numerics==5.4rc4
+Requires-Dist: itk-io==5.4rc4
+Requires-Dist: itk-filtering==5.4rc4
+Requires-Dist: itk-registration==5.4rc4
+Requires-Dist: itk-segmentation==5.4rc4
 Requires-Dist: numpy
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: ITK-source\ITK\LICENSE
 License-File: ITK-source\ITK\NOTICE
 
 ![ITK - The Insight Toolkit](https://raw.githubusercontent.com/InsightSoftwareConsortium/ITK/801370c025c7d296783481779a41c6d559c992c5/Documentation/Art/itkBannerSmall.png)
@@ -251,16 +251,17 @@
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/InsightSoftwareConsortium/ITK/blob/master/LICENSE)
 [![DOI](https://zenodo.org/badge/800928.svg)](https://zenodo.org/badge/latestdoi/800928)
 [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)
 
 | | C++ | Python |
 |:------:|:--------:|:--------:|
 | Linux | [![Build Status](https://dev.azure.com/itkrobotlinux/ITK.Linux/_apis/build/status/ITK.Linux?branchName=master)](https://dev.azure.com/itkrobotlinux/ITK.Linux/_build/latest?definitionId=2&branchName=master) | [![Build Status](https://dev.azure.com/itkrobotlinuxpython/ITK.Linux.Python/_apis/build/status/ITK.Linux.Python?branchName=master)](https://dev.azure.com/itkrobotlinuxpython/ITK.Linux.Python/_build/latest?definitionId=3&branchName=master) |
-| macOS | [![Build Status](https://dev.azure.com/itkrobotmacos/ITK.macOS/_apis/build/status/ITK.macOS?branchName=master)](https://dev.azure.com/itkrobotmacos/ITK.macOS/_build/latest?definitionId=2&branchName=master) | [![Build Status](https://dev.azure.com/itkrobotmacospython/ITK.macOS.Python/_apis/build/status/ITK.macOS.Python?branchName=master)](https://dev.azure.com/itkrobotmacospython/ITK.macOS.Python/_build/latest?definitionId=2&branchName=master) |
 | Windows | [![Build Status](https://dev.azure.com/itkrobotwindow/ITK.Windows/_apis/build/status/ITK.Windows?branchName=master)](https://dev.azure.com/itkrobotwindow/ITK.Windows/_build/latest?definitionId=2&branchName=master) | [![Build Status](https://dev.azure.com/itkrobotwindowpython/ITK.Windows.Python/_apis/build/status/ITK.Windows.Python?branchName=master)](https://dev.azure.com/itkrobotwindowpython/ITK.Windows.Python/_build/latest?definitionId=1) |
+| macOS | [![Build Status](https://dev.azure.com/itkrobotmacos/ITK.macOS/_apis/build/status/ITK.macOS?branchName=master)](https://dev.azure.com/itkrobotmacos/ITK.macOS/_build/latest?definitionId=2&branchName=master) | [![Build Status](https://dev.azure.com/itkrobotmacospython/ITK.macOS.Python/_apis/build/status/ITK.macOS.Python?branchName=master)](https://dev.azure.com/itkrobotmacospython/ITK.macOS.Python/_build/latest?definitionId=2&branchName=master) |
+| macOS (Apple Silicon)|  [![ITK.macOS.Arm64](https://github.com/InsightSoftwareConsortium/ITK/actions/workflows/macos-arm.yml/badge.svg)](https://github.com/InsightSoftwareConsortium/ITK/actions/workflows/macos-arm.yml)| |
 | Linux (Code coverage)| [![Build Status](https://dev.azure.com/itkrobotbatch/ITK.Coverage/_apis/build/status/ITK.Coverage?branchName=master)](https://dev.azure.com/itkrobotbatch/ITK.Coverage/_build/latest?definitionId=3&branchName=master) | |
 
 Links
 -----
 
 * [Homepage](https://itk.org)
 * [Download](https://docs.itk.org/en/latest/download.html)
```

## Comparing `itk-5.4rc3.dist-info/licenses/LICENSE` & `itk-5.4rc4.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `itk-5.4rc3.dist-info/licenses/ITK-source/ITK/LICENSE` & `itk-5.4rc4.dist-info/licenses/ITK-source/ITK/LICENSE`

 * *Files identical despite different names*

