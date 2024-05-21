# Comparing `tmp/Martinoid-0.0.9-py3-none-any.whl.zip` & `tmp/Martinoid-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 21620 bytes, number of entries: 37
+Zip file size: 21655 bytes, number of entries: 37
 -rw-rw-rw-  2.0 fat    17634 b- defN 24-Jan-22 09:44 Martinoid/Martinoid2.py
 -rw-rw-rw-  2.0 fat      231 b- defN 23-Dec-03 19:14 Martinoid/__init__.py
 -rw-rw-rw-  2.0 fat     4984 b- defN 23-Dec-03 19:14 Martinoid/__main__.py
 -rw-rw-rw-  2.0 fat     9619 b- defN 23-Oct-25 18:14 Martinoid/_martinoid_data.py
--rw-rw-rw-  2.0 fat      217 b- defN 24-Jan-22 09:44 Martinoid/version.py
+-rw-rw-rw-  2.0 fat      217 b- defN 24-May-21 21:05 Martinoid/version.py
 -rw-rw-rw-  2.0 fat      629 b- defN 23-Oct-18 09:29 Martinoid/Data/Na.csv
 -rw-rw-rw-  2.0 fat      657 b- defN 23-Oct-18 09:29 Martinoid/Data/Nab.csv
 -rw-rw-rw-  2.0 fat      657 b- defN 23-Oct-18 09:29 Martinoid/Data/Nd.csv
 -rw-rw-rw-  2.0 fat      657 b- defN 23-Oct-18 09:29 Martinoid/Data/Ne.csv
 -rw-rw-rw-  2.0 fat      796 b- defN 23-Oct-18 09:29 Martinoid/Data/Nf.csv
 -rw-rw-rw-  2.0 fat      834 b- defN 23-Oct-18 09:29 Martinoid/Data/Nfe.csv
 -rw-rw-rw-  2.0 fat      920 b- defN 23-Oct-18 09:29 Martinoid/Data/NfeB4.csv
@@ -28,12 +28,12 @@
 -rw-rw-rw-  2.0 fat      658 b- defN 23-Oct-18 09:29 Martinoid/Data/Ns.csv
 -rw-rw-rw-  2.0 fat      657 b- defN 23-Oct-18 09:29 Martinoid/Data/Nse.csv
 -rw-rw-rw-  2.0 fat      658 b- defN 23-Oct-18 09:29 Martinoid/Data/Nt.csv
 -rw-rw-rw-  2.0 fat      658 b- defN 23-Oct-18 09:29 Martinoid/Data/Nv.csv
 -rw-rw-rw-  2.0 fat      869 b- defN 23-Oct-18 09:29 Martinoid/Data/Nw.csv
 -rw-rw-rw-  2.0 fat      927 b- defN 23-Oct-18 09:29 Martinoid/Data/Nwe.csv
 -rw-rw-rw-  2.0 fat      796 b- defN 23-Oct-18 09:29 Martinoid/Data/Ny.csv
--rw-rw-rw-  2.0 fat     3992 b- defN 24-Jan-22 09:45 Martinoid-0.0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Jan-22 09:45 Martinoid-0.0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Jan-22 09:45 Martinoid-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2880 b- defN 24-Jan-22 09:45 Martinoid-0.0.9.dist-info/RECORD
-37 files, 60151 bytes uncompressed, 17070 bytes compressed:  71.6%
+-rw-rw-rw-  2.0 fat     4050 b- defN 24-May-21 21:05 Martinoid-0.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-21 21:05 Martinoid-0.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-May-21 21:05 Martinoid-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2880 b- defN 24-May-21 21:05 Martinoid-0.1.0.dist-info/RECORD
+37 files, 60209 bytes uncompressed, 17105 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -93,20 +93,20 @@
 
 Filename: Martinoid/Data/Nwe.csv
 Comment: 
 
 Filename: Martinoid/Data/Ny.csv
 Comment: 
 
-Filename: Martinoid-0.0.9.dist-info/METADATA
+Filename: Martinoid-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: Martinoid-0.0.9.dist-info/WHEEL
+Filename: Martinoid-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: Martinoid-0.0.9.dist-info/top_level.txt
+Filename: Martinoid-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: Martinoid-0.0.9.dist-info/RECORD
+Filename: Martinoid-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Martinoid/version.py

```diff
@@ -1,5 +1,5 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
-__version__ = '0.0.9'
+__version__ = '0.1.0'
```

## Comparing `Martinoid-0.0.9.dist-info/METADATA` & `Martinoid-0.1.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Martinoid
-Version: 0.0.9
+Version: 0.1.0
 Summary: This module was inspired by martinize (http://cgmartini.nl/index.php/tools2/proteins-and-bilayers/204-martinize) and has been created to perform automatic topology building of peptoids within the MARTINI forcefield (v2.1) in the GROMACS program.
 Home-page: https://github.com/Hamish-cmyk/MartinoidPeptoidCG
 Author: Hamish W. A. Swanson, Alexander van Teijlingen
 Author-email: a.vant@linuxmail.org
 License: BSD 2-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.10
@@ -14,15 +14,17 @@
 Requires-Dist: numpy
 Requires-Dist: mdtraj
 Requires-Dist: matplotlib
 Requires-Dist: argparse
 
 # Martinoid Peptoid CG
 
-Originally written as part of the publication title "Martinoid: The Martini Peptoid Force Field", published in the ***Journal of Very Cool Science***.
+Originally written as part of the publication title "Martinoid: The Martini Peptoid Force Field", published in ***Phys. Chem. Chem. Phys.***. 
+
+https://pubs.rsc.org/en/content/articlehtml/2024/cp/d3cp05907c
 
 This module was inspired by martinize (http://cgmartini.nl/index.php/tools2/proteins-and-bilayers/204-martinize) and has been created to perform automatic topology building of peptoids within the MARTINI forcefield (v2.1) in the GROMACS program.
 
 A key difference between Martinoid and Martinize is that the former does not require an input all-atom peptoid structure while Martinize does. This has obvious advantages but does mean the output guessed CG structures [generally] require a greater degree of minimization.
 
 ## Installation
 ```bash
```

## Comparing `Martinoid-0.0.9.dist-info/RECORD` & `Martinoid-0.1.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Martinoid/Martinoid2.py,sha256=hUxn1QXjTfoeVDXhSSKu3RXqXv2FwiWFVsFozjcxm30,17634
 Martinoid/__init__.py,sha256=yYrcB0tF-fvsYJ2djaRJS95Ay0_sIMMPJRr2q-VgcoM,231
 Martinoid/__main__.py,sha256=XDl6WvO5z6xJchSUvAdSbbeuDh5N9RAt1srWUO8lCpc,4984
 Martinoid/_martinoid_data.py,sha256=WaCi86w2PkHrxpBlKLWRIhzqB91BnzCvR1rYBCzujRE,9619
-Martinoid/version.py,sha256=3-zCOYHOwgvxRJIFA5l_-HwR612KDcuOEoZqX5aY7jk,217
+Martinoid/version.py,sha256=dmDhQPxFajIKok0NkBcbIOPJbg0GzTo1iLkEfTxIxP8,217
 Martinoid/Data/Na.csv,sha256=h2p0aOTHKDsjEbCZWoJ76JrQyGthDBIn6UdCOnwi71o,629
 Martinoid/Data/Nab.csv,sha256=ZV_jI-ci3EbfZv_bu7S7wnF__5Jp5SgcOtW1MJFBT40,657
 Martinoid/Data/Nd.csv,sha256=ONlmh4f-NhYIbO3cjk8gtOp8U_bzxw422EnFRJ3RH9w,657
 Martinoid/Data/Ne.csv,sha256=bSNi0txnpwdQGh9xlCsYnqMWwWkdacJc3suq9q42gko,657
 Martinoid/Data/Nf.csv,sha256=cJLltb1-h_6uCWyWNlP69nSt0W404-74CwHtBAu2iy8,796
 Martinoid/Data/Nfe.csv,sha256=rtJcd5St8MVnKzaXTSv_dF3JQO0F2ciCCiRvMXBOlm0,834
 Martinoid/Data/NfeB4.csv,sha256=DUijGUsEY3tevG2cprazxl1es0xlyKsZB_cqinKeWio,920
@@ -27,11 +27,11 @@
 Martinoid/Data/Ns.csv,sha256=1WJdseiKr_M9mqCSoutlCIGwMO8fbZ2cwKH8IiGS38k,658
 Martinoid/Data/Nse.csv,sha256=i09bCCOxjMHKWjyQbARyN9NnktnYT6HS5cckUf5KtI8,657
 Martinoid/Data/Nt.csv,sha256=AwVq6fYo_OTiejaTJ_jlHNfpetDsS14SyJ8UgHe-NTU,658
 Martinoid/Data/Nv.csv,sha256=-utIsxDN69SvEnRG5icERTYARRwMpAtXM-ZC93d-gxo,658
 Martinoid/Data/Nw.csv,sha256=3Vs6vwbHOMjERfR6LNrZb2wLxR5r3dv7gm8YSbQBvZI,869
 Martinoid/Data/Nwe.csv,sha256=GwYLYr_Fo2qj8LhiZd_EQDPnQxy0-ebhOoHw9caXKB4,927
 Martinoid/Data/Ny.csv,sha256=mYPMakQha4O6KLNXeP0OSO849HhW14aWOwEkb8SbuYM,796
-Martinoid-0.0.9.dist-info/METADATA,sha256=uthUI5lNDW-2MYnMS8kFv1ziM1ybKMOrL7hFUvDSIBU,3992
-Martinoid-0.0.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-Martinoid-0.0.9.dist-info/top_level.txt,sha256=jJSbRpexlCpBsK5RuN3sPtqbUWi50mEZEmertTFoCNg,10
-Martinoid-0.0.9.dist-info/RECORD,,
+Martinoid-0.1.0.dist-info/METADATA,sha256=fyAd1MCKUiCejrW4Pr4J5jzg4Ojyc_uv5IwqUOQp6fw,4050
+Martinoid-0.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+Martinoid-0.1.0.dist-info/top_level.txt,sha256=jJSbRpexlCpBsK5RuN3sPtqbUWi50mEZEmertTFoCNg,10
+Martinoid-0.1.0.dist-info/RECORD,,
```

