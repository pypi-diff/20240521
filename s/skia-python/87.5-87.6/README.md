# Comparing `tmp/skia_python-87.5-cp39-cp39-win_amd64.whl.zip` & `tmp/skia_python-87.6-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4373511 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat 11247616 b- defN 22-Nov-07 14:49 skia.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1551 b- defN 22-Nov-07 14:49 skia_python-87.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2891 b- defN 22-Nov-07 14:49 skia_python-87.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 22-Nov-07 14:49 skia_python-87.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 22-Nov-07 14:49 skia_python-87.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      485 b- defN 22-Nov-07 14:49 skia_python-87.5.dist-info/RECORD
-6 files, 11252648 bytes uncompressed, 4372639 bytes compressed:  61.1%
+Zip file size: 4421428 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat 11376128 b- defN 24-May-16 18:44 skia.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1551 b- defN 24-May-16 18:44 skia_python-87.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3001 b- defN 24-May-16 18:44 skia_python-87.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-May-16 18:44 skia_python-87.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 24-May-16 18:44 skia_python-87.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      485 b- defN 24-May-16 18:44 skia_python-87.6.dist-info/RECORD
+6 files, 11381270 bytes uncompressed, 4420556 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: skia.cp39-win_amd64.pyd
 Comment: 
 
-Filename: skia_python-87.5.dist-info/LICENSE
+Filename: skia_python-87.6.dist-info/LICENSE
 Comment: 
 
-Filename: skia_python-87.5.dist-info/METADATA
+Filename: skia_python-87.6.dist-info/METADATA
 Comment: 
 
-Filename: skia_python-87.5.dist-info/WHEEL
+Filename: skia_python-87.6.dist-info/WHEEL
 Comment: 
 
-Filename: skia_python-87.5.dist-info/top_level.txt
+Filename: skia_python-87.6.dist-info/top_level.txt
 Comment: 
 
-Filename: skia_python-87.5.dist-info/RECORD
+Filename: skia_python-87.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `skia_python-87.5.dist-info/LICENSE` & `skia_python-87.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `skia_python-87.5.dist-info/METADATA` & `skia_python-87.6.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-Metadata-Version: 2.1
-Name: skia-python
-Version: 87.5
-Summary: Skia python binding
-Home-page: https://github.com/kyamagu/skia-python
-Author: Kota Yamaguchi
-Author-email: KotaYamaguchi1984@gmail.com
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Multimedia :: Graphics
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: pybind11 (>=2.6)
-
-# Skia python binding
-
-![Build and test](https://github.com/kyamagu/skia-python/workflows/Build%20and%20test/badge.svg)
-[![PyPI version](https://badge.fury.io/py/skia-python.svg)](https://badge.fury.io/py/skia-python)
-
-Python binding to [Skia Graphics Library](https://skia.org/).
-
-- Binding based on [pybind11](https://github.com/pybind/pybind11).
-
-## Install
-
-Binary package is available on PyPI:
-
-```bash
-pip install skia-python
-```
-
-Supported platforms:
-
-- Linux x86_64, aarch64
-- macOS x86_64, arm64
-- Windows x86_64
-
-For Linux platforms, there must be OpenGL and fontconfig installed:
-
-```bash
-apt-get install libfontconfig1 libgl1-mesa-glx libgl1-mesa-dri
-```
-
-Or:
-
-```bash
-yum install fontconfig mesa-libGL mesa-dri-drivers
-```
-
-For unsupported environment, check the [build instruction](https://kyamagu.github.io/skia-python/install.html).
-
-## Examples
-
-- [Showcase](https://github.com/kyamagu/skia-python/blob/main/notebooks/Showcase.ipynb)
-- [Canvas Overview](https://github.com/kyamagu/skia-python/blob/main/notebooks/Canvas-Overview.ipynb)
-- [Canvas Creation](https://github.com/kyamagu/skia-python/blob/main/notebooks/Canvas-Creation.ipynb)
-- [Path Overview](https://github.com/kyamagu/skia-python/blob/main/notebooks/Path-Overview.ipynb)
-- [Paint Overview](https://github.com/kyamagu/skia-python/blob/main/notebooks/Paint-Overview.ipynb)
-- [Python Image I/O](https://github.com/kyamagu/skia-python/blob/main/notebooks/Python-Image-IO.ipynb)
-- [Drawing Texts](https://github.com/kyamagu/skia-python/blob/main/notebooks/Drawing-Texts.ipynb)
-
-## Documentation
-
-https://kyamagu.github.io/skia-python
-
-- [Tutorial](https://kyamagu.github.io/skia-python/tutorial/)
-- [Reference](https://kyamagu.github.io/skia-python/reference.html)
-
-## Contributing
-
-Feel free to [post an issue](https://github.com/kyamagu/skia-python/issues) or [PR](https://github.com/kyamagu/skia-python/pulls).
+Metadata-Version: 2.1
+Name: skia-python
+Version: 87.6
+Summary: Skia python binding
+Home-page: https://github.com/kyamagu/skia-python
+Author: Kota Yamaguchi
+Author-email: KotaYamaguchi1984@gmail.com
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pybind11 >=2.6
+
+# Skia python binding
+
+![Build and test](https://github.com/kyamagu/skia-python/workflows/Build%20and%20test/badge.svg)
+[![PyPI version](https://badge.fury.io/py/skia-python.svg)](https://badge.fury.io/py/skia-python)
+
+Python binding to [Skia Graphics Library](https://skia.org/).
+
+- Binding based on [pybind11](https://github.com/pybind/pybind11).
+
+## Install
+
+Binary package is available on PyPI:
+
+```bash
+pip install skia-python
+```
+
+Supported platforms: Python 3.8-3.12 (CPython) on
+
+- Linux x86_64, aarch64
+- macOS x86_64, arm64
+- Windows x86_64
+
+For Linux platforms, there must be OpenGL and fontconfig installed:
+
+```bash
+apt-get install libfontconfig1 libgl1-mesa-glx libgl1-mesa-dri
+```
+
+Or:
+
+```bash
+yum install fontconfig mesa-libGL mesa-dri-drivers
+```
+
+For unsupported environment, check the [build instruction](https://kyamagu.github.io/skia-python/install.html).
+
+## Examples
+
+- [Showcase](https://github.com/kyamagu/skia-python/blob/main/notebooks/Showcase.ipynb)
+- [Canvas Overview](https://github.com/kyamagu/skia-python/blob/main/notebooks/Canvas-Overview.ipynb)
+- [Canvas Creation](https://github.com/kyamagu/skia-python/blob/main/notebooks/Canvas-Creation.ipynb)
+- [Path Overview](https://github.com/kyamagu/skia-python/blob/main/notebooks/Path-Overview.ipynb)
+- [Paint Overview](https://github.com/kyamagu/skia-python/blob/main/notebooks/Paint-Overview.ipynb)
+- [Python Image I/O](https://github.com/kyamagu/skia-python/blob/main/notebooks/Python-Image-IO.ipynb)
+- [Drawing Texts](https://github.com/kyamagu/skia-python/blob/main/notebooks/Drawing-Texts.ipynb)
+
+## Documentation
+
+https://kyamagu.github.io/skia-python
+
+- [Tutorial](https://kyamagu.github.io/skia-python/tutorial/)
+- [Reference](https://kyamagu.github.io/skia-python/reference.html)
+
+## Contributing
+
+Feel free to [post an issue](https://github.com/kyamagu/skia-python/issues) or [PR](https://github.com/kyamagu/skia-python/pulls).
```

