# Comparing `tmp/dust_extinction-1.4.tar.gz` & `tmp/dust_extinction-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dust_extinction-1.4.tar", last modified: Tue May  7 19:41:30 2024, max compression
+gzip compressed data, was "dust_extinction-1.4.1.tar", last modified: Tue May 21 12:50:35 2024, max compression
```

## Comparing `dust_extinction-1.4.tar` & `dust_extinction-1.4.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.328994 dust_extinction-1.4/
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.319994 dust_extinction-1.4/.github/
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.320994 dust_extinction-1.4/.github/workflows/
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     4803 2024-05-07 15:29:44.000000 dust_extinction-1.4/.github/workflows/tox-tests.yml
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      720 2022-01-04 15:34:07.000000 dust_extinction-1.4/.gitignore
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)      219 2023-11-28 13:31:44.000000 dust_extinction-1.4/.readthedocs.yml
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1356 2024-05-07 19:41:12.000000 dust_extinction-1.4/CHANGES.rst
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)      367 2023-04-19 09:36:19.000000 dust_extinction-1.4/CITATION.cff
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1517 2024-05-07 15:08:39.000000 dust_extinction-1.4/LICENSE
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      305 2022-01-04 15:34:07.000000 dust_extinction-1.4/MANIFEST.in
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     5695 2024-05-07 19:41:30.328994 dust_extinction-1.4/PKG-INFO
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     5144 2023-11-28 13:31:44.000000 dust_extinction-1.4/README.rst
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.321994 dust_extinction-1.4/docs/
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4581 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/Makefile
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.319994 dust_extinction-1.4/docs/_templates/
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.321994 dust_extinction-1.4/docs/_templates/autosummary/
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      250 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/_templates/autosummary/base.rst
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      251 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/_templates/autosummary/class.rst
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      252 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/_templates/autosummary/module.rst
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     7210 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/conf.py
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.322994 dust_extinction-1.4/docs/dust_extinction/
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)    11854 2024-05-07 19:37:16.000000 dust_extinction-1.4/docs/dust_extinction/choose_model.rst
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4220 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/dust_extinction/extinction.rst
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2521 2023-04-04 15:22:25.000000 dust_extinction-1.4/docs/dust_extinction/extinguish.rst
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4666 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/dust_extinction/fit_extinction.rst
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      774 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/dust_extinction/install.rst
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)    18458 2024-05-07 19:37:16.000000 dust_extinction-1.4/docs/dust_extinction/model_flavors.rst
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      330 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/dust_extinction/reference_api.rst
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     3436 2024-05-07 19:37:16.000000 dust_extinction-1.4/docs/dust_extinction/references.rst
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     6155 2024-01-18 14:25:03.000000 dust_extinction-1.4/docs/index.rst
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4549 2022-01-04 15:34:07.000000 dust_extinction-1.4/docs/make.bat
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.322994 dust_extinction-1.4/dust_extinction/
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)      174 2023-11-28 17:49:38.000000 dust_extinction-1.4/dust_extinction/__init__.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)    44332 2024-05-07 19:37:16.000000 dust_extinction-1.4/dust_extinction/averages.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     3954 2024-03-19 17:36:34.000000 dust_extinction-1.4/dust_extinction/baseclasses.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1961 2023-11-28 19:59:56.000000 dust_extinction-1.4/dust_extinction/conftest.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1149 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/conversions.py
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.327994 dust_extinction-1.4/dust_extinction/data/
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4924 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/CT06_pixiedust.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     8758 2022-03-30 13:46:42.000000 dust_extinction-1.4/dust_extinction/data/D22.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1513 2022-03-30 13:46:42.000000 dust_extinction-1.4/dust_extinction/data/D22_Rv_slope.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   145064 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/EXT_C11.RES.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    90880 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/EXT_DBP90.RES.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   121046 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/EXT_J13.RES.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     3193 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/F19_tabulated.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     2724 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/G21_IRS.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    16186 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/G21_IRS_fullres.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      550 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/G21_PHOT.dat
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2001 2024-05-07 19:37:16.000000 dust_extinction-1.4/dust_extinction/data/G24_SMCAvg.dat
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1874 2024-05-07 19:37:16.000000 dust_extinction-1.4/dust_extinction/data/G24_SMCBumps.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1868 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/GCC09_FUSE.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     7385 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/GCC09_IUE.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      181 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/GCC09_PHOT.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      246 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/README.rst
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)  3098880 2023-11-28 17:20:24.000000 dust_extinction-1.4/dust_extinction/data/astrodust+PAH_MW_RV3.1.fits
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      373 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/fritz11_galcenter.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110119 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_LMC2_10.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110125 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_LMCavg_20.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110428 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_3.1_60.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    64842 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_3.1_60_D03.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    64842 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_4.0A_40_D03.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110130 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_4.0B_40.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    64849 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_5.5A_30_D03.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110130 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_5.5B_30.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110116 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_SMCbar_0.dat
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    32453 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/data/zubko2004_bare-gr-s_alam_av.dat
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)    16750 2023-11-28 17:20:24.000000 dust_extinction-1.4/dust_extinction/grain_models.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2217 2023-11-28 19:59:56.000000 dust_extinction-1.4/dust_extinction/helpers.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)    44065 2024-03-19 17:36:34.000000 dust_extinction-1.4/dust_extinction/parameter_averages.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)    25744 2024-03-19 16:39:20.000000 dust_extinction-1.4/dust_extinction/shapes.py
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.328994 dust_extinction-1.4/dust_extinction/tests/
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      108 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/tests/__init__.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1592 2024-05-07 19:37:16.000000 dust_extinction-1.4/dust_extinction/tests/helpers.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2466 2023-04-04 14:41:44.000000 dust_extinction-1.4/dust_extinction/tests/test_axavtoexv.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     5520 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/tests/test_ccm89.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     5220 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/tests/test_corvals.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1225 2022-03-04 18:58:24.000000 dust_extinction-1.4/dust_extinction/tests/test_corvals_aves.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1222 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/tests/test_corvals_grainmods.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2309 2023-11-28 19:59:56.000000 dust_extinction-1.4/dust_extinction/tests/test_fm90.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     2095 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/tests/test_g16.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     2971 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/tests/test_gcc09.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     3699 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/tests/test_o94.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     3860 2023-04-04 14:41:44.000000 dust_extinction-1.4/dust_extinction/tests/test_p92.py
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1896 2022-01-04 15:34:07.000000 dust_extinction-1.4/dust_extinction/tests/test_vcg04.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2970 2024-03-19 17:36:34.000000 dust_extinction-1.4/dust_extinction/tests/test_warnings.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)      335 2024-05-07 19:41:30.000000 dust_extinction-1.4/dust_extinction/version.py
-drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-07 19:41:30.328994 dust_extinction-1.4/dust_extinction.egg-info/
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     5695 2024-05-07 19:41:30.000000 dust_extinction-1.4/dust_extinction.egg-info/PKG-INFO
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2860 2024-05-07 19:41:30.000000 dust_extinction-1.4/dust_extinction.egg-info/SOURCES.txt
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)        1 2024-05-07 19:41:30.000000 dust_extinction-1.4/dust_extinction.egg-info/dependency_links.txt
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)        1 2024-05-07 19:41:30.000000 dust_extinction-1.4/dust_extinction.egg-info/not-zip-safe
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)       80 2024-05-07 19:41:30.000000 dust_extinction-1.4/dust_extinction.egg-info/requires.txt
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)       16 2024-05-07 19:41:30.000000 dust_extinction-1.4/dust_extinction.egg-info/top_level.txt
--rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      134 2022-01-04 15:34:07.000000 dust_extinction-1.4/pyproject.toml
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1773 2024-05-07 19:41:30.329994 dust_extinction-1.4/setup.cfg
--rwxrwxr-x   0 kgordon   (1000) kgordon   (1000)     1964 2022-01-04 15:34:07.000000 dust_extinction-1.4/setup.py
--rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2306 2024-05-07 15:29:44.000000 dust_extinction-1.4/tox.ini
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-21 12:50:35.608777 dust_extinction-1.4.1/
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-21 12:50:35.587777 dust_extinction-1.4.1/.github/
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-21 12:50:35.589777 dust_extinction-1.4.1/.github/workflows/
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     4803 2024-05-07 15:29:44.000000 dust_extinction-1.4.1/.github/workflows/tox-tests.yml
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      720 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/.gitignore
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)      219 2023-11-28 13:31:44.000000 dust_extinction-1.4.1/.readthedocs.yml
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1477 2024-05-21 12:47:30.000000 dust_extinction-1.4.1/CHANGES.rst
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)      367 2023-04-19 09:36:19.000000 dust_extinction-1.4.1/CITATION.cff
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1517 2024-05-07 15:08:39.000000 dust_extinction-1.4.1/LICENSE
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      305 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/MANIFEST.in
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     5697 2024-05-21 12:50:35.608777 dust_extinction-1.4.1/PKG-INFO
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     5144 2023-11-28 13:31:44.000000 dust_extinction-1.4.1/README.rst
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-21 12:50:35.589777 dust_extinction-1.4.1/docs/
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4581 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/docs/Makefile
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-21 12:50:35.588777 dust_extinction-1.4.1/docs/_templates/
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-21 12:50:35.589777 dust_extinction-1.4.1/docs/_templates/autosummary/
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      250 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/docs/_templates/autosummary/base.rst
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      251 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/docs/_templates/autosummary/class.rst
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      252 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/docs/_templates/autosummary/module.rst
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     7210 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/docs/conf.py
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-21 12:50:35.590777 dust_extinction-1.4.1/docs/dust_extinction/
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)    11854 2024-05-07 19:37:16.000000 dust_extinction-1.4.1/docs/dust_extinction/choose_model.rst
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4220 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/docs/dust_extinction/extinction.rst
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2521 2023-04-04 15:22:25.000000 dust_extinction-1.4.1/docs/dust_extinction/extinguish.rst
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4666 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/docs/dust_extinction/fit_extinction.rst
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      774 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/docs/dust_extinction/install.rst
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)    18458 2024-05-07 19:37:16.000000 dust_extinction-1.4.1/docs/dust_extinction/model_flavors.rst
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      330 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/docs/dust_extinction/reference_api.rst
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     3436 2024-05-07 19:37:16.000000 dust_extinction-1.4.1/docs/dust_extinction/references.rst
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     6155 2024-01-18 14:25:03.000000 dust_extinction-1.4.1/docs/index.rst
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4549 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/docs/make.bat
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-21 12:50:35.601777 dust_extinction-1.4.1/dust_extinction/
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)      174 2023-11-28 17:49:38.000000 dust_extinction-1.4.1/dust_extinction/__init__.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)    44332 2024-05-21 12:44:13.000000 dust_extinction-1.4.1/dust_extinction/averages.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     3954 2024-03-19 17:36:34.000000 dust_extinction-1.4.1/dust_extinction/baseclasses.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1961 2023-11-28 19:59:56.000000 dust_extinction-1.4.1/dust_extinction/conftest.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1149 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/conversions.py
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-21 12:50:35.606777 dust_extinction-1.4.1/dust_extinction/data/
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     4924 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/CT06_pixiedust.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     8758 2022-03-30 13:46:42.000000 dust_extinction-1.4.1/dust_extinction/data/D22.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1513 2022-03-30 13:46:42.000000 dust_extinction-1.4.1/dust_extinction/data/D22_Rv_slope.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   145064 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/EXT_C11.RES.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    90880 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/EXT_DBP90.RES.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   121046 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/EXT_J13.RES.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     3193 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/F19_tabulated.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     2724 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/G21_IRS.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    16186 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/G21_IRS_fullres.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      550 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/G21_PHOT.dat
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2009 2024-05-21 12:44:13.000000 dust_extinction-1.4.1/dust_extinction/data/G24_SMCAvg.dat
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1877 2024-05-21 12:44:13.000000 dust_extinction-1.4.1/dust_extinction/data/G24_SMCBumps.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1868 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/GCC09_FUSE.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     7385 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/GCC09_IUE.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      181 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/GCC09_PHOT.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      246 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/README.rst
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)  3098880 2023-11-28 17:20:24.000000 dust_extinction-1.4.1/dust_extinction/data/astrodust+PAH_MW_RV3.1.fits
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      373 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/fritz11_galcenter.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110119 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_LMC2_10.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110125 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_LMCavg_20.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110428 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_MW_3.1_60.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    64842 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_MW_3.1_60_D03.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    64842 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_MW_4.0A_40_D03.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110130 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_MW_4.0B_40.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    64849 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_MW_5.5A_30_D03.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110130 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_MW_5.5B_30.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)   110116 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_SMCbar_0.dat
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)    32453 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/data/zubko2004_bare-gr-s_alam_av.dat
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)    16750 2023-11-28 17:20:24.000000 dust_extinction-1.4.1/dust_extinction/grain_models.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2217 2023-11-28 19:59:56.000000 dust_extinction-1.4.1/dust_extinction/helpers.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)    44065 2024-03-19 17:36:34.000000 dust_extinction-1.4.1/dust_extinction/parameter_averages.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)    25744 2024-03-19 16:39:20.000000 dust_extinction-1.4.1/dust_extinction/shapes.py
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-21 12:50:35.608777 dust_extinction-1.4.1/dust_extinction/tests/
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      108 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/tests/__init__.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1592 2024-05-07 19:37:16.000000 dust_extinction-1.4.1/dust_extinction/tests/helpers.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2466 2023-04-04 14:41:44.000000 dust_extinction-1.4.1/dust_extinction/tests/test_axavtoexv.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     5520 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/tests/test_ccm89.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     5220 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/tests/test_corvals.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1225 2022-03-04 18:58:24.000000 dust_extinction-1.4.1/dust_extinction/tests/test_corvals_aves.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1222 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/tests/test_corvals_grainmods.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2309 2023-11-28 19:59:56.000000 dust_extinction-1.4.1/dust_extinction/tests/test_fm90.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     2095 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/tests/test_g16.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     2971 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/tests/test_gcc09.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     3699 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/tests/test_o94.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     3860 2023-04-04 14:41:44.000000 dust_extinction-1.4.1/dust_extinction/tests/test_p92.py
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)     1896 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/dust_extinction/tests/test_vcg04.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2970 2024-03-19 17:36:34.000000 dust_extinction-1.4.1/dust_extinction/tests/test_warnings.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)      337 2024-05-21 12:50:35.000000 dust_extinction-1.4.1/dust_extinction/version.py
+drwxr-xr-x   0 kgordon   (1000) kgordon   (1000)        0 2024-05-21 12:50:35.608777 dust_extinction-1.4.1/dust_extinction.egg-info/
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     5697 2024-05-21 12:50:35.000000 dust_extinction-1.4.1/dust_extinction.egg-info/PKG-INFO
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2860 2024-05-21 12:50:35.000000 dust_extinction-1.4.1/dust_extinction.egg-info/SOURCES.txt
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)        1 2024-05-21 12:50:35.000000 dust_extinction-1.4.1/dust_extinction.egg-info/dependency_links.txt
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)        1 2024-05-21 12:50:35.000000 dust_extinction-1.4.1/dust_extinction.egg-info/not-zip-safe
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)       80 2024-05-21 12:50:35.000000 dust_extinction-1.4.1/dust_extinction.egg-info/requires.txt
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)       16 2024-05-21 12:50:35.000000 dust_extinction-1.4.1/dust_extinction.egg-info/top_level.txt
+-rw-rw-r--   0 kgordon   (1000) kgordon   (1000)      134 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/pyproject.toml
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     1773 2024-05-21 12:50:35.609777 dust_extinction-1.4.1/setup.cfg
+-rwxrwxr-x   0 kgordon   (1000) kgordon   (1000)     1964 2022-01-04 15:34:07.000000 dust_extinction-1.4.1/setup.py
+-rw-r--r--   0 kgordon   (1000) kgordon   (1000)     2306 2024-05-07 15:29:44.000000 dust_extinction-1.4.1/tox.ini
```

### Comparing `dust_extinction-1.4/.github/workflows/tox-tests.yml` & `dust_extinction-1.4.1/.github/workflows/tox-tests.yml`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/.gitignore` & `dust_extinction-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/CHANGES.rst` & `dust_extinction-1.4.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+1.5 (unreleased)
+================
+
+- no changes yet
+
+1.4.1 (2024-05-21)
+================
+
+- Minor updates to G24 models
+
 1.4 (2024-05-07)
 ================
 
 - Added G24 Average and Bumps average models
 
 1.3 (2023-11-28)
 ================
```

### Comparing `dust_extinction-1.4/LICENSE` & `dust_extinction-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/PKG-INFO` & `dust_extinction-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dust_extinction
-Version: 1.4
+Version: 1.4.1
 Summary: Interstellar Dust Extinction Models
 Home-page: http://dust-extinction.readthedocs.io/
 Author: Karl Gordon
 Author-email: kgordon@stsci.edu
 License: BSD 3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `dust_extinction-1.4/README.rst` & `dust_extinction-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/docs/Makefile` & `dust_extinction-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/docs/conf.py` & `dust_extinction-1.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/docs/dust_extinction/choose_model.rst` & `dust_extinction-1.4.1/docs/dust_extinction/choose_model.rst`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/docs/dust_extinction/extinction.rst` & `dust_extinction-1.4.1/docs/dust_extinction/extinction.rst`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/docs/dust_extinction/extinguish.rst` & `dust_extinction-1.4.1/docs/dust_extinction/extinguish.rst`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/docs/dust_extinction/fit_extinction.rst` & `dust_extinction-1.4.1/docs/dust_extinction/fit_extinction.rst`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/docs/dust_extinction/install.rst` & `dust_extinction-1.4.1/docs/dust_extinction/install.rst`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/docs/dust_extinction/model_flavors.rst` & `dust_extinction-1.4.1/docs/dust_extinction/model_flavors.rst`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/docs/dust_extinction/references.rst` & `dust_extinction-1.4.1/docs/dust_extinction/references.rst`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/docs/index.rst` & `dust_extinction-1.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/docs/make.bat` & `dust_extinction-1.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/averages.py` & `dust_extinction-1.4.1/dust_extinction/averages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1561,15 +1561,15 @@
 
         ax.legend(loc='best')
         plt.show()
     """
 
     x_range = [0.3, 10.0]
 
-    Rv = 3.06
+    Rv = 3.02
 
     def __init__(self, **kwargs):
 
         # get the tabulated information
         data_path = pkg_resources.resource_filename("dust_extinction", "data/")
 
         # D22 sigma clipped average of 13 diffuse sightlines
@@ -1608,20 +1608,20 @@
         ------
         ValueError
            Input x values outside of defined range
         """
         C1 = -5.07
         C2 = 2.30
         C3 = 0.12
-        C4 = 0.08
+        C4 = 0.07
         xo = 4.59
         gamma = 0.95
 
         optnir_axav_x = 1.0 / np.array([2.198, 1.65, 1.25, 0.55, 0.44, 0.37])
-        optnir_axav_y = [0.075, 0.137, 0.333, 1.021, 1.345, 1.507]
+        optnir_axav_y = [0.062, 0.125, 0.324, 1.021, 1.349, 1.514]
 
         # return A(x)/A(V)
         return _curve_F99_method(
             in_x,
             self.Rv,
             C1,
             C2,
@@ -1684,15 +1684,15 @@
 
         ax.legend(loc='best')
         plt.show()
     """
 
     x_range = [0.3, 10.0]
 
-    Rv = 2.59
+    Rv = 2.55
 
     def __init__(self, **kwargs):
 
         # get the tabulated information
         data_path = pkg_resources.resource_filename("dust_extinction", "data/")
 
         # D22 sigma clipped average of 13 diffuse sightlines
@@ -1728,23 +1728,23 @@
             A(x)/A(V) extinction curve [mag]
 
         Raises
         ------
         ValueError
            Input x values outside of defined range
         """
-        C1 = -2.87
+        C1 = -2.85
         C2 = 1.51
         C3 = 2.64
         C4 = 0.25
         xo = 4.73
-        gamma = 1.16
+        gamma = 1.15
 
         optnir_axav_x = 1.0 / np.array([2.198, 1.65, 1.25, 0.55, 0.44, 0.37])
-        optnir_axav_y = [0.068, 0.174, 0.302, 1.017, 1.394, 1.675]
+        optnir_axav_y = [0.055, 0.162, 0.293, 1.017, 1.400, 1.684]
 
         # return A(x)/A(V)
         return _curve_F99_method(
             in_x,
             self.Rv,
             C1,
             C2,
```

### Comparing `dust_extinction-1.4/dust_extinction/baseclasses.py` & `dust_extinction-1.4.1/dust_extinction/baseclasses.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/conftest.py` & `dust_extinction-1.4.1/dust_extinction/conftest.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/conversions.py` & `dust_extinction-1.4.1/dust_extinction/conversions.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/CT06_pixiedust.dat` & `dust_extinction-1.4.1/dust_extinction/data/CT06_pixiedust.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/D22.dat` & `dust_extinction-1.4.1/dust_extinction/data/D22.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/D22_Rv_slope.dat` & `dust_extinction-1.4.1/dust_extinction/data/D22_Rv_slope.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/EXT_C11.RES.dat` & `dust_extinction-1.4.1/dust_extinction/data/EXT_C11.RES.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/EXT_DBP90.RES.dat` & `dust_extinction-1.4.1/dust_extinction/data/EXT_DBP90.RES.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/EXT_J13.RES.dat` & `dust_extinction-1.4.1/dust_extinction/data/EXT_J13.RES.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/F19_tabulated.dat` & `dust_extinction-1.4.1/dust_extinction/data/F19_tabulated.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/G21_IRS.dat` & `dust_extinction-1.4.1/dust_extinction/data/G21_IRS.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/G21_IRS_fullres.dat` & `dust_extinction-1.4.1/dust_extinction/data/G21_IRS_fullres.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/G21_PHOT.dat` & `dust_extinction-1.4.1/dust_extinction/data/G21_PHOT.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/GCC09_FUSE.dat` & `dust_extinction-1.4.1/dust_extinction/data/GCC09_FUSE.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/GCC09_IUE.dat` & `dust_extinction-1.4.1/dust_extinction/data/GCC09_IUE.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/astrodust+PAH_MW_RV3.1.fits` & `dust_extinction-1.4.1/dust_extinction/data/astrodust+PAH_MW_RV3.1.fits`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_LMC2_10.dat` & `dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_LMC2_10.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_LMCavg_20.dat` & `dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_LMCavg_20.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_3.1_60.dat` & `dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_MW_3.1_60.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_3.1_60_D03.dat` & `dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_MW_3.1_60_D03.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_4.0A_40_D03.dat` & `dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_MW_4.0A_40_D03.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_4.0B_40.dat` & `dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_MW_4.0B_40.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_5.5A_30_D03.dat` & `dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_MW_5.5A_30_D03.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_MW_5.5B_30.dat` & `dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_MW_5.5B_30.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/kext_albedo_WD_SMCbar_0.dat` & `dust_extinction-1.4.1/dust_extinction/data/kext_albedo_WD_SMCbar_0.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/data/zubko2004_bare-gr-s_alam_av.dat` & `dust_extinction-1.4.1/dust_extinction/data/zubko2004_bare-gr-s_alam_av.dat`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/grain_models.py` & `dust_extinction-1.4.1/dust_extinction/grain_models.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/helpers.py` & `dust_extinction-1.4.1/dust_extinction/helpers.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/parameter_averages.py` & `dust_extinction-1.4.1/dust_extinction/parameter_averages.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/shapes.py` & `dust_extinction-1.4.1/dust_extinction/shapes.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/tests/helpers.py` & `dust_extinction-1.4.1/dust_extinction/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/tests/test_axavtoexv.py` & `dust_extinction-1.4.1/dust_extinction/tests/test_axavtoexv.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/tests/test_ccm89.py` & `dust_extinction-1.4.1/dust_extinction/tests/test_ccm89.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/tests/test_corvals.py` & `dust_extinction-1.4.1/dust_extinction/tests/test_corvals.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/tests/test_corvals_aves.py` & `dust_extinction-1.4.1/dust_extinction/tests/test_corvals_aves.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/tests/test_corvals_grainmods.py` & `dust_extinction-1.4.1/dust_extinction/tests/test_corvals_grainmods.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/tests/test_fm90.py` & `dust_extinction-1.4.1/dust_extinction/tests/test_fm90.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/tests/test_g16.py` & `dust_extinction-1.4.1/dust_extinction/tests/test_g16.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/tests/test_gcc09.py` & `dust_extinction-1.4.1/dust_extinction/tests/test_gcc09.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/tests/test_o94.py` & `dust_extinction-1.4.1/dust_extinction/tests/test_o94.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/tests/test_p92.py` & `dust_extinction-1.4.1/dust_extinction/tests/test_p92.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/tests/test_vcg04.py` & `dust_extinction-1.4.1/dust_extinction/tests/test_vcg04.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction/tests/test_warnings.py` & `dust_extinction-1.4.1/dust_extinction/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/dust_extinction.egg-info/PKG-INFO` & `dust_extinction-1.4.1/dust_extinction.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dust_extinction
-Version: 1.4
+Version: 1.4.1
 Summary: Interstellar Dust Extinction Models
 Home-page: http://dust-extinction.readthedocs.io/
 Author: Karl Gordon
 Author-email: kgordon@stsci.edu
 License: BSD 3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `dust_extinction-1.4/dust_extinction.egg-info/SOURCES.txt` & `dust_extinction-1.4.1/dust_extinction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/setup.cfg` & `dust_extinction-1.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/setup.py` & `dust_extinction-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `dust_extinction-1.4/tox.ini` & `dust_extinction-1.4.1/tox.ini`

 * *Files identical despite different names*

