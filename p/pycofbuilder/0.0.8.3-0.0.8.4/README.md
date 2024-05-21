# Comparing `tmp/pycofbuilder-0.0.8.3.tar.gz` & `tmp/pycofbuilder-0.0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycofbuilder-0.0.8.3.tar", last modified: Tue Apr 16 17:58:19 2024, max compression
+gzip compressed data, was "pycofbuilder-0.0.8.4.tar", last modified: Tue May 21 14:53:13 2024, max compression
```

## Comparing `pycofbuilder-0.0.8.3.tar` & `pycofbuilder-0.0.8.4.tar`

### file list

```diff
@@ -1,167 +1,174 @@
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.497946 pycofbuilder-0.0.8.3/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1081 2023-10-06 15:52:45.000000 pycofbuilder-0.0.8.3/LICENSE
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      202 2024-03-05 14:34:09.000000 pycofbuilder-0.0.8.3/MANIFEST.in
--rw-r--r--   0 felipe    (1001) felipe    (1001)     8983 2024-04-16 17:58:19.497946 pycofbuilder-0.0.8.3/PKG-INFO
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     6345 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/README.md
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1009 2024-04-16 14:15:54.000000 pycofbuilder-0.0.8.3/pyproject.toml
--rw-rw-r--   0 felipe    (1001) felipe    (1001)       38 2024-04-16 17:58:19.497946 pycofbuilder-0.0.8.3/setup.cfg
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1445 2024-04-16 14:15:43.000000 pycofbuilder-0.0.8.3/setup.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.445945 pycofbuilder-0.0.8.3/src/
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.461946 pycofbuilder-0.0.8.3/src/pycofbuilder/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1043 2024-04-16 14:14:35.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/__init__.py
--rwxrwxr-x   0 felipe    (1001) felipe    (1001)    26448 2024-04-16 16:05:38.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/building_block.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)    15250 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/cjson.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.465946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/__init__.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.465946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/__pycache__/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      175 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     6651 2024-04-16 17:25:24.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/__pycache__/topology.cpython-311.pyc
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.469946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      627 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/BOH2.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      612 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/Br.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      859 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CH2CN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      720 2024-01-10 16:37:07.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CH3.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      999 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CHNNH2.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      867 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CHO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1465 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/COCHCHOH.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1116 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CONHNH2.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      873 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/COOH.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      613 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/Cl.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      608 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/NH2.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      741 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/NHOH.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      609 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/O.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      893 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/OH2.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/__init__.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.469946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.469946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3679 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/ADAM.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5816 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/SBFE.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)    14640 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/TDAT.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     9212 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/TKAT.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)    11916 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/TKDM.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     6483 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/TTPM.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/__init__.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.473946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/H6/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     8080 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/H6/HECO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     9885 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/H6/HEXB.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)    15793 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/H6/HPCO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/H6/__init__.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.477946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2906 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/2BPD.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2970 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/3BPD.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3746 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/3IDT.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3727 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/4IDT.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3608 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/ANTR.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2446 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BBTZ.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2708 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BDFN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2714 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BDTP.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1898 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BENZ.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3215 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BPNY.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4995 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BPYB.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2455 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BTPH.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3098 2024-04-16 13:59:02.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DFDB.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5259 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DFFE.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2965 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DHPI.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2967 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DHSI.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3645 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DPBY.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3495 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DPDA.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3730 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DPEL.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3395 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DPEY.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      620 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/HDZN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4689 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/IITT.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3715 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/INDE.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4498 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/INFL.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2630 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/INTO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2705 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/NAPT.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3457 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/NDTP.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4125 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PHEN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5243 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PTCD.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3860 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PYEN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3659 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PYRN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3400 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PYTO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4191 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TIDA.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     6343 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TIEN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4772 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TPDI.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4501 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TPNY.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1942 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TTPH.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/__init__.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.477946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/R4/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     7553 2024-04-16 14:05:34.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/R4/TPDT.cjson
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.477946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2684 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/CoBTC.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2684 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/CuBTC.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1428 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/NiBTC.gjf
--rw-rw-r--   0 felipe    (1001) felipe    (1001)    10913 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/PHPR.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5215 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/PORP.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     7719 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/PTCA.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2684 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/ZnBTC.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/__init__.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.485946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1892 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/BENZ.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1851 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/BRZN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     3087 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/BTTP.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4953 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/DBA1.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5680 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/DBA2.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5710 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/DICZ.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     8873 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/STAR.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     9549 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/STAR1.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     9612 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TBBZ.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1492 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TOTB.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4789 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPAM.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5790 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPBZ.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     4180 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPNY.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     6011 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPOB.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5689 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPTA.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5389 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPTZ.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1477 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TRZN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/__init__.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/__init__.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.493946 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      615 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/Br.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1030 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CF3.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      987 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CH3.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      878 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CHO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      878 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CHS.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      723 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CN.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      999 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/COOH.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      617 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/Cl.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2696 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/DMPE.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2008 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/EEPO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2145 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/EMEPO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1248 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/EPO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      610 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/F.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      614 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/H.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      609 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/I.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1630 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/MEPO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      844 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/NH2.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      735 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/NO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      886 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/NO2.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      609 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/O.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1391 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OCOCH3.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1762 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OEEPO.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1503 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OEt.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      728 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OH.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1129 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OMe.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1883 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OProp.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1881 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/Ph.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      726 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/SH.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1009 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/SO2H.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1143 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/SO3H.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/__init__.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2117 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/tBu.cjson
--rw-rw-r--   0 felipe    (1001) felipe    (1001)    66018 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/periodic_table.json
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     7993 2024-04-16 17:23:55.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/data/topology.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     1910 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/exceptions.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)   179874 2024-04-16 17:48:27.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/framework.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)    47784 2024-03-12 17:46:14.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/io_tools.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     2492 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/logger.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)    32273 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.3/src/pycofbuilder/tools.py
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.465946 pycofbuilder-0.0.8.3/src/pycofbuilder.egg-info/
--rw-r--r--   0 felipe    (1001) felipe    (1001)     8983 2024-04-16 17:58:19.000000 pycofbuilder-0.0.8.3/src/pycofbuilder.egg-info/PKG-INFO
--rw-rw-r--   0 felipe    (1001) felipe    (1001)     5959 2024-04-16 17:58:19.000000 pycofbuilder-0.0.8.3/src/pycofbuilder.egg-info/SOURCES.txt
--rw-rw-r--   0 felipe    (1001) felipe    (1001)        1 2024-04-16 17:58:19.000000 pycofbuilder-0.0.8.3/src/pycofbuilder.egg-info/dependency_links.txt
--rw-rw-r--   0 felipe    (1001) felipe    (1001)       95 2024-04-16 17:58:19.000000 pycofbuilder-0.0.8.3/src/pycofbuilder.egg-info/requires.txt
--rw-rw-r--   0 felipe    (1001) felipe    (1001)       13 2024-04-16 17:58:19.000000 pycofbuilder-0.0.8.3/src/pycofbuilder.egg-info/top_level.txt
-drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-04-16 17:58:19.497946 pycofbuilder-0.0.8.3/tests/
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      266 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.3/tests/test_advanced.py
--rw-rw-r--   0 felipe    (1001) felipe    (1001)      258 2023-10-06 15:52:45.000000 pycofbuilder-0.0.8.3/tests/test_basic.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-05-21 14:53:13.187567 pycofbuilder-0.0.8.4/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1081 2023-10-06 15:52:45.000000 pycofbuilder-0.0.8.4/LICENSE
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      202 2024-03-05 14:34:09.000000 pycofbuilder-0.0.8.4/MANIFEST.in
+-rw-r--r--   0 felipe    (1001) felipe    (1001)     9188 2024-05-21 14:53:13.187567 pycofbuilder-0.0.8.4/PKG-INFO
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     6550 2024-05-02 14:28:08.000000 pycofbuilder-0.0.8.4/README.md
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1009 2024-05-21 14:50:56.000000 pycofbuilder-0.0.8.4/pyproject.toml
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)       38 2024-05-21 14:53:13.187567 pycofbuilder-0.0.8.4/setup.cfg
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1445 2024-05-21 14:51:05.000000 pycofbuilder-0.0.8.4/setup.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-05-21 14:53:13.179566 pycofbuilder-0.0.8.4/src/
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-05-21 14:53:13.179566 pycofbuilder-0.0.8.4/src/pycofbuilder/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1043 2024-04-16 14:14:35.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/__init__.py
+-rwxrwxr-x   0 felipe    (1001) felipe    (1001)    26448 2024-04-16 16:05:38.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/building_block.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)    15250 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/cjson.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-05-21 14:53:13.183567 pycofbuilder-0.0.8.4/src/pycofbuilder/data/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/__init__.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-05-21 14:53:13.183567 pycofbuilder-0.0.8.4/src/pycofbuilder/data/__pycache__/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      175 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     6651 2024-04-16 17:25:24.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/__pycache__/topology.cpython-311.pyc
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-05-21 14:53:13.183567 pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      627 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/BOH2.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      612 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/Br.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      873 2024-05-02 14:28:14.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/CH2CN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      720 2024-01-10 16:37:07.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/CH3.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      999 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/CHNNH2.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      863 2024-05-02 14:28:14.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/CHO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1465 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/COCHCHOH.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1116 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/CONHNH2.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      873 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/COOH.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      613 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/Cl.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      608 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/NH2.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      741 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/NHOH.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      609 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/O.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      893 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/OH2.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/__init__.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-05-21 14:53:13.183567 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-05-21 14:53:13.183567 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/D4/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3679 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/D4/ADAM.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     6794 2024-05-02 14:50:29.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/D4/CUBA.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5816 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/D4/SBFE.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)    14640 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/D4/TDAT.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     9212 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/D4/TKAT.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)    11916 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/D4/TKDM.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     6483 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/D4/TTPM.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/D4/__init__.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-05-21 14:53:13.183567 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/H6/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     8080 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/H6/HECO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     9885 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/H6/HEXB.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)    15793 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/H6/HPCO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/H6/__init__.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-05-21 14:53:13.183567 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2906 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/2BPD.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2970 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/3BPD.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3746 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/3IDT.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3727 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/4IDT.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3608 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/ANTR.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2446 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/BBTZ.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2708 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/BDFN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2714 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/BDTP.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1898 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/BENZ.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3215 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/BPNY.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4995 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/BPYB.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2455 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/BTPH.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3098 2024-04-16 13:59:02.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/DFDB.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5259 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/DFFE.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2965 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/DHPI.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2967 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/DHSI.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3645 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/DPBY.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3495 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/DPDA.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3730 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/DPEL.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3395 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/DPEY.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      620 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/HDZN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4689 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/IITT.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3715 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/INDE.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4498 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/INFL.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2630 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/INTO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2700 2024-05-21 14:47:45.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/NAP2.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2705 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/NAPT.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3457 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/NDTP.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4125 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/PHEN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5243 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/PTCD.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3860 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/PYEN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3659 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/PYRN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3400 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/PYTO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4191 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/TIDA.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     6343 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/TIEN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4772 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/TPDI.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4501 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/TPNY.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1942 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/TTPH.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/__init__.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-05-21 14:53:13.183567 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/R4/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5227 2024-05-02 14:28:14.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/R4/ATTP.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)    11705 2024-05-21 14:34:06.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/R4/ETKB.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4424 2024-05-02 14:28:14.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/R4/PRLN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     7553 2024-04-16 14:05:34.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/R4/TPDT.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     9582 2024-05-02 14:28:14.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/R4/TPLN.cjson
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-05-21 14:53:13.187567 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/S4/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2684 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/S4/CoBTC.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2684 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/S4/CuBTC.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1428 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/S4/NiBTC.gjf
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     7698 2024-05-02 14:28:14.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/S4/OTPR.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)    10913 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/S4/PHPR.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5215 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/S4/PORP.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     7719 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/S4/PTCA.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     6171 2024-05-02 14:28:14.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/S4/TBPR.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2684 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/S4/ZnBTC.cjson
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-05-21 14:53:13.187567 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1892 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/BENZ.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1851 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/BRZN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     3087 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/BTTP.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4953 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/DBA1.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5680 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/DBA2.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5710 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/DICZ.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     8873 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/STAR.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     9549 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/STAR1.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     9612 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TBBZ.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1492 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TOTB.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4789 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TPAM.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5790 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TPBZ.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     4180 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TPNY.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     6011 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TPOB.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5689 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TPTA.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     5389 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TPTZ.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1477 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TRZN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/__init__.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/__init__.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-05-21 14:53:13.187567 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      615 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/Br.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1030 2024-03-11 22:50:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/CF3.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      987 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/CH3.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      878 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/CHO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      878 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/CHS.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      723 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/CN.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      999 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/COOH.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      617 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/Cl.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2696 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/DMPE.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2008 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/EEPO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2145 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/EMEPO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1248 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/EPO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      610 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/F.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      614 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/H.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      609 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/I.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1630 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/MEPO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      844 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/NH2.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      735 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/NO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      886 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/NO2.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      609 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/O.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1391 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/OCOCH3.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1762 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/OEEPO.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1503 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/OEt.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      728 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/OH.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1129 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/OMe.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1883 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/OProp.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1881 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/Ph.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      726 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/SH.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1009 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/SO2H.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1143 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/SO3H.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        0 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/__init__.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2117 2023-11-29 18:21:23.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/tBu.cjson
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)    66018 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/periodic_table.json
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     7993 2024-04-16 17:23:55.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/data/topology.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     1910 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/exceptions.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)   181968 2024-05-21 14:35:27.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/framework.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)    47784 2024-03-12 17:46:14.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/io_tools.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     2492 2024-03-05 12:59:30.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/logger.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)    32308 2024-05-06 16:48:47.000000 pycofbuilder-0.0.8.4/src/pycofbuilder/tools.py
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-05-21 14:53:13.179566 pycofbuilder-0.0.8.4/src/pycofbuilder.egg-info/
+-rw-r--r--   0 felipe    (1001) felipe    (1001)     9188 2024-05-21 14:53:13.000000 pycofbuilder-0.0.8.4/src/pycofbuilder.egg-info/PKG-INFO
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)     6245 2024-05-21 14:53:13.000000 pycofbuilder-0.0.8.4/src/pycofbuilder.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)        1 2024-05-21 14:53:13.000000 pycofbuilder-0.0.8.4/src/pycofbuilder.egg-info/dependency_links.txt
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)       95 2024-05-21 14:53:13.000000 pycofbuilder-0.0.8.4/src/pycofbuilder.egg-info/requires.txt
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)       13 2024-05-21 14:53:13.000000 pycofbuilder-0.0.8.4/src/pycofbuilder.egg-info/top_level.txt
+drwxrwxr-x   0 felipe    (1001) felipe    (1001)        0 2024-05-21 14:53:13.187567 pycofbuilder-0.0.8.4/tests/
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      266 2023-09-18 20:15:06.000000 pycofbuilder-0.0.8.4/tests/test_advanced.py
+-rw-rw-r--   0 felipe    (1001) felipe    (1001)      258 2023-10-06 15:52:45.000000 pycofbuilder-0.0.8.4/tests/test_basic.py
```

### Comparing `pycofbuilder-0.0.8.3/LICENSE` & `pycofbuilder-0.0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/PKG-INFO` & `pycofbuilder-0.0.8.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycofbuilder
-Version: 0.0.8.3
+Version: 0.0.8.4
 Summary: A package for Covalent Organic Frameworks sturcture creation based on the reticular approach.
 Home-page: https://github.com/lipelopesoliveira/pyCOFBuilder
 Author: Felipe Lopes Oliveira
 Author-email: Felipe Lopes <felipe.lopes@nano.ufrj.br>
 License: MIT License
         
         Copyright (c) 2023, Felipe Lopes de Oliveira
@@ -58,14 +58,15 @@
 
 
 [![image](https://img.shields.io/pypi/v/pycofbuilder.svg?style=flat-square&logoColor=green)](https://pypi.python.org/pypi/pycofbuilder/)
 [![Pyversions](https://img.shields.io/pypi/pyversions/pycofbuilder.svg?style=flat-square&label=Python%20Versions)](https://pypi.python.org/pypi/pycofbuilder)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/pycofbuilder?logo=pypi&style=flat-square&logoColor=white&color=blue&label=PyPI)](https://pypi.org/project/pycofbuilder)
 [![GitHub release](https://img.shields.io/github/release/lipelopesoliveira/pycofbuilder.svg?style=flat-square&logo=github)](https://GitHub.com/lipelopesoliveira/pycofbuilder/releases/)
 [![Paper](https://img.shields.io/badge/arXiv-2310.14822v2-red?logo=arxiv&logoColor=white&style=flat-square)](https://arxiv.org/abs/2310.14822)
+[![Paper](https://img.shields.io/badge/JCIM-10.1021/acs.jcim.3c01918-red?logo=acs&logoColor=white&style=flat-square)](https://doi.org/10.1021/acs.jcim.3c01918)
 [![GitHub license](https://img.shields.io/github/license/lipelopesoliveira/pycofbuilder.svg?style=flat-square)](https://github.com/lipelopesoliveira/pycofbuilder/blob/master/LICENSE)
 
 # What is pyCOFBuilder?
 
 **pyCOFBuilder** is a simple and powerful python package to automatically assembly COF structures with specifics building blocks, topologies, and functionalizations following the reticular approach to build and represent COF structures. The project was developed to address the need for generation of COFs structures in a high-throughput style, based on a nomenclature tha allows direct sctructural feature interpretation from a simple name. The package uses [pymatgen](https://pymatgen.org/) to create the structures.
 
 This package is still under development and, but it is already possible to create a large number of COFs structures.
@@ -211,9 +212,9 @@
 
 ## Citation
 
 If you find **pyCOFBuilder** useful in your research please consider citing the following paper:
 
 > F. L. Oliveira and P. M. Esteves,
 > _pyCOFBuilder: A python package for automated creation of Covalent Organic Framework models based on the reticular approach_
->
-> _arxiv.org/abs/2310.14822_ [DOI](https://doi.org/10.48550/arXiv.2310.14822)
+> J. Chem. Inf. Model. 2024, 64, 8, 3278–3289
+> _10.1021/acs.jcim.3c01918_ [DOI](https://doi.org/10.1021/acs.jcim.3c01918)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pycofbuilder-0.0.8.3/README.md` & `pycofbuilder-0.0.8.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 [![image](https://img.shields.io/pypi/v/pycofbuilder.svg?style=flat-square&logoColor=green)](https://pypi.python.org/pypi/pycofbuilder/)
 [![Pyversions](https://img.shields.io/pypi/pyversions/pycofbuilder.svg?style=flat-square&label=Python%20Versions)](https://pypi.python.org/pypi/pycofbuilder)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/pycofbuilder?logo=pypi&style=flat-square&logoColor=white&color=blue&label=PyPI)](https://pypi.org/project/pycofbuilder)
 [![GitHub release](https://img.shields.io/github/release/lipelopesoliveira/pycofbuilder.svg?style=flat-square&logo=github)](https://GitHub.com/lipelopesoliveira/pycofbuilder/releases/)
 [![Paper](https://img.shields.io/badge/arXiv-2310.14822v2-red?logo=arxiv&logoColor=white&style=flat-square)](https://arxiv.org/abs/2310.14822)
+[![Paper](https://img.shields.io/badge/JCIM-10.1021/acs.jcim.3c01918-red?logo=acs&logoColor=white&style=flat-square)](https://doi.org/10.1021/acs.jcim.3c01918)
 [![GitHub license](https://img.shields.io/github/license/lipelopesoliveira/pycofbuilder.svg?style=flat-square)](https://github.com/lipelopesoliveira/pycofbuilder/blob/master/LICENSE)
 
 # What is pyCOFBuilder?
 
 **pyCOFBuilder** is a simple and powerful python package to automatically assembly COF structures with specifics building blocks, topologies, and functionalizations following the reticular approach to build and represent COF structures. The project was developed to address the need for generation of COFs structures in a high-throughput style, based on a nomenclature tha allows direct sctructural feature interpretation from a simple name. The package uses [pymatgen](https://pymatgen.org/) to create the structures.
 
 This package is still under development and, but it is already possible to create a large number of COFs structures.
@@ -157,9 +158,9 @@
 
 ## Citation
 
 If you find **pyCOFBuilder** useful in your research please consider citing the following paper:
 
 > F. L. Oliveira and P. M. Esteves,
 > _pyCOFBuilder: A python package for automated creation of Covalent Organic Framework models based on the reticular approach_
->
-> _arxiv.org/abs/2310.14822_ [DOI](https://doi.org/10.48550/arXiv.2310.14822)
+> J. Chem. Inf. Model. 2024, 64, 8, 3278–3289
+> _10.1021/acs.jcim.3c01918_ [DOI](https://doi.org/10.1021/acs.jcim.3c01918)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pycofbuilder-0.0.8.3/pyproject.toml` & `pycofbuilder-0.0.8.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyproject.toml
 
 [project]
 name = "pycofbuilder"
-version = '0.0.8.3'
+version = '0.0.8.4'
 authors = [
   { name="Felipe Lopes", email="felipe.lopes@nano.ufrj.br" },
 ]
 description = 'A package for Covalent Organic Frameworks sturcture creation based on the reticular approach.'
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pycofbuilder-0.0.8.3/setup.py` & `pycofbuilder-0.0.8.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 with open('LICENSE') as f:
     license = f.read()
 
 
-VERSION = '0.0.8.3'
+VERSION = '0.0.8.4'
 DESCRIPTION = 'A package for Covalent Organic Frameworks sturcture assembly.'
 
 setup(
     name='pyCOFBuilder',
     version=VERSION,
     description=DESCRIPTION,
     long_description=open('README.md').read(),
```

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/__init__.py` & `pycofbuilder-0.0.8.4/src/pycofbuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/building_block.py` & `pycofbuilder-0.0.8.4/src/pycofbuilder/building_block.py`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/cjson.py` & `pycofbuilder-0.0.8.4/src/pycofbuilder/cjson.py`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/__pycache__/topology.cpython-311.pyc` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/__pycache__/topology.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/BOH2.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/BOH2.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/Br.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/Br.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CH2CN.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/CN.cjson`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7384375000000001%*

 * *Differences: {"'atoms'": "{'elements': {'type': {insert: [(0, 'R')], delete: [3, 0]}, 'number': {delete: [3]}}, "*

 * *            "'coords': {'3d': {insert: [(3, 0.43389), (6, 1.59042)], delete: [9, 7, 6, 4, 3]}}}",*

 * * "'formula'": "'R1C1N1'",*

 * * "'name'": "'cyano'",*

 * * "'properties'": "{'smiles': '[R]C#N', 'code': 'CN', 'xsmiles': '[*]C#N', 'xsmiles_label': "*

 * *                 "'|$R;;$|'}"}*

```diff
@@ -1,43 +1,38 @@
 {
     "atoms": {
         "coords": {
             "3d": [
                 0.0,
                 0.0,
                 0.0,
-                1.59802718,
-                1.24936702,
+                0.43389,
                 0.0,
-                2.16935957,
-                2.24348516,
                 0.0,
-                0.881,
+                1.59042,
                 0.0,
                 0.0
             ]
         },
         "elements": {
             "number": [
                 0.0,
                 6,
-                7,
-                0.0
+                7
             ],
             "type": [
-                "Q",
+                "R",
                 "C",
-                "N",
-                "X"
+                "N"
             ]
         }
     },
     "chemical json": 1,
-    "formula": "N1X1C1Q1",
-    "name": "nitrile",
+    "formula": "R1C1N1",
+    "name": "cyano",
     "properties": {
-        "code": "CHCN",
-        "smiles": "[Q]CC#N",
-        "xsmiles": "[*]CC#N",
-        "xsmiles_label": "|$Q;;;$|"
+        "code": "CN",
+        "smiles": "[R]C#N",
+        "xsmiles": "[*]C#N",
+        "xsmiles_label": "|$R;;$|"
     }
 }
```

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CH3.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/CH3.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CHNNH2.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/CHNNH2.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CHO.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/CHO.cjson`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7591228070175439%*

 * *Differences: {"'atoms'": "{'elements': {'type': {insert: [(0, 'R'), (2, 'O')], delete: [2, 0]}, 'number': "*

 * *            "{insert: [(2, 8)], delete: [2]}}, 'coords': {'3d': {insert: [(3, 0.45), (6, "*

 * *            '1.17508507), (7, -0.85756574), (8, 0.49511581), (9, 1.09769069), (10, 0.78115892), '*

 * *            '(11, -0.45100232)], delete: [10, 9, 7, 6, 3, 1, 0]}}}',*

 * * "'formula'": "'O1R1C1H1'",*

 * * "'name'": "'formyl'",*

 * * "'properties'": "{'smiles': '[R]C([H])=O', 'xsmiles_label': '|$R;;;$|'}"}*

```diff
@@ -1,43 +1,43 @@
 {
     "atoms": {
         "coords": {
             "3d": [
                 0.0,
                 0.0,
                 0.0,
-                0.95,
+                0.45,
                 0.0,
                 0.0,
-                1.67508507,
-                -0.99023162,
-                0.0,
-                1.59769069,
-                0.90200463,
-                0.0
+                1.17508507,
+                -0.85756574,
+                0.49511581,
+                1.09769069,
+                0.78115892,
+                -0.45100232
             ]
         },
         "elements": {
             "number": [
                 0.0,
                 6,
-                0.0,
+                8,
                 1
             ],
             "type": [
-                "Q",
+                "R",
                 "C",
-                "X",
+                "O",
                 "H"
             ]
         }
     },
     "chemical json": 1,
-    "formula": "H1X1C1Q1",
-    "name": "aldehyde",
+    "formula": "O1R1C1H1",
+    "name": "formyl",
     "properties": {
         "code": "CHO",
-        "smiles": "[Q]C([H])=O",
+        "smiles": "[R]C([H])=O",
         "xsmiles": "[*]C([H])=O",
-        "xsmiles_label": "|$Q;;;$|"
+        "xsmiles_label": "|$R;;;$|"
     }
 }
```

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/COCHCHOH.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/COCHCHOH.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/CONHNH2.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/CONHNH2.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/COOH.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/COOH.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/Cl.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/Cl.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/NH2.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/NH2.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/NHOH.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/NHOH.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/O.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/O.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/conector/OH2.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/conector/OH2.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/ADAM.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/D4/ADAM.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/SBFE.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/D4/SBFE.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/TDAT.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/D4/TDAT.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/TKAT.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/D4/TKAT.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/TKDM.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/D4/TKDM.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/D4/TTPM.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/D4/TTPM.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/H6/HECO.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/H6/HECO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/H6/HEXB.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/H6/HEXB.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/H6/HPCO.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/H6/HPCO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/2BPD.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/2BPD.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/3BPD.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/3BPD.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/3IDT.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/3IDT.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/4IDT.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/4IDT.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/ANTR.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/ANTR.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BBTZ.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/BBTZ.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BDFN.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/BDFN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BDTP.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/BDTP.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BENZ.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/BENZ.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BPNY.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/BPNY.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BPYB.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/BPYB.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/BTPH.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/BTPH.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DFDB.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/DFDB.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DFFE.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/DFFE.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DHPI.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/DHPI.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DHSI.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/DHSI.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DPBY.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/DPBY.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DPDA.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/DPDA.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DPEL.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/DPEL.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/DPEY.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/DPEY.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/HDZN.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/HDZN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/IITT.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/IITT.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/INDE.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/INDE.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/INFL.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/INFL.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/INTO.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/INTO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/NAPT.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/NAPT.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/NDTP.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/NDTP.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PHEN.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/PHEN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PTCD.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/PTCD.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PYEN.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/PYEN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PYRN.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/PYRN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/PYTO.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/PYTO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TIDA.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/TIDA.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TIEN.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/TIEN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TPDI.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/TPDI.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TPNY.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/TPNY.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/L2/TTPH.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/L2/TTPH.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/R4/TPDT.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/R4/TPDT.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/CoBTC.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/S4/CoBTC.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/CuBTC.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/S4/CuBTC.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/NiBTC.gjf` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/S4/NiBTC.gjf`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/PHPR.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/S4/PHPR.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/PORP.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/S4/PORP.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/PTCA.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/S4/PTCA.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/S4/ZnBTC.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/S4/ZnBTC.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/BENZ.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/BENZ.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/BRZN.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/BRZN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/BTTP.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/BTTP.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/DBA1.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/DBA1.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/DBA2.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/DBA2.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/DICZ.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/DICZ.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/STAR.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/STAR.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/STAR1.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/STAR1.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TBBZ.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TBBZ.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TOTB.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TOTB.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPAM.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TPAM.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPBZ.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TPBZ.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPNY.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TPNY.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPOB.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TPOB.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPTA.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TPTA.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TPTZ.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TPTZ.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/core/T3/TRZN.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/core/T3/TRZN.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/Br.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/Br.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CF3.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/CF3.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CH3.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/CH3.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CHO.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/SO3H.cjson`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7328571428571429%*

 * *Differences: {"'atoms'": "{'elements': {'type': {insert: [(1, 'S'), (4, 'O'), (5, 'O')], delete: [1]}, "*

 * *            "'number': {insert: [(1, 16), (4, 8), (5, 8)], delete: [1]}}, 'coords': {'3d': "*

 * *            '{insert: [(3, 0.86934), (6, 1.70340865), (7, 1.0059434), (8, -0.58078169), (9, '*

 * *            '2.62538031), (10, 0.7751445), (11, -0.44550371), (12, 1.18066449), (13, -1.09689608), '*

 * *            '(14, -0.68623953), (15, 1.18066449), (16, 0.04585282), (17, 1.29305964)], delete: '*

 * *            '[11, 10, 9, 8, 7, 6, 3 […]*

```diff
@@ -1,43 +1,53 @@
 {
     "atoms": {
         "coords": {
             "3d": [
                 0.0,
                 0.0,
                 0.0,
-                0.45,
+                0.86934,
                 0.0,
                 0.0,
-                1.17508507,
-                -0.85756574,
-                0.49511581,
-                1.09769069,
-                0.78115892,
-                -0.45100232
+                1.70340865,
+                1.0059434,
+                -0.58078169,
+                2.62538031,
+                0.7751445,
+                -0.44550371,
+                1.18066449,
+                -1.09689608,
+                -0.68623953,
+                1.18066449,
+                0.04585282,
+                1.29305964
             ]
         },
         "elements": {
             "number": [
                 0.0,
-                6,
+                16,
                 8,
-                1
+                1,
+                8,
+                8
             ],
             "type": [
                 "R",
-                "C",
+                "S",
+                "O",
+                "H",
                 "O",
-                "H"
+                "O"
             ]
         }
     },
     "chemical json": 1,
-    "formula": "O1R1C1H1",
-    "name": "formyl",
+    "formula": "O3R1S1H1",
+    "name": "sulfonic acid",
     "properties": {
-        "code": "CHO",
-        "smiles": "[R]C([H])=O",
-        "xsmiles": "[*]C([H])=O",
-        "xsmiles_label": "|$R;;;$|"
+        "code": "SO3H",
+        "smiles": "[R]S(=O)(O)=O",
+        "xsmiles": "[*]S(=O)(O)=O",
+        "xsmiles_label": "|$R;;;;$|"
     }
 }
```

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CHS.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/CHS.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/CN.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/NO.cjson`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'atoms'": "{'elements': {'type': {insert: [(2, 'O')], delete: [1]}, 'number': {insert: [(2, 8)], "*

 * *            "delete: [1]}}, 'coords': {'3d': {insert: [(3, 0.45389), (6, 1.02537385), (7, "*

 * *            '1.04253989)], delete: [6, 3, 0]}}}',*

 * * "'formula'": "'O1R1N1'",*

 * * "'name'": "'nitroso'",*

 * * "'properties'": "{'smiles': '[R]N=O', 'code': 'NO', 'xsmiles': '[*]N=O'}"}*

```diff
@@ -1,38 +1,38 @@
 {
     "atoms": {
         "coords": {
             "3d": [
                 0.0,
                 0.0,
                 0.0,
-                0.43389,
+                0.45389,
                 0.0,
                 0.0,
-                1.59042,
-                0.0,
+                1.02537385,
+                1.04253989,
                 0.0
             ]
         },
         "elements": {
             "number": [
                 0.0,
-                6,
-                7
+                7,
+                8
             ],
             "type": [
                 "R",
-                "C",
-                "N"
+                "N",
+                "O"
             ]
         }
     },
     "chemical json": 1,
-    "formula": "R1C1N1",
-    "name": "cyano",
+    "formula": "O1R1N1",
+    "name": "nitroso",
     "properties": {
-        "code": "CN",
-        "smiles": "[R]C#N",
-        "xsmiles": "[*]C#N",
+        "code": "NO",
+        "smiles": "[R]N=O",
+        "xsmiles": "[*]N=O",
         "xsmiles_label": "|$R;;$|"
     }
 }
```

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/COOH.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/COOH.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/Cl.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/Cl.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/DMPE.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/DMPE.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/EEPO.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/EEPO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/EMEPO.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/EMEPO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/EPO.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/EPO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/F.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/F.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/H.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/H.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/I.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/I.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/MEPO.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/MEPO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/NH2.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/NH2.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/NO.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/OH.cjson`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7375%*

 * *Differences: {"'atoms'": "{'elements': {'type': {insert: [(2, 'H')], delete: [1]}, 'number': {insert: [(2, 1)], "*

 * *            "delete: [1]}}, 'coords': {'3d': {insert: [(3, 0.43), (6, 0.93564026), (7, "*

 * *            '0.88708817)], delete: [7, 6, 3]}}}',*

 * * "'formula'": "'O1R1H1'",*

 * * "'name'": "'hydroxyl'",*

 * * "'properties'": "{'smiles': '[R]O', 'code': 'OH', 'xsmiles': '[*]O', 'xsmiles_label': '|$R;$|'}"}*

```diff
@@ -1,38 +1,38 @@
 {
     "atoms": {
         "coords": {
             "3d": [
                 0.0,
                 0.0,
                 0.0,
-                0.45389,
+                0.43,
                 0.0,
                 0.0,
-                1.02537385,
-                1.04253989,
+                0.93564026,
+                0.88708817,
                 0.0
             ]
         },
         "elements": {
             "number": [
                 0.0,
-                7,
-                8
+                8,
+                1
             ],
             "type": [
                 "R",
-                "N",
-                "O"
+                "O",
+                "H"
             ]
         }
     },
     "chemical json": 1,
-    "formula": "O1R1N1",
-    "name": "nitroso",
+    "formula": "O1R1H1",
+    "name": "hydroxyl",
     "properties": {
-        "code": "NO",
-        "smiles": "[R]N=O",
-        "xsmiles": "[*]N=O",
-        "xsmiles_label": "|$R;;$|"
+        "code": "OH",
+        "smiles": "[R]O",
+        "xsmiles": "[*]O",
+        "xsmiles_label": "|$R;$|"
     }
 }
```

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/NO2.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/NO2.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/O.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/O.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OCOCH3.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/OCOCH3.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OEEPO.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/OEEPO.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OEt.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/OEt.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OMe.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/OMe.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/OProp.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/OProp.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/Ph.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/Ph.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/SH.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/SH.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/SO2H.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/SO2H.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/func_groups/tBu.cjson` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/func_groups/tBu.cjson`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/periodic_table.json` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/periodic_table.json`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/data/topology.py` & `pycofbuilder-0.0.8.4/src/pycofbuilder/data/topology.py`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/exceptions.py` & `pycofbuilder-0.0.8.4/src/pycofbuilder/exceptions.py`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/framework.py` & `pycofbuilder-0.0.8.4/src/pycofbuilder/framework.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import os
 import copy
 import numpy as np
 
 # Import pymatgen
 from pymatgen.core import Lattice, Structure
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
+from pymatgen.transformations.advanced_transformations import CubicSupercellTransformation
 
 from scipy.spatial.transform import Rotation as R
 
 # Import pycofbuilder exceptions
 from pycofbuilder.exceptions import (BondLenghError,
                                      BBConnectivityError)
 
@@ -214,15 +215,17 @@
                                                                                   self.atom_pos[i][1],
                                                                                   self.atom_pos[i][2],
                                                                                   self.atom_labels[i])
 
         return fram_str
 
     def get_n_atoms(self) -> int:
-        ''' Returns the number of atoms in the unitary cell'''
+        """
+        Returns the number of atoms in the unitary cell
+        """
         return len(self.atom_types)
 
     def get_available_topologies(self, dimensionality: str = 'all', print_result: bool = True):
         """
         Get the available topologies implemented in the class.
 
         Parameters
@@ -277,18 +280,18 @@
 
         Returns
         -------
         tuple[str, str, str, str]
             A tuple with the building blocks names, the net and the stacking.
         """
 
-        string_error = 'FrameworkName must be in the format: BB1_BB2_Net_Stacking'
+        string_error = 'FrameworkName must be a string'
         assert isinstance(FrameworkName, str), string_error
 
-        name_error = 'FrameworkName must be in the format: BB1_BB2_Net_Stacking'
+        name_error = 'FrameworkName must be in the format: BB1-BB2-Net-Stacking'
         assert len(FrameworkName.split('-')) == 4, name_error
 
         bb1_name, bb2_name, Net, Stacking = FrameworkName.split('-')
 
         net_error = f'{Net} not in the available list: {self.available_topologies}'
         assert Net in self.available_topologies, net_error
 
@@ -384,15 +387,15 @@
 
     def save(self,
              fmt: str = 'cif',
              supercell: list = [1, 1, 1],
              save_dir=None,
              primitive=False,
              save_bonds=True) -> None:
-        '''
+        """
         Save the structure in a specif file format.
 
         Parameters
         ----------
         fmt : str, optional
             The file format to be saved
             Can be `json`, `cif`, `xyz`, `turbomole`, `vasp`, `xsf`, `pdb`, `pqr`, `qe`.
@@ -402,15 +405,15 @@
             Default: [1,1,1]
         save_dir : str, optional
             The path to save the structure. By default, the structure is saved in a
             `out` folder created in the current directory.
         primitive : bool, optional
             If True, the primitive cell is saved. Otherwise, the conventional cell is saved.
             Default: False
-        '''
+        """
 
         save_dict = {
             'cjson': save_chemjson,
             'cif': save_cif,
             'xyz': save_xyz,
             'turbomole': save_turbomole,
             'vasp': save_vasp,
@@ -432,22 +435,22 @@
                 self.cellMatrix,
                 self.atom_types,
                 self.atom_pos,
                 coords_are_cartesian=True,
                 site_properties={'source': self.atom_labels}
             )
 
-        final_structure = structure.make_supercell(supercell, in_place=False)
+        structure.make_supercell(supercell)
 
         if save_bonds:
-            bonds = get_bonds(final_structure, self.bond_threshold)
+            bonds = get_bonds(structure, self.bond_threshold)
         else:
             bonds = []
 
-        structure_dict = final_structure.as_dict()
+        structure_dict = structure.as_dict()
 
         cell = structure_dict['lattice']['matrix']
 
         atom_types = [site['species'][0]['element'] for site in structure_dict['sites']]
         atom_labels = [site['properties']['source'] for site in structure_dict['sites']]
         atom_pos = [site['xyz'] for site in structure_dict['sites']]
 
@@ -460,22 +463,67 @@
                        file_name=self.name,
                        cell=cell,
                        atom_types=atom_types,
                        atom_labels=atom_labels,
                        atom_pos=atom_pos,
                        bonds=bonds)
 
+    def make_cubic(self,
+                   min_length=10,
+                   force_diagonal=False,
+                   force_90_degrees=True,
+                   min_atoms=None,
+                   max_atoms=None,
+                   angle_tolerance=1e-3):
+        """
+        Transform the primitive structure into a supercell with alpha, beta, and
+        gamma equal to 90 degrees. The algorithm will iteratively increase the size
+        of the supercell until the largest inscribed cube's side length is at least 'min_length'
+        and the number of atoms in the supercell falls in the range ``min_atoms < n < max_atoms``.
+
+        Parameters
+        ----------
+        min_length : float, optional
+            Minimum length of the cubic cell (default is 10)
+        force_diagonal : bool, optional
+            If True, generate a transformation with a diagonal transformation matrix (default is False)
+        force_90_degrees : bool, optional
+            If True, force the angles to be 90 degrees (default is True)
+        min_atoms : int, optional
+            Minimum number of atoms in the supercell (default is None)
+        max_atoms : int, optional
+            Maximum number of atoms in the supercell (default is None)
+        angle_tolerance : float, optional
+            The angle tolerance for the transformation (default is 1e-3)
+        """
+
+        cubic_dict = CubicSupercellTransformation(
+            min_length=min_length,
+            force_90_degrees=force_90_degrees,
+            force_diagonal=force_diagonal,
+            min_atoms=min_atoms,
+            max_atoms=max_atoms,
+            angle_tolerance=angle_tolerance
+            ).apply_transformation(self.prim_structure).as_dict()
+
+        self.cellMatrix = np.array(cubic_dict['lattice']['matrix']).astype(float)
+        self.cellParameters = cell_to_cellpar(self.cellMatrix)
+
+        self.atom_types = [i['label'] for i in cubic_dict['sites']]
+        self.atom_pos = [i['xyz'] for i in cubic_dict['sites']]
+        self.atom_labels = [i['properties']['source'] for i in cubic_dict['sites']]
+
 # --------------- Net creation methods -------------------------- #
 
     def create_hcb_structure(self,
                              BB_T3_A,
                              BB_T3_B,
                              stacking: str = 'AA',
                              slab: float = 10.0,
-                             shift_vector: list = [1.0, 1.0, 0],
+                             shift_vector: list = (1.0, 1.0, 0),
                              tilt_angle: float = 5.0):
         """Creates a COF with HCB network.
 
         The HCB net is composed of two tripodal building blocks.
 
         Parameters
         ----------
@@ -1808,29 +1856,29 @@
         self.cellParameters = np.array([a, b, c, alpha, beta, gamma]).astype(float)
 
         # Create the structure
         self.atom_types = []
         self.atom_labels = []
         self.atom_pos = []
 
-        # Add the building blocks to the structure
+        # Add the S4 building blocks to the structure
         for vertice_data in topology_info['vertices']:
             self.atom_types += BB_S4.atom_types
             vertice_pos = np.array(vertice_data['position']) * np.array([a, b, c])
 
             R_Matrix = R.from_euler('z', -alpha_S4, degrees=False).as_matrix()
 
             rotated_pos = np.dot(BB_S4.atom_pos, R_Matrix) + vertice_pos
             self.atom_pos += rotated_pos.tolist()
 
             self.atom_labels += ['C1' if i == 'C' else i for i in BB_S4.atom_labels]
 
         L2_angle_list = [-alpha_S4, alpha_S4, -alpha_S4, alpha_S4]
 
-        # Add the building blocks to the structure
+        # Add the L2 building blocks to the structure
         for i, edge_data in enumerate(topology_info['edges']):
             self.atom_types += BB_L2.atom_types
             edge_pos = np.array(edge_data['position']) * np.array([a, b, c])
 
             R_Matrix = R.from_euler('z', L2_angle_list[i], degrees=False).as_matrix()
 
             rotated_pos = np.dot(BB_L2.atom_pos, R_Matrix) + edge_pos
@@ -3850,17 +3898,17 @@
 
         # Determine the angle that alings the X[1] to one of the vertices of the tetrahedron
         vertice_pos = unit_vector(np.array([1, 0, 1]))
         Q_vertice_pos = BB_D41.get_X_points()[1][1]
 
         rotated_list = [
              R.from_rotvec(
-                 angle * unit_vector(topology_info['vertices'][0]['align_v']), degrees=False
+                 a * unit_vector(topology_info['vertices'][0]['align_v']), degrees=False
                  ).apply(Q_vertice_pos)
-             for angle in np.linspace(0, 2*np.pi, 360)
+             for a in np.linspace(0, 2*np.pi, 360)
              ]
 
         # Calculate the angle between the vertice_pos and the elements of rotated_list
         angle_list = [angle(vertice_pos, i) for i in rotated_list]
 
         rot_angle = np.linspace(0, 360, 360)[np.argmax(angle_list)]
 
@@ -3881,17 +3929,17 @@
 
         # Determine the angle that alings the X[1] to one of the vertices of the tetrahedron
         vertice_pos = unit_vector(np.array([1, 0, 1]))
         Q_vertice_pos = BB_D42.get_X_points()[1][1]
 
         rotated_list = [
              R.from_rotvec(
-                 angle * unit_vector(topology_info['vertices'][0]['align_v']), degrees=False
+                 a * unit_vector(topology_info['vertices'][0]['align_v']), degrees=False
                  ).apply(Q_vertice_pos)
-             for angle in np.linspace(0, 2*np.pi, 360)
+             for a in np.linspace(0, 2*np.pi, 360)
              ]
 
         # Calculate the angle between the vertice_pos and the elements of rotated_list
         angle_list = [angle(vertice_pos, i) for i in rotated_list]
 
         rot_angle = np.linspace(0, 360, 360)[np.argmax(angle_list)]
 
@@ -4094,17 +4142,17 @@
 
         # Determine the angle that alings the X[1] to one of the vertices of the tetrahedron
         vertice_pos = unit_vector(np.array([1, 0, 1]))
         Q_vertice_pos = BB_D4.get_X_points()[1][1]
 
         rotated_list = [
              R.from_rotvec(
-                 angle * unit_vector(topology_info['vertices'][0]['align_v']), degrees=False
+                 a * unit_vector(topology_info['vertices'][0]['align_v']), degrees=False
                  ).apply(Q_vertice_pos)
-             for angle in np.linspace(0, 2*np.pi, 360)
+             for a in np.linspace(0, 2*np.pi, 360)
              ]
 
         # Calculate the angle between the vertice_pos and the elements of rotated_list
         angle_list = [angle(vertice_pos, i) for i in rotated_list]
 
         rot_angle = np.linspace(0, 360, 360)[np.argmax(angle_list)]
```

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/io_tools.py` & `pycofbuilder-0.0.8.4/src/pycofbuilder/io_tools.py`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/logger.py` & `pycofbuilder-0.0.8.4/src/pycofbuilder/logger.py`

 * *Files identical despite different names*

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder/tools.py` & `pycofbuilder-0.0.8.4/src/pycofbuilder/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 import os
 import simplejson
 import numpy as np
 from scipy.spatial import distance
 
 
 def elements_dict(property='atomic_mass'):
-    '''Returns a dictionary containing the elements symbol and its selected property.
+    """
+    Returns a dictionary containing the elements symbol and its selected property.
 
     Parameters
     ----------
     prop : string
         The desired property can be:
             - "full_name"
             - "atomic_number"
@@ -34,15 +35,15 @@
             - "covalent_radius"
             - "vdw_radius"
 
     Returns
     -------
     prop_dic : dictionary
         A dictionary containing the elements symbol and its respective property.
-    '''
+    """
 
     file_name = os.path.join(os.path.dirname(__file__), 'data', 'periodic_table.json')
 
     with open(file_name, 'r') as f:
         periodic_table = simplejson.load(f)
 
     prop_list = periodic_table['H'].keys()
@@ -94,28 +95,28 @@
         angle = np.arccos(dot_product)
     if unit == 'cos':
         angle = dot_product
     return angle
 
 
 def rotation_matrix_from_vectors(vec1, vec2):
-    '''
+    """
     Find the rotation matrix that aligns vec1 to vec2
 
     Parameters
     ----------
     vec1 : array
         (3,3) array
     vec2 : array
         (3,3) array
     Returns
     -------
     rotation_matrix : array
         A transform matrix (3x3) which when applied to vec1, aligns it with vec2.
-    '''
+    """
     a, b = (vec1 / np.linalg.norm(vec1)).reshape(3), (vec2 / np.linalg.norm(vec2)).reshape(3)
     v = np.cross(a, b)
     c = np.dot(a, b)
     s = np.linalg.norm(v)
     if s != 0:
         kmat = np.array([[0, -v[2], v[1]],
                          [v[2], 0, -v[0]],
@@ -459,15 +460,15 @@
                         [bx, by, bz],
                         [cx, cy, cz]])
 
     return CellBox
 
 
 def calculate_UnitCells(cell, cutoff):
-    '''
+    """
     Calculate the number of unit cell repetitions so that all supercell lengths are larger than
     twice the interaction potential cut-off radius.
 
     RASPA considers the perpendicular directions the directions perpendicular to the `ab`, `bc`,
     and `ca` planes. Thus, the directions depend on who the crystallographic vectors `a`, `b`,
     and `c` are and the length in the perpendicular directions would be the projections
     of the crystallographic vectors on the vectors `a x b`, `b x c`, and `c x a`.
@@ -477,15 +478,15 @@
     ----------
     cell_matrix : array
         (3,3) cell vectors or (6,1)
     Returns
     -------
     superCell
         (3,1) list containg the number of repiting units in `x`, `y`, `z` directions.
-    '''
+    """
 
     # Make sure that the cell is in the format of cell matrix
     if len(cell) == 6:
         cell_box = cellpar_to_cell(cell)
     if len(cell) == 3:
         cell_box = cell
 
@@ -566,45 +567,45 @@
         if np.array_equal(e_list[i], element):
             index = i
             break
     return index
 
 
 def change_X_atoms(atom_labels, atom_pos, bond_atom) -> tuple:
-    '''
+    """
     Changes the X atom for the desired bond_atom or remove it if bond_atom == 'R'.
 
     Parameters
     ----------
     atom_labels : list
         List containing the atom labels
     atom_pos : list
         List containing the atom position
     Returns
     ----------
     labels : list
         List containing the processed atom labels
     pos : list
         List containing the processed atom position
-    '''
+    """
     label, pos = [], []
 
     for i in range(len(atom_labels)):
         if atom_labels[i] == 'X' and bond_atom != 'R':
             label += [bond_atom]
             pos += [atom_pos[i]]
         if atom_labels[i] != 'X':
             label += [atom_labels[i]]
             pos += [atom_pos[i]]
 
     return label, pos
 
 
 def closest_atom(label_1: str, pos_1: list, labels: list, pos: list):
-    '''
+    """
     Find the closest atom to a given atom
 
     Parameters
     ----------
     label_1 : string
         String containing the label of the atom
     pos_1 : list
@@ -618,15 +619,15 @@
     ----------
     closest_label : string
         String containing the label of the closest atom
     closest_position : array
         Array containing the position of the closest atom
     euclidian_distance : float
         Euclidian distance between the two atoms
-    '''
+    """
 
     list_labels = []
     list_pos = []
 
     for i in range(len(labels)):
         if labels[i] != label_1:
             list_labels += [labels[i]]
@@ -641,15 +642,17 @@
     closest_position = list_pos[closest_index]
     euclidian_distance = np.linalg.norm(pos_1 - list_pos[closest_index])
 
     return closest_label, closest_position, euclidian_distance
 
 
 def closest_atom_struc(label_1, pos_1, labels, pos):
-    '''Finds the closest atom on the structure to a given atom'''
+    """
+    Finds the closest atom on the structure to a given atom
+    """
 
     list_labels = []
     list_pos = []
     for i in range(len(labels)):
         if labels[i] != label_1:
             if 'C' in labels[i]:
                 list_labels += [labels[i]]
@@ -661,17 +664,17 @@
     closet_position = list_pos[closest_index]
     euclidian_distance = np.linalg.norm(pos_1 - list_pos[closest_index])
 
     return closet_label, closet_position, euclidian_distance
 
 
 def get_bond_atom(connector_1: str, connector_2: str) -> str:
-    '''
+    """
     Get the atom that will be used to bond two building blocks.
-    '''
+    """
 
     bond_dict = {
         'NH2': 'N',
         'NHOH': 'N',
         'COCHCHOH': 'N',
         'CONHNH2': 'N',
         'CHNNH2': 'N',
@@ -689,26 +692,30 @@
         if group in [connector_1, connector_2]:
             bond_atom = bond_dict[group]
 
     return bond_atom
 
 
 def get_framework_symm_text(name, lattice, hall, space_group, space_number, symm_op):
-    '''Get the text for the framework symmop'''
+    """
+    Get the text for the framework symmop
+    """
     text = '{:<60s} {:^12s} {:<4s} {:^4s} #{:^5s}   {:^2} sym. op.'.format(name,
                                                                            lattice,
                                                                            hall.lstrip('-'),
                                                                            space_group,
                                                                            space_number,
                                                                            symm_op)
     return text
 
 
 def print_framework_name(name, lattice, hall, space_group, space_number, symm_op):
-    '''Print the results of the created structure'''
+    """
+    Print the results of the created structure
+    """
     print('{:<60s} {:^12s} {:<4s} {:^4s} #{:^5s}   {:^2} sym. op.'.format(name,
                                                                           lattice,
                                                                           hall.lstrip('-'),
                                                                           space_group,
                                                                           space_number,
                                                                           symm_op))
 
@@ -737,15 +744,15 @@
     for i in set(AtomLabels):
         formula += i + str(AtomLabels.count(i))
 
     return formula
 
 
 def smiles_to_xsmiles(smiles_string: str) -> str:
-    '''
+    """
     Converts a SMILES string to an extended SMILES string with labels
 
     Parameters
     ----------
     smiles_string : str
         SMILES string to be converted
 
@@ -753,15 +760,15 @@
     -------
     xsmiles : str
         Extended SMILES string with special labels
     xsmiles_label : str
         xsmiles labels for images with the special labels
     composition : str
         String containing the composition
-    '''
+    """
     SPECIAL_ATOMS = ['Q', 'R', 'X']
     REGULAR_ATOMS = ['C', 'N', 'H', 'O', 'S', 'B', 'F']
 
     xsmiles = ''
     labels = []
     atom_list = []
 
@@ -904,22 +911,22 @@
     else:
         raise NotImplementedError('ibrav = {0} is not implemented'.format(ibrav))
 
     return cell
 
 
 def equal_value(val1, val2, threshold=1e-3) -> bool:
-    '''
+    """
     Determine if two values are equal based on a given threshold.
-    '''
+    """
     return abs(val1 - val2) <= threshold
 
 
 def classify_unit_cell(cell, thr=1e-3) -> str:
-    '''
+    """
     Determine the bravais lattice based on the cell lattice.
     The cell lattice can be the cell parameters as (6,1) array or
     the cell vectors as (3x3) array.
 
     Bravais lattice can be cubic, tetragonal, orthorhombic, hexagonal,
     monoclinic, or triclinic.
 
@@ -930,15 +937,15 @@
     threshold: float
         Numeric threshold for the analysis. Default: 1e-3
 
     Returns
     -------
     cell_type : string
         Bravais lattice.
-    '''
+    """
 
     if len(cell) == 3:
         a, b, c, alpha, beta, gamma = cell_to_cellpar(cell)
 
     cell_type = None
 
     if equal_value(alpha, 90, thr) and equal_value(beta, 90, thr) and equal_value(gamma, 90, thr):
@@ -957,17 +964,17 @@
     else:
         cell_type = "triclinic"
 
     return cell_type
 
 
 def cell_to_ibrav(cell):
-    '''
+    """
     Return the ibrav number for a given cell.
-    '''
+    """
 
     if len(cell) == 3:
         a, b, c, alpha, beta, gamma = cell_to_cellpar(cell)
     else:
         a, b, c, alpha, beta, gamma = cell
 
     cell_type = classify_unit_cell(cell)
```

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder.egg-info/PKG-INFO` & `pycofbuilder-0.0.8.4/src/pycofbuilder.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycofbuilder
-Version: 0.0.8.3
+Version: 0.0.8.4
 Summary: A package for Covalent Organic Frameworks sturcture creation based on the reticular approach.
 Home-page: https://github.com/lipelopesoliveira/pyCOFBuilder
 Author: Felipe Lopes Oliveira
 Author-email: Felipe Lopes <felipe.lopes@nano.ufrj.br>
 License: MIT License
         
         Copyright (c) 2023, Felipe Lopes de Oliveira
@@ -58,14 +58,15 @@
 
 
 [![image](https://img.shields.io/pypi/v/pycofbuilder.svg?style=flat-square&logoColor=green)](https://pypi.python.org/pypi/pycofbuilder/)
 [![Pyversions](https://img.shields.io/pypi/pyversions/pycofbuilder.svg?style=flat-square&label=Python%20Versions)](https://pypi.python.org/pypi/pycofbuilder)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/pycofbuilder?logo=pypi&style=flat-square&logoColor=white&color=blue&label=PyPI)](https://pypi.org/project/pycofbuilder)
 [![GitHub release](https://img.shields.io/github/release/lipelopesoliveira/pycofbuilder.svg?style=flat-square&logo=github)](https://GitHub.com/lipelopesoliveira/pycofbuilder/releases/)
 [![Paper](https://img.shields.io/badge/arXiv-2310.14822v2-red?logo=arxiv&logoColor=white&style=flat-square)](https://arxiv.org/abs/2310.14822)
+[![Paper](https://img.shields.io/badge/JCIM-10.1021/acs.jcim.3c01918-red?logo=acs&logoColor=white&style=flat-square)](https://doi.org/10.1021/acs.jcim.3c01918)
 [![GitHub license](https://img.shields.io/github/license/lipelopesoliveira/pycofbuilder.svg?style=flat-square)](https://github.com/lipelopesoliveira/pycofbuilder/blob/master/LICENSE)
 
 # What is pyCOFBuilder?
 
 **pyCOFBuilder** is a simple and powerful python package to automatically assembly COF structures with specifics building blocks, topologies, and functionalizations following the reticular approach to build and represent COF structures. The project was developed to address the need for generation of COFs structures in a high-throughput style, based on a nomenclature tha allows direct sctructural feature interpretation from a simple name. The package uses [pymatgen](https://pymatgen.org/) to create the structures.
 
 This package is still under development and, but it is already possible to create a large number of COFs structures.
@@ -211,9 +212,9 @@
 
 ## Citation
 
 If you find **pyCOFBuilder** useful in your research please consider citing the following paper:
 
 > F. L. Oliveira and P. M. Esteves,
 > _pyCOFBuilder: A python package for automated creation of Covalent Organic Framework models based on the reticular approach_
->
-> _arxiv.org/abs/2310.14822_ [DOI](https://doi.org/10.48550/arXiv.2310.14822)
+> J. Chem. Inf. Model. 2024, 64, 8, 3278–3289
+> _10.1021/acs.jcim.3c01918_ [DOI](https://doi.org/10.1021/acs.jcim.3c01918)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pycofbuilder-0.0.8.3/src/pycofbuilder.egg-info/SOURCES.txt` & `pycofbuilder-0.0.8.4/src/pycofbuilder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 src/pycofbuilder/data/conector/NH2.cjson
 src/pycofbuilder/data/conector/NHOH.cjson
 src/pycofbuilder/data/conector/O.cjson
 src/pycofbuilder/data/conector/OH2.cjson
 src/pycofbuilder/data/conector/__init__.py
 src/pycofbuilder/data/core/__init__.py
 src/pycofbuilder/data/core/D4/ADAM.cjson
+src/pycofbuilder/data/core/D4/CUBA.cjson
 src/pycofbuilder/data/core/D4/SBFE.cjson
 src/pycofbuilder/data/core/D4/TDAT.cjson
 src/pycofbuilder/data/core/D4/TKAT.cjson
 src/pycofbuilder/data/core/D4/TKDM.cjson
 src/pycofbuilder/data/core/D4/TTPM.cjson
 src/pycofbuilder/data/core/D4/__init__.py
 src/pycofbuilder/data/core/H6/HECO.cjson
@@ -69,36 +70,42 @@
 src/pycofbuilder/data/core/L2/DPEL.cjson
 src/pycofbuilder/data/core/L2/DPEY.cjson
 src/pycofbuilder/data/core/L2/HDZN.cjson
 src/pycofbuilder/data/core/L2/IITT.cjson
 src/pycofbuilder/data/core/L2/INDE.cjson
 src/pycofbuilder/data/core/L2/INFL.cjson
 src/pycofbuilder/data/core/L2/INTO.cjson
+src/pycofbuilder/data/core/L2/NAP2.cjson
 src/pycofbuilder/data/core/L2/NAPT.cjson
 src/pycofbuilder/data/core/L2/NDTP.cjson
 src/pycofbuilder/data/core/L2/PHEN.cjson
 src/pycofbuilder/data/core/L2/PTCD.cjson
 src/pycofbuilder/data/core/L2/PYEN.cjson
 src/pycofbuilder/data/core/L2/PYRN.cjson
 src/pycofbuilder/data/core/L2/PYTO.cjson
 src/pycofbuilder/data/core/L2/TIDA.cjson
 src/pycofbuilder/data/core/L2/TIEN.cjson
 src/pycofbuilder/data/core/L2/TPDI.cjson
 src/pycofbuilder/data/core/L2/TPNY.cjson
 src/pycofbuilder/data/core/L2/TTPH.cjson
 src/pycofbuilder/data/core/L2/__init__.py
+src/pycofbuilder/data/core/R4/ATTP.cjson
+src/pycofbuilder/data/core/R4/ETKB.cjson
+src/pycofbuilder/data/core/R4/PRLN.cjson
 src/pycofbuilder/data/core/R4/TPDT.cjson
+src/pycofbuilder/data/core/R4/TPLN.cjson
 src/pycofbuilder/data/core/S4/CoBTC.cjson
 src/pycofbuilder/data/core/S4/CuBTC.cjson
 src/pycofbuilder/data/core/S4/NiBTC.gjf
+src/pycofbuilder/data/core/S4/OTPR.cjson
 src/pycofbuilder/data/core/S4/PHPR.cjson
 src/pycofbuilder/data/core/S4/PORP.cjson
 src/pycofbuilder/data/core/S4/PTCA.cjson
+src/pycofbuilder/data/core/S4/TBPR.cjson
 src/pycofbuilder/data/core/S4/ZnBTC.cjson
-src/pycofbuilder/data/core/S4/__init__.py
 src/pycofbuilder/data/core/T3/BENZ.cjson
 src/pycofbuilder/data/core/T3/BRZN.cjson
 src/pycofbuilder/data/core/T3/BTTP.cjson
 src/pycofbuilder/data/core/T3/DBA1.cjson
 src/pycofbuilder/data/core/T3/DBA2.cjson
 src/pycofbuilder/data/core/T3/DICZ.cjson
 src/pycofbuilder/data/core/T3/STAR.cjson
```

