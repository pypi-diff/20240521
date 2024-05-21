# Comparing `tmp/wsidemerger-0.1.2.tar.gz` & `tmp/wsidemerger-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsidemerger-0.1.2.tar", last modified: Tue May 21 11:53:32 2024, max compression
+gzip compressed data, was "wsidemerger-0.1.3.tar", last modified: Tue May 21 12:07:30 2024, max compression
```

## Comparing `wsidemerger-0.1.2.tar` & `wsidemerger-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 11:53:32.214850 wsidemerger-0.1.2/
--rw-rw-rw-   0        0        0     1086 2024-05-21 10:23:57.000000 wsidemerger-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       19 2024-05-21 11:21:04.000000 wsidemerger-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3463 2024-05-21 11:53:32.213853 wsidemerger-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2731 2024-05-21 11:40:02.000000 wsidemerger-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 11:53:32.202646 wsidemerger-0.1.2/WSIdemerger/
--rw-rw-rw-   0        0        0     1137 2024-05-21 11:11:18.000000 wsidemerger-0.1.2/WSIdemerger/Colour_standardisation.py
--rw-rw-rw-   0        0        0     2892 2024-05-21 11:11:24.000000 wsidemerger-0.1.2/WSIdemerger/Patches_generation.py
--rw-rw-rw-   0        0        0      936 2024-05-21 11:10:13.000000 wsidemerger-0.1.2/WSIdemerger/__init__.py
--rw-rw-rw-   0        0        0     1690 2024-05-21 11:12:01.000000 wsidemerger-0.1.2/WSIdemerger/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 11:53:32.212856 wsidemerger-0.1.2/WSIdemerger.egg-info/
--rw-rw-rw-   0        0        0     3463 2024-05-21 11:53:31.000000 wsidemerger-0.1.2/WSIdemerger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-21 11:53:32.000000 wsidemerger-0.1.2/WSIdemerger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 11:53:31.000000 wsidemerger-0.1.2/WSIdemerger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-21 11:53:31.000000 wsidemerger-0.1.2/WSIdemerger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-21 11:53:31.000000 wsidemerger-0.1.2/WSIdemerger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 11:53:32.214850 wsidemerger-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1123 2024-05-21 11:49:28.000000 wsidemerger-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:07:30.141935 wsidemerger-0.1.3/
+-rw-rw-rw-   0        0        0     1086 2024-05-21 10:23:57.000000 wsidemerger-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       19 2024-05-21 11:21:04.000000 wsidemerger-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3476 2024-05-21 12:07:30.140742 wsidemerger-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2744 2024-05-21 12:02:51.000000 wsidemerger-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 12:07:30.128898 wsidemerger-0.1.3/WSIdemerger/
+-rw-rw-rw-   0        0        0     1135 2024-05-21 12:04:52.000000 wsidemerger-0.1.3/WSIdemerger/Colour_standardisation.py
+-rw-rw-rw-   0        0        0     2890 2024-05-21 12:05:15.000000 wsidemerger-0.1.3/WSIdemerger/Patches_generation.py
+-rw-rw-rw-   0        0        0      936 2024-05-21 11:10:13.000000 wsidemerger-0.1.3/WSIdemerger/__init__.py
+-rw-rw-rw-   0        0        0     1688 2024-05-21 12:05:38.000000 wsidemerger-0.1.3/WSIdemerger/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:07:30.137240 wsidemerger-0.1.3/WSIdemerger.egg-info/
+-rw-rw-rw-   0        0        0     3476 2024-05-21 12:07:29.000000 wsidemerger-0.1.3/WSIdemerger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-21 12:07:30.000000 wsidemerger-0.1.3/WSIdemerger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 12:07:29.000000 wsidemerger-0.1.3/WSIdemerger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-21 12:07:29.000000 wsidemerger-0.1.3/WSIdemerger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 12:07:29.000000 wsidemerger-0.1.3/WSIdemerger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 12:07:30.142938 wsidemerger-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1123 2024-05-21 12:04:13.000000 wsidemerger-0.1.3/setup.py
```

### Comparing `wsidemerger-0.1.2/LICENSE` & `wsidemerger-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wsidemerger-0.1.2/PKG-INFO` & `wsidemerger-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WSIdemerger
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for extracting image patches from SVS files and performing color normalization
 Home-page: https://github.com/yourusername/WSI_Preprocessing
 Author: Thirteen
 Author-email: 506607814@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -28,26 +28,26 @@
 ## Installation
 
 To install this package, use:
 
 ```sh
 pip install WSIdemerger
 ```
-
+![img.png](img.png)
 ## Usage
 
 ### Key Verification
 
 To use this package, you will need to input a key for verification. When you run the functions from this package, you will be prompted to enter the key. Ensure you have the correct key to proceed.
 
 ### Extract Patches
 To extract patches from SVS files, use the process_svs_files function:
 
 ```sh
-from WSIprocessing import process_svs_files
+from WSIdemerger import process_svs_files
 
 # Define the paths
 base_path = 'path/to/your/svs/files'
 output_base = 'path/to/output/folder'
 threshold = 50  # Saturation threshold for saving patches
 patch_size = 512  # Size of the patches
 target_magnification = 20  # Target magnification level
@@ -56,15 +56,15 @@
 process_svs_files(base_path, output_base, saturation_threshold=threshold, patch_size=patch_size, target_magnification=target_magnification)
 ```
 
 ### Normalize Images
 
 To normalize images using a reference image, use the normalize_images function:
 ```sh
-from WSIprocessing import normalize_images
+from WSIdemerger import normalize_images
 
 # Define the paths
 input_folder = 'path/to/your/input/images'
 reference_image_path = 'path/to/your/reference/image.png'
 output_folder = 'path/to/output/folder'
 
 # Normalize images
@@ -75,15 +75,15 @@
 Here is a complete example of how to use both functionalities:
 
 1、Extract patches from SVS files and save them to a specified directory.
 
 2、Normalize the extracted patches using a reference image.
 
 ```sh
-from WSIprocessing import process_svs_files, normalize_images
+from WSIdemerger import process_svs_files, normalize_images
 
 # Step 1: Extract patches
 base_path = 'path/to/your/svs/files'
 output_base = 'path/to/output/folder'
 threshold = 50  # Saturation threshold for saving patches
 patch_size = 512  # Size of the patches
 target_magnification = 20  # Target magnification level
```

### Comparing `wsidemerger-0.1.2/README.md` & `wsidemerger-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 ## Installation
 
 To install this package, use:
 
 ```sh
 pip install WSIdemerger
 ```
-
+![img.png](img.png)
 ## Usage
 
 ### Key Verification
 
 To use this package, you will need to input a key for verification. When you run the functions from this package, you will be prompted to enter the key. Ensure you have the correct key to proceed.
 
 ### Extract Patches
 To extract patches from SVS files, use the process_svs_files function:
 
 ```sh
-from WSIprocessing import process_svs_files
+from WSIdemerger import process_svs_files
 
 # Define the paths
 base_path = 'path/to/your/svs/files'
 output_base = 'path/to/output/folder'
 threshold = 50  # Saturation threshold for saving patches
 patch_size = 512  # Size of the patches
 target_magnification = 20  # Target magnification level
@@ -33,15 +33,15 @@
 process_svs_files(base_path, output_base, saturation_threshold=threshold, patch_size=patch_size, target_magnification=target_magnification)
 ```
 
 ### Normalize Images
 
 To normalize images using a reference image, use the normalize_images function:
 ```sh
-from WSIprocessing import normalize_images
+from WSIdemerger import normalize_images
 
 # Define the paths
 input_folder = 'path/to/your/input/images'
 reference_image_path = 'path/to/your/reference/image.png'
 output_folder = 'path/to/output/folder'
 
 # Normalize images
@@ -52,15 +52,15 @@
 Here is a complete example of how to use both functionalities:
 
 1、Extract patches from SVS files and save them to a specified directory.
 
 2、Normalize the extracted patches using a reference image.
 
 ```sh
-from WSIprocessing import process_svs_files, normalize_images
+from WSIdemerger import process_svs_files, normalize_images
 
 # Step 1: Extract patches
 base_path = 'path/to/your/svs/files'
 output_base = 'path/to/output/folder'
 threshold = 50  # Saturation threshold for saving patches
 patch_size = 512  # Size of the patches
 target_magnification = 20  # Target magnification level
```

### Comparing `wsidemerger-0.1.2/WSIdemerger/Colour_standardisation.py` & `wsidemerger-0.1.3/WSIdemerger/Colour_standardisation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# WSIprocessing/Colour_standardisation.py
+# WSIdemerger/Colour_standardisation.py
 import os
 import cv2
 import staintools
 from pathlib import Path
 from tqdm import tqdm
 
 def normalize_images(input_folder, reference_image_path, output_folder):
```

### Comparing `wsidemerger-0.1.2/WSIdemerger/Patches_generation.py` & `wsidemerger-0.1.3/WSIdemerger/Patches_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# WSIprocessing/Patches_generation.py
+# WSIdemerger/Patches_generation.py
 import os
 import pandas as pd
 import openslide
 from PIL import Image
 import numpy as np
 from skimage.color import rgb2hsv
 from skimage import img_as_ubyte
```

### Comparing `wsidemerger-0.1.2/WSIdemerger/__init__.py` & `wsidemerger-0.1.3/WSIdemerger/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidemerger-0.1.2/WSIdemerger/utils.py` & `wsidemerger-0.1.3/WSIdemerger/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# WSIprocessing/utils.py
+# WSIdemerger/utils.py
 import numpy as np
 from skimage.color import rgb2hsv
 from skimage import img_as_ubyte
 import os
 import shutil
 import logging
```

### Comparing `wsidemerger-0.1.2/WSIdemerger.egg-info/PKG-INFO` & `wsidemerger-0.1.3/WSIdemerger.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WSIdemerger
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for extracting image patches from SVS files and performing color normalization
 Home-page: https://github.com/yourusername/WSI_Preprocessing
 Author: Thirteen
 Author-email: 506607814@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -28,26 +28,26 @@
 ## Installation
 
 To install this package, use:
 
 ```sh
 pip install WSIdemerger
 ```
-
+![img.png](img.png)
 ## Usage
 
 ### Key Verification
 
 To use this package, you will need to input a key for verification. When you run the functions from this package, you will be prompted to enter the key. Ensure you have the correct key to proceed.
 
 ### Extract Patches
 To extract patches from SVS files, use the process_svs_files function:
 
 ```sh
-from WSIprocessing import process_svs_files
+from WSIdemerger import process_svs_files
 
 # Define the paths
 base_path = 'path/to/your/svs/files'
 output_base = 'path/to/output/folder'
 threshold = 50  # Saturation threshold for saving patches
 patch_size = 512  # Size of the patches
 target_magnification = 20  # Target magnification level
@@ -56,15 +56,15 @@
 process_svs_files(base_path, output_base, saturation_threshold=threshold, patch_size=patch_size, target_magnification=target_magnification)
 ```
 
 ### Normalize Images
 
 To normalize images using a reference image, use the normalize_images function:
 ```sh
-from WSIprocessing import normalize_images
+from WSIdemerger import normalize_images
 
 # Define the paths
 input_folder = 'path/to/your/input/images'
 reference_image_path = 'path/to/your/reference/image.png'
 output_folder = 'path/to/output/folder'
 
 # Normalize images
@@ -75,15 +75,15 @@
 Here is a complete example of how to use both functionalities:
 
 1、Extract patches from SVS files and save them to a specified directory.
 
 2、Normalize the extracted patches using a reference image.
 
 ```sh
-from WSIprocessing import process_svs_files, normalize_images
+from WSIdemerger import process_svs_files, normalize_images
 
 # Step 1: Extract patches
 base_path = 'path/to/your/svs/files'
 output_base = 'path/to/output/folder'
 threshold = 50  # Saturation threshold for saving patches
 patch_size = 512  # Size of the patches
 target_magnification = 20  # Target magnification level
```

### Comparing `wsidemerger-0.1.2/setup.py` & `wsidemerger-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     try:
         return open(os.path.join(os.path.dirname(__file__), file_name)).read()
     except FileNotFoundError:
         return ""
 
 setup(
     name='WSIdemerger',
-    version='0.1.2',  # 更新版本号
+    version='0.1.3',  # 更新版本号
     packages=find_packages(),
     install_requires=[
         'pandas',
         'openslide-python',
         'Pillow',
         'numpy',
         'scikit-image',
```

