# Comparing `tmp/scalib-0.5.7.tar.gz` & `tmp/scalib-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalib-0.5.7.tar", last modified: Mon Mar 18 10:57:01 2024, max compression
+gzip compressed data, was "scalib-0.5.8.tar", last modified: Tue May 21 11:32:54 2024, max compression
```

## Comparing `scalib-0.5.7.tar` & `scalib-0.5.8.tar`

### file list

```diff
@@ -1,586 +1,590 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.509938 scalib-0.5.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.405938 scalib-0.5.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.417938 scalib-0.5.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-18 10:56:54.000000 scalib-0.5.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-18 10:56:54.000000 scalib-0.5.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-18 10:56:54.000000 scalib-0.5.7/.github/ISSUE_TEMPLATE/install_issue.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.417938 scalib-0.5.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-03-18 10:56:54.000000 scalib-0.5.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-18 10:56:54.000000 scalib-0.5.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-18 10:56:54.000000 scalib-0.5.7/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-03-18 10:56:54.000000 scalib-0.5.7/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-18 10:56:54.000000 scalib-0.5.7/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-03-18 10:56:54.000000 scalib-0.5.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-18 10:56:54.000000 scalib-0.5.7/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-18 10:56:54.000000 scalib-0.5.7/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-18 10:56:54.000000 scalib-0.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-18 10:56:54.000000 scalib-0.5.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-03-18 10:57:01.509938 scalib-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-03-18 10:56:54.000000 scalib-0.5.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.417938 scalib-0.5.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-18 10:56:54.000000 scalib-0.5.7/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.405938 scalib-0.5.7/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.417938 scalib-0.5.7/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-18 10:56:54.000000 scalib-0.5.7/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-18 10:56:54.000000 scalib-0.5.7/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-03-18 10:56:54.000000 scalib-0.5.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-03-18 10:56:54.000000 scalib-0.5.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-18 10:56:54.000000 scalib-0.5.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-18 10:56:54.000000 scalib-0.5.7/docs/refs.bib
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-18 10:56:54.000000 scalib-0.5.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.417938 scalib-0.5.7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-18 10:56:54.000000 scalib-0.5.7/docs/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-18 10:56:54.000000 scalib-0.5.7/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-18 10:56:54.000000 scalib-0.5.7/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-18 10:56:54.000000 scalib-0.5.7/docs/source/copyright.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-03-18 10:56:54.000000 scalib-0.5.7/docs/source/papers.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.421938 scalib-0.5.7/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-03-18 10:56:54.000000 scalib-0.5.7/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-03-18 10:56:54.000000 scalib-0.5.7/examples/aes_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-03-18 10:56:54.000000 scalib-0.5.7/examples/aes_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-03-18 10:56:54.000000 scalib-0.5.7/examples/aes_tvla.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-18 10:56:54.000000 scalib-0.5.7/examples/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-18 10:56:54.000000 scalib-0.5.7/examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.421938 scalib-0.5.7/paper/
--rwxr-xr-x   0 runner    (1001) docker     (127)      111 2024-03-18 10:56:54.000000 scalib-0.5.7/paper/build_paper.sh
--rw-r--r--   0 runner    (1001) docker     (127)     9313 2024-03-18 10:56:54.000000 scalib-0.5.7/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-03-18 10:56:54.000000 scalib-0.5.7/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-18 10:56:54.000000 scalib-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-18 10:57:01.509938 scalib-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-03-18 10:56:54.000000 scalib-0.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.409938 scalib-0.5.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.421938 scalib-0.5.7/src/scalib/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.421938 scalib-0.5.7/src/scalib/attacks/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib/attacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18815 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib/attacks/factor_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    24799 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib/attacks/sascagraph.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-18 10:57:01.000000 scalib-0.5.7/src/scalib/build_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.421938 scalib-0.5.7/src/scalib/config/
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib/config/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.425938 scalib-0.5.7/src/scalib/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib/metrics/information.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib/metrics/snr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib/metrics/ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.425938 scalib-0.5.7/src/scalib/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10804 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib/modeling/ldaclassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib/modeling/rldaclassifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.425938 scalib-0.5.7/src/scalib/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib/postprocessing/rankestimation.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-18 10:57:01.000000 scalib-0.5.7/src/scalib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.509938 scalib-0.5.7/src/scalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-03-18 10:57:01.000000 scalib-0.5.7/src/scalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27388 2024-03-18 10:57:01.000000 scalib-0.5.7/src/scalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 10:57:01.000000 scalib-0.5.7/src/scalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 10:57:01.000000 scalib-0.5.7/src/scalib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-18 10:57:01.000000 scalib-0.5.7/src/scalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-18 10:57:01.000000 scalib-0.5.7/src/scalib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.425938 scalib-0.5.7/src/scalib_ext/
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    45613 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.425938 scalib-0.5.7/src/scalib_ext/geigen/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.425938 scalib-0.5.7/src/scalib_ext/geigen/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.429938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/Cholesky
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/CholmodSupport
--rw-r--r--   0 runner    (1001) docker     (127)    18103 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/Core
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/Dense
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/Eigen
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/Eigenvalues
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/Geometry
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/Householder
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/IterativeLinearSolvers
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/Jacobi
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/LU
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/MetisSupport
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/OrderingMethods
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/PaStiXSupport
--rwxr-xr-x   0 runner    (1001) docker     (127)     1116 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/PardisoSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/QR
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/QtAlignedMalloc
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/SPQRSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/SVD
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/Sparse
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/SparseCholesky
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/SparseCore
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/SparseLU
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/SparseQR
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/StdDeque
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/StdList
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/StdVector
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/SuperLUSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/UmfPackSupport
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.413938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.429938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Cholesky/
--rw-r--r--   0 runner    (1001) docker     (127)    24480 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0 runner    (1001) docker     (127)    18395 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.429938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    22307 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.441938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/
--rw-r--r--   0 runner    (1001) docker     (127)    12115 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Array.h
--rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Assign.h
--rw-r--r--   0 runner    (1001) docker     (127)    38153 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/AssignEvaluator.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    12479 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 runner    (1001) docker     (127)    13910 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    18064 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Block.h
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 runner    (1001) docker     (127)    62197 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)    31424 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 runner    (1001) docker     (127)    27551 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    24212 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    22205 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 runner    (1001) docker     (127)    12666 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)    11507 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Dot.h
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 runner    (1001) docker     (127)    21123 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/IO.h
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Inverse.h
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Map.h
--rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/MapBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    41000 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    19067 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    23276 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 runner    (1001) docker     (127)    20694 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    45354 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Product.h
--rw-r--r--   0 runner    (1001) docker     (127)    51070 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Random.h
--rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Redux.h
--rw-r--r--   0 runner    (1001) docker     (127)    12844 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Ref.h
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Replicate.h
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Reverse.h
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Select.h
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Solve.h
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Stride.h
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Swap.h
--rw-r--r--   0 runner    (1001) docker     (127)    14856 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Transpose.h
--rw-r--r--   0 runner    (1001) docker     (127)    13092 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 runner    (1001) docker     (127)    37304 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 runner    (1001) docker     (127)    29441 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.409938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.445938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 runner    (1001) docker     (127)    18037 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)    17776 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    27841 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.445938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 runner    (1001) docker     (127)    15528 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    50865 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.445938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 runner    (1001) docker     (127)    16443 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    37671 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.445938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)    23547 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Half.h
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)    35476 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.445938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/Settings.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.445938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 runner    (1001) docker     (127)    17706 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    28726 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.449938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 runner    (1001) docker     (127)    19426 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)    18888 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    35843 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.449938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 runner    (1001) docker     (127)    15366 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    32283 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.449938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/functors/
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)    18263 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)    27946 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.453938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/
--rw-r--r--   0 runner    (1001) docker     (127)    81646 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (127)    18887 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)    26808 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 runner    (1001) docker     (127)    20103 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 runner    (1001) docker     (127)    20879 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)    14540 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.457938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/
--rwxr-xr-x   0 runner    (1001) docker     (127)    19307 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 runner    (1001) docker     (127)    21579 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/Constants.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     4360 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (127)    14094 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/ForwardDeclarations.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     4026 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 runner    (1001) docker     (127)    38322 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 runner    (1001) docker     (127)    40579 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/Memory.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    21356 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 runner    (1001) docker     (127)    34903 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.457938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/
--rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    17273 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    22944 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     9715 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0 runner    (1001) docker     (127)    23586 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0 runner    (1001) docker     (127)    20749 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    33705 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    22444 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.461938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/
--rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0 runner    (1001) docker     (127)    20539 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0 runner    (1001) docker     (127)    32704 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/RotationBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0 runner    (1001) docker     (127)    60555 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/Transform.h
--rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/Translation.h
--rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/Umeyama.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.461938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/Geometry_SSE.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.461938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Householder/
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Householder/Householder.h
--rw-r--r--   0 runner    (1001) docker     (127)    20603 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Householder/HouseholderSequence.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.465938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0 runner    (1001) docker     (127)     7253 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (127)    15062 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.465938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Jacobi/
--rw-r--r--   0 runner    (1001) docker     (127)    15902 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Jacobi/Jacobi.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.465938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/LU/
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/LU/Determinant.h
--rw-r--r--   0 runner    (1001) docker     (127)    32803 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0 runner    (1001) docker     (127)    15064 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    21538 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.465938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/LU/arch/
--rw-r--r--   0 runner    (1001) docker     (127)    13662 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/LU/arch/Inverse_SSE.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.465938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/MetisSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.465938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/
--rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0 runner    (1001) docker     (127)    62266 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Ordering.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.465938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    22248 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.465938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    20060 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.469938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/QR/
--rw-r--r--   0 runner    (1001) docker     (127)    24881 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    20805 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (127)    25478 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (127)    14022 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.469938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.469938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SVD/
--rw-r--r--   0 runner    (1001) docker     (127)    49870 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0 runner    (1001) docker     (127)    32949 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SVD/UpperBidiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.469938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/
--rw-r--r--   0 runner    (1001) docker     (127)    24017 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.473938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0 runner    (1001) docker     (127)    25592 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    25840 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0 runner    (1001) docker     (127)    52401 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    17923 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0 runner    (1001) docker     (127)    25721 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0 runner    (1001) docker     (127)    14831 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/TriangularSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.477938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/
--rw-r--r--   0 runner    (1001) docker     (127)    27844 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.477938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseQR/
--rw-r--r--   0 runner    (1001) docker     (127)    28373 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseQR/SparseQR.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.477938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/StlSupport/
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/StlSupport/details.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.477938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    34345 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.477938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.481938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/misc/Image.h
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/misc/Kernel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0 runner    (1001) docker     (127)    30560 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/misc/blas.h
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/misc/lapack.h
--rwxr-xr-x   0 runner    (1001) docker     (127)  1058368 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke.h
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke_mangling.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.485938 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)    16929 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)    37403 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.485938 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/DavidsonSymEigsSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    18186 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/GenEigsBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/GenEigsComplexShiftSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/GenEigsRealShiftSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/GenEigsSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/JDSymEigsBase.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.485938 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/
--rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/Arnoldi.h
--rw-r--r--   0 runner    (1001) docker     (127)    17496 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/BKLDLT.h
--rw-r--r--   0 runner    (1001) docker     (127)    14768 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/DoubleShiftQR.h
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/Lanczos.h
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/Orthogonalization.h
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/RitzPairs.h
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/SearchSpace.h
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/TridiagEigen.h
--rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergEigen.h
--rw-r--r--   0 runner    (1001) docker     (127)    28001 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergQR.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.489938 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/DenseCholesky.h
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenComplexShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenMatProd.h
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenRealShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymMatProd.h
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/SparseCholesky.h
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenComplexShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenMatProd.h
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenRealShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/SparseRegularInverse.h
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymMatProd.h
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/SymShiftInvert.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.489938 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/internal/
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/internal/ArnoldiOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsBucklingOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCayleyOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCholeskyOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsRegInvOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsShiftInvertOp.h
--rw-r--r--   0 runner    (1001) docker     (127)    15129 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/SymEigsBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/SymEigsShiftSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/SymEigsSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    21455 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/SymGEigsShiftSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    13190 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/SymGEigsSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.493938 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/Util/
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/Util/CompInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/Util/GEigsMode.h
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/Util/SelectionRule.h
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/Util/SimpleRandom.h
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/Util/TypeTraits.h
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/Util/Version.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.493938 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)    19212 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/contrib/LOBPCGSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/contrib/PartialSVDSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/include/geigen.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.493938 scalib-0.5.7/src/scalib_ext/geigen/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/src/geigen.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/src/geigen.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/geigen/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.493938 scalib-0.5.7/src/scalib_ext/ranklib/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.493938 scalib-0.5.7/src/scalib_ext/ranklib/fuzz/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/fuzz/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/fuzz/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.493938 scalib-0.5.7/src/scalib_ext/ranklib/fuzz/fuzz_targets/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/fuzz/fuzz_targets/rank2vsnaive_2.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.497938 scalib-0.5.7/src/scalib_ext/ranklib/src/
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/aes.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/aes.h
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/bignumpoly.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/bignumpoly.h
--rw-r--r--   0 runner    (1001) docker     (127)    22744 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/hel_enum.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/hel_enum.h
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/hel_execute.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/hel_execute.h
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/hel_histo.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/hel_histo.h
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/hel_if.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/hel_if.h
--rw-r--r--   0 runner    (1001) docker     (127)    15653 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/hel_init.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/hel_init.h
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/hel_struct.h
--rw-r--r--   0 runner    (1001) docker     (127)    10066 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/hel_util.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/hel_util.h
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/histogram.rs
--rw-r--r--   0 runner    (1001) docker     (127)    13628 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    16237 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/main_example.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/rank.rs
--rw-r--r--   0 runner    (1001) docker     (127)   274225 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/score_example_data.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/scores_example.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/scores_example.h
--rw-r--r--   0 runner    (1001) docker     (127)   224884 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/scores_example_data.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/ranklib/src/top.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.497938 scalib-0.5.7/src/scalib_ext/scalib/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.501938 scalib-0.5.7/src/scalib_ext/scalib/benches/
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/benches/belief_propagation.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/benches/get_snr.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/benches/mttest.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/benches/snr_update.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/benches/ttest.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.505938 scalib-0.5.7/src/scalib_ext/scalib/src/
--rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/src/belief_propagation.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/src/information.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10955 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/src/lda.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/src/matrixmul.rs
--rw-r--r--   0 runner    (1001) docker     (127)    25696 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/src/mttest.rs
--rw-r--r--   0 runner    (1001) docker     (127)    30804 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/src/rlda.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.505938 scalib-0.5.7/src/scalib_ext/scalib/src/sasca/
--rw-r--r--   0 runner    (1001) docker     (127)    37584 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/src/sasca/belief_propagation.rs
--rw-r--r--   0 runner    (1001) docker     (127)    24567 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/src/sasca/bp_compute.rs
--rw-r--r--   0 runner    (1001) docker     (127)    19393 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/src/sasca/factor_graph.rs
--rw-r--r--   0 runner    (1001) docker     (127)    15051 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/src/sasca/fg_build.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/src/sasca/fg_parser.rs
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/src/sasca/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/src/snr.rs
--rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/src/ttest.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/src/utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.505938 scalib-0.5.7/src/scalib_ext/scalib/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/tests/lda.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/tests/multivarcs.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib/tests/ttest.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.497938 scalib-0.5.7/src/scalib_ext/scalib-py/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib-py/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.501938 scalib-0.5.7/src/scalib_ext/scalib-py/src/
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib-py/src/belief_propagation.rs
--rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib-py/src/factor_graph.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib-py/src/information.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib-py/src/lda.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib-py/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib-py/src/ranking.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib-py/src/rlda.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib-py/src/snr.rs
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib-py/src/thread_pool.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-03-18 10:56:54.000000 scalib-0.5.7/src/scalib_ext/scalib-py/src/ttest.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:57:01.505938 scalib-0.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-18 10:56:54.000000 scalib-0.5.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-03-18 10:56:54.000000 scalib-0.5.7/tests/mttest_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-18 10:56:54.000000 scalib-0.5.7/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    41344 2024-03-18 10:56:54.000000 scalib-0.5.7/tests/test_factorgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-03-18 10:56:54.000000 scalib-0.5.7/tests/test_lda.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-18 10:56:54.000000 scalib-0.5.7/tests/test_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-03-18 10:56:54.000000 scalib-0.5.7/tests/test_rlda.py
--rw-r--r--   0 runner    (1001) docker     (127)    12334 2024-03-18 10:56:54.000000 scalib-0.5.7/tests/test_sascagraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-03-18 10:56:54.000000 scalib-0.5.7/tests/test_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-18 10:56:54.000000 scalib-0.5.7/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-03-18 10:56:54.000000 scalib-0.5.7/tests/test_ttest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-18 10:56:54.000000 scalib-0.5.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.622439 scalib-0.5.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.534439 scalib-0.5.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.542439 scalib-0.5.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-21 11:32:47.000000 scalib-0.5.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-21 11:32:47.000000 scalib-0.5.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-21 11:32:47.000000 scalib-0.5.8/.github/ISSUE_TEMPLATE/install_issue.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.542439 scalib-0.5.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-21 11:32:47.000000 scalib-0.5.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-21 11:32:47.000000 scalib-0.5.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-21 11:32:47.000000 scalib-0.5.8/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-05-21 11:32:47.000000 scalib-0.5.8/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-21 11:32:47.000000 scalib-0.5.8/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-05-21 11:32:47.000000 scalib-0.5.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-21 11:32:47.000000 scalib-0.5.8/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-21 11:32:47.000000 scalib-0.5.8/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-21 11:32:47.000000 scalib-0.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-21 11:32:47.000000 scalib-0.5.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-05-21 11:32:54.622439 scalib-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-05-21 11:32:47.000000 scalib-0.5.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.546439 scalib-0.5.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-21 11:32:47.000000 scalib-0.5.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.534439 scalib-0.5.8/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.546439 scalib-0.5.8/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-21 11:32:47.000000 scalib-0.5.8/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 11:32:47.000000 scalib-0.5.8/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-21 11:32:47.000000 scalib-0.5.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-21 11:32:47.000000 scalib-0.5.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-21 11:32:47.000000 scalib-0.5.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-21 11:32:47.000000 scalib-0.5.8/docs/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-21 11:32:47.000000 scalib-0.5.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.546439 scalib-0.5.8/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-21 11:32:47.000000 scalib-0.5.8/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 11:32:47.000000 scalib-0.5.8/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 11:32:47.000000 scalib-0.5.8/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 11:32:47.000000 scalib-0.5.8/docs/source/copyright.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-21 11:32:47.000000 scalib-0.5.8/docs/source/papers.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.546439 scalib-0.5.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-21 11:32:47.000000 scalib-0.5.8/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-21 11:32:47.000000 scalib-0.5.8/examples/aes_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-21 11:32:47.000000 scalib-0.5.8/examples/aes_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-21 11:32:47.000000 scalib-0.5.8/examples/aes_tvla.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-21 11:32:47.000000 scalib-0.5.8/examples/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-21 11:32:47.000000 scalib-0.5.8/examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.546439 scalib-0.5.8/paper/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      111 2024-05-21 11:32:47.000000 scalib-0.5.8/paper/build_paper.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     9313 2024-05-21 11:32:47.000000 scalib-0.5.8/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-21 11:32:47.000000 scalib-0.5.8/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-21 11:32:47.000000 scalib-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-21 11:32:54.622439 scalib-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-21 11:32:47.000000 scalib-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.534439 scalib-0.5.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.546439 scalib-0.5.8/src/scalib/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.550439 scalib-0.5.8/src/scalib/attacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/attacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18815 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/attacks/factor_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24799 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/attacks/sascagraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 11:32:54.000000 scalib-0.5.8/src/scalib/build_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.550439 scalib-0.5.8/src/scalib/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/config/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.550439 scalib-0.5.8/src/scalib/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/metrics/information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/metrics/snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/metrics/ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.550439 scalib-0.5.8/src/scalib/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10804 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/modeling/ldaclassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/modeling/rldaclassifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.550439 scalib-0.5.8/src/scalib/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/postprocessing/rankestimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.550439 scalib-0.5.8/src/scalib/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/preprocessing/quantization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-21 11:32:54.000000 scalib-0.5.8/src/scalib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.622439 scalib-0.5.8/src/scalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-05-21 11:32:54.000000 scalib-0.5.8/src/scalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27490 2024-05-21 11:32:54.000000 scalib-0.5.8/src/scalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:32:54.000000 scalib-0.5.8/src/scalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:32:54.000000 scalib-0.5.8/src/scalib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 11:32:54.000000 scalib-0.5.8/src/scalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 11:32:54.000000 scalib-0.5.8/src/scalib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.550439 scalib-0.5.8/src/scalib_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    43514 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.550439 scalib-0.5.8/src/scalib_ext/geigen/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.550439 scalib-0.5.8/src/scalib_ext/geigen/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.558439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/Cholesky
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/CholmodSupport
+-rw-r--r--   0 runner    (1001) docker     (127)    18103 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/Core
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/Dense
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/Eigen
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/Eigenvalues
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/Geometry
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/Householder
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/Jacobi
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/LU
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/MetisSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/OrderingMethods
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/PaStiXSupport
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1116 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/PardisoSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/QR
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/QtAlignedMalloc
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/SPQRSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/SVD
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/Sparse
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/SparseCholesky
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/SparseCore
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/SparseLU
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/SparseQR
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/StdDeque
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/StdList
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/StdVector
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/SuperLUSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/UmfPackSupport
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.538439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.558439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Cholesky/
+-rw-r--r--   0 runner    (1001) docker     (127)    24480 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18395 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.558439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    22307 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.566439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/
+-rw-r--r--   0 runner    (1001) docker     (127)    12115 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Assign.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38153 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/AssignEvaluator.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12479 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13910 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18064 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Block.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    62197 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31424 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27551 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24212 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22205 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12666 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11507 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Dot.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21123 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/IO.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Map.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    41000 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19067 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23276 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20694 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    45354 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Product.h
+-rw-r--r--   0 runner    (1001) docker     (127)    51070 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Random.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Redux.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12844 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Ref.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Select.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Stride.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Swap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14856 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13092 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37304 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29441 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.534439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.570439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (127)    18037 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17776 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27841 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.570439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (127)    15528 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    50865 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.570439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 runner    (1001) docker     (127)    16443 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37671 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.570439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23547 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Half.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35476 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.570439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/Settings.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.570439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (127)    17706 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28726 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.570439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 runner    (1001) docker     (127)    19426 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18888 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35843 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.574439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 runner    (1001) docker     (127)    15366 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32283 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.574439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/functors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18263 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27946 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.578439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/
+-rw-r--r--   0 runner    (1001) docker     (127)    81646 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18887 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26808 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20103 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20879 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14540 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.578439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19307 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21579 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/Constants.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4360 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14094 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/ForwardDeclarations.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4026 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38322 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40579 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/Memory.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21356 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34903 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.582439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17273 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22944 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9715 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23586 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20749 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    33705 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22444 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.582439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20539 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32704 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 runner    (1001) docker     (127)    60555 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.582439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/Geometry_SSE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.582439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Householder/
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20603 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.586439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7253 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15062 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.586439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Jacobi/
+-rw-r--r--   0 runner    (1001) docker     (127)    15902 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.586439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/LU/
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32803 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15064 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21538 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.586439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/LU/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)    13662 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/LU/arch/Inverse_SSE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.586439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.586439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/
+-rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 runner    (1001) docker     (127)    62266 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.586439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    22248 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.586439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    20060 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.590439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/QR/
+-rw-r--r--   0 runner    (1001) docker     (127)    24881 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20805 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25478 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14022 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.590439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.590439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SVD/
+-rw-r--r--   0 runner    (1001) docker     (127)    49870 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32949 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.590439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/
+-rw-r--r--   0 runner    (1001) docker     (127)    24017 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.594439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25592 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25840 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    52401 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17923 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25721 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14831 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.598439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/
+-rw-r--r--   0 runner    (1001) docker     (127)    27844 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.598439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseQR/
+-rw-r--r--   0 runner    (1001) docker     (127)    28373 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.598439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/StlSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.598439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    34345 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.598439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.602439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/misc/Image.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30560 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/misc/blas.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/misc/lapack.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1058368 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.602439 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16929 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37403 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.602439 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/DavidsonSymEigsSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18186 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/GenEigsBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/GenEigsComplexShiftSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/GenEigsRealShiftSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/GenEigsSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/JDSymEigsBase.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.606439 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/
+-rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/Arnoldi.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17496 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/BKLDLT.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14768 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/DoubleShiftQR.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/Lanczos.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/Orthogonalization.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/RitzPairs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/SearchSpace.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/TridiagEigen.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergEigen.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28001 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergQR.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.606439 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/DenseCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenComplexShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenMatProd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenRealShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymMatProd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/SparseCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenComplexShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenMatProd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenRealShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/SparseRegularInverse.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymMatProd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/SymShiftInvert.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.610439 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/internal/ArnoldiOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsBucklingOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCayleyOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCholeskyOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsRegInvOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsShiftInvertOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15129 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/SymEigsBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/SymEigsShiftSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/SymEigsSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21455 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/SymGEigsShiftSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13190 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/SymGEigsSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.610439 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/Util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/Util/CompInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/Util/GEigsMode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/Util/SelectionRule.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/Util/SimpleRandom.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/Util/TypeTraits.h
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/Util/Version.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.610439 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)    19212 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/contrib/LOBPCGSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/contrib/PartialSVDSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/include/geigen.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.610439 scalib-0.5.8/src/scalib_ext/geigen/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/src/geigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/src/geigen.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/geigen/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.610439 scalib-0.5.8/src/scalib_ext/ranklib/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.610439 scalib-0.5.8/src/scalib_ext/ranklib/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/fuzz/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/fuzz/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.610439 scalib-0.5.8/src/scalib_ext/ranklib/fuzz/fuzz_targets/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/fuzz/fuzz_targets/rank2vsnaive_2.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.614439 scalib-0.5.8/src/scalib_ext/ranklib/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/aes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/aes.h
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/bignumpoly.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/bignumpoly.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22744 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/hel_enum.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/hel_enum.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/hel_execute.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/hel_execute.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/hel_histo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/hel_histo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/hel_if.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/hel_if.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15653 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/hel_init.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/hel_init.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/hel_struct.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10066 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/hel_util.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/hel_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/histogram.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    13628 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16237 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/main_example.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/rank.rs
+-rw-r--r--   0 runner    (1001) docker     (127)   274225 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/score_example_data.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/scores_example.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/scores_example.h
+-rw-r--r--   0 runner    (1001) docker     (127)   224884 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/scores_example_data.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/ranklib/src/top.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.614439 scalib-0.5.8/src/scalib_ext/scalib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.618439 scalib-0.5.8/src/scalib_ext/scalib/benches/
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/benches/belief_propagation.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/benches/get_snr.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/benches/mttest.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/benches/snr_update.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/benches/ttest.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.618439 scalib-0.5.8/src/scalib_ext/scalib/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/src/belief_propagation.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/src/information.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10955 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/src/lda.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/src/matrixmul.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    25696 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/src/mttest.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    30804 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/src/rlda.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.622439 scalib-0.5.8/src/scalib_ext/scalib/src/sasca/
+-rw-r--r--   0 runner    (1001) docker     (127)    37723 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/src/sasca/belief_propagation.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    24567 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/src/sasca/bp_compute.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/src/sasca/factor_graph.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    15368 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/src/sasca/fg_build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/src/sasca/fg_parser.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/src/sasca/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/src/snr.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/src/ttest.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/src/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.622439 scalib-0.5.8/src/scalib_ext/scalib/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/tests/lda.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/tests/multivarcs.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib/tests/ttest.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.614439 scalib-0.5.8/src/scalib_ext/scalib-py/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib-py/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.618439 scalib-0.5.8/src/scalib_ext/scalib-py/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib-py/src/belief_propagation.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib-py/src/factor_graph.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib-py/src/information.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib-py/src/lda.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib-py/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib-py/src/ranking.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib-py/src/rlda.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib-py/src/snr.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib-py/src/thread_pool.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-21 11:32:47.000000 scalib-0.5.8/src/scalib_ext/scalib-py/src/ttest.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:32:54.622439 scalib-0.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-21 11:32:47.000000 scalib-0.5.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-21 11:32:47.000000 scalib-0.5.8/tests/mttest_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-21 11:32:47.000000 scalib-0.5.8/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    43153 2024-05-21 11:32:47.000000 scalib-0.5.8/tests/test_factorgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-21 11:32:47.000000 scalib-0.5.8/tests/test_lda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-21 11:32:47.000000 scalib-0.5.8/tests/test_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-21 11:32:47.000000 scalib-0.5.8/tests/test_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-21 11:32:47.000000 scalib-0.5.8/tests/test_rlda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12334 2024-05-21 11:32:47.000000 scalib-0.5.8/tests/test_sascagraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-21 11:32:47.000000 scalib-0.5.8/tests/test_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-21 11:32:47.000000 scalib-0.5.8/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-21 11:32:47.000000 scalib-0.5.8/tests/test_ttest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-21 11:32:47.000000 scalib-0.5.8/tox.ini
```

### Comparing `scalib-0.5.7/.github/ISSUE_TEMPLATE/bug_report.md` & `scalib-0.5.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/.github/ISSUE_TEMPLATE/feature_request.md` & `scalib-0.5.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/.github/ISSUE_TEMPLATE/install_issue.md` & `scalib-0.5.8/.github/ISSUE_TEMPLATE/install_issue.md`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/.github/workflows/ci.yml` & `scalib-0.5.8/.github/workflows/ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
               with:
                   path: |
                       ${{ runner.temp }}/cargo_build
                       ${{ runner.temp }}/cargo_home
                   key: linux-wheel-cache-rust-build-cargo-v1-${{ matrix.arch}}
             - uses: actions/setup-python@v3
               with:
-                  python-version: "3.8"
+                  python-version: "3.9"
             - name: wheels Linux ${{ matrix.arch }}
               uses: pypa/cibuildwheel@v2.16.5
               env:
                 CARGO_TARGET_DIR: "/host${{ runner.temp }}/cargo_build"
                 CARGO_HOME: "/host${{ runner.temp }}/cargo_home"
                 CIBW_PLATFORM: "linux"
             - uses: actions/upload-artifact@v3
@@ -62,15 +62,15 @@
     test:
         name: Run tests (on linux).
         needs: [build_wheel_linux]
         runs-on: ubuntu-latest
         strategy:
             fail-fast: false
             matrix:
-                python: ["3.8", "3.12"]
+                python: ["3.9", "3.12"]
         steps:
             - uses: actions/checkout@v3
             - uses: actions/download-artifact@v3
               with:
                   name: dist
                   path: dist
             - name: Setup Python
@@ -123,15 +123,15 @@
               with:
                   path: |
                       ${{ runner.temp }}/cargo_build
                       ${{ runner.temp }}/cargo_home
                   key: windows-wheel-cache-rust-build-cargo-v1-${{ matrix.arch}}
             - uses: actions/setup-python@v3
               with:
-                  python-version: "3.8"
+                  python-version: "3.9"
             - name: wheels Windows ${{ matrix.arch}}
               uses: pypa/cibuildwheel@v2.16.5
               env:
                 CARGO_TARGET_DIR: "${{ runner.temp }}\\cargo_build"
                 CARGO_HOME: "${{ runner.temp }}\\cargo_home"
                 CIBW_PLATFORM: "windows"
                 CIBW_TEST_COMMAND: pytest {project}/tests
@@ -139,35 +139,35 @@
             - uses: actions/upload-artifact@v3
               with:
                   name: dist
                   path: ./wheelhouse/*.whl
 
     build_wheel_macos:
         name: Build wheels on Mac Os (${{ matrix.vers }})
-        runs-on: macos-latest
+        # macos-13 is on x86_64 and macos-14 is on arm64
+        runs-on: ${{ matrix.os }}
         strategy:
             fail-fast: false
             matrix:
                 include:
                    - vers: arm64
+                     os: macos-14
                    - vers: x86_64
+                     os: macos-13
         steps:
             - uses: actions/checkout@v3
             - uses: actions/cache@v3
               with:
                   path: |
                       ${{ runner.temp }}/cargo_build
                       ${{ runner.temp }}/cargo_home
                   key: macos-wheel-cache-rust-build-cargo-v1-${{ matrix.arch}}
             - uses: actions/setup-python@v3
               with:
-                  python-version: "3.8"
-            - name: add aarch64 lib
-              if: ${{ matrix.vers }} == 'arm64'
-              run: "rustup target add aarch64-apple-darwin"
+                  python-version: "3.9"
             - name: wheels Mac Os ${{ matrix.vers }}
               uses: pypa/cibuildwheel@v2.16.5
               env:
                 CARGO_TARGET_DIR: "${{ runner.temp }}\\cargo_build"
                 CARGO_HOME: "${{ runner.temp }}\\cargo_home"
                 CIBW_PLATFORM: "macos"
                 CIBW_TEST_COMMAND: pytest {project}/tests
```

### Comparing `scalib-0.5.7/CHANGELOG.rst` & `scalib-0.5.8/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 =========
 Changelog
 =========
 
 Not released
 ------------
 
+v0.5.8 (2024/05/21)
+-------------------
+* Add ``scalib.preprocessing.Quantizer`` for conversions of floating-point
+  traces to int.
+* Support modular subtractions (generalized summation) in FactorGraph.
+* Raise minimum supported python version to 3.9.
+
 v0.5.7 (2024/03/18)
 -------------------
 
 * ``scalib.attacks.FactorGraph``:
 
     * Add ``GENERIC`` factors
```

### Comparing `scalib-0.5.7/CITATION.cff` & `scalib-0.5.8/CITATION.cff`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/CONTRIBUTING.rst` & `scalib-0.5.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/COPYING` & `scalib-0.5.8/COPYING`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/COPYRIGHT` & `scalib-0.5.8/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/MANIFEST.in` & `scalib-0.5.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/Makefile` & `scalib-0.5.8/Makefile`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/PKG-INFO` & `scalib-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: scalib
-Version: 0.5.7
+Version: 0.5.8
 Summary: Side-Channel Analysis Library
 Home-page: https://github.com/simple-crypto/scalib
 Author: Olivier Bronchain, Gaëtan Cassiers
 Author-email: olivier.bronchain@uclouvain.be, gaetan.cassiers@uclouvain.be
 License: GNU AGPL v3+
 Project-URL: Bug Tracker, https://github.com/simple-crypto/scalib/issues
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: COPYING
-Requires-Dist: numpy~=1.19
+Requires-Dist: numpy~=1.21
 Requires-Dist: py-cpuinfo~=9.0
 
 ======
 SCALib
 ======
 
 .. image:: https://badge.fury.io/py/scalib.svg
```

### Comparing `scalib-0.5.7/README.rst` & `scalib-0.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/docs/Makefile` & `scalib-0.5.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/docs/_templates/autosummary/class.rst` & `scalib-0.5.8/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/docs/_templates/autosummary/module.rst` & `scalib-0.5.8/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/docs/conf.py` & `scalib-0.5.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/docs/index.rst` & `scalib-0.5.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/docs/make.bat` & `scalib-0.5.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/docs/refs.bib` & `scalib-0.5.8/docs/refs.bib`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/docs/source/papers.rst` & `scalib-0.5.8/docs/source/papers.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/examples/README.rst` & `scalib-0.5.8/examples/README.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/examples/aes_attack.py` & `scalib-0.5.8/examples/aes_attack.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/examples/aes_info.py` & `scalib-0.5.8/examples/aes_info.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/examples/aes_tvla.py` & `scalib-0.5.8/examples/aes_tvla.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/examples/utils.py` & `scalib-0.5.8/examples/utils.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/paper/paper.bib` & `scalib-0.5.8/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/paper/paper.md` & `scalib-0.5.8/paper/paper.md`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/pyproject.toml` & `scalib-0.5.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,27 @@
 [build-system]
 requires = [
     "setuptools>=62.4",
-     "setuptools-scm[toml]>=3.4",
-     "setuptools-scm-git-archive",
+    "setuptools-scm[toml]>=3.4",
+    "setuptools-scm-git-archive",
     "wheel",
     "setuptools-rust>=1.6",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "src/scalib/version.py"
 
 [tool.pytest.ini_options]
-addopts = [
-    "--cov=scalib",
-    "--doctest-modules",
-    "-ra",
-    "--pyargs",
-]
-testpaths = [
-    "tests",
-    "scalib",
-    "examples",
-]
+addopts = ["--cov=scalib", "--doctest-modules", "-ra", "--pyargs"]
+testpaths = ["tests", "scalib", "examples"]
 
 [tool.cibuildwheel]
 manylinux-x86_64-image = "ghcr.io/simple-crypto/manylinux2014_x86_64-clang:rust-1.66.1"
-build-verbosity = "1"
-build = [
-    "cp38-*",
-]
-skip = [
-    "*musllinux*",
-]
+build-verbosity = 1
+build = ["cp39-*"]
+skip = ["*musllinux*"]
 archs = "auto64"
-environment-pass = [
-    "CARGO_TARGET_DIR",
-    "CARGO_HOME",
-]
+environment-pass = ["CARGO_TARGET_DIR", "CARGO_HOME"]
 [tool.cibuildwheel.environment]
-RUST_BACKTRACE="full"
-SCALIB_AVX2="1"
+RUST_BACKTRACE = "full"
+SCALIB_AVX2 = "1"
```

### Comparing `scalib-0.5.7/setup.cfg` & `scalib-0.5.8/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 license_files = COPYING
 
 [options]
 package_dir = 
 	=src
 packages = find:
 zip_safe = False
-python_requires = >=3.8
+python_requires = >=3.9
 install_requires = 
-	numpy~=1.19
+	numpy~=1.21
 	py-cpuinfo~=9.0
 
 [options.packages.find]
 where = src
 
 [coverage:report]
 exclude_lines = 
@@ -29,13 +29,13 @@
 	raise AssertionError
 	raise NotImplementedError
 	def main\(.*\):
 	pragma: py{ignore_python_version}
 	def _ipython_key_completions_
 
 [bdist_wheel]
-py-limited-api = cp38
+py-limited-api = cp39
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `scalib-0.5.7/setup.py` & `scalib-0.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib/__init__.py` & `scalib-0.5.8/src/scalib/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 __all__ = [
+    "preprocessing",
     "config",
     "attacks",
     "metrics",
     "modeling",
     "postprocessing",
     "tools",
     "ScalibError",
```

### Comparing `scalib-0.5.7/src/scalib/attacks/__init__.py` & `scalib-0.5.8/src/scalib/attacks/__init__.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib/attacks/factor_graph.py` & `scalib-0.5.8/src/scalib/attacks/factor_graph.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib/attacks/sascagraph.py` & `scalib-0.5.8/src/scalib/attacks/sascagraph.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib/config/__init__.py` & `scalib-0.5.8/src/scalib/config/__init__.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib/config/threading.py` & `scalib-0.5.8/src/scalib/config/threading.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib/metrics/information.py` & `scalib-0.5.8/src/scalib/metrics/information.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     References
     ----------
 
     .. footbibliography::
     """
 
     def __init__(self, model: RLDAClassifier.ClusteredModel, max_popped_classes: int):
-        """
+        r"""
         Parameters
         ----------
         model
             The clustered model, it is obtained by calling `get_clustered_model()` on an RLDA object.
         max_popped_classes
             Number of classes that are calculated without using the associated cluster. Corresponds to parameter :math:`\zeta` in :footcite:p:`RLDA`.
         """
```

### Comparing `scalib-0.5.7/src/scalib/metrics/snr.py` & `scalib-0.5.8/src/scalib/metrics/snr.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib/metrics/ttest.py` & `scalib-0.5.8/src/scalib/metrics/ttest.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib/modeling/__init__.py` & `scalib-0.5.8/src/scalib/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib/modeling/ldaclassifier.py` & `scalib-0.5.8/src/scalib/modeling/ldaclassifier.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib/modeling/rldaclassifier.py` & `scalib-0.5.8/src/scalib/modeling/rldaclassifier.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib/postprocessing/rankestimation.py` & `scalib-0.5.8/src/scalib/postprocessing/rankestimation.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib/tools.py` & `scalib-0.5.8/src/scalib/tools.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib/utils.py` & `scalib-0.5.8/src/scalib/utils.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib.egg-info/PKG-INFO` & `scalib-0.5.8/src/scalib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: scalib
-Version: 0.5.7
+Version: 0.5.8
 Summary: Side-Channel Analysis Library
 Home-page: https://github.com/simple-crypto/scalib
 Author: Olivier Bronchain, Gaëtan Cassiers
 Author-email: olivier.bronchain@uclouvain.be, gaetan.cassiers@uclouvain.be
 License: GNU AGPL v3+
 Project-URL: Bug Tracker, https://github.com/simple-crypto/scalib/issues
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: COPYING
-Requires-Dist: numpy~=1.19
+Requires-Dist: numpy~=1.21
 Requires-Dist: py-cpuinfo~=9.0
 
 ======
 SCALib
 ======
 
 .. image:: https://badge.fury.io/py/scalib.svg
```

### Comparing `scalib-0.5.7/src/scalib.egg-info/SOURCES.txt` & `scalib-0.5.8/src/scalib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,16 @@
 src/scalib/metrics/snr.py
 src/scalib/metrics/ttest.py
 src/scalib/modeling/__init__.py
 src/scalib/modeling/ldaclassifier.py
 src/scalib/modeling/rldaclassifier.py
 src/scalib/postprocessing/__init__.py
 src/scalib/postprocessing/rankestimation.py
+src/scalib/preprocessing/__init__.py
+src/scalib/preprocessing/quantization.py
 src/scalib_ext/.gitignore
 src/scalib_ext/Cargo.lock
 src/scalib_ext/Cargo.toml
 src/scalib_ext/geigen/Cargo.toml
 src/scalib_ext/geigen/build.rs
 src/scalib_ext/geigen/include/geigen.h
 src/scalib_ext/geigen/include/Eigen/CMakeLists.txt
@@ -493,12 +495,13 @@
 src/scalib_ext/scalib/tests/ttest.rs
 tests/conftest.py
 tests/mttest_test.py
 tests/requirements.txt
 tests/test_factorgraph.py
 tests/test_lda.py
 tests/test_postprocessing.py
+tests/test_quantizer.py
 tests/test_rlda.py
 tests/test_sascagraph.py
 tests/test_snr.py
 tests/test_tools.py
 tests/test_ttest.py
```

### Comparing `scalib-0.5.7/src/scalib_ext/.gitignore` & `scalib-0.5.8/src/scalib_ext/.gitignore`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/Cargo.lock` & `scalib-0.5.8/src/scalib_ext/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -10,38 +10,20 @@
 dependencies = [
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
-name = "aho-corasick"
-version = "0.7.20"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
-dependencies = [
- "memchr",
-]
-
-[[package]]
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
-name = "ansi_term"
-version = "0.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d52a9bb7ec0cf484c551830a7ce27bd20d67eac647e1befb56b0be4ee39a55d2"
-dependencies = [
- "winapi",
-]
-
-[[package]]
 name = "approx"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f2a05fd1bd10b2527e20a2cd32d8873d115b8b39fe219ee25f42a8aca6ba278"
 dependencies = [
  "num-traits",
 ]
@@ -62,18 +44,19 @@
 checksum = "3e90af4de65aa7b293ef2d09daff88501eb254f58edde2e1ac02c82d873eadad"
 dependencies = [
  "derive_arbitrary",
 ]
 
 [[package]]
 name = "ariadne"
-version = "0.1.5"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1cb2a2046bea8ce5e875551f5772024882de0b540c7f93dfc5d6cf1ca8b030c"
+checksum = "dd002a6223f12c7a95cdd4b1cb3a0149d22d37f7a9ecdb2cb691a071fe236c29"
 dependencies = [
+ "unicode-width",
  "yansi",
 ]
 
 [[package]]
 name = "atomic"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -106,76 +89,60 @@
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "bindgen"
-version = "0.58.1"
+version = "0.69.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f8523b410d7187a43085e7e064416ea32ded16bd0a4e6fc025e21616d01258f"
+checksum = "a00dc851838a2120612785d195287475a3ac45514741da670b735818822129a0"
 dependencies = [
- "bitflags",
- "cexpr 0.4.0",
+ "bitflags 2.5.0",
+ "cexpr",
  "clang-sys",
- "clap 2.34.0",
- "env_logger",
+ "itertools 0.10.5",
  "lazy_static",
  "lazycell",
  "log",
- "peeking_take_while",
+ "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "which 3.1.1",
+ "syn 2.0.55",
+ "which",
 ]
 
 [[package]]
-name = "bindgen"
-version = "0.64.0"
+name = "bitflags"
+version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4243e6031260db77ede97ad86c27e501d646a27ab57b59a574f725d98ab1fb4"
-dependencies = [
- "bitflags",
- "cexpr 0.6.0",
- "clang-sys",
- "lazy_static",
- "lazycell",
- "log",
- "peeking_take_while",
- "proc-macro2",
- "quote",
- "regex",
- "rustc-hash",
- "shlex",
- "syn",
- "which 4.4.0",
-]
+checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "blis-src"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "890f81b2cda67a66e45ae13a35363502e84d6a7da86e429d609ede4f3463d086"
 
 [[package]]
 name = "blis-sys2"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d718a14b1fd18063a14830fea23025a6c5b9f521fe8a641279790eaca0f8ab29"
+checksum = "9ad941266574a81515606c15761783569e8fca8a54cf8bc3caa72781806c827e"
 dependencies = [
- "bindgen 0.58.1",
+ "bindgen",
  "blis-src",
 ]
 
 [[package]]
 name = "bumpalo"
 version = "3.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -203,28 +170,19 @@
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cexpr"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4aedb84272dbe89af497cf81375129abda4fc0a9e7c5d317498c15cc30c0d27"
-dependencies = [
- "nom 5.1.2",
-]
-
-[[package]]
-name = "cexpr"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
 dependencies = [
- "nom 7.1.3",
+ "nom",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
@@ -275,37 +233,22 @@
  "glob",
  "libc",
  "libloading",
 ]
 
 [[package]]
 name = "clap"
-version = "2.34.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0610544180c38b88101fecf2dd634b174a62eef6946f84dfc6a7127512b381c"
-dependencies = [
- "ansi_term",
- "atty",
- "bitflags",
- "strsim",
- "textwrap 0.11.0",
- "unicode-width",
- "vec_map",
-]
-
-[[package]]
-name = "clap"
 version = "3.2.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "clap_lex",
  "indexmap",
- "textwrap 0.16.0",
+ "textwrap",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
@@ -348,17 +291,17 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7c76e09c1aae2bc52b3d2f29e13c6572553b30c4aa1b8a49fd70de6412654cb"
 dependencies = [
  "anes",
  "atty",
  "cast",
  "ciborium",
- "clap 3.2.23",
+ "clap",
  "criterion-plot",
- "itertools",
+ "itertools 0.10.5",
  "lazy_static",
  "num-traits",
  "oorandom",
  "plotters",
  "rayon",
  "regex",
  "serde",
@@ -371,15 +314,15 @@
 [[package]]
 name = "criterion-plot"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6b50826342786a51a89e2da3a28f1c32b06e387201bc2d19791f622c673706b1"
 dependencies = [
  "cast",
- "itertools",
+ "itertools 0.10.5",
 ]
 
 [[package]]
 name = "crossbeam-channel"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c2dd04ddaf88237dc3b8d8f9a3c1004b506b54b3313403944054d23c0870c521"
@@ -441,15 +384,15 @@
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
 version = "1.0.89"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "48dcd35ba14ca9b40d6e4b4b39961f23d835dbb8eed74565ded361d93e1feb8a"
@@ -458,26 +401,26 @@
 name = "cxxbridge-macro"
 version = "1.0.89"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81bbeb29798b407ccd82a3324ade1a7286e0d29851475990b612670f6f5124d2"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "derive_arbitrary"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8beee4701e2e229e8098bbdecdca12449bc3e322f137d269182fa1291e20bd00"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
@@ -485,27 +428,14 @@
 [[package]]
 name = "encode_unicode"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a357d28ed41a50f9c765dbfe56cbc04a64e53e5fc58ba79fbc34c10ef3df831f"
 
 [[package]]
-name = "env_logger"
-version = "0.8.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a19187fea3ac7e84da7dacf48de0c45d63c6a76f9490dae389aead16c243fce3"
-dependencies = [
- "atty",
- "humantime",
- "log",
- "regex",
- "termcolor",
-]
-
-[[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
 name = "geigen"
@@ -566,20 +496,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
-name = "humantime"
-version = "2.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
-
-[[package]]
 name = "hytra"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1d7ee43a7d27a202506374a5afb36b89c3be719ace2082e492dabb2034028124"
 dependencies = [
  "atomic",
  "crossbeam-utils",
@@ -645,14 +569,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itertools"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
 version = "1.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fad582f4b9e86b6caa621cabeb0963332d92eea04729ab12892c2533951e6440"
 
 [[package]]
 name = "js-sys"
@@ -661,21 +594,22 @@
 checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "kdtree"
-version = "0.5.1"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b63d659081717fe428fbaf9549559083956450194e57e8d28498a0dfa31b3b04"
+checksum = "0f0a0e9f770b65bac9aad00f97a67ab5c5319effed07f6da385da3c2115e47ba"
 dependencies = [
  "num-traits",
  "serde",
  "serde_derive",
+ "thiserror",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
@@ -795,15 +729,15 @@
 name = "nalgebra-macros"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01fcc0b8149b4632adc89ac3b7b31a12fb6099a0317a4eb2ebff574ef7de7218"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "ndarray"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
@@ -832,15 +766,15 @@
 [[package]]
 name = "ndarray-stats"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af5a8477ac96877b5bd1fd67e0c28736c12943aba24eda92b127e036b0c8f400"
 dependencies = [
  "indexmap",
- "itertools",
+ "itertools 0.10.5",
  "ndarray",
  "noisy_float",
  "num-integer",
  "num-traits",
  "rand",
 ]
 
@@ -851,24 +785,14 @@
 checksum = "978fe6e6ebc0bf53de533cd456ca2d9de13de13856eda1518a285d7705a213af"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "nom"
-version = "5.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffb4262d26ed83a1c0a33a38fe2bb15797329c85770da05e6b828ddb782627af"
-dependencies = [
- "memchr",
- "version_check",
-]
-
-[[package]]
-name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
@@ -999,20 +923,14 @@
 [[package]]
 name = "paste"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d01a5bd0424d00070b0098dd17ebca6f961a959dead1dbcbbbc1d1cd8d3deeba"
 
 [[package]]
-name = "peeking_take_while"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
-
-[[package]]
 name = "petgraph"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4dd7d28ee937e54fe3080c91faa1c3a46c06de6252988a7f4592ba2310ef22a4"
 dependencies = [
  "fixedbitset",
  "indexmap",
@@ -1057,27 +975,37 @@
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
+name = "prettyplease"
+version = "0.2.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8d3928fb5db768cb86f891ff014f0144589297e3c6a1aba6ed7cecfdace270c7"
+dependencies = [
+ "proc-macro2",
+ "syn 2.0.55",
+]
+
+[[package]]
 name = "primal-check"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9df7f93fd637f083201473dab4fee2db4c429d32e55e3299980ab3957ab916a0"
 dependencies = [
  "num-integer",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "psm"
 version = "0.1.21"
@@ -1129,33 +1057,33 @@
 version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1206,18 +1134,18 @@
 ]
 
 [[package]]
 name = "ranklib"
 version = "0.1.0"
 dependencies = [
  "arbitrary",
- "bindgen 0.64.0",
+ "bindgen",
  "cc",
- "itertools",
- "realfft 3.2.0",
+ "itertools 0.12.1",
+ "realfft 3.3.0",
 ]
 
 [[package]]
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
@@ -1251,38 +1179,36 @@
 checksum = "d7695c87f31dc3644760f23fb59a3fed47659703abf76cf2d111f03b9e712342"
 dependencies = [
  "rustfft",
 ]
 
 [[package]]
 name = "realfft"
-version = "3.2.0"
+version = "3.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93d6b8e8f0c6d2234aa58048d7290c60bf92cd36fd2888cd8331c66ad4f2e1d2"
+checksum = "953d9f7e5cdd80963547b456251296efc2626ed4e3cbf36c869d9564e0220571"
 dependencies = [
  "rustfft",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
 version = "1.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
 dependencies = [
- "aho-corasick",
- "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.6.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1345,15 +1271,15 @@
  "criterion",
  "crossbeam-utils",
  "geigen",
  "hytra",
  "index_vec",
  "indexmap",
  "indicatif",
- "itertools",
+ "itertools 0.12.1",
  "kdtree",
  "matrixmultiply",
  "nalgebra",
  "ndarray",
  "ndarray-rand",
  "ndarray-stats",
  "nshare",
@@ -1408,15 +1334,15 @@
 name = "serde_derive"
 version = "1.0.152"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.93"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cad406b69c91885b5107daf2c29572f6c8cdb3c66826821e286c533490c0bc76"
@@ -1467,24 +1393,29 @@
 [[package]]
 name = "strength_reduce"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe895eb47f22e2ddd4dabc02bce419d2e643c8e3b585c78158b349195bc24d82"
 
 [[package]]
-name = "strsim"
-version = "0.8.0"
+name = "syn"
+version = "1.0.107"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ea5119cdb4c55b55d432abb513a0429384878c15dde60cc77b1c99de1a95a6a"
+checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "2.0.55"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "002a1b3dbf967edfafc32655d0f377ab0bb7b994aa1d32c8cc7e9b8bf3ebb8f0"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1500,23 +1431,14 @@
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "textwrap"
-version = "0.11.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d326610f408c7a4eb6f51c37c330e496b08506c9457c9d34287ecc38809fb060"
-dependencies = [
- "unicode-width",
-]
-
-[[package]]
-name = "textwrap"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
 
 [[package]]
 name = "thiserror"
 version = "1.0.38"
@@ -1530,15 +1452,15 @@
 name = "thiserror-impl"
 version = "1.0.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fb327af4685e4d03fa8cbcf1716380da910eeb2bb8be417e7f9fd3fb164f36f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50f297120ff9d4efe680df143d5631bba9c75fa371992b7fcb33eb3453cb0a07"
@@ -1588,20 +1510,14 @@
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
-name = "vec_map"
-version = "0.8.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1bddf1187be692e79c5ffeab891132dfb0f236ed36a43c7ed39f1165ee20191"
-
-[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
@@ -1637,15 +1553,15 @@
 checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1659,15 +1575,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.84"
@@ -1682,23 +1598,14 @@
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "which"
-version = "3.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d011071ae14a2f6671d0b74080ae0cd8ebf3a6f8c9589a2cd45f23126fe29724"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "which"
 version = "4.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2441c784c52b289a054b7201fc93253e288f094e2f4be9058343127c4226a269"
 dependencies = [
  "either",
  "libc",
  "once_cell",
```

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/build.rs` & `scalib-0.5.8/src/scalib_ext/geigen/build.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/CMakeLists.txt` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/Cholesky` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/CholmodSupport` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/Core` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/Core`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/Eigenvalues` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/Geometry` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/Householder` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/IterativeLinearSolvers` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/Jacobi` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/LU` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/LU`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/MetisSupport` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/OrderingMethods` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/PaStiXSupport` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/PardisoSupport` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/QR` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/QR`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/QtAlignedMalloc` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/SPQRSupport` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/SVD` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/Sparse` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/SparseCholesky` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/SparseCore` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/SparseLU` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/SparseQR` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/StdDeque` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/StdList` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/StdVector` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/SuperLUSupport` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/UmfPackSupport` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LDLT.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT_LAPACKE.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/CholmodSupport.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Array.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayBase.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayWrapper.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Assign.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/AssignEvaluator.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Assign_MKL.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/BandMatrix.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Block.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/BooleanRedux.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/CommaInitializer.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/ConditionEstimator.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/CoreEvaluators.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/CoreIterators.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseBinaryOp.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseNullaryOp.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseTernaryOp.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryOp.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryView.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/DenseBase.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/DenseCoeffsBase.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/DenseStorage.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Diagonal.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalMatrix.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalProduct.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Dot.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/EigenBase.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/ForceAlignedAccess.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Fuzzy.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/GeneralProduct.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/GenericPacketMath.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/GlobalFunctions.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/IO.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Inverse.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Map.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/MapBase.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctions.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctionsImpl.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Matrix.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/MatrixBase.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/NestByValue.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/NoAlias.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/NumTraits.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/PermutationMatrix.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/PlainObjectBase.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Product.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/ProductEvaluators.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Random.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Redux.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Ref.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Replicate.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/ReturnByValue.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Reverse.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Select.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/SelfAdjointView.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/SelfCwiseBinaryOp.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Solve.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/SolveTriangular.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/SolverBase.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/StableNorm.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Stride.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Swap.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Transpose.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Transpositions.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/TriangularMatrix.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/VectorBlock.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/VectorwiseOp.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/Visitor.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/Complex.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/MathFunctions.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/PacketMath.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/TypeCasting.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/PacketMath.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/Complex.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Complex.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Half.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Half.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/MathFunctions.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMath.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/TypeCasting.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/ConjHelper.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/Settings.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/Complex.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/MathFunctions.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/PacketMath.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/Complex.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/MathFunctions.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/PacketMath.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/TypeCasting.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/Complex.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/PacketMath.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/functors/AssignmentFunctors.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/functors/BinaryFunctors.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/functors/NullaryFunctors.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/functors/StlFunctors.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/functors/TernaryFunctors.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/functors/UnaryFunctors.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/Parallelizer.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointProduct.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointRank2Update.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverVector.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/BlasUtil.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/Constants.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/DisableStupidWarnings.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/ForwardDeclarations.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/MKL_support.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/Macros.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/Memory.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/Meta.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/ReenableStupidWarnings.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/StaticAssert.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Core/util/XprHelper.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/EigenSolver.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealQZ.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/Tridiagonalization.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/AlignedBox.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/AngleAxis.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/EulerAngles.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/Homogeneous.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/Hyperplane.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/OrthoMethods.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/ParametrizedLine.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/Quaternion.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/Rotation2D.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/RotationBase.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/Scaling.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/Transform.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/Translation.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/Umeyama.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/Geometry_SSE.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/Geometry_SSE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Householder/BlockHouseholder.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Householder/Householder.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Householder/HouseholderSequence.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/Jacobi/Jacobi.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/LU/Determinant.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/LU/FullPivLU.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/LU/InverseImpl.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/LU/arch/Inverse_SSE.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/LU/arch/Inverse_SSE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/MetisSupport.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Amd.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Ordering.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/PardisoSupport.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/QR/FullPivHouseholderQR.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SVD/BDCSVD.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SVD/SVDBase.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SVD/UpperBidiagonalization.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/AmbiVector.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/CompressedStorage.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/MappedSparseMatrix.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseAssign.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseBlock.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseColEtree.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCompressedBase.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDenseProduct.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDot.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseFuzzy.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMap.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrix.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrixBase.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparsePermutation.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseProduct.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRedux.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRef.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSolverBase.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTranspose.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTriangularView.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseUtil.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseVector.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseView.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseCore/TriangularSolver.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLUImpl.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Memory.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Structs.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Utils.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pivotL.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pruneL.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SparseQR/SparseQR.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdDeque.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdList.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdVector.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/StlSupport/details.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/misc/Image.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/misc/Kernel.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/misc/RealSvd2x2.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/misc/blas.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/misc/lapack.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/plugins/BlockMethods.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/DavidsonSymEigsSolver.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/DavidsonSymEigsSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/GenEigsBase.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/GenEigsBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/GenEigsComplexShiftSolver.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/GenEigsComplexShiftSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/GenEigsRealShiftSolver.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/GenEigsRealShiftSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/GenEigsSolver.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/GenEigsSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/JDSymEigsBase.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/JDSymEigsBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/Arnoldi.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/Arnoldi.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/BKLDLT.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/BKLDLT.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/DoubleShiftQR.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/DoubleShiftQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/Lanczos.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/Lanczos.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/Orthogonalization.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/Orthogonalization.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/RitzPairs.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/RitzPairs.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/SearchSpace.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/SearchSpace.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/TridiagEigen.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/TridiagEigen.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergEigen.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergEigen.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergQR.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/DenseCholesky.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/DenseCholesky.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenComplexShiftSolve.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenComplexShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenMatProd.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenMatProd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenRealShiftSolve.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenRealShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymMatProd.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymMatProd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymShiftSolve.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/SparseCholesky.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/SparseCholesky.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenComplexShiftSolve.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenComplexShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenMatProd.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenMatProd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenRealShiftSolve.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenRealShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/SparseRegularInverse.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/SparseRegularInverse.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymMatProd.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymMatProd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymShiftSolve.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/SymShiftInvert.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/SymShiftInvert.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/internal/ArnoldiOp.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/internal/ArnoldiOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsBucklingOp.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsBucklingOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCayleyOp.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCayleyOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCholeskyOp.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCholeskyOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsRegInvOp.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsRegInvOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsShiftInvertOp.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsShiftInvertOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/SymEigsBase.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/SymEigsBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/SymEigsShiftSolver.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/SymEigsShiftSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/SymEigsSolver.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/SymEigsSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/SymGEigsShiftSolver.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/SymGEigsShiftSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/SymGEigsSolver.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/SymGEigsSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/Util/CompInfo.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/Util/CompInfo.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/Util/GEigsMode.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/Util/GEigsMode.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/Util/SelectionRule.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/Util/SelectionRule.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/Util/SimpleRandom.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/Util/SimpleRandom.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/Util/TypeTraits.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/Util/TypeTraits.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/Util/Version.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/Util/Version.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/contrib/LOBPCGSolver.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/contrib/LOBPCGSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/Spectra/contrib/PartialSVDSolver.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/Spectra/contrib/PartialSVDSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/include/geigen.h` & `scalib-0.5.8/src/scalib_ext/geigen/include/geigen.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/src/geigen.cpp` & `scalib-0.5.8/src/scalib_ext/geigen/src/geigen.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/src/geigen.rs` & `scalib-0.5.8/src/scalib_ext/geigen/src/geigen.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/geigen/src/lib.rs` & `scalib-0.5.8/src/scalib_ext/geigen/src/lib.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/build.rs` & `scalib-0.5.8/src/scalib_ext/ranklib/build.rs`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     println!("cargo:rerun-if-changed=src/bignumpoly.h");
     let bindings = bindgen::Builder::default()
         // The input header we would like to generate
         // bindings for.
         .header("src/bignumpoly.h")
         // Tell cargo to invalidate the built crate whenever any of the
         // included header files changed.
-        .parse_callbacks(Box::new(bindgen::CargoCallbacks))
+        .parse_callbacks(Box::new(bindgen::CargoCallbacks::new()))
         .size_t_is_usize(true)
         .prepend_enum_name(false)
         .raw_line("#[repr(C)] pub struct NTL_ZZ { _private: [u64; 1]}")
         .raw_line("#[repr(C)] pub struct NTL_ZZX { _private: [u64; 1]}")
         .allowlist_function("bnp_.*")
         .allowlist_recursively(false)
         .clang_args(vec!["-x", "c++"])
@@ -32,15 +32,15 @@
     println!("cargo:rerun-if-changed=src/hel_if.h");
     let bindings = bindgen::Builder::default()
         // The input header we would like to generate
         // bindings for.
         .header("src/hel_if.h")
         // Tell cargo to invalidate the built crate whenever any of the
         // included header files changed.
-        .parse_callbacks(Box::new(bindgen::CargoCallbacks))
+        .parse_callbacks(Box::new(bindgen::CargoCallbacks::new()))
         .size_t_is_usize(true)
         .prepend_enum_name(false)
         .raw_line("#[repr(C)] pub struct NTL_ZZ { _private: [u64; 1]}")
         .raw_line("#[repr(C)] pub struct NTL_ZZX { _private: [u64; 1]}")
         .raw_line("#[repr(C)] pub struct NTL_RR { _private: [u64; 2]}")
         .allowlist_type("hel_.*")
         .allowlist_function("hel_.*")
```

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/fuzz/Cargo.toml` & `scalib-0.5.8/src/scalib_ext/ranklib/fuzz/Cargo.toml`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/fuzz/fuzz_targets/rank2vsnaive_2.rs` & `scalib-0.5.8/src/scalib_ext/ranklib/fuzz/fuzz_targets/rank2vsnaive_2.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/aes.cpp` & `scalib-0.5.8/src/scalib_ext/ranklib/src/aes.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/bignumpoly.cpp` & `scalib-0.5.8/src/scalib_ext/ranklib/src/bignumpoly.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/bignumpoly.h` & `scalib-0.5.8/src/scalib_ext/ranklib/src/bignumpoly.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/hel_enum.cpp` & `scalib-0.5.8/src/scalib_ext/ranklib/src/hel_enum.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/hel_enum.h` & `scalib-0.5.8/src/scalib_ext/ranklib/src/hel_enum.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/hel_execute.cpp` & `scalib-0.5.8/src/scalib_ext/ranklib/src/hel_execute.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/hel_histo.cpp` & `scalib-0.5.8/src/scalib_ext/ranklib/src/hel_histo.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/hel_histo.h` & `scalib-0.5.8/src/scalib_ext/ranklib/src/hel_histo.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/hel_if.cpp` & `scalib-0.5.8/src/scalib_ext/ranklib/src/hel_if.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/hel_if.h` & `scalib-0.5.8/src/scalib_ext/ranklib/src/hel_if.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/hel_init.cpp` & `scalib-0.5.8/src/scalib_ext/ranklib/src/hel_init.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/hel_init.h` & `scalib-0.5.8/src/scalib_ext/ranklib/src/hel_init.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/hel_struct.h` & `scalib-0.5.8/src/scalib_ext/ranklib/src/hel_struct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/hel_util.cpp` & `scalib-0.5.8/src/scalib_ext/ranklib/src/hel_util.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/hel_util.h` & `scalib-0.5.8/src/scalib_ext/ranklib/src/hel_util.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/histogram.rs` & `scalib-0.5.8/src/scalib_ext/ranklib/src/histogram.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/lib.rs` & `scalib-0.5.8/src/scalib_ext/ranklib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/main_example.cpp` & `scalib-0.5.8/src/scalib_ext/ranklib/src/main_example.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/rank.rs` & `scalib-0.5.8/src/scalib_ext/ranklib/src/rank.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/score_example_data.rs` & `scalib-0.5.8/src/scalib_ext/ranklib/src/score_example_data.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/scores_example.cpp` & `scalib-0.5.8/src/scalib_ext/ranklib/src/scores_example.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/scores_example.h` & `scalib-0.5.8/src/scalib_ext/ranklib/src/scores_example.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/scores_example_data.cpp` & `scalib-0.5.8/src/scalib_ext/ranklib/src/scores_example_data.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/ranklib/src/top.cpp` & `scalib-0.5.8/src/scalib_ext/ranklib/src/top.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/Cargo.toml` & `scalib-0.5.8/src/scalib_ext/scalib/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -10,44 +10,52 @@
 [features]
 blis = ["blis-src", "blis-sys2"]
 
 [dependencies]
 
 # Utilities
 thiserror = "1.0"
-itertools = "0.10"
+itertools = "0.12"
 rayon = "1.7"
 num-integer = "0.1"
-index_vec = { version = "0.1", features = ["serde"] } # Type-safe indices in FactorGraph
+index_vec = { version = "0.1", features = [
+    "serde",
+] } # Type-safe indices in FactorGraph
 indexmap = { version = "1.9", features = ["serde"] } # Factor graph data
-serde = { version = "1.0", features = ["derive", "rc"] } # Serialization for pickle support
+serde = { version = "1.0", features = [
+    "derive",
+    "rc",
+] } # Serialization for pickle support
 
 # Factor graph parsing and error display
 chumsky = "0.9"
-ariadne = "0.1"
+ariadne = "0.4"
 
 # analysis of factor graphs
-petgraph = {version = "0.6", default-features=false, features = ["serde-1"]}
+petgraph = { version = "0.6", default-features = false, features = ["serde-1"] }
 
 
 # Progress bars
 indicatif = { version = "0.17" }
 hytra = "0.1"
 crossbeam-utils = "0.8"
 
 geigen = { path = "../geigen" }
 
 # Numerical libs
 ndarray = { version = "0.15", features = ["rayon", "approx", "serde"] }
-blis-src = { version = "0.2.1", default-features=false, features=["static", "pthreads"], optional = true }
-blis-sys2 = { version = "0.2.1", optional = true }
+blis-src = { version = "0.2.1", default-features = false, features = [
+    "static",
+    "pthreads",
+], optional = true }
+blis-sys2 = { version = "0.2.2", optional = true }
 matrixmultiply = "0.3"
-kdtree = { version = "0.5.1", features = ["serialize"] }
+kdtree = { version = "0.7", features = ["serialize"] }
 nalgebra = "0.30.1"
-nshare = { version="0.9", features=["nalgebra", "ndarray"] }
+nshare = { version = "0.9", features = ["nalgebra", "ndarray"] }
 
 realfft = "2.0"
 num-traits = "0.2"
 
 [lib]
 bench = false
```

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/benches/belief_propagation.rs` & `scalib-0.5.8/src/scalib_ext/scalib/benches/belief_propagation.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/benches/get_snr.rs` & `scalib-0.5.8/src/scalib_ext/scalib/benches/get_snr.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/benches/mttest.rs` & `scalib-0.5.8/src/scalib_ext/scalib/benches/mttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/benches/snr_update.rs` & `scalib-0.5.8/src/scalib_ext/scalib/benches/snr_update.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/benches/ttest.rs` & `scalib-0.5.8/src/scalib_ext/scalib/benches/ttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/src/belief_propagation.rs` & `scalib-0.5.8/src/scalib_ext/scalib/src/belief_propagation.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/src/information.rs` & `scalib-0.5.8/src/scalib_ext/scalib/src/information.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/src/lda.rs` & `scalib-0.5.8/src/scalib_ext/scalib/src/lda.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/src/lib.rs` & `scalib-0.5.8/src/scalib_ext/scalib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/src/matrixmul.rs` & `scalib-0.5.8/src/scalib_ext/scalib/src/matrixmul.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/src/mttest.rs` & `scalib-0.5.8/src/scalib_ext/scalib/src/mttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/src/rlda.rs` & `scalib-0.5.8/src/scalib_ext/scalib/src/rlda.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/src/sasca/belief_propagation.rs` & `scalib-0.5.8/src/scalib_ext/scalib/src/sasca/belief_propagation.rs`

 * *Files 2% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         match &factor.kind {
             FactorKind::Assign { expr, .. } => match expr {
                 ExprFactor::AND { .. } => {
                     prop_factor!(factor_gen_and, &self.pub_reduced[factor_id])
                 }
                 ExprFactor::XOR => prop_factor!(factor_xor, &self.pub_reduced[factor_id]),
                 ExprFactor::NOT => prop_factor!(factor_not, (self.graph.nc - 1) as u32),
-                ExprFactor::ADD => {
+                ExprFactor::ADD { .. } => {
                     prop_factor!(factor_add, &self.pub_reduced[factor_id], &self.plans)
                 }
                 ExprFactor::MUL => prop_factor!(factor_mul, &self.pub_reduced[factor_id]),
                 ExprFactor::LOOKUP { table } => {
                     prop_factor!(factor_lookup, &self.graph.tables[*table])
                 }
             },
@@ -654,30 +654,38 @@
     factor: &'a Factor,
     belief_from_var: &'a mut EdgeSlice<Distribution>,
     dest: &'a [VarId],
     clear_incoming: bool,
     pub_red: &PublicValue,
     plans: &FftPlans,
 ) -> impl Iterator<Item = Distribution> + 'a {
+    let FactorKind::Assign {
+        expr: ExprFactor::ADD { vars_neg },
+        ..
+    } = &factor.kind
+    else {
+        unreachable!()
+    };
     // Special case for single-input ADD
     if factor.edges.len() == 2 {
         // FIXME check for negative operand
         return dest
             .iter()
             .map(|var| {
                 let i = factor.edges.get_index_of(var).unwrap();
                 let mut distr = belief_from_var[factor.edges[1 - i]].take_or_clone(clear_incoming);
                 distr.add_cst(pub_red, i != 0);
                 distr
             })
             .collect::<Vec<_>>()
             .into_iter();
     }
+
     let mut taken_dest = vec![false; factor.edges.len()];
-    let mut negated_vars = vec![false; factor.edges.len()];
+    let mut negated_vars = vars_neg.clone();
     negated_vars[0] = true;
     for dest in dest {
         taken_dest[factor.edges.get_index_of(dest).unwrap()] = true;
     }
     let mut uniform_iter = factor
         .edges
         .iter()
```

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/src/sasca/bp_compute.rs` & `scalib-0.5.8/src/scalib_ext/scalib/src/sasca/bp_compute.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/src/sasca/factor_graph.rs` & `scalib-0.5.8/src/scalib_ext/scalib/src/sasca/factor_graph.rs`

 * *Files 2% similar despite different names*

```diff
@@ -108,1106 +108,1112 @@
 000006b0: 653a 3a53 6572 6961 6c69 7a65 2c20 7365  e::Serialize, se
 000006c0: 7264 653a 3a44 6573 6572 6961 6c69 7a65  rde::Deserialize
 000006d0: 295d 0a70 7562 2873 7570 6572 2920 656e  )].pub(super) en
 000006e0: 756d 2045 7870 7246 6163 746f 7220 7b0a  um ExprFactor {.
 000006f0: 2020 2020 414e 4420 7b20 7661 7273 5f6e      AND { vars_n
 00000700: 6567 3a20 5665 633c 626f 6f6c 3e20 7d2c  eg: Vec<bool> },
 00000710: 0a20 2020 2058 4f52 2c0a 2020 2020 4e4f  .    XOR,.    NO
-00000720: 542c 0a20 2020 2041 4444 2c0a 2020 2020  T,.    ADD,.    
-00000730: 4d55 4c2c 0a20 2020 204c 4f4f 4b55 5020  MUL,.    LOOKUP 
-00000740: 7b20 7461 626c 653a 2054 6162 6c65 4964  { table: TableId
-00000750: 207d 2c0a 7d0a 0a23 5b64 6572 6976 6528   },.}..#[derive(
-00000760: 4465 6275 672c 2043 6c6f 6e65 2c20 7365  Debug, Clone, se
-00000770: 7264 653a 3a53 6572 6961 6c69 7a65 2c20  rde::Serialize, 
-00000780: 7365 7264 653a 3a44 6573 6572 6961 6c69  serde::Deseriali
-00000790: 7a65 295d 0a70 7562 2873 7570 6572 2920  ze)].pub(super) 
-000007a0: 656e 756d 2047 656e 4661 6374 6f72 4f70  enum GenFactorOp
-000007b0: 6572 616e 6420 7b0a 2020 2020 5661 7228  erand {.    Var(
-000007c0: 7573 697a 652c 2062 6f6f 6c29 2c0a 2020  usize, bool),.  
-000007d0: 2020 5075 6228 7573 697a 6529 2c0a 7d0a    Pub(usize),.}.
-000007e0: 0a23 5b64 6572 6976 6528 4465 6275 672c  .#[derive(Debug,
-000007f0: 2043 6c6f 6e65 2c20 7365 7264 653a 3a53   Clone, serde::S
-00000800: 6572 6961 6c69 7a65 2c20 7365 7264 653a  erialize, serde:
-00000810: 3a44 6573 6572 6961 6c69 7a65 295d 0a70  :Deserialize)].p
-00000820: 7562 2873 7570 6572 2920 656e 756d 2046  ub(super) enum F
-00000830: 6163 746f 724b 696e 6420 7b0a 2020 2020  actorKind {.    
-00000840: 4173 7369 676e 207b 0a20 2020 2020 2020  Assign {.       
-00000850: 2065 7870 723a 2045 7870 7246 6163 746f   expr: ExprFacto
-00000860: 722c 0a20 2020 2020 2020 202f 2f20 4973  r,.        // Is
-00000870: 2074 6865 2072 6573 756c 7420 6120 7661   the result a va
-00000880: 7269 6162 6c65 2028 616e 6420 6e6f 7420  riable (and not 
-00000890: 6120 7075 626c 6963 2920 3f0a 2020 2020  a public) ?.    
-000008a0: 2020 2020 6861 735f 7265 733a 2062 6f6f      has_res: boo
-000008b0: 6c2c 0a20 2020 207d 2c0a 2020 2020 4765  l,.    },.    Ge
-000008c0: 6e46 6163 746f 7220 7b0a 2020 2020 2020  nFactor {.      
-000008d0: 2020 6964 3a20 4765 6e46 6163 746f 7249    id: GenFactorI
-000008e0: 642c 0a20 2020 2020 2020 206f 7065 7261  d,.        opera
-000008f0: 6e64 733a 2056 6563 3c47 656e 4661 6374  nds: Vec<GenFact
-00000900: 6f72 4f70 6572 616e 643e 2c0a 2020 2020  orOperand>,.    
-00000910: 7d2c 0a7d 0a0a 696d 706c 2045 7870 7246  },.}..impl ExprF
-00000920: 6163 746f 7220 7b0a 2020 2020 666e 206d  actor {.    fn m
-00000930: 6572 6765 2826 7365 6c66 2c20 613a 2043  erge(&self, a: C
-00000940: 6c61 7373 5661 6c2c 2062 3a20 436c 6173  lassVal, b: Clas
-00000950: 7356 616c 2c20 6e63 3a20 7573 697a 6529  sVal, nc: usize)
-00000960: 202d 3e20 436c 6173 7356 616c 207b 0a20   -> ClassVal {. 
-00000970: 2020 2020 2020 206d 6174 6368 2073 656c         match sel
-00000980: 6620 7b0a 2020 2020 2020 2020 2020 2020  f {.            
-00000990: 5365 6c66 3a3a 414e 4420 7b20 7661 7273  Self::AND { vars
-000009a0: 5f6e 6567 3a20 5f20 7d20 3d3e 2061 2026  _neg: _ } => a &
-000009b0: 2062 2c0a 2020 2020 2020 2020 2020 2020   b,.            
-000009c0: 5365 6c66 3a3a 584f 5220 3d3e 2061 205e  Self::XOR => a ^
-000009d0: 2062 2c0a 2020 2020 2020 2020 2020 2020   b,.            
-000009e0: 5365 6c66 3a3a 4144 4420 3d3e 2028 2828  Self::ADD => (((
-000009f0: 6120 6173 2075 3634 2920 2b20 2862 2061  a as u64) + (b a
-00000a00: 7320 7536 3429 2920 2520 286e 6320 6173  s u64)) % (nc as
-00000a10: 2075 3634 2929 2061 7320 436c 6173 7356   u64)) as ClassV
-00000a20: 616c 2c0a 2020 2020 2020 2020 2020 2020  al,.            
-00000a30: 5365 6c66 3a3a 4d55 4c20 3d3e 2028 2828  Self::MUL => (((
-00000a40: 6120 6173 2075 3634 2920 2a20 2862 2061  a as u64) * (b a
-00000a50: 7320 7536 3429 2920 2520 286e 6320 6173  s u64)) % (nc as
-00000a60: 2075 3634 2929 2061 7320 436c 6173 7356   u64)) as ClassV
-00000a70: 616c 2c0a 2020 2020 2020 2020 2020 2020  al,.            
-00000a80: 5365 6c66 3a3a 4e4f 5420 7c20 5365 6c66  Self::NOT | Self
-00000a90: 3a3a 4c4f 4f4b 5550 207b 202e 2e20 7d20  ::LOOKUP { .. } 
-00000aa0: 3d3e 2075 6e72 6561 6368 6162 6c65 2128  => unreachable!(
-00000ab0: 292c 0a20 2020 2020 2020 207d 0a20 2020  ),.        }.   
-00000ac0: 207d 0a20 2020 2066 6e20 6e65 7574 7261   }.    fn neutra
-00000ad0: 6c28 2673 656c 662c 206e 633a 2075 7369  l(&self, nc: usi
-00000ae0: 7a65 2920 2d3e 2043 6c61 7373 5661 6c20  ze) -> ClassVal 
-00000af0: 7b0a 2020 2020 2020 2020 6d61 7463 6820  {.        match 
-00000b00: 7365 6c66 207b 0a20 2020 2020 2020 2020  self {.         
-00000b10: 2020 2053 656c 663a 3a41 4e44 207b 2076     Self::AND { v
-00000b20: 6172 735f 6e65 673a 205f 207d 203d 3e20  ars_neg: _ } => 
-00000b30: 286e 6320 2d20 3129 2061 7320 436c 6173  (nc - 1) as Clas
-00000b40: 7356 616c 2c0a 2020 2020 2020 2020 2020  sVal,.          
-00000b50: 2020 5365 6c66 3a3a 584f 5220 7c20 5365    Self::XOR | Se
-00000b60: 6c66 3a3a 4144 4420 3d3e 2030 2c0a 2020  lf::ADD => 0,.  
+00000720: 542c 0a20 2020 2041 4444 207b 2076 6172  T,.    ADD { var
+00000730: 735f 6e65 673a 2056 6563 3c62 6f6f 6c3e  s_neg: Vec<bool>
+00000740: 207d 2c0a 2020 2020 4d55 4c2c 0a20 2020   },.    MUL,.   
+00000750: 204c 4f4f 4b55 5020 7b20 7461 626c 653a   LOOKUP { table:
+00000760: 2054 6162 6c65 4964 207d 2c0a 7d0a 0a23   TableId },.}..#
+00000770: 5b64 6572 6976 6528 4465 6275 672c 2043  [derive(Debug, C
+00000780: 6c6f 6e65 2c20 7365 7264 653a 3a53 6572  lone, serde::Ser
+00000790: 6961 6c69 7a65 2c20 7365 7264 653a 3a44  ialize, serde::D
+000007a0: 6573 6572 6961 6c69 7a65 295d 0a70 7562  eserialize)].pub
+000007b0: 2873 7570 6572 2920 656e 756d 2047 656e  (super) enum Gen
+000007c0: 4661 6374 6f72 4f70 6572 616e 6420 7b0a  FactorOperand {.
+000007d0: 2020 2020 5661 7228 7573 697a 652c 2062      Var(usize, b
+000007e0: 6f6f 6c29 2c0a 2020 2020 5075 6228 7573  ool),.    Pub(us
+000007f0: 697a 6529 2c0a 7d0a 0a23 5b64 6572 6976  ize),.}..#[deriv
+00000800: 6528 4465 6275 672c 2043 6c6f 6e65 2c20  e(Debug, Clone, 
+00000810: 7365 7264 653a 3a53 6572 6961 6c69 7a65  serde::Serialize
+00000820: 2c20 7365 7264 653a 3a44 6573 6572 6961  , serde::Deseria
+00000830: 6c69 7a65 295d 0a70 7562 2873 7570 6572  lize)].pub(super
+00000840: 2920 656e 756d 2046 6163 746f 724b 696e  ) enum FactorKin
+00000850: 6420 7b0a 2020 2020 4173 7369 676e 207b  d {.    Assign {
+00000860: 0a20 2020 2020 2020 2065 7870 723a 2045  .        expr: E
+00000870: 7870 7246 6163 746f 722c 0a20 2020 2020  xprFactor,.     
+00000880: 2020 202f 2f20 4973 2074 6865 2072 6573     // Is the res
+00000890: 756c 7420 6120 7661 7269 6162 6c65 2028  ult a variable (
+000008a0: 616e 6420 6e6f 7420 6120 7075 626c 6963  and not a public
+000008b0: 2920 3f0a 2020 2020 2020 2020 6861 735f  ) ?.        has_
+000008c0: 7265 733a 2062 6f6f 6c2c 0a20 2020 207d  res: bool,.    }
+000008d0: 2c0a 2020 2020 4765 6e46 6163 746f 7220  ,.    GenFactor 
+000008e0: 7b0a 2020 2020 2020 2020 6964 3a20 4765  {.        id: Ge
+000008f0: 6e46 6163 746f 7249 642c 0a20 2020 2020  nFactorId,.     
+00000900: 2020 206f 7065 7261 6e64 733a 2056 6563     operands: Vec
+00000910: 3c47 656e 4661 6374 6f72 4f70 6572 616e  <GenFactorOperan
+00000920: 643e 2c0a 2020 2020 7d2c 0a7d 0a0a 696d  d>,.    },.}..im
+00000930: 706c 2045 7870 7246 6163 746f 7220 7b0a  pl ExprFactor {.
+00000940: 2020 2020 666e 206d 6572 6765 2826 7365      fn merge(&se
+00000950: 6c66 2c20 613a 2043 6c61 7373 5661 6c2c  lf, a: ClassVal,
+00000960: 2062 3a20 436c 6173 7356 616c 2c20 6e63   b: ClassVal, nc
+00000970: 3a20 7573 697a 6529 202d 3e20 436c 6173  : usize) -> Clas
+00000980: 7356 616c 207b 0a20 2020 2020 2020 206d  sVal {.        m
+00000990: 6174 6368 2073 656c 6620 7b0a 2020 2020  atch self {.    
+000009a0: 2020 2020 2020 2020 5365 6c66 3a3a 414e          Self::AN
+000009b0: 4420 7b20 7661 7273 5f6e 6567 3a20 5f20  D { vars_neg: _ 
+000009c0: 7d20 3d3e 2061 2026 2062 2c0a 2020 2020  } => a & b,.    
+000009d0: 2020 2020 2020 2020 5365 6c66 3a3a 584f          Self::XO
+000009e0: 5220 3d3e 2061 205e 2062 2c0a 2020 2020  R => a ^ b,.    
+000009f0: 2020 2020 2020 2020 5365 6c66 3a3a 4144          Self::AD
+00000a00: 4420 7b20 7661 7273 5f6e 6567 3a20 5f20  D { vars_neg: _ 
+00000a10: 7d20 3d3e 2028 2828 6120 6173 2075 3634  } => (((a as u64
+00000a20: 2920 2b20 2862 2061 7320 7536 3429 2920  ) + (b as u64)) 
+00000a30: 2520 286e 6320 6173 2075 3634 2929 2061  % (nc as u64)) a
+00000a40: 7320 436c 6173 7356 616c 2c0a 2020 2020  s ClassVal,.    
+00000a50: 2020 2020 2020 2020 5365 6c66 3a3a 4d55          Self::MU
+00000a60: 4c20 3d3e 2028 2828 6120 6173 2075 3634  L => (((a as u64
+00000a70: 2920 2a20 2862 2061 7320 7536 3429 2920  ) * (b as u64)) 
+00000a80: 2520 286e 6320 6173 2075 3634 2929 2061  % (nc as u64)) a
+00000a90: 7320 436c 6173 7356 616c 2c0a 2020 2020  s ClassVal,.    
+00000aa0: 2020 2020 2020 2020 5365 6c66 3a3a 4e4f          Self::NO
+00000ab0: 5420 7c20 5365 6c66 3a3a 4c4f 4f4b 5550  T | Self::LOOKUP
+00000ac0: 207b 202e 2e20 7d20 3d3e 2075 6e72 6561   { .. } => unrea
+00000ad0: 6368 6162 6c65 2128 292c 0a20 2020 2020  chable!(),.     
+00000ae0: 2020 207d 0a20 2020 207d 0a20 2020 2066     }.    }.    f
+00000af0: 6e20 6e65 7574 7261 6c28 2673 656c 662c  n neutral(&self,
+00000b00: 206e 633a 2075 7369 7a65 2920 2d3e 2043   nc: usize) -> C
+00000b10: 6c61 7373 5661 6c20 7b0a 2020 2020 2020  lassVal {.      
+00000b20: 2020 6d61 7463 6820 7365 6c66 207b 0a20    match self {. 
+00000b30: 2020 2020 2020 2020 2020 2053 656c 663a             Self:
+00000b40: 3a41 4e44 207b 2076 6172 735f 6e65 673a  :AND { vars_neg:
+00000b50: 205f 207d 203d 3e20 286e 6320 2d20 3129   _ } => (nc - 1)
+00000b60: 2061 7320 436c 6173 7356 616c 2c0a 2020   as ClassVal,.  
 00000b70: 2020 2020 2020 2020 2020 5365 6c66 3a3a            Self::
-00000b80: 4d55 4c20 3d3e 2031 2c0a 2020 2020 2020  MUL => 1,.      
-00000b90: 2020 2020 2020 5365 6c66 3a3a 4e4f 5420        Self::NOT 
-00000ba0: 7c20 5365 6c66 3a3a 4c4f 4f4b 5550 207b  | Self::LOOKUP {
-00000bb0: 202e 2e20 7d20 3d3e 2075 6e72 6561 6368   .. } => unreach
-00000bc0: 6162 6c65 2128 292c 0a20 2020 2020 2020  able!(),.       
-00000bd0: 207d 0a20 2020 207d 0a7d 0a0a 235b 6465   }.    }.}..#[de
-00000be0: 7269 7665 2844 6562 7567 2c20 436c 6f6e  rive(Debug, Clon
-00000bf0: 652c 2073 6572 6465 3a3a 5365 7269 616c  e, serde::Serial
-00000c00: 697a 652c 2073 6572 6465 3a3a 4465 7365  ize, serde::Dese
-00000c10: 7269 616c 697a 6529 5d0a 7075 6228 7375  rialize)].pub(su
-00000c20: 7065 7229 2073 7472 7563 7420 4564 6765  per) struct Edge
-00000c30: 207b 0a20 2020 2070 7562 2873 7570 6572   {.    pub(super
-00000c40: 2920 7661 723a 2056 6172 4964 2c0a 2020  ) var: VarId,.  
-00000c50: 2020 7075 6228 7375 7065 7229 2070 6f73    pub(super) pos
-00000c60: 5f76 6172 3a20 7573 697a 652c 0a20 2020  _var: usize,.   
-00000c70: 2070 7562 2873 7570 6572 2920 6661 6374   pub(super) fact
-00000c80: 6f72 3a20 4661 6374 6f72 4964 2c0a 2020  or: FactorId,.  
-00000c90: 2020 7075 6228 7375 7065 7229 2070 6f73    pub(super) pos
-00000ca0: 5f66 6163 746f 723a 2075 7369 7a65 2c0a  _factor: usize,.
-00000cb0: 7d0a 0a23 5b64 6572 6976 6528 4465 6275  }..#[derive(Debu
-00000cc0: 672c 2043 6c6f 6e65 2c20 7365 7264 653a  g, Clone, serde:
-00000cd0: 3a53 6572 6961 6c69 7a65 2c20 7365 7264  :Serialize, serd
-00000ce0: 653a 3a44 6573 6572 6961 6c69 7a65 295d  e::Deserialize)]
-00000cf0: 0a70 7562 2873 7570 6572 2920 7374 7275  .pub(super) stru
-00000d00: 6374 2050 7562 6c69 6320 7b0a 2020 2020  ct Public {.    
-00000d10: 7075 6228 7375 7065 7229 206d 756c 7469  pub(super) multi
-00000d20: 3a20 626f 6f6c 2c0a 7d0a 0a23 5b64 6572  : bool,.}..#[der
-00000d30: 6976 6528 4465 6275 672c 2043 6c6f 6e65  ive(Debug, Clone
-00000d40: 2c20 7365 7264 653a 3a53 6572 6961 6c69  , serde::Seriali
-00000d50: 7a65 2c20 7365 7264 653a 3a44 6573 6572  ze, serde::Deser
-00000d60: 6961 6c69 7a65 295d 0a70 7562 2873 7570  ialize)].pub(sup
-00000d70: 6572 2920 7374 7275 6374 2047 656e 4661  er) struct GenFa
-00000d80: 6374 6f72 207b 0a20 2020 2070 7562 2873  ctor {.    pub(s
-00000d90: 7570 6572 2920 6d75 6c74 693a 2062 6f6f  uper) multi: boo
-00000da0: 6c2c 0a7d 0a0a 235b 6465 7269 7665 2844  l,.}..#[derive(D
-00000db0: 6562 7567 2c20 436c 6f6e 652c 2073 6572  ebug, Clone, ser
-00000dc0: 6465 3a3a 5365 7269 616c 697a 652c 2073  de::Serialize, s
-00000dd0: 6572 6465 3a3a 4465 7365 7269 616c 697a  erde::Deserializ
-00000de0: 6529 5d0a 7075 6228 7375 7065 7229 2073  e)].pub(super) s
-00000df0: 7472 7563 7420 5461 626c 6520 7b0a 2020  truct Table {.  
-00000e00: 2020 7075 6228 7375 7065 7229 2076 616c    pub(super) val
-00000e10: 7565 733a 2056 6563 3c43 6c61 7373 5661  ues: Vec<ClassVa
-00000e20: 6c3e 2c0a 7d0a 0a23 5b64 6572 6976 6528  l>,.}..#[derive(
-00000e30: 4465 6275 672c 2043 6f70 792c 2043 6c6f  Debug, Copy, Clo
-00000e40: 6e65 2c20 7365 7264 653a 3a53 6572 6961  ne, serde::Seria
-00000e50: 6c69 7a65 2c20 7365 7264 653a 3a44 6573  lize, serde::Des
-00000e60: 6572 6961 6c69 7a65 295d 0a70 7562 2873  erialize)].pub(s
-00000e70: 7570 6572 2920 656e 756d 204e 6f64 6520  uper) enum Node 
-00000e80: 7b0a 2020 2020 5661 7228 5661 7249 6429  {.    Var(VarId)
-00000e90: 2c0a 2020 2020 4661 6374 6f72 2846 6163  ,.    Factor(Fac
-00000ea0: 746f 7249 6429 2c0a 7d0a 0a23 5b64 6572  torId),.}..#[der
-00000eb0: 6976 6528 4465 6275 672c 2043 6c6f 6e65  ive(Debug, Clone
-00000ec0: 2c20 7365 7264 653a 3a53 6572 6961 6c69  , serde::Seriali
-00000ed0: 7a65 2c20 7365 7264 653a 3a44 6573 6572  ze, serde::Deser
-00000ee0: 6961 6c69 7a65 295d 0a70 7562 2073 7472  ialize)].pub str
-00000ef0: 7563 7420 4661 6374 6f72 4772 6170 6820  uct FactorGraph 
-00000f00: 7b0a 2020 2020 7075 6228 7375 7065 7229  {.    pub(super)
-00000f10: 206e 633a 2075 7369 7a65 2c0a 2020 2020   nc: usize,.    
-00000f20: 7075 6228 7375 7065 7229 2076 6172 733a  pub(super) vars:
-00000f30: 204e 616d 6564 4c69 7374 3c56 6172 3e2c   NamedList<Var>,
-00000f40: 0a20 2020 2070 7562 2873 7570 6572 2920  .    pub(super) 
-00000f50: 6661 6374 6f72 733a 204e 616d 6564 4c69  factors: NamedLi
-00000f60: 7374 3c46 6163 746f 723e 2c0a 2020 2020  st<Factor>,.    
-00000f70: 7075 6228 7375 7065 7229 2065 6467 6573  pub(super) edges
-00000f80: 3a20 4564 6765 5665 633c 4564 6765 3e2c  : EdgeVec<Edge>,
-00000f90: 0a20 2020 2070 7562 2873 7570 6572 2920  .    pub(super) 
-00000fa0: 7075 626c 6963 733a 204e 616d 6564 4c69  publics: NamedLi
-00000fb0: 7374 3c50 7562 6c69 633e 2c0a 2020 2020  st<Public>,.    
-00000fc0: 7075 6228 7375 7065 7229 2074 6162 6c65  pub(super) table
-00000fd0: 733a 204e 616d 6564 4c69 7374 3c54 6162  s: NamedList<Tab
-00000fe0: 6c65 3e2c 0a20 2020 2070 7562 2873 7570  le>,.    pub(sup
-00000ff0: 6572 2920 6765 6e5f 6661 6374 6f72 733a  er) gen_factors:
-00001000: 204e 616d 6564 4c69 7374 3c47 656e 4661   NamedList<GenFa
-00001010: 6374 6f72 3e2c 0a20 2020 2070 7562 2873  ctor>,.    pub(s
-00001020: 7570 6572 2920 7065 7467 7261 7068 3a20  uper) petgraph: 
-00001030: 7065 7467 7261 7068 3a3a 4772 6170 683c  petgraph::Graph<
-00001040: 4e6f 6465 2c20 4564 6765 4964 2c20 7065  Node, EdgeId, pe
-00001050: 7467 7261 7068 3a3a 556e 6469 7265 6374  tgraph::Undirect
-00001060: 6564 3e2c 0a20 2020 2070 7562 2873 7570  ed>,.    pub(sup
-00001070: 6572 2920 7661 725f 6772 6170 685f 6964  er) var_graph_id
-00001080: 733a 2056 6172 5665 633c 7065 7467 7261  s: VarVec<petgra
-00001090: 7068 3a3a 6772 6170 683a 3a4e 6f64 6549  ph::graph::NodeI
-000010a0: 6e64 6578 3e2c 0a20 2020 2070 7562 2873  ndex>,.    pub(s
-000010b0: 7570 6572 2920 6661 6374 6f72 5f67 7261  uper) factor_gra
-000010c0: 7068 5f69 6473 3a20 4661 6374 6f72 5665  ph_ids: FactorVe
-000010d0: 633c 7065 7467 7261 7068 3a3a 6772 6170  c<petgraph::grap
-000010e0: 683a 3a4e 6f64 6549 6e64 6578 3e2c 0a20  h::NodeIndex>,. 
-000010f0: 2020 2070 7562 2873 7570 6572 2920 6379     pub(super) cy
-00001100: 636c 6963 5f73 696e 676c 653a 2062 6f6f  clic_single: boo
-00001110: 6c2c 0a20 2020 2070 7562 2873 7570 6572  l,.    pub(super
-00001120: 2920 6379 636c 6963 5f6d 756c 7469 3a20  ) cyclic_multi: 
-00001130: 626f 6f6c 2c0a 7d0a 0a23 5b64 6572 6976  bool,.}..#[deriv
-00001140: 6528 4465 6275 672c 2043 6c6f 6e65 2c20  e(Debug, Clone, 
-00001150: 4571 2c20 5061 7274 6961 6c45 712c 2073  Eq, PartialEq, s
-00001160: 6572 6465 3a3a 5365 7269 616c 697a 652c  erde::Serialize,
-00001170: 2073 6572 6465 3a3a 4465 7365 7269 616c   serde::Deserial
-00001180: 697a 6529 5d0a 7075 6220 656e 756d 2050  ize)].pub enum P
-00001190: 7562 6c69 6356 616c 7565 207b 0a20 2020  ublicValue {.   
-000011a0: 2053 696e 676c 6528 436c 6173 7356 616c   Single(ClassVal
-000011b0: 292c 0a20 2020 204d 756c 7469 2856 6563  ),.    Multi(Vec
-000011c0: 3c43 6c61 7373 5661 6c3e 292c 0a7d 0a69  <ClassVal>),.}.i
-000011d0: 6d70 6c20 5075 626c 6963 5661 6c75 6520  mpl PublicValue 
-000011e0: 7b0a 2020 2020 7075 6220 666e 2061 735f  {.    pub fn as_
-000011f0: 736c 6963 6528 2673 656c 6629 202d 3e20  slice(&self) -> 
-00001200: 265b 436c 6173 7356 616c 5d20 7b0a 2020  &[ClassVal] {.  
-00001210: 2020 2020 2020 6d61 7463 6820 7365 6c66        match self
-00001220: 207b 0a20 2020 2020 2020 2020 2020 2050   {.            P
-00001230: 7562 6c69 6356 616c 7565 3a3a 5369 6e67  ublicValue::Sing
-00001240: 6c65 2878 2920 3d3e 2073 7464 3a3a 736c  le(x) => std::sl
-00001250: 6963 653a 3a66 726f 6d5f 7265 6628 7829  ice::from_ref(x)
-00001260: 2c0a 2020 2020 2020 2020 2020 2020 5075  ,.            Pu
-00001270: 626c 6963 5661 6c75 653a 3a4d 756c 7469  blicValue::Multi
-00001280: 2878 2920 3d3e 2078 2e61 735f 736c 6963  (x) => x.as_slic
-00001290: 6528 292c 0a20 2020 2020 2020 207d 0a20  e(),.        }. 
-000012a0: 2020 207d 0a20 2020 2070 7562 2066 6e20     }.    pub fn 
-000012b0: 6974 6572 2826 7365 6c66 2c20 6e3a 2075  iter(&self, n: u
-000012c0: 7369 7a65 2920 2d3e 2069 6d70 6c20 4974  size) -> impl It
-000012d0: 6572 6174 6f72 3c49 7465 6d20 3d20 436c  erator<Item = Cl
-000012e0: 6173 7356 616c 3e20 2b20 275f 207b 0a20  assVal> + '_ {. 
-000012f0: 2020 2020 2020 2069 6620 6c65 7420 5075         if let Pu
-00001300: 626c 6963 5661 6c75 653a 3a4d 756c 7469  blicValue::Multi
-00001310: 2878 2920 3d20 7365 6c66 207b 0a20 2020  (x) = self {.   
-00001320: 2020 2020 2020 2020 2061 7373 6572 745f           assert_
-00001330: 6571 2128 782e 6c65 6e28 292c 206e 293b  eq!(x.len(), n);
-00001340: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-00001350: 2020 2028 302e 2e6e 292e 6d61 7028 7c69     (0..n).map(|i
-00001360: 7c20 7365 6c66 2e67 6574 2869 2929 0a20  | self.get(i)). 
-00001370: 2020 207d 0a20 2020 2070 7562 2066 6e20     }.    pub fn 
-00001380: 6765 7428 2673 656c 662c 206e 3a20 7573  get(&self, n: us
-00001390: 697a 6529 202d 3e20 436c 6173 7356 616c  ize) -> ClassVal
-000013a0: 207b 0a20 2020 2020 2020 206d 6174 6368   {.        match
-000013b0: 2073 656c 6620 7b0a 2020 2020 2020 2020   self {.        
-000013c0: 2020 2020 5075 626c 6963 5661 6c75 653a      PublicValue:
-000013d0: 3a53 696e 676c 6528 7829 203d 3e20 2a78  :Single(x) => *x
-000013e0: 2c0a 2020 2020 2020 2020 2020 2020 5075  ,.            Pu
-000013f0: 626c 6963 5661 6c75 653a 3a4d 756c 7469  blicValue::Multi
-00001400: 2878 2920 3d3e 2078 5b6e 5d2c 0a20 2020  (x) => x[n],.   
-00001410: 2020 2020 207d 0a20 2020 207d 0a20 2020       }.    }.   
-00001420: 2070 7562 2066 6e20 6d61 7028 2673 656c   pub fn map(&sel
-00001430: 662c 2066 3a20 696d 706c 2046 6e28 436c  f, f: impl Fn(Cl
-00001440: 6173 7356 616c 2920 2d3e 2043 6c61 7373  assVal) -> Class
-00001450: 5661 6c29 202d 3e20 5365 6c66 207b 0a20  Val) -> Self {. 
-00001460: 2020 2020 2020 206d 6174 6368 2073 656c         match sel
-00001470: 6620 7b0a 2020 2020 2020 2020 2020 2020  f {.            
-00001480: 5075 626c 6963 5661 6c75 653a 3a53 696e  PublicValue::Sin
-00001490: 676c 6528 7829 203d 3e20 5075 626c 6963  gle(x) => Public
-000014a0: 5661 6c75 653a 3a53 696e 676c 6528 6628  Value::Single(f(
-000014b0: 2a78 2929 2c0a 2020 2020 2020 2020 2020  *x)),.          
-000014c0: 2020 5075 626c 6963 5661 6c75 653a 3a4d    PublicValue::M
-000014d0: 756c 7469 2878 2920 3d3e 2050 7562 6c69  ulti(x) => Publi
-000014e0: 6356 616c 7565 3a3a 4d75 6c74 6928 782e  cValue::Multi(x.
-000014f0: 6974 6572 2829 2e63 6c6f 6e65 6428 292e  iter().cloned().
-00001500: 6d61 7028 6629 2e63 6f6c 6c65 6374 2829  map(f).collect()
-00001510: 292c 0a20 2020 2020 2020 207d 0a20 2020  ),.        }.   
-00001520: 207d 0a7d 0a69 6d70 6c20 666d 743a 3a44   }.}.impl fmt::D
-00001530: 6973 706c 6179 2066 6f72 2050 7562 6c69  isplay for Publi
-00001540: 6356 616c 7565 207b 0a20 2020 2066 6e20  cValue {.    fn 
-00001550: 666d 7428 2673 656c 662c 2066 3a20 266d  fmt(&self, f: &m
-00001560: 7574 2066 6d74 3a3a 466f 726d 6174 7465  ut fmt::Formatte
-00001570: 723c 275f 3e29 202d 3e20 666d 743a 3a52  r<'_>) -> fmt::R
-00001580: 6573 756c 7420 7b0a 2020 2020 2020 2020  esult {.        
-00001590: 6d61 7463 6820 7365 6c66 207b 0a20 2020  match self {.   
-000015a0: 2020 2020 2020 2020 2050 7562 6c69 6356           PublicV
-000015b0: 616c 7565 3a3a 5369 6e67 6c65 2878 2920  alue::Single(x) 
-000015c0: 3d3e 2077 7269 7465 2128 662c 2022 7b7d  => write!(f, "{}
-000015d0: 222c 2078 292c 0a20 2020 2020 2020 2020  ", x),.         
-000015e0: 2020 2050 7562 6c69 6356 616c 7565 3a3a     PublicValue::
-000015f0: 4d75 6c74 6928 7829 203d 3e20 7772 6974  Multi(x) => writ
-00001600: 6521 2866 2c20 227b 3a3f 7d22 2c20 782e  e!(f, "{:?}", x.
-00001610: 6173 5f73 6c69 6365 2829 292c 0a20 2020  as_slice()),.   
-00001620: 2020 2020 207d 0a20 2020 207d 0a7d 0a0a       }.    }.}..
-00001630: 235b 6465 7269 7665 2844 6562 7567 2c20  #[derive(Debug, 
-00001640: 436c 6f6e 652c 2045 7272 6f72 295d 0a70  Clone, Error)].p
-00001650: 7562 2065 6e75 6d20 4647 4572 726f 7220  ub enum FGError 
-00001660: 7b0a 2020 2020 235b 6572 726f 7228 224e  {.    #[error("N
-00001670: 6f20 7661 7269 6162 6c65 206e 616d 6564  o variable named
-00001680: 207b 307d 2e22 295d 0a20 2020 204e 6f56   {0}.")].    NoV
-00001690: 6172 2853 7472 696e 6729 2c0a 2020 2020  ar(String),.    
-000016a0: 235b 6572 726f 7228 224e 6f20 6661 6374  #[error("No fact
-000016b0: 6f72 206e 616d 6564 207b 307d 2e22 295d  or named {0}.")]
-000016c0: 0a20 2020 204e 6f46 6163 746f 7228 5374  .    NoFactor(St
-000016d0: 7269 6e67 292c 0a20 2020 2023 5b65 7272  ring),.    #[err
-000016e0: 6f72 2822 4e6f 2065 6467 6520 6265 7477  or("No edge betw
-000016f0: 6565 6e20 7661 7269 6162 6c65 207b 7661  een variable {va
-00001700: 727d 2061 6e64 2066 6163 746f 7220 7b66  r} and factor {f
-00001710: 6163 746f 727d 2e22 295d 0a20 2020 204e  actor}.")].    N
-00001720: 6f45 6467 6520 7b20 7661 723a 2053 7472  oEdge { var: Str
-00001730: 696e 672c 2066 6163 746f 723a 2046 6163  ing, factor: Fac
-00001740: 746f 7249 6420 7d2c 0a20 2020 2023 5b65  torId },.    #[e
-00001750: 7272 6f72 2822 4661 696c 7572 6520 6174  rror("Failure at
-00001760: 2066 6163 746f 7220 7b30 7d2e 2045 7870   factor {0}. Exp
-00001770: 6563 7465 6420 7265 7375 6c74 207b 317d  ected result {1}
-00001780: 2c20 676f 7420 7b32 7d2e 2229 5d0a 2020  , got {2}.")].  
-00001790: 2020 4368 6563 6b46 6169 6c28 5374 7269    CheckFail(Stri
-000017a0: 6e67 2c20 5075 626c 6963 5661 6c75 652c  ng, PublicValue,
-000017b0: 2050 7562 6c69 6356 616c 7565 292c 0a20   PublicValue),. 
-000017c0: 2020 2023 5b65 7272 6f72 2822 2229 5d0a     #[error("")].
-000017d0: 2020 2020 496e 7661 6c69 6447 656e 6572      InvalidGener
-000017e0: 6963 4661 6374 6f72 4173 7369 676e 6d65  icFactorAssignme
-000017f0: 6e74 2853 7472 696e 6729 2c0a 7d0a 0a74  nt(String),.}..t
-00001800: 7970 6520 4647 5265 7375 6c74 3c54 3e20  ype FGResult<T> 
-00001810: 3d20 5265 7375 6c74 3c54 2c20 4647 4572  = Result<T, FGEr
-00001820: 726f 723e 3b0a 0a69 6d70 6c20 4661 6374  ror>;..impl Fact
-00001830: 6f72 4772 6170 6820 7b0a 2020 2020 7075  orGraph {.    pu
-00001840: 6220 666e 2065 6467 6528 2673 656c 662c  b fn edge(&self,
-00001850: 2076 6172 3a20 5661 7249 642c 2066 6163   var: VarId, fac
-00001860: 746f 723a 2046 6163 746f 7249 6429 202d  tor: FactorId) -
-00001870: 3e20 4647 5265 7375 6c74 3c45 6467 6549  > FGResult<EdgeI
-00001880: 643e 207b 0a20 2020 2020 2020 2073 656c  d> {.        sel
-00001890: 662e 7661 7228 7661 7229 0a20 2020 2020  f.var(var).     
-000018a0: 2020 2020 2020 202e 6564 6765 730a 2020         .edges.  
-000018b0: 2020 2020 2020 2020 2020 2e67 6574 2826            .get(&
-000018c0: 6661 6374 6f72 290a 2020 2020 2020 2020  factor).        
-000018d0: 2020 2020 2e6d 6170 287c 657c 202a 6529      .map(|e| *e)
-000018e0: 0a20 2020 2020 2020 2020 2020 202e 6f6b  .            .ok
-000018f0: 5f6f 725f 656c 7365 287c 7c20 4647 4572  _or_else(|| FGEr
-00001900: 726f 723a 3a4e 6f45 6467 6520 7b0a 2020  ror::NoEdge {.  
-00001910: 2020 2020 2020 2020 2020 2020 2020 7661                va
-00001920: 723a 2073 656c 662e 7661 7273 2e67 6574  r: self.vars.get
-00001930: 5f69 6e64 6578 2876 6172 2e69 6478 2829  _index(var.idx()
-00001940: 292e 756e 7772 6170 2829 2e30 2e74 6f5f  ).unwrap().0.to_
-00001950: 6f77 6e65 6428 292c 0a20 2020 2020 2020  owned(),.       
-00001960: 2020 2020 2020 2020 2066 6163 746f 722c           factor,
-00001970: 0a20 2020 2020 2020 2020 2020 207d 290a  .            }).
-00001980: 2020 2020 7d0a 2020 2020 7075 6220 666e      }.    pub fn
-00001990: 2070 7562 6c69 635f 6d75 6c74 6928 2673   public_multi(&s
-000019a0: 656c 6629 202d 3e20 696d 706c 2049 7465  elf) -> impl Ite
-000019b0: 7261 746f 723c 4974 656d 203d 2028 2673  rator<Item = (&s
-000019c0: 7472 2c20 626f 6f6c 293e 207b 0a20 2020  tr, bool)> {.   
-000019d0: 2020 2020 2073 656c 662e 7075 626c 6963       self.public
-000019e0: 732e 6974 6572 2829 2e6d 6170 287c 286e  s.iter().map(|(n
-000019f0: 2c20 7629 7c20 286e 2e61 735f 7374 7228  , v)| (n.as_str(
-00001a00: 292c 2076 2e6d 756c 7469 2929 0a20 2020  ), v.multi)).   
-00001a10: 207d 0a20 2020 2070 7562 2066 6e20 6766   }.    pub fn gf
-00001a20: 5f6d 756c 7469 2826 7365 6c66 2920 2d3e  _multi(&self) ->
-00001a30: 2069 6d70 6c20 4974 6572 6174 6f72 3c49   impl Iterator<I
-00001a40: 7465 6d20 3d20 2826 7374 722c 2062 6f6f  tem = (&str, boo
-00001a50: 6c29 3e20 7b0a 2020 2020 2020 2020 7365  l)> {.        se
-00001a60: 6c66 2e67 656e 5f66 6163 746f 7273 2e69  lf.gen_factors.i
-00001a70: 7465 7228 292e 6d61 7028 7c28 6e2c 2076  ter().map(|(n, v
-00001a80: 297c 2028 6e2e 6173 5f73 7472 2829 2c20  )| (n.as_str(), 
-00001a90: 762e 6d75 6c74 6929 290a 2020 2020 7d0a  v.multi)).    }.
-00001aa0: 2020 2020 7075 6220 666e 2067 6574 5f76      pub fn get_v
-00001ab0: 6172 6964 2826 7365 6c66 2c20 7661 723a  arid(&self, var:
-00001ac0: 2026 7374 7229 202d 3e20 4647 5265 7375   &str) -> FGResu
-00001ad0: 6c74 3c56 6172 4964 3e20 7b0a 2020 2020  lt<VarId> {.    
-00001ae0: 2020 2020 7365 6c66 2e76 6172 730a 2020      self.vars.  
-00001af0: 2020 2020 2020 2020 2020 2e67 6574 5f69            .get_i
-00001b00: 6e64 6578 5f6f 6628 7661 7229 0a20 2020  ndex_of(var).   
-00001b10: 2020 2020 2020 2020 202e 6d61 7028 5661           .map(Va
-00001b20: 7249 643a 3a66 726f 6d5f 6964 7829 0a20  rId::from_idx). 
-00001b30: 2020 2020 2020 2020 2020 202e 6f6b 5f6f             .ok_o
-00001b40: 725f 656c 7365 287c 7c20 4647 4572 726f  r_else(|| FGErro
-00001b50: 723a 3a4e 6f56 6172 2876 6172 2e74 6f5f  r::NoVar(var.to_
-00001b60: 6f77 6e65 6428 2929 290a 2020 2020 7d0a  owned())).    }.
-00001b70: 2020 2020 7075 6228 7375 7065 7229 2066      pub(super) f
-00001b80: 6e20 7661 7228 2673 656c 662c 2076 6172  n var(&self, var
-00001b90: 3a20 5661 7249 6429 202d 3e20 2656 6172  : VarId) -> &Var
-00001ba0: 207b 0a20 2020 2020 2020 2026 7365 6c66   {.        &self
-00001bb0: 2e76 6172 735b 7661 722e 6964 7828 295d  .vars[var.idx()]
-00001bc0: 0a20 2020 207d 0a20 2020 2070 7562 2066  .    }.    pub f
-00001bd0: 6e20 7661 725f 6d75 6c74 6928 2673 656c  n var_multi(&sel
-00001be0: 662c 2076 6172 3a20 5661 7249 6429 202d  f, var: VarId) -
-00001bf0: 3e20 626f 6f6c 207b 0a20 2020 2020 2020  > bool {.       
-00001c00: 2073 656c 662e 7661 7228 7661 7229 2e6d   self.var(var).m
-00001c10: 756c 7469 0a20 2020 207d 0a20 2020 2070  ulti.    }.    p
-00001c20: 7562 2066 6e20 6661 6374 6f72 5f6d 756c  ub fn factor_mul
-00001c30: 7469 2826 7365 6c66 2c20 6661 6374 6f72  ti(&self, factor
-00001c40: 3a20 4661 6374 6f72 4964 2920 2d3e 2062  : FactorId) -> b
-00001c50: 6f6f 6c20 7b0a 2020 2020 2020 2020 7365  ool {.        se
-00001c60: 6c66 2e66 6163 746f 7228 6661 6374 6f72  lf.factor(factor
-00001c70: 292e 6d75 6c74 690a 2020 2020 7d0a 2020  ).multi.    }.  
-00001c80: 2020 7075 6220 666e 2065 6467 655f 6d75    pub fn edge_mu
-00001c90: 6c74 6928 2673 656c 662c 2065 6467 653a  lti(&self, edge:
-00001ca0: 2045 6467 6549 6429 202d 3e20 626f 6f6c   EdgeId) -> bool
-00001cb0: 207b 0a20 2020 2020 2020 2073 656c 662e   {.        self.
-00001cc0: 6661 6374 6f72 5f6d 756c 7469 2873 656c  factor_multi(sel
-00001cd0: 662e 6564 6765 735b 6564 6765 5d2e 6661  f.edges[edge].fa
-00001ce0: 6374 6f72 290a 2020 2020 7d0a 2020 2020  ctor).    }.    
-00001cf0: 7075 6220 666e 2072 616e 6765 5f76 6172  pub fn range_var
-00001d00: 7328 2673 656c 6629 202d 3e20 696d 706c  s(&self) -> impl
-00001d10: 2049 7465 7261 746f 723c 4974 656d 203d   Iterator<Item =
-00001d20: 2056 6172 4964 3e20 7b0a 2020 2020 2020   VarId> {.      
-00001d30: 2020 2830 2e2e 7365 6c66 2e76 6172 732e    (0..self.vars.
-00001d40: 6c65 6e28 2929 2e6d 6170 2856 6172 4964  len()).map(VarId
-00001d50: 3a3a 6672 6f6d 5f69 6478 290a 2020 2020  ::from_idx).    
-00001d60: 7d0a 2020 2020 7075 6220 666e 2072 616e  }.    pub fn ran
-00001d70: 6765 5f66 6163 746f 7273 2826 7365 6c66  ge_factors(&self
-00001d80: 2920 2d3e 2069 6d70 6c20 4974 6572 6174  ) -> impl Iterat
-00001d90: 6f72 3c49 7465 6d20 3d20 4661 6374 6f72  or<Item = Factor
-00001da0: 4964 3e20 7b0a 2020 2020 2020 2020 2830  Id> {.        (0
-00001db0: 2e2e 7365 6c66 2e66 6163 746f 7273 2e6c  ..self.factors.l
-00001dc0: 656e 2829 292e 6d61 7028 4661 6374 6f72  en()).map(Factor
-00001dd0: 4964 3a3a 6672 6f6d 5f69 6478 290a 2020  Id::from_idx).  
-00001de0: 2020 7d0a 2020 2020 7075 6228 7375 7065    }.    pub(supe
-00001df0: 7229 2066 6e20 6661 6374 6f72 2826 7365  r) fn factor(&se
-00001e00: 6c66 2c20 6661 6374 6f72 3a20 4661 6374  lf, factor: Fact
-00001e10: 6f72 4964 2920 2d3e 2026 4661 6374 6f72  orId) -> &Factor
-00001e20: 207b 0a20 2020 2020 2020 2026 7365 6c66   {.        &self
-00001e30: 2e66 6163 746f 7273 5b66 6163 746f 722e  .factors[factor.
-00001e40: 6964 7828 295d 0a20 2020 207d 0a20 2020  idx()].    }.   
-00001e50: 2070 7562 2066 6e20 6765 745f 6661 6374   pub fn get_fact
-00001e60: 6f72 6964 2826 7365 6c66 2c20 6661 6374  orid(&self, fact
-00001e70: 6f72 3a20 2673 7472 2920 2d3e 2046 4752  or: &str) -> FGR
-00001e80: 6573 756c 743c 4661 6374 6f72 4964 3e20  esult<FactorId> 
-00001e90: 7b0a 2020 2020 2020 2020 7365 6c66 2e66  {.        self.f
-00001ea0: 6163 746f 7273 0a20 2020 2020 2020 2020  actors.         
-00001eb0: 2020 202e 6765 745f 696e 6465 785f 6f66     .get_index_of
-00001ec0: 2866 6163 746f 7229 0a20 2020 2020 2020  (factor).       
-00001ed0: 2020 2020 202e 6d61 7028 4661 6374 6f72       .map(Factor
-00001ee0: 4964 3a3a 6672 6f6d 5f69 6478 290a 2020  Id::from_idx).  
-00001ef0: 2020 2020 2020 2020 2020 2e6f 6b5f 6f72            .ok_or
-00001f00: 5f65 6c73 6528 7c7c 2046 4745 7272 6f72  _else(|| FGError
-00001f10: 3a3a 4e6f 4661 6374 6f72 2866 6163 746f  ::NoFactor(facto
-00001f20: 722e 746f 5f6f 776e 6564 2829 2929 0a20  r.to_owned())). 
-00001f30: 2020 207d 0a20 2020 2070 7562 2066 6e20     }.    pub fn 
-00001f40: 7661 725f 6e61 6d65 7328 2673 656c 6629  var_names(&self)
-00001f50: 202d 3e20 696d 706c 2049 7465 7261 746f   -> impl Iterato
-00001f60: 723c 4974 656d 203d 2026 7374 723e 207b  r<Item = &str> {
-00001f70: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
-00001f80: 7273 2e6b 6579 7328 292e 6d61 7028 5374  rs.keys().map(St
-00001f90: 7269 6e67 3a3a 6173 5f73 7472 290a 2020  ring::as_str).  
-00001fa0: 2020 7d0a 2020 2020 7075 6220 666e 2076    }.    pub fn v
-00001fb0: 6172 7328 2673 656c 6629 202d 3e20 696d  ars(&self) -> im
-00001fc0: 706c 2049 7465 7261 746f 723c 4974 656d  pl Iterator<Item
-00001fd0: 203d 2028 5661 7249 642c 2026 7374 7229   = (VarId, &str)
-00001fe0: 3e20 7b0a 2020 2020 2020 2020 7365 6c66  > {.        self
-00001ff0: 2e76 6172 730a 2020 2020 2020 2020 2020  .vars.          
-00002000: 2020 2e6b 6579 7328 290a 2020 2020 2020    .keys().      
-00002010: 2020 2020 2020 2e65 6e75 6d65 7261 7465        .enumerate
-00002020: 2829 0a20 2020 2020 2020 2020 2020 202e  ().            .
-00002030: 6d61 7028 7c28 692c 2076 6e29 7c20 2856  map(|(i, vn)| (V
-00002040: 6172 4964 3a3a 6672 6f6d 5f69 6478 2869  arId::from_idx(i
-00002050: 292c 2076 6e2e 6173 5f73 7472 2829 2929  ), vn.as_str()))
-00002060: 0a20 2020 207d 0a20 2020 2070 7562 2066  .    }.    pub f
-00002070: 6e20 7661 725f 6e61 6d65 2826 7365 6c66  n var_name(&self
-00002080: 2c20 763a 2056 6172 4964 2920 2d3e 2026  , v: VarId) -> &
-00002090: 7374 7220 7b0a 2020 2020 2020 2020 7365  str {.        se
-000020a0: 6c66 2e76 6172 732e 6765 745f 696e 6465  lf.vars.get_inde
-000020b0: 7828 762e 6964 7828 2929 2e75 6e77 7261  x(v.idx()).unwra
-000020c0: 7028 292e 302e 6173 5f73 7472 2829 0a20  p().0.as_str(). 
-000020d0: 2020 207d 0a20 2020 2070 7562 2066 6e20     }.    pub fn 
-000020e0: 6661 6374 6f72 5f6e 616d 6573 2826 7365  factor_names(&se
-000020f0: 6c66 2920 2d3e 2069 6d70 6c20 4974 6572  lf) -> impl Iter
-00002100: 6174 6f72 3c49 7465 6d20 3d20 2673 7472  ator<Item = &str
-00002110: 3e20 7b0a 2020 2020 2020 2020 7365 6c66  > {.        self
-00002120: 2e66 6163 746f 7273 2e6b 6579 7328 292e  .factors.keys().
-00002130: 6d61 7028 5374 7269 6e67 3a3a 6173 5f73  map(String::as_s
-00002140: 7472 290a 2020 2020 7d0a 2020 2020 7075  tr).    }.    pu
-00002150: 6220 666e 2066 6163 746f 725f 6e61 6d65  b fn factor_name
-00002160: 2826 7365 6c66 2c20 663a 2046 6163 746f  (&self, f: Facto
-00002170: 7249 6429 202d 3e20 2673 7472 207b 0a20  rId) -> &str {. 
-00002180: 2020 2020 2020 2073 656c 662e 6661 6374         self.fact
-00002190: 6f72 732e 6765 745f 696e 6465 7828 662e  ors.get_index(f.
-000021a0: 6964 7828 2929 2e75 6e77 7261 7028 292e  idx()).unwrap().
-000021b0: 302e 6173 5f73 7472 2829 0a20 2020 207d  0.as_str().    }
-000021c0: 0a20 2020 2070 7562 2066 6e20 6661 6374  .    pub fn fact
-000021d0: 6f72 5f73 636f 7065 3c27 733e 2826 2773  or_scope<'s>(&'s
-000021e0: 2073 656c 662c 2066 6163 746f 723a 2046   self, factor: F
-000021f0: 6163 746f 7249 6429 202d 3e20 696d 706c  actorId) -> impl
-00002200: 2049 7465 7261 746f 723c 4974 656d 203d   Iterator<Item =
-00002210: 2056 6172 4964 3e20 2b20 2773 207b 0a20   VarId> + 's {. 
-00002220: 2020 2020 2020 2073 656c 662e 6661 6374         self.fact
-00002230: 6f72 2866 6163 746f 7229 2e65 6467 6573  or(factor).edges
-00002240: 2e6b 6579 7328 292e 636c 6f6e 6564 2829  .keys().cloned()
-00002250: 0a20 2020 207d 0a20 2020 2070 7562 2066  .    }.    pub f
-00002260: 6e20 7361 6e69 7479 5f63 6865 636b 280a  n sanity_check(.
-00002270: 2020 2020 2020 2020 2673 656c 662c 0a20          &self,. 
-00002280: 2020 2020 2020 2070 7562 6c69 635f 7661         public_va
-00002290: 6c75 6573 3a20 5665 633c 5075 626c 6963  lues: Vec<Public
-000022a0: 5661 6c75 653e 2c0a 2020 2020 2020 2020  Value>,.        
-000022b0: 7661 725f 6173 7369 676e 6d65 6e74 733a  var_assignments:
-000022c0: 2056 6172 5665 633c 5075 626c 6963 5661   VarVec<PublicVa
-000022d0: 6c75 653e 2c0a 2020 2020 2020 2020 6765  lue>,.        ge
-000022e0: 6e5f 6661 6374 6f72 733a 2056 6563 3c73  n_factors: Vec<s
-000022f0: 7570 6572 3a3a 4765 6e46 6163 746f 723e  uper::GenFactor>
-00002300: 2c0a 2020 2020 2920 2d3e 2046 4752 6573  ,.    ) -> FGRes
-00002310: 756c 743c 2829 3e20 7b0a 2020 2020 2020  ult<()> {.      
-00002320: 2020 6173 7365 7274 5f65 7121 2870 7562    assert_eq!(pub
-00002330: 6c69 635f 7661 6c75 6573 2e6c 656e 2829  lic_values.len()
-00002340: 2c20 7365 6c66 2e70 7562 6c69 6373 2e6c  , self.publics.l
-00002350: 656e 2829 293b 0a20 2020 2020 2020 2061  en());.        a
-00002360: 7373 6572 745f 6571 2128 7661 725f 6173  ssert_eq!(var_as
-00002370: 7369 676e 6d65 6e74 732e 6c65 6e28 292c  signments.len(),
-00002380: 2073 656c 662e 7661 7273 2e6c 656e 2829   self.vars.len()
-00002390: 293b 0a20 2020 2020 2020 206c 6574 2072  );.        let r
-000023a0: 6564 7563 6564 5f70 7562 203d 2073 656c  educed_pub = sel
-000023b0: 662e 7265 6475 6365 5f70 7562 2870 7562  f.reduce_pub(pub
-000023c0: 6c69 635f 7661 6c75 6573 2e61 735f 736c  lic_values.as_sl
-000023d0: 6963 6528 2929 3b0a 2020 2020 2020 2020  ice());.        
-000023e0: 666f 7220 2828 6661 6374 6f72 5f6e 616d  for ((factor_nam
-000023f0: 652c 2066 6163 746f 7229 2c20 6373 7429  e, factor), cst)
-00002400: 2069 6e20 7365 6c66 2e66 6163 746f 7273   in self.factors
-00002410: 2e69 7465 7228 292e 7a69 7028 7265 6475  .iter().zip(redu
-00002420: 6365 645f 7075 6229 207b 0a20 2020 2020  ced_pub) {.     
-00002430: 2020 2020 2020 206d 6174 6368 2026 6661         match &fa
-00002440: 6374 6f72 2e6b 696e 6420 7b0a 2020 2020  ctor.kind {.    
-00002450: 2020 2020 2020 2020 2020 2020 4661 6374              Fact
-00002460: 6f72 4b69 6e64 3a3a 4173 7369 676e 207b  orKind::Assign {
-00002470: 2065 7870 722c 2068 6173 5f72 6573 207d   expr, has_res }
-00002480: 203d 3e20 7b0a 2020 2020 2020 2020 2020   => {.          
-00002490: 2020 2020 2020 2020 2020 6c65 7420 6578            let ex
-000024a0: 7065 6374 6564 5f72 6573 203d 2066 6163  pected_res = fac
-000024b0: 746f 720a 2020 2020 2020 2020 2020 2020  tor.            
-000024c0: 2020 2020 2020 2020 2020 2020 2e72 6573              .res
-000024d0: 5f69 6428 290a 2020 2020 2020 2020 2020  _id().          
-000024e0: 2020 2020 2020 2020 2020 2020 2020 2e6d                .m
-000024f0: 6170 287c 765f 6964 7c20 2676 6172 5f61  ap(|v_id| &var_a
-00002500: 7373 6967 6e6d 656e 7473 5b76 5f69 645d  ssignments[v_id]
-00002510: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00002520: 2020 2020 2020 2020 2020 2e75 6e77 7261            .unwra
-00002530: 705f 6f72 2826 6373 7429 3b0a 2020 2020  p_or(&cst);.    
-00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002550: 6c65 7420 736b 6970 5f72 6573 203d 2069  let skip_res = i
-00002560: 6620 2a68 6173 5f72 6573 207b 2031 207d  f *has_res { 1 }
-00002570: 2065 6c73 6520 7b20 3020 7d3b 0a20 2020   else { 0 };.   
-00002580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002590: 206c 6574 206d 7574 206f 7073 203d 2066   let mut ops = f
-000025a0: 6163 746f 720a 2020 2020 2020 2020 2020  actor.          
-000025b0: 2020 2020 2020 2020 2020 2020 2020 2e65                .e
-000025c0: 6467 6573 0a20 2020 2020 2020 2020 2020  dges.           
-000025d0: 2020 2020 2020 2020 2020 2020 202e 6b65               .ke
-000025e0: 7973 2829 0a20 2020 2020 2020 2020 2020  ys().           
-000025f0: 2020 2020 2020 2020 2020 2020 202e 736b               .sk
-00002600: 6970 2873 6b69 705f 7265 7329 0a20 2020  ip(skip_res).   
-00002610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002620: 2020 2020 202e 6d61 7028 7c76 5f69 647c       .map(|v_id|
-00002630: 2026 7661 725f 6173 7369 676e 6d65 6e74   &var_assignment
-00002640: 735b 2a76 5f69 645d 293b 0a20 2020 2020  s[*v_id]);.     
-00002650: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00002660: 6574 2072 6573 203d 206d 6174 6368 2065  et res = match e
-00002670: 7870 7220 7b0a 2020 2020 2020 2020 2020  xpr {.          
-00002680: 2020 2020 2020 2020 2020 2020 2020 4578                Ex
-00002690: 7072 4661 6374 6f72 3a3a 414e 4420 7b20  prFactor::AND { 
-000026a0: 7661 7273 5f6e 6567 207d 203d 3e20 7b0a  vars_neg } => {.
+00000b80: 584f 5220 7c20 5365 6c66 3a3a 4144 4420  XOR | Self::ADD 
+00000b90: 7b20 7661 7273 5f6e 6567 3a20 5f20 7d20  { vars_neg: _ } 
+00000ba0: 3d3e 2030 2c0a 2020 2020 2020 2020 2020  => 0,.          
+00000bb0: 2020 5365 6c66 3a3a 4d55 4c20 3d3e 2031    Self::MUL => 1
+00000bc0: 2c0a 2020 2020 2020 2020 2020 2020 5365  ,.            Se
+00000bd0: 6c66 3a3a 4e4f 5420 7c20 5365 6c66 3a3a  lf::NOT | Self::
+00000be0: 4c4f 4f4b 5550 207b 202e 2e20 7d20 3d3e  LOOKUP { .. } =>
+00000bf0: 2075 6e72 6561 6368 6162 6c65 2128 292c   unreachable!(),
+00000c00: 0a20 2020 2020 2020 207d 0a20 2020 207d  .        }.    }
+00000c10: 0a7d 0a0a 235b 6465 7269 7665 2844 6562  .}..#[derive(Deb
+00000c20: 7567 2c20 436c 6f6e 652c 2073 6572 6465  ug, Clone, serde
+00000c30: 3a3a 5365 7269 616c 697a 652c 2073 6572  ::Serialize, ser
+00000c40: 6465 3a3a 4465 7365 7269 616c 697a 6529  de::Deserialize)
+00000c50: 5d0a 7075 6228 7375 7065 7229 2073 7472  ].pub(super) str
+00000c60: 7563 7420 4564 6765 207b 0a20 2020 2070  uct Edge {.    p
+00000c70: 7562 2873 7570 6572 2920 7661 723a 2056  ub(super) var: V
+00000c80: 6172 4964 2c0a 2020 2020 7075 6228 7375  arId,.    pub(su
+00000c90: 7065 7229 2070 6f73 5f76 6172 3a20 7573  per) pos_var: us
+00000ca0: 697a 652c 0a20 2020 2070 7562 2873 7570  ize,.    pub(sup
+00000cb0: 6572 2920 6661 6374 6f72 3a20 4661 6374  er) factor: Fact
+00000cc0: 6f72 4964 2c0a 2020 2020 7075 6228 7375  orId,.    pub(su
+00000cd0: 7065 7229 2070 6f73 5f66 6163 746f 723a  per) pos_factor:
+00000ce0: 2075 7369 7a65 2c0a 7d0a 0a23 5b64 6572   usize,.}..#[der
+00000cf0: 6976 6528 4465 6275 672c 2043 6c6f 6e65  ive(Debug, Clone
+00000d00: 2c20 7365 7264 653a 3a53 6572 6961 6c69  , serde::Seriali
+00000d10: 7a65 2c20 7365 7264 653a 3a44 6573 6572  ze, serde::Deser
+00000d20: 6961 6c69 7a65 295d 0a70 7562 2873 7570  ialize)].pub(sup
+00000d30: 6572 2920 7374 7275 6374 2050 7562 6c69  er) struct Publi
+00000d40: 6320 7b0a 2020 2020 7075 6228 7375 7065  c {.    pub(supe
+00000d50: 7229 206d 756c 7469 3a20 626f 6f6c 2c0a  r) multi: bool,.
+00000d60: 7d0a 0a23 5b64 6572 6976 6528 4465 6275  }..#[derive(Debu
+00000d70: 672c 2043 6c6f 6e65 2c20 7365 7264 653a  g, Clone, serde:
+00000d80: 3a53 6572 6961 6c69 7a65 2c20 7365 7264  :Serialize, serd
+00000d90: 653a 3a44 6573 6572 6961 6c69 7a65 295d  e::Deserialize)]
+00000da0: 0a70 7562 2873 7570 6572 2920 7374 7275  .pub(super) stru
+00000db0: 6374 2047 656e 4661 6374 6f72 207b 0a20  ct GenFactor {. 
+00000dc0: 2020 2070 7562 2873 7570 6572 2920 6d75     pub(super) mu
+00000dd0: 6c74 693a 2062 6f6f 6c2c 0a7d 0a0a 235b  lti: bool,.}..#[
+00000de0: 6465 7269 7665 2844 6562 7567 2c20 436c  derive(Debug, Cl
+00000df0: 6f6e 652c 2073 6572 6465 3a3a 5365 7269  one, serde::Seri
+00000e00: 616c 697a 652c 2073 6572 6465 3a3a 4465  alize, serde::De
+00000e10: 7365 7269 616c 697a 6529 5d0a 7075 6228  serialize)].pub(
+00000e20: 7375 7065 7229 2073 7472 7563 7420 5461  super) struct Ta
+00000e30: 626c 6520 7b0a 2020 2020 7075 6228 7375  ble {.    pub(su
+00000e40: 7065 7229 2076 616c 7565 733a 2056 6563  per) values: Vec
+00000e50: 3c43 6c61 7373 5661 6c3e 2c0a 7d0a 0a23  <ClassVal>,.}..#
+00000e60: 5b64 6572 6976 6528 4465 6275 672c 2043  [derive(Debug, C
+00000e70: 6f70 792c 2043 6c6f 6e65 2c20 7365 7264  opy, Clone, serd
+00000e80: 653a 3a53 6572 6961 6c69 7a65 2c20 7365  e::Serialize, se
+00000e90: 7264 653a 3a44 6573 6572 6961 6c69 7a65  rde::Deserialize
+00000ea0: 295d 0a70 7562 2873 7570 6572 2920 656e  )].pub(super) en
+00000eb0: 756d 204e 6f64 6520 7b0a 2020 2020 5661  um Node {.    Va
+00000ec0: 7228 5661 7249 6429 2c0a 2020 2020 4661  r(VarId),.    Fa
+00000ed0: 6374 6f72 2846 6163 746f 7249 6429 2c0a  ctor(FactorId),.
+00000ee0: 7d0a 0a23 5b64 6572 6976 6528 4465 6275  }..#[derive(Debu
+00000ef0: 672c 2043 6c6f 6e65 2c20 7365 7264 653a  g, Clone, serde:
+00000f00: 3a53 6572 6961 6c69 7a65 2c20 7365 7264  :Serialize, serd
+00000f10: 653a 3a44 6573 6572 6961 6c69 7a65 295d  e::Deserialize)]
+00000f20: 0a70 7562 2073 7472 7563 7420 4661 6374  .pub struct Fact
+00000f30: 6f72 4772 6170 6820 7b0a 2020 2020 7075  orGraph {.    pu
+00000f40: 6228 7375 7065 7229 206e 633a 2075 7369  b(super) nc: usi
+00000f50: 7a65 2c0a 2020 2020 7075 6228 7375 7065  ze,.    pub(supe
+00000f60: 7229 2076 6172 733a 204e 616d 6564 4c69  r) vars: NamedLi
+00000f70: 7374 3c56 6172 3e2c 0a20 2020 2070 7562  st<Var>,.    pub
+00000f80: 2873 7570 6572 2920 6661 6374 6f72 733a  (super) factors:
+00000f90: 204e 616d 6564 4c69 7374 3c46 6163 746f   NamedList<Facto
+00000fa0: 723e 2c0a 2020 2020 7075 6228 7375 7065  r>,.    pub(supe
+00000fb0: 7229 2065 6467 6573 3a20 4564 6765 5665  r) edges: EdgeVe
+00000fc0: 633c 4564 6765 3e2c 0a20 2020 2070 7562  c<Edge>,.    pub
+00000fd0: 2873 7570 6572 2920 7075 626c 6963 733a  (super) publics:
+00000fe0: 204e 616d 6564 4c69 7374 3c50 7562 6c69   NamedList<Publi
+00000ff0: 633e 2c0a 2020 2020 7075 6228 7375 7065  c>,.    pub(supe
+00001000: 7229 2074 6162 6c65 733a 204e 616d 6564  r) tables: Named
+00001010: 4c69 7374 3c54 6162 6c65 3e2c 0a20 2020  List<Table>,.   
+00001020: 2070 7562 2873 7570 6572 2920 6765 6e5f   pub(super) gen_
+00001030: 6661 6374 6f72 733a 204e 616d 6564 4c69  factors: NamedLi
+00001040: 7374 3c47 656e 4661 6374 6f72 3e2c 0a20  st<GenFactor>,. 
+00001050: 2020 2070 7562 2873 7570 6572 2920 7065     pub(super) pe
+00001060: 7467 7261 7068 3a20 7065 7467 7261 7068  tgraph: petgraph
+00001070: 3a3a 4772 6170 683c 4e6f 6465 2c20 4564  ::Graph<Node, Ed
+00001080: 6765 4964 2c20 7065 7467 7261 7068 3a3a  geId, petgraph::
+00001090: 556e 6469 7265 6374 6564 3e2c 0a20 2020  Undirected>,.   
+000010a0: 2070 7562 2873 7570 6572 2920 7661 725f   pub(super) var_
+000010b0: 6772 6170 685f 6964 733a 2056 6172 5665  graph_ids: VarVe
+000010c0: 633c 7065 7467 7261 7068 3a3a 6772 6170  c<petgraph::grap
+000010d0: 683a 3a4e 6f64 6549 6e64 6578 3e2c 0a20  h::NodeIndex>,. 
+000010e0: 2020 2070 7562 2873 7570 6572 2920 6661     pub(super) fa
+000010f0: 6374 6f72 5f67 7261 7068 5f69 6473 3a20  ctor_graph_ids: 
+00001100: 4661 6374 6f72 5665 633c 7065 7467 7261  FactorVec<petgra
+00001110: 7068 3a3a 6772 6170 683a 3a4e 6f64 6549  ph::graph::NodeI
+00001120: 6e64 6578 3e2c 0a20 2020 2070 7562 2873  ndex>,.    pub(s
+00001130: 7570 6572 2920 6379 636c 6963 5f73 696e  uper) cyclic_sin
+00001140: 676c 653a 2062 6f6f 6c2c 0a20 2020 2070  gle: bool,.    p
+00001150: 7562 2873 7570 6572 2920 6379 636c 6963  ub(super) cyclic
+00001160: 5f6d 756c 7469 3a20 626f 6f6c 2c0a 7d0a  _multi: bool,.}.
+00001170: 0a23 5b64 6572 6976 6528 4465 6275 672c  .#[derive(Debug,
+00001180: 2043 6c6f 6e65 2c20 4571 2c20 5061 7274   Clone, Eq, Part
+00001190: 6961 6c45 712c 2073 6572 6465 3a3a 5365  ialEq, serde::Se
+000011a0: 7269 616c 697a 652c 2073 6572 6465 3a3a  rialize, serde::
+000011b0: 4465 7365 7269 616c 697a 6529 5d0a 7075  Deserialize)].pu
+000011c0: 6220 656e 756d 2050 7562 6c69 6356 616c  b enum PublicVal
+000011d0: 7565 207b 0a20 2020 2053 696e 676c 6528  ue {.    Single(
+000011e0: 436c 6173 7356 616c 292c 0a20 2020 204d  ClassVal),.    M
+000011f0: 756c 7469 2856 6563 3c43 6c61 7373 5661  ulti(Vec<ClassVa
+00001200: 6c3e 292c 0a7d 0a69 6d70 6c20 5075 626c  l>),.}.impl Publ
+00001210: 6963 5661 6c75 6520 7b0a 2020 2020 7075  icValue {.    pu
+00001220: 6220 666e 2061 735f 736c 6963 6528 2673  b fn as_slice(&s
+00001230: 656c 6629 202d 3e20 265b 436c 6173 7356  elf) -> &[ClassV
+00001240: 616c 5d20 7b0a 2020 2020 2020 2020 6d61  al] {.        ma
+00001250: 7463 6820 7365 6c66 207b 0a20 2020 2020  tch self {.     
+00001260: 2020 2020 2020 2050 7562 6c69 6356 616c         PublicVal
+00001270: 7565 3a3a 5369 6e67 6c65 2878 2920 3d3e  ue::Single(x) =>
+00001280: 2073 7464 3a3a 736c 6963 653a 3a66 726f   std::slice::fro
+00001290: 6d5f 7265 6628 7829 2c0a 2020 2020 2020  m_ref(x),.      
+000012a0: 2020 2020 2020 5075 626c 6963 5661 6c75        PublicValu
+000012b0: 653a 3a4d 756c 7469 2878 2920 3d3e 2078  e::Multi(x) => x
+000012c0: 2e61 735f 736c 6963 6528 292c 0a20 2020  .as_slice(),.   
+000012d0: 2020 2020 207d 0a20 2020 207d 0a20 2020       }.    }.   
+000012e0: 2070 7562 2066 6e20 6974 6572 2826 7365   pub fn iter(&se
+000012f0: 6c66 2c20 6e3a 2075 7369 7a65 2920 2d3e  lf, n: usize) ->
+00001300: 2069 6d70 6c20 4974 6572 6174 6f72 3c49   impl Iterator<I
+00001310: 7465 6d20 3d20 436c 6173 7356 616c 3e20  tem = ClassVal> 
+00001320: 2b20 275f 207b 0a20 2020 2020 2020 2069  + '_ {.        i
+00001330: 6620 6c65 7420 5075 626c 6963 5661 6c75  f let PublicValu
+00001340: 653a 3a4d 756c 7469 2878 2920 3d20 7365  e::Multi(x) = se
+00001350: 6c66 207b 0a20 2020 2020 2020 2020 2020  lf {.           
+00001360: 2061 7373 6572 745f 6571 2128 782e 6c65   assert_eq!(x.le
+00001370: 6e28 292c 206e 293b 0a20 2020 2020 2020  n(), n);.       
+00001380: 207d 0a20 2020 2020 2020 2028 302e 2e6e   }.        (0..n
+00001390: 292e 6d61 7028 7c69 7c20 7365 6c66 2e67  ).map(|i| self.g
+000013a0: 6574 2869 2929 0a20 2020 207d 0a20 2020  et(i)).    }.   
+000013b0: 2070 7562 2066 6e20 6765 7428 2673 656c   pub fn get(&sel
+000013c0: 662c 206e 3a20 7573 697a 6529 202d 3e20  f, n: usize) -> 
+000013d0: 436c 6173 7356 616c 207b 0a20 2020 2020  ClassVal {.     
+000013e0: 2020 206d 6174 6368 2073 656c 6620 7b0a     match self {.
+000013f0: 2020 2020 2020 2020 2020 2020 5075 626c              Publ
+00001400: 6963 5661 6c75 653a 3a53 696e 676c 6528  icValue::Single(
+00001410: 7829 203d 3e20 2a78 2c0a 2020 2020 2020  x) => *x,.      
+00001420: 2020 2020 2020 5075 626c 6963 5661 6c75        PublicValu
+00001430: 653a 3a4d 756c 7469 2878 2920 3d3e 2078  e::Multi(x) => x
+00001440: 5b6e 5d2c 0a20 2020 2020 2020 207d 0a20  [n],.        }. 
+00001450: 2020 207d 0a20 2020 2070 7562 2066 6e20     }.    pub fn 
+00001460: 6d61 7028 2673 656c 662c 2066 3a20 696d  map(&self, f: im
+00001470: 706c 2046 6e28 436c 6173 7356 616c 2920  pl Fn(ClassVal) 
+00001480: 2d3e 2043 6c61 7373 5661 6c29 202d 3e20  -> ClassVal) -> 
+00001490: 5365 6c66 207b 0a20 2020 2020 2020 206d  Self {.        m
+000014a0: 6174 6368 2073 656c 6620 7b0a 2020 2020  atch self {.    
+000014b0: 2020 2020 2020 2020 5075 626c 6963 5661          PublicVa
+000014c0: 6c75 653a 3a53 696e 676c 6528 7829 203d  lue::Single(x) =
+000014d0: 3e20 5075 626c 6963 5661 6c75 653a 3a53  > PublicValue::S
+000014e0: 696e 676c 6528 6628 2a78 2929 2c0a 2020  ingle(f(*x)),.  
+000014f0: 2020 2020 2020 2020 2020 5075 626c 6963            Public
+00001500: 5661 6c75 653a 3a4d 756c 7469 2878 2920  Value::Multi(x) 
+00001510: 3d3e 2050 7562 6c69 6356 616c 7565 3a3a  => PublicValue::
+00001520: 4d75 6c74 6928 782e 6974 6572 2829 2e63  Multi(x.iter().c
+00001530: 6c6f 6e65 6428 292e 6d61 7028 6629 2e63  loned().map(f).c
+00001540: 6f6c 6c65 6374 2829 292c 0a20 2020 2020  ollect()),.     
+00001550: 2020 207d 0a20 2020 207d 0a7d 0a69 6d70     }.    }.}.imp
+00001560: 6c20 666d 743a 3a44 6973 706c 6179 2066  l fmt::Display f
+00001570: 6f72 2050 7562 6c69 6356 616c 7565 207b  or PublicValue {
+00001580: 0a20 2020 2066 6e20 666d 7428 2673 656c  .    fn fmt(&sel
+00001590: 662c 2066 3a20 266d 7574 2066 6d74 3a3a  f, f: &mut fmt::
+000015a0: 466f 726d 6174 7465 723c 275f 3e29 202d  Formatter<'_>) -
+000015b0: 3e20 666d 743a 3a52 6573 756c 7420 7b0a  > fmt::Result {.
+000015c0: 2020 2020 2020 2020 6d61 7463 6820 7365          match se
+000015d0: 6c66 207b 0a20 2020 2020 2020 2020 2020  lf {.           
+000015e0: 2050 7562 6c69 6356 616c 7565 3a3a 5369   PublicValue::Si
+000015f0: 6e67 6c65 2878 2920 3d3e 2077 7269 7465  ngle(x) => write
+00001600: 2128 662c 2022 7b7d 222c 2078 292c 0a20  !(f, "{}", x),. 
+00001610: 2020 2020 2020 2020 2020 2050 7562 6c69             Publi
+00001620: 6356 616c 7565 3a3a 4d75 6c74 6928 7829  cValue::Multi(x)
+00001630: 203d 3e20 7772 6974 6521 2866 2c20 227b   => write!(f, "{
+00001640: 3a3f 7d22 2c20 782e 6173 5f73 6c69 6365  :?}", x.as_slice
+00001650: 2829 292c 0a20 2020 2020 2020 207d 0a20  ()),.        }. 
+00001660: 2020 207d 0a7d 0a0a 235b 6465 7269 7665     }.}..#[derive
+00001670: 2844 6562 7567 2c20 436c 6f6e 652c 2045  (Debug, Clone, E
+00001680: 7272 6f72 295d 0a70 7562 2065 6e75 6d20  rror)].pub enum 
+00001690: 4647 4572 726f 7220 7b0a 2020 2020 235b  FGError {.    #[
+000016a0: 6572 726f 7228 224e 6f20 7661 7269 6162  error("No variab
+000016b0: 6c65 206e 616d 6564 207b 307d 2e22 295d  le named {0}.")]
+000016c0: 0a20 2020 204e 6f56 6172 2853 7472 696e  .    NoVar(Strin
+000016d0: 6729 2c0a 2020 2020 235b 6572 726f 7228  g),.    #[error(
+000016e0: 224e 6f20 6661 6374 6f72 206e 616d 6564  "No factor named
+000016f0: 207b 307d 2e22 295d 0a20 2020 204e 6f46   {0}.")].    NoF
+00001700: 6163 746f 7228 5374 7269 6e67 292c 0a20  actor(String),. 
+00001710: 2020 2023 5b65 7272 6f72 2822 4e6f 2065     #[error("No e
+00001720: 6467 6520 6265 7477 6565 6e20 7661 7269  dge between vari
+00001730: 6162 6c65 207b 7661 727d 2061 6e64 2066  able {var} and f
+00001740: 6163 746f 7220 7b66 6163 746f 727d 2e22  actor {factor}."
+00001750: 295d 0a20 2020 204e 6f45 6467 6520 7b20  )].    NoEdge { 
+00001760: 7661 723a 2053 7472 696e 672c 2066 6163  var: String, fac
+00001770: 746f 723a 2046 6163 746f 7249 6420 7d2c  tor: FactorId },
+00001780: 0a20 2020 2023 5b65 7272 6f72 2822 4661  .    #[error("Fa
+00001790: 696c 7572 6520 6174 2066 6163 746f 7220  ilure at factor 
+000017a0: 7b30 7d2e 2045 7870 6563 7465 6420 7265  {0}. Expected re
+000017b0: 7375 6c74 207b 317d 2c20 676f 7420 7b32  sult {1}, got {2
+000017c0: 7d2e 2229 5d0a 2020 2020 4368 6563 6b46  }.")].    CheckF
+000017d0: 6169 6c28 5374 7269 6e67 2c20 5075 626c  ail(String, Publ
+000017e0: 6963 5661 6c75 652c 2050 7562 6c69 6356  icValue, PublicV
+000017f0: 616c 7565 292c 0a20 2020 2023 5b65 7272  alue),.    #[err
+00001800: 6f72 2822 2229 5d0a 2020 2020 496e 7661  or("")].    Inva
+00001810: 6c69 6447 656e 6572 6963 4661 6374 6f72  lidGenericFactor
+00001820: 4173 7369 676e 6d65 6e74 2853 7472 696e  Assignment(Strin
+00001830: 6729 2c0a 7d0a 0a74 7970 6520 4647 5265  g),.}..type FGRe
+00001840: 7375 6c74 3c54 3e20 3d20 5265 7375 6c74  sult<T> = Result
+00001850: 3c54 2c20 4647 4572 726f 723e 3b0a 0a69  <T, FGError>;..i
+00001860: 6d70 6c20 4661 6374 6f72 4772 6170 6820  mpl FactorGraph 
+00001870: 7b0a 2020 2020 7075 6220 666e 2065 6467  {.    pub fn edg
+00001880: 6528 2673 656c 662c 2076 6172 3a20 5661  e(&self, var: Va
+00001890: 7249 642c 2066 6163 746f 723a 2046 6163  rId, factor: Fac
+000018a0: 746f 7249 6429 202d 3e20 4647 5265 7375  torId) -> FGResu
+000018b0: 6c74 3c45 6467 6549 643e 207b 0a20 2020  lt<EdgeId> {.   
+000018c0: 2020 2020 2073 656c 662e 7661 7228 7661       self.var(va
+000018d0: 7229 0a20 2020 2020 2020 2020 2020 202e  r).            .
+000018e0: 6564 6765 730a 2020 2020 2020 2020 2020  edges.          
+000018f0: 2020 2e67 6574 2826 6661 6374 6f72 290a    .get(&factor).
+00001900: 2020 2020 2020 2020 2020 2020 2e6d 6170              .map
+00001910: 287c 657c 202a 6529 0a20 2020 2020 2020  (|e| *e).       
+00001920: 2020 2020 202e 6f6b 5f6f 725f 656c 7365       .ok_or_else
+00001930: 287c 7c20 4647 4572 726f 723a 3a4e 6f45  (|| FGError::NoE
+00001940: 6467 6520 7b0a 2020 2020 2020 2020 2020  dge {.          
+00001950: 2020 2020 2020 7661 723a 2073 656c 662e        var: self.
+00001960: 7661 7273 2e67 6574 5f69 6e64 6578 2876  vars.get_index(v
+00001970: 6172 2e69 6478 2829 292e 756e 7772 6170  ar.idx()).unwrap
+00001980: 2829 2e30 2e74 6f5f 6f77 6e65 6428 292c  ().0.to_owned(),
+00001990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000019a0: 2066 6163 746f 722c 0a20 2020 2020 2020   factor,.       
+000019b0: 2020 2020 207d 290a 2020 2020 7d0a 2020       }).    }.  
+000019c0: 2020 7075 6220 666e 2070 7562 6c69 635f    pub fn public_
+000019d0: 6d75 6c74 6928 2673 656c 6629 202d 3e20  multi(&self) -> 
+000019e0: 696d 706c 2049 7465 7261 746f 723c 4974  impl Iterator<It
+000019f0: 656d 203d 2028 2673 7472 2c20 626f 6f6c  em = (&str, bool
+00001a00: 293e 207b 0a20 2020 2020 2020 2073 656c  )> {.        sel
+00001a10: 662e 7075 626c 6963 732e 6974 6572 2829  f.publics.iter()
+00001a20: 2e6d 6170 287c 286e 2c20 7629 7c20 286e  .map(|(n, v)| (n
+00001a30: 2e61 735f 7374 7228 292c 2076 2e6d 756c  .as_str(), v.mul
+00001a40: 7469 2929 0a20 2020 207d 0a20 2020 2070  ti)).    }.    p
+00001a50: 7562 2066 6e20 6766 5f6d 756c 7469 2826  ub fn gf_multi(&
+00001a60: 7365 6c66 2920 2d3e 2069 6d70 6c20 4974  self) -> impl It
+00001a70: 6572 6174 6f72 3c49 7465 6d20 3d20 2826  erator<Item = (&
+00001a80: 7374 722c 2062 6f6f 6c29 3e20 7b0a 2020  str, bool)> {.  
+00001a90: 2020 2020 2020 7365 6c66 2e67 656e 5f66        self.gen_f
+00001aa0: 6163 746f 7273 2e69 7465 7228 292e 6d61  actors.iter().ma
+00001ab0: 7028 7c28 6e2c 2076 297c 2028 6e2e 6173  p(|(n, v)| (n.as
+00001ac0: 5f73 7472 2829 2c20 762e 6d75 6c74 6929  _str(), v.multi)
+00001ad0: 290a 2020 2020 7d0a 2020 2020 7075 6220  ).    }.    pub 
+00001ae0: 666e 2067 6574 5f76 6172 6964 2826 7365  fn get_varid(&se
+00001af0: 6c66 2c20 7661 723a 2026 7374 7229 202d  lf, var: &str) -
+00001b00: 3e20 4647 5265 7375 6c74 3c56 6172 4964  > FGResult<VarId
+00001b10: 3e20 7b0a 2020 2020 2020 2020 7365 6c66  > {.        self
+00001b20: 2e76 6172 730a 2020 2020 2020 2020 2020  .vars.          
+00001b30: 2020 2e67 6574 5f69 6e64 6578 5f6f 6628    .get_index_of(
+00001b40: 7661 7229 0a20 2020 2020 2020 2020 2020  var).           
+00001b50: 202e 6d61 7028 5661 7249 643a 3a66 726f   .map(VarId::fro
+00001b60: 6d5f 6964 7829 0a20 2020 2020 2020 2020  m_idx).         
+00001b70: 2020 202e 6f6b 5f6f 725f 656c 7365 287c     .ok_or_else(|
+00001b80: 7c20 4647 4572 726f 723a 3a4e 6f56 6172  | FGError::NoVar
+00001b90: 2876 6172 2e74 6f5f 6f77 6e65 6428 2929  (var.to_owned())
+00001ba0: 290a 2020 2020 7d0a 2020 2020 7075 6228  ).    }.    pub(
+00001bb0: 7375 7065 7229 2066 6e20 7661 7228 2673  super) fn var(&s
+00001bc0: 656c 662c 2076 6172 3a20 5661 7249 6429  elf, var: VarId)
+00001bd0: 202d 3e20 2656 6172 207b 0a20 2020 2020   -> &Var {.     
+00001be0: 2020 2026 7365 6c66 2e76 6172 735b 7661     &self.vars[va
+00001bf0: 722e 6964 7828 295d 0a20 2020 207d 0a20  r.idx()].    }. 
+00001c00: 2020 2070 7562 2066 6e20 7661 725f 6d75     pub fn var_mu
+00001c10: 6c74 6928 2673 656c 662c 2076 6172 3a20  lti(&self, var: 
+00001c20: 5661 7249 6429 202d 3e20 626f 6f6c 207b  VarId) -> bool {
+00001c30: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+00001c40: 7228 7661 7229 2e6d 756c 7469 0a20 2020  r(var).multi.   
+00001c50: 207d 0a20 2020 2070 7562 2066 6e20 6661   }.    pub fn fa
+00001c60: 6374 6f72 5f6d 756c 7469 2826 7365 6c66  ctor_multi(&self
+00001c70: 2c20 6661 6374 6f72 3a20 4661 6374 6f72  , factor: Factor
+00001c80: 4964 2920 2d3e 2062 6f6f 6c20 7b0a 2020  Id) -> bool {.  
+00001c90: 2020 2020 2020 7365 6c66 2e66 6163 746f        self.facto
+00001ca0: 7228 6661 6374 6f72 292e 6d75 6c74 690a  r(factor).multi.
+00001cb0: 2020 2020 7d0a 2020 2020 7075 6220 666e      }.    pub fn
+00001cc0: 2065 6467 655f 6d75 6c74 6928 2673 656c   edge_multi(&sel
+00001cd0: 662c 2065 6467 653a 2045 6467 6549 6429  f, edge: EdgeId)
+00001ce0: 202d 3e20 626f 6f6c 207b 0a20 2020 2020   -> bool {.     
+00001cf0: 2020 2073 656c 662e 6661 6374 6f72 5f6d     self.factor_m
+00001d00: 756c 7469 2873 656c 662e 6564 6765 735b  ulti(self.edges[
+00001d10: 6564 6765 5d2e 6661 6374 6f72 290a 2020  edge].factor).  
+00001d20: 2020 7d0a 2020 2020 7075 6220 666e 2072    }.    pub fn r
+00001d30: 616e 6765 5f76 6172 7328 2673 656c 6629  ange_vars(&self)
+00001d40: 202d 3e20 696d 706c 2049 7465 7261 746f   -> impl Iterato
+00001d50: 723c 4974 656d 203d 2056 6172 4964 3e20  r<Item = VarId> 
+00001d60: 7b0a 2020 2020 2020 2020 2830 2e2e 7365  {.        (0..se
+00001d70: 6c66 2e76 6172 732e 6c65 6e28 2929 2e6d  lf.vars.len()).m
+00001d80: 6170 2856 6172 4964 3a3a 6672 6f6d 5f69  ap(VarId::from_i
+00001d90: 6478 290a 2020 2020 7d0a 2020 2020 7075  dx).    }.    pu
+00001da0: 6220 666e 2072 616e 6765 5f66 6163 746f  b fn range_facto
+00001db0: 7273 2826 7365 6c66 2920 2d3e 2069 6d70  rs(&self) -> imp
+00001dc0: 6c20 4974 6572 6174 6f72 3c49 7465 6d20  l Iterator<Item 
+00001dd0: 3d20 4661 6374 6f72 4964 3e20 7b0a 2020  = FactorId> {.  
+00001de0: 2020 2020 2020 2830 2e2e 7365 6c66 2e66        (0..self.f
+00001df0: 6163 746f 7273 2e6c 656e 2829 292e 6d61  actors.len()).ma
+00001e00: 7028 4661 6374 6f72 4964 3a3a 6672 6f6d  p(FactorId::from
+00001e10: 5f69 6478 290a 2020 2020 7d0a 2020 2020  _idx).    }.    
+00001e20: 7075 6228 7375 7065 7229 2066 6e20 6661  pub(super) fn fa
+00001e30: 6374 6f72 2826 7365 6c66 2c20 6661 6374  ctor(&self, fact
+00001e40: 6f72 3a20 4661 6374 6f72 4964 2920 2d3e  or: FactorId) ->
+00001e50: 2026 4661 6374 6f72 207b 0a20 2020 2020   &Factor {.     
+00001e60: 2020 2026 7365 6c66 2e66 6163 746f 7273     &self.factors
+00001e70: 5b66 6163 746f 722e 6964 7828 295d 0a20  [factor.idx()]. 
+00001e80: 2020 207d 0a20 2020 2070 7562 2066 6e20     }.    pub fn 
+00001e90: 6765 745f 6661 6374 6f72 6964 2826 7365  get_factorid(&se
+00001ea0: 6c66 2c20 6661 6374 6f72 3a20 2673 7472  lf, factor: &str
+00001eb0: 2920 2d3e 2046 4752 6573 756c 743c 4661  ) -> FGResult<Fa
+00001ec0: 6374 6f72 4964 3e20 7b0a 2020 2020 2020  ctorId> {.      
+00001ed0: 2020 7365 6c66 2e66 6163 746f 7273 0a20    self.factors. 
+00001ee0: 2020 2020 2020 2020 2020 202e 6765 745f             .get_
+00001ef0: 696e 6465 785f 6f66 2866 6163 746f 7229  index_of(factor)
+00001f00: 0a20 2020 2020 2020 2020 2020 202e 6d61  .            .ma
+00001f10: 7028 4661 6374 6f72 4964 3a3a 6672 6f6d  p(FactorId::from
+00001f20: 5f69 6478 290a 2020 2020 2020 2020 2020  _idx).          
+00001f30: 2020 2e6f 6b5f 6f72 5f65 6c73 6528 7c7c    .ok_or_else(||
+00001f40: 2046 4745 7272 6f72 3a3a 4e6f 4661 6374   FGError::NoFact
+00001f50: 6f72 2866 6163 746f 722e 746f 5f6f 776e  or(factor.to_own
+00001f60: 6564 2829 2929 0a20 2020 207d 0a20 2020  ed())).    }.   
+00001f70: 2070 7562 2066 6e20 7661 725f 6e61 6d65   pub fn var_name
+00001f80: 7328 2673 656c 6629 202d 3e20 696d 706c  s(&self) -> impl
+00001f90: 2049 7465 7261 746f 723c 4974 656d 203d   Iterator<Item =
+00001fa0: 2026 7374 723e 207b 0a20 2020 2020 2020   &str> {.       
+00001fb0: 2073 656c 662e 7661 7273 2e6b 6579 7328   self.vars.keys(
+00001fc0: 292e 6d61 7028 5374 7269 6e67 3a3a 6173  ).map(String::as
+00001fd0: 5f73 7472 290a 2020 2020 7d0a 2020 2020  _str).    }.    
+00001fe0: 7075 6220 666e 2076 6172 7328 2673 656c  pub fn vars(&sel
+00001ff0: 6629 202d 3e20 696d 706c 2049 7465 7261  f) -> impl Itera
+00002000: 746f 723c 4974 656d 203d 2028 5661 7249  tor<Item = (VarI
+00002010: 642c 2026 7374 7229 3e20 7b0a 2020 2020  d, &str)> {.    
+00002020: 2020 2020 7365 6c66 2e76 6172 730a 2020      self.vars.  
+00002030: 2020 2020 2020 2020 2020 2e6b 6579 7328            .keys(
+00002040: 290a 2020 2020 2020 2020 2020 2020 2e65  ).            .e
+00002050: 6e75 6d65 7261 7465 2829 0a20 2020 2020  numerate().     
+00002060: 2020 2020 2020 202e 6d61 7028 7c28 692c         .map(|(i,
+00002070: 2076 6e29 7c20 2856 6172 4964 3a3a 6672   vn)| (VarId::fr
+00002080: 6f6d 5f69 6478 2869 292c 2076 6e2e 6173  om_idx(i), vn.as
+00002090: 5f73 7472 2829 2929 0a20 2020 207d 0a20  _str())).    }. 
+000020a0: 2020 2070 7562 2066 6e20 7661 725f 6e61     pub fn var_na
+000020b0: 6d65 2826 7365 6c66 2c20 763a 2056 6172  me(&self, v: Var
+000020c0: 4964 2920 2d3e 2026 7374 7220 7b0a 2020  Id) -> &str {.  
+000020d0: 2020 2020 2020 7365 6c66 2e76 6172 732e        self.vars.
+000020e0: 6765 745f 696e 6465 7828 762e 6964 7828  get_index(v.idx(
+000020f0: 2929 2e75 6e77 7261 7028 292e 302e 6173  )).unwrap().0.as
+00002100: 5f73 7472 2829 0a20 2020 207d 0a20 2020  _str().    }.   
+00002110: 2070 7562 2066 6e20 6661 6374 6f72 5f6e   pub fn factor_n
+00002120: 616d 6573 2826 7365 6c66 2920 2d3e 2069  ames(&self) -> i
+00002130: 6d70 6c20 4974 6572 6174 6f72 3c49 7465  mpl Iterator<Ite
+00002140: 6d20 3d20 2673 7472 3e20 7b0a 2020 2020  m = &str> {.    
+00002150: 2020 2020 7365 6c66 2e66 6163 746f 7273      self.factors
+00002160: 2e6b 6579 7328 292e 6d61 7028 5374 7269  .keys().map(Stri
+00002170: 6e67 3a3a 6173 5f73 7472 290a 2020 2020  ng::as_str).    
+00002180: 7d0a 2020 2020 7075 6220 666e 2066 6163  }.    pub fn fac
+00002190: 746f 725f 6e61 6d65 2826 7365 6c66 2c20  tor_name(&self, 
+000021a0: 663a 2046 6163 746f 7249 6429 202d 3e20  f: FactorId) -> 
+000021b0: 2673 7472 207b 0a20 2020 2020 2020 2073  &str {.        s
+000021c0: 656c 662e 6661 6374 6f72 732e 6765 745f  elf.factors.get_
+000021d0: 696e 6465 7828 662e 6964 7828 2929 2e75  index(f.idx()).u
+000021e0: 6e77 7261 7028 292e 302e 6173 5f73 7472  nwrap().0.as_str
+000021f0: 2829 0a20 2020 207d 0a20 2020 2070 7562  ().    }.    pub
+00002200: 2066 6e20 6661 6374 6f72 5f73 636f 7065   fn factor_scope
+00002210: 3c27 733e 2826 2773 2073 656c 662c 2066  <'s>(&'s self, f
+00002220: 6163 746f 723a 2046 6163 746f 7249 6429  actor: FactorId)
+00002230: 202d 3e20 696d 706c 2049 7465 7261 746f   -> impl Iterato
+00002240: 723c 4974 656d 203d 2056 6172 4964 3e20  r<Item = VarId> 
+00002250: 2b20 2773 207b 0a20 2020 2020 2020 2073  + 's {.        s
+00002260: 656c 662e 6661 6374 6f72 2866 6163 746f  elf.factor(facto
+00002270: 7229 2e65 6467 6573 2e6b 6579 7328 292e  r).edges.keys().
+00002280: 636c 6f6e 6564 2829 0a20 2020 207d 0a20  cloned().    }. 
+00002290: 2020 2070 7562 2066 6e20 7361 6e69 7479     pub fn sanity
+000022a0: 5f63 6865 636b 280a 2020 2020 2020 2020  _check(.        
+000022b0: 2673 656c 662c 0a20 2020 2020 2020 2070  &self,.        p
+000022c0: 7562 6c69 635f 7661 6c75 6573 3a20 5665  ublic_values: Ve
+000022d0: 633c 5075 626c 6963 5661 6c75 653e 2c0a  c<PublicValue>,.
+000022e0: 2020 2020 2020 2020 7661 725f 6173 7369          var_assi
+000022f0: 676e 6d65 6e74 733a 2056 6172 5665 633c  gnments: VarVec<
+00002300: 5075 626c 6963 5661 6c75 653e 2c0a 2020  PublicValue>,.  
+00002310: 2020 2020 2020 6765 6e5f 6661 6374 6f72        gen_factor
+00002320: 733a 2056 6563 3c73 7570 6572 3a3a 4765  s: Vec<super::Ge
+00002330: 6e46 6163 746f 723e 2c0a 2020 2020 2920  nFactor>,.    ) 
+00002340: 2d3e 2046 4752 6573 756c 743c 2829 3e20  -> FGResult<()> 
+00002350: 7b0a 2020 2020 2020 2020 6173 7365 7274  {.        assert
+00002360: 5f65 7121 2870 7562 6c69 635f 7661 6c75  _eq!(public_valu
+00002370: 6573 2e6c 656e 2829 2c20 7365 6c66 2e70  es.len(), self.p
+00002380: 7562 6c69 6373 2e6c 656e 2829 293b 0a20  ublics.len());. 
+00002390: 2020 2020 2020 2061 7373 6572 745f 6571         assert_eq
+000023a0: 2128 7661 725f 6173 7369 676e 6d65 6e74  !(var_assignment
+000023b0: 732e 6c65 6e28 292c 2073 656c 662e 7661  s.len(), self.va
+000023c0: 7273 2e6c 656e 2829 293b 0a20 2020 2020  rs.len());.     
+000023d0: 2020 206c 6574 2072 6564 7563 6564 5f70     let reduced_p
+000023e0: 7562 203d 2073 656c 662e 7265 6475 6365  ub = self.reduce
+000023f0: 5f70 7562 2870 7562 6c69 635f 7661 6c75  _pub(public_valu
+00002400: 6573 2e61 735f 736c 6963 6528 2929 3b0a  es.as_slice());.
+00002410: 2020 2020 2020 2020 666f 7220 2828 6661          for ((fa
+00002420: 6374 6f72 5f6e 616d 652c 2066 6163 746f  ctor_name, facto
+00002430: 7229 2c20 6373 7429 2069 6e20 7365 6c66  r), cst) in self
+00002440: 2e66 6163 746f 7273 2e69 7465 7228 292e  .factors.iter().
+00002450: 7a69 7028 7265 6475 6365 645f 7075 6229  zip(reduced_pub)
+00002460: 207b 0a20 2020 2020 2020 2020 2020 206d   {.            m
+00002470: 6174 6368 2026 6661 6374 6f72 2e6b 696e  atch &factor.kin
+00002480: 6420 7b0a 2020 2020 2020 2020 2020 2020  d {.            
+00002490: 2020 2020 4661 6374 6f72 4b69 6e64 3a3a      FactorKind::
+000024a0: 4173 7369 676e 207b 2065 7870 722c 2068  Assign { expr, h
+000024b0: 6173 5f72 6573 207d 203d 3e20 7b0a 2020  as_res } => {.  
+000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024d0: 2020 6c65 7420 6578 7065 6374 6564 5f72    let expected_r
+000024e0: 6573 203d 2066 6163 746f 720a 2020 2020  es = factor.    
+000024f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002500: 2020 2020 2e72 6573 5f69 6428 290a 2020      .res_id().  
+00002510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002520: 2020 2020 2020 2e6d 6170 287c 765f 6964        .map(|v_id
+00002530: 7c20 2676 6172 5f61 7373 6967 6e6d 656e  | &var_assignmen
+00002540: 7473 5b76 5f69 645d 290a 2020 2020 2020  ts[v_id]).      
+00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002560: 2020 2e75 6e77 7261 705f 6f72 2826 6373    .unwrap_or(&cs
+00002570: 7429 3b0a 2020 2020 2020 2020 2020 2020  t);.            
+00002580: 2020 2020 2020 2020 6c65 7420 736b 6970          let skip
+00002590: 5f72 6573 203d 2069 6620 2a68 6173 5f72  _res = if *has_r
+000025a0: 6573 207b 2031 207d 2065 6c73 6520 7b20  es { 1 } else { 
+000025b0: 3020 7d3b 0a20 2020 2020 2020 2020 2020  0 };.           
+000025c0: 2020 2020 2020 2020 206c 6574 206d 7574           let mut
+000025d0: 206f 7073 203d 2066 6163 746f 720a 2020   ops = factor.  
+000025e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025f0: 2020 2020 2020 2e65 6467 6573 0a20 2020        .edges.   
+00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002610: 2020 2020 202e 6b65 7973 2829 0a20 2020       .keys().   
+00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002630: 2020 2020 202e 736b 6970 2873 6b69 705f       .skip(skip_
+00002640: 7265 7329 0a20 2020 2020 2020 2020 2020  res).           
+00002650: 2020 2020 2020 2020 2020 2020 202e 6d61               .ma
+00002660: 7028 7c76 5f69 647c 2026 7661 725f 6173  p(|v_id| &var_as
+00002670: 7369 676e 6d65 6e74 735b 2a76 5f69 645d  signments[*v_id]
+00002680: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
+00002690: 2020 2020 2020 206c 6574 2072 6573 203d         let res =
+000026a0: 206d 6174 6368 2065 7870 7220 7b0a 2020   match expr {.  
 000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026c0: 2020 2020 2020 2020 2020 2020 6c65 7420              let 
-000026d0: 7820 3d20 7365 6c66 2e6d 6572 6765 5f70  x = self.merge_p
-000026e0: 7562 7328 0a20 2020 2020 2020 2020 2020  ubs(.           
+000026c0: 2020 2020 2020 4578 7072 4661 6374 6f72        ExprFactor
+000026d0: 3a3a 414e 4420 7b20 7661 7273 5f6e 6567  ::AND { vars_neg
+000026e0: 207d 203d 3e20 7b0a 2020 2020 2020 2020   } => {.        
 000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002700: 2020 2020 2065 7870 722c 0a20 2020 2020       expr,.     
-00002710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002720: 2020 2020 2020 2020 2020 206f 7073 2e7a             ops.z
-00002730: 6970 2876 6172 735f 6e65 672e 6974 6572  ip(vars_neg.iter
-00002740: 2829 2e63 6c6f 6e65 6428 2929 0a20 2020  ().cloned()).   
+00002700: 2020 2020 6c65 7420 7820 3d20 7365 6c66      let x = self
+00002710: 2e6d 6572 6765 5f70 7562 7328 0a20 2020  .merge_pubs(.   
+00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002730: 2020 2020 2020 2020 2020 2020 2065 7870               exp
+00002740: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
 00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002770: 202e 6368 6169 6e28 7374 643a 3a69 7465   .chain(std::ite
-00002780: 723a 3a6f 6e63 6528 2826 6373 742c 2066  r::once((&cst, f
-00002790: 616c 7365 2929 292c 0a20 2020 2020 2020  alse))),.       
-000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027b0: 2020 2020 2029 3b0a 2020 2020 2020 2020       );.        
-000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027d0: 2020 2020 2f2f 2069 6e76 6572 7420 6966      // invert if
-000027e0: 2077 6520 6172 6520 646f 696e 6720 616e   we are doing an
-000027f0: 204f 520a 2020 2020 2020 2020 2020 2020   OR.            
-00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002810: 6d61 7463 6820 7820 7b0a 2020 2020 2020  match x {.      
-00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002830: 2020 2020 2020 2020 2020 5075 626c 6963            Public
-00002840: 5661 6c75 653a 3a53 696e 676c 6528 6376  Value::Single(cv
-00002850: 2920 6966 2076 6172 735f 6e65 675b 305d  ) if vars_neg[0]
-00002860: 203d 3e20 7b0a 2020 2020 2020 2020 2020   => {.          
-00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002880: 2020 2020 2020 2020 2020 5075 626c 6963            Public
-00002890: 5661 6c75 653a 3a53 696e 676c 6528 7365  Value::Single(se
-000028a0: 6c66 2e6e 6f74 2863 7629 290a 2020 2020  lf.not(cv)).    
+00002760: 2020 206f 7073 2e7a 6970 2876 6172 735f     ops.zip(vars_
+00002770: 6e65 672e 6974 6572 2829 2e63 6c6f 6e65  neg.iter().clone
+00002780: 6428 2929 0a20 2020 2020 2020 2020 2020  d()).           
+00002790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027a0: 2020 2020 2020 2020 202e 6368 6169 6e28           .chain(
+000027b0: 7374 643a 3a69 7465 723a 3a6f 6e63 6528  std::iter::once(
+000027c0: 2826 6373 742c 2066 616c 7365 2929 292c  (&cst, false))),
+000027d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000027e0: 2020 2020 2020 2020 2020 2020 2029 3b0a               );.
+000027f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002800: 2020 2020 2020 2020 2020 2020 2f2f 2069              // i
+00002810: 6e76 6572 7420 6966 2077 6520 6172 6520  nvert if we are 
+00002820: 646f 696e 6720 616e 204f 520a 2020 2020  doing an OR.    
+00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002840: 2020 2020 2020 2020 6d61 7463 6820 7820          match x 
+00002850: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002870: 2020 5075 626c 6963 5661 6c75 653a 3a53    PublicValue::S
+00002880: 696e 676c 6528 6376 2920 6966 2076 6172  ingle(cv) if var
+00002890: 735f 6e65 675b 305d 203d 3e20 7b0a 2020  s_neg[0] => {.  
+000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028c0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-000028d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028e0: 2020 2020 2020 2020 2020 2020 2020 5075                Pu
-000028f0: 626c 6963 5661 6c75 653a 3a4d 756c 7469  blicValue::Multi
-00002900: 2863 7629 2069 6620 7661 7273 5f6e 6567  (cv) if vars_neg
-00002910: 5b30 5d20 3d3e 207b 0a20 2020 2020 2020  [0] => {.       
-00002920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002930: 2020 2020 2020 2020 2020 2020 2050 7562               Pub
-00002940: 6c69 6356 616c 7565 3a3a 4d75 6c74 6928  licValue::Multi(
-00002950: 6376 2e69 7465 7228 292e 6d61 7028 7c76  cv.iter().map(|v
-00002960: 7c20 7365 6c66 2e6e 6f74 282a 7629 292e  | self.not(*v)).
-00002970: 636f 6c6c 6563 7428 2929 0a20 2020 2020  collect()).     
-00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002990: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-000029a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029b0: 2020 2020 2020 2020 2020 2020 205f 203d               _ =
-000029c0: 3e20 782c 0a20 2020 2020 2020 2020 2020  > x,.           
-000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029e0: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
-000029f0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+000028c0: 2020 5075 626c 6963 5661 6c75 653a 3a53    PublicValue::S
+000028d0: 696e 676c 6528 7365 6c66 2e6e 6f74 2863  ingle(self.not(c
+000028e0: 7629 290a 2020 2020 2020 2020 2020 2020  v)).            
+000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002900: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00002910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002920: 2020 2020 2020 5075 626c 6963 5661 6c75        PublicValu
+00002930: 653a 3a4d 756c 7469 2863 7629 2069 6620  e::Multi(cv) if 
+00002940: 7661 7273 5f6e 6567 5b30 5d20 3d3e 207b  vars_neg[0] => {
+00002950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002970: 2020 2020 2050 7562 6c69 6356 616c 7565       PublicValue
+00002980: 3a3a 4d75 6c74 6928 6376 2e69 7465 7228  ::Multi(cv.iter(
+00002990: 292e 6d61 7028 7c76 7c20 7365 6c66 2e6e  ).map(|v| self.n
+000029a0: 6f74 282a 7629 292e 636f 6c6c 6563 7428  ot(*v)).collect(
+000029b0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029d0: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029f0: 2020 2020 205f 203d 3e20 782c 0a20 2020       _ => x,.   
 00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a10: 2020 2020 2045 7870 7246 6163 746f 723a       ExprFactor:
-00002a20: 3a58 4f52 207c 2045 7870 7246 6163 746f  :XOR | ExprFacto
-00002a30: 723a 3a41 4444 207c 2045 7870 7246 6163  r::ADD | ExprFac
-00002a40: 746f 723a 3a4d 554c 203d 3e20 7365 6c66  tor::MUL => self
-00002a50: 2e6d 6572 6765 5f70 7562 7328 0a20 2020  .merge_pubs(.   
-00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a70: 2020 2020 2020 2020 2065 7870 722c 0a20           expr,. 
-00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a90: 2020 2020 2020 2020 2020 206f 7073 2e7a             ops.z
-00002aa0: 6970 2873 7464 3a3a 6974 6572 3a3a 7265  ip(std::iter::re
-00002ab0: 7065 6174 2866 616c 7365 2929 0a20 2020  peat(false)).   
+00002a10: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a30: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+00002a40: 2020 2020 2020 2020 2020 2020 2045 7870               Exp
+00002a50: 7246 6163 746f 723a 3a58 4f52 207c 2045  rFactor::XOR | E
+00002a60: 7870 7246 6163 746f 723a 3a41 4444 207b  xprFactor::ADD {
+00002a70: 202e 2e20 7d20 7c20 4578 7072 4661 6374   .. } | ExprFact
+00002a80: 6f72 3a3a 4d55 4c20 3d3e 2073 656c 660a  or::MUL => self.
+00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002aa0: 2020 2020 2020 2020 2020 2020 2e6d 6572              .mer
+00002ab0: 6765 5f70 7562 7328 0a20 2020 2020 2020  ge_pubs(.       
 00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ad0: 2020 2020 2020 2020 2020 2020 202e 6368               .ch
-00002ae0: 6169 6e28 7374 643a 3a69 7465 723a 3a6f  ain(std::iter::o
-00002af0: 6e63 6528 2826 6373 742c 2066 616c 7365  nce((&cst, false
-00002b00: 2929 292c 0a20 2020 2020 2020 2020 2020  ))),.           
-00002b10: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
-00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b30: 2020 2020 2020 2020 4578 7072 4661 6374          ExprFact
-00002b40: 6f72 3a3a 4e4f 5420 3d3e 206f 7073 2e6e  or::NOT => ops.n
-00002b50: 6578 7428 292e 756e 7772 6170 2829 2e6d  ext().unwrap().m
-00002b60: 6170 287c 787c 2073 656c 662e 6e6f 7428  ap(|x| self.not(
-00002b70: 7829 292c 0a20 2020 2020 2020 2020 2020  x)),.           
-00002b80: 2020 2020 2020 2020 2020 2020 2045 7870               Exp
-00002b90: 7246 6163 746f 723a 3a4c 4f4f 4b55 5020  rFactor::LOOKUP 
-00002ba0: 7b20 7461 626c 6520 7d20 3d3e 206f 7073  { table } => ops
-00002bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002bc0: 2020 2020 2020 2020 2020 2020 202e 6e65               .ne
-00002bd0: 7874 2829 0a20 2020 2020 2020 2020 2020  xt().           
-00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bf0: 202e 756e 7772 6170 2829 0a20 2020 2020   .unwrap().     
-00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c10: 2020 2020 2020 202e 6d61 7028 7c78 7c20         .map(|x| 
-00002c20: 7365 6c66 2e74 6162 6c65 735b 2a74 6162  self.tables[*tab
-00002c30: 6c65 5d2e 7661 6c75 6573 5b78 2061 7320  le].values[x as 
-00002c40: 7573 697a 655d 292c 0a20 2020 2020 2020  usize]),.       
-00002c50: 2020 2020 2020 2020 2020 2020 207d 3b0a               };.
-00002c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c70: 2020 2020 6c65 7420 6368 6563 6b20 3d20      let check = 
-00002c80: 6d61 7463 6820 2826 7265 732c 2065 7870  match (&res, exp
-00002c90: 6563 7465 645f 7265 7329 207b 0a20 2020  ected_res) {.   
-00002ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cb0: 2020 2020 2028 5075 626c 6963 5661 6c75       (PublicValu
-00002cc0: 653a 3a53 696e 676c 6528 7631 292c 2050  e::Single(v1), P
-00002cd0: 7562 6c69 6356 616c 7565 3a3a 4d75 6c74  ublicValue::Mult
-00002ce0: 6928 7632 2929 203d 3e20 7b0a 2020 2020  i(v2)) => {.    
-00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d00: 2020 2020 2020 2020 7632 2e69 7465 7228          v2.iter(
-00002d10: 292e 616e 7928 7c78 7c20 7820 213d 2076  ).any(|x| x != v
-00002d20: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
-00002d30: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00002d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d50: 2020 2020 2028 5075 626c 6963 5661 6c75       (PublicValu
-00002d60: 653a 3a4d 756c 7469 2876 3129 2c20 5075  e::Multi(v1), Pu
-00002d70: 626c 6963 5661 6c75 653a 3a53 696e 676c  blicValue::Singl
-00002d80: 6528 7632 2929 203d 3e20 7b0a 2020 2020  e(v2)) => {.    
+00002ad0: 2020 2020 2020 2020 2065 7870 722c 0a20           expr,. 
+00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002af0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00002b00: 7073 2e7a 6970 2873 7464 3a3a 6974 6572  ps.zip(std::iter
+00002b10: 3a3a 7265 7065 6174 2866 616c 7365 2929  ::repeat(false))
+00002b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b40: 2020 2020 202e 6368 6169 6e28 7374 643a       .chain(std:
+00002b50: 3a69 7465 723a 3a6f 6e63 6528 2826 6373  :iter::once((&cs
+00002b60: 742c 2066 616c 7365 2929 292c 0a20 2020  t, false))),.   
+00002b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b80: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ba0: 2020 2020 4578 7072 4661 6374 6f72 3a3a      ExprFactor::
+00002bb0: 4e4f 5420 3d3e 206f 7073 2e6e 6578 7428  NOT => ops.next(
+00002bc0: 292e 756e 7772 6170 2829 2e6d 6170 287c  ).unwrap().map(|
+00002bd0: 787c 2073 656c 662e 6e6f 7428 7829 292c  x| self.not(x)),
+00002be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002bf0: 2020 2020 2020 2020 2045 7870 7246 6163           ExprFac
+00002c00: 746f 723a 3a4c 4f4f 4b55 5020 7b20 7461  tor::LOOKUP { ta
+00002c10: 626c 6520 7d20 3d3e 206f 7073 0a20 2020  ble } => ops.   
+00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c30: 2020 2020 2020 2020 202e 6e65 7874 2829           .next()
+00002c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002c50: 2020 2020 2020 2020 2020 2020 202e 756e               .un
+00002c60: 7772 6170 2829 0a20 2020 2020 2020 2020  wrap().         
+00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c80: 2020 202e 6d61 7028 7c78 7c20 7365 6c66     .map(|x| self
+00002c90: 2e74 6162 6c65 735b 2a74 6162 6c65 5d2e  .tables[*table].
+00002ca0: 7661 6c75 6573 5b78 2061 7320 7573 697a  values[x as usiz
+00002cb0: 655d 292c 0a20 2020 2020 2020 2020 2020  e]),.           
+00002cc0: 2020 2020 2020 2020 207d 3b0a 2020 2020           };.    
+00002cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ce0: 6c65 7420 6368 6563 6b20 3d20 6d61 7463  let check = matc
+00002cf0: 6820 2826 7265 732c 2065 7870 6563 7465  h (&res, expecte
+00002d00: 645f 7265 7329 207b 0a20 2020 2020 2020  d_res) {.       
+00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d20: 2028 5075 626c 6963 5661 6c75 653a 3a53   (PublicValue::S
+00002d30: 696e 676c 6528 7631 292c 2050 7562 6c69  ingle(v1), Publi
+00002d40: 6356 616c 7565 3a3a 4d75 6c74 6928 7632  cValue::Multi(v2
+00002d50: 2929 203d 3e20 7b0a 2020 2020 2020 2020  )) => {.        
+00002d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d70: 2020 2020 7632 2e69 7465 7228 292e 616e      v2.iter().an
+00002d80: 7928 7c78 7c20 7820 213d 2076 3129 0a20  y(|x| x != v1). 
 00002d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002da0: 2020 2020 2020 2020 7631 2e69 7465 7228          v1.iter(
-00002db0: 292e 616e 7928 7c78 7c20 7820 213d 2076  ).any(|x| x != v
-00002dc0: 3229 0a20 2020 2020 2020 2020 2020 2020  2).             
-00002dd0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00002de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002df0: 2020 2020 2028 5f2c 205f 2920 3d3e 2026       (_, _) => &
-00002e00: 7265 7320 213d 2065 7870 6563 7465 645f  res != expected_
-00002e10: 7265 732c 0a20 2020 2020 2020 2020 2020  res,.           
-00002e20: 2020 2020 2020 2020 207d 3b0a 2020 2020           };.    
+00002da0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002dc0: 2028 5075 626c 6963 5661 6c75 653a 3a4d   (PublicValue::M
+00002dd0: 756c 7469 2876 3129 2c20 5075 626c 6963  ulti(v1), Public
+00002de0: 5661 6c75 653a 3a53 696e 676c 6528 7632  Value::Single(v2
+00002df0: 2929 203d 3e20 7b0a 2020 2020 2020 2020  )) => {.        
+00002e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e10: 2020 2020 7631 2e69 7465 7228 292e 616e      v1.iter().an
+00002e20: 7928 7c78 7c20 7820 213d 2076 3229 0a20  y(|x| x != v2). 
 00002e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e40: 6966 2063 6865 636b 207b 0a20 2020 2020  if check {.     
+00002e40: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
 00002e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e60: 2020 2072 6574 7572 6e20 4572 7228 4647     return Err(FG
-00002e70: 4572 726f 723a 3a43 6865 636b 4661 696c  Error::CheckFail
-00002e80: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00002e90: 2020 2020 2020 2020 2020 2020 2020 6661                fa
-00002ea0: 6374 6f72 5f6e 616d 652e 636c 6f6e 6528  ctor_name.clone(
-00002eb0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00002ec0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00002ed0: 7870 6563 7465 645f 7265 732e 636c 6f6e  xpected_res.clon
-00002ee0: 6528 292c 0a20 2020 2020 2020 2020 2020  e(),.           
+00002e60: 2028 5f2c 205f 2920 3d3e 2026 7265 7320   (_, _) => &res 
+00002e70: 213d 2065 7870 6563 7465 645f 7265 732c  != expected_res,
+00002e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002e90: 2020 2020 207d 3b0a 2020 2020 2020 2020       };.        
+00002ea0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00002eb0: 6865 636b 207b 0a20 2020 2020 2020 2020  heck {.         
+00002ec0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00002ed0: 6574 7572 6e20 4572 7228 4647 4572 726f  eturn Err(FGErro
+00002ee0: 723a 3a43 6865 636b 4661 696c 280a 2020  r::CheckFail(.  
 00002ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f00: 2072 6573 2c0a 2020 2020 2020 2020 2020   res,.          
-00002f10: 2020 2020 2020 2020 2020 2020 2020 2929                ))
-00002f20: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-00002f30: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00002f40: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00002f50: 2020 2020 2020 2020 2020 4661 6374 6f72            Factor
-00002f60: 4b69 6e64 3a3a 4765 6e46 6163 746f 7220  Kind::GenFactor 
-00002f70: 7b20 6964 2c20 6f70 6572 616e 6473 207d  { id, operands }
-00002f80: 203d 3e20 7b0a 2020 2020 2020 2020 2020   => {.          
-00002f90: 2020 2020 2020 2020 2020 6c65 7420 6f70            let op
-00002fa0: 733a 2056 6563 3c26 5075 626c 6963 5661  s: Vec<&PublicVa
-00002fb0: 6c75 653e 203d 206f 7065 7261 6e64 730a  lue> = operands.
-00002fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fd0: 2020 2020 2020 2020 2e69 7465 7228 290a          .iter().
-00002fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ff0: 2020 2020 2020 2020 2e6d 6170 287c 6f70          .map(|op
-00003000: 7c20 6d61 7463 6820 6f70 207b 0a20 2020  | match op {.   
-00003010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003020: 2020 2020 2020 2020 2047 656e 4661 6374           GenFact
-00003030: 6f72 4f70 6572 616e 643a 3a56 6172 2869  orOperand::Var(i
-00003040: 6478 2c20 2e2e 2920 3d3e 2026 7661 725f  dx, ..) => &var_
-00003050: 6173 7369 676e 6d65 6e74 735b 2a69 6478  assignments[*idx
-00003060: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00003070: 2020 2020 2020 2020 2020 2020 2020 2047                 G
-00003080: 656e 4661 6374 6f72 4f70 6572 616e 643a  enFactorOperand:
-00003090: 3a50 7562 2869 6478 2920 3d3e 2026 7075  :Pub(idx) => &pu
-000030a0: 626c 6963 5f76 616c 7565 735b 2a69 6478  blic_values[*idx
-000030b0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-000030c0: 2020 2020 2020 2020 2020 207d 290a 2020             }).  
+00002f00: 2020 2020 2020 2020 2020 6661 6374 6f72            factor
+00002f10: 5f6e 616d 652e 636c 6f6e 6528 292c 0a20  _name.clone(),. 
+00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f30: 2020 2020 2020 2020 2020 2065 7870 6563             expec
+00002f40: 7465 645f 7265 732e 636c 6f6e 6528 292c  ted_res.clone(),
+00002f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002f60: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00002f70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002f80: 2020 2020 2020 2020 2020 2929 3b0a 2020            ));.  
+00002f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fa0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00002fb0: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00002fc0: 2020 2020 2020 4661 6374 6f72 4b69 6e64        FactorKind
+00002fd0: 3a3a 4765 6e46 6163 746f 7220 7b20 6964  ::GenFactor { id
+00002fe0: 2c20 6f70 6572 616e 6473 207d 203d 3e20  , operands } => 
+00002ff0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00003000: 2020 2020 2020 6c65 7420 6f70 733a 2056        let ops: V
+00003010: 6563 3c26 5075 626c 6963 5661 6c75 653e  ec<&PublicValue>
+00003020: 203d 206f 7065 7261 6e64 730a 2020 2020   = operands.    
+00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003040: 2020 2020 2e69 7465 7228 290a 2020 2020      .iter().    
+00003050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003060: 2020 2020 2e6d 6170 287c 6f70 7c20 6d61      .map(|op| ma
+00003070: 7463 6820 6f70 207b 0a20 2020 2020 2020  tch op {.       
+00003080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003090: 2020 2020 2047 656e 4661 6374 6f72 4f70       GenFactorOp
+000030a0: 6572 616e 643a 3a56 6172 2869 6478 2c20  erand::Var(idx, 
+000030b0: 2e2e 2920 3d3e 2026 7661 725f 6173 7369  ..) => &var_assi
+000030c0: 676e 6d65 6e74 735b 2a69 6478 5d2c 0a20  gnments[*idx],. 
 000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030e0: 2020 2020 2020 2e63 6f6c 6c65 6374 2829        .collect()
-000030f0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-00003100: 2020 2020 2020 6c65 7420 6e6d 756c 7469        let nmulti
-00003110: 5f6f 7073 203d 206f 7073 2e69 7465 7228  _ops = ops.iter(
-00003120: 292e 6669 6e64 5f6d 6170 287c 6f70 7c20  ).find_map(|op| 
-00003130: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00003140: 2020 2020 2020 2020 2020 6966 206c 6574            if let
-00003150: 2050 7562 6c69 6356 616c 7565 3a3a 4d75   PublicValue::Mu
-00003160: 6c74 6928 7829 203d 206f 7020 7b0a 2020  lti(x) = op {.  
-00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003180: 2020 2020 2020 2020 2020 536f 6d65 2878            Some(x
-00003190: 2e6c 656e 2829 290a 2020 2020 2020 2020  .len()).        
+000030e0: 2020 2020 2020 2020 2020 2047 656e 4661             GenFa
+000030f0: 6374 6f72 4f70 6572 616e 643a 3a50 7562  ctorOperand::Pub
+00003100: 2869 6478 2920 3d3e 2026 7075 626c 6963  (idx) => &public
+00003110: 5f76 616c 7565 735b 2a69 6478 5d2c 0a20  _values[*idx],. 
+00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003130: 2020 2020 2020 207d 290a 2020 2020 2020         }).      
+00003140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003150: 2020 2e63 6f6c 6c65 6374 2829 3b0a 2020    .collect();.  
+00003160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003170: 2020 6c65 7420 6e6d 756c 7469 5f6f 7073    let nmulti_ops
+00003180: 203d 206f 7073 2e69 7465 7228 292e 6669   = ops.iter().fi
+00003190: 6e64 5f6d 6170 287c 6f70 7c20 7b0a 2020  nd_map(|op| {.  
 000031a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031b0: 7d20 656c 7365 207b 0a20 2020 2020 2020  } else {.       
-000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031d0: 2020 2020 204e 6f6e 650a 2020 2020 2020       None.      
+000031b0: 2020 2020 2020 6966 206c 6574 2050 7562        if let Pub
+000031c0: 6c69 6356 616c 7565 3a3a 4d75 6c74 6928  licValue::Multi(
+000031d0: 7829 203d 206f 7020 7b0a 2020 2020 2020  x) = op {.      
 000031e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031f0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00003200: 2020 2020 2020 2020 7d29 3b0a 2020 2020          });.    
-00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003220: 6c65 7420 6e6d 756c 7469 5f66 6163 746f  let nmulti_facto
-00003230: 7220 3d20 6966 206c 6574 2073 7570 6572  r = if let super
-00003240: 3a3a 4765 6e46 6163 746f 723a 3a4d 756c  ::GenFactor::Mul
-00003250: 7469 2867 6676 2920 3d20 2667 656e 5f66  ti(gfv) = &gen_f
-00003260: 6163 746f 7273 5b2a 6964 5d20 7b0a 2020  actors[*id] {.  
-00003270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003280: 2020 2020 2020 536f 6d65 2867 6676 2e6c        Some(gfv.l
-00003290: 656e 2829 290a 2020 2020 2020 2020 2020  en()).          
-000032a0: 2020 2020 2020 2020 2020 7d20 656c 7365            } else
-000032b0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-000032c0: 2020 2020 2020 2020 2020 204e 6f6e 650a             None.
-000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032e0: 2020 2020 7d3b 0a20 2020 2020 2020 2020      };.         
-000032f0: 2020 2020 2020 2020 2020 206c 6574 206e             let n
-00003300: 6d75 6c74 6920 3d20 6d61 7463 6820 286e  multi = match (n
-00003310: 6d75 6c74 695f 6f70 732c 206e 6d75 6c74  multi_ops, nmult
-00003320: 695f 6661 6374 6f72 2920 7b0a 2020 2020  i_factor) {.    
-00003330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003340: 2020 2020 2853 6f6d 6528 6e6d 5f6f 7073      (Some(nm_ops
-00003350: 292c 2053 6f6d 6528 6e6d 5f66 6163 746f  ), Some(nm_facto
-00003360: 7273 2929 2069 6620 6e6d 5f6f 7073 203d  rs)) if nm_ops =
-00003370: 3d20 6e6d 5f66 6163 746f 7273 203d 3e20  = nm_factors => 
-00003380: 6e6d 5f66 6163 746f 7273 2c0a 2020 2020  nm_factors,.    
-00003390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033a0: 2020 2020 2853 6f6d 6528 6e6d 5f6f 7073      (Some(nm_ops
-000033b0: 292c 2053 6f6d 6528 6e6d 5f66 6163 746f  ), Some(nm_facto
-000033c0: 7273 2929 203d 3e20 7b0a 2020 2020 2020  rs)) => {.      
-000033d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033e0: 2020 2020 2020 7265 7475 726e 2045 7272        return Err
-000033f0: 2846 4745 7272 6f72 3a3a 496e 7661 6c69  (FGError::Invali
-00003400: 6447 656e 6572 6963 4661 6374 6f72 4173  dGenericFactorAs
-00003410: 7369 676e 6d65 6e74 2866 6f72 6d61 7421  signment(format!
-00003420: 2822 4d69 736d 6174 6368 2062 6574 7765  ("Mismatch betwe
-00003430: 656e 206d 756c 7469 2064 6563 6c61 7261  en multi declara
-00003440: 7469 6f6e 206f 6620 4765 6e46 6163 746f  tion of GenFacto
-00003450: 7220 6f70 6572 616e 6473 207b 7d20 616e  r operands {} an
-00003460: 6420 4765 6e46 6163 746f 7220 7b7d 222c  d GenFactor {}",
-00003470: 206e 6d5f 6f70 732c 206e 6d5f 6661 6374   nm_ops, nm_fact
-00003480: 6f72 7329 2929 0a20 2020 2020 2020 2020  ors))).         
-00003490: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-000034a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000034b0: 2020 2020 2020 2020 2028 536f 6d65 286e           (Some(n
-000034c0: 6d75 6c74 6929 2c20 4e6f 6e65 2920 7c20  multi), None) | 
-000034d0: 284e 6f6e 652c 2053 6f6d 6528 6e6d 756c  (None, Some(nmul
-000034e0: 7469 2929 203d 3e20 6e6d 756c 7469 2c0a  ti)) => nmulti,.
-000034f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003500: 2020 2020 2020 2020 284e 6f6e 652c 204e          (None, N
-00003510: 6f6e 6529 203d 3e20 312c 0a20 2020 2020  one) => 1,.     
-00003520: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00003530: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-00003540: 2020 2020 2020 666f 7220 6920 696e 2030        for i in 0
-00003550: 2e2e 6e6d 756c 7469 207b 0a20 2020 2020  ..nmulti {.     
+000031f0: 2020 2020 2020 536f 6d65 2878 2e6c 656e        Some(x.len
+00003200: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
+00003210: 2020 2020 2020 2020 2020 2020 7d20 656c              } el
+00003220: 7365 207b 0a20 2020 2020 2020 2020 2020  se {.           
+00003230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003240: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00003250: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00003260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003270: 2020 2020 7d29 3b0a 2020 2020 2020 2020      });.        
+00003280: 2020 2020 2020 2020 2020 2020 6c65 7420              let 
+00003290: 6e6d 756c 7469 5f66 6163 746f 7220 3d20  nmulti_factor = 
+000032a0: 6966 206c 6574 2073 7570 6572 3a3a 4765  if let super::Ge
+000032b0: 6e46 6163 746f 723a 3a4d 756c 7469 2867  nFactor::Multi(g
+000032c0: 6676 2920 3d20 2667 656e 5f66 6163 746f  fv) = &gen_facto
+000032d0: 7273 5b2a 6964 5d20 7b0a 2020 2020 2020  rs[*id] {.      
+000032e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032f0: 2020 536f 6d65 2867 6676 2e6c 656e 2829    Some(gfv.len()
+00003300: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003310: 2020 2020 2020 7d20 656c 7365 207b 0a20        } else {. 
+00003320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003330: 2020 2020 2020 204e 6f6e 650a 2020 2020         None.    
+00003340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003350: 7d3b 0a20 2020 2020 2020 2020 2020 2020  };.             
+00003360: 2020 2020 2020 206c 6574 206e 6d75 6c74         let nmult
+00003370: 6920 3d20 6d61 7463 6820 286e 6d75 6c74  i = match (nmult
+00003380: 695f 6f70 732c 206e 6d75 6c74 695f 6661  i_ops, nmulti_fa
+00003390: 6374 6f72 2920 7b0a 2020 2020 2020 2020  ctor) {.        
+000033a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033b0: 2853 6f6d 6528 6e6d 5f6f 7073 292c 2053  (Some(nm_ops), S
+000033c0: 6f6d 6528 6e6d 5f66 6163 746f 7273 2929  ome(nm_factors))
+000033d0: 2069 6620 6e6d 5f6f 7073 203d 3d20 6e6d   if nm_ops == nm
+000033e0: 5f66 6163 746f 7273 203d 3e20 6e6d 5f66  _factors => nm_f
+000033f0: 6163 746f 7273 2c0a 2020 2020 2020 2020  actors,.        
+00003400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003410: 2853 6f6d 6528 6e6d 5f6f 7073 292c 2053  (Some(nm_ops), S
+00003420: 6f6d 6528 6e6d 5f66 6163 746f 7273 2929  ome(nm_factors))
+00003430: 203d 3e20 7b0a 2020 2020 2020 2020 2020   => {.          
+00003440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003450: 2020 7265 7475 726e 2045 7272 2846 4745    return Err(FGE
+00003460: 7272 6f72 3a3a 496e 7661 6c69 6447 656e  rror::InvalidGen
+00003470: 6572 6963 4661 6374 6f72 4173 7369 676e  ericFactorAssign
+00003480: 6d65 6e74 2866 6f72 6d61 7421 2822 4d69  ment(format!("Mi
+00003490: 736d 6174 6368 2062 6574 7765 656e 206d  smatch between m
+000034a0: 756c 7469 2064 6563 6c61 7261 7469 6f6e  ulti declaration
+000034b0: 206f 6620 4765 6e46 6163 746f 7220 6f70   of GenFactor op
+000034c0: 6572 616e 6473 207b 7d20 616e 6420 4765  erands {} and Ge
+000034d0: 6e46 6163 746f 7220 7b7d 222c 206e 6d5f  nFactor {}", nm_
+000034e0: 6f70 732c 206e 6d5f 6661 6374 6f72 7329  ops, nm_factors)
+000034f0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00003500: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003520: 2020 2020 2028 536f 6d65 286e 6d75 6c74       (Some(nmult
+00003530: 6929 2c20 4e6f 6e65 2920 7c20 284e 6f6e  i), None) | (Non
+00003540: 652c 2053 6f6d 6528 6e6d 756c 7469 2929  e, Some(nmulti))
+00003550: 203d 3e20 6e6d 756c 7469 2c0a 2020 2020   => nmulti,.    
 00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003570: 2020 206c 6574 2067 6620 3d20 6d61 7463     let gf = matc
-00003580: 6820 2667 656e 5f66 6163 746f 7273 5b2a  h &gen_factors[*
-00003590: 6964 5d20 7b0a 2020 2020 2020 2020 2020  id] {.          
+00003570: 2020 2020 284e 6f6e 652c 204e 6f6e 6529      (None, None)
+00003580: 203d 3e20 312c 0a20 2020 2020 2020 2020   => 1,.         
+00003590: 2020 2020 2020 2020 2020 207d 3b0a 2020             };.  
 000035a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035b0: 2020 7375 7065 723a 3a47 656e 4661 6374    super::GenFact
-000035c0: 6f72 3a3a 5369 6e67 6c65 2867 6673 2920  or::Single(gfs) 
-000035d0: 3d3e 2067 6673 2c0a 2020 2020 2020 2020  => gfs,.        
-000035e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035f0: 2020 2020 7375 7065 723a 3a47 656e 4661      super::GenFa
-00003600: 6374 6f72 3a3a 4d75 6c74 6928 6766 7629  ctor::Multi(gfv)
-00003610: 203d 3e20 2667 6676 5b69 5d2c 0a20 2020   => &gfv[i],.   
-00003620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003630: 2020 2020 207d 3b0a 2020 2020 2020 2020       };.        
-00003640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003650: 6c65 7420 696e 6469 6365 733a 2056 6563  let indices: Vec
-00003660: 3c43 6c61 7373 5661 6c3e 203d 206f 7073  <ClassVal> = ops
-00003670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003680: 2020 2020 2020 2020 2020 2020 202e 6974               .it
-00003690: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
-000036a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036b0: 202e 6d61 7028 7c70 767c 206d 6174 6368   .map(|pv| match
-000036c0: 202a 7076 207b 0a20 2020 2020 2020 2020   *pv {.         
-000036d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036e0: 2020 2020 2020 2050 7562 6c69 6356 616c         PublicVal
-000036f0: 7565 3a3a 5369 6e67 6c65 2878 2920 3d3e  ue::Single(x) =>
-00003700: 202a 782c 0a20 2020 2020 2020 2020 2020   *x,.           
-00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003720: 2020 2020 2050 7562 6c69 6356 616c 7565       PublicValue
-00003730: 3a3a 4d75 6c74 6928 7876 6563 2920 3d3e  ::Multi(xvec) =>
-00003740: 2078 7665 635b 695d 2c0a 2020 2020 2020   xvec[i],.      
-00003750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003760: 2020 2020 2020 7d29 0a20 2020 2020 2020        }).       
-00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003780: 2020 2020 202e 636f 6c6c 6563 7428 293b       .collect();
-00003790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000037a0: 2020 2020 2020 2020 206d 6174 6368 2067           match g
-000037b0: 6620 7b0a 2020 2020 2020 2020 2020 2020  f {.            
+000035b0: 2020 666f 7220 6920 696e 2030 2e2e 6e6d    for i in 0..nm
+000035c0: 756c 7469 207b 0a20 2020 2020 2020 2020  ulti {.         
+000035d0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000035e0: 6574 2067 6620 3d20 6d61 7463 6820 2667  et gf = match &g
+000035f0: 656e 5f66 6163 746f 7273 5b2a 6964 5d20  en_factors[*id] 
+00003600: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00003610: 2020 2020 2020 2020 2020 2020 2020 7375                su
+00003620: 7065 723a 3a47 656e 4661 6374 6f72 3a3a  per::GenFactor::
+00003630: 5369 6e67 6c65 2867 6673 2920 3d3e 2067  Single(gfs) => g
+00003640: 6673 2c0a 2020 2020 2020 2020 2020 2020  fs,.            
+00003650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003660: 7375 7065 723a 3a47 656e 4661 6374 6f72  super::GenFactor
+00003670: 3a3a 4d75 6c74 6928 6766 7629 203d 3e20  ::Multi(gfv) => 
+00003680: 2667 6676 5b69 5d2c 0a20 2020 2020 2020  &gfv[i],.       
+00003690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036a0: 207d 3b0a 2020 2020 2020 2020 2020 2020   };.            
+000036b0: 2020 2020 2020 2020 2020 2020 6c65 7420              let 
+000036c0: 696e 6469 6365 733a 2056 6563 3c43 6c61  indices: Vec<Cla
+000036d0: 7373 5661 6c3e 203d 206f 7073 0a20 2020  ssVal> = ops.   
+000036e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036f0: 2020 2020 2020 2020 202e 6974 6572 2829           .iter()
+00003700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003710: 2020 2020 2020 2020 2020 2020 202e 6d61               .ma
+00003720: 7028 7c70 767c 206d 6174 6368 202a 7076  p(|pv| match *pv
+00003730: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00003740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003750: 2020 2050 7562 6c69 6356 616c 7565 3a3a     PublicValue::
+00003760: 5369 6e67 6c65 2878 2920 3d3e 202a 782c  Single(x) => *x,
+00003770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003790: 2050 7562 6c69 6356 616c 7565 3a3a 4d75   PublicValue::Mu
+000037a0: 6c74 6928 7876 6563 2920 3d3e 2078 7665  lti(xvec) => xve
+000037b0: 635b 695d 2c0a 2020 2020 2020 2020 2020  c[i],.          
 000037c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037d0: 7375 7065 723a 3a47 656e 4661 6374 6f72  super::GenFactor
-000037e0: 496e 6e65 723a 3a44 656e 7365 2864 656e  Inner::Dense(den
-000037f0: 7365 5f66 6163 746f 7229 203d 3e20 7b0a  se_factor) => {.
+000037d0: 2020 7d29 0a20 2020 2020 2020 2020 2020    }).           
+000037e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037f0: 202e 636f 6c6c 6563 7428 293b 0a20 2020   .collect();.   
 00003800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003820: 6966 2021 2864 656e 7365 5f66 6163 746f  if !(dense_facto
-00003830: 725b 696e 6469 6365 730a 2020 2020 2020  r[indices.      
-00003840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003850: 2020 2020 2020 2020 2020 2020 2020 2e69                .i
-00003860: 7465 7228 290a 2020 2020 2020 2020 2020  ter().          
+00003810: 2020 2020 206d 6174 6368 2067 6620 7b0a       match gf {.
+00003820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003830: 2020 2020 2020 2020 2020 2020 7375 7065              supe
+00003840: 723a 3a47 656e 4661 6374 6f72 496e 6e65  r::GenFactorInne
+00003850: 723a 3a44 656e 7365 2864 656e 7365 5f66  r::Dense(dense_f
+00003860: 6163 746f 7229 203d 3e20 7b0a 2020 2020  actor) => {.    
 00003870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003880: 2020 2020 2020 2020 2020 2e6d 6170 287c            .map(|
-00003890: 787c 202a 7820 6173 2075 7369 7a65 290a  x| *x as usize).
-000038a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003880: 2020 2020 2020 2020 2020 2020 6966 2021              if !
+00003890: 2864 656e 7365 5f66 6163 746f 725b 696e  (dense_factor[in
+000038a0: 6469 6365 730a 2020 2020 2020 2020 2020  dices.          
 000038b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038c0: 2020 2020 2e63 6f6c 6c65 6374 3a3a 3c56      .collect::<V
-000038d0: 6563 3c75 7369 7a65 3e3e 2829 0a20 2020  ec<usize>>().   
+000038c0: 2020 2020 2020 2020 2020 2e69 7465 7228            .iter(
+000038d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
 000038e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003900: 202e 6173 5f73 6c69 6365 2829 5d0a 2020   .as_slice()].  
+000038f0: 2020 2020 2020 2e6d 6170 287c 787c 202a        .map(|x| *
+00003900: 7820 6173 2075 7369 7a65 290a 2020 2020  x as usize).    
 00003910: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003930: 2020 3e20 302e 3029 0a20 2020 2020 2020    > 0.0).       
-00003940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003950: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00003960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003970: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00003980: 6574 7572 6e20 4572 7228 4647 4572 726f  eturn Err(FGErro
-00003990: 723a 3a49 6e76 616c 6964 4765 6e65 7269  r::InvalidGeneri
-000039a0: 6346 6163 746f 7241 7373 6967 6e6d 656e  cFactorAssignmen
-000039b0: 7428 666f 726d 6174 2128 0a20 2020 2020  t(format!(.     
-000039c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003930: 2e63 6f6c 6c65 6374 3a3a 3c56 6563 3c75  .collect::<Vec<u
+00003940: 7369 7a65 3e3e 2829 0a20 2020 2020 2020  size>>().       
+00003950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003960: 2020 2020 2020 2020 2020 2020 202e 6173               .as
+00003970: 5f73 6c69 6365 2829 5d0a 2020 2020 2020  _slice()].      
+00003980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003990: 2020 2020 2020 2020 2020 2020 2020 3e20                > 
+000039a0: 302e 3029 0a20 2020 2020 2020 2020 2020  0.0).           
+000039b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039c0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
 000039d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039e0: 2020 2022 496e 7661 6c69 6420 6173 7369     "Invalid assi
-000039f0: 676e 6d65 6e74 2074 6f20 7b7d 3a20 7b3a  gnment to {}: {:
-00003a00: 3f7d 222c 0a20 2020 2020 2020 2020 2020  ?}",.           
-00003a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a20: 2020 2020 2020 2020 2020 2020 2066 6163               fac
-00003a30: 746f 725f 6e61 6d65 2e63 6c6f 6e65 2829  tor_name.clone()
-00003a40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a60: 2020 2020 2020 2020 2020 696e 6469 6365            indice
-00003a70: 732e 636c 6f6e 6528 290a 2020 2020 2020  s.clone().      
+000039e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000039f0: 6e20 4572 7228 4647 4572 726f 723a 3a49  n Err(FGError::I
+00003a00: 6e76 616c 6964 4765 6e65 7269 6346 6163  nvalidGenericFac
+00003a10: 746f 7241 7373 6967 6e6d 656e 7428 666f  torAssignment(fo
+00003a20: 726d 6174 2128 0a20 2020 2020 2020 2020  rmat!(.         
+00003a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003a50: 496e 7661 6c69 6420 6173 7369 676e 6d65  Invalid assignme
+00003a60: 6e74 2074 6f20 7b7d 3a20 7b3a 3f7d 222c  nt to {}: {:?}",
+00003a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00003a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a90: 2020 2020 2020 2020 2020 2020 2020 2929                ))
-00003aa0: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
+00003a90: 2020 2020 2020 2020 2066 6163 746f 725f           factor_
+00003aa0: 6e61 6d65 2e63 6c6f 6e65 2829 2c0a 2020  name.clone(),.  
 00003ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ac0: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ae0: 207d 0a0a 2020 2020 2020 2020 2020 2020   }..            
+00003ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ad0: 2020 2020 2020 696e 6469 6365 732e 636c        indices.cl
+00003ae0: 6f6e 6528 290a 2020 2020 2020 2020 2020  one().          
 00003af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b00: 7375 7065 723a 3a47 656e 4661 6374 6f72  super::GenFactor
-00003b10: 496e 6e65 723a 3a53 7061 7273 6546 756e  Inner::SparseFun
-00003b20: 6374 696f 6e61 6c28 7366 5f66 6163 746f  ctional(sf_facto
-00003b30: 7229 203d 3e20 7b0a 2020 2020 2020 2020  r) => {.        
-00003b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b50: 2020 2020 2020 2020 6966 2021 2873 665f          if !(sf_
-00003b60: 6661 6374 6f72 0a20 2020 2020 2020 2020  factor.         
-00003b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b80: 2020 2020 2020 2020 2020 202e 6f75 7465             .oute
-00003b90: 725f 6974 6572 2829 0a20 2020 2020 2020  r_iter().       
-00003ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bb0: 2020 2020 2020 2020 2020 2020 202e 616e               .an
-00003bc0: 7928 7c78 7c20 782e 6173 5f73 6c69 6365  y(|x| x.as_slice
-00003bd0: 2829 2e75 6e77 7261 7028 2920 3d3d 2069  ().unwrap() == i
-00003be0: 6e64 6963 6573 2e61 735f 736c 6963 6528  ndices.as_slice(
-00003bf0: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-00003c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c10: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00003c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c30: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00003c40: 2045 7272 2846 4745 7272 6f72 3a3a 496e   Err(FGError::In
-00003c50: 7661 6c69 6447 656e 6572 6963 4661 6374  validGenericFact
-00003c60: 6f72 4173 7369 676e 6d65 6e74 2866 6f72  orAssignment(for
-00003c70: 6d61 7421 280a 2020 2020 2020 2020 2020  mat!(.          
-00003c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c90: 2020 2020 2020 2020 2020 2020 2020 2249                "I
-00003ca0: 6e76 616c 6964 2061 7373 6967 6e6d 656e  nvalid assignmen
-00003cb0: 7420 746f 207b 7d3a 207b 3a3f 7d22 2c0a  t to {}: {:?}",.
-00003cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ce0: 2020 2020 2020 2020 6661 6374 6f72 5f6e          factor_n
-00003cf0: 616d 652e 636c 6f6e 6528 292c 0a20 2020  ame.clone(),.   
-00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d20: 2020 2020 2069 6e64 6963 6573 2e63 6c6f       indices.clo
-00003d30: 6e65 2829 0a20 2020 2020 2020 2020 2020  ne().           
+00003b00: 2020 2020 2020 2020 2020 2929 293b 0a20            )));. 
+00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b20: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00003b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003b40: 2020 2020 2020 2020 2020 2020 207d 0a0a               }..
+00003b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b60: 2020 2020 2020 2020 2020 2020 7375 7065              supe
+00003b70: 723a 3a47 656e 4661 6374 6f72 496e 6e65  r::GenFactorInne
+00003b80: 723a 3a53 7061 7273 6546 756e 6374 696f  r::SparseFunctio
+00003b90: 6e61 6c28 7366 5f66 6163 746f 7229 203d  nal(sf_factor) =
+00003ba0: 3e20 7b0a 2020 2020 2020 2020 2020 2020  > {.            
+00003bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bc0: 2020 2020 6966 2021 2873 665f 6661 6374      if !(sf_fact
+00003bd0: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
+00003be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bf0: 2020 2020 2020 202e 6f75 7465 725f 6974         .outer_it
+00003c00: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
+00003c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c20: 2020 2020 2020 2020 202e 616e 7928 7c78           .any(|x
+00003c30: 7c20 782e 6173 5f73 6c69 6365 2829 2e75  | x.as_slice().u
+00003c40: 6e77 7261 7028 2920 3d3d 2069 6e64 6963  nwrap() == indic
+00003c50: 6573 2e61 735f 736c 6963 6528 2929 290a  es.as_slice())).
+00003c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c80: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00003c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ca0: 2020 2020 2020 7265 7475 726e 2045 7272        return Err
+00003cb0: 2846 4745 7272 6f72 3a3a 496e 7661 6c69  (FGError::Invali
+00003cc0: 6447 656e 6572 6963 4661 6374 6f72 4173  dGenericFactorAs
+00003cd0: 7369 676e 6d65 6e74 2866 6f72 6d61 7421  signment(format!
+00003ce0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00003cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d00: 2020 2020 2020 2020 2020 2249 6e76 616c            "Inval
+00003d10: 6964 2061 7373 6967 6e6d 656e 7420 746f  id assignment to
+00003d20: 207b 7d3a 207b 3a3f 7d22 2c0a 2020 2020   {}: {:?}",.    
+00003d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d50: 2020 2020 2020 2020 2029 2929 3b0a 2020           )));.  
-00003d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d70: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00003d50: 2020 2020 6661 6374 6f72 5f6e 616d 652e      factor_name.
+00003d60: 636c 6f6e 6528 292c 0a20 2020 2020 2020  clone(),.       
+00003d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d90: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00003da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003db0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00003dc0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00003dd0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00003de0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00003df0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00003e00: 4f6b 2828 2929 0a20 2020 207d 0a0a 2020  Ok(()).    }..  
-00003e10: 2020 7075 6228 7375 7065 7229 2066 6e20    pub(super) fn 
-00003e20: 7265 6475 6365 5f70 7562 2826 7365 6c66  reduce_pub(&self
-00003e30: 2c20 7075 626c 6963 5f76 616c 7565 733a  , public_values:
-00003e40: 2026 5b50 7562 6c69 6356 616c 7565 5d29   &[PublicValue])
-00003e50: 202d 3e20 4661 6374 6f72 5665 633c 5075   -> FactorVec<Pu
-00003e60: 626c 6963 5661 6c75 653e 207b 0a20 2020  blicValue> {.   
-00003e70: 2020 2020 2073 656c 662e 6661 6374 6f72       self.factor
-00003e80: 730a 2020 2020 2020 2020 2020 2020 2e76  s.            .v
-00003e90: 616c 7565 7328 290a 2020 2020 2020 2020  alues().        
-00003ea0: 2020 2020 2e6d 6170 287c 6661 6374 6f72      .map(|factor
-00003eb0: 7c20 7b0a 2020 2020 2020 2020 2020 2020  | {.            
-00003ec0: 2020 2020 6d61 7463 6820 2666 6163 746f      match &facto
-00003ed0: 722e 6b69 6e64 207b 0a20 2020 2020 2020  r.kind {.       
-00003ee0: 2020 2020 2020 2020 2020 2020 202f 2f20               // 
-00003ef0: 4e6f 7420 7573 6564 0a20 2020 2020 2020  Not used.       
-00003f00: 2020 2020 2020 2020 2020 2020 2046 6163               Fac
-00003f10: 746f 724b 696e 643a 3a41 7373 6967 6e20  torKind::Assign 
-00003f20: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00003f30: 2020 2020 2020 2020 2020 6578 7072 3a20            expr: 
-00003f40: 4578 7072 4661 6374 6f72 3a3a 4e4f 542c  ExprFactor::NOT,
-00003f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003f60: 2020 2020 2020 2020 202e 2e0a 2020 2020           ...    
-00003f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f80: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00003f90: 2020 2020 2020 7c20 4661 6374 6f72 4b69        | FactorKi
-00003fa0: 6e64 3a3a 4173 7369 676e 207b 0a20 2020  nd::Assign {.   
-00003fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fc0: 2020 2020 2065 7870 723a 2045 7870 7246       expr: ExprF
-00003fd0: 6163 746f 723a 3a4c 4f4f 4b55 5020 7b20  actor::LOOKUP { 
-00003fe0: 2e2e 207d 2c0a 2020 2020 2020 2020 2020  .. },.          
-00003ff0: 2020 2020 2020 2020 2020 2020 2020 2e2e                ..
-00004000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004010: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-00004020: 2020 2020 2020 2020 2020 207c 2046 6163             | Fac
-00004030: 746f 724b 696e 643a 3a47 656e 4661 6374  torKind::GenFact
-00004040: 6f72 207b 202e 2e20 7d20 3d3e 2050 7562  or { .. } => Pub
-00004050: 6c69 6356 616c 7565 3a3a 5369 6e67 6c65  licValue::Single
-00004060: 2830 292c 0a20 2020 2020 2020 2020 2020  (0),.           
-00004070: 2020 2020 2020 2020 2046 6163 746f 724b           FactorK
-00004080: 696e 643a 3a41 7373 6967 6e20 7b20 6578  ind::Assign { ex
-00004090: 7072 2c20 2e2e 207d 203d 3e20 7365 6c66  pr, .. } => self
-000040a0: 2e6d 6572 6765 5f70 7562 7328 0a20 2020  .merge_pubs(.   
-000040b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040c0: 2020 2020 2065 7870 722c 0a20 2020 2020       expr,.     
-000040d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040e0: 2020 2066 6163 746f 720a 2020 2020 2020     factor.      
-000040f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004100: 2020 2020 2020 2e70 7562 6c69 6373 0a20        .publics. 
-00004110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004120: 2020 2020 2020 2020 2020 202e 6974 6572             .iter
-00004130: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00004140: 2020 2020 2020 2020 2020 2020 2020 202e                 .
-00004150: 6d61 7028 7c28 7075 625f 6964 2c20 6e76  map(|(pub_id, nv
-00004160: 297c 2028 2670 7562 6c69 635f 7661 6c75  )| (&public_valu
-00004170: 6573 5b2a 7075 625f 6964 5d2c 202a 6e76  es[*pub_id], *nv
-00004180: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-00004190: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-000041a0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-000041b0: 2020 2020 2020 2020 207d 290a 2020 2020           }).    
-000041c0: 2020 2020 2020 2020 2e63 6f6c 6c65 6374          .collect
-000041d0: 2829 0a20 2020 207d 0a20 2020 2066 6e20  ().    }.    fn 
-000041e0: 6e6f 7428 2673 656c 662c 2078 3a20 436c  not(&self, x: Cl
-000041f0: 6173 7356 616c 2920 2d3e 2043 6c61 7373  assVal) -> Class
-00004200: 5661 6c20 7b0a 2020 2020 2020 2020 2828  Val {.        ((
-00004210: 7365 6c66 2e6e 6320 2d20 3129 2061 7320  self.nc - 1) as 
-00004220: 436c 6173 7356 616c 2920 5e20 780a 2020  ClassVal) ^ x.  
-00004230: 2020 7d0a 2020 2020 666e 206d 6572 6765    }.    fn merge
-00004240: 5f70 7562 733c 2761 3e28 0a20 2020 2020  _pubs<'a>(.     
-00004250: 2020 2026 7365 6c66 2c0a 2020 2020 2020     &self,.      
-00004260: 2020 6578 7072 3a20 2645 7870 7246 6163    expr: &ExprFac
-00004270: 746f 722c 0a20 2020 2020 2020 202f 2f20  tor,.        // 
-00004280: 626f 6f6c 2069 7320 7468 6520 2269 6e76  bool is the "inv
-00004290: 7365 7273 6522 2066 6f72 2065 7665 7279  serse" for every
-000042a0: 2069 7465 6d0a 2020 2020 2020 2020 7075   item.        pu
-000042b0: 6273 3a20 696d 706c 2049 7465 7261 746f  bs: impl Iterato
-000042c0: 723c 4974 656d 203d 2028 2627 6120 5075  r<Item = (&'a Pu
-000042d0: 626c 6963 5661 6c75 652c 2062 6f6f 6c29  blicValue, bool)
-000042e0: 3e2c 0a20 2020 2029 202d 3e20 5075 626c  >,.    ) -> Publ
-000042f0: 6963 5661 6c75 6520 7b0a 2020 2020 2020  icValue {.      
-00004300: 2020 6c65 7420 6d65 7267 655f 696e 6e65    let merge_inne
-00004310: 7220 3d20 7c70 313a 2050 7562 6c69 6356  r = |p1: PublicV
-00004320: 616c 7565 2c20 2870 322c 206e 7632 293a  alue, (p2, nv2):
-00004330: 2028 2650 7562 6c69 6356 616c 7565 2c20   (&PublicValue, 
-00004340: 626f 6f6c 297c 207b 0a20 2020 2020 2020  bool)| {.       
-00004350: 2020 2020 206c 6574 2066 203d 207c 783a       let f = |x:
-00004360: 2043 6c61 7373 5661 6c2c 2079 3a20 436c   ClassVal, y: Cl
-00004370: 6173 7356 616c 7c20 7b0a 2020 2020 2020  assVal| {.      
-00004380: 2020 2020 2020 2020 2020 6578 7072 2e6d            expr.m
-00004390: 6572 6765 2878 2c20 6966 206e 7632 207b  erge(x, if nv2 {
-000043a0: 2073 656c 662e 6e6f 7428 7929 207d 2065   self.not(y) } e
-000043b0: 6c73 6520 7b20 7920 7d2c 2073 656c 662e  lse { y }, self.
-000043c0: 6e63 290a 2020 2020 2020 2020 2020 2020  nc).            
-000043d0: 7d3b 0a20 2020 2020 2020 2020 2020 206d  };.            m
-000043e0: 6174 6368 2028 7031 2c20 7032 2920 7b0a  atch (p1, p2) {.
-000043f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004400: 2850 7562 6c69 6356 616c 7565 3a3a 5369  (PublicValue::Si
-00004410: 6e67 6c65 2863 3129 2c20 5075 626c 6963  ngle(c1), Public
-00004420: 5661 6c75 653a 3a53 696e 676c 6528 6332  Value::Single(c2
-00004430: 2929 203d 3e20 7b0a 2020 2020 2020 2020  )) => {.        
-00004440: 2020 2020 2020 2020 2020 2020 5075 626c              Publ
-00004450: 6963 5661 6c75 653a 3a53 696e 676c 6528  icValue::Single(
-00004460: 6628 6331 2c20 2a63 3229 290a 2020 2020  f(c1, *c2)).    
-00004470: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00004480: 2020 2020 2020 2020 2020 2020 2020 2850                (P
-00004490: 7562 6c69 6356 616c 7565 3a3a 5369 6e67  ublicValue::Sing
-000044a0: 6c65 2863 3129 2c20 5075 626c 6963 5661  le(c1), PublicVa
-000044b0: 6c75 653a 3a4d 756c 7469 2863 3229 2920  lue::Multi(c2)) 
-000044c0: 3d3e 207b 0a20 2020 2020 2020 2020 2020  => {.           
-000044d0: 2020 2020 2020 2020 2050 7562 6c69 6356           PublicV
-000044e0: 616c 7565 3a3a 4d75 6c74 6928 6332 2e69  alue::Multi(c2.i
-000044f0: 7465 7228 292e 6d61 7028 7c63 327c 2066  ter().map(|c2| f
-00004500: 2863 312c 202a 6332 2929 2e63 6f6c 6c65  (c1, *c2)).colle
-00004510: 6374 2829 290a 2020 2020 2020 2020 2020  ct()).          
-00004520: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00004530: 2020 2020 2020 2020 2850 7562 6c69 6356          (PublicV
-00004540: 616c 7565 3a3a 4d75 6c74 6928 6d75 7420  alue::Multi(mut 
-00004550: 6331 292c 2050 7562 6c69 6356 616c 7565  c1), PublicValue
-00004560: 3a3a 5369 6e67 6c65 2863 3229 2920 3d3e  ::Single(c2)) =>
-00004570: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00004580: 2020 2020 2020 2066 6f72 2063 3120 696e         for c1 in
-00004590: 2063 312e 6974 6572 5f6d 7574 2829 207b   c1.iter_mut() {
-000045a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000045b0: 2020 2020 2020 2020 202a 6331 203d 2066           *c1 = f
-000045c0: 282a 6331 2c20 2a63 3229 3b0a 2020 2020  (*c1, *c2);.    
-000045d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045e0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-000045f0: 2020 2020 2020 5075 626c 6963 5661 6c75        PublicValu
-00004600: 653a 3a4d 756c 7469 2863 3129 0a20 2020  e::Multi(c1).   
-00004610: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-00004620: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00004630: 5075 626c 6963 5661 6c75 653a 3a4d 756c  PublicValue::Mul
-00004640: 7469 286d 7574 2063 3129 2c20 5075 626c  ti(mut c1), Publ
-00004650: 6963 5661 6c75 653a 3a4d 756c 7469 2863  icValue::Multi(c
-00004660: 3229 2920 3d3e 207b 0a20 2020 2020 2020  2)) => {.       
-00004670: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00004680: 2028 6331 2c20 6332 2920 696e 2063 312e   (c1, c2) in c1.
-00004690: 6974 6572 5f6d 7574 2829 2e7a 6970 2863  iter_mut().zip(c
-000046a0: 322e 6974 6572 2829 2920 7b0a 2020 2020  2.iter()) {.    
-000046b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046c0: 2020 2020 2a63 3120 3d20 6628 2a63 312c      *c1 = f(*c1,
-000046d0: 202a 6332 293b 0a20 2020 2020 2020 2020   *c2);.         
-000046e0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-000046f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004700: 2050 7562 6c69 6356 616c 7565 3a3a 4d75   PublicValue::Mu
-00004710: 6c74 6928 6331 290a 2020 2020 2020 2020  lti(c1).        
-00004720: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00004730: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00004740: 7d3b 0a20 2020 2020 2020 2070 7562 732e  };.        pubs.
-00004750: 666f 6c64 2850 7562 6c69 6356 616c 7565  fold(PublicValue
-00004760: 3a3a 5369 6e67 6c65 2865 7870 722e 6e65  ::Single(expr.ne
-00004770: 7574 7261 6c28 7365 6c66 2e6e 6329 292c  utral(self.nc)),
-00004780: 206d 6572 6765 5f69 6e6e 6572 290a 2020   merge_inner).  
-00004790: 2020 7d0a 0a20 2020 2070 7562 2873 7570    }..    pub(sup
-000047a0: 6572 2920 666e 2069 735f 6379 636c 6963  er) fn is_cyclic
-000047b0: 2826 7365 6c66 2c20 6d75 6c74 695f 6578  (&self, multi_ex
-000047c0: 6563 3a20 626f 6f6c 2920 2d3e 2062 6f6f  ec: bool) -> boo
-000047d0: 6c20 7b0a 2020 2020 2020 2020 6966 206d  l {.        if m
-000047e0: 756c 7469 5f65 7865 6320 7b0a 2020 2020  ulti_exec {.    
-000047f0: 2020 2020 2020 2020 7365 6c66 2e63 7963          self.cyc
-00004800: 6c69 635f 6d75 6c74 690a 2020 2020 2020  lic_multi.      
-00004810: 2020 7d20 656c 7365 207b 0a20 2020 2020    } else {.     
-00004820: 2020 2020 2020 2073 656c 662e 6379 636c         self.cycl
-00004830: 6963 5f73 696e 676c 650a 2020 2020 2020  ic_single.      
-00004840: 2020 7d0a 2020 2020 7d0a 0a20 2020 2070    }.    }..    p
-00004850: 7562 2873 7570 6572 2920 666e 2070 726f  ub(super) fn pro
-00004860: 7061 6761 7469 6f6e 5f6f 7264 6572 2826  pagation_order(&
-00004870: 7365 6c66 2c20 7661 723a 2056 6172 4964  self, var: VarId
-00004880: 2920 2d3e 2056 6563 3c28 4e6f 6465 2c20  ) -> Vec<(Node, 
-00004890: 4f70 7469 6f6e 3c4e 6f64 653e 293e 207b  Option<Node>)> {
-000048a0: 0a20 2020 2020 2020 206c 6574 206d 7574  .        let mut
-000048b0: 2070 726f 7061 6761 7469 6f6e 7320 3d20   propagations = 
-000048c0: 7665 6321 5b28 4e6f 6465 3a3a 5661 7228  vec![(Node::Var(
-000048d0: 7661 7229 2c20 4e6f 6e65 295d 3b0a 2020  var), None)];.  
-000048e0: 2020 2020 2020 7065 7467 7261 7068 3a3a        petgraph::
-000048f0: 7669 7369 743a 3a64 6570 7468 5f66 6972  visit::depth_fir
-00004900: 7374 5f73 6561 7263 6828 2673 656c 662e  st_search(&self.
-00004910: 7065 7467 7261 7068 2c20 5b73 656c 662e  petgraph, [self.
-00004920: 7661 725f 6772 6170 685f 6964 735b 7661  var_graph_ids[va
-00004930: 725d 5d2c 207c 6576 656e 747c 207b 0a20  r]], |event| {. 
-00004940: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00004950: 7420 7065 7467 7261 7068 3a3a 7669 7369  t petgraph::visi
-00004960: 743a 3a44 6673 4576 656e 743a 3a54 7265  t::DfsEvent::Tre
-00004970: 6545 6467 6528 7061 7265 6e74 2c20 6e6f  eEdge(parent, no
-00004980: 6465 2920 3d20 6576 656e 7420 7b0a 2020  de) = event {.  
-00004990: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000049a0: 6f70 6167 6174 696f 6e73 2e70 7573 6828  opagations.push(
-000049b0: 2873 656c 662e 7065 7467 7261 7068 5b6e  (self.petgraph[n
-000049c0: 6f64 655d 2c20 536f 6d65 2873 656c 662e  ode], Some(self.
-000049d0: 7065 7467 7261 7068 5b70 6172 656e 745d  petgraph[parent]
-000049e0: 2929 293b 0a20 2020 2020 2020 2020 2020  )));.           
-000049f0: 207d 0a20 2020 2020 2020 2020 2020 2070   }.            p
-00004a00: 6574 6772 6170 683a 3a76 6973 6974 3a3a  etgraph::visit::
-00004a10: 436f 6e74 726f 6c3a 3a3c 2829 3e3a 3a43  Control::<()>::C
-00004a20: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-00004a30: 7d29 3b0a 2020 2020 2020 2020 7072 6f70  });.        prop
-00004a40: 6167 6174 696f 6e73 2e72 6576 6572 7365  agations.reverse
-00004a50: 2829 3b0a 2020 2020 2020 2020 7072 6f70  ();.        prop
-00004a60: 6167 6174 696f 6e73 0a20 2020 207d 0a7d  agations.    }.}
-00004a70: 0a0a 696d 706c 204e 6f64 6520 7b0a 2020  ..impl Node {.  
-00004a80: 2020 7075 6228 7375 7065 7229 2066 6e20    pub(super) fn 
-00004a90: 7661 7228 7365 6c66 2920 2d3e 204f 7074  var(self) -> Opt
-00004aa0: 696f 6e3c 5661 7249 643e 207b 0a20 2020  ion<VarId> {.   
-00004ab0: 2020 2020 2069 6620 6c65 7420 4e6f 6465       if let Node
-00004ac0: 3a3a 5661 7228 6964 2920 3d20 7365 6c66  ::Var(id) = self
-00004ad0: 207b 0a20 2020 2020 2020 2020 2020 2053   {.            S
-00004ae0: 6f6d 6528 6964 290a 2020 2020 2020 2020  ome(id).        
-00004af0: 7d20 656c 7365 207b 0a20 2020 2020 2020  } else {.       
-00004b00: 2020 2020 204e 6f6e 650a 2020 2020 2020       None.      
-00004b10: 2020 7d0a 2020 2020 7d0a 2020 2020 7075    }.    }.    pu
-00004b20: 6228 7375 7065 7229 2066 6e20 6661 6374  b(super) fn fact
-00004b30: 6f72 2873 656c 6629 202d 3e20 4f70 7469  or(self) -> Opti
-00004b40: 6f6e 3c46 6163 746f 7249 643e 207b 0a20  on<FactorId> {. 
-00004b50: 2020 2020 2020 2069 6620 6c65 7420 4e6f         if let No
-00004b60: 6465 3a3a 4661 6374 6f72 2869 6429 203d  de::Factor(id) =
-00004b70: 2073 656c 6620 7b0a 2020 2020 2020 2020   self {.        
-00004b80: 2020 2020 536f 6d65 2869 6429 0a20 2020      Some(id).   
-00004b90: 2020 2020 207d 2065 6c73 6520 7b0a 2020       } else {.  
-00004ba0: 2020 2020 2020 2020 2020 4e6f 6e65 0a20            None. 
-00004bb0: 2020 2020 2020 207d 0a20 2020 207d 0a7d         }.    }.}
-00004bc0: 0a                                       .
+00003d90: 2069 6e64 6963 6573 2e63 6c6f 6e65 2829   indices.clone()
+00003da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003dc0: 2020 2020 2029 2929 3b0a 2020 2020 2020       )));.      
+00003dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003de0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00003df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e00: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00003e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e20: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00003e30: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00003e40: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00003e50: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00003e60: 2020 7d0a 2020 2020 2020 2020 4f6b 2828    }.        Ok((
+00003e70: 2929 0a20 2020 207d 0a0a 2020 2020 7075  )).    }..    pu
+00003e80: 6228 7375 7065 7229 2066 6e20 7265 6475  b(super) fn redu
+00003e90: 6365 5f70 7562 2826 7365 6c66 2c20 7075  ce_pub(&self, pu
+00003ea0: 626c 6963 5f76 616c 7565 733a 2026 5b50  blic_values: &[P
+00003eb0: 7562 6c69 6356 616c 7565 5d29 202d 3e20  ublicValue]) -> 
+00003ec0: 4661 6374 6f72 5665 633c 5075 626c 6963  FactorVec<Public
+00003ed0: 5661 6c75 653e 207b 0a20 2020 2020 2020  Value> {.       
+00003ee0: 2073 656c 662e 6661 6374 6f72 730a 2020   self.factors.  
+00003ef0: 2020 2020 2020 2020 2020 2e76 616c 7565            .value
+00003f00: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+00003f10: 2e6d 6170 287c 6661 6374 6f72 7c20 7b0a  .map(|factor| {.
+00003f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f30: 6d61 7463 6820 2666 6163 746f 722e 6b69  match &factor.ki
+00003f40: 6e64 207b 0a20 2020 2020 2020 2020 2020  nd {.           
+00003f50: 2020 2020 2020 2020 202f 2f20 4e6f 7420           // Not 
+00003f60: 7573 6564 0a20 2020 2020 2020 2020 2020  used.           
+00003f70: 2020 2020 2020 2020 2046 6163 746f 724b           FactorK
+00003f80: 696e 643a 3a41 7373 6967 6e20 7b0a 2020  ind::Assign {.  
+00003f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fa0: 2020 2020 2020 6578 7072 3a20 4578 7072        expr: Expr
+00003fb0: 4661 6374 6f72 3a3a 4e4f 542c 0a20 2020  Factor::NOT,.   
+00003fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fd0: 2020 2020 202e 2e0a 2020 2020 2020 2020       ...        
+00003fe0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00003ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004000: 2020 7c20 4661 6374 6f72 4b69 6e64 3a3a    | FactorKind::
+00004010: 4173 7369 676e 207b 0a20 2020 2020 2020  Assign {.       
+00004020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004030: 2065 7870 723a 2045 7870 7246 6163 746f   expr: ExprFacto
+00004040: 723a 3a4c 4f4f 4b55 5020 7b20 2e2e 207d  r::LOOKUP { .. }
+00004050: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004060: 2020 2020 2020 2020 2020 2e2e 0a20 2020            ...   
+00004070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004080: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
+00004090: 2020 2020 2020 207c 2046 6163 746f 724b         | FactorK
+000040a0: 696e 643a 3a47 656e 4661 6374 6f72 207b  ind::GenFactor {
+000040b0: 202e 2e20 7d20 3d3e 2050 7562 6c69 6356   .. } => PublicV
+000040c0: 616c 7565 3a3a 5369 6e67 6c65 2830 292c  alue::Single(0),
+000040d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000040e0: 2020 2020 2046 6163 746f 724b 696e 643a       FactorKind:
+000040f0: 3a41 7373 6967 6e20 7b20 6578 7072 2c20  :Assign { expr, 
+00004100: 2e2e 207d 203d 3e20 7365 6c66 2e6d 6572  .. } => self.mer
+00004110: 6765 5f70 7562 7328 0a20 2020 2020 2020  ge_pubs(.       
+00004120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004130: 2065 7870 722c 0a20 2020 2020 2020 2020   expr,.         
+00004140: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00004150: 6163 746f 720a 2020 2020 2020 2020 2020  actor.          
+00004160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004170: 2020 2e70 7562 6c69 6373 0a20 2020 2020    .publics.     
+00004180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004190: 2020 2020 2020 202e 6974 6572 2829 0a20         .iter(). 
+000041a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041b0: 2020 2020 2020 2020 2020 202e 6d61 7028             .map(
+000041c0: 7c28 7075 625f 6964 2c20 6e76 297c 2028  |(pub_id, nv)| (
+000041d0: 2670 7562 6c69 635f 7661 6c75 6573 5b2a  &public_values[*
+000041e0: 7075 625f 6964 5d2c 202a 6e76 2929 2c0a  pub_id], *nv)),.
+000041f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004200: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00004210: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00004220: 2020 2020 207d 290a 2020 2020 2020 2020       }).        
+00004230: 2020 2020 2e63 6f6c 6c65 6374 2829 0a20      .collect(). 
+00004240: 2020 207d 0a20 2020 2066 6e20 6e6f 7428     }.    fn not(
+00004250: 2673 656c 662c 2078 3a20 436c 6173 7356  &self, x: ClassV
+00004260: 616c 2920 2d3e 2043 6c61 7373 5661 6c20  al) -> ClassVal 
+00004270: 7b0a 2020 2020 2020 2020 2828 7365 6c66  {.        ((self
+00004280: 2e6e 6320 2d20 3129 2061 7320 436c 6173  .nc - 1) as Clas
+00004290: 7356 616c 2920 5e20 780a 2020 2020 7d0a  sVal) ^ x.    }.
+000042a0: 2020 2020 666e 206d 6572 6765 5f70 7562      fn merge_pub
+000042b0: 733c 2761 3e28 0a20 2020 2020 2020 2026  s<'a>(.        &
+000042c0: 7365 6c66 2c0a 2020 2020 2020 2020 6578  self,.        ex
+000042d0: 7072 3a20 2645 7870 7246 6163 746f 722c  pr: &ExprFactor,
+000042e0: 0a20 2020 2020 2020 202f 2f20 626f 6f6c  .        // bool
+000042f0: 2069 7320 7468 6520 2269 6e76 7365 7273   is the "invsers
+00004300: 6522 2066 6f72 2065 7665 7279 2069 7465  e" for every ite
+00004310: 6d0a 2020 2020 2020 2020 7075 6273 3a20  m.        pubs: 
+00004320: 696d 706c 2049 7465 7261 746f 723c 4974  impl Iterator<It
+00004330: 656d 203d 2028 2627 6120 5075 626c 6963  em = (&'a Public
+00004340: 5661 6c75 652c 2062 6f6f 6c29 3e2c 0a20  Value, bool)>,. 
+00004350: 2020 2029 202d 3e20 5075 626c 6963 5661     ) -> PublicVa
+00004360: 6c75 6520 7b0a 2020 2020 2020 2020 6c65  lue {.        le
+00004370: 7420 6d65 7267 655f 696e 6e65 7220 3d20  t merge_inner = 
+00004380: 7c70 313a 2050 7562 6c69 6356 616c 7565  |p1: PublicValue
+00004390: 2c20 2870 322c 206e 7632 293a 2028 2650  , (p2, nv2): (&P
+000043a0: 7562 6c69 6356 616c 7565 2c20 626f 6f6c  ublicValue, bool
+000043b0: 297c 207b 0a20 2020 2020 2020 2020 2020  )| {.           
+000043c0: 206c 6574 2066 203d 207c 783a 2043 6c61   let f = |x: Cla
+000043d0: 7373 5661 6c2c 2079 3a20 436c 6173 7356  ssVal, y: ClassV
+000043e0: 616c 7c20 7b0a 2020 2020 2020 2020 2020  al| {.          
+000043f0: 2020 2020 2020 6578 7072 2e6d 6572 6765        expr.merge
+00004400: 2878 2c20 6966 206e 7632 207b 2073 656c  (x, if nv2 { sel
+00004410: 662e 6e6f 7428 7929 207d 2065 6c73 6520  f.not(y) } else 
+00004420: 7b20 7920 7d2c 2073 656c 662e 6e63 290a  { y }, self.nc).
+00004430: 2020 2020 2020 2020 2020 2020 7d3b 0a20              };. 
+00004440: 2020 2020 2020 2020 2020 206d 6174 6368             match
+00004450: 2028 7031 2c20 7032 2920 7b0a 2020 2020   (p1, p2) {.    
+00004460: 2020 2020 2020 2020 2020 2020 2850 7562              (Pub
+00004470: 6c69 6356 616c 7565 3a3a 5369 6e67 6c65  licValue::Single
+00004480: 2863 3129 2c20 5075 626c 6963 5661 6c75  (c1), PublicValu
+00004490: 653a 3a53 696e 676c 6528 6332 2929 203d  e::Single(c2)) =
+000044a0: 3e20 7b0a 2020 2020 2020 2020 2020 2020  > {.            
+000044b0: 2020 2020 2020 2020 5075 626c 6963 5661          PublicVa
+000044c0: 6c75 653a 3a53 696e 676c 6528 6628 6331  lue::Single(f(c1
+000044d0: 2c20 2a63 3229 290a 2020 2020 2020 2020  , *c2)).        
+000044e0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+000044f0: 2020 2020 2020 2020 2020 2850 7562 6c69            (Publi
+00004500: 6356 616c 7565 3a3a 5369 6e67 6c65 2863  cValue::Single(c
+00004510: 3129 2c20 5075 626c 6963 5661 6c75 653a  1), PublicValue:
+00004520: 3a4d 756c 7469 2863 3229 2920 3d3e 207b  :Multi(c2)) => {
+00004530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004540: 2020 2020 2050 7562 6c69 6356 616c 7565       PublicValue
+00004550: 3a3a 4d75 6c74 6928 6332 2e69 7465 7228  ::Multi(c2.iter(
+00004560: 292e 6d61 7028 7c63 327c 2066 2863 312c  ).map(|c2| f(c1,
+00004570: 202a 6332 2929 2e63 6f6c 6c65 6374 2829   *c2)).collect()
+00004580: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00004590: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+000045a0: 2020 2020 2850 7562 6c69 6356 616c 7565      (PublicValue
+000045b0: 3a3a 4d75 6c74 6928 6d75 7420 6331 292c  ::Multi(mut c1),
+000045c0: 2050 7562 6c69 6356 616c 7565 3a3a 5369   PublicValue::Si
+000045d0: 6e67 6c65 2863 3229 2920 3d3e 207b 0a20  ngle(c2)) => {. 
+000045e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045f0: 2020 2066 6f72 2063 3120 696e 2063 312e     for c1 in c1.
+00004600: 6974 6572 5f6d 7574 2829 207b 0a20 2020  iter_mut() {.   
+00004610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004620: 2020 2020 202a 6331 203d 2066 282a 6331       *c1 = f(*c1
+00004630: 2c20 2a63 3229 3b0a 2020 2020 2020 2020  , *c2);.        
+00004640: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00004650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004660: 2020 5075 626c 6963 5661 6c75 653a 3a4d    PublicValue::M
+00004670: 756c 7469 2863 3129 0a20 2020 2020 2020  ulti(c1).       
+00004680: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00004690: 2020 2020 2020 2020 2020 2028 5075 626c             (Publ
+000046a0: 6963 5661 6c75 653a 3a4d 756c 7469 286d  icValue::Multi(m
+000046b0: 7574 2063 3129 2c20 5075 626c 6963 5661  ut c1), PublicVa
+000046c0: 6c75 653a 3a4d 756c 7469 2863 3229 2920  lue::Multi(c2)) 
+000046d0: 3d3e 207b 0a20 2020 2020 2020 2020 2020  => {.           
+000046e0: 2020 2020 2020 2020 2066 6f72 2028 6331           for (c1
+000046f0: 2c20 6332 2920 696e 2063 312e 6974 6572  , c2) in c1.iter
+00004700: 5f6d 7574 2829 2e7a 6970 2863 322e 6974  _mut().zip(c2.it
+00004710: 6572 2829 2920 7b0a 2020 2020 2020 2020  er()) {.        
+00004720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004730: 2a63 3120 3d20 6628 2a63 312c 202a 6332  *c1 = f(*c1, *c2
+00004740: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
+00004750: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00004760: 2020 2020 2020 2020 2020 2020 2050 7562               Pub
+00004770: 6c69 6356 616c 7565 3a3a 4d75 6c74 6928  licValue::Multi(
+00004780: 6331 290a 2020 2020 2020 2020 2020 2020  c1).            
+00004790: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+000047a0: 2020 7d0a 2020 2020 2020 2020 7d3b 0a20    }.        };. 
+000047b0: 2020 2020 2020 2070 7562 732e 666f 6c64         pubs.fold
+000047c0: 2850 7562 6c69 6356 616c 7565 3a3a 5369  (PublicValue::Si
+000047d0: 6e67 6c65 2865 7870 722e 6e65 7574 7261  ngle(expr.neutra
+000047e0: 6c28 7365 6c66 2e6e 6329 292c 206d 6572  l(self.nc)), mer
+000047f0: 6765 5f69 6e6e 6572 290a 2020 2020 7d0a  ge_inner).    }.
+00004800: 0a20 2020 2070 7562 2873 7570 6572 2920  .    pub(super) 
+00004810: 666e 2069 735f 6379 636c 6963 2826 7365  fn is_cyclic(&se
+00004820: 6c66 2c20 6d75 6c74 695f 6578 6563 3a20  lf, multi_exec: 
+00004830: 626f 6f6c 2920 2d3e 2062 6f6f 6c20 7b0a  bool) -> bool {.
+00004840: 2020 2020 2020 2020 6966 206d 756c 7469          if multi
+00004850: 5f65 7865 6320 7b0a 2020 2020 2020 2020  _exec {.        
+00004860: 2020 2020 7365 6c66 2e63 7963 6c69 635f      self.cyclic_
+00004870: 6d75 6c74 690a 2020 2020 2020 2020 7d20  multi.        } 
+00004880: 656c 7365 207b 0a20 2020 2020 2020 2020  else {.         
+00004890: 2020 2073 656c 662e 6379 636c 6963 5f73     self.cyclic_s
+000048a0: 696e 676c 650a 2020 2020 2020 2020 7d0a  ingle.        }.
+000048b0: 2020 2020 7d0a 0a20 2020 2070 7562 2873      }..    pub(s
+000048c0: 7570 6572 2920 666e 2070 726f 7061 6761  uper) fn propaga
+000048d0: 7469 6f6e 5f6f 7264 6572 2826 7365 6c66  tion_order(&self
+000048e0: 2c20 7661 723a 2056 6172 4964 2920 2d3e  , var: VarId) ->
+000048f0: 2056 6563 3c28 4e6f 6465 2c20 4f70 7469   Vec<(Node, Opti
+00004900: 6f6e 3c4e 6f64 653e 293e 207b 0a20 2020  on<Node>)> {.   
+00004910: 2020 2020 206c 6574 206d 7574 2070 726f       let mut pro
+00004920: 7061 6761 7469 6f6e 7320 3d20 7665 6321  pagations = vec!
+00004930: 5b28 4e6f 6465 3a3a 5661 7228 7661 7229  [(Node::Var(var)
+00004940: 2c20 4e6f 6e65 295d 3b0a 2020 2020 2020  , None)];.      
+00004950: 2020 7065 7467 7261 7068 3a3a 7669 7369    petgraph::visi
+00004960: 743a 3a64 6570 7468 5f66 6972 7374 5f73  t::depth_first_s
+00004970: 6561 7263 6828 2673 656c 662e 7065 7467  earch(&self.petg
+00004980: 7261 7068 2c20 5b73 656c 662e 7661 725f  raph, [self.var_
+00004990: 6772 6170 685f 6964 735b 7661 725d 5d2c  graph_ids[var]],
+000049a0: 207c 6576 656e 747c 207b 0a20 2020 2020   |event| {.     
+000049b0: 2020 2020 2020 2069 6620 6c65 7420 7065         if let pe
+000049c0: 7467 7261 7068 3a3a 7669 7369 743a 3a44  tgraph::visit::D
+000049d0: 6673 4576 656e 743a 3a54 7265 6545 6467  fsEvent::TreeEdg
+000049e0: 6528 7061 7265 6e74 2c20 6e6f 6465 2920  e(parent, node) 
+000049f0: 3d20 6576 656e 7420 7b0a 2020 2020 2020  = event {.      
+00004a00: 2020 2020 2020 2020 2020 7072 6f70 6167            propag
+00004a10: 6174 696f 6e73 2e70 7573 6828 2873 656c  ations.push((sel
+00004a20: 662e 7065 7467 7261 7068 5b6e 6f64 655d  f.petgraph[node]
+00004a30: 2c20 536f 6d65 2873 656c 662e 7065 7467  , Some(self.petg
+00004a40: 7261 7068 5b70 6172 656e 745d 2929 293b  raph[parent])));
+00004a50: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00004a60: 2020 2020 2020 2020 2020 2070 6574 6772             petgr
+00004a70: 6170 683a 3a76 6973 6974 3a3a 436f 6e74  aph::visit::Cont
+00004a80: 726f 6c3a 3a3c 2829 3e3a 3a43 6f6e 7469  rol::<()>::Conti
+00004a90: 6e75 650a 2020 2020 2020 2020 7d29 3b0a  nue.        });.
+00004aa0: 2020 2020 2020 2020 7072 6f70 6167 6174          propagat
+00004ab0: 696f 6e73 2e72 6576 6572 7365 2829 3b0a  ions.reverse();.
+00004ac0: 2020 2020 2020 2020 7072 6f70 6167 6174          propagat
+00004ad0: 696f 6e73 0a20 2020 207d 0a7d 0a0a 696d  ions.    }.}..im
+00004ae0: 706c 204e 6f64 6520 7b0a 2020 2020 7075  pl Node {.    pu
+00004af0: 6228 7375 7065 7229 2066 6e20 7661 7228  b(super) fn var(
+00004b00: 7365 6c66 2920 2d3e 204f 7074 696f 6e3c  self) -> Option<
+00004b10: 5661 7249 643e 207b 0a20 2020 2020 2020  VarId> {.       
+00004b20: 2069 6620 6c65 7420 4e6f 6465 3a3a 5661   if let Node::Va
+00004b30: 7228 6964 2920 3d20 7365 6c66 207b 0a20  r(id) = self {. 
+00004b40: 2020 2020 2020 2020 2020 2053 6f6d 6528             Some(
+00004b50: 6964 290a 2020 2020 2020 2020 7d20 656c  id).        } el
+00004b60: 7365 207b 0a20 2020 2020 2020 2020 2020  se {.           
+00004b70: 204e 6f6e 650a 2020 2020 2020 2020 7d0a   None.        }.
+00004b80: 2020 2020 7d0a 2020 2020 7075 6228 7375      }.    pub(su
+00004b90: 7065 7229 2066 6e20 6661 6374 6f72 2873  per) fn factor(s
+00004ba0: 656c 6629 202d 3e20 4f70 7469 6f6e 3c46  elf) -> Option<F
+00004bb0: 6163 746f 7249 643e 207b 0a20 2020 2020  actorId> {.     
+00004bc0: 2020 2069 6620 6c65 7420 4e6f 6465 3a3a     if let Node::
+00004bd0: 4661 6374 6f72 2869 6429 203d 2073 656c  Factor(id) = sel
+00004be0: 6620 7b0a 2020 2020 2020 2020 2020 2020  f {.            
+00004bf0: 536f 6d65 2869 6429 0a20 2020 2020 2020  Some(id).       
+00004c00: 207d 2065 6c73 6520 7b0a 2020 2020 2020   } else {.      
+00004c10: 2020 2020 2020 4e6f 6e65 0a20 2020 2020        None.     
+00004c20: 2020 207d 0a20 2020 207d 0a7d 0a            }.    }.}.
```

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/src/sasca/fg_build.rs` & `scalib-0.5.8/src/scalib_ext/scalib/src/sasca/fg_build.rs`

 * *Files 2% similar despite different names*

```diff
@@ -301,26 +301,33 @@
             .chain(vars_neg)
             .collect();
         Ok(match self {
             Self::Not(_) => fg::ExprFactor::NOT,
             Self::Lookup { table, .. } => fg::ExprFactor::LOOKUP {
                 table: ft(table.as_str())?,
             },
-            Self::Add(_) => fg::ExprFactor::ADD,
+            Self::Sum(_) => fg::ExprFactor::ADD { vars_neg },
             Self::Mul(_) => fg::ExprFactor::MUL,
             Self::Xor(_) => fg::ExprFactor::XOR,
             Self::And(_) | Self::Or(_) => fg::ExprFactor::AND { vars_neg },
         })
     }
     /// Returns operands with their negation.
     /// Maps Or to And using De Morgan law.
     fn vars_neg(&self) -> Vec<(&fg_parser::Var, bool)> {
         match self {
             Self::Not(var) | Self::Lookup { var, .. } => vec![(var, false)],
-            Self::Xor(v) | Self::Add(v) | Self::Mul(v) => v.iter().map(|v| (v, false)).collect(),
+            Self::Xor(v) | Self::Mul(v) => v.iter().map(|v| (v, false)).collect(),
+            Self::Sum(v) => v
+                .iter()
+                .map(|signed_var| match signed_var.sign {
+                    fg_parser::SumOperation::Add => (&signed_var.var, false),
+                    fg_parser::SumOperation::Subtract => (&signed_var.var, true),
+                })
+                .collect(),
             Self::And(v) => v.iter().map(|v| (&v.var, v.neg)).collect(),
             Self::Or(v) => v.iter().map(|v| (&v.var, !v.neg)).collect(),
         }
     }
     /// Should we negate the result due to De Morgan law use ?
     fn neg_res(&self) -> bool {
         match self {
```

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/src/sasca/fg_parser.rs` & `scalib-0.5.8/src/scalib_ext/scalib/src/sasca/fg_parser.rs`

 * *Files 21% similar despite different names*

```diff
@@ -14,22 +14,41 @@
 impl NVar {
     fn new(var: Var, neg: bool) -> Self {
         Self { var, neg }
     }
 }
 
 #[derive(Debug, Clone)]
+pub(super) enum SumOperation {
+    Add,
+    Subtract,
+}
+
+#[derive(Debug, Clone)]
+pub(super) struct SignedVar {
+    pub(super) var: Var,
+    pub(super) sign: SumOperation,
+}
+
+impl From<&(SumOperation, Var)> for SignedVar {
+    fn from(op_var: &(SumOperation, Var)) -> Self {
+        let (sign, var) = op_var.clone();
+        SignedVar { var, sign }
+    }
+}
+
+#[derive(Debug, Clone)]
 pub(super) enum Expr {
     Not(Var),
     Lookup { var: Var, table: String },
-    Add(Vec<Var>),
+    And(Vec<NVar>),
     Mul(Vec<Var>),
     Xor(Vec<Var>),
-    And(Vec<NVar>),
     Or(Vec<NVar>),
+    Sum(Vec<SignedVar>),
 }
 
 #[derive(Debug, Clone)]
 pub(super) enum Property {
     // Assign a variable to an expression.
     Assign { dest: Var, expr: Expr },
     // General factor as a table.
@@ -73,22 +92,45 @@
     let not_var = || op('!').ignore_then(var);
     let nvar = || {
         var.map(|v| NVar::new(v, false))
             .or(not_var().map(|v| NVar::new(v, true)))
     };
     let op_nexpr = |c, f| nvar().separated_by(op(c)).at_least(2).map(f);
     let op_expr = |c, f| var.separated_by(op(c)).at_least(2).map(f);
+
+    let first_sum_operand = op('-')
+        .to(SumOperation::Subtract)
+        .or(pad.to(SumOperation::Add))
+        .then(var);
+    let sum_operand = op('-')
+        .to(SumOperation::Subtract)
+        .or(op('+').to(SumOperation::Add))
+        .then(var);
+
+    let sum_expr = || {
+        first_sum_operand
+            .then(sum_operand.repeated())
+            .map(|(first, ops)| {
+                Expr::Sum(
+                    std::iter::once(&first)
+                        .chain(ops.iter())
+                        .map(Into::into)
+                        .collect::<Vec<SignedVar>>(),
+                )
+            })
+    };
+
     let expr = ident
         .then(var.delimited_by(op('['), op(']')))
         .map(|(table, var)| Expr::Lookup { table, var })
         .or(op_expr('^', Expr::Xor as fn(_) -> _))
         .or(op_nexpr('&', Expr::And as fn(_) -> _))
         .or(op_nexpr('|', Expr::Or as fn(_) -> _))
-        .or(op_expr('+', Expr::Add as fn(_) -> _))
         .or(op_expr('*', Expr::Mul as fn(_) -> _))
+        .or(sum_expr())
         .or(not_var().map(|v| Expr::Not(v)));
     let prop_assign = var
         .then_ignore(op('='))
         .then(expr)
         .map(|(dest, expr)| Property::Assign { dest, expr });
     let prop_factor = ident
         .then(nvar().separated_by(op(',')).delimited_by(op('('), op(')')))
```

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/src/sasca/mod.rs` & `scalib-0.5.8/src/scalib_ext/scalib/src/sasca/mod.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/src/snr.rs` & `scalib-0.5.8/src/scalib_ext/scalib/src/snr.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/src/ttest.rs` & `scalib-0.5.8/src/scalib_ext/scalib/src/ttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/src/utils.rs` & `scalib-0.5.8/src/scalib_ext/scalib/src/utils.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/tests/lda.rs` & `scalib-0.5.8/src/scalib_ext/scalib/tests/lda.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/tests/multivarcs.rs` & `scalib-0.5.8/src/scalib_ext/scalib/tests/multivarcs.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib/tests/ttest.rs` & `scalib-0.5.8/src/scalib_ext/scalib/tests/ttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib-py/Cargo.toml` & `scalib-0.5.8/src/scalib_ext/scalib-py/Cargo.toml`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib-py/src/belief_propagation.rs` & `scalib-0.5.8/src/scalib_ext/scalib-py/src/belief_propagation.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib-py/src/factor_graph.rs` & `scalib-0.5.8/src/scalib_ext/scalib-py/src/factor_graph.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib-py/src/information.rs` & `scalib-0.5.8/src/scalib_ext/scalib-py/src/information.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib-py/src/lda.rs` & `scalib-0.5.8/src/scalib_ext/scalib-py/src/lda.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib-py/src/lib.rs` & `scalib-0.5.8/src/scalib_ext/scalib-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib-py/src/ranking.rs` & `scalib-0.5.8/src/scalib_ext/scalib-py/src/ranking.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib-py/src/rlda.rs` & `scalib-0.5.8/src/scalib_ext/scalib-py/src/rlda.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib-py/src/snr.rs` & `scalib-0.5.8/src/scalib_ext/scalib-py/src/snr.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib-py/src/thread_pool.rs` & `scalib-0.5.8/src/scalib_ext/scalib-py/src/thread_pool.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/src/scalib_ext/scalib-py/src/ttest.rs` & `scalib-0.5.8/src/scalib_ext/scalib-py/src/ttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/tests/mttest_test.py` & `scalib-0.5.8/tests/mttest_test.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/tests/test_factorgraph.py` & `scalib-0.5.8/tests/test_factorgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1396,14 +1396,88 @@
     bp.bp_loopy(1, False, clear_beliefs=False)
 
     assert bp.get_belief_from_var("x", "s1") is not None
     assert bp.get_belief_from_var("a", "s1") is not None
     assert bp.get_belief_from_var("b", "s1") is not None
 
 
+def test_sub():
+    g = """
+    NC 256
+    PROPERTY s1: z = x - y
+    VAR MULTI x
+    VAR MULTI y
+    VAR MULTI z
+    """
+
+    nc = 256
+    n = 10
+    fg = FactorGraph(g)
+    bp = BPState(fg, n)
+    distri_x = make_distri(nc, n)
+    distri_y = make_distri(nc, n)
+    bp.set_evidence("x", distri_x)
+    bp.set_evidence("y", distri_y)
+    z_distri_ref = np.zeros(distri_x.shape)
+
+    for x in range(nc):
+        for y in range(nc):
+            z_distri_ref[:, (x - y) % nc] += distri_x[:, x] * distri_y[:, y]
+
+    z_distri_ref = (z_distri_ref.T / np.sum(z_distri_ref, axis=1)).T
+    bp.bp_loopy(1, True)
+    distri_z = bp.get_distribution("z")
+
+    assert np.allclose(z_distri_ref, distri_z)
+
+
+def test_sub_multi_ops():
+    g = """
+    NC 13
+    PROPERTY s1: z = -x + q - w + y
+    VAR MULTI x
+    VAR MULTI y
+    VAR MULTI z
+    VAR MULTI q
+    VAR MULTI w
+    """
+
+    nc = 13
+    n = 10
+    fg = FactorGraph(g)
+    bp = BPState(fg, n)
+    distri_x = make_distri(nc, n)
+    distri_y = make_distri(nc, n)
+    distri_q = make_distri(nc, n)
+    distri_w = make_distri(nc, n)
+
+    bp.set_evidence("x", distri_x)
+    bp.set_evidence("y", distri_y)
+    bp.set_evidence("w", distri_w)
+    bp.set_evidence("q", distri_q)
+    z_distri_ref = np.zeros(distri_x.shape)
+
+    for x in range(nc):
+        for y in range(nc):
+            for w in range(nc):
+                for q in range(nc):
+                    z_distri_ref[:, (-x + q - w + y) % nc] += (
+                        distri_x[:, x]
+                        * distri_y[:, y]
+                        * distri_w[:, w]
+                        * distri_q[:, q]
+                    )
+
+    z_distri_ref = (z_distri_ref.T / np.sum(z_distri_ref, axis=1)).T
+    bp.bp_acyclic("z")
+    distri_z = bp.get_distribution("z")
+
+    assert np.allclose(z_distri_ref, distri_z)
+
+
 def test_single_gf_sanity_check():
     from scalib.attacks.factor_graph import GenFactor
 
     nc = 13
     graph = f"""NC {nc}
     VAR MULTI a
     VAR MULTI b
```

### Comparing `scalib-0.5.7/tests/test_lda.py` & `scalib-0.5.8/tests/test_lda.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/tests/test_rlda.py` & `scalib-0.5.8/tests/test_rlda.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/tests/test_sascagraph.py` & `scalib-0.5.8/tests/test_sascagraph.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/tests/test_snr.py` & `scalib-0.5.8/tests/test_snr.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/tests/test_tools.py` & `scalib-0.5.8/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/tests/test_ttest.py` & `scalib-0.5.8/tests/test_ttest.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.7/tox.ini` & `scalib-0.5.8/tox.ini`

 * *Files identical despite different names*

