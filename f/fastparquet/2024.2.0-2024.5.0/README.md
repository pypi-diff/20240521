# Comparing `tmp/fastparquet-2024.2.0.tar.gz` & `tmp/fastparquet-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastparquet-2024.2.0.tar", last modified: Mon Feb 12 17:54:31 2024, max compression
+gzip compressed data, was "fastparquet-2024.5.0.tar", last modified: Tue May 21 16:50:49 2024, max compression
```

## Comparing `fastparquet-2024.2.0.tar` & `fastparquet-2024.5.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-12 17:54:31.295927 fastparquet-2024.2.0/
--rw-r--r--   0 mdurant    (502) staff       (20)      258 2022-09-26 14:54:53.000000 fastparquet-2024.2.0/.coveragerc
--rw-r--r--   0 mdurant    (502) staff       (20)       37 2022-11-14 22:02:19.000000 fastparquet-2024.2.0/.gitattributes
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-12 17:54:31.278538 fastparquet-2024.2.0/.github/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-12 17:54:31.282672 fastparquet-2024.2.0/.github/workflows/
--rw-r--r--   0 mdurant    (502) staff       (20)     4050 2023-12-11 16:36:36.000000 fastparquet-2024.2.0/.github/workflows/main.yaml
--rw-r--r--   0 mdurant    (502) staff       (20)     2415 2024-02-07 18:38:55.000000 fastparquet-2024.2.0/.github/workflows/test_wheel.yaml
--rw-r--r--   0 mdurant    (502) staff       (20)     6874 2024-02-07 18:38:55.000000 fastparquet-2024.2.0/.github/workflows/wheel.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      168 2022-11-18 01:33:09.000000 fastparquet-2024.2.0/.gitignore
--rw-r--r--   0 mdurant    (502) staff       (20)    12406 2022-09-26 14:54:53.000000 fastparquet-2024.2.0/.pylintrc
--rw-r--r--   0 mdurant    (502) staff       (20)      631 2023-08-17 20:51:27.000000 fastparquet-2024.2.0/.readthedocs.yaml
--rw-r--r--   0 mdurant    (502) staff       (20)    10173 2022-09-26 14:54:53.000000 fastparquet-2024.2.0/LICENSE
--rw-r--r--   0 mdurant    (502) staff       (20)      253 2022-09-26 14:54:53.000000 fastparquet-2024.2.0/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)      109 2022-09-26 14:54:53.000000 fastparquet-2024.2.0/Makefile
--rw-r--r--   0 mdurant    (502) staff       (20)     4086 2024-02-12 17:54:31.295817 fastparquet-2024.2.0/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     3087 2022-09-26 14:54:53.000000 fastparquet-2024.2.0/README.rst
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-12 17:54:31.284021 fastparquet-2024.2.0/ci/
--rw-r--r--   0 mdurant    (502) staff       (20)      291 2023-07-01 01:52:53.000000 fastparquet-2024.2.0/ci/environment-py310.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      243 2023-10-25 15:16:22.000000 fastparquet-2024.2.0/ci/environment-py310win.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      259 2023-10-25 15:16:22.000000 fastparquet-2024.2.0/ci/environment-py311.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      259 2023-10-25 15:16:22.000000 fastparquet-2024.2.0/ci/environment-py312.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      258 2023-07-01 01:52:53.000000 fastparquet-2024.2.0/ci/environment-py39.yml
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-12 17:54:31.290283 fastparquet-2024.2.0/fastparquet/
--rwxr-xr-x   0 mdurant    (502) staff       (20)      294 2024-02-07 18:38:55.000000 fastparquet-2024.2.0/fastparquet/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      417 2024-02-12 17:54:29.000000 fastparquet-2024.2.0/fastparquet/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)    63524 2024-02-07 18:38:55.000000 fastparquet-2024.2.0/fastparquet/api.py
--rw-r--r--   0 mdurant    (502) staff       (20)  1929247 2024-02-12 17:54:28.000000 fastparquet-2024.2.0/fastparquet/cencoding.c
--rw-r--r--   0 mdurant    (502) staff       (20)    37355 2023-12-22 19:32:01.000000 fastparquet-2024.2.0/fastparquet/cencoding.pyx
--rw-r--r--   0 mdurant    (502) staff       (20)     3691 2024-02-07 18:38:55.000000 fastparquet-2024.2.0/fastparquet/compression.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9742 2024-02-07 18:38:55.000000 fastparquet-2024.2.0/fastparquet/converted_types.py
--rw-r--r--   0 mdurant    (502) staff       (20)    29904 2024-02-07 18:38:55.000000 fastparquet-2024.2.0/fastparquet/core.py
--rw-r--r--   0 mdurant    (502) staff       (20)    11010 2024-02-07 18:38:55.000000 fastparquet-2024.2.0/fastparquet/dataframe.py
--rwxr-xr-x   0 mdurant    (502) staff       (20)     1572 2024-02-07 18:38:55.000000 fastparquet-2024.2.0/fastparquet/encoding.py
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2024-02-07 18:38:55.000000 fastparquet-2024.2.0/fastparquet/evolve.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3731 2022-09-26 14:54:53.000000 fastparquet-2024.2.0/fastparquet/json.py
--rw-r--r--   0 mdurant    (502) staff       (20)    34890 2022-09-26 14:54:53.000000 fastparquet-2024.2.0/fastparquet/parquet.thrift
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-12 17:54:31.294392 fastparquet-2024.2.0/fastparquet/parquet_thrift/
--rw-r--r--   0 mdurant    (502) staff       (20)      340 2024-02-07 18:38:55.000000 fastparquet-2024.2.0/fastparquet/parquet_thrift/__init__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-12 17:54:31.294852 fastparquet-2024.2.0/fastparquet/parquet_thrift/parquet/
--rw-r--r--   0 mdurant    (502) staff       (20)       34 2022-09-26 14:54:53.000000 fastparquet-2024.2.0/fastparquet/parquet_thrift/parquet/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5681 2022-09-26 14:54:53.000000 fastparquet-2024.2.0/fastparquet/parquet_thrift/parquet/ttypes.py
--rwxr-xr-x   0 mdurant    (502) staff       (20)     7073 2024-02-07 18:38:55.000000 fastparquet-2024.2.0/fastparquet/schema.py
--rw-r--r--   0 mdurant    (502) staff       (20)  1162541 2024-02-12 17:54:29.000000 fastparquet-2024.2.0/fastparquet/speedups.c
--rw-r--r--   0 mdurant    (502) staff       (20)     3287 2022-09-26 14:54:53.000000 fastparquet-2024.2.0/fastparquet/speedups.pyx
--rw-r--r--   0 mdurant    (502) staff       (20)      133 2024-02-07 18:38:55.000000 fastparquet-2024.2.0/fastparquet/thrift_structures.py
--rw-r--r--   0 mdurant    (502) staff       (20)    17380 2024-02-07 18:38:55.000000 fastparquet-2024.2.0/fastparquet/util.py
--rw-r--r--   0 mdurant    (502) staff       (20)    70583 2024-02-07 18:38:55.000000 fastparquet-2024.2.0/fastparquet/writer.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-12 17:54:31.295186 fastparquet-2024.2.0/fastparquet.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     4086 2024-02-12 17:54:29.000000 fastparquet-2024.2.0/fastparquet.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     1136 2024-02-12 17:54:31.000000 fastparquet-2024.2.0/fastparquet.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2024-02-12 17:54:29.000000 fastparquet-2024.2.0/fastparquet.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)       76 2024-02-12 17:54:29.000000 fastparquet-2024.2.0/fastparquet.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)       12 2024-02-12 17:54:29.000000 fastparquet-2024.2.0/fastparquet.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      114 2023-12-11 16:36:27.000000 fastparquet-2024.2.0/pyproject.toml
--rw-r--r--   0 mdurant    (502) staff       (20)       58 2022-10-31 17:25:30.000000 fastparquet-2024.2.0/requirements.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      236 2024-02-12 17:54:31.296289 fastparquet-2024.2.0/setup.cfg
--rw-r--r--   0 mdurant    (502) staff       (20)     3288 2022-11-18 01:33:09.000000 fastparquet-2024.2.0/setup.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-21 16:50:49.310073 fastparquet-2024.5.0/
+-rw-r--r--   0 mdurant    (502) staff       (20)      258 2022-09-26 14:54:53.000000 fastparquet-2024.5.0/.coveragerc
+-rw-r--r--   0 mdurant    (502) staff       (20)       37 2022-11-14 22:02:19.000000 fastparquet-2024.5.0/.gitattributes
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-21 16:50:49.292705 fastparquet-2024.5.0/.github/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-21 16:50:49.297555 fastparquet-2024.5.0/.github/workflows/
+-rw-r--r--   0 mdurant    (502) staff       (20)     3322 2024-05-21 13:27:18.000000 fastparquet-2024.5.0/.github/workflows/main.yaml
+-rw-r--r--   0 mdurant    (502) staff       (20)     2415 2024-02-07 18:38:55.000000 fastparquet-2024.5.0/.github/workflows/test_wheel.yaml
+-rw-r--r--   0 mdurant    (502) staff       (20)     6829 2024-05-21 14:45:38.000000 fastparquet-2024.5.0/.github/workflows/wheel.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      168 2022-11-18 01:33:09.000000 fastparquet-2024.5.0/.gitignore
+-rw-r--r--   0 mdurant    (502) staff       (20)    12406 2022-09-26 14:54:53.000000 fastparquet-2024.5.0/.pylintrc
+-rw-r--r--   0 mdurant    (502) staff       (20)      631 2023-08-17 20:51:27.000000 fastparquet-2024.5.0/.readthedocs.yaml
+-rw-r--r--   0 mdurant    (502) staff       (20)    10173 2022-09-26 14:54:53.000000 fastparquet-2024.5.0/LICENSE
+-rw-r--r--   0 mdurant    (502) staff       (20)      253 2024-05-21 13:27:18.000000 fastparquet-2024.5.0/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)      109 2022-09-26 14:54:53.000000 fastparquet-2024.5.0/Makefile
+-rw-r--r--   0 mdurant    (502) staff       (20)     4130 2024-05-21 16:50:49.309969 fastparquet-2024.5.0/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     3087 2022-09-26 14:54:53.000000 fastparquet-2024.5.0/README.rst
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-21 16:50:49.299001 fastparquet-2024.5.0/ci/
+-rw-r--r--   0 mdurant    (502) staff       (20)      291 2023-07-01 01:52:53.000000 fastparquet-2024.5.0/ci/environment-py310.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      243 2023-10-25 15:16:22.000000 fastparquet-2024.5.0/ci/environment-py310win.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      259 2023-10-25 15:16:22.000000 fastparquet-2024.5.0/ci/environment-py311.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      259 2023-10-25 15:16:22.000000 fastparquet-2024.5.0/ci/environment-py312.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      258 2023-07-01 01:52:53.000000 fastparquet-2024.5.0/ci/environment-py39.yml
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-21 16:50:49.306871 fastparquet-2024.5.0/fastparquet/
+-rwxr-xr-x   0 mdurant    (502) staff       (20)      294 2024-02-07 18:38:55.000000 fastparquet-2024.5.0/fastparquet/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      417 2024-05-21 16:50:47.000000 fastparquet-2024.5.0/fastparquet/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    63524 2024-05-21 13:27:18.000000 fastparquet-2024.5.0/fastparquet/api.py
+-rw-r--r--   0 mdurant    (502) staff       (20)  1929847 2024-05-21 16:50:46.000000 fastparquet-2024.5.0/fastparquet/cencoding.c
+-rw-r--r--   0 mdurant    (502) staff       (20)    37355 2024-05-21 13:27:18.000000 fastparquet-2024.5.0/fastparquet/cencoding.pyx
+-rw-r--r--   0 mdurant    (502) staff       (20)     3691 2024-02-07 18:38:55.000000 fastparquet-2024.5.0/fastparquet/compression.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9855 2024-05-21 13:27:18.000000 fastparquet-2024.5.0/fastparquet/converted_types.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    29904 2024-05-21 13:27:18.000000 fastparquet-2024.5.0/fastparquet/core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10999 2024-05-21 13:27:18.000000 fastparquet-2024.5.0/fastparquet/dataframe.py
+-rwxr-xr-x   0 mdurant    (502) staff       (20)     1572 2024-05-21 13:27:18.000000 fastparquet-2024.5.0/fastparquet/encoding.py
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2024-02-07 18:38:55.000000 fastparquet-2024.5.0/fastparquet/evolve.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3731 2024-05-21 13:27:18.000000 fastparquet-2024.5.0/fastparquet/json.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    34890 2022-09-26 14:54:53.000000 fastparquet-2024.5.0/fastparquet/parquet.thrift
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-21 16:50:49.308403 fastparquet-2024.5.0/fastparquet/parquet_thrift/
+-rw-r--r--   0 mdurant    (502) staff       (20)      340 2024-02-07 18:38:55.000000 fastparquet-2024.5.0/fastparquet/parquet_thrift/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-21 16:50:49.308972 fastparquet-2024.5.0/fastparquet/parquet_thrift/parquet/
+-rw-r--r--   0 mdurant    (502) staff       (20)       34 2022-09-26 14:54:53.000000 fastparquet-2024.5.0/fastparquet/parquet_thrift/parquet/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5681 2022-09-26 14:54:53.000000 fastparquet-2024.5.0/fastparquet/parquet_thrift/parquet/ttypes.py
+-rwxr-xr-x   0 mdurant    (502) staff       (20)     7073 2024-05-21 13:27:18.000000 fastparquet-2024.5.0/fastparquet/schema.py
+-rw-r--r--   0 mdurant    (502) staff       (20)  1189192 2024-05-21 16:50:47.000000 fastparquet-2024.5.0/fastparquet/speedups.c
+-rw-r--r--   0 mdurant    (502) staff       (20)     3287 2024-05-21 13:27:18.000000 fastparquet-2024.5.0/fastparquet/speedups.pyx
+-rw-r--r--   0 mdurant    (502) staff       (20)      133 2024-02-07 18:38:55.000000 fastparquet-2024.5.0/fastparquet/thrift_structures.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    17606 2024-05-21 13:27:18.000000 fastparquet-2024.5.0/fastparquet/util.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    70583 2024-05-21 13:27:18.000000 fastparquet-2024.5.0/fastparquet/writer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-21 16:50:49.309357 fastparquet-2024.5.0/fastparquet.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     4130 2024-05-21 16:50:47.000000 fastparquet-2024.5.0/fastparquet.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     1136 2024-05-21 16:50:49.000000 fastparquet-2024.5.0/fastparquet.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2024-05-21 16:50:47.000000 fastparquet-2024.5.0/fastparquet.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)       68 2024-05-21 16:50:47.000000 fastparquet-2024.5.0/fastparquet.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)       12 2024-05-21 16:50:47.000000 fastparquet-2024.5.0/fastparquet.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)       99 2024-05-21 13:27:18.000000 fastparquet-2024.5.0/pyproject.toml
+-rw-r--r--   0 mdurant    (502) staff       (20)       50 2024-05-21 13:27:18.000000 fastparquet-2024.5.0/requirements.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      236 2024-05-21 16:50:49.310429 fastparquet-2024.5.0/setup.cfg
+-rw-r--r--   0 mdurant    (502) staff       (20)     3176 2024-05-21 13:53:44.000000 fastparquet-2024.5.0/setup.py
```

### Comparing `fastparquet-2024.2.0/.github/workflows/main.yaml` & `fastparquet-2024.5.0/.github/workflows/main.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -66,44 +66,14 @@
       - name: Run Tests
         shell: bash -l {0}
         env:
           FASTPARQUET_DATAPAGE_V2: TRUE
         run: |
           echo "FASTPARQUET_DATAPAGE_V2=$FASTPARQUET_DATAPAGE_V2"
           pytest --verbose --cov=fastparquet
-  dask:
-    name: dask
-    runs-on: ubuntu-latest
-    steps:
-      - name: APT
-        run: sudo apt-get install liblzo2-dev
-
-      - name: Checkout
-        uses: actions/checkout@v4
-        with:
-          fetch-depth: 0
-
-      - name: Setup conda
-        uses: mamba-org/provision-with-micromamba@main
-        with:
-          environment-file: ci/environment-py39.yml
-
-      - name: pip-install
-        shell: bash -l {0}
-        run: |
-          git clone https://github.com/dask/dask
-          pip install pyarrow
-          pip install -e dask/
-          pip install -e . --no-deps
-
-      - name: Run Tests
-        shell: bash -l {0}
-        run: |
-          pytest --verbose dask/dask/dataframe/io/tests/test_parquet.py
-  
   pandas:
     name: pandas
     runs-on: ubuntu-latest
     steps:
       - name: APT
         run: sudo apt-get install liblzo2-dev
```

### Comparing `fastparquet-2024.2.0/.github/workflows/test_wheel.yaml` & `fastparquet-2024.5.0/.github/workflows/test_wheel.yaml`

 * *Files identical despite different names*

### Comparing `fastparquet-2024.2.0/.github/workflows/wheel.yml` & `fastparquet-2024.5.0/.github/workflows/wheel.yml`

 * *Files 6% similar despite different names*

```diff
@@ -12,21 +12,19 @@
       matrix:
         os: [ubuntu-22.04]
         architecture: ['x64']
         include:
           # https://cibuildwheel.readthedocs.io/en/stable/options/#build-skip
           - os: ubuntu-22.04
             linux_archs: "aarch64"
-            skip: "pp* *-musllinux_aarch64"
-
     name: ${{ matrix.os }} ${{ matrix.architecture }} ${{ matrix.linux_archs }}
     env:
       CIBW_REPAIR_WHEEL_COMMAND_WINDOWS: "delvewheel repair -w {dest_dir} {wheel}"
       CIBW_BEFORE_ALL: "pip install numpy cython"
-      CIBW_SKIP: ${{ matrix.skip }}
+      CIBW_SKIP: "pp* *37* *38* *-musllinux_aarch64"
       CIBW_ARCHS_LINUX: ${{ matrix.linux_archs }}
       CIBW_TEST_SKIP: "*"
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
@@ -48,15 +46,15 @@
 
       - name: delvewheel install
         if: runner.os == 'Windows'
         run: |
           python -m pip install delvewheel cython
 
       - name: Build wheels
-        uses: joerick/cibuildwheel@v2.16.5
+        uses: joerick/cibuildwheel@v2.18.1
 
       - uses: actions/upload-artifact@v3
         with:
           path: ./wheelhouse/*.whl
           name: wheels
 
   buildLinx686:
@@ -67,20 +65,20 @@
       matrix:
         os: [ubuntu-22.04]
         architecture: ['x64']
         include:
           # https://cibuildwheel.readthedocs.io/en/stable/options/#build-skip
           - os: ubuntu-22.04
             linux_archs: "i686"
-            skip: "pp* *312*"
+            skip: "pp*"
 
     name: ${{ matrix.os }} ${{ matrix.architecture }} ${{ matrix.linux_archs }}
     env:
       CIBW_REPAIR_WHEEL_COMMAND_WINDOWS: "delvewheel repair -w {dest_dir} {wheel}"
-      CIBW_BEFORE_ALL: "pip install numpy cython"
+      CIBW_BEFORE_ALL: "pip install cython"
       CIBW_SKIP: ${{ matrix.skip }}
       CIBW_ARCHS_LINUX: ${{ matrix.linux_archs }}
       CIBW_TEST_SKIP: "*"
 
     steps:
       - uses: actions/checkout@v4
         with:
@@ -103,15 +101,15 @@
 
       - name: delvewheel install
         if: runner.os == 'Windows'
         run: |
           python -m pip install delvewheel cython
 
       - name: Build wheels
-        uses: joerick/cibuildwheel@v2.16.5
+        uses: joerick/cibuildwheel@v2.18.1
 
       - uses: actions/upload-artifact@v3
         with:
           path: ./wheelhouse/*.whl
           name: wheels
 
   buildLinx86x64:
@@ -127,15 +125,15 @@
           - os: ubuntu-22.04
             linux_archs: "x86_64"
             skip: "pp*"
 
     name: ${{ matrix.os }} ${{ matrix.architecture}}
     env:
       CIBW_REPAIR_WHEEL_COMMAND_WINDOWS: "delvewheel repair -w {dest_dir} {wheel}"
-      CIBW_BEFORE_ALL: "pip install numpy cython"
+      CIBW_BEFORE_ALL: "pip install cython"
       CIBW_SKIP: ${{ matrix.skip }}
       CIBW_ARCHS_LINUX: ${{ matrix.linux_archs }}
       CIBW_TEST_SKIP: "*"
 
     steps:
       - uses: actions/checkout@v4
         with:
@@ -158,15 +156,15 @@
 
       - name: delvewheel install
         if: runner.os == 'Windows'
         run: |
           python -m pip install delvewheel cython
 
       - name: Build wheels
-        uses: joerick/cibuildwheel@v2.16.5
+        uses: joerick/cibuildwheel@v2.18.1
 
       - uses: actions/upload-artifact@v3
         with:
           path: ./wheelhouse/*.whl
           name: wheels
 
   buildWin:
@@ -181,15 +179,15 @@
           # https://cibuildwheel.readthedocs.io/en/stable/options/#build-skip
           - os: windows-latest
             skip: "*2*win* *win32 pp*"
 
     name: ${{ matrix.os }} ${{ matrix.architecture}}
     env:
       CIBW_REPAIR_WHEEL_COMMAND_WINDOWS: "delvewheel repair -w {dest_dir} {wheel}"
-      CIBW_BEFORE_ALL: "pip install numpy cython"
+      CIBW_BEFORE_ALL: "pip install cython"
       CIBW_SKIP: ${{ matrix.skip }}
       CIBW_ARCHS_LINUX: ${{ matrix.linux_archs }}
       CIBW_TEST_SKIP: "*"
       CIBW_BEFORE_TEST: "git status"
 
     steps:
         - uses: actions/checkout@v4
@@ -213,15 +211,15 @@
 
         - name: delvewheel install
           if: runner.os == 'Windows'
           run: |
             python -m pip install delvewheel cython
 
         - name: Build wheels
-          uses: joerick/cibuildwheel@v2.16.5
+          uses: joerick/cibuildwheel@v2.18.1
 
         - uses: actions/upload-artifact@v3
           with:
             path: ./wheelhouse/*.whl
             name: wheels
 
   buildMAC:
@@ -231,29 +229,29 @@
       fail-fast: false
       matrix:
         os: [macos-latest]
         architecture: ["universal2",  "arm64"]
 
     name: ${{ matrix.os }} ${{ matrix.architecture}}
     env:
-      CIBW_BEFORE_ALL: "pip install numpy cython"
-      CIBW_SKIP: ${{ matrix.skip }}
+      CIBW_BEFORE_ALL: "pip install numpy==2.0.0rc1 cython"
+      CIBW_SKIP: "pp* *37* *38*"
       CIBW_ARCHS_MACOS: ${{ matrix.architecture }}
       CIBW_TEST_SKIP: "*"
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Setup Python
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
 
       - name: Build wheels
-        uses: joerick/cibuildwheel@v2.16.5
+        uses: joerick/cibuildwheel@v2.18.1
 
       - uses: actions/upload-artifact@v3
         with:
           path: ./wheelhouse/*.whl
           name: wheels
```

### Comparing `fastparquet-2024.2.0/.pylintrc` & `fastparquet-2024.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `fastparquet-2024.2.0/.readthedocs.yaml` & `fastparquet-2024.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fastparquet-2024.2.0/LICENSE` & `fastparquet-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastparquet-2024.2.0/PKG-INFO` & `fastparquet-2024.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: fastparquet
-Version: 2024.2.0
+Version: 2024.5.0
 Summary: Python support for Parquet file format
 Home-page: https://github.com/dask/fastparquet/
 Author: Martin Durant
 Author-email: mdurant@anaconda.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: pandas>=1.5.0
-Requires-Dist: numpy>=1.20.3
+Requires-Dist: numpy
 Requires-Dist: cramjam>=2.3
 Requires-Dist: fsspec
 Requires-Dist: packaging
 Provides-Extra: lzo
 Requires-Dist: python-lzo; extra == "lzo"
 
 fastparquet
```

### Comparing `fastparquet-2024.2.0/README.rst` & `fastparquet-2024.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `fastparquet-2024.2.0/fastparquet/api.py` & `fastparquet-2024.5.0/fastparquet/api.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2024.2.0/fastparquet/cencoding.c` & `fastparquet-2024.5.0/fastparquet/cencoding.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "fastparquet.cencoding",
         "sources": [
@@ -50,18 +50,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -145,14 +145,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -206,14 +208,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -267,60 +271,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -403,14 +430,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -746,16 +776,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1099,15 +1134,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1186,15 +1221,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1296,32 +1331,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -2766,30 +2784,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_8
-#define __PYX_HAVE_RT_ImportType_proto_3_0_8
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_8 {
-   __Pyx_ImportType_CheckSize_Error_3_0_8 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_8 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_8 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* GetNameInClass.proto */
 #define __Pyx_GetNameInClass(var, nmspace, name)  (var) = __Pyx__GetNameInClass(nmspace, name)
 static PyObject *__Pyx__GetNameInClass(PyObject *nmspace, PyObject *name);
 
 /* CLineInTraceback.proto */
@@ -19377,70 +19395,70 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4real_real(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
 
   /* "cpython/complex.pxd":20
  *         @property
- *         cdef inline double real(self):
+ *         cdef inline double real(self) noexcept:
  *             return self.cval.real             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = __pyx_v_self->cval.real;
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
 /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4imag_imag(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
 
   /* "cpython/complex.pxd":24
  *         @property
- *         cdef inline double imag(self):
+ *         cdef inline double imag(self) noexcept:
  *             return self.cval.imag             # <<<<<<<<<<<<<<
  * 
  *     # PyTypeObject PyComplex_Type
  */
   __pyx_r = __pyx_v_self->cval.imag;
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
@@ -35067,25 +35085,27 @@
   __Pyx_XDECREF(__pyx_v_d2);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static struct __pyx_vtabstruct_11fastparquet_9cencoding_NumpyIO __pyx_vtable_11fastparquet_9cencoding_NumpyIO;
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_11fastparquet_9cencoding_NumpyIO *__pyx_freelist_11fastparquet_9cencoding_NumpyIO[100];
 static int __pyx_freecount_11fastparquet_9cencoding_NumpyIO = 0;
+#endif
 
 static PyObject *__pyx_tp_new_11fastparquet_9cencoding_NumpyIO(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_11fastparquet_9cencoding_NumpyIO *p;
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_11fastparquet_9cencoding_NumpyIO > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_11fastparquet_9cencoding_NumpyIO)))) {
     o = (PyObject*)__pyx_freelist_11fastparquet_9cencoding_NumpyIO[--__pyx_freecount_11fastparquet_9cencoding_NumpyIO];
     memset(o, 0, sizeof(struct __pyx_obj_11fastparquet_9cencoding_NumpyIO));
     (void) PyObject_INIT(o, t);
   } else
   #endif
   {
@@ -35104,15 +35124,15 @@
   return NULL;
 }
 
 static void __pyx_tp_dealloc_11fastparquet_9cencoding_NumpyIO(PyObject *o) {
   struct __pyx_obj_11fastparquet_9cencoding_NumpyIO *p = (struct __pyx_obj_11fastparquet_9cencoding_NumpyIO *)o;
   __PYX_XCLEAR_MEMVIEW(&p->data, 1);
   p->data.memview = NULL; p->data.data = NULL;
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_11fastparquet_9cencoding_NumpyIO < 100) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_11fastparquet_9cencoding_NumpyIO)))) {
     __pyx_freelist_11fastparquet_9cencoding_NumpyIO[__pyx_freecount_11fastparquet_9cencoding_NumpyIO++] = ((struct __pyx_obj_11fastparquet_9cencoding_NumpyIO *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -35245,25 +35265,27 @@
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 static struct __pyx_vtabstruct_11fastparquet_9cencoding_ThriftObject __pyx_vtable_11fastparquet_9cencoding_ThriftObject;
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_11fastparquet_9cencoding_ThriftObject *__pyx_freelist_11fastparquet_9cencoding_ThriftObject[1000];
 static int __pyx_freecount_11fastparquet_9cencoding_ThriftObject = 0;
+#endif
 
 static PyObject *__pyx_tp_new_11fastparquet_9cencoding_ThriftObject(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_11fastparquet_9cencoding_ThriftObject *p;
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_11fastparquet_9cencoding_ThriftObject > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_11fastparquet_9cencoding_ThriftObject)))) {
     o = (PyObject*)__pyx_freelist_11fastparquet_9cencoding_ThriftObject[--__pyx_freecount_11fastparquet_9cencoding_ThriftObject];
     memset(o, 0, sizeof(struct __pyx_obj_11fastparquet_9cencoding_ThriftObject));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -35284,15 +35306,15 @@
 static void __pyx_tp_dealloc_11fastparquet_9cencoding_ThriftObject(PyObject *o) {
   struct __pyx_obj_11fastparquet_9cencoding_ThriftObject *p = (struct __pyx_obj_11fastparquet_9cencoding_ThriftObject *)o;
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   Py_CLEAR(p->spec);
   Py_CLEAR(p->children);
   Py_CLEAR(p->data);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_11fastparquet_9cencoding_ThriftObject < 1000) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_11fastparquet_9cencoding_ThriftObject)))) {
     __pyx_freelist_11fastparquet_9cencoding_ThriftObject[__pyx_freecount_11fastparquet_9cencoding_ThriftObject++] = ((struct __pyx_obj_11fastparquet_9cencoding_ThriftObject *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -35548,24 +35570,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_11fastparquet_9cencoding___pyx_scope_struct__genexpr *__pyx_freelist_11fastparquet_9cencoding___pyx_scope_struct__genexpr[8];
 static int __pyx_freecount_11fastparquet_9cencoding___pyx_scope_struct__genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_11fastparquet_9cencoding___pyx_scope_struct__genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_11fastparquet_9cencoding___pyx_scope_struct__genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_11fastparquet_9cencoding___pyx_scope_struct__genexpr)))) {
     o = (PyObject*)__pyx_freelist_11fastparquet_9cencoding___pyx_scope_struct__genexpr[--__pyx_freecount_11fastparquet_9cencoding___pyx_scope_struct__genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_11fastparquet_9cencoding___pyx_scope_struct__genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -35586,15 +35610,15 @@
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_a);
   Py_CLEAR(p->__pyx_v_b);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_11fastparquet_9cencoding___pyx_scope_struct__genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_11fastparquet_9cencoding___pyx_scope_struct__genexpr)))) {
     __pyx_freelist_11fastparquet_9cencoding___pyx_scope_struct__genexpr[__pyx_freecount_11fastparquet_9cencoding___pyx_scope_struct__genexpr++] = ((struct __pyx_obj_11fastparquet_9cencoding___pyx_scope_struct__genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -37605,31 +37629,31 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -42994,18 +43018,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_8
-#define __PYX_HAVE_RT_ImportType_3_0_8
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -43051,23 +43075,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_8 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_8 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `fastparquet-2024.2.0/fastparquet/cencoding.pyx` & `fastparquet-2024.5.0/fastparquet/cencoding.pyx`

 * *Files identical despite different names*

### Comparing `fastparquet-2024.2.0/fastparquet/compression.py` & `fastparquet-2024.5.0/fastparquet/compression.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2024.2.0/fastparquet/converted_types.py` & `fastparquet-2024.5.0/fastparquet/converted_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,17 @@
         tobson = bson.dumps
     except:
         def unbson(x):
             raise ImportError("BSON not found")
         def tobson(x):
             raise ImportError("BSON not found")
 
-DAYS_TO_MILLIS = 86400000000000
-"""Number of millis in a day. Used to convert a Date to a date"""
+# Explicitly use numpy type in order to avoid promotion errors due to NEP 50 in numpy >= 2
+DAYS_TO_NANOS = np.int64(86400000000000)
+"""Number of nanoseconds in a day. Used to convert a Date to a date"""
 nat = np.datetime64('NaT').view('int64')
 
 simple = {
     parquet_thrift.Type.INT32: np.dtype('int32'),
     parquet_thrift.Type.INT64: np.dtype('int64'),
     parquet_thrift.Type.FLOAT: np.dtype('float32'),
     parquet_thrift.Type.DOUBLE: np.dtype('float64'),
@@ -154,15 +155,15 @@
     se: a schema element.
     timestamp96: convert int96 as if it were written by mr-parquet
     """
     ctype = se.converted_type
     if se.type == parquet_thrift.Type.INT96 and timestamp96:
         data2 = data.view([('ns', 'i8'), ('day', 'i4')])
         # TODO: this should be ms unit, now that we can?
-        return ((data2['day'] - 2440588) * 86400000000000 +
+        return ((data2['day'] - np.int64(2440588)) * DAYS_TO_NANOS +
                 data2['ns']).view('M8[ns]')
     if se.logicalType is not None and se.logicalType.TIMESTAMP is not None:
         dt = _logical_to_time_dtype(se.logicalType.TIMESTAMP)
         return data.view(dt)
     if ctype is None:
         return data
     if ctype == parquet_thrift.ConvertedType.UTF8:
@@ -184,15 +185,15 @@
             return np.array([
                 int.from_bytes(
                     data.data[i:i + 1], byteorder='big', signed=True
                 ) * scale_factor
                 for i in range(len(data))
             ])
     elif ctype == parquet_thrift.ConvertedType.DATE:
-        data = data * DAYS_TO_MILLIS
+        data = data * DAYS_TO_NANOS
         return data.view('datetime64[ns]')
     elif ctype == parquet_thrift.ConvertedType.TIME_MILLIS:
         # this was not covered by new pandas time units
         data = data.astype('int64', copy=False)
         time_shift(data, 1000000)
         return data.view('timedelta64[ns]')
     elif ctype == parquet_thrift.ConvertedType.TIMESTAMP_MILLIS:
```

### Comparing `fastparquet-2024.2.0/fastparquet/core.py` & `fastparquet-2024.5.0/fastparquet/core.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2024.2.0/fastparquet/dataframe.py` & `fastparquet-2024.5.0/fastparquet/dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                 # 1) create the DatetimeIndex in UTC as no datetime conversion is needed and
                 # it works with d uninitialised data (no NonExistentTimeError or AmbiguousTimeError)
                 # 2) convert to timezone (if UTC=noop, if None=remove tz, if other=change tz)
                 index = DatetimeIndex(d, tz="UTC").tz_convert(
                     tz_to_dt_tz(timezones[str(col)]))
             else:
                 index = Index(d)
-            views[col] = index.values
+            views[col] = d
     else:
         index = MultiIndex([[]], [[]])
         # index = MultiIndex.from_arrays(indexes)
         index._levels = list()
         index._labels = list()
         index._codes = list()
         index._names = list(index_names)
```

### Comparing `fastparquet-2024.2.0/fastparquet/encoding.py` & `fastparquet-2024.5.0/fastparquet/encoding.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2024.2.0/fastparquet/json.py` & `fastparquet-2024.5.0/fastparquet/json.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2024.2.0/fastparquet/parquet.thrift` & `fastparquet-2024.5.0/fastparquet/parquet.thrift`

 * *Files identical despite different names*

### Comparing `fastparquet-2024.2.0/fastparquet/parquet_thrift/parquet/ttypes.py` & `fastparquet-2024.5.0/fastparquet/parquet_thrift/parquet/ttypes.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2024.2.0/fastparquet/schema.py` & `fastparquet-2024.5.0/fastparquet/schema.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2024.2.0/fastparquet/speedups.c` & `fastparquet-2024.5.0/fastparquet/speedups.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "fastparquet.speedups",
         "sources": [
@@ -50,18 +50,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -145,14 +145,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -206,14 +208,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -267,60 +271,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -403,14 +430,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -746,16 +776,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1099,15 +1134,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1186,15 +1221,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1303,32 +1338,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1663,200 +1681,164 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":770
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":735
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":778
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":742
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":784
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":747
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":756
- * # The int types are mapped a bit surprising --
- * # numpy.int corresponds to 'l' and numpy.long to 'q'
- * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
- * ctypedef npy_longlong   longlong_t
- */
-typedef npy_long __pyx_t_5numpy_int_t;
-
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
- * # numpy.int corresponds to 'l' and numpy.long to 'q'
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+ * ctypedef double complex complex128_t
  * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
+ * ctypedef npy_ulonglong  ulonglong_t
  * 
- * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
- * ctypedef npy_longlong   longlong_t
- * 
- * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
- * ctypedef npy_ulonglong  ulonglong_t
- */
-typedef npy_ulong __pyx_t_5numpy_uint_t;
-
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
- * 
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
  * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":762
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
+ * ctypedef npy_longlong   longlong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":795
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":796
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":798
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":799
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":800
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
- * ctypedef npy_cfloat      cfloat_t
+ * ctypedef float complex       cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
 /* #### Code section: complex_type_declarations ### */
 /* Declarations.proto */
 #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     typedef ::std::complex< float > __pyx_t_float_complex;
@@ -1876,14 +1858,26 @@
     typedef double _Complex __pyx_t_double_complex;
   #endif
 #else
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
+/* Declarations.proto */
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
+  #ifdef __cplusplus
+    typedef ::std::complex< long double > __pyx_t_long_double_complex;
+  #else
+    typedef long double _Complex __pyx_t_long_double_complex;
+  #endif
+#else
+    typedef struct { long double real, imag; } __pyx_t_long_double_complex;
+#endif
+static CYTHON_INLINE __pyx_t_long_double_complex __pyx_t_long_double_complex_from_parts(long double, long double);
+
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
@@ -1910,49 +1904,31 @@
  *     or the provided default value if no such value was found.
  */
 struct __pyx_opt_args_7cpython_11contextvars_get_value_no_default {
   int __pyx_n;
   PyObject *default_value;
 };
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
- * ctypedef npy_longdouble longdouble_t
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1096
  * 
- * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
- * ctypedef npy_cdouble     cdouble_t
- * ctypedef npy_clongdouble clongdouble_t
- */
-typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
-
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":772
- * 
- * ctypedef npy_cfloat      cfloat_t
- * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
- * ctypedef npy_clongdouble clongdouble_t
- * 
- */
-typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
-
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
- * ctypedef npy_cfloat      cfloat_t
- * ctypedef npy_cdouble     cdouble_t
- * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
+ * # Iterator API added in v1.6
+ * ctypedef int (*NpyIter_IterNextFunc)(NpyIter* it) noexcept nogil             # <<<<<<<<<<<<<<
+ * ctypedef void (*NpyIter_GetMultiIndexFunc)(NpyIter* it, npy_intp* outcoords) noexcept nogil
  * 
- * ctypedef npy_cdouble     complex_t
  */
-typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
+typedef int (*__pyx_t_5numpy_NpyIter_IterNextFunc)(NpyIter *);
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":775
- * ctypedef npy_clongdouble clongdouble_t
- * 
- * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1097
+ * # Iterator API added in v1.6
+ * ctypedef int (*NpyIter_IterNextFunc)(NpyIter* it) noexcept nogil
+ * ctypedef void (*NpyIter_GetMultiIndexFunc)(NpyIter* it, npy_intp* outcoords) noexcept nogil             # <<<<<<<<<<<<<<
  * 
- * cdef inline object PyArray_MultiIterNew1(a):
+ * cdef extern from "numpy/arrayobject.h":
  */
-typedef npy_cdouble __pyx_t_5numpy_complex_t;
+typedef void (*__pyx_t_5numpy_NpyIter_GetMultiIndexFunc)(NpyIter *, npy_intp *);
 
 /* "View.MemoryView":114
  * @cython.collection_type("sequence")
  * @cname("__pyx_array")
  * cdef class array:             # <<<<<<<<<<<<<<
  * 
  *     cdef:
@@ -2745,30 +2721,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_8
-#define __PYX_HAVE_RT_ImportType_proto_3_0_8
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_8 {
-   __Pyx_ImportType_CheckSize_Error_3_0_8 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_8 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_8 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -3077,14 +3053,52 @@
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_conj_double(__pyx_t_double_complex);
     #if 1
         static CYTHON_INLINE double __Pyx_c_abs_double(__pyx_t_double_complex);
         static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_pow_double(__pyx_t_double_complex, __pyx_t_double_complex);
     #endif
 #endif
 
+/* Arithmetic.proto */
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
+    #define __Pyx_c_eq_long__double(a, b)   ((a)==(b))
+    #define __Pyx_c_sum_long__double(a, b)  ((a)+(b))
+    #define __Pyx_c_diff_long__double(a, b) ((a)-(b))
+    #define __Pyx_c_prod_long__double(a, b) ((a)*(b))
+    #define __Pyx_c_quot_long__double(a, b) ((a)/(b))
+    #define __Pyx_c_neg_long__double(a)     (-(a))
+  #ifdef __cplusplus
+    #define __Pyx_c_is_zero_long__double(z) ((z)==(long double)0)
+    #define __Pyx_c_conj_long__double(z)    (::std::conj(z))
+    #if 1
+        #define __Pyx_c_abs_long__double(z)     (::std::abs(z))
+        #define __Pyx_c_pow_long__double(a, b)  (::std::pow(a, b))
+    #endif
+  #else
+    #define __Pyx_c_is_zero_long__double(z) ((z)==0)
+    #define __Pyx_c_conj_long__double(z)    (conjl(z))
+    #if 1
+        #define __Pyx_c_abs_long__double(z)     (cabsl(z))
+        #define __Pyx_c_pow_long__double(a, b)  (cpowl(a, b))
+    #endif
+ #endif
+#else
+    static CYTHON_INLINE int __Pyx_c_eq_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_sum_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_diff_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_prod_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_quot_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_neg_long__double(__pyx_t_long_double_complex);
+    static CYTHON_INLINE int __Pyx_c_is_zero_long__double(__pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_conj_long__double(__pyx_t_long_double_complex);
+    #if 1
+        static CYTHON_INLINE long double __Pyx_c_abs_long__double(__pyx_t_long_double_complex);
+        static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_pow_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    #endif
+#endif
+
 /* MemviewSliceCopyTemplate.proto */
 static __Pyx_memviewslice
 __pyx_memoryview_copy_new_contig(const __Pyx_memviewslice *from_mvs,
                                  const char *mode, int ndim,
                                  size_t sizeof_dtype, int contig_flag,
                                  int dtype_is_object);
 
@@ -3159,14 +3173,26 @@
 static PyObject *__pyx_memoryview_assign_item_from_object(struct __pyx_memoryview_obj *__pyx_v_self, char *__pyx_v_itemp, PyObject *__pyx_v_value); /* proto*/
 static PyObject *__pyx_memoryview__get_base(struct __pyx_memoryview_obj *__pyx_v_self); /* proto*/
 static PyObject *__pyx_memoryviewslice_convert_item_to_object(struct __pyx_memoryviewslice_obj *__pyx_v_self, char *__pyx_v_itemp); /* proto*/
 static PyObject *__pyx_memoryviewslice_assign_item_from_object(struct __pyx_memoryviewslice_obj *__pyx_v_self, char *__pyx_v_itemp, PyObject *__pyx_v_value); /* proto*/
 static PyObject *__pyx_memoryviewslice__get_base(struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto*/
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4real_real(PyComplexObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4imag_imag(PyComplexObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_8itemsize_itemsize(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_9alignment_alignment(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_6fields_fields(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_5names_names(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyArray_ArrayDescr *__pyx_f_5numpy_5dtype_8subarray_subarray(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_uint64 __pyx_f_5numpy_5dtype_5flags_flags(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_7numiter_numiter(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_4size_size(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_5index_index(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_2nd_nd(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_9broadcast_10dimensions_dimensions(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE void **__pyx_f_5numpy_9broadcast_5iters_iters(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self); /* proto*/
@@ -3460,30 +3486,30 @@
 static const char __pyx_k_Dimension_d_is_not_direct[] = "Dimension %d is not direct";
 static const char __pyx_k_Index_out_of_bounds_axis_d[] = "Index out of bounds (axis %d)";
 static const char __pyx_k_Step_may_not_be_zero_axis_d[] = "Step may not be zero (axis %d)";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_Native_accelerators_for_Parquet[] = "\nNative accelerators for Parquet encoding and decoding.\n";
-static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_All_dimensions_preceding_dimensi[] = "All dimensions preceding dimension %d must be indexed and not sliced";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
 static const char __pyx_k_Cannot_transpose_memoryview_with[] = "Cannot transpose memoryview with indirect dimensions";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))";
 static const char __pyx_k_Indirect_dimensions_not_supporte[] = "Indirect dimensions not supported";
 static const char __pyx_k_Invalid_mode_expected_c_or_fortr[] = "Invalid mode, expected 'c' or 'fortran', got ";
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis ";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension ";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
-static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
+static const char __pyx_k_numpy__core_multiarray_failed_to[] = "numpy._core.multiarray failed to import";
+static const char __pyx_k_numpy__core_umath_failed_to_impo[] = "numpy._core.umath failed to import";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
 /* #### Code section: decls ### */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
@@ -3778,16 +3804,16 @@
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_name_2;
   PyObject *__pyx_n_s_ndim;
   PyObject *__pyx_n_s_new;
   PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
   PyObject *__pyx_n_s_np;
   PyObject *__pyx_n_s_numpy;
-  PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
-  PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
+  PyObject *__pyx_kp_u_numpy__core_multiarray_failed_to;
+  PyObject *__pyx_kp_u_numpy__core_umath_failed_to_impo;
   PyObject *__pyx_n_s_obj;
   PyObject *__pyx_n_s_obj_dtype;
   PyObject *__pyx_n_s_object;
   PyObject *__pyx_n_u_object;
   PyObject *__pyx_n_s_out;
   PyObject *__pyx_n_s_pack;
   PyObject *__pyx_n_s_pack_byte_array;
@@ -4027,16 +4053,16 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_name_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_ndim);
   Py_CLEAR(clear_module_state->__pyx_n_s_new);
   Py_CLEAR(clear_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_CLEAR(clear_module_state->__pyx_n_s_np);
   Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy__core_multiarray_failed_to);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy__core_umath_failed_to_impo);
   Py_CLEAR(clear_module_state->__pyx_n_s_obj);
   Py_CLEAR(clear_module_state->__pyx_n_s_obj_dtype);
   Py_CLEAR(clear_module_state->__pyx_n_s_object);
   Py_CLEAR(clear_module_state->__pyx_n_u_object);
   Py_CLEAR(clear_module_state->__pyx_n_s_out);
   Py_CLEAR(clear_module_state->__pyx_n_s_pack);
   Py_CLEAR(clear_module_state->__pyx_n_s_pack_byte_array);
@@ -4254,16 +4280,16 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_name_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_ndim);
   Py_VISIT(traverse_module_state->__pyx_n_s_new);
   Py_VISIT(traverse_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_VISIT(traverse_module_state->__pyx_n_s_np);
   Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy__core_multiarray_failed_to);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy__core_umath_failed_to_impo);
   Py_VISIT(traverse_module_state->__pyx_n_s_obj);
   Py_VISIT(traverse_module_state->__pyx_n_s_obj_dtype);
   Py_VISIT(traverse_module_state->__pyx_n_s_object);
   Py_VISIT(traverse_module_state->__pyx_n_u_object);
   Py_VISIT(traverse_module_state->__pyx_n_s_out);
   Py_VISIT(traverse_module_state->__pyx_n_s_pack);
   Py_VISIT(traverse_module_state->__pyx_n_s_pack_byte_array);
@@ -4587,16 +4613,16 @@
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_name_2 __pyx_mstate_global->__pyx_n_s_name_2
 #define __pyx_n_s_ndim __pyx_mstate_global->__pyx_n_s_ndim
 #define __pyx_n_s_new __pyx_mstate_global->__pyx_n_s_new
 #define __pyx_kp_s_no_default___reduce___due_to_non __pyx_mstate_global->__pyx_kp_s_no_default___reduce___due_to_non
 #define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
 #define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
-#define __pyx_kp_u_numpy_core_multiarray_failed_to __pyx_mstate_global->__pyx_kp_u_numpy_core_multiarray_failed_to
-#define __pyx_kp_u_numpy_core_umath_failed_to_impor __pyx_mstate_global->__pyx_kp_u_numpy_core_umath_failed_to_impor
+#define __pyx_kp_u_numpy__core_multiarray_failed_to __pyx_mstate_global->__pyx_kp_u_numpy__core_multiarray_failed_to
+#define __pyx_kp_u_numpy__core_umath_failed_to_impo __pyx_mstate_global->__pyx_kp_u_numpy__core_umath_failed_to_impo
 #define __pyx_n_s_obj __pyx_mstate_global->__pyx_n_s_obj
 #define __pyx_n_s_obj_dtype __pyx_mstate_global->__pyx_n_s_obj_dtype
 #define __pyx_n_s_object __pyx_mstate_global->__pyx_n_s_object
 #define __pyx_n_u_object __pyx_mstate_global->__pyx_n_u_object
 #define __pyx_n_s_out __pyx_mstate_global->__pyx_n_s_out
 #define __pyx_n_s_pack __pyx_mstate_global->__pyx_n_s_pack
 #define __pyx_n_s_pack_byte_array __pyx_mstate_global->__pyx_n_s_pack_byte_array
@@ -18298,70 +18324,70 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4real_real(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
 
   /* "cpython/complex.pxd":20
  *         @property
- *         cdef inline double real(self):
+ *         cdef inline double real(self) noexcept:
  *             return self.cval.real             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = __pyx_v_self->cval.real;
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
 /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4imag_imag(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
 
   /* "cpython/complex.pxd":24
  *         @property
- *         cdef inline double imag(self):
+ *         cdef inline double imag(self) noexcept:
  *             return self.cval.imag             # <<<<<<<<<<<<<<
  * 
  *     # PyTypeObject PyComplex_Type
  */
   __pyx_r = __pyx_v_self->cval.imag;
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
@@ -18588,262 +18614,686 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_pyvalue);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":246
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":286
+ * 
+ *         @property
+ *         cdef inline npy_intp itemsize(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_ELSIZE(self)
+ * 
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_8itemsize_itemsize(PyArray_Descr *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":287
+ *         @property
+ *         cdef inline npy_intp itemsize(self) noexcept nogil:
+ *             return PyDataType_ELSIZE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyDataType_ELSIZE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":286
+ * 
+ *         @property
+ *         cdef inline npy_intp itemsize(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_ELSIZE(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+ * 
+ *         @property
+ *         cdef inline npy_intp alignment(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_ALIGNMENT(self)
+ * 
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_9alignment_alignment(PyArray_Descr *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":291
+ *         @property
+ *         cdef inline npy_intp alignment(self) noexcept nogil:
+ *             return PyDataType_ALIGNMENT(self)             # <<<<<<<<<<<<<<
+ * 
+ *         # Use fields/names with care as they may be NULL.  You must check
+ */
+  __pyx_r = PyDataType_ALIGNMENT(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+ * 
+ *         @property
+ *         cdef inline npy_intp alignment(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_ALIGNMENT(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":296
+ *         # for this using PyDataType_HASFIELDS.
+ *         @property
+ *         cdef inline object fields(self):             # <<<<<<<<<<<<<<
+ *             return <object>PyDataType_FIELDS(self)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_6fields_fields(PyArray_Descr *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1;
+  __Pyx_RefNannySetupContext("fields", 1);
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":297
+ *         @property
+ *         cdef inline object fields(self):
+ *             return <object>PyDataType_FIELDS(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyDataType_FIELDS(__pyx_v_self);
+  __Pyx_INCREF(((PyObject *)__pyx_t_1));
+  __pyx_r = ((PyObject *)__pyx_t_1);
+  goto __pyx_L0;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":296
+ *         # for this using PyDataType_HASFIELDS.
+ *         @property
+ *         cdef inline object fields(self):             # <<<<<<<<<<<<<<
+ *             return <object>PyDataType_FIELDS(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":300
+ * 
+ *         @property
+ *         cdef inline tuple names(self):             # <<<<<<<<<<<<<<
+ *             return <tuple>PyDataType_NAMES(self)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_5names_names(PyArray_Descr *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1;
+  __Pyx_RefNannySetupContext("names", 1);
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":301
+ *         @property
+ *         cdef inline tuple names(self):
+ *             return <tuple>PyDataType_NAMES(self)             # <<<<<<<<<<<<<<
+ * 
+ *         # Use PyDataType_HASSUBARRAY to test whether this field is
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyDataType_NAMES(__pyx_v_self);
+  __Pyx_INCREF(((PyObject*)__pyx_t_1));
+  __pyx_r = ((PyObject*)__pyx_t_1);
+  goto __pyx_L0;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":300
+ * 
+ *         @property
+ *         cdef inline tuple names(self):             # <<<<<<<<<<<<<<
+ *             return <tuple>PyDataType_NAMES(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":307
+ *         # this field via the inline helper method PyDataType_SHAPE.
+ *         @property
+ *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_SUBARRAY(self)
+ * 
+ */
+
+static CYTHON_INLINE PyArray_ArrayDescr *__pyx_f_5numpy_5dtype_8subarray_subarray(PyArray_Descr *__pyx_v_self) {
+  PyArray_ArrayDescr *__pyx_r;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":308
+ *         @property
+ *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:
+ *             return PyDataType_SUBARRAY(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyDataType_SUBARRAY(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":307
+ *         # this field via the inline helper method PyDataType_SHAPE.
+ *         @property
+ *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_SUBARRAY(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":311
  * 
  *         @property
- *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_uint64 flags(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The data types flags."""
+ *             return PyDataType_FLAGS(self)
+ */
+
+static CYTHON_INLINE npy_uint64 __pyx_f_5numpy_5dtype_5flags_flags(PyArray_Descr *__pyx_v_self) {
+  npy_uint64 __pyx_r;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":313
+ *         cdef inline npy_uint64 flags(self) noexcept nogil:
+ *             """The data types flags."""
+ *             return PyDataType_FLAGS(self)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyDataType_FLAGS(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":311
+ * 
+ *         @property
+ *         cdef inline npy_uint64 flags(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The data types flags."""
+ *             return PyDataType_FLAGS(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":323
+ * 
+ *         @property
+ *         cdef inline int numiter(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The number of arrays that need to be broadcast to the same shape."""
+ *             return PyArray_MultiIter_NUMITER(self)
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_7numiter_numiter(PyArrayMultiIterObject *__pyx_v_self) {
+  int __pyx_r;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":325
+ *         cdef inline int numiter(self) noexcept nogil:
+ *             """The number of arrays that need to be broadcast to the same shape."""
+ *             return PyArray_MultiIter_NUMITER(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_NUMITER(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":323
+ * 
+ *         @property
+ *         cdef inline int numiter(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The number of arrays that need to be broadcast to the same shape."""
+ *             return PyArray_MultiIter_NUMITER(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":328
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The total broadcasted size."""
+ *             return PyArray_MultiIter_SIZE(self)
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_4size_size(PyArrayMultiIterObject *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":330
+ *         cdef inline npy_intp size(self) noexcept nogil:
+ *             """The total broadcasted size."""
+ *             return PyArray_MultiIter_SIZE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_SIZE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":328
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The total broadcasted size."""
+ *             return PyArray_MultiIter_SIZE(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":333
+ * 
+ *         @property
+ *         cdef inline npy_intp index(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The current (1-d) index into the broadcasted result."""
+ *             return PyArray_MultiIter_INDEX(self)
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_5index_index(PyArrayMultiIterObject *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":335
+ *         cdef inline npy_intp index(self) noexcept nogil:
+ *             """The current (1-d) index into the broadcasted result."""
+ *             return PyArray_MultiIter_INDEX(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_INDEX(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":333
+ * 
+ *         @property
+ *         cdef inline npy_intp index(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The current (1-d) index into the broadcasted result."""
+ *             return PyArray_MultiIter_INDEX(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":338
+ * 
+ *         @property
+ *         cdef inline int nd(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The number of dimensions in the broadcasted result."""
+ *             return PyArray_MultiIter_NDIM(self)
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_2nd_nd(PyArrayMultiIterObject *__pyx_v_self) {
+  int __pyx_r;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":340
+ *         cdef inline int nd(self) noexcept nogil:
+ *             """The number of dimensions in the broadcasted result."""
+ *             return PyArray_MultiIter_NDIM(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_NDIM(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":338
+ * 
+ *         @property
+ *         cdef inline int nd(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The number of dimensions in the broadcasted result."""
+ *             return PyArray_MultiIter_NDIM(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":343
+ * 
+ *         @property
+ *         cdef inline npy_intp* dimensions(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The shape of the broadcasted result."""
+ *             return PyArray_MultiIter_DIMS(self)
+ */
+
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_9broadcast_10dimensions_dimensions(PyArrayMultiIterObject *__pyx_v_self) {
+  npy_intp *__pyx_r;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":345
+ *         cdef inline npy_intp* dimensions(self) noexcept nogil:
+ *             """The shape of the broadcasted result."""
+ *             return PyArray_MultiIter_DIMS(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_DIMS(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":343
+ * 
+ *         @property
+ *         cdef inline npy_intp* dimensions(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The shape of the broadcasted result."""
+ *             return PyArray_MultiIter_DIMS(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":348
+ * 
+ *         @property
+ *         cdef inline void** iters(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
+ *             On return, the iterators are adjusted for broadcasting."""
+ */
+
+static CYTHON_INLINE void **__pyx_f_5numpy_9broadcast_5iters_iters(PyArrayMultiIterObject *__pyx_v_self) {
+  void **__pyx_r;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":351
+ *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
+ *             On return, the iterators are adjusted for broadcasting."""
+ *             return PyArray_MultiIter_ITERS(self)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyArray_MultiIter_ITERS(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":348
+ * 
+ *         @property
+ *         cdef inline void** iters(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
+ *             On return, the iterators are adjusted for broadcasting."""
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":366
+ * 
+ *         @property
+ *         cdef inline PyObject* base(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":249
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":369
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":246
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":366
  * 
  *         @property
- *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline PyObject* base(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":252
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":372
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":255
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":375
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":252
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":372
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":258
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":378
  * 
  *         @property
- *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline int ndim(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":261
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":381
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":258
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":378
  * 
  *         @property
- *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline int ndim(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":264
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":384
  * 
  *         @property
- *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp *shape(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":269
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":389
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":264
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":384
  * 
  *         @property
- *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp *shape(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":272
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":392
  * 
  *         @property
- *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp *strides(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":276
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":396
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":272
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":392
  * 
  *         @property
- *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp *strides(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":279
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":399
  * 
  *         @property
- *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":282
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":402
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":279
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":399
  * 
  *         @property
- *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":285
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":405
  * 
  *         @property
- *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline char* data(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":291
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":411
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
- *     ctypedef unsigned char      npy_bool
+ * 
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":285
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":405
  * 
  *         @property
- *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline char* data(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
- * ctypedef npy_cdouble     complex_t
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":807
+ * ctypedef long double complex clongdouble_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
@@ -18851,30 +19301,30 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":778
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":808
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 778, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 808, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
- * ctypedef npy_cdouble     complex_t
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":807
+ * ctypedef long double complex clongdouble_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
   /* function exit code */
@@ -18884,15 +19334,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":810
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18901,29 +19351,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":781
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":811
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 781, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 811, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":810
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18934,15 +19384,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":813
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18951,29 +19401,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":784
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":814
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 784, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 814, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":813
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18984,15 +19434,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":816
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19001,29 +19451,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":787
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":817
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 787, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 817, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":816
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19034,15 +19484,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":819
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19051,29 +19501,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":820
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 790, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 820, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":819
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19084,209 +19534,219 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":822
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
+  PyObject *__pyx_t_2;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":823
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":794
+    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":824
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
-    __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
+    __pyx_t_2 = __pyx_f_5numpy_5dtype_8subarray_subarray(__pyx_v_d)->shape;
+    __Pyx_INCREF(((PyObject*)__pyx_t_2));
+    __pyx_r = ((PyObject*)__pyx_t_2);
     goto __pyx_L0;
 
-    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":823
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":796
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":826
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":822
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
  *     int _import_umath() except -1
  * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ * cdef inline void set_array_base(ndarray arr, object base) except *:             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  * 
- * cdef inline void set_array_base(ndarray arr, object base):
+ * cdef inline void set_array_base(ndarray arr, object base) except *:
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
- * cdef inline void set_array_base(ndarray arr, object base):
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1012
+ * cdef inline void set_array_base(ndarray arr, object base) except *:
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(3, 1012, __pyx_L1_error)
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
  *     int _import_umath() except -1
  * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ * cdef inline void set_array_base(ndarray arr, object base) except *:             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_L0:;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1015
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":977
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1016
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":978
+    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1016
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1018
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1022
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19302,15 +19762,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19318,68 +19778,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1024
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")
+ *         raise ImportError("numpy._core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 985, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 1024, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.multiarray failed to import")
+ *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 986, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 1025, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *         __pyx_import_array()
  *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 987, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 1026, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(3, 987, __pyx_L5_except_error)
+      __PYX_ERR(3, 1026, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19387,15 +19847,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1022
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19410,16 +19870,16 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
- *         raise ImportError("numpy.core.multiarray failed to import")
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+ *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_umath(void) {
@@ -19434,15 +19894,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19450,68 +19910,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1030
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
+ *         raise ImportError("numpy._core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 991, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 1030, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1031
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
+ *         raise ImportError("numpy._core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 992, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 1031, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
  *         _import_umath()
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 993, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 1032, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(3, 993, __pyx_L5_except_error)
+      __PYX_ERR(3, 1032, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19519,16 +19979,16 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
- *         raise ImportError("numpy.core.multiarray failed to import")
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+ *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
   /* function exit code */
@@ -19542,16 +20002,16 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
- *         raise ImportError("numpy.core.umath failed to import")
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1034
+ *         raise ImportError("numpy._core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_ufunc(void) {
@@ -19566,15 +20026,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19582,68 +20042,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":997
+      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
+ *         raise ImportError("numpy._core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 997, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 1036, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1037
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
+ *         raise ImportError("numpy._core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 998, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 1037, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
+      /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
  *         _import_umath()
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 999, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 1038, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(3, 999, __pyx_L5_except_error)
+      __PYX_ERR(3, 1038, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+    /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19651,16 +20111,16 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
- *         raise ImportError("numpy.core.umath failed to import")
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1034
+ *         raise ImportError("numpy._core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
   /* function exit code */
@@ -19674,173 +20134,175 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1002
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ * cdef inline bint is_timedelta64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1053
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1002
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ * cdef inline bint is_timedelta64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1056
  * 
  * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ * cdef inline bint is_datetime64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1068
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1056
  * 
  * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ * cdef inline bint is_datetime64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1071
  * 
  * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline npy_datetime get_datetime64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1078
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1071
  * 
  * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline npy_datetime get_datetime64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1081
  * 
  * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1085
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1081
  * 
  * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+/* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1088
  * 
  * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1053
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1092
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ * 
+ * 
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1088
  * 
  * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
@@ -19967,21 +20429,20 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyArrayObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
-  npy_intp *__pyx_t_10;
-  PyArrayObject *__pyx_t_11 = NULL;
+  PyArrayObject *__pyx_t_10 = NULL;
+  Py_ssize_t __pyx_t_11;
   Py_ssize_t __pyx_t_12;
   Py_ssize_t __pyx_t_13;
   Py_ssize_t __pyx_t_14;
-  Py_ssize_t __pyx_t_15;
-  PyObject **__pyx_t_16;
+  PyObject **__pyx_t_15;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("array_encode_utf8", 1);
   __pyx_pybuffer_arr.pybuffer.buf = NULL;
   __pyx_pybuffer_arr.refcount = 0;
   __pyx_pybuffernd_arr.data = NULL;
@@ -20042,16 +20503,15 @@
   /* "fastparquet/speedups.pyx":45
  *     arr = np.array(inp, copy=False)
  * 
  *     n = arr.shape[0]             # <<<<<<<<<<<<<<
  *     # TODO: why not inplace?
  *     result = np.empty(n, dtype=object)
  */
-  __pyx_t_10 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_arr)); if (unlikely(__pyx_t_10 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L1_error)
-  __pyx_v_n = (__pyx_t_10[0]);
+  __pyx_v_n = (__pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_arr))[0]);
 
   /* "fastparquet/speedups.pyx":47
  *     n = arr.shape[0]
  *     # TODO: why not inplace?
  *     result = np.empty(n, dtype=object)             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         # Fast utf-8 encoding, avoiding method call and codec lookup indirection
@@ -20073,86 +20533,86 @@
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 47, __pyx_L1_error)
-  __pyx_t_11 = ((PyArrayObject *)__pyx_t_2);
+  __pyx_t_10 = ((PyArrayObject *)__pyx_t_2);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_result.rcbuffer->pybuffer);
-    __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_result.rcbuffer->pybuffer, (PyObject*)__pyx_t_11, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack);
+    __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_result.rcbuffer->pybuffer, (PyObject*)__pyx_t_10, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack);
     if (unlikely(__pyx_t_6 < 0)) {
       PyErr_Fetch(&__pyx_t_9, &__pyx_t_8, &__pyx_t_7);
       if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_result.rcbuffer->pybuffer, (PyObject*)__pyx_v_result, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
         Py_XDECREF(__pyx_t_9); Py_XDECREF(__pyx_t_8); Py_XDECREF(__pyx_t_7);
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_9, __pyx_t_8, __pyx_t_7);
       }
       __pyx_t_9 = __pyx_t_8 = __pyx_t_7 = 0;
     }
     __pyx_pybuffernd_result.diminfo[0].strides = __pyx_pybuffernd_result.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_result.diminfo[0].shape = __pyx_pybuffernd_result.rcbuffer->pybuffer.shape[0];
     if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 47, __pyx_L1_error)
   }
-  __pyx_t_11 = 0;
+  __pyx_t_10 = 0;
   __pyx_v_result = ((PyArrayObject *)__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "fastparquet/speedups.pyx":48
  *     # TODO: why not inplace?
  *     result = np.empty(n, dtype=object)
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         # Fast utf-8 encoding, avoiding method call and codec lookup indirection
  *         result[i] = PyUnicode_AsUTF8String(arr[i])
  */
-  __pyx_t_12 = __pyx_v_n;
-  __pyx_t_13 = __pyx_t_12;
-  for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_13; __pyx_t_14+=1) {
-    __pyx_v_i = __pyx_t_14;
+  __pyx_t_11 = __pyx_v_n;
+  __pyx_t_12 = __pyx_t_11;
+  for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
+    __pyx_v_i = __pyx_t_13;
 
     /* "fastparquet/speedups.pyx":50
  *     for i in range(n):
  *         # Fast utf-8 encoding, avoiding method call and codec lookup indirection
  *         result[i] = PyUnicode_AsUTF8String(arr[i])             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
-    __pyx_t_15 = __pyx_v_i;
+    __pyx_t_14 = __pyx_v_i;
     __pyx_t_6 = -1;
-    if (__pyx_t_15 < 0) {
-      __pyx_t_15 += __pyx_pybuffernd_arr.diminfo[0].shape;
-      if (unlikely(__pyx_t_15 < 0)) __pyx_t_6 = 0;
-    } else if (unlikely(__pyx_t_15 >= __pyx_pybuffernd_arr.diminfo[0].shape)) __pyx_t_6 = 0;
+    if (__pyx_t_14 < 0) {
+      __pyx_t_14 += __pyx_pybuffernd_arr.diminfo[0].shape;
+      if (unlikely(__pyx_t_14 < 0)) __pyx_t_6 = 0;
+    } else if (unlikely(__pyx_t_14 >= __pyx_pybuffernd_arr.diminfo[0].shape)) __pyx_t_6 = 0;
     if (unlikely(__pyx_t_6 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_6);
       __PYX_ERR(0, 50, __pyx_L1_error)
     }
-    __pyx_t_2 = (PyObject *) *__Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_arr.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_arr.diminfo[0].strides);
+    __pyx_t_2 = (PyObject *) *__Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_arr.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_arr.diminfo[0].strides);
     if (unlikely(__pyx_t_2 == NULL)) __pyx_t_2 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_2);
     __pyx_t_4 = PyUnicode_AsUTF8String(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 50, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_15 = __pyx_v_i;
+    __pyx_t_14 = __pyx_v_i;
     __pyx_t_6 = -1;
-    if (__pyx_t_15 < 0) {
-      __pyx_t_15 += __pyx_pybuffernd_result.diminfo[0].shape;
-      if (unlikely(__pyx_t_15 < 0)) __pyx_t_6 = 0;
-    } else if (unlikely(__pyx_t_15 >= __pyx_pybuffernd_result.diminfo[0].shape)) __pyx_t_6 = 0;
+    if (__pyx_t_14 < 0) {
+      __pyx_t_14 += __pyx_pybuffernd_result.diminfo[0].shape;
+      if (unlikely(__pyx_t_14 < 0)) __pyx_t_6 = 0;
+    } else if (unlikely(__pyx_t_14 >= __pyx_pybuffernd_result.diminfo[0].shape)) __pyx_t_6 = 0;
     if (unlikely(__pyx_t_6 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_6);
       __PYX_ERR(0, 50, __pyx_L1_error)
     }
-    __pyx_t_16 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_result.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_result.diminfo[0].strides);
-    __Pyx_XGOTREF(*__pyx_t_16);
-    __Pyx_INCREF(__pyx_t_4); __Pyx_XDECREF(*__pyx_t_16);
-    *__pyx_t_16 = __pyx_t_4;
-    __Pyx_XGIVEREF(*__pyx_t_16);
+    __pyx_t_15 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_result.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_result.diminfo[0].strides);
+    __Pyx_XGOTREF(*__pyx_t_15);
+    __Pyx_INCREF(__pyx_t_4); __Pyx_XDECREF(*__pyx_t_15);
+    *__pyx_t_15 = __pyx_t_4;
+    __Pyx_XGIVEREF(*__pyx_t_15);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
 
   /* "fastparquet/speedups.pyx":52
  *         result[i] = PyUnicode_AsUTF8String(arr[i])
  * 
  *     return result             # <<<<<<<<<<<<<<
@@ -22072,16 +22532,16 @@
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
     {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
     {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
     {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
     {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
     {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
-    {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
-    {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
+    {&__pyx_kp_u_numpy__core_multiarray_failed_to, __pyx_k_numpy__core_multiarray_failed_to, sizeof(__pyx_k_numpy__core_multiarray_failed_to), 0, 1, 0, 0},
+    {&__pyx_kp_u_numpy__core_umath_failed_to_impo, __pyx_k_numpy__core_umath_failed_to_impo, sizeof(__pyx_k_numpy__core_umath_failed_to_impo), 0, 1, 0, 0},
     {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
     {&__pyx_n_s_obj_dtype, __pyx_k_obj_dtype, sizeof(__pyx_k_obj_dtype), 0, 0, 1, 1},
     {&__pyx_n_s_object, __pyx_k_object, sizeof(__pyx_k_object), 0, 0, 1, 1},
     {&__pyx_n_u_object, __pyx_k_object, sizeof(__pyx_k_object), 0, 1, 0, 1},
     {&__pyx_n_s_out, __pyx_k_out, sizeof(__pyx_k_out), 0, 0, 1, 1},
     {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
     {&__pyx_n_s_pack_byte_array, __pyx_k_pack_byte_array, sizeof(__pyx_k_pack_byte_array), 0, 0, 1, 1},
@@ -22138,15 +22598,15 @@
   __pyx_builtin___import__ = __Pyx_GetBuiltinName(__pyx_n_s_import); if (!__pyx_builtin___import__) __PYX_ERR(1, 100, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 141, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 156, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 159, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 408, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 618, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 914, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(3, 987, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(3, 1026, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -22185,33 +22645,33 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *         __pyx_import_array()
  *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(3, 987, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy__core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(3, 1026, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-q4nhitod/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../private/var/folders/j9/_t7bg0ss12qbyy27ly_c2t180000gp/T/build-env-9_s12rbh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
  *         _import_umath()
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(3, 993, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy__core_umath_failed_to_impo); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(3, 1032, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "fastparquet/speedups.pyx":72
  *         val = items[i]
  *         if not PyBytes_CheckExact(val):
  *             raise TypeError("expected list of bytes")             # <<<<<<<<<<<<<<
@@ -22623,49 +23083,49 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 203, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 203, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 230, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(3, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_number) __PYX_ERR(3, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(3, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(3, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(3, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(3, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(3, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(3, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(3, 829, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_character) __PYX_ERR(3, 831, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 869, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 271, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 316, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 320, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 359, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(3, 848, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(3, 850, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(3, 852, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(3, 854, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(3, 856, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(3, 858, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(3, 860, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(3, 862, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(3, 864, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(3, 866, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 930, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -27251,18 +27711,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_3_0_8
-#define __PYX_HAVE_RT_ImportType_3_0_8
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -27308,23 +27768,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_8 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_8 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -28316,15 +28776,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -29485,14 +29945,168 @@
             z.real = z_r * cos(z_theta);
             z.imag = z_r * sin(z_theta);
             return z;
         }
     #endif
 #endif
 
+/* Declarations */
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
+  #ifdef __cplusplus
+    static CYTHON_INLINE __pyx_t_long_double_complex __pyx_t_long_double_complex_from_parts(long double x, long double y) {
+      return ::std::complex< long double >(x, y);
+    }
+  #else
+    static CYTHON_INLINE __pyx_t_long_double_complex __pyx_t_long_double_complex_from_parts(long double x, long double y) {
+      return x + y*(__pyx_t_long_double_complex)_Complex_I;
+    }
+  #endif
+#else
+    static CYTHON_INLINE __pyx_t_long_double_complex __pyx_t_long_double_complex_from_parts(long double x, long double y) {
+      __pyx_t_long_double_complex z;
+      z.real = x;
+      z.imag = y;
+      return z;
+    }
+#endif
+
+/* Arithmetic */
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
+#else
+    static CYTHON_INLINE int __Pyx_c_eq_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+       return (a.real == b.real) && (a.imag == b.imag);
+    }
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_sum_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        __pyx_t_long_double_complex z;
+        z.real = a.real + b.real;
+        z.imag = a.imag + b.imag;
+        return z;
+    }
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_diff_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        __pyx_t_long_double_complex z;
+        z.real = a.real - b.real;
+        z.imag = a.imag - b.imag;
+        return z;
+    }
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_prod_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        __pyx_t_long_double_complex z;
+        z.real = a.real * b.real - a.imag * b.imag;
+        z.imag = a.real * b.imag + a.imag * b.real;
+        return z;
+    }
+    #if 1
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_quot_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        if (b.imag == 0) {
+            return __pyx_t_long_double_complex_from_parts(a.real / b.real, a.imag / b.real);
+        } else if (fabsl(b.real) >= fabsl(b.imag)) {
+            if (b.real == 0 && b.imag == 0) {
+                return __pyx_t_long_double_complex_from_parts(a.real / b.real, a.imag / b.imag);
+            } else {
+                long double r = b.imag / b.real;
+                long double s = (long double)(1.0) / (b.real + b.imag * r);
+                return __pyx_t_long_double_complex_from_parts(
+                    (a.real + a.imag * r) * s, (a.imag - a.real * r) * s);
+            }
+        } else {
+            long double r = b.real / b.imag;
+            long double s = (long double)(1.0) / (b.imag + b.real * r);
+            return __pyx_t_long_double_complex_from_parts(
+                (a.real * r + a.imag) * s, (a.imag * r - a.real) * s);
+        }
+    }
+    #else
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_quot_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        if (b.imag == 0) {
+            return __pyx_t_long_double_complex_from_parts(a.real / b.real, a.imag / b.real);
+        } else {
+            long double denom = b.real * b.real + b.imag * b.imag;
+            return __pyx_t_long_double_complex_from_parts(
+                (a.real * b.real + a.imag * b.imag) / denom,
+                (a.imag * b.real - a.real * b.imag) / denom);
+        }
+    }
+    #endif
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_neg_long__double(__pyx_t_long_double_complex a) {
+        __pyx_t_long_double_complex z;
+        z.real = -a.real;
+        z.imag = -a.imag;
+        return z;
+    }
+    static CYTHON_INLINE int __Pyx_c_is_zero_long__double(__pyx_t_long_double_complex a) {
+       return (a.real == 0) && (a.imag == 0);
+    }
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_conj_long__double(__pyx_t_long_double_complex a) {
+        __pyx_t_long_double_complex z;
+        z.real =  a.real;
+        z.imag = -a.imag;
+        return z;
+    }
+    #if 1
+        static CYTHON_INLINE long double __Pyx_c_abs_long__double(__pyx_t_long_double_complex z) {
+          #if !defined(HAVE_HYPOT) || defined(_MSC_VER)
+            return sqrtl(z.real*z.real + z.imag*z.imag);
+          #else
+            return hypotl(z.real, z.imag);
+          #endif
+        }
+        static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_pow_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+            __pyx_t_long_double_complex z;
+            long double r, lnr, theta, z_r, z_theta;
+            if (b.imag == 0 && b.real == (int)b.real) {
+                if (b.real < 0) {
+                    long double denom = a.real * a.real + a.imag * a.imag;
+                    a.real = a.real / denom;
+                    a.imag = -a.imag / denom;
+                    b.real = -b.real;
+                }
+                switch ((int)b.real) {
+                    case 0:
+                        z.real = 1;
+                        z.imag = 0;
+                        return z;
+                    case 1:
+                        return a;
+                    case 2:
+                        return __Pyx_c_prod_long__double(a, a);
+                    case 3:
+                        z = __Pyx_c_prod_long__double(a, a);
+                        return __Pyx_c_prod_long__double(z, a);
+                    case 4:
+                        z = __Pyx_c_prod_long__double(a, a);
+                        return __Pyx_c_prod_long__double(z, z);
+                }
+            }
+            if (a.imag == 0) {
+                if (a.real == 0) {
+                    return a;
+                } else if ((b.imag == 0) && (a.real >= 0)) {
+                    z.real = powl(a.real, b.real);
+                    z.imag = 0;
+                    return z;
+                } else if (a.real > 0) {
+                    r = a.real;
+                    theta = 0;
+                } else {
+                    r = -a.real;
+                    theta = atan2l(0.0, -1.0);
+                }
+            } else {
+                r = __Pyx_c_abs_long__double(a);
+                theta = atan2l(a.imag, a.real);
+            }
+            lnr = logl(r);
+            z_r = expl(lnr * b.real - theta * b.imag);
+            z_theta = theta * b.real + lnr * b.imag;
+            z.real = z_r * cosl(z_theta);
+            z.imag = z_r * sinl(z_theta);
+            return z;
+        }
+    #endif
+#endif
+
 /* MemviewSliceCopyTemplate */
   static __Pyx_memviewslice
 __pyx_memoryview_copy_new_contig(const __Pyx_memviewslice *from_mvs,
                                  const char *mode, int ndim,
                                  size_t sizeof_dtype, int contig_flag,
                                  int dtype_is_object)
 {
```

### Comparing `fastparquet-2024.2.0/fastparquet/speedups.pyx` & `fastparquet-2024.5.0/fastparquet/speedups.pyx`

 * *Files identical despite different names*

### Comparing `fastparquet-2024.2.0/fastparquet/util.py` & `fastparquet-2024.5.0/fastparquet/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from functools import lru_cache
 import io
 import struct
 import os
 import operator
 import re
 import numbers
+import zoneinfo
 
 import numpy as np
 import pandas as pd
 
 import fsspec
 
 from fastparquet import parquet_thrift
@@ -413,33 +414,36 @@
 
     if isinstance(dtype, pd.CategoricalDtype):
         extra_metadata = {
             'num_categories': len(column.cat.categories),
             'ordered': column.cat.ordered,
         }
         dtype = column.cat.codes.dtype
-    elif hasattr(dtype, 'tz'):
-        try:
-            stz = str(dtype.tz)
-            if "UTC" in stz and ":" in stz:
-                extra_metadata = {'timezone': stz.strip("UTC")}
-            elif len(str(stz)) == 3:  # like "UTC", "CET", ...
-                extra_metadata = {'timezone': str(stz)}
-            elif getattr(dtype.tz, "zone", False):
-                extra_metadata = {'timezone': dtype.tz.zone}
-            elif "pytz" not in stz:
-                pd.Series([pd.to_datetime('now', utc=True)]).dt.tz_localize(stz)
-                extra_metadata = {'timezone': stz}
-            elif "Offset" in stz:
-                extra_metadata = {'timezone': f"{dtype.tz._minutes // 60:+03}:00"}
-            else:
-                raise KeyError
-        except Exception as e:
-            raise ValueError("Time-zone information could not be serialised: "
-                             "%s, please use another" % str(dtype.tz)) from e
+    elif isinstance(dtype, pd.DatetimeTZDtype):
+        if isinstance(dtype.tz, zoneinfo.ZoneInfo):
+            extra_metadata = {'timezone': dtype.tz.key}
+        else:
+            try:
+                stz = str(dtype.tz)
+                if "UTC" in stz and ":" in stz:
+                    extra_metadata = {'timezone': stz.strip("UTC")}
+                elif len(str(stz)) == 3:  # like "UTC", "CET", ...
+                    extra_metadata = {'timezone': str(stz)}
+                elif getattr(dtype.tz, "zone", False):
+                    extra_metadata = {'timezone': dtype.tz.zone}
+                elif "pytz" not in stz:
+                    pd.Series([pd.to_datetime('now', utc=True)]).dt.tz_localize(stz)
+                    extra_metadata = {'timezone': stz}
+                elif "Offset" in stz:
+                    extra_metadata = {'timezone': f"{dtype.tz._minutes // 60:+03}:00"}
+                else:
+                    raise KeyError
+            except Exception as e:
+                raise ValueError("Time-zone information could not be serialised: "
+                                "%s, please use another" % str(dtype.tz)) from e
     else:
         extra_metadata = None
 
     if isinstance(name, tuple):
         name = str(name)
     elif not isinstance(name, str):
         raise TypeError(
```

### Comparing `fastparquet-2024.2.0/fastparquet/writer.py` & `fastparquet-2024.5.0/fastparquet/writer.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2024.2.0/fastparquet.egg-info/PKG-INFO` & `fastparquet-2024.5.0/fastparquet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: fastparquet
-Version: 2024.2.0
+Version: 2024.5.0
 Summary: Python support for Parquet file format
 Home-page: https://github.com/dask/fastparquet/
 Author: Martin Durant
 Author-email: mdurant@anaconda.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: pandas>=1.5.0
-Requires-Dist: numpy>=1.20.3
+Requires-Dist: numpy
 Requires-Dist: cramjam>=2.3
 Requires-Dist: fsspec
 Requires-Dist: packaging
 Provides-Extra: lzo
 Requires-Dist: python-lzo; extra == "lzo"
 
 fastparquet
```

### Comparing `fastparquet-2024.2.0/fastparquet.egg-info/SOURCES.txt` & `fastparquet-2024.5.0/fastparquet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastparquet-2024.2.0/setup.py` & `fastparquet-2024.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,36 +49,30 @@
 setup(
     name='fastparquet',
     use_scm_version={
         'version_scheme': 'guess-next-dev',
         'local_scheme': 'no-local-version',
         'write_to': 'fastparquet/_version.py'
     },
-    setup_requires=[
-        'setuptools>18.0',
-        'setuptools-scm>1.5.4',
-        'Cython',
-        'pytest-runner',
-        'oldest-supported-numpy'
-    ],
     description='Python support for Parquet file format',
     author='Martin Durant',
     author_email='mdurant@anaconda.com',
     url='https://github.com/dask/fastparquet/',
     license='Apache License 2.0',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython',
     ],
     packages=['fastparquet'],
     cmdclass={'build_ext': build_ext},
     install_requires=install_requires,
     extras_require={
         'lzo': ['python-lzo'],
@@ -86,10 +80,10 @@
     tests_require=[
         'pytest',
     ],
     long_description=(open('README.rst').read() if os.path.exists('README.rst')
                       else ''),
     include_package_data=True,
     exclude_package_data={'fastparquet': ['test/*']},
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     **extra
 )
```

