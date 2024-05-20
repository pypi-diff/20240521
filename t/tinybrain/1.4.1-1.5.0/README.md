# Comparing `tmp/tinybrain-1.4.1.tar.gz` & `tmp/tinybrain-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybrain-1.4.1.tar", last modified: Tue Dec 19 07:52:12 2023, max compression
+gzip compressed data, was "tinybrain-1.5.0.tar", last modified: Mon May 20 22:41:11 2024, max compression
```

## Comparing `tinybrain-1.4.1.tar` & `tinybrain-1.5.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-12-19 07:52:12.822786 tinybrain-1.4.1/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-12-19 07:52:12.812539 tinybrain-1.4.1/.github/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-12-19 07:52:12.819851 tinybrain-1.4.1/.github/workflows/
--rw-r--r--   0 wms        (501) staff       (20)      966 2023-12-19 06:51:58.000000 tinybrain-1.4.1/.github/workflows/build_wheel.yml
--rw-r--r--   0 wms        (501) staff       (20)      878 2022-08-26 19:08:36.000000 tinybrain-1.4.1/.github/workflows/run_tests.yml
--rw-r--r--   0 wms        (501) staff       (20)       97 2023-12-19 07:52:11.000000 tinybrain-1.4.1/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     4952 2023-12-19 07:52:11.000000 tinybrain-1.4.1/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)    35149 2021-01-20 17:58:46.000000 tinybrain-1.4.1/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)    10798 2023-12-19 07:52:12.823161 tinybrain-1.4.1/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     8879 2022-03-05 06:53:04.000000 tinybrain-1.4.1/README.md
--rw-r--r--   0 wms        (501) staff       (20)    23095 2023-06-08 20:17:42.000000 tinybrain-1.4.1/automated_test.py
--rwxr-xr-x   0 wms        (501) staff       (20)      709 2022-02-07 19:05:06.000000 tinybrain-1.4.1/build_linux.sh
--rw-r--r--   0 wms        (501) staff       (20)     1204 2021-03-17 20:30:55.000000 tinybrain-1.4.1/manylinux1.Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)     1235 2021-03-17 20:30:55.000000 tinybrain-1.4.1/manylinux2010.Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)     1558 2022-02-07 19:05:11.000000 tinybrain-1.4.1/manylinux2014.Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)     4337 2022-03-05 06:53:04.000000 tinybrain-1.4.1/perf.py
--rw-r--r--   0 wms        (501) staff       (20)       90 2022-02-07 19:58:32.000000 tinybrain-1.4.1/pyproject.toml
--rw-r--r--   0 wms        (501) staff       (20)        6 2021-12-02 23:06:40.000000 tinybrain-1.4.1/requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)        6 2023-05-11 20:23:25.000000 tinybrain-1.4.1/requirements_dev.txt
--rw-r--r--   0 wms        (501) staff       (20)      925 2023-12-19 07:52:12.823995 tinybrain-1.4.1/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)     1146 2023-12-19 06:52:32.000000 tinybrain-1.4.1/setup.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-12-19 07:52:12.821101 tinybrain-1.4.1/tinybrain/
--rw-r--r--   0 wms        (501) staff       (20)      183 2023-12-19 06:53:47.000000 tinybrain-1.4.1/tinybrain/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)    29621 2023-06-08 20:17:42.000000 tinybrain-1.4.1/tinybrain/accelerated.hpp
--rw-r--r--   0 wms        (501) staff       (20)    28263 2023-06-08 20:17:42.000000 tinybrain-1.4.1/tinybrain/accelerated.pyx
--rw-r--r--   0 wms        (501) staff       (20)    15569 2023-06-08 20:17:42.000000 tinybrain-1.4.1/tinybrain/downsample.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-12-19 07:52:12.822603 tinybrain-1.4.1/tinybrain.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)    10798 2023-12-19 07:52:11.000000 tinybrain-1.4.1/tinybrain.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      616 2023-12-19 07:52:12.000000 tinybrain-1.4.1/tinybrain.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-12-19 07:52:11.000000 tinybrain-1.4.1/tinybrain.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2021-01-20 17:59:34.000000 tinybrain-1.4.1/tinybrain.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2023-12-19 07:52:11.000000 tinybrain-1.4.1/tinybrain.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)        6 2023-12-19 07:52:11.000000 tinybrain-1.4.1/tinybrain.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)       10 2023-12-19 07:52:11.000000 tinybrain-1.4.1/tinybrain.egg-info/top_level.txt
--rw-r--r--   0 wms        (501) staff       (20)      241 2023-12-19 06:54:23.000000 tinybrain-1.4.1/tox.ini
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-05-20 22:41:11.908557 tinybrain-1.5.0/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-05-20 22:41:11.899271 tinybrain-1.5.0/.github/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-05-20 22:41:11.904645 tinybrain-1.5.0/.github/workflows/
+-rw-r--r--   0 wms        (501) staff       (20)      966 2024-05-20 21:45:30.000000 tinybrain-1.5.0/.github/workflows/build_wheel.yml
+-rw-r--r--   0 wms        (501) staff       (20)      904 2024-05-20 21:46:23.000000 tinybrain-1.5.0/.github/workflows/run_tests.yml
+-rw-r--r--   0 wms        (501) staff       (20)       97 2024-05-20 22:41:10.000000 tinybrain-1.5.0/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     5108 2024-05-20 22:41:10.000000 tinybrain-1.5.0/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)    35149 2021-01-20 17:58:46.000000 tinybrain-1.5.0/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)     9791 2024-05-20 22:41:11.908412 tinybrain-1.5.0/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     8879 2022-03-05 06:53:04.000000 tinybrain-1.5.0/README.md
+-rw-r--r--   0 wms        (501) staff       (20)    24432 2024-05-20 21:38:58.000000 tinybrain-1.5.0/automated_test.py
+-rwxr-xr-x   0 wms        (501) staff       (20)      709 2022-02-07 19:05:06.000000 tinybrain-1.5.0/build_linux.sh
+-rw-r--r--   0 wms        (501) staff       (20)     1204 2021-03-17 20:30:55.000000 tinybrain-1.5.0/manylinux1.Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)     1235 2021-03-17 20:30:55.000000 tinybrain-1.5.0/manylinux2010.Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)     1558 2022-02-07 19:05:11.000000 tinybrain-1.5.0/manylinux2014.Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)     4337 2022-03-05 06:53:04.000000 tinybrain-1.5.0/perf.py
+-rw-r--r--   0 wms        (501) staff       (20)       90 2022-02-07 19:58:32.000000 tinybrain-1.5.0/pyproject.toml
+-rw-r--r--   0 wms        (501) staff       (20)        6 2021-12-02 23:06:40.000000 tinybrain-1.5.0/requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)        6 2023-05-11 20:23:25.000000 tinybrain-1.5.0/requirements_dev.txt
+-rw-r--r--   0 wms        (501) staff       (20)      925 2024-05-20 22:41:11.908977 tinybrain-1.5.0/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)     1146 2023-12-19 06:52:32.000000 tinybrain-1.5.0/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-05-20 22:41:11.906059 tinybrain-1.5.0/tinybrain/
+-rw-r--r--   0 wms        (501) staff       (20)      183 2023-12-19 06:53:47.000000 tinybrain-1.5.0/tinybrain/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)    29621 2023-06-08 20:17:42.000000 tinybrain-1.5.0/tinybrain/accelerated.hpp
+-rw-r--r--   0 wms        (501) staff       (20)    28263 2023-06-08 20:17:42.000000 tinybrain-1.5.0/tinybrain/accelerated.pyx
+-rw-r--r--   0 wms        (501) staff       (20)    16031 2024-05-20 21:29:24.000000 tinybrain-1.5.0/tinybrain/downsample.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-05-20 22:41:11.908034 tinybrain-1.5.0/tinybrain.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)     9791 2024-05-20 22:41:10.000000 tinybrain-1.5.0/tinybrain.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      616 2024-05-20 22:41:11.000000 tinybrain-1.5.0/tinybrain.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2024-05-20 22:41:10.000000 tinybrain-1.5.0/tinybrain.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2021-01-20 17:59:34.000000 tinybrain-1.5.0/tinybrain.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2024-05-20 22:41:10.000000 tinybrain-1.5.0/tinybrain.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)        6 2024-05-20 22:41:10.000000 tinybrain-1.5.0/tinybrain.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)       10 2024-05-20 22:41:10.000000 tinybrain-1.5.0/tinybrain.egg-info/top_level.txt
+-rw-r--r--   0 wms        (501) staff       (20)      241 2023-12-19 06:54:23.000000 tinybrain-1.5.0/tox.ini
```

### Comparing `tinybrain-1.4.1/.github/workflows/build_wheel.yml` & `tinybrain-1.5.0/.github/workflows/build_wheel.yml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
       - uses: actions/checkout@v4
 
       - name: Set up QEMU
         if:  ${{ matrix.arch == 'aarch64' }}
         uses: docker/setup-qemu-action@v1
 
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.16.2
+        uses: pypa/cibuildwheel@v2.16.5
         # to supply options, put them in 'env', like:
         env:
           CIBW_ARCHS_LINUX: ${{matrix.arch}}
           CIBW_BEFORE_BUILD: pip install oldest-supported-numpy setuptools wheel cython
 
       - uses: actions/upload-artifact@v2
         with:
```

### Comparing `tinybrain-1.4.1/.github/workflows/run_tests.yml` & `tinybrain-1.5.0/.github/workflows/run_tests.yml`

 * *Files 27% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 jobs:
   run_tests:
     name: Test ${{ matrix.os }} Python ${{ matrix.python-version }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-20.04, macos-latest, windows-2019]
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
 
       - uses: actions/checkout@v2
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install pytest -r requirements.txt -r requirements_dev.txt
+          python -m pip install pytest -r requirements.txt -r requirements_dev.txt setuptools wheel
 
       - name: Compile
         run: python setup.py develop
 
       - name: Test with pytest
         run: pytest -v -x automated_test.py
```

### Comparing `tinybrain-1.4.1/ChangeLog` & `tinybrain-1.5.0/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+1.5.0
+-----
+
+* ci: install setuptools, wheel
+* ci: update cibuildwheel to non-buggy version
+* ci: update tests, -3.7, +3.11, +3.12
+* feat: add min pooling
+
 1.4.1
 -----
 
 * build: more update for py312
 * build: update for py312
 
 1.4.0
```

### Comparing `tinybrain-1.4.1/LICENSE` & `tinybrain-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tinybrain-1.4.1/PKG-INFO` & `tinybrain-1.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,150 +1,151 @@
 Metadata-Version: 2.1
 Name: tinybrain
-Version: 1.4.1
+Version: 1.5.0
 Summary: Image pyramid generation specialized for connectomics data types and procedures.
 Home-page: https://github.com/seung-lab/tinybrain/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
-License: UNKNOWN
-Description: [![Build Status](https://travis-ci.org/seung-lab/tinybrain.svg?branch=master)](https://travis-ci.org/seung-lab/tinybrain) [![PyPI version](https://badge.fury.io/py/tinybrain.svg)](https://badge.fury.io/py/tinybrain)  
-        
-        # tinybrain
-        
-        Image pyramid generation specialized for connectomics data types and procedures. If your brain wasn't tiny before, it will be now.  
-        
-        ```python 
-        import tinybrain 
-        
-        img = load_3d_em_stack()
-        
-        # 2x2 and 2x2x2 downsamples are on a fast path.
-        # e.g. (2,2), (2,2,1), (2,2,1,1), (2,2,2), (2,2,2,1)
-        img_pyramid = tinybrain.downsample_with_averaging(img, factor=(2,2,1), num_mips=5, sparse=False)
-        
-        labels = load_3d_labels()
-        label_pyramid = tinybrain.downsample_segmentation(labels, factor=(2,2,1), num_mips=5, sparse=False))
-        ```
-        
-        ## Installation 
-        
-        ```bash
-        pip install numpy
-        pip install tinybrain
-        ```
-        
-        ## Motivation
-        
-        Image hierarchy generation in connectomics uses a few different techniques for
-        visualizing data, but predominantly we create image pyramids of uint8 grayscale images using 2x2 average pooling and of uint8 to uint64 segmentation labels using 2x2 mode pooling. When images become very large and people wish to visualze upper mip levels using three axes at once, it becomes desirable to perform 2x2x2 downsamples to maintain isotropy.
-        
-        It's possible to compute both of these using numpy, however as multiple packages found it useful to copy the downsample functions, it makes sense to formalize these functions into a seperate library located on PyPI.
-        
-        Given the disparate circumstances that they will be used in, these functions should work 
-        fast as possible with low memory usage and avoid numerical issues such as integer truncation
-        while generating multiple mip levels.
-        
-        ## Considerations: downsample_with_averaging 
-        
-        It's advisable to generate multiple mip levels at once rather than recursively computing
-        new images as for integer type images, this leads to integer truncation issues. In the common
-        case of 2x2x1 downsampling, a recursively computed image would lose 0.75 brightness per a 
-        mip level. Therefore, take advantage of the `num_mips` argument which strikes a balance
-        that limits integer truncation loss to once every 4 mip levels. This compromise allows
-        for the use of integer arithmatic and no more memory usage than 2x the input image including
-        the output downsamples. If you seek to eliminate the loss beyond 4 mip levels, try promoting 
-        the type before downsampling. 2x2x2x1 downsamples truncate every 8 mip levels.
-        
-        A C++ high performance path is triggered for 2x2x1x1 and 2x2x2x1 downsample factors on uint8, uint16, float32, 
-        and float64 data types in Fortran order. Other factors, data types, and orderings are computed using a numpy pathway that is much slower and more memory intensive.
-        
-        We also include a sparse mode for downsampling 2x2x2 patches, which prevents "ghosting" where one z-slice overlaps a black region on the next slice and becomes semi-transparent after downsampling. We deal with this by neglecting the background pixels from the averaging operation. 
-        
-        ### Example Benchmark 
-        
-        On a 1024x1024x100 uint8 image I ran the following code. PIL and OpenCV are actually much faster than this benchmark shows because most of the time is spent writing to the numpy array. tinybrain has a large advantage working on 3D and 4D arrays. Of course, this is a very simple benchmark and it may be possible to tune each of these approaches. On single slices, Pillow was faster than tinybrain.
-        
-        ```python
-        img = np.load("image.npy")
-        
-        s = time.time()
-        downsample_with_averaging(img, (2,2,1))
-        print("Original ", time.time() - s)
-        
-        s = time.time()
-        out = tinybrain.downsample_with_averaging(img, (2,2,1))
-        print("tinybrain ", time.time() - s)
-        
-        s = time.time()
-        out = np.zeros(shape=(512,512,100))
-        for z in range(img.shape[2]):
-          out[:,:,z] = cv2.resize(img[:,:,z], dsize=(512, 512) )
-        print("OpenCV ", time.time() - s)
-        
-        s = time.time()
-        out = np.zeros(shape=(512,512,100))
-        for z in range(img.shape[2]):
-          pilimg = Image.fromarray(img[:,:,z])
-          out[:,:,z] = pilimg.resize( (512, 512) )
-        print("Pillow ", time.time() - s)
-        
-        # Method     Run Time             Rel. Perf.
-        # Original   1820 ms +/- 3.73 ms    1.0x
-        # tinybrain    67 ms +/- 0.40 ms   27.2x 
-        # OpenCV      469 ms +/- 1.12 ms    3.9x
-        # Pillow      937 ms +/- 7.63 ms    1.9x
-        ```
-        
-        Here's the output from `perf.py` on an Apple Silicon 2021 Macbook Pro M1.
-        Note that the image used was a random 2048x2048x64 array that was a uint8
-        for average pooling and a uint64 for mode pooling to represent real use cases more fairly. In the table, read it as 2D or 3D downsamples, generating a single or multiple mip levels, with sparse mode enabled or disabled. The speed values are in megavoxels per a second and are the mean of ten runs.
-        
-        
-        | dwnsmpl  |   mips  |   sparse  |   AVG (MVx/sec)  |   MODE (MVx/sec)  |
-        |----------|---------|-----------|------------------|-------------------|
-        |   2x2    |   1     |   N       |   3856.07        |   1057.87         |
-        |   2x2    |   2     |   N       |   2685.80        |   1062.69         |
-        |   2x2    |   1     |   Y       |   N/A            |   129.64          |
-        |   2x2    |   2     |   Y       |   N/A            |   81.62           |
-        |   2x2x2  |   1     |   N       |   4468.55        |   336.85          |
-        |   2x2x2  |   2     |   N       |   2867.80        |   298.45          |
-        |   2x2x2  |   1     |   Y       |   1389.47        |   337.87          |
-        |   2x2x2  |   2     |   Y       |   1259.58        |   293.84          |
-        
-        As the downsampling code's performance is data dependent due to branching, I also used [`connectomics.npy`](https://github.com/seung-lab/connected-components-3d/blob/master/benchmarks/connectomics.npy.gz) (512<sup>3</sup> uint32 extended to uint64) to see how that affected performance. This data comes from mouse visual cortex and has many equal adjacent voxels. In this volume, the 2x2x2 non-sparse mode is much faster as the "instant" majority detection can skip examining half the voxels in many cases.
-        
-        | dwnsmpl  |   mips  |   sparse  |   MODE (MVx/sec)  |
-        |----------|---------|-----------|-------------------|
-        |   2x2    |   1     |   N       |   1078.09         |
-        |   2x2    |   2     |   N       |   1030.90         |
-        |   2x2    |   1     |   Y       |   146.15          |
-        |   2x2    |   2     |   Y       |   69.25           |
-        |   2x2x2  |   1     |   N       |   1966.74         |
-        |   2x2x2  |   2     |   N       |   1790.60         |
-        |   2x2x2  |   1     |   Y       |   2041.96         |
-        |   2x2x2  |   2     |   Y       |   1758.42         |
-        
-        
-        ## Considerations: downsample_segmentation 
-        
-        The `downsample_segmentation` function performs mode pooling operations provided the downsample factor is a power of two, including in three dimensions. If the factor is a non-power of two, striding is used. The mode pooling, which is usually what you want, is computed recursively. Mode pooling is superior to striding, but the recursive calculation can introduce defects at mip levels higher than 1. This may be improved in the future.  
-        
-        The way the calculation is actually done uses an ensemble of several different methods. For (2,2,1,1) and (2,2,2,1) downsamples, a Cython fast, low memory path is selected. (2,2,1,1) implements [*countless if*](https://towardsdatascience.com/countless-high-performance-2x-downsampling-of-labeled-images-using-python-and-numpy-e70ad3275589). (2,2,2,1) uses a combination of counting and "instant" majority detection. For (4,4,1) or other 2D powers of two, the [*countless 2d*](https://towardsdatascience.com/countless-high-performance-2x-downsampling-of-labeled-images-using-python-and-numpy-e70ad3275589) algorithm is used. For (4,4,4), (8,8,8) etc, the [*dynamic countless 3d*](https://towardsdatascience.com/countless-3d-vectorized-2x-downsampling-of-labeled-volume-images-using-python-and-numpy-59d686c2f75) algorithm is used. For 2D powers of two, [*stippled countless 2d*](https://medium.com/@willsilversmith/countless-2d-inflated-2x-downsampling-of-labeled-images-holding-zero-values-as-background-4d13a7675f2d) is used if the sparse flag is enabled. For all other configurations, striding is used.  
-        
-        Countless 2d paths are also fast, but use slightly more memory and time. Countless 3D is okay for (2,2,2) and (4,4,4) but will use time and memory exponential in the product of dimensions. This state of affairs could be improved by implementing a counting based algorithm in Cython/C++ for arbitrary factors that doesn't compute recursively. The countless algorithms were developed before I knew how to write Cython and package libraries. However, C++ implementations of countless are much faster than counting for computing the first 2x2x1 mip level. In particular, an AVX2 SIMD implementation can saturate memory bandwidth.    
-        
-        Documentation for the countless algorithm family is located here: https://github.com/william-silversmith/countless
-        
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+Requires-Dist: numpy
+
+[![Build Status](https://travis-ci.org/seung-lab/tinybrain.svg?branch=master)](https://travis-ci.org/seung-lab/tinybrain) [![PyPI version](https://badge.fury.io/py/tinybrain.svg)](https://badge.fury.io/py/tinybrain)  
+
+# tinybrain
+
+Image pyramid generation specialized for connectomics data types and procedures. If your brain wasn't tiny before, it will be now.  
+
+```python 
+import tinybrain 
+
+img = load_3d_em_stack()
+
+# 2x2 and 2x2x2 downsamples are on a fast path.
+# e.g. (2,2), (2,2,1), (2,2,1,1), (2,2,2), (2,2,2,1)
+img_pyramid = tinybrain.downsample_with_averaging(img, factor=(2,2,1), num_mips=5, sparse=False)
+
+labels = load_3d_labels()
+label_pyramid = tinybrain.downsample_segmentation(labels, factor=(2,2,1), num_mips=5, sparse=False))
+```
+
+## Installation 
+
+```bash
+pip install numpy
+pip install tinybrain
+```
+
+## Motivation
+
+Image hierarchy generation in connectomics uses a few different techniques for
+visualizing data, but predominantly we create image pyramids of uint8 grayscale images using 2x2 average pooling and of uint8 to uint64 segmentation labels using 2x2 mode pooling. When images become very large and people wish to visualze upper mip levels using three axes at once, it becomes desirable to perform 2x2x2 downsamples to maintain isotropy.
+
+It's possible to compute both of these using numpy, however as multiple packages found it useful to copy the downsample functions, it makes sense to formalize these functions into a seperate library located on PyPI.
+
+Given the disparate circumstances that they will be used in, these functions should work 
+fast as possible with low memory usage and avoid numerical issues such as integer truncation
+while generating multiple mip levels.
+
+## Considerations: downsample_with_averaging 
+
+It's advisable to generate multiple mip levels at once rather than recursively computing
+new images as for integer type images, this leads to integer truncation issues. In the common
+case of 2x2x1 downsampling, a recursively computed image would lose 0.75 brightness per a 
+mip level. Therefore, take advantage of the `num_mips` argument which strikes a balance
+that limits integer truncation loss to once every 4 mip levels. This compromise allows
+for the use of integer arithmatic and no more memory usage than 2x the input image including
+the output downsamples. If you seek to eliminate the loss beyond 4 mip levels, try promoting 
+the type before downsampling. 2x2x2x1 downsamples truncate every 8 mip levels.
+
+A C++ high performance path is triggered for 2x2x1x1 and 2x2x2x1 downsample factors on uint8, uint16, float32, 
+and float64 data types in Fortran order. Other factors, data types, and orderings are computed using a numpy pathway that is much slower and more memory intensive.
+
+We also include a sparse mode for downsampling 2x2x2 patches, which prevents "ghosting" where one z-slice overlaps a black region on the next slice and becomes semi-transparent after downsampling. We deal with this by neglecting the background pixels from the averaging operation. 
+
+### Example Benchmark 
+
+On a 1024x1024x100 uint8 image I ran the following code. PIL and OpenCV are actually much faster than this benchmark shows because most of the time is spent writing to the numpy array. tinybrain has a large advantage working on 3D and 4D arrays. Of course, this is a very simple benchmark and it may be possible to tune each of these approaches. On single slices, Pillow was faster than tinybrain.
+
+```python
+img = np.load("image.npy")
+
+s = time.time()
+downsample_with_averaging(img, (2,2,1))
+print("Original ", time.time() - s)
+
+s = time.time()
+out = tinybrain.downsample_with_averaging(img, (2,2,1))
+print("tinybrain ", time.time() - s)
+
+s = time.time()
+out = np.zeros(shape=(512,512,100))
+for z in range(img.shape[2]):
+  out[:,:,z] = cv2.resize(img[:,:,z], dsize=(512, 512) )
+print("OpenCV ", time.time() - s)
+
+s = time.time()
+out = np.zeros(shape=(512,512,100))
+for z in range(img.shape[2]):
+  pilimg = Image.fromarray(img[:,:,z])
+  out[:,:,z] = pilimg.resize( (512, 512) )
+print("Pillow ", time.time() - s)
+
+# Method     Run Time             Rel. Perf.
+# Original   1820 ms +/- 3.73 ms    1.0x
+# tinybrain    67 ms +/- 0.40 ms   27.2x 
+# OpenCV      469 ms +/- 1.12 ms    3.9x
+# Pillow      937 ms +/- 7.63 ms    1.9x
+```
+
+Here's the output from `perf.py` on an Apple Silicon 2021 Macbook Pro M1.
+Note that the image used was a random 2048x2048x64 array that was a uint8
+for average pooling and a uint64 for mode pooling to represent real use cases more fairly. In the table, read it as 2D or 3D downsamples, generating a single or multiple mip levels, with sparse mode enabled or disabled. The speed values are in megavoxels per a second and are the mean of ten runs.
+
+
+| dwnsmpl  |   mips  |   sparse  |   AVG (MVx/sec)  |   MODE (MVx/sec)  |
+|----------|---------|-----------|------------------|-------------------|
+|   2x2    |   1     |   N       |   3856.07        |   1057.87         |
+|   2x2    |   2     |   N       |   2685.80        |   1062.69         |
+|   2x2    |   1     |   Y       |   N/A            |   129.64          |
+|   2x2    |   2     |   Y       |   N/A            |   81.62           |
+|   2x2x2  |   1     |   N       |   4468.55        |   336.85          |
+|   2x2x2  |   2     |   N       |   2867.80        |   298.45          |
+|   2x2x2  |   1     |   Y       |   1389.47        |   337.87          |
+|   2x2x2  |   2     |   Y       |   1259.58        |   293.84          |
+
+As the downsampling code's performance is data dependent due to branching, I also used [`connectomics.npy`](https://github.com/seung-lab/connected-components-3d/blob/master/benchmarks/connectomics.npy.gz) (512<sup>3</sup> uint32 extended to uint64) to see how that affected performance. This data comes from mouse visual cortex and has many equal adjacent voxels. In this volume, the 2x2x2 non-sparse mode is much faster as the "instant" majority detection can skip examining half the voxels in many cases.
+
+| dwnsmpl  |   mips  |   sparse  |   MODE (MVx/sec)  |
+|----------|---------|-----------|-------------------|
+|   2x2    |   1     |   N       |   1078.09         |
+|   2x2    |   2     |   N       |   1030.90         |
+|   2x2    |   1     |   Y       |   146.15          |
+|   2x2    |   2     |   Y       |   69.25           |
+|   2x2x2  |   1     |   N       |   1966.74         |
+|   2x2x2  |   2     |   N       |   1790.60         |
+|   2x2x2  |   1     |   Y       |   2041.96         |
+|   2x2x2  |   2     |   Y       |   1758.42         |
+
+
+## Considerations: downsample_segmentation 
+
+The `downsample_segmentation` function performs mode pooling operations provided the downsample factor is a power of two, including in three dimensions. If the factor is a non-power of two, striding is used. The mode pooling, which is usually what you want, is computed recursively. Mode pooling is superior to striding, but the recursive calculation can introduce defects at mip levels higher than 1. This may be improved in the future.  
+
+The way the calculation is actually done uses an ensemble of several different methods. For (2,2,1,1) and (2,2,2,1) downsamples, a Cython fast, low memory path is selected. (2,2,1,1) implements [*countless if*](https://towardsdatascience.com/countless-high-performance-2x-downsampling-of-labeled-images-using-python-and-numpy-e70ad3275589). (2,2,2,1) uses a combination of counting and "instant" majority detection. For (4,4,1) or other 2D powers of two, the [*countless 2d*](https://towardsdatascience.com/countless-high-performance-2x-downsampling-of-labeled-images-using-python-and-numpy-e70ad3275589) algorithm is used. For (4,4,4), (8,8,8) etc, the [*dynamic countless 3d*](https://towardsdatascience.com/countless-3d-vectorized-2x-downsampling-of-labeled-volume-images-using-python-and-numpy-59d686c2f75) algorithm is used. For 2D powers of two, [*stippled countless 2d*](https://medium.com/@willsilversmith/countless-2d-inflated-2x-downsampling-of-labeled-images-holding-zero-values-as-background-4d13a7675f2d) is used if the sparse flag is enabled. For all other configurations, striding is used.  
+
+Countless 2d paths are also fast, but use slightly more memory and time. Countless 3D is okay for (2,2,2) and (4,4,4) but will use time and memory exponential in the product of dimensions. This state of affairs could be improved by implementing a counting based algorithm in Cython/C++ for arbitrary factors that doesn't compute recursively. The countless algorithms were developed before I knew how to write Cython and package libraries. However, C++ implementations of countless are much faster than counting for computing the first 2x2x1 mip level. In particular, an AVX2 SIMD implementation can saturate memory bandwidth.    
+
+Documentation for the countless algorithm family is located here: https://github.com/william-silversmith/countless
+
```

### Comparing `tinybrain-1.4.1/README.md` & `tinybrain-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tinybrain-1.4.1/automated_test.py` & `tinybrain-1.5.0/automated_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -356,64 +356,64 @@
   data = np.ones(shape=(1024, 62, 511, 1), dtype=int)
   result, = downsamplefn(data, (1,2,2))
   assert result.shape == (1024, 31, 256, 1)
 
   result, = downsamplefn(result, (1,2,2))
   assert result.shape == (1024, 16, 128, 1)
 
-def test_downsample_max_pooling():
-  for dtype in (np.int8, np.float32):
-    cases = [
-      np.array([ [ -1, 0 ], [ 0, 0 ] ], dtype=dtype), 
-      np.array([ [ 0, 0 ], [ 0, 0 ] ], dtype=dtype), 
-      np.array([ [ 0, 1 ], [ 0, 0 ] ], dtype=dtype),
-      np.array([ [ 0, 1 ], [ 1, 0 ] ], dtype=dtype),
-      np.array([ [ 0, 1 ], [ 0, 2 ] ], dtype=dtype)
-    ]
-
-    for i in range(len(cases)):
-      case = cases[i]
-      result, = tinybrain.downsample.downsample_with_max_pooling(case, (1, 1))
-      assert np.all(result == cases[i])
-
-    answers = [ 0, 0, 1, 1, 2 ]
-
-    for i in range(len(cases)):
-      case = cases[i]
-      result, = tinybrain.downsample.downsample_with_max_pooling(case, (2, 2))
-      assert result == answers[i]
-
-
-    cast = lambda arr: np.array(arr, dtype=dtype) 
-
-    answers = list(map(cast, [  
-      [[ 0, 0 ]],
-      [[ 0, 0 ]],
-      [[ 0, 1 ]],
-      [[ 1, 1 ]],
-      [[ 0, 2 ]],
-    ]))
-
-    for i in range(len(cases)):
-      case = cases[i]
-      result, = tinybrain.downsample.downsample_with_max_pooling(case, (2, 1))
-      assert np.all(result == answers[i])
-
-    answers = list(map(cast, [  
-      [[ 0 ], [ 0 ]],
-      [[ 0 ], [ 0 ]],
-      [[ 1 ], [ 0 ]],
-      [[ 1 ], [ 1 ]],
-      [[ 1 ], [ 2 ]],
-    ]))
-
-    for i in range(len(cases)):
-      case = cases[i]
-      result, = tinybrain.downsample.downsample_with_max_pooling(case, (1, 2))
-      assert np.all(result == answers[i])
+@pytest.mark.parametrize("dtype", [np.int8, np.float32])
+def test_downsample_max_pooling(dtype):
+  cases = [
+    np.array([ [ -1, 0 ], [ 0, 0 ] ], dtype=dtype), 
+    np.array([ [ 0, 0 ], [ 0, 0 ] ], dtype=dtype), 
+    np.array([ [ 0, 1 ], [ 0, 0 ] ], dtype=dtype),
+    np.array([ [ 0, 1 ], [ 1, 0 ] ], dtype=dtype),
+    np.array([ [ 0, 1 ], [ 0, 2 ] ], dtype=dtype)
+  ]
+
+  for i in range(len(cases)):
+    case = cases[i]
+    result, = tinybrain.downsample.downsample_with_max_pooling(case, (1, 1))
+    assert np.all(result == cases[i])
+
+  answers = [ 0, 0, 1, 1, 2 ]
+
+  for i in range(len(cases)):
+    case = cases[i]
+    result, = tinybrain.downsample.downsample_with_max_pooling(case, (2, 2))
+    assert result == answers[i]
+
+
+  cast = lambda arr: np.array(arr, dtype=dtype) 
+
+  answers = list(map(cast, [  
+    [[ 0, 0 ]],
+    [[ 0, 0 ]],
+    [[ 0, 1 ]],
+    [[ 1, 1 ]],
+    [[ 0, 2 ]],
+  ]))
+
+  for i in range(len(cases)):
+    case = cases[i]
+    result, = tinybrain.downsample.downsample_with_max_pooling(case, (2, 1))
+    assert np.all(result == answers[i])
+
+  answers = list(map(cast, [  
+    [[ 0 ], [ 0 ]],
+    [[ 0 ], [ 0 ]],
+    [[ 1 ], [ 0 ]],
+    [[ 1 ], [ 1 ]],
+    [[ 1 ], [ 2 ]],
+  ]))
+
+  for i in range(len(cases)):
+    case = cases[i]
+    result, = tinybrain.downsample.downsample_with_max_pooling(case, (1, 2))
+    assert np.all(result == answers[i])
 
   result, = tinybrain.downsample.downsample_with_max_pooling(image4x4x4, (2, 2, 2))
   answer = cast([
     [
       [ [2], [2] ], # y=0    # x = 0
       [ [2], [2] ]  # y=1
     ],
@@ -445,14 +445,65 @@
       [ [4], [4], [4], [4] ], # y = 0     # x = 1
       [ [4], [4], [4], [4] ]  # y = 1
     ]
   ])
 
   assert np.all(result == answer)
 
+@pytest.mark.parametrize("dtype", [np.int8, np.float32])
+def test_downsample_min_pooling(dtype):
+  cases = [
+    np.array([ [ -1, 0 ], [ 0, 0 ] ], dtype=dtype), 
+    np.array([ [ 0, 0 ], [ 0, 0 ] ], dtype=dtype), 
+    np.array([ [ 0, 1 ], [ 0, 0 ] ], dtype=dtype),
+    np.array([ [ 0, 1 ], [ 1, 0 ] ], dtype=dtype),
+    np.array([ [ 0, 1 ], [ 0, 2 ] ], dtype=dtype)
+  ]
+
+  for i in range(len(cases)):
+    case = cases[i]
+    result, = tinybrain.downsample.downsample_with_min_pooling(case, (1, 1))
+    assert np.all(result == cases[i])
+
+  answers = [ -1, 0, 0, 0, 0 ]
+
+  for i in range(len(cases)):
+    case = cases[i]
+    result, = tinybrain.downsample.downsample_with_min_pooling(case, (2, 2))
+    assert result == answers[i]
+
+  cast = lambda arr: np.array(arr, dtype=dtype) 
+
+  answers = list(map(cast, [  
+    [[ -1, 0 ]],
+    [[ 0, 0 ]],
+    [[ 0, 0 ]],
+    [[ 0, 0 ]],
+    [[ 0, 1 ]],
+  ]))
+
+  for i in range(len(cases)):
+    case = cases[i]
+    result, = tinybrain.downsample.downsample_with_min_pooling(case, (2, 1))
+    print(result)
+    assert np.all(result == answers[i])
+
+  answers = list(map(cast, [  
+    [[ -1 ], [ 0 ]],
+    [[ 0 ], [ 0 ]],
+    [[ 0 ], [ 0 ]],
+    [[ 0 ], [ 0 ]],
+    [[ 0 ], [ 0 ]],
+  ]))
+
+  for i in range(len(cases)):
+    case = cases[i]
+    result, = tinybrain.downsample.downsample_with_min_pooling(case, (1, 2))
+    assert np.all(result == answers[i])
+
 def test_countless3d():
   def test_all_cases(fn):
     alldifferent = [
       [
         [1,2],
         [3,4],
       ],
```

### Comparing `tinybrain-1.4.1/build_linux.sh` & `tinybrain-1.5.0/build_linux.sh`

 * *Files identical despite different names*

### Comparing `tinybrain-1.4.1/manylinux1.Dockerfile` & `tinybrain-1.5.0/manylinux1.Dockerfile`

 * *Files identical despite different names*

### Comparing `tinybrain-1.4.1/manylinux2010.Dockerfile` & `tinybrain-1.5.0/manylinux2010.Dockerfile`

 * *Files identical despite different names*

### Comparing `tinybrain-1.4.1/manylinux2014.Dockerfile` & `tinybrain-1.5.0/manylinux2014.Dockerfile`

 * *Files identical despite different names*

### Comparing `tinybrain-1.4.1/perf.py` & `tinybrain-1.5.0/perf.py`

 * *Files identical despite different names*

### Comparing `tinybrain-1.4.1/setup.cfg` & `tinybrain-1.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tinybrain-1.4.1/setup.py` & `tinybrain-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `tinybrain-1.4.1/tinybrain/accelerated.hpp` & `tinybrain-1.5.0/tinybrain/accelerated.hpp`

 * *Files identical despite different names*

### Comparing `tinybrain-1.4.1/tinybrain/accelerated.pyx` & `tinybrain-1.5.0/tinybrain/accelerated.pyx`

 * *Files identical despite different names*

### Comparing `tinybrain-1.4.1/tinybrain/downsample.py` & `tinybrain-1.5.0/tinybrain/downsample.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,19 +150,33 @@
   cuboid specified by factor. That is, a reduction factor
   of 2x2 works by summarizing many 2x2 cuboids. If factor's 
   length is smaller than array.shape, the remaining factors will
   be filled with 1.
   """
   results = []
   for mip in range(num_mips):
-    array = _downsample_with_max_pooling(array, factor)
+    array = _downsample_with(array, factor, fn=np.maximum)
     results.append(array)
   return results
 
-def _downsample_with_max_pooling(array, factor):
+def downsample_with_min_pooling(array, factor, num_mips=1):
+  """
+  Downsample by picking the minimum value within a
+  cuboid specified by factor. That is, a reduction factor
+  of 2x2 works by summarizing many 2x2 cuboids. If factor's 
+  length is smaller than array.shape, the remaining factors will
+  be filled with 1.
+  """
+  results = []
+  for mip in range(num_mips):
+    array = _downsample_with(array, factor, fn=np.minimum)
+    results.append(array)
+  return results
+
+def _downsample_with(array, factor, fn):
   """
   Downsample by picking the maximum value within a
   cuboid specified by factor. That is, a reduction factor
   of 2x2 works by summarizing many 2x2 cuboids. If factor's 
   length is smaller than array.shape, the remaining factors will
   be filled with 1.
   """
@@ -175,15 +189,15 @@
   for offset in np.ndindex(factor):
     part = array[tuple(np.s_[o::f] for o, f in zip(offset, factor))]
     sections.append(part)
 
   output = sections[0].copy()
 
   for section in sections[1:]:
-    np.maximum(output, section, output)
+    fn(output, section, output)
 
   return output
 
 def downsample_segmentation(img, factor, sparse=False, num_mips=1):
   """
   Downsampling machine labels requires choosing an actual
   pixel, not a linear combination (or otherwise) of the
```

### Comparing `tinybrain-1.4.1/tinybrain.egg-info/PKG-INFO` & `tinybrain-1.5.0/tinybrain.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,150 +1,151 @@
 Metadata-Version: 2.1
 Name: tinybrain
-Version: 1.4.1
+Version: 1.5.0
 Summary: Image pyramid generation specialized for connectomics data types and procedures.
 Home-page: https://github.com/seung-lab/tinybrain/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
-License: UNKNOWN
-Description: [![Build Status](https://travis-ci.org/seung-lab/tinybrain.svg?branch=master)](https://travis-ci.org/seung-lab/tinybrain) [![PyPI version](https://badge.fury.io/py/tinybrain.svg)](https://badge.fury.io/py/tinybrain)  
-        
-        # tinybrain
-        
-        Image pyramid generation specialized for connectomics data types and procedures. If your brain wasn't tiny before, it will be now.  
-        
-        ```python 
-        import tinybrain 
-        
-        img = load_3d_em_stack()
-        
-        # 2x2 and 2x2x2 downsamples are on a fast path.
-        # e.g. (2,2), (2,2,1), (2,2,1,1), (2,2,2), (2,2,2,1)
-        img_pyramid = tinybrain.downsample_with_averaging(img, factor=(2,2,1), num_mips=5, sparse=False)
-        
-        labels = load_3d_labels()
-        label_pyramid = tinybrain.downsample_segmentation(labels, factor=(2,2,1), num_mips=5, sparse=False))
-        ```
-        
-        ## Installation 
-        
-        ```bash
-        pip install numpy
-        pip install tinybrain
-        ```
-        
-        ## Motivation
-        
-        Image hierarchy generation in connectomics uses a few different techniques for
-        visualizing data, but predominantly we create image pyramids of uint8 grayscale images using 2x2 average pooling and of uint8 to uint64 segmentation labels using 2x2 mode pooling. When images become very large and people wish to visualze upper mip levels using three axes at once, it becomes desirable to perform 2x2x2 downsamples to maintain isotropy.
-        
-        It's possible to compute both of these using numpy, however as multiple packages found it useful to copy the downsample functions, it makes sense to formalize these functions into a seperate library located on PyPI.
-        
-        Given the disparate circumstances that they will be used in, these functions should work 
-        fast as possible with low memory usage and avoid numerical issues such as integer truncation
-        while generating multiple mip levels.
-        
-        ## Considerations: downsample_with_averaging 
-        
-        It's advisable to generate multiple mip levels at once rather than recursively computing
-        new images as for integer type images, this leads to integer truncation issues. In the common
-        case of 2x2x1 downsampling, a recursively computed image would lose 0.75 brightness per a 
-        mip level. Therefore, take advantage of the `num_mips` argument which strikes a balance
-        that limits integer truncation loss to once every 4 mip levels. This compromise allows
-        for the use of integer arithmatic and no more memory usage than 2x the input image including
-        the output downsamples. If you seek to eliminate the loss beyond 4 mip levels, try promoting 
-        the type before downsampling. 2x2x2x1 downsamples truncate every 8 mip levels.
-        
-        A C++ high performance path is triggered for 2x2x1x1 and 2x2x2x1 downsample factors on uint8, uint16, float32, 
-        and float64 data types in Fortran order. Other factors, data types, and orderings are computed using a numpy pathway that is much slower and more memory intensive.
-        
-        We also include a sparse mode for downsampling 2x2x2 patches, which prevents "ghosting" where one z-slice overlaps a black region on the next slice and becomes semi-transparent after downsampling. We deal with this by neglecting the background pixels from the averaging operation. 
-        
-        ### Example Benchmark 
-        
-        On a 1024x1024x100 uint8 image I ran the following code. PIL and OpenCV are actually much faster than this benchmark shows because most of the time is spent writing to the numpy array. tinybrain has a large advantage working on 3D and 4D arrays. Of course, this is a very simple benchmark and it may be possible to tune each of these approaches. On single slices, Pillow was faster than tinybrain.
-        
-        ```python
-        img = np.load("image.npy")
-        
-        s = time.time()
-        downsample_with_averaging(img, (2,2,1))
-        print("Original ", time.time() - s)
-        
-        s = time.time()
-        out = tinybrain.downsample_with_averaging(img, (2,2,1))
-        print("tinybrain ", time.time() - s)
-        
-        s = time.time()
-        out = np.zeros(shape=(512,512,100))
-        for z in range(img.shape[2]):
-          out[:,:,z] = cv2.resize(img[:,:,z], dsize=(512, 512) )
-        print("OpenCV ", time.time() - s)
-        
-        s = time.time()
-        out = np.zeros(shape=(512,512,100))
-        for z in range(img.shape[2]):
-          pilimg = Image.fromarray(img[:,:,z])
-          out[:,:,z] = pilimg.resize( (512, 512) )
-        print("Pillow ", time.time() - s)
-        
-        # Method     Run Time             Rel. Perf.
-        # Original   1820 ms +/- 3.73 ms    1.0x
-        # tinybrain    67 ms +/- 0.40 ms   27.2x 
-        # OpenCV      469 ms +/- 1.12 ms    3.9x
-        # Pillow      937 ms +/- 7.63 ms    1.9x
-        ```
-        
-        Here's the output from `perf.py` on an Apple Silicon 2021 Macbook Pro M1.
-        Note that the image used was a random 2048x2048x64 array that was a uint8
-        for average pooling and a uint64 for mode pooling to represent real use cases more fairly. In the table, read it as 2D or 3D downsamples, generating a single or multiple mip levels, with sparse mode enabled or disabled. The speed values are in megavoxels per a second and are the mean of ten runs.
-        
-        
-        | dwnsmpl  |   mips  |   sparse  |   AVG (MVx/sec)  |   MODE (MVx/sec)  |
-        |----------|---------|-----------|------------------|-------------------|
-        |   2x2    |   1     |   N       |   3856.07        |   1057.87         |
-        |   2x2    |   2     |   N       |   2685.80        |   1062.69         |
-        |   2x2    |   1     |   Y       |   N/A            |   129.64          |
-        |   2x2    |   2     |   Y       |   N/A            |   81.62           |
-        |   2x2x2  |   1     |   N       |   4468.55        |   336.85          |
-        |   2x2x2  |   2     |   N       |   2867.80        |   298.45          |
-        |   2x2x2  |   1     |   Y       |   1389.47        |   337.87          |
-        |   2x2x2  |   2     |   Y       |   1259.58        |   293.84          |
-        
-        As the downsampling code's performance is data dependent due to branching, I also used [`connectomics.npy`](https://github.com/seung-lab/connected-components-3d/blob/master/benchmarks/connectomics.npy.gz) (512<sup>3</sup> uint32 extended to uint64) to see how that affected performance. This data comes from mouse visual cortex and has many equal adjacent voxels. In this volume, the 2x2x2 non-sparse mode is much faster as the "instant" majority detection can skip examining half the voxels in many cases.
-        
-        | dwnsmpl  |   mips  |   sparse  |   MODE (MVx/sec)  |
-        |----------|---------|-----------|-------------------|
-        |   2x2    |   1     |   N       |   1078.09         |
-        |   2x2    |   2     |   N       |   1030.90         |
-        |   2x2    |   1     |   Y       |   146.15          |
-        |   2x2    |   2     |   Y       |   69.25           |
-        |   2x2x2  |   1     |   N       |   1966.74         |
-        |   2x2x2  |   2     |   N       |   1790.60         |
-        |   2x2x2  |   1     |   Y       |   2041.96         |
-        |   2x2x2  |   2     |   Y       |   1758.42         |
-        
-        
-        ## Considerations: downsample_segmentation 
-        
-        The `downsample_segmentation` function performs mode pooling operations provided the downsample factor is a power of two, including in three dimensions. If the factor is a non-power of two, striding is used. The mode pooling, which is usually what you want, is computed recursively. Mode pooling is superior to striding, but the recursive calculation can introduce defects at mip levels higher than 1. This may be improved in the future.  
-        
-        The way the calculation is actually done uses an ensemble of several different methods. For (2,2,1,1) and (2,2,2,1) downsamples, a Cython fast, low memory path is selected. (2,2,1,1) implements [*countless if*](https://towardsdatascience.com/countless-high-performance-2x-downsampling-of-labeled-images-using-python-and-numpy-e70ad3275589). (2,2,2,1) uses a combination of counting and "instant" majority detection. For (4,4,1) or other 2D powers of two, the [*countless 2d*](https://towardsdatascience.com/countless-high-performance-2x-downsampling-of-labeled-images-using-python-and-numpy-e70ad3275589) algorithm is used. For (4,4,4), (8,8,8) etc, the [*dynamic countless 3d*](https://towardsdatascience.com/countless-3d-vectorized-2x-downsampling-of-labeled-volume-images-using-python-and-numpy-59d686c2f75) algorithm is used. For 2D powers of two, [*stippled countless 2d*](https://medium.com/@willsilversmith/countless-2d-inflated-2x-downsampling-of-labeled-images-holding-zero-values-as-background-4d13a7675f2d) is used if the sparse flag is enabled. For all other configurations, striding is used.  
-        
-        Countless 2d paths are also fast, but use slightly more memory and time. Countless 3D is okay for (2,2,2) and (4,4,4) but will use time and memory exponential in the product of dimensions. This state of affairs could be improved by implementing a counting based algorithm in Cython/C++ for arbitrary factors that doesn't compute recursively. The countless algorithms were developed before I knew how to write Cython and package libraries. However, C++ implementations of countless are much faster than counting for computing the first 2x2x1 mip level. In particular, an AVX2 SIMD implementation can saturate memory bandwidth.    
-        
-        Documentation for the countless algorithm family is located here: https://github.com/william-silversmith/countless
-        
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+Requires-Dist: numpy
+
+[![Build Status](https://travis-ci.org/seung-lab/tinybrain.svg?branch=master)](https://travis-ci.org/seung-lab/tinybrain) [![PyPI version](https://badge.fury.io/py/tinybrain.svg)](https://badge.fury.io/py/tinybrain)  
+
+# tinybrain
+
+Image pyramid generation specialized for connectomics data types and procedures. If your brain wasn't tiny before, it will be now.  
+
+```python 
+import tinybrain 
+
+img = load_3d_em_stack()
+
+# 2x2 and 2x2x2 downsamples are on a fast path.
+# e.g. (2,2), (2,2,1), (2,2,1,1), (2,2,2), (2,2,2,1)
+img_pyramid = tinybrain.downsample_with_averaging(img, factor=(2,2,1), num_mips=5, sparse=False)
+
+labels = load_3d_labels()
+label_pyramid = tinybrain.downsample_segmentation(labels, factor=(2,2,1), num_mips=5, sparse=False))
+```
+
+## Installation 
+
+```bash
+pip install numpy
+pip install tinybrain
+```
+
+## Motivation
+
+Image hierarchy generation in connectomics uses a few different techniques for
+visualizing data, but predominantly we create image pyramids of uint8 grayscale images using 2x2 average pooling and of uint8 to uint64 segmentation labels using 2x2 mode pooling. When images become very large and people wish to visualze upper mip levels using three axes at once, it becomes desirable to perform 2x2x2 downsamples to maintain isotropy.
+
+It's possible to compute both of these using numpy, however as multiple packages found it useful to copy the downsample functions, it makes sense to formalize these functions into a seperate library located on PyPI.
+
+Given the disparate circumstances that they will be used in, these functions should work 
+fast as possible with low memory usage and avoid numerical issues such as integer truncation
+while generating multiple mip levels.
+
+## Considerations: downsample_with_averaging 
+
+It's advisable to generate multiple mip levels at once rather than recursively computing
+new images as for integer type images, this leads to integer truncation issues. In the common
+case of 2x2x1 downsampling, a recursively computed image would lose 0.75 brightness per a 
+mip level. Therefore, take advantage of the `num_mips` argument which strikes a balance
+that limits integer truncation loss to once every 4 mip levels. This compromise allows
+for the use of integer arithmatic and no more memory usage than 2x the input image including
+the output downsamples. If you seek to eliminate the loss beyond 4 mip levels, try promoting 
+the type before downsampling. 2x2x2x1 downsamples truncate every 8 mip levels.
+
+A C++ high performance path is triggered for 2x2x1x1 and 2x2x2x1 downsample factors on uint8, uint16, float32, 
+and float64 data types in Fortran order. Other factors, data types, and orderings are computed using a numpy pathway that is much slower and more memory intensive.
+
+We also include a sparse mode for downsampling 2x2x2 patches, which prevents "ghosting" where one z-slice overlaps a black region on the next slice and becomes semi-transparent after downsampling. We deal with this by neglecting the background pixels from the averaging operation. 
+
+### Example Benchmark 
+
+On a 1024x1024x100 uint8 image I ran the following code. PIL and OpenCV are actually much faster than this benchmark shows because most of the time is spent writing to the numpy array. tinybrain has a large advantage working on 3D and 4D arrays. Of course, this is a very simple benchmark and it may be possible to tune each of these approaches. On single slices, Pillow was faster than tinybrain.
+
+```python
+img = np.load("image.npy")
+
+s = time.time()
+downsample_with_averaging(img, (2,2,1))
+print("Original ", time.time() - s)
+
+s = time.time()
+out = tinybrain.downsample_with_averaging(img, (2,2,1))
+print("tinybrain ", time.time() - s)
+
+s = time.time()
+out = np.zeros(shape=(512,512,100))
+for z in range(img.shape[2]):
+  out[:,:,z] = cv2.resize(img[:,:,z], dsize=(512, 512) )
+print("OpenCV ", time.time() - s)
+
+s = time.time()
+out = np.zeros(shape=(512,512,100))
+for z in range(img.shape[2]):
+  pilimg = Image.fromarray(img[:,:,z])
+  out[:,:,z] = pilimg.resize( (512, 512) )
+print("Pillow ", time.time() - s)
+
+# Method     Run Time             Rel. Perf.
+# Original   1820 ms +/- 3.73 ms    1.0x
+# tinybrain    67 ms +/- 0.40 ms   27.2x 
+# OpenCV      469 ms +/- 1.12 ms    3.9x
+# Pillow      937 ms +/- 7.63 ms    1.9x
+```
+
+Here's the output from `perf.py` on an Apple Silicon 2021 Macbook Pro M1.
+Note that the image used was a random 2048x2048x64 array that was a uint8
+for average pooling and a uint64 for mode pooling to represent real use cases more fairly. In the table, read it as 2D or 3D downsamples, generating a single or multiple mip levels, with sparse mode enabled or disabled. The speed values are in megavoxels per a second and are the mean of ten runs.
+
+
+| dwnsmpl  |   mips  |   sparse  |   AVG (MVx/sec)  |   MODE (MVx/sec)  |
+|----------|---------|-----------|------------------|-------------------|
+|   2x2    |   1     |   N       |   3856.07        |   1057.87         |
+|   2x2    |   2     |   N       |   2685.80        |   1062.69         |
+|   2x2    |   1     |   Y       |   N/A            |   129.64          |
+|   2x2    |   2     |   Y       |   N/A            |   81.62           |
+|   2x2x2  |   1     |   N       |   4468.55        |   336.85          |
+|   2x2x2  |   2     |   N       |   2867.80        |   298.45          |
+|   2x2x2  |   1     |   Y       |   1389.47        |   337.87          |
+|   2x2x2  |   2     |   Y       |   1259.58        |   293.84          |
+
+As the downsampling code's performance is data dependent due to branching, I also used [`connectomics.npy`](https://github.com/seung-lab/connected-components-3d/blob/master/benchmarks/connectomics.npy.gz) (512<sup>3</sup> uint32 extended to uint64) to see how that affected performance. This data comes from mouse visual cortex and has many equal adjacent voxels. In this volume, the 2x2x2 non-sparse mode is much faster as the "instant" majority detection can skip examining half the voxels in many cases.
+
+| dwnsmpl  |   mips  |   sparse  |   MODE (MVx/sec)  |
+|----------|---------|-----------|-------------------|
+|   2x2    |   1     |   N       |   1078.09         |
+|   2x2    |   2     |   N       |   1030.90         |
+|   2x2    |   1     |   Y       |   146.15          |
+|   2x2    |   2     |   Y       |   69.25           |
+|   2x2x2  |   1     |   N       |   1966.74         |
+|   2x2x2  |   2     |   N       |   1790.60         |
+|   2x2x2  |   1     |   Y       |   2041.96         |
+|   2x2x2  |   2     |   Y       |   1758.42         |
+
+
+## Considerations: downsample_segmentation 
+
+The `downsample_segmentation` function performs mode pooling operations provided the downsample factor is a power of two, including in three dimensions. If the factor is a non-power of two, striding is used. The mode pooling, which is usually what you want, is computed recursively. Mode pooling is superior to striding, but the recursive calculation can introduce defects at mip levels higher than 1. This may be improved in the future.  
+
+The way the calculation is actually done uses an ensemble of several different methods. For (2,2,1,1) and (2,2,2,1) downsamples, a Cython fast, low memory path is selected. (2,2,1,1) implements [*countless if*](https://towardsdatascience.com/countless-high-performance-2x-downsampling-of-labeled-images-using-python-and-numpy-e70ad3275589). (2,2,2,1) uses a combination of counting and "instant" majority detection. For (4,4,1) or other 2D powers of two, the [*countless 2d*](https://towardsdatascience.com/countless-high-performance-2x-downsampling-of-labeled-images-using-python-and-numpy-e70ad3275589) algorithm is used. For (4,4,4), (8,8,8) etc, the [*dynamic countless 3d*](https://towardsdatascience.com/countless-3d-vectorized-2x-downsampling-of-labeled-volume-images-using-python-and-numpy-59d686c2f75) algorithm is used. For 2D powers of two, [*stippled countless 2d*](https://medium.com/@willsilversmith/countless-2d-inflated-2x-downsampling-of-labeled-images-holding-zero-values-as-background-4d13a7675f2d) is used if the sparse flag is enabled. For all other configurations, striding is used.  
+
+Countless 2d paths are also fast, but use slightly more memory and time. Countless 3D is okay for (2,2,2) and (4,4,4) but will use time and memory exponential in the product of dimensions. This state of affairs could be improved by implementing a counting based algorithm in Cython/C++ for arbitrary factors that doesn't compute recursively. The countless algorithms were developed before I knew how to write Cython and package libraries. However, C++ implementations of countless are much faster than counting for computing the first 2x2x1 mip level. In particular, an AVX2 SIMD implementation can saturate memory bandwidth.    
+
+Documentation for the countless algorithm family is located here: https://github.com/william-silversmith/countless
+
```

### Comparing `tinybrain-1.4.1/tinybrain.egg-info/SOURCES.txt` & `tinybrain-1.5.0/tinybrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

