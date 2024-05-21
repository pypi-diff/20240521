# Comparing `tmp/myplotlib-1.2.0.tar.gz` & `tmp/myplotlib-1.3.0.tar.gz`

## Comparing `myplotlib-1.2.0.tar` & `myplotlib-1.3.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 myplotlib-1.2.0/MANIFEST.in
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 myplotlib-1.2.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/__init__.py
--rw-r--r--   0        0        0    12462 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/plots.py
--rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/tests.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/fancy.dark.mplstyle
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/fancy.light.mplstyle
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/hershey.dark.mplstyle
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/hershey.light.mplstyle
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/mono.dark.mplstyle
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/mono.light.mplstyle
--rw-r--r--   0        0        0    76725 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/colormaps/bipolar.csv
--rw-r--r--   0        0        0    76800 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/colormaps/colt.csv
--rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/colormaps/fire.csv
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/colormaps/idl.csv
--rw-r--r--   0        0        0    38400 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/colormaps/sunrise.csv
--rw-r--r--   0        0        0    38400 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/colormaps/thermal.csv
--rw-r--r--   0        0        0    38400 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/colormaps/vanilla.csv
--rwxr-xr-x   0        0        0   244278 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/fonts/AppleChancery.ttf
--rw-r--r--   0        0        0   601316 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-Bold.ttf
--rw-r--r--   0        0        0   567300 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-BoldItalic.ttf
--rw-r--r--   0        0        0   600940 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-ExtraBold.ttf
--rw-r--r--   0        0        0   566936 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-ExtraBoldItalic.ttf
--rw-r--r--   0        0        0   564280 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-Italic.ttf
--rw-r--r--   0        0        0   601412 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-Medium.ttf
--rw-r--r--   0        0        0   566872 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-MediumItalic.ttf
--rw-r--r--   0        0        0   599076 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-Regular.ttf
--rw-r--r--   0        0        0   601652 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-SemiBold.ttf
--rw-r--r--   0        0        0   567528 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-SemiBoldItalic.ttf
--rwxr-xr-x   0        0        0    44328 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/fonts/HersheyTex-Book.otf
--rwxr-xr-x   0        0        0    31664 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/assets/fonts/HersheyTex-Light.otf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/tools/__init__.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 myplotlib-1.2.0/myplotlib/tools/lic.py
--rw-r--r--   0        0        0   185577 2020-02-02 00:00:00.000000 myplotlib-1.2.0/previews/None.jpg
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 myplotlib-1.2.0/previews/README.md
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 myplotlib-1.2.0/previews/export_previews.py
--rw-r--r--   0        0        0   311067 2020-02-02 00:00:00.000000 myplotlib-1.2.0/previews/fancy_dark.jpg
--rw-r--r--   0        0        0   323081 2020-02-02 00:00:00.000000 myplotlib-1.2.0/previews/fancy_light.jpg
--rw-r--r--   0        0        0   986550 2020-02-02 00:00:00.000000 myplotlib-1.2.0/previews/hershey_dark.jpg
--rw-r--r--   0        0        0  1028568 2020-02-02 00:00:00.000000 myplotlib-1.2.0/previews/hershey_light.jpg
--rw-r--r--   0        0        0   316147 2020-02-02 00:00:00.000000 myplotlib-1.2.0/previews/mono_dark.jpg
--rw-r--r--   0        0        0   325963 2020-02-02 00:00:00.000000 myplotlib-1.2.0/previews/mono_light.jpg
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 myplotlib-1.2.0/.gitignore
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 myplotlib-1.2.0/LICENSE
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 myplotlib-1.2.0/README.md
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 myplotlib-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 myplotlib-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 myplotlib-1.3.0/MANIFEST.in
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 myplotlib-1.3.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/__init__.py
+-rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/plots.py
+-rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/tests.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/fancy.dark.mplstyle
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/fancy.light.mplstyle
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/hershey.dark.mplstyle
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/hershey.light.mplstyle
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/mono.dark.mplstyle
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/mono.light.mplstyle
+-rw-r--r--   0        0        0    76725 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/colormaps/bipolar.csv
+-rw-r--r--   0        0        0    76800 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/colormaps/colt.csv
+-rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/colormaps/fire.csv
+-rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/colormaps/idl.csv
+-rw-r--r--   0        0        0    38400 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/colormaps/sunrise.csv
+-rw-r--r--   0        0        0    38400 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/colormaps/thermal.csv
+-rw-r--r--   0        0        0    38400 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/colormaps/vanilla.csv
+-rwxr-xr-x   0        0        0   244278 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/fonts/AppleChancery.ttf
+-rw-r--r--   0        0        0   601316 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-Bold.ttf
+-rw-r--r--   0        0        0   567300 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-BoldItalic.ttf
+-rw-r--r--   0        0        0   600940 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-ExtraBold.ttf
+-rw-r--r--   0        0        0   566936 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-ExtraBoldItalic.ttf
+-rw-r--r--   0        0        0   564280 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-Italic.ttf
+-rw-r--r--   0        0        0   601412 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-Medium.ttf
+-rw-r--r--   0        0        0   566872 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-MediumItalic.ttf
+-rw-r--r--   0        0        0   599076 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-Regular.ttf
+-rw-r--r--   0        0        0   601652 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-SemiBold.ttf
+-rw-r--r--   0        0        0   567528 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-SemiBoldItalic.ttf
+-rwxr-xr-x   0        0        0    44328 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/fonts/HersheyTex-Book.otf
+-rwxr-xr-x   0        0        0    31664 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/assets/fonts/HersheyTex-Light.otf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/tools/__init__.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 myplotlib-1.3.0/myplotlib/tools/lic.py
+-rw-r--r--   0        0        0   183246 2020-02-02 00:00:00.000000 myplotlib-1.3.0/previews/None.jpg
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 myplotlib-1.3.0/previews/README.md
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 myplotlib-1.3.0/previews/export_previews.py
+-rw-r--r--   0        0        0   309105 2020-02-02 00:00:00.000000 myplotlib-1.3.0/previews/fancy_dark.jpg
+-rw-r--r--   0        0        0   314876 2020-02-02 00:00:00.000000 myplotlib-1.3.0/previews/fancy_light.jpg
+-rw-r--r--   0        0        0   988613 2020-02-02 00:00:00.000000 myplotlib-1.3.0/previews/hershey_dark.jpg
+-rw-r--r--   0        0        0  1041506 2020-02-02 00:00:00.000000 myplotlib-1.3.0/previews/hershey_light.jpg
+-rw-r--r--   0        0        0   313592 2020-02-02 00:00:00.000000 myplotlib-1.3.0/previews/mono_dark.jpg
+-rw-r--r--   0        0        0   325210 2020-02-02 00:00:00.000000 myplotlib-1.3.0/previews/mono_light.jpg
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 myplotlib-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 myplotlib-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 myplotlib-1.3.0/README.md
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 myplotlib-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 myplotlib-1.3.0/PKG-INFO
```

### Comparing `myplotlib-1.2.0/myplotlib/__init__.py` & `myplotlib-1.3.0/myplotlib/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 
 CUSTOM_CMAPS = []
 
 
 def __RGBToPyCmap(rgbdata):
     import numpy as np
 
@@ -23,28 +23,27 @@
 
 
 def __InstallCmapFromCSV(csv):
     global CUSTOM_CMAPS
     import os
     import numpy as np
     import matplotlib as mpl
-    import matplotlib.pyplot as plt
 
     cmap = os.path.splitext(os.path.basename(csv))[0]
     cmap_data = np.loadtxt(csv, delimiter=",")
-    if cmap not in plt.colormaps():
+    if cmap not in mpl.colormaps.keys():
         CUSTOM_CMAPS.append(cmap)
         mpl_data = __RGBToPyCmap(cmap_data)
-        plt.register_cmap(
+        mpl.colormaps.register(
             cmap=mpl.colors.LinearSegmentedColormap(cmap, mpl_data, cmap_data.shape[0])
         )
     cmap = f"{cmap}_r"
-    if cmap not in plt.colormaps():
+    if cmap not in mpl.colormaps.keys():
         mpl_data_r = __RGBToPyCmap(cmap_data[::-1, :])
-        plt.register_cmap(
+        mpl.colormaps.register(
             cmap=mpl.colors.LinearSegmentedColormap(
                 cmap, mpl_data_r, cmap_data.shape[0]
             )
         )
 
 
 def load(style=None, flavor="light"):
```

### Comparing `myplotlib-1.2.0/myplotlib/plots.py` & `myplotlib-1.3.0/myplotlib/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,15 +332,15 @@
     alphas[alphas < lic_alphamin] = 0
     alphas[alphas > lic_alphamax] = 1
     _ = (
         np.sign(weights - np.average(weights))
         * np.abs(weights - np.average(weights)) ** lic_contrast
     )
     colors = matplotlib.colors.Normalize(None, None)(_)
-    colors = plt.cm.get_cmap(lic_cmap)(colors)
+    colors = matplotlib.colormaps[lic_cmap](colors)
     colors[..., -1] = alphas
 
     colorbar = plot2d(
         ax,
         x,
         y,
         background,
```

### Comparing `myplotlib-1.2.0/myplotlib/tests.py` & `myplotlib-1.3.0/myplotlib/tests.py`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/fancy.dark.mplstyle` & `myplotlib-1.3.0/myplotlib/assets/fancy.dark.mplstyle`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/hershey.dark.mplstyle` & `myplotlib-1.3.0/myplotlib/assets/hershey.dark.mplstyle`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/colormaps/bipolar.csv` & `myplotlib-1.3.0/myplotlib/assets/colormaps/bipolar.csv`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/colormaps/colt.csv` & `myplotlib-1.3.0/myplotlib/assets/colormaps/colt.csv`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/colormaps/fire.csv` & `myplotlib-1.3.0/myplotlib/assets/colormaps/fire.csv`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/colormaps/idl.csv` & `myplotlib-1.3.0/myplotlib/assets/colormaps/idl.csv`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/colormaps/sunrise.csv` & `myplotlib-1.3.0/myplotlib/assets/colormaps/sunrise.csv`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/colormaps/thermal.csv` & `myplotlib-1.3.0/myplotlib/assets/colormaps/thermal.csv`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/colormaps/vanilla.csv` & `myplotlib-1.3.0/myplotlib/assets/colormaps/vanilla.csv`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/fonts/AppleChancery.ttf` & `myplotlib-1.3.0/myplotlib/assets/fonts/AppleChancery.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-Bold.ttf` & `myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-Bold.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-BoldItalic.ttf` & `myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-ExtraBold.ttf` & `myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-ExtraBoldItalic.ttf` & `myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-Italic.ttf` & `myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-Italic.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-Medium.ttf` & `myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-Medium.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-MediumItalic.ttf` & `myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-Regular.ttf` & `myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-Regular.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-SemiBold.ttf` & `myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/fonts/EBGaramond-SemiBoldItalic.ttf` & `myplotlib-1.3.0/myplotlib/assets/fonts/EBGaramond-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/fonts/HersheyTex-Book.otf` & `myplotlib-1.3.0/myplotlib/assets/fonts/HersheyTex-Book.otf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/assets/fonts/HersheyTex-Light.otf` & `myplotlib-1.3.0/myplotlib/assets/fonts/HersheyTex-Light.otf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/myplotlib/tools/lic.py` & `myplotlib-1.3.0/myplotlib/tools/lic.py`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/previews/None.jpg` & `myplotlib-1.3.0/previews/None.jpg`

 * *Files 9% similar despite different names*

#### Image content

```diff
@@ -7,42 +7,42 @@
  . .;t%S;;;;;;tXtt%Xt;t;ttS%t%t%.  .  8%%tt;:::S     %%;t;  
     t;%;;;;;;;;;St;tX%tttXttt%tt.   ..8.t8@%88X;8% 88 8t@%  
   . ;t:::;;t;;:::t;;;%%S%;;;ttt;. .   S8;8%888@8@SS@8@8%SS  
     tttt;.   :t;;;;::::::::;;;;t     .@XX8X8XX@X%tS  88t. . 
   .     .  .      :t;::::;;:       . .;88S%@8;@8@88X%S8S;   
      .        . .       .     .                         . . 
   .   .  .  .      .  .   . .   . .                         
-   .%::ttStt:;:;:%%;%;%@@S8X@@S. t:;::::;::::.::....8::;:;:t
-    %;   .:: . ::.:. :t :;:.:;t.%t@:.       :     ..8:    :t
- %  t.:    .::::t.: .::::%. .;t.:tXX:  .  .:;. .  X8%.. ..@t
- 8. t.;:t::; .;.;    : ::t:;%;t%%88S8:   .%tS8  ..St8: . %8t
- @::t  .:.   .;.  :.   :.::.t:%8S%S.X    SX %S   S8 .%   SXt
- 8t.% ::  . . :..: ...;   .::St8 8. :% ..t: .8.  X:  S  .8%t
- @  %   .  ; :.: .: ..::.   ..tSS%   XX 88. .@S  X. .S8 .X t
- S  t . .;   : :  . ;  ; .: ..t. t . %8:8:   ;.t.X   :;::@ t
-  . %;.XSSX;. :. .  . :     : t St   .8.@  .  %SS:    8@X. t
-  :;S%t8@88St;:;:;:;t;:;:;t:%:t  %;:;:X8@:;::;;88:;:;;;@8:;t
- .;:%.  .     . .S.    .   . .  .;   .S.   %:;;t;t   .S .   
-    .     .:SSS%SS%%SSS          . .    .    %;:  .  .      
-:; .%:;X%%S:::::;::;:::%XS:@:;t     :8%@888%t;t%8@@8S.8@  . 
-%S;%t.%. :@.  .     ..;t t%t. t  .  .8::8@8.  .;.8@@8:8;    
-;XtSt;: . ;:.    .   @t.  :S..t    . X..8X: :: .;@X@8 8%    
-t%;%%t   . t.     .  8 .  .%..t . .; 8 8@@8%;.. 8888@ @S    
-;X.;X.     :;. .    %:  .  ;t t.  .8 X t;%8:::tt:Xt88 88   .
-tS:t%  .  . S..   . t.   . ;;.t .  8 8.8%S. 8888;;t8X.8@    
-tStS%   .   ;t .   %.  .     tt  ..%;.S%X8: .:.:;XSS8.8@ . .
-;StSt .   .  :; . t;       . :S   .  S :@t88  ;;88X8X 8X    
-;St%t.  .   . ;..:X   .  .   .t   . ;8888X8 : ; ;8888 88    
-:: .%::;:;:;:;;@%tt;;::;:;:;::t.    :8 t8@8tt;8.SX888X@8   .
- .  t   .X.   X;t;;S;   %%   %X . .  t% :  ;;:  .  ;  .  .  
-      .;  . .  .:::. . .  ::       .  .    ;t;;.. ..        
-  .  .:tX8X888S8@@@888@@88:;. . . .    .          .    .  . 
-      ;%8X88888@@8X88888@8             .     .           .  
-  . . tS8@8888X888:8888888.  .  . .  .  . .         .  .    
-      ;%8X88@888.X888 XX88.   .    .       .  .  .        . 
-  .  .:t8@@@88:8%8;@888888.%   . .    . .    .    . . . .   
-    . ::S8 8X888X88.@8 888S.       .     . .   .           .
-  .   t%8X@88888:8888S8@%;:.  .  .   .           . . .  .   
-    . tS88@%8@%@8@:88 88S8 .       .   .  . . .       .   . 
-  .  .t%88@888888 X8 @S8@8    . .    .          . .     .   
-     .;%8XX@888@88@888@8@X;t      .    . . .  .    . .    . 
-  .   ..t;..t;;.:: .% ...:..   .    .           .     . .   
+   .%::;;;t;:%S%:ttt;S;tS8XX88%  %%%::::;:t:X.::...;::::;:;t
+    %. ...: ..: ;;:;t .t;.:%tSS %t8t%     @.8  .  .:  .   ;t
+ %  t; :..     .t. t;::  %; :tt.S%888:    SS8:  . :%@%  . ;t
+ 8. t   .  .   :;    .  .:.;;.t%.%8;8;    X:%:   :8:Xt..  %S
+ @;;t  .  .. .:   ...:.; :;...%8SXS.@8  .:X :S   %X .8  . %t
+ 8: % :. .  ;.. .t..:;.   ....t8 @   8   X. .@   X.  X  .:;;
+ @. %    .:  . .:::. : :  ;.; tSSt . X. SX.  tt.88   S  .% t
+ S  t  .;   ...; ;  .t.t    .:t  t   tt:8S   .St88   .@ .% t
+   .%;.XSSX;;..:..     .::  .;t.St   .X88  .  8%8: .  X X; ;
+ .::St;8@88%:t::;;;:;%::;;%::;t  %;:;:X88;::;:S8@:;:;:%88:;t
+  ;;%. .  . . . ;% .  .  . .    .;    X;  .t:;tt;t   :S.    
+      .    :SSS%SS%%SS%       .  .  .   .   .t;:  .    . .  
+:; .%:;8S%S:::::;::::;;%8t:t:;;.    :8%8888%tt;%8@X8S.88    
+%St%t.tt :X.  .   . .t;tSt%S  t   . .8::8X8.  .;.88@8:8;   .
+;X;St;:t  ;:.        @t.;..X. t  .   X..8X: :: .:@X@8 8S    
+t%t%%t.t   t..  . .  8    .%..t   .; 8 8@@8%;.. 8888@ @%   .
+;X.:X  . . ::..     %;. .  .t t.  .8 X t;%8:::tt:Xt@8 88    
+t%;t%.      S..   . %:      ;.t . .8 8.8%S. 8888:;:@X.88  . 
+tStSt . . . :t ..  %    .   .tt   .%;.S%X8: .:.:;@SX8.@@ .  
+;StSt        :: . :;  .   .  :S  .   S :@t88  ;;88X8X 8S   .
+;St%% .  . . .t. :% .   .     %   . ;8888X8 : ; ;8888 88    
+::. %::;:;::::;X%t:;::;::;:;:;t .   :8 t8@8tt;8.S@888X@8    
+    t   .X: . X;t;;S;   %%   tX   .  t% :  ;;:  .  ;  . . . 
+  .  ..;   .  . ;::. . . ..; . .   .  .    ;t;;.. .         
+      :tX8@88SX88X888@8@88:;    . .    .          .    .  . 
+  .  .;%8888@88888888@@888  .          .     .       .      
+   .  ;S8@8X88@88X888tXX88.  . . . .  .  . .       .    .  .
+      t%8@88@@8X@S88XX8888t         .   .     .  .    .     
+ .  . :t88888@t@88:8888@8@;;   . .       .  .      .    . . 
+   .  ::S88@88@.888X8@888@...      . .    .   . .   .       
+     .tt8%888888;8888X@@8;.  .  .      .          .   .  .  
+ .   .tS888888XS@888888@@8.   .   .  .   . . .  .   .  .   .
+   .  t%@@888888X88@88@888  .   .      .          .      .  
+  .  .;%8@@@8888888888888@tt      . .     .  . .    . .    .
+      .:tt: :t. %:  t::..... . .      .    .    . .    . .
```

#### Image metadata

```diff
@@ -10,10 +10,10 @@
 Interlace mode: None
 Rendering intent: Perceptual
 X resolution: 100
 Y resolution: 100
 Resolution units: PixelsPerInch
 Transparency channel enabled: False
 Gamma: 0.454545
-Number of unique colors: 165819
+Number of unique colors: 158290
 Comment: 
 EXIF data:
```

### Comparing `myplotlib-1.2.0/previews/export_previews.py` & `myplotlib-1.3.0/previews/export_previews.py`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/previews/fancy_dark.jpg` & `myplotlib-1.3.0/previews/fancy_dark.jpg`

 * *Files 6% similar despite different names*

#### Image content

```diff
@@ -7,42 +7,42 @@
 8888888888888888888@SXX@8@888@@8888888%88;88.8.:;;%tS%88@888
 88888@88888888@888888@888@8888@8888888;: X8X@t8.S8@8..;88@88
 8888888888888888888@88@888888888888888@8@8S@888@@88S%%@8XX88
 8888888X88888888@88888888888888888888@S888@8@888X8888.S8X888
 888888888888888888@8@8888888888888888@S8@@%%X8X88....S88@888
 888888888888888888888888888888888888888888888@8@888X88888888
 888888888888888888888888888888888X8@@88888888888888@8@888@88
-888XSS@XSXSX%%8S%X;tXSS:t%SSX;X88XX%8XXS%S%X@XXXSSXSX%XSS@@X
-888XX@SS8tSX@XSS8S8SSStXSSSXS%888tX;XSSSSXXXS@SS8X8SXSSXSSSS
-888XS8XSX@XX%XSXt@XX%@SS%@SXXt888:S%%@S8S@S@@SX@S@%;S8S8SSX@
-8S@8SSXXSXXX@S@SSSStXSSXXSS%XS888.%X@8@SXXX@St@%XXSX%S8SSSS8
-8@8X%@@XSXS@SX%@SXS8SSSS@XSX;X@S8 X8%XS8S@XXX;SSS88@%88@%X:@
-8S8@SX@@tXXSt@SS8XXt@@SXSSX@XX@@8:XSS%8X8%SX%X88XSSX8%XSXS%8
-8X8@SSXS@SSSX%X8tXS@SSX@S@%@XSX8@:SSXXS8XS@@8t@@StXSSSSX@X88
-8888%XSXSX@S%8XX@%8S@S8%SS@%8@888;SSXSS88@XXSS8XXXSX@XSSSSXS
-888@%X@ttX@X@S@tXX@SXS@@X8S8XS@8@tSSXSSX%XSSSXt@tXXSXSt%XSXX
-888@S8@SXSXXXtXSS8SSX@SS@%S@SS888SXSS@;%XSSXSXt%@XSSSSSXS8%8
-88888888888888888@88888888888888888888@8888X8888888888@88888
-88888@@@88@88S@XSX@XX@888888888888888@@8888XS8XS@8888X@88888
-888@SX;%%;SSXSSSSSS@X8XS:;S:SXX88888888X8@8;%t;. ::8@ %%8888
-88@XSSt@X;%8@8SSXSXX8SSX@@;S@S8888888@8SX8t;:8 8;8888 XS8888
-8X8SXttSXXt@X@@SX@%8XSSXSSX.X@@888888X8X@@8     S@S@8.8S8888
-8@8@;X@X@tX:XSS8XS8SS SSSXS%SS8888888X;@Xt8;88  8 %SS XX8888
-8X8Xt8@XXX8X@SXSXX8@:%@SXSStS@@8888@8%:%@S. @8:;:8:88.8S8888
-8@8SSSS@X@X@;%8SS88%X@XSSXSS@X@8888X8@8@X8:;88@: 8@@8 XS@888
-8@@SSXXSS8S8SSS8XSXt@XXXSSSX8;8888888S88%8 ..:888SSX8 XX8888
-8@@XSXSXXS8XXSXX@SXXS@SSSSXSSt@88888@%888@S;  ;t88S88.8X@888
-888@SXS@8SSSXSSXSS;SSX8SXXX8X8X88888@S8S888.;.:.t%t8X%8S8888
-888X%@XSSXSSX8S;%S%XXSX@X8@%@t8888888X8@88t%;t8.88@@8XtX@888
-8888@88888@@X@@888X88@@X888X88@888888@888@X8S@88888888S88888
-88888888@S8X8S8X@X@8X8S8X88888888888@8888888888@888888888888
-88888888888888X@.8@8888@88@888888888888888888888888888888888
-8888888888@88@@8X8@888S88XX8888888888888888888@8888888888888
-88888888@X8888888X@;888@888888888888888888888888888888888888
-8888888X88@8S888@S88888S888888888888888888888888888888888888
-888888888@888X8@8X@@8t888888@8888888888888888888888888888888
-8888888@@888@%X888:88888X88888888888888888888888888888888888
-888888@@88@8888@@88 S@888;8888888888888888888888888888888888
-888888@88X8888S88X@8.888@88888888888888888888888888888888888
-888888@X88@8@888888@88@888@888888888888888888888888888888888
-888888888@X@@@8X888888888:@888888888888888888888888888888888
-88888888@8@8@@@8@@@XS888@88888888888888888888888888888888888
+888XSXXSSSSXSSX%%SXSS%SSS;:.: S88%@XSSSX%SSXSXXXSSXtXSSS@S@@
+888XSXXSSSXSS@X@@XS@%@SS@SStS%888;X%S@SSSSS%@SSSXS%S%XSXSXS@
+888XSX@X8X@8@%SSSS%@XS@XX@SS@S@88;;tXXSXSS:tXSSXS@SXt@8SS8S8
+8S@8S8X@X8XXXS@XSXSS@SXX@SXStS@88:tSS8SSStSSSSXSS@;XSXS8XXt@
+8@8@SS@88%X@X@SXS%@@SSXXtXS%@S8X8;@@%@SS@X@@SSSXXSXXS%8SSX%X
+8S8XS@SXXSSSX8@XX@8SS@X88S8XSS@X8:XXSt8@SS@SS8XS%S@X@tSSSSX8
+8X8@%X%@%X8@XSSXXSXSSS@SX@StXS@88;SSX8XSS8SS8SSSX;XSXt%XX88@
+8888SXXSS8SSSSSStXS%8SS%X%XStX888;XSXtS8tS@XSX%8:%@@@SSSXSXX
+888@;SStS%XSX%SSXtX@%@8X@XSXSX@8@tXXXXt%X@X%@@%%%@X@S8t%tXS@
+8888%SXS%SSSSSSS8SSXX8XXS8SXXS@88%X%XStS8S@SSStSXX%XXSS%X8S@
+8888888888888888888888888888888888888888888@8888@88888888888
+888888@@@8888SXSSX@X%888@888@88888888@@888@XX8@X88888SX88888
+888XXS;%%tSS@SSXXSS@@%8S.;X%XX@88888888X8@8;;;;. ;;8@ %S8888
+888@S8;XXSS@%8XSSSSSX%SSSXtSSS@888888@8SX8t;.8 8;8X@8 X%@888
+8X@XX:SS@StXSXXSSSSSS:%8XXSSXX@888888X8S@@888   SXX@8 8S8888
+8@8S;SSSS@StXSSSSXS%X.X%XSX:SS8888888X;@Xt88   ..%8@X SX8888
+8X8StXSXXSXt%XSSSXSS;t@@@XS%S@@8888X8%:%@S88@X;%88t88.8S8888
+8@8SSSSSSX@@:S@SXSStXX8SSXXSSS88888X8@8@@8 .888.;@S88 XS@888
+8@@SSSSSXXXStSXXX8SS8SSXSS@X@t888888@S88S8 ....;t@SX8 XX8888
+8@@XXSSXSSS@XSSXXSXSX@X8@XSSXSX8888@8%888@S; ..8.88@8.8X8888
+888@S@XSXSXXXS%XS8S@SS@SSSSSX8888888@S;8888 ;  8SSt8@%8S8888
+888@tSXSX@XSSSXttSS%@XXSXXX@XS@888888X8@88;%;.8 88@@8XtX@888
+88888@8@@8@@8@8888@8@@8@88X888@888888888@XXXS88@X8@888S88888
+8888888@8S8X8S88SS@S8S8S@8@8888888888@8888888888888888888888
+888888888@8@88@888@@88@@888888888888888888888888888888888888
+8888888888@888X8X8 @8@8@8tX@88888888888888888888888888888888
+88888888@@888X@@88@@888X@88@88888888888888888888888888888888
+8888888X8@8888@@.8X@88888X@888888888888888888888888888888888
+88888888888X8@888X@8@@ 888@888888888888888888888888888888888
+8888888@888.@8t888;88888@@8@88888888888888888888888888888888
+888888@88888888@.8888 t;8t8888888888888888888888888888888888
+888888@@8S88 %8:8@;88888@8XX88888888888888888888888888888888
+888888@@88%8S8888 X8888@8@8888888888888888888888888888888888
+88888888X88@88@8XX88@8@88 @888888888888888888888888888888888
+88888888X8@8X88@S88@88S8S88888888888888888888888888888888888
```

#### Image metadata

```diff
@@ -10,10 +10,10 @@
 Interlace mode: None
 Rendering intent: Perceptual
 X resolution: 150
 Y resolution: 150
 Resolution units: PixelsPerInch
 Transparency channel enabled: False
 Gamma: 0.454545
-Number of unique colors: 264670
+Number of unique colors: 260525
 Comment: 
 EXIF data:
```

### Comparing `myplotlib-1.2.0/previews/fancy_light.jpg` & `myplotlib-1.3.0/previews/mono_light.jpg`

 * *Files 9% similar despite different names*

#### Image content

```diff
@@ -1,48 +1,48 @@
-              tS%%tt                       :%t%%t           
-  . . .;;:;:;;:.   . . .  . . . . .  ;@@88X %S8X88 8X88%t.  
-   .:::;tt;t;tt:;;:;.   ..:;:;::    .%; @XS SSX.8 8 888:  . 
-  ..:tt;tttttt;;ttt;::;:::t;tt;:.    8tS;8888%8 @888888S;   
-   ::tt;:.:.::;%ttt;;t;tt;;ttt;:  .  8X88888;8S XS88888%%%. 
-   .::..:;;;::..:::;%tt;tt;:::;:.    tt8888SX;  8 8 % 8;.:. 
- . .:;;;:t;tt;;;;::..:::::.:;;:.  .  ;%tSX:;:%8X S%St %:;;  
-   .:ttt:t%tt:tttt;;;:;:;:;;ttt;   . :..8S8@888.@8S:  8 %%. 
-  ..;%%%%:t%:t%%%%;t;tttttt;%t%:    .tX8X.8XS88@XS@X888;t%. 
-   ::tttt;  ;tt%ttt%%%t%t%%tttt; .   t8XSXS@ 8XXSXX  88;    
-          .     ..tttttttttt.     .  S88:888@8 88 8SSX@;t. .
- .  . . .    .     .  .  .    . .     ;:;                   
-   .:::;::;:;:;:;:::;::;::;;;:.  :;;;::;::..   .    .:::;:;.
-  .t .  ;. ;.X .  .::;t%.;;;;%t .t @       ;. .    .  .    t
-   %.   ;.:.. .: :: t;::::;t.:t.;%.X; . .  t      .@.   .  t
-   t  . %:: t;:  ; ..:;.::.S;tt.:XXS%  .  .8:; . .;8;    . %
- X t    :;  :.;. :  ;.: ;:  :@%:.%S.@.  . X:%8   S8.8. .  %S
- S;% . :   ..  t;.  . .%  ::.t%@;8  8   .:; X@.  %S .S   .%t
- X.t   % :;. ;    .  :.:  ;. .tX S  %X. :@ .:S:. S   S.  t;;
- S t.. . : ;:  .         . ;  t:;t.  S  X%   S8. @  .%S.%@.t
-  .t ..; .    :.: . :  .. .. :t .t  .%:.X.  .%8:;;   .S %t t
-   t:;;%t%. .t .  t. . .   t .t.;t   ;X.S .   S;% .   S.X .t
-  :%.;;%%;S . .;:;:    t .:;. %  t  . SS:    .t@t   . :X%  t
-  :t;::;:;;::;;;%t;;;;:;::;:;;  .t:;::S;:;:S;:t;%;;::;S::::.
-  ..:;;::;:;;SSSSXtSSt::;;:;::. .   :X@8@t%;;8;t;%X@8S%:.   
-   t  %::t            .;;: ;  t  .  .S88888.:.::88;X%.tX    
-.:;S .%  t:  .  . .   ;. :;; .t     :X88@8;;8   ;8X88;8:    
-;%tS t   ;;.        .;..  .t. t . .  X8XX@8 .   8@S@8:8:    
-:%;S:. . :.;   .  . .t     %. t    :.S:t%S8t8 .  t8@X Xt . .
-:%:S;      ;. .     ; .  . ;; t . .S:SSX8@. X8.t88t88tS@    
-:%:%  .  .  t    . ::  .   :::t   .X.X8@@8:;88@.;XS88;8X  . 
-:ttS .      :: .   ; .    .  ;t     :S88X8 .   t%XSX8:8;    
-:%tS   .  .  ;. . t:   .   . :%  . . X8X8@S; .:8:8S88;@;.  .
- .;S .  .     t  :t  .   .    t    .:X8X888.;  8S%%8@ @%    
-  .t:;:::;:;:;;X%;t;::;:;::;:;t .  .:@88X8t%;:. tS%@8.XS  . 
-   :.  .:t   .% :; %.   t:   ;%   . .:  :  ::     .:   .    
-  .   ;;S%SSSSXX88XXSSS%S@t:    .          .:..   .      .  
-    . ..8XX@8X8S8@X8@X88@8   .    .       .               . 
-  .   :.8@88888@88888888@X     .   .            .     . .   
-      ;t@@888@8@8@@@888@X8    .  .   . .  .      .  .      .
-  . . ::8888%88@t8@@88888;     .   .       . .         .    
-      ;t8@8@88X8S8:88@@@88.:     .    . .      .  .  .   .  
-  .  . .888888;88888888888   . .    .     . .      .   .   .
-      ;t88888@St@88888S@8;       .    .  .   . . .       .  
-  . . ;t8X@;8@S88@@@88@8X8   .     .       .        . .     
-      ;.888888888.88@@@%X8.   . .    . .     .  . .     .  .
-  .  .;t88888@888888888@X ::      .      . .  .     .    .  
-   .    .  :.:..S. .; ..       .    .  .        .    .     .
+            %XS%tS%;SS                    SSt%SS@t          
+  . . .:;;:;:;::       .  . . .  . . ;@888: S8t8@X8 8@St%.  
+   .::;;;t;t;tt:;;:;..  ..:;:t;;     @. @@X XS@8 8 888X   . 
+   .;;t:tttttt;;ttt;::;:::t;t%tt. .  S%S;8@:888 @8888XStt   
+ . .;;tt::.:.::%ttt;;t;tt;;ttSt;    .%@88888S X X88888tt%S; 
+   .:::.:;;:;;..:::;%ttttt;::;;:..   %%XS888X;:.8%;@S %:::. 
+   .::;;:tttt;;;;;:..:.::.:;:t;;   . %8:8S.X.:S S S   @;t;: 
+ . .t;tt;tt%t;;ttt;;;:;:;;:tt%tt .   ;;@:88888%t8St.  :%S%. 
+   .t;%%t;ttt;%%%%t;tttt;tt;tX%%    .%8SX8 XS@8@SX8@S8S;%t:.
+   .;;ttt:. .;%t%tt%%%t%%%%ttSS%   . X@@XS@ 8XXSXX   88:... 
+ .   .  .        .;tttttttt;     .   :8888888:8@X8@X@@t%t.  
+   .   .    .  .    . .   .  .     . .;::              ..   
+          .       .     .      .    . .                . .  
+ .  S;:;:;:t;%;:;t:St:;%:tXSS8 .%S;:8::::;;8 .:;:.:X::::;:8 
+   .S %;;;  ..:; .: .t...St8:X   SS%8     @S.   .S:8. .  .8 
+ X  t.:.  . :::: :...:.X. t.t% :%8X@8   ..8S%    8%XS     8 
+ @  t   . ;;: .    .t. .:..: ttt.8; S    ;; S.   8S 8.. .;8 
+ %:;S .:   ...:;. :% :.: . . %;%%8  %. . S  %.  .@. ;%  :St 
+ 8:.t.  : .  :. ..;.t.:  . ;:ttS.t  .t  tS  ;X .%X   @  S8t.
+ S  %: ;:    :;        .  ::%ttS%t   8.;8:   8  8.  .S: %;t 
+ @  S; :  ;  : .  ..;..:;.;..t..:t . t8X8. . S.%8    t:.X t 
+    %.:SX%S%. : ..     :. ;t;S  tt   .SXt    :8@@. . .X%8 t 
+  ;;S%%8XX@X;%:;:;;:;:;:;:t;S8   S:;:;@8:;:;::X8;:::::X8;:S 
+  :;S   .    . .tt . .  . .  .  .t   .S    X::::X. . %;     
+.:  ::;::;:@XX@S8@%X%@St;::;::      :;;t;;;:StS;;;;tt;;  .  
+;t  t .%:;:          : ;;: ; t .  . :S%X8X. .:;;:;@88XXt  . 
+tSt%t ;: .t      .   ;;..::; t      :;@@X8::8 8 888XtXS:    
+;%tSt;. . ;..  .   . %:   :t t  . . .X88X:;88   t88@8Xt    .
+;tt%%;     ; .      .%    .S t.   :;;;88Stt:8  .Xt888@t:    
+;S:;X.  .  :; .  .  ;;  .  ;;t  . :S:S%888  %8S8;t@S8X8;    
+;%;tS    .  S  .   :::.   ..;t    ;X.;88%8:8888 S88%8%@:  . 
+t%t%%  .    ;;   . ;    .  . X  . ;%;t88@:     88;%@.S@     
+;S%St .  .  :::   :: .       S.      ;@88@t. .8 %@t%@88     
+:%t%t     .   ;. :;    .  .  t   . .t@8X@8.8   :X88@888;   .
+:%  S:;:;::;:;:X%;:;:;::;::;:S .   .:t8@S88:.t %t8@X.88; .  
+... t  ..8    8;t:;@: . Xt   SX  . .:: ;: .  %    :         
+     .:%tttt%%t%X%St%%t%tS;t       .   .  .;;t. .  .      . 
+  .   .:S8@8888888888@88@8 :  . .  .             ..         
+    . t%S88X88@888@888@88@       .  . .  .   .    .       . 
+  .   tSS88888888888888@88:  . .           .    .           
+    . t%X888@8@8.8X@88888S   .   . . . . .    .    .   .  . 
+  .   ;St@888@S8X@@t@888@8%t  .             .    .   .      
+     ..:88888;888X8@888888 ..   .  .  .  .    .        . . .
+  .  .t%S88 S888@@888S@8@S .           .   .    . . .       
+   . .tSXXX@8@8:S888888888     . . .     .   .       . . .  
+     .t%S@8@888@88888888@8   .       .     .   . . .      . 
+ .  ..:XSX8888@88888@@88%;;%    .  .   . .   .       .  .   
+      .:%   %: .X:  t; . ;..  .      .     .   .  .   .   .
```

#### Image metadata

```diff
@@ -10,10 +10,10 @@
 Interlace mode: None
 Rendering intent: Perceptual
 X resolution: 150
 Y resolution: 150
 Resolution units: PixelsPerInch
 Transparency channel enabled: False
 Gamma: 0.454545
-Number of unique colors: 238643
+Number of unique colors: 225946
 Comment: 
 EXIF data:
```

### Comparing `myplotlib-1.2.0/previews/hershey_dark.jpg` & `myplotlib-1.3.0/previews/hershey_dark.jpg`

 * *Files 7% similar despite different names*

#### Image content

```diff
@@ -6,43 +6,43 @@
    .;%%ttXX@XS%%S%tS%%X%%%t%%%t;.    8%SXXXXXSX@St@X8X8.... 
    .;SXX%SXXt%XX@XSX%St%%%%%XX%;..   8 8888888;8%8SSXSXt;:. 
    :;XS@Xt%t;SX@SXSXXSS@X@XX%%%;:.    @8@SSX8X8t:S88;. ;t;: 
    .;S@SXSt;SXX%XX%XX%XSX@%S%S%t.    @%t88X8%S888:8@888:::. 
    .;%%XtX;StS%Xtt@SSS%SXtSXS;;;.   .8:X888XSX888 .S888.::. 
     .:......:::.:;tSttXttS@t;;::    .;@@Xt;X8X:  ;;   8;;:  
      ..     ..  .:..:..:::......     .::  ..::%;:;:::;:..   
-    .....::...:..::::::::.::::.  ..........:.::......:......
-   :.;....;t;.;:.;;::..:;:SXX8:.;:t:...  ..::..     :  ... :
-   ;:;.. :::::::.:;tt;..;:;::@:.;:t:.     :;:.    :%:.    .;
- ..::.  .....;::...;:S:.t;;;.S::tt%;.    .:t;.   .t%;.    ;;
- ;::..  . :......:.....:X;X;%t;;t%t;:.   :;;%:.  :t;t..  .tt
- t:;;. ;:...  ;t%;.:...:St%ttt%XtX..:.   ::.;;.  ;;.:::  ;;;
- t;t:. .. .;:::%;... ;:%t::;t:;%tt..::. .::..;. .%:..%:. %;;
- t:t...   .;:..;;::. :::%.%;t:;tX.. .%:.t;. .;. :;:..::.;S:;
- ::;...   %:%..:..:...;..:::.;;:::. .;..%:. .:::;:.  .t;@:.;
- ..;.....;;..... ....:;;:;t;::;:S.  ..%:;:  ..%:t:.  .ttt:.:
-   :.;;t@t;...:.   :;.::.:.t.:;.:.   .tS;.   .;X;.   .;t;:.:
-  :t;tt;;;t;:::::;;;;::::::::;:.::::::X:;.:;::;;tt::::%t;::.
-  .::;::::;;ttt%%S;tt%;:;;::;:.......%tt;t%@%8@8%tt;tSX;:.. 
-   ;::%;;t..:::::.::::.;t;....:.    .t8S@88.:.;;88%8X t8    
-.;;S..;..::......  ..:;;::::..:.    :;8@@8:;:@ 8:t888 8@    
-.ttt:;:...:..        t:....t..:.    .;88X@:@8    .S@8 X8;   
-.;Stt:.  .::.       .%:.  .t:.:.   ..;.@%tt;    .t8X@.%X.   
- t;S::    .:.       :t..  ..:.:.   ;: t888;t88;;88t88 8t.   
-.;;t:.     .;..    .::.    .:.:.  .t;:8XS@:;XX8;;S%@@.8%:.  
-.ttX.      .S.     ::.      .:;.. .;::8X%8  :;.%@@%S8 @S:.  
- tt%:.      .:.   ;:.       .;;.   ..t8SX8t: .8.88%@8 88:.  
- t;%;.      ..:. .S.        ..:.    :;8%@88 :  888S88:88.   
- ::t..        .;;::.          :.   ..:@8@8t;:. 888S@8 88.   
- ..;::..;t::.;%%t;;S:::.t;:::;t:.   :SS;tS@%SSSX8%t;SX8:    
-  ....:;888@8888888@88888%t:.:.     .:::.: :;t;::......     
-      .@8X888X@88@88888@88t..        . ..  .. . .  ..       
-      :@888SX888888888@8@8;                                 
-      :8XS 888S88@@88@@8@8%                                 
-      :8888888S8@8%@88888X:                                 
-      :S88@88S8888X;88888X%.                                
-      :8888888;88888@8X88@%                                 
-      ;@888888@X:88@8@888%:                                 
-     .:@888888@@88888888X8;                                 
-     .;8888.@8888@88X8@8@8%                                 
-      .%8X@8Xt88@@8888@@8@t                                 
-      :;;;t;;tS;SX%t%t:;;t:.                                
+    .....::::.:..:::::::::::::.  ..........:.::......:......
+   :.:..:%;S:t;;;:::%:%;:@%X8@:.:..;.... .... .    .  ... .:
+   ;:..:..;:;;:;:;.;St;8.:8.SXt:t:%:..    :;:.    .;.     .:
+ ..;:.  ;.:;:.::.;::X.:..:.;Xtt:t:St:.   .t%t.    t%;:     ;
+ ;:;..:.. .:...;.;;:. ...Xt:;;t;%;tt:.   ;t;;.   .;:%:.   .;
+ t:;...  ....  ;.... :.:;;:.;ttX%%;:t.. .t;:;..  :;:;;.   ;;
+ t;t:.    ..%;.:..   ....t;::;t%%t:.:;. .t:.:.. :;:.:;.. .:;
+ t:;:   ;.  ;:;. .  t:. ..;::.;tX:...:...:. .;. :;:..t.. ;.:
+ ::;:   :. :...  ::.%:.:.:;t%tt::.   ;.t:.. .:.:S:. ..;..;::
+ ..:.;.:.:t:.    ..%:. .:;::::::S.  ..;St:.  .;;t:.  .;.:..:
+   ::%XS%t;;:. :. .;:.  .:;...:.:.   .%X..    :t;.    .t;:.:
+  :tt;:;;;;;::::;;:;:::::::::::..:::::t;:::;::;tt;::::ttt:::
+  .:::;;;;;;tt%%%Stttt;::;::::.......%St;tt@%8@@Xt;;tSXt... 
+  .;:.%;:%::::::::::::.;S:....:.    :;8X@88 ::.:88S8X t8    
+.;;%::t::t:........ ..::::::..:.    :;88@8:;:: 88X888 8X    
+.ttX.;t:.::.         ;;.:.:%..:.    .t8@SX: ;   8Xt@8 X8;   
+.tttt:.. .::.       .%:....t:.:.   .:.t8StS:8   8:@XX:S@    
+ t;%;:.   .:.       :;.   ..:.:.   ;:;8X88t.S8t:t8X88 8t.   
+.ttX:     ..:.     .:..    .:.:.. .t;:88S888888: ;%@X.8%:.  
+.ttt:.     .;:.    ::.     ..:;.  .;:t8X@::  .8 @X%S8 8X    
+ tSt:.     ..:.   ::.       .:;.   ..;@8@8S. .;8;88X@ 88..  
+ ;;%:.      ..:. .t:.        .;..   :;8%@88 :.. XSt@8:88.   
+ .:t:.        :::::.         .:.    .:@888 t::8 %S%8@ 88.   
+ ..;::..;;::::t%;;;%;:::t;:::;t:.   :SS;S8XXS@@X8S;XXX8:    
+  ....:t888@8888@88888888%t:.:.     .:::..:;;;;:.......     
+      .88@888@8888888@8@88t..        .      ...     .       
+      .S88@@88@8X88888X@8St.                                
+      ;88@888@888X888X88@:S:                                
+     .:8@@88X8@8:8@@S88@88;                                 
+      :@88888@S@88:888888X%.                                
+      .%88888888X8@@88888@S.                                
+      ;88@@88888t8888X8@8 t                                 
+     .;888888@8888@888888@;                                 
+      :888X888X88X88888888%                                 
+     ..%@@8@@88@X@88888XtX;                                 
+      :;::;%@S%tXStt%::;:t:.
```

#### Image metadata

```diff
@@ -10,10 +10,10 @@
 Interlace mode: None
 Rendering intent: Perceptual
 X resolution: 300
 Y resolution: 300
 Resolution units: PixelsPerInch
 Transparency channel enabled: False
 Gamma: 0.454545
-Number of unique colors: 449443
+Number of unique colors: 466381
 Comment: 
 EXIF data:
```

### Comparing `myplotlib-1.2.0/previews/hershey_light.jpg` & `myplotlib-1.3.0/previews/hershey_light.jpg`

 * *Files 22% similar despite different names*

#### Image content

```diff
@@ -6,43 +6,43 @@
   ..;%%%:;:;::%%%St;;:;;:;;%%tt;     Xt@888S@S. 8X8  :8. .  
    .:;;;.%ttt:;;;:;%%S%%%%%;:;:: . . St.:S.:S  8XXX  X;:;:  
   ..:;tt;.:::;tt%t;;:;:;;;::%t;:     :.8888888%S8@t88 8:t;  
    .:ttttt.:;tttt:tttt%ttt%;;;:;  . .%8XXSSX88@XS%@SSS8:.:  
    ..:::::::::::::ttt;;tt;tt:.:.     %88 888 @@X88XXS88%::. 
  .   .           :::::::::::..  .  . S88@88X88:t;8 @  8;:   
    .   . . . . .     .           .   ..%t::          ..   . 
-   ..:.:.:..:.:.:.::.:.:.:::.:. ..:.:...:... .     ..:.::...
- . ;     ;;  ;. ;.:;tS %t8X8%8t ;.;  .    :        :;    . :
-   ;.. .  %  t:  :   .S..;8;@8; t:@.  .   S  .    ;;; .    ;
- : ;:    t %.   .:;:t ;;t;S%;t:.t%X%    ..S; .    XSX    . t
- % :%;  %S..:X@%.:  . :. :t; 8;:;tt:..   .t.:.   .%.t     :;
- t.;  :  .; ;.@ ..  8: : :t8:.tttt  ;: . ;. ;..  ;: .:   .;:
- t.;   ;8:tt :  .. . .;t: X% ;:%:; .;:   ; .:S  .t   :  .:.:
- t.;;;:;.::   .      %:@;  ;:%:;t:  .S  .;   S% :;  .;  .t :
- : : ..%  ;.  .t t :; .  :  ..: :    t..t  . ;t.X.   .:;:: :
-   ; t:.::;:   .  .     .t.   :.t. . :%tt     ;.t  .  ;S%  :
-  .;8%;StS; . : :   .     ; : : ;    .St..  . ;::    .:X;. :
-  :t;:.:..:..:.:;;::::::.:.:.:. .::.::t;:.:t:.:;t;::::t::.:.
-   ..::.:..;tttt;%;;;t:.::.:.:  .   .tttXXSttXS%SXXSt%t     
- . ;  t:.:           . ;;.    :     .;88t8:.   .;8X88 @8    
-:t:% :t  :..   .   . ;:. ::;  ;  .  .t8XX@8 ::.: .t88.t;.   
-.t;% ;: . ;      .   t.   .t .:    . ;8@S88.8   88S88 8@    
-.;;t:.    .: .      .t.    %  : .  ...;8ttS8 .   %8XX @8..  
-.t.t: .  . ;:  .  . ;:  .  .:.:   .t.:8S88;:8X;:88t88 88:  .
-.;:S       .t      .::      ; : .  %.:88%@88888::X%@X 88    
-.t;%   .    %. . . ;   . .   ;:    :.%88%;.  .:;;8SS8 S8    
-.t;% .   .  :;    :.       . :; . .  :X888S: ...88X@8 @t    
-.;.t       . .;  .t . .  .    ;     :tXS@88 :.::%St@8 88.   
- .:;.  . .    .::..     .   . :  .   :@888 t:::8:t88@ @8:   
-   :.::.tt:::;%;;;:%::::t;::.t;.    :;t@%::8X@S%;.%S;:S;    
-  .   :;%ttt%;;%S%tt%%tt%8;.     .    .    ;::::   .      . 
-   .  .S8%8S8X888@8X8@@888    .   .    .   .   .  ..    .   
-     .:;@8888888S8888@8@88      .   .   .  .    .  . .    . 
- .  . :X@X8888X@8@@@888@88.       .  . .  .  . .   .   .    
-      ;X@X88 @8XX8888888S;    . .        .       .  .    .  
-  .  .:@8.8888X888 @88@@88;       . . .    .  .      .    . 
-   .  .;888888;888;888888@  . .         .       . .   . .   
- .   .:@@88888S@S@@888888:     . .  .      . .      .      .
-     .;X888888@888%8888888   .       . . .     .  .   .  .  
-  .   :S8@8 88888 X88@8S8@      . .          .              
-    . .S8@88@88X8X88@@@8@%..        .  .  .     .  . . . .  
-  .  ...:. tS;; ; .:t:;; t:.  .  .       .   .             .
+   ..:.:..:.:.:.:.:.:.:.:::.:: . .:.:...:... .     ..:.::...
+ . ;;. 8 %X :t  t  ;t@%%S8@t8@; %..; .    :.       ;     . :
+   ;.X S  ; .  :;% %tt; ;%t%tS; :.t;   .  %. .     ;..     :
+ : :..  ::  ;;. %:. :t :S % ;%:.%:;; .   :t;;     .::: . .::
+ % ;..;  .. @:  ;.  t.: X.;: S;::t:::  . .; ;.    ; %.    ;;
+ t.: t:     ;            :;t%Xtt%t  ;.   ;. tt . .; :t   .;:
+ t.t;.  . ;%  :;  .  t .S: t8t;%:;. :;  .;   ;   ;   t  .: :
+ t.:.    ...t    ;   t; .  ..;:;t.  .S: :; . t. .;  .:. ;: :
+ : ;  .; %:t.  .   .   S:   .:: :.   %; %.   ;S %:   .;.;; :
+   : ..;.:.  .;  .  %     .  :; %    .;.;    .@:;. .  tX; .:
+  .:St;tXt%    :   @:@ .;     :.:.  . t;. .   tt:     .St  :
+  :t:.::..::.:::;;:.:::.::t:::. :::.::t;:.:t:::;t:::::t::.:.
+ . ..:..::.:ttt;tt;;tt:.:......     .t%%SXSttXS%SXXStS;     
+   ;  %:.t           : ;t: .  :  .  .;8@%8:.    ;8X88 @8    
+:t;t..t  t..   .  .  ;:.:.:.. :.    .t8XSX8 ::.; .t88.t::   
+.t;% ;   .;  .      .t. :..t .:   .  ;8@X88.t.  .%88X 88:   
+.;;t:.  . .:    . . .t .   t  : .  : .;8%t88 . 8 %8@@.88:.  
+.t.t:      ;. .     ;:    . ; :    % ;8S888 X8.:;%S88 88.  .
+.;:S  .  .  %     ..::.     :.: .  %.:88X8. S@8..SS8X 88    
+.t;%   .    %.  .  ; .  .  . ;:   ...t8S@:   .:;t8%S8 X8    
+.t;% .    . .;    :.         :;      ;@88Xt  .8 tt;8@ @%    
+.;.t    .   . ;  .t   .  .  . :. .  :;8X@8.8  8.%8@88 88.   
+ .:;. .  .    :t:. .    .     :   . .:@8X8:::..8:X8@8 @8:   
+   ::.::;t:::;t;;;:%::::t;:::t;.    :;t@Xt;t;8@SX%SS::S:  . 
+  .   :;%ttt%t;%S%%t%%tt%8;.     .    .    ..::...          
+     . S@X88@X88888X8%8888     .  .       .    .  .     .  .
+  .   :;X@8@88 8@8:@88S@88           . .          .      .  
+    . ;S8S:88888@88@ X8@88.    .  .     .       .  .  .     
+  .   ;SX888X88@%8X8@88@88   .     . .    .       .    .  . 
+    . :X88888@X8888t88@888t..   .     . .   .  .   . .      
+  .   .tt8@@88t8X8;8X@ 888       . .      .     .       . . 
+     .:88X8@8..8;8@8X@S88.    .      .  .   .    . .  .     
+  .  .;X88888@8X8888888@88     .  .    .  .  .      .    .  
+   .  :X88@:X8.X88.8@8@888.         .         . .     .    .
+     ..S8@@8@8888@88888@8:.. .  . .   .  . .      .  .  .   
+ .   ....;t;%. ;%:;:t: : ::    .    .        .  .         .
```

#### Image metadata

```diff
@@ -10,10 +10,10 @@
 Interlace mode: None
 Rendering intent: Perceptual
 X resolution: 300
 Y resolution: 300
 Resolution units: PixelsPerInch
 Transparency channel enabled: False
 Gamma: 0.454545
-Number of unique colors: 482273
+Number of unique colors: 509450
 Comment: 
 EXIF data:
```

### Comparing `myplotlib-1.2.0/previews/mono_dark.jpg` & `myplotlib-1.3.0/previews/mono_dark.jpg`

 * *Files 9% similar despite different names*

#### Image content

```diff
@@ -7,42 +7,42 @@
 8888@8@@88@8@888@88XX@8@@X88888888888XS88S88.8%%;S%S%8888888
 8888@8888@8@8@8888888888@@@8888888888@tS..888t8:t888.:SXXX88
 8888888888888888888@888888888888888888S8.S:@8@88@8@St%88X@88
 888888888888888@8888888888888888888888@8;%8@@8X8@88tS8888888
 8888888888888888888888888888888888888@@888X;tX888:.:%8;@X888
 88888888888888888888888888888888888888@8@@888@8@888888888888
 8888888888888888888888888888888888888888888888888@8888888888
-8888%%S;ttt%XtS%%St%tXt;:.    888t:SS%XSSXSSSS%S@@StS%XS%St@
-8888%8%S8XXX@XXS@SS8@SS@t%S:: 88StX@S@X@X@SX@X@@@8S%S@XXXS%X
-8S@8X@XXSSSSS%X%S8S@XSSSSXSS@.888;%@@SSSX@@SS8%XXXX%%SX%@St8
-8S88SX8tX@XS@XS@SS@SXXSXXXS%Xt8X8ttSX@SXXttStXXSSX;X@XXS@S;@
-8X88SXSXXXX8S@SS@8X@SX%8SSSSS%8S@.XX%SSSXtSX@@SX@XSX;X@XSttX
-8;88%@S8SS%@SXX@@SSXXX@tSXS8S%8X@tX@SSXX;tXXSSX@%tSSXt%@ttX8
-8X88SXXXX@XXS@SSS@8SSSS@XSSSXX8X@;XXSSSX;XXS@%SSSSSXStXXXXS8
-8%@8XXS@XXSS@XSSSSS%@@SX@XX@XSX88;SSXt%S%8S8S%8%;XSSSXS8SXXX
-8888SS@t.;ttSXS@%8%@SX@X@X%@Xt@8@%@S@SS@X8SX@S%SXXSSSS@%X8SX
-8888tXX;.:::%XXX@XS%SXX;@@S%t;@88;S@SSStS%XSSXXtXXXSXS%tXS%@
-88888@888888@@@@88@@@@88@X@@888888X888S8@@@@8888@8X@@@@@@8@8
-88888888888X8%@8tX@SXS@@88888888888888888888X@X@888888888888
-8@88SX%;%tSSX@XS@XX%XSSt.tXSXt8888888%8X@88.::;888@S8SXS8888
-@XX@S@t%8XSXS%8S8%SSXSXX%XX%@t8888888t8XX8.;::. ;88S8@8X8888
-8X@XSSXt@XtSXXS@S8S@X:%88XXSXSX88888@t8XX@:%t. 8:8@X.:8S8888
-8@@@%S@SSXStXSSSSXXXX.@SXSX:XS88888@8:;8S:8;8   88S8@X8@8888
-8S8@t@XSX%X%@8SSSSSS;;XSXSSS;S8888@@8t8X88  t8;.t88S8@@88888
-8X88tXSSSXXS:SXSS%X%XX@SSSSSSS88888@8%88t8:888S.X88X..@88888
-8X@@%@XSSSS@:S@SSSX@8S@SXSSXX:8888@@8%@8S;     88%%X8XX88888
-8S@XX@@8SSSXX8%8@SSSXXSXS8SXS:8888888%8S8@t. .8 %@tS888S8888
-8@@8%8X@@X8S@St@XX:SS@SX@XXSS;888888@%8SX88 :  :S88@8X8S@888
-8@88XSS@@@SSXSXS%%SSXSXSXtXS@S888888@S88X8:Stt; S@S888X88888
-888888@X8S@@88S8888X@@8@S8X@@XS@888888888@X88XS8%88888888888
-8888888X@XX@@XXS@@X8@@@8@88888888888@@88888888888888888@8888
-8888888888888@@88@X@.X8888@888888888888888888888888888888888
-888888@S888@888@88@8888888X888888888888888888888888888888888
-8888888@88@888@88 8@@888888888888888888888888888888888888888
-888888@X888@X8@888@88@8@888888888888888888888888888888888888
-888888@Xt@@88S88@8;8@88@888@88888888888888888888888888888888
-88888888X88888:8.%@X888@88X888888888888888888888888888888888
-888888X88@8888S88@@88@@88%8888888888888888888888888888888888
-8888888S888888@888@8@88@888888888888888888888888888888888888
-888888@888@@@8@8X 8  @@8888888888888888888888888888888888888
-888888@S8@XX88@;888888@88.8@88888888888888888888888888888888
-88888888SX88X@88S8888888X88888888888888888888888888888888888
+8888%tS%X%XSt%%S%St%;t;;;;:   88@t.%S%XSSX%%SSSSS%StS%XS%S;8
+8888%@XX@@%S8@SSX8%SSX%X@S%%; 888%XS@@X@X@;S@8XX@@XXX8XX@S.8
+8S@8XSS@%@X@%XSS@S8SSSXSSXXSS%@88%X;X@S@SS;SSXX8%8tS%SX%@8%8
+8S88S@SX@%SXX%SSSXSSSS8@SXSS8;888SSSX8XX@;%X%SXSSX@XSS8@8%t8
+8X88@@%@XXSXSSS@X8S%@XSSXX8ttS8X@;X8%@8XSXS@SSXS@SSXtXXXS%S8
+8;88S8XtSSSt@%@%8S@@@S@SSS%X8S8S@;X@SX8XSX8XX88SStX@X%@XXtS8
+8X88SSt@SSS8SSSXSSXXSXSSSSX@X;8X@%@XX8@%XS%8@%SS;%@SS;S;S%@S
+8%@8tS@8t8S%@SXSXS@XSX@SSX@SStX88%XSXtX%tS@SXt:SX8%SSS%XX@X8
+8888%XS.:;::SX%SXXSXX%@8%XSS@%88@SXSSS%;SXX8SXtSXXSSXX8StXS8
+8888;%S:.. ::%8SX@XSSSSSSXX8XS@88;SSX8S;%XXX8Xt%%SX8@t%%;SS@
+88888@8888888@@@8888888X8@XX@88888@@X8S8@@X@8888@8XX8@888@@8
+88888888888S@SS@tSXSXS@@88888888888888888888X@X88888@8@88888
+8@88%X%%X%XSSSSXSXSSSXSt.%XSX%8888888%8X@88.::: S88%8X@X8888
+@X@@SXt8@StXXSSSS%XXX%SX;SSX@S@888888t8XX@.;8 8 S88@8XSS8888
+8X@X@XXSXXtX%XSXS8XXStSS%8S:Xt8888888t8XXX:;   .X88X..8X8888
+8@@@S%@XSS@S@SS8XSSSStSXX%X:SS@8888@8::8S:8:8 8.:XX8XX888888
+8S8@.XSSSXS%:X@SSSSStXS%@SXXS%88888@8%8@88  t88;88XX8@8X8888
+8X88%SSXSXX@;SSSS@SS%SX@S8SXSS88888@8t88t8; ;8S ;88%.:X88888
+8X@@S@SSSSS@tX8SXS8;@SS@8S@X@%8888@X8%@8S;     88%SS8@@88888
+8S@X@@SXSX@StSX@SSSSXSX@XS%8S;8888888%8S8@t. .8 %@%%888S8888
+8@@8SSXSXSSX8St@X%%8SS@S%@SSX;@88888@%8@@8.8   :S8888X8X@888
+8@88XX%XtX@8@SS%;S%SSXt@X@X%@t@888888S88X8 t8 8.88X@8@@@8888
+88888@@88S%888X@888S8@@@@8@@@@S@8888@@88@XSX88888@8888888888
+8888888X88SXX@8XS88XXXXXX88888888888X@8888888888@88888888888
+8888888888XX88@88@8X@X88@8@888888888888888888888888888888888
+888888XX8@88888@88888@88XXX888888888888888888888888888888888
+888888@888888@@@S@@88X88888X88888888888888888888888888888888
+8888888X88888 88;8S@888X8X@888888888888888888888888888888888
+888888@X888@8888;8.88888X88888888888888888888888888888888888
+888888888@:@8;8.888;88@8888888888888888888888888888888888888
+888888X@88@88X88 88888@88t8888888888888888888888888888888888
+8888888X8@@88X;88XX8888@@X8888888888888888888888888888888888
+888888@@88@@8888@ 8888888@8888888888888888888888888888888888
+888888@S888@@88%888@888@S:8@88888888888888888888888888888888
+88888888X888X8@8@8@8888@@@8888888888888888888888888888888888
```

#### Image metadata

```diff
@@ -10,10 +10,10 @@
 Interlace mode: None
 Rendering intent: Perceptual
 X resolution: 150
 Y resolution: 150
 Resolution units: PixelsPerInch
 Transparency channel enabled: False
 Gamma: 0.454545
-Number of unique colors: 261763
+Number of unique colors: 254521
 Comment: 
 EXIF data:
```

### Comparing `myplotlib-1.2.0/previews/mono_light.jpg` & `myplotlib-1.3.0/previews/fancy_light.jpg`

 * *Files 12% similar despite different names*

#### Image content

```diff
@@ -1,48 +1,48 @@
-            %XS%tS%;SS                    SSt%SS@t          
-  . . .:;;:;:;::       .  . . .  . . ;@888: S8t8@X8 8@St%.  
-   .::;;;t;t;tt:;;:;..  ..:;:t;;     @. @@X XS@8 8 888X   . 
-   .;;t:tttttt;;ttt;::;:::t;t%tt. .  S%S;8@:888 @8888XStt   
- . .;;tt::.:.::%ttt;;t;tt;;ttSt;    .%@88888S X X88888tt%S; 
-   .:::.:;;:;;..:::;%ttttt;::;;:..   %%XS888X;:.8%;@S %:::. 
-   .::;;:tttt;;;;;:..:.::.:;:t;;   . %8:8S.X.:S S S   @;t;: 
- . .t;tt;tt%t;;ttt;;;:;:;;:tt%tt .   ;;@:88888%t8St.  :%S%. 
-   .t;%%t;ttt;%%%%t;tttt;tt;tX%%    .%8SX8 XS@8@SX8@S8S;%t:.
-   .;;ttt:. .;%t%tt%%%t%%%%ttSS%   . X@@XS@ 8XXSXX   88:... 
- .   .  .        .;tttttttt;     .   :8888888:8@X8@X@@t%t.  
-   .   .    .  .    . .   .  .     . .;::              ..   
-          .   .   .     .   .  .     .                 . .  
- .  S;:;:;:t;:t%%;;:%S;;t%tXX8. ;S@:::;::;:..::;:.@.::::;:X 
-   .t. ;  ;;;   . . ;S. :t%..8 .:@S:      X%    . @t  .  .S 
- X  t;  . .%:.  ;;  ;.:.;.:.:% :%@8;   . .888   ..88 .   ;X 
- @  %t    ;  :. ;.:: ; .:t; ;Stt @t;;   .SX:X:   @%.%  . ;8 
- %;;S. :t ;:  :.. ;  .  .;..;S;%%8  8.  tX  S%. .@: %   .%t 
- 8:.t .  ;  .;    :..t.;. . .ttS @  t;. 8S  .@ .:8  ;8.  St 
- X  t .   .:t  :.  :.. .:    ttS%%   X: @; . X%.t; . 8;:S%t 
- @  tt ;;  ..   . t   ::; .  t.  t . X:.S    XX%8    ;%;@.t 
-   .t.:%X%SS . ..:. :t.%    :t .St   :tSS. . .8X%  . .SXX t 
-  :;X%;8@X@X;::;;;;%;:t%;;t::8   S:;::X8::;:::X@;:;::;8@t:%.
- .:;S   .   . . ;%.  .   . . .  .t   .S .  X::;.X    %:  .  
-..  ::;::;:@XX@S8@%X%@Xt;::;::     ..;tt;;;:St%t;;ttt;;     
-;t .t .%:;:            ;%:   t . .  :S%S@88 ::;;:;@8 XXt. . 
-tSt%t ;; .%   .   . . :.;::: t      ;;@@X@.;. 8 88@%8X:     
-;%tS%:.; .t..   .    t: : :t.t . .  .X@8%@::8   t888.@:     
-;tt%S; . ::;       . % .  .t t    :t;.88%;8%8 8 : 88%8:.    
-;S:;X    ..:: .  .  t      .;t .  :%;S;88888S8%  S8S8X@;    
-;%;tS .     %.     .:  . .  ;t   .;X.;XXS8.;:8S X88@:X@:  . 
-t%t%%   . . ;;  .  t .      .S .  ;%;:88XX:    88;%S8X@.    
-;StX% .      ::  .::    .    S.      t@S88%: .8 %@t%8@8    .
-:%t%t   .  .  ;. :t .  .  .  t   . .t@%8888 :  :%88X8X8;  . 
-:% .%;:;:;::;:;S%;;;::;:;::;:S .   .:t8S88.tt;;;S8@8:88;.   
-..  t   .8   .@;t::@:   Xt   SX  . ..  ::  t:S... ;.        
- .  . :%tt%%t%t%X%S%%t%tt%tt       .       t;t::.         . 
-      ::%@@888888888888888 .. . .  .         .              
-  . . t%@88@@88@88888@888@       .        .       .       . 
-      tXX88S88888@88888@8@  . .    .   .   .  . .   .   .   
-  .  .t%X88888@@@@88@888X@     . .  .   .         .   .   . 
-      ;S%88888XSS8XX88888@t;         .     . .  .   .      .
-  . . ..X88@8;8@88888@8888.. . .  .   .  .     .       . .  
-     .t%S8@888S8S8888S@88;  .    .  .   .   .    . . .     .
-  .  .tSX8888@8888@888888@    .       .   .   .         .   
-    ..t%S888888@@ @8888%S@      .  .    .   .   .  .  .   . 
-  .  .:XS@8888X88X88@X8SS ;%  .     .     .             .   
-      .:S; .S:.:S:. S; . ;. .    .    . .   . .  . . .   . .
+              tS%%tt                       :%t%%t           
+  . . .;;:;:;;:.   . . .  . . . . .  ;@@88X %S8X88 8X88%t.  
+   .:::;tt;t;tt:;;:;.   ..:;:;::    .%; @XS SSX.8 8 888:  . 
+  ..:tt;tttttt;;ttt;::;:::t;tt;:.    8tS;8888%8 @888888S;   
+   ::tt;:.:.::;%ttt;;t;tt;;ttt;:  .  8X88888;8S XS88888%%%. 
+   .::..:;;;::..:::;%tt;tt;:::;:.    tt8888SX;  8 8 % 8;.:. 
+ . .:;;;:t;tt;;;;::..:::::.:;;:.  .  ;%tSX:;:%8X S%St %:;;  
+   .:ttt:t%tt:tttt;;;:;:;:;;ttt;   . :..8S8@888.@8S:  8 %%. 
+  ..;%%%%:t%:t%%%%;t;tttttt;%t%:    .tX8X.8XS88@XS@X888;t%. 
+   ::tttt;  ;tt%ttt%%%t%t%%tttt; .   t8XSXS@ 8XXSXX  88;    
+          .     ..tttttttttt.     .  S88:888@8 88 8SSX@;t. .
+ .  . . .    .     .  .  .    . .     ;:;                   
+   .:::;:;:;::;:;:::;:;;:;:;;:.  :;;:::;::..   .    .:::;:;.
+  .t . .:;; .:   t..:.:Xt:;t;Xt  t@. .        .       .    t
+   t%.:  : t   . ..t.::::t.:;tt.;t8@   .   S  .   :S%   . .S
+  .t        :; . ;.t..:  :;.tXt .SX8   . .@@t  .  %8%.     X
+ X t : . .; .; t.   :: : .. ..t:;8%%@;  .tS;8.    @:S  .  ;%
+ S;% t. :..  t  :  ..::  . :.t%@:8  8%   8t S   .:S %;   .%t
+ X %:   ;.;.:      ;: :.    ::%S S .t% ..S  .%.  @.. S  :;%;
+ S t . . S:   . ;%:.  .. ; t. t:tt   S t;%.  S. ;S   Xt t@ t
+  .t  .;  :. % ; ;:  .  ;t.t;:t. t  .% 8X.  .t%;8:  . %;8X t
+   t.:;%%%.  ..    .  ;..t tX%t tt   t@@8    .%@8     S;X. t
+  :%.;;tS;..  t. :; .  .    . t  t    SS      t@: .  ..8:  t
+  :t;::;::;:;:;;t%;;:;;:;;;:;;  .t:;:;%.:::S;;tt%t:;:;%::;:.
+  ..:;;::;::;X%SXS%SSt:;;:::::.   . .X@8X%t;;SS;ttX@8S%:    
+   t  %::t    .        ;%: : .t     .S88888.:::t.%X@t.tX    
+.:;S .t  ;:.     .  . ;.;:;;  t  . .:X8888t;.8 888S88;8:    
+;%tS t  . ; .        ;: ; .% .;      X88888     ;X%@@ 8;    
+:%;X:.    .;   .  . .t  .  %. t. . :.%;:%%8;. 8 .t8S@t@%   .
+:%:S; .  . ;..      ;.   . :; t   .S:XSX8@;:88:t88t88 8X .  
+:%:S.       S  .  .::  .    ::t . .X.S8@@88 88@.;XS@S;8X   .
+:ttS  . .   t:  .  ;     .  .;t     :S88S%: . .;t@SS8;8;  . 
+:%tS.    .  .;.   t: .       :t  .   X8X88X;. .8.8S88;@t    
+ .tS  .   .   ;. :t   . . .   t   ..:X8X888.:  8S%%8@ @%    
+   t:;:;:;::;:;X%;t;;::;:::;:;t .   :@8S88t%;:. tS%@8.XS  . 
+   :.   :t   .% :; %.   t:   ;%   . .:  ;  :;     .:   .    
+ .   .:tS%%SSSXX88@SSS%SS@t:    .  .       .:..  .       .  
+   .  ..8888888888@8@@8888   .                             .
+      :.888X8888X88@88888S     . . .      .     .     . .   
+ .  . :t8@8@888X@8888@88X8           .  .  .      .       . 
+   .  ;:8888X888X8S@8888Xt    . . .    .     .  .   . .  .  
+      ;t@88888S8888@8888@8;.        .    . .      .         
+ .  . . 888X8888 @88888@88    .  .    .      . .    .  .  . 
+   .  :;888@88X888@8@8888S     .   .    .  .     .    .     
+     .;tX8888888888@888888   .   .   .    .  . .   .    . . 
+ .    ;t8888888888@8X88@@X         .   .    .    .   .      
+   .  ;:@@88@@88@X8@8@8@  ;.   .     .   .    .    .   .  . 
+  .  . .t...:.  %  .t  ;:    .   .     .   .   . .
```

#### Image metadata

```diff
@@ -10,10 +10,10 @@
 Interlace mode: None
 Rendering intent: Perceptual
 X resolution: 150
 Y resolution: 150
 Resolution units: PixelsPerInch
 Transparency channel enabled: False
 Gamma: 0.454545
-Number of unique colors: 228681
+Number of unique colors: 219907
 Comment: 
 EXIF data:
```

### Comparing `myplotlib-1.2.0/.gitignore` & `myplotlib-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/LICENSE` & `myplotlib-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/README.md` & `myplotlib-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `myplotlib-1.2.0/pyproject.toml` & `myplotlib-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires      = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "myplotlib"
 dynamic = ["version"]
-dependencies = ["matplotlib>=3.0.0", "numpy", "numba>=0.57.0"]
+dependencies = ["matplotlib>=3.5.0", "numpy", "numba>=0.57.0"]
 requires-python = ">=3.8"
 authors = [{ name = "Hayk", email = "haykh.astro@gmail.com" }]
 maintainers = [{ name = "Hayk", email = "haykh.astro@gmail.com" }]
 description = "`matplotlib` binder with custom styles and routines for fast plotting"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `myplotlib-1.2.0/PKG-INFO` & `myplotlib-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: myplotlib
-Version: 1.2.0
+Version: 1.3.0
 Summary: `matplotlib` binder with custom styles and routines for fast plotting
 Project-URL: Repository, https://github.com/haykh/myplotlib
 Author-email: Hayk <haykh.astro@gmail.com>
 Maintainer-email: Hayk <haykh.astro@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Hayk Hakobyan
@@ -43,15 +43,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.8
-Requires-Dist: matplotlib>=3.0.0
+Requires-Dist: matplotlib>=3.5.0
 Requires-Dist: numba>=0.57.0
 Requires-Dist: numpy
 Description-Content-Type: text/markdown
 
 # `myplotlib`
 
 `matplotlib` binder with custom styles and routines for fast plotting. see [previews of available styles](https://github.com/haykh/myplotlib/tree/master/previews#readme).
```

