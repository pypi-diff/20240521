# Comparing `tmp/pyisic-0.1.8.tar.gz` & `tmp/pyisic-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pyisic/pyisic/dist/tmpt2ykwvtu/pyisic-0.1.8.tar", last modified: Mon Feb 28 19:18:21 2022, max compression
+gzip compressed data, was "/home/runner/work/pyisic/pyisic/dist/tmp3vjgd3zg/pyisic-0.1.9.tar", last modified: Wed Mar 16 15:26:42 2022, max compression
```

## Comparing `pyisic-0.1.8.tar` & `pyisic-0.1.9.tar`

### file list

```diff
@@ -1,86 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-02-28 19:18:09.000000 pyisic-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-28 19:18:09.000000 pyisic-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-02-28 19:18:21.000000 pyisic-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2233 2022-02-28 19:18:09.000000 pyisic-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/cnae2/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/cnae2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   122830 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/cnae2/cnae2.py
--rw-r--r--   0 runner    (1001) docker     (121)    77237 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/cnae2/cnae2_to_isic4.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/gced2011/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/gced2011/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   296522 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/gced2011/gced2011.py
--rw-r--r--   0 runner    (1001) docker     (121)    67822 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/gced2011/gced2011_to_nace2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/isic3/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/isic3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    53835 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/isic3/isic3.py
--rw-r--r--   0 runner    (1001) docker     (121)    20784 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/isic3/isic3_to_isic31.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/isic31/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/isic31/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    55417 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/isic31/isic31.py
--rw-r--r--   0 runner    (1001) docker     (121)    48252 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/isic31/isic31_to_isic4.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/isic4/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/isic4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    82099 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/isic4/isic4.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/jsic13/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/jsic13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   165992 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/jsic13/jsic13.py
--rw-r--r--   0 runner    (1001) docker     (121)   122482 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/jsic13/jsic13_to_isic4.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/ksic10/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/ksic10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   202771 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/ksic10/ksic10.py
--rw-r--r--   0 runner    (1001) docker     (121)    69802 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/ksic10/ksic10_to_isic4.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/nace2/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/nace2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    97222 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/nace2/nace2.py
--rw-r--r--   0 runner    (1001) docker     (121)    63950 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/nace2/nace2_to_isic4.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/nacebel2003/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/nacebel2003/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   435549 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/nacebel2003/nacebel2003.py
--rw-r--r--   0 runner    (1001) docker     (121)   291106 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/nacebel2003/nacebel2003_to_nacebel2008.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/nacebel2008/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/nacebel2008/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   323873 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/nacebel2008/nacebel2008.py
--rw-r--r--   0 runner    (1001) docker     (121)    35081 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/nacebel2008/nacebel2008_to_nace2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/naf1/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/naf1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    97578 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/naf1/naf1.py
--rw-r--r--   0 runner    (1001) docker     (121)    86477 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/naf1/naf1_to_naf2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/naf2/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/naf2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   182804 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/naf2/naf2.py
--rw-r--r--   0 runner    (1001) docker     (121)   112249 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/naf2/naf2_to_nace2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/naics2017/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/naics2017/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    82273 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/naics2017/naics2017.py
--rw-r--r--   0 runner    (1001) docker     (121)   116052 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/naics2017/naics2017_to_isic4.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/skd2002/
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/skd2002/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    55706 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/skd2002/skd2002.py
--rw-r--r--   0 runner    (1001) docker     (121)    65245 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/skd2002/skd2002_to_nace2.py
--rw-r--r--   0 runner    (1001) docker     (121)    79311 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/skd2002/skd2002_to_skd2008.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/skd2008/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/skd2008/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   163093 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/skd2008/skd2008.py
--rw-r--r--   0 runner    (1001) docker     (121)    79311 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/skd2008/skd2008_to_skd2002.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/skis2010/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/skis2010/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6792 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/skis2010/skis2010.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic/_standards/tsic2552/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/tsic2552/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   152397 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/tsic2552/tsic2552.py
--rw-r--r--   0 runner    (1001) docker     (121)    94646 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/_standards/tsic2552/tsic2552_to_isic3.py
--rw-r--r--   0 runner    (1001) docker     (121)     6760 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyisic/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2271 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-28 19:18:21.000000 pyisic-0.1.8/pyisic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-02-28 19:18:09.000000 pyisic-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-28 19:18:21.000000 pyisic-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-02-28 19:18:09.000000 pyisic-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-03-16 15:26:26.000000 pyisic-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-03-16 15:26:26.000000 pyisic-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-03-16 15:26:42.000000 pyisic-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2233 2022-03-16 15:26:26.000000 pyisic-0.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/
+-rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/cnae2/
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/cnae2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   122830 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/cnae2/cnae2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    77237 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/cnae2/cnae2_to_isic4.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/gced2011/
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/gced2011/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   296522 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/gced2011/gced2011.py
+-rw-r--r--   0 runner    (1001) docker     (121)    67822 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/gced2011/gced2011_to_nace2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/isic3/
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/isic3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53835 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/isic3/isic3.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20784 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/isic3/isic3_to_isic31.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/isic31/
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/isic31/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    55417 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/isic31/isic31.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48252 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/isic31/isic31_to_isic4.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/isic4/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/isic4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    82099 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/isic4/isic4.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/jsic13/
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/jsic13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   165992 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/jsic13/jsic13.py
+-rw-r--r--   0 runner    (1001) docker     (121)   122482 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/jsic13/jsic13_to_isic4.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/ksic10/
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/ksic10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   202771 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/ksic10/ksic10.py
+-rw-r--r--   0 runner    (1001) docker     (121)    69802 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/ksic10/ksic10_to_isic4.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/nace1/
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/nace1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51163 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/nace1/nace1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    66706 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/nace1/nace1_to_nace2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/nace2/
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/nace2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    97222 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/nace2/nace2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    63950 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/nace2/nace2_to_isic4.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/nacebel2003/
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/nacebel2003/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   435549 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/nacebel2003/nacebel2003.py
+-rw-r--r--   0 runner    (1001) docker     (121)   291106 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/nacebel2003/nacebel2003_to_nacebel2008.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/nacebel2008/
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/nacebel2008/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   323873 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/nacebel2008/nacebel2008.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35081 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/nacebel2008/nacebel2008_to_nace2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/naf1/
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/naf1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    97578 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/naf1/naf1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    86477 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/naf1/naf1_to_naf2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/naf2/
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/naf2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   182804 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/naf2/naf2.py
+-rw-r--r--   0 runner    (1001) docker     (121)   112249 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/naf2/naf2_to_nace2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/naics2017/
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/naics2017/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    82273 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/naics2017/naics2017.py
+-rw-r--r--   0 runner    (1001) docker     (121)   116052 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/naics2017/naics2017_to_isic4.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/skd2002/
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/skd2002/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    55706 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/skd2002/skd2002.py
+-rw-r--r--   0 runner    (1001) docker     (121)    65245 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/skd2002/skd2002_to_nace2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    79311 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/skd2002/skd2002_to_skd2008.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/skd2008/
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/skd2008/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   163093 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/skd2008/skd2008.py
+-rw-r--r--   0 runner    (1001) docker     (121)    79311 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/skd2008/skd2008_to_skd2002.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/skis2010/
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/skis2010/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6792 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/skis2010/skis2010.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic/_standards/tsic2552/
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/tsic2552/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   152397 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/tsic2552/tsic2552.py
+-rw-r--r--   0 runner    (1001) docker     (121)    94646 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/_standards/tsic2552/tsic2552_to_isic3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6780 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyisic/types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-03-16 15:26:41.000000 pyisic-0.1.9/pyisic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2382 2022-03-16 15:26:42.000000 pyisic-0.1.9/pyisic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 15:26:41.000000 pyisic-0.1.9/pyisic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-03-16 15:26:41.000000 pyisic-0.1.9/pyisic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-16 15:26:41.000000 pyisic-0.1.9/pyisic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-03-16 15:26:26.000000 pyisic-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-16 15:26:42.000000 pyisic-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-03-16 15:26:26.000000 pyisic-0.1.9/setup.py
```

### Comparing `pyisic-0.1.8/LICENSE` & `pyisic-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/PKG-INFO` & `pyisic-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyisic
-Version: 0.1.8
+Version: 0.1.9
 Summary: Standard industrial classification standardization
 Home-page: https://github.com/sayari-analytics/pyisic
 Author: Jordan Vani
 Author-email: tech@sayari.com
 License: MIT
 Project-URL: Documentation, https://pyisic.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/sayari-analytics/pyisic/issues
```

### Comparing `pyisic-0.1.8/README.rst` & `pyisic-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/__init__.py` & `pyisic-0.1.9/pyisic/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from ._standards.cnae2 import CNAE2, CNAE2_to_ISIC4
 from ._standards.gced2011 import GCED2011, GCED2011_to_NACE2
 from ._standards.isic3 import ISIC3, ISIC3_to_ISIC31
 from ._standards.isic4 import ISIC4
 from ._standards.isic31 import ISIC31, ISIC31_to_ISIC4
 from ._standards.jsic13 import JSIC13, JSIC13_to_ISIC4
 from ._standards.ksic10 import KSIC10, KSIC10_to_ISIC4
+from ._standards.nace1 import NACE1, NACE1_to_NACE2
 from ._standards.nace2 import NACE2, NACE2_to_ISIC4
 from ._standards.nacebel2003 import NACEBEL2003, NACEBEL2003_to_NACEBEL2008
 from ._standards.nacebel2008 import NACEBEL2008, NACEBEL2008_to_NACE2
 from ._standards.naf1 import NAF1, NAF1_to_NAF2
 from ._standards.naf2 import NAF2, NAF2_to_NACE2
 from ._standards.naics2017 import NAICS2017, NAICS2017_to_ISIC4
 from ._standards.skd2002 import SKD2002, SKD2002_to_NACE2, SKD2002_to_SKD2008
@@ -32,9 +33,10 @@
         SKD2002_to_NACE2,
         CNAE2_to_ISIC4,
         NACEBEL2003_to_NACEBEL2008,
         NACEBEL2008_to_NACE2,
         NAF1_to_NAF2,
         NAF2_to_NACE2,
         GCED2011_to_NACE2,
+        NACE1_to_NACE2,
     ],
 )
```

### Comparing `pyisic-0.1.8/pyisic/_standards/cnae2/cnae2.py` & `pyisic-0.1.9/pyisic/_standards/cnae2/cnae2.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/cnae2/cnae2_to_isic4.py` & `pyisic-0.1.9/pyisic/_standards/cnae2/cnae2_to_isic4.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/gced2011/gced2011.py` & `pyisic-0.1.9/pyisic/_standards/gced2011/gced2011.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/gced2011/gced2011_to_nace2.py` & `pyisic-0.1.9/pyisic/_standards/gced2011/gced2011_to_nace2.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/isic3/isic3.py` & `pyisic-0.1.9/pyisic/_standards/isic3/isic3.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/isic3/isic3_to_isic31.py` & `pyisic-0.1.9/pyisic/_standards/isic3/isic3_to_isic31.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/isic31/isic31.py` & `pyisic-0.1.9/pyisic/_standards/isic31/isic31.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/isic31/isic31_to_isic4.py` & `pyisic-0.1.9/pyisic/_standards/isic31/isic31_to_isic4.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/isic4/isic4.py` & `pyisic-0.1.9/pyisic/_standards/isic4/isic4.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/jsic13/jsic13.py` & `pyisic-0.1.9/pyisic/_standards/jsic13/jsic13.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/jsic13/jsic13_to_isic4.py` & `pyisic-0.1.9/pyisic/_standards/jsic13/jsic13_to_isic4.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/ksic10/ksic10.py` & `pyisic-0.1.9/pyisic/_standards/ksic10/ksic10.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/ksic10/ksic10_to_isic4.py` & `pyisic-0.1.9/pyisic/_standards/ksic10/ksic10_to_isic4.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/nace2/nace2.py` & `pyisic-0.1.9/pyisic/_standards/nace2/nace2.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/nace2/nace2_to_isic4.py` & `pyisic-0.1.9/pyisic/_standards/nace2/nace2_to_isic4.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/nacebel2003/nacebel2003.py` & `pyisic-0.1.9/pyisic/_standards/nacebel2003/nacebel2003.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/nacebel2003/nacebel2003_to_nacebel2008.py` & `pyisic-0.1.9/pyisic/_standards/nacebel2003/nacebel2003_to_nacebel2008.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/nacebel2008/nacebel2008.py` & `pyisic-0.1.9/pyisic/_standards/nacebel2008/nacebel2008.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/nacebel2008/nacebel2008_to_nace2.py` & `pyisic-0.1.9/pyisic/_standards/nacebel2008/nacebel2008_to_nace2.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/naf1/naf1.py` & `pyisic-0.1.9/pyisic/_standards/naf1/naf1.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/naf1/naf1_to_naf2.py` & `pyisic-0.1.9/pyisic/_standards/naf1/naf1_to_naf2.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/naf2/naf2.py` & `pyisic-0.1.9/pyisic/_standards/naf2/naf2.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/naf2/naf2_to_nace2.py` & `pyisic-0.1.9/pyisic/_standards/naf2/naf2_to_nace2.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/naics2017/naics2017.py` & `pyisic-0.1.9/pyisic/_standards/naics2017/naics2017.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/naics2017/naics2017_to_isic4.py` & `pyisic-0.1.9/pyisic/_standards/naics2017/naics2017_to_isic4.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/skd2002/skd2002.py` & `pyisic-0.1.9/pyisic/_standards/skd2002/skd2002.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/skd2002/skd2002_to_nace2.py` & `pyisic-0.1.9/pyisic/_standards/skd2002/skd2002_to_nace2.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/skd2002/skd2002_to_skd2008.py` & `pyisic-0.1.9/pyisic/_standards/skd2002/skd2002_to_skd2008.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/skd2008/skd2008.py` & `pyisic-0.1.9/pyisic/_standards/skd2008/skd2008.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/skd2008/skd2008_to_skd2002.py` & `pyisic-0.1.9/pyisic/_standards/skd2008/skd2008_to_skd2002.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/skis2010/skis2010.py` & `pyisic-0.1.9/pyisic/_standards/skis2010/skis2010.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/tsic2552/tsic2552.py` & `pyisic-0.1.9/pyisic/_standards/tsic2552/tsic2552.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/_standards/tsic2552/tsic2552_to_isic3.py` & `pyisic-0.1.9/pyisic/_standards/tsic2552/tsic2552_to_isic3.py`

 * *Files identical despite different names*

### Comparing `pyisic-0.1.8/pyisic/types.py` & `pyisic-0.1.9/pyisic/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 class Standards(_Enum):  # pragma: no cover
     """Industry classification standards enum."""
 
     ISIC3 = "ISIC3"
     ISIC31 = "ISIC31"
     ISIC4 = "ISIC4"
+    NACE1 = "NACE1"
     NACE2 = "NACE2"
     NAICS2017 = "NAICS2017"
     TSIC2552 = "TSIC2552"
     JSIC13 = "JSIC13"
     KSIC10 = "KSIC10"
     SKD2002 = "SKD2002"
     SKD2008 = "SKD2008"
```

### Comparing `pyisic-0.1.8/pyisic.egg-info/PKG-INFO` & `pyisic-0.1.9/pyisic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyisic
-Version: 0.1.8
+Version: 0.1.9
 Summary: Standard industrial classification standardization
 Home-page: https://github.com/sayari-analytics/pyisic
 Author: Jordan Vani
 Author-email: tech@sayari.com
 License: MIT
 Project-URL: Documentation, https://pyisic.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/sayari-analytics/pyisic/issues
```

### Comparing `pyisic-0.1.8/pyisic.egg-info/SOURCES.txt` & `pyisic-0.1.9/pyisic.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 pyisic/_standards/isic4/isic4.py
 pyisic/_standards/jsic13/__init__.py
 pyisic/_standards/jsic13/jsic13.py
 pyisic/_standards/jsic13/jsic13_to_isic4.py
 pyisic/_standards/ksic10/__init__.py
 pyisic/_standards/ksic10/ksic10.py
 pyisic/_standards/ksic10/ksic10_to_isic4.py
+pyisic/_standards/nace1/__init__.py
+pyisic/_standards/nace1/nace1.py
+pyisic/_standards/nace1/nace1_to_nace2.py
 pyisic/_standards/nace2/__init__.py
 pyisic/_standards/nace2/nace2.py
 pyisic/_standards/nace2/nace2_to_isic4.py
 pyisic/_standards/nacebel2003/__init__.py
 pyisic/_standards/nacebel2003/nacebel2003.py
 pyisic/_standards/nacebel2003/nacebel2003_to_nacebel2008.py
 pyisic/_standards/nacebel2008/__init__.py
```

### Comparing `pyisic-0.1.8/setup.py` & `pyisic-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.rst", "r") as infile:
     long_description = infile.read()
 
 setuptools.setup(
     name="pyisic",
-    version="0.1.8",
+    version="0.1.9",
     author="Jordan Vani",
     author_email="tech@sayari.com",
     description="Standard industrial classification standardization",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/sayari-analytics/pyisic",
     project_urls={
```

