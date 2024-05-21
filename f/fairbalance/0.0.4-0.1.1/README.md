# Comparing `tmp/fairbalance-0.0.4.tar.gz` & `tmp/fairbalance-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairbalance-0.0.4.tar", last modified: Tue May 21 07:26:34 2024, max compression
+gzip compressed data, was "fairbalance-0.1.1.tar", last modified: Tue May 21 13:51:30 2024, max compression
```

## Comparing `fairbalance-0.0.4.tar` & `fairbalance-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.768938 fairbalance-0.0.4/
--rw-rw-rw-   0        0        0      285 2024-05-17 10:03:47.000000 fairbalance-0.0.4/.gitignore
--rw-rw-rw-   0        0        0      602 2024-05-21 07:26:34.759725 fairbalance-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       92 2024-05-17 12:00:14.000000 fairbalance-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.444362 fairbalance-0.0.4/fairbalance/
--rw-rw-rw-   0        0        0       54 2024-05-15 13:38:01.000000 fairbalance-0.0.4/fairbalance/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.535697 fairbalance-0.0.4/fairbalance/datasets/
--rw-rw-rw-   0        0        0      308 2024-05-16 13:58:22.000000 fairbalance-0.0.4/fairbalance/datasets/__init__.py
--rw-rw-rw-   0        0        0    11236 2024-05-17 08:03:24.000000 fairbalance-0.0.4/fairbalance/datasets/_datasets_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.556830 fairbalance-0.0.4/fairbalance/datasets/tests/
--rw-rw-rw-   0        0        0        0 2024-05-16 13:59:33.000000 fairbalance-0.0.4/fairbalance/datasets/tests/test_datasets_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.594830 fairbalance-0.0.4/fairbalance/metrics/
--rw-rw-rw-   0        0        0      263 2024-05-15 13:29:26.000000 fairbalance-0.0.4/fairbalance/metrics/__init__.py
--rw-rw-rw-   0        0        0     7673 2024-05-15 09:52:05.000000 fairbalance-0.0.4/fairbalance/metrics/_dataset_metrics.py
--rw-rw-rw-   0        0        0     2849 2024-05-15 09:30:16.000000 fairbalance-0.0.4/fairbalance/metrics/_model_metrics.py
-drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.628465 fairbalance-0.0.4/fairbalance/metrics/tests/
--rw-rw-rw-   0        0        0        0 2024-05-15 13:38:19.000000 fairbalance-0.0.4/fairbalance/metrics/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:38:46.000000 fairbalance-0.0.4/fairbalance/metrics/tests/test_dataset_metrics.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:38:54.000000 fairbalance-0.0.4/fairbalance/metrics/tests/test_model_metrics.py
-drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.697057 fairbalance-0.0.4/fairbalance/tools/
--rw-rw-rw-   0        0        0      305 2024-05-15 13:32:38.000000 fairbalance-0.0.4/fairbalance/tools/__init__.py
--rw-rw-rw-   0        0        0    10474 2024-05-17 08:27:03.000000 fairbalance-0.0.4/fairbalance/tools/_fairness_analysis.py
--rw-rw-rw-   0        0        0    21172 2024-05-17 09:17:53.000000 fairbalance-0.0.4/fairbalance/tools/_mitigator.py
--rw-rw-rw-   0        0        0     5271 2024-05-17 14:01:21.000000 fairbalance-0.0.4/fairbalance/tools/_processor.py
--rw-rw-rw-   0        0        0     2115 2024-05-17 08:30:33.000000 fairbalance-0.0.4/fairbalance/tools/_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.748744 fairbalance-0.0.4/fairbalance/tools/tests/
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:11.000000 fairbalance-0.0.4/fairbalance/tools/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:25.000000 fairbalance-0.0.4/fairbalance/tools/tests/test_fairness_analysis.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:32.000000 fairbalance-0.0.4/fairbalance/tools/tests/test_mitigator.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:44.000000 fairbalance-0.0.4/fairbalance/tools/tests/test_processor.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:56.000000 fairbalance-0.0.4/fairbalance/tools/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 07:26:34.511926 fairbalance-0.0.4/fairbalance.egg-info/
--rw-rw-rw-   0        0        0      602 2024-05-21 07:26:30.000000 fairbalance-0.0.4/fairbalance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      985 2024-05-21 07:26:33.000000 fairbalance-0.0.4/fairbalance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 07:26:31.000000 fairbalance-0.0.4/fairbalance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-05-21 07:26:31.000000 fairbalance-0.0.4/fairbalance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-21 07:26:31.000000 fairbalance-0.0.4/fairbalance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2024-05-17 11:08:16.000000 fairbalance-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 07:26:34.776901 fairbalance-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      765 2024-05-21 07:26:22.000000 fairbalance-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:30.067652 fairbalance-0.1.1/
+-rw-rw-rw-   0        0        0      285 2024-05-21 09:43:17.000000 fairbalance-0.1.1/.gitignore
+-rw-rw-rw-   0        0        0      602 2024-05-21 13:51:30.050928 fairbalance-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2024-05-17 12:00:14.000000 fairbalance-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:29.471280 fairbalance-0.1.1/fairbalance/
+-rw-rw-rw-   0        0        0       54 2024-05-15 13:38:01.000000 fairbalance-0.1.1/fairbalance/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:29.575116 fairbalance-0.1.1/fairbalance/datasets/
+-rw-rw-rw-   0        0        0      308 2024-05-16 13:58:22.000000 fairbalance-0.1.1/fairbalance/datasets/__init__.py
+-rw-rw-rw-   0        0        0    11236 2024-05-17 08:03:24.000000 fairbalance-0.1.1/fairbalance/datasets/_datasets_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:29.589763 fairbalance-0.1.1/fairbalance/datasets/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-16 13:59:33.000000 fairbalance-0.1.1/fairbalance/datasets/tests/test_datasets_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:29.655663 fairbalance-0.1.1/fairbalance/metrics/
+-rw-rw-rw-   0        0        0      263 2024-05-15 13:29:26.000000 fairbalance-0.1.1/fairbalance/metrics/__init__.py
+-rw-rw-rw-   0        0        0     7673 2024-05-15 09:52:05.000000 fairbalance-0.1.1/fairbalance/metrics/_dataset_metrics.py
+-rw-rw-rw-   0        0        0    10471 2024-05-21 13:49:32.000000 fairbalance-0.1.1/fairbalance/metrics/_fairness_analysis.py
+-rw-rw-rw-   0        0        0     2849 2024-05-15 09:30:16.000000 fairbalance-0.1.1/fairbalance/metrics/_model_metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:29.709837 fairbalance-0.1.1/fairbalance/metrics/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:38:19.000000 fairbalance-0.1.1/fairbalance/metrics/tests/__init__.py
+-rw-rw-rw-   0        0        0      652 2024-05-21 09:26:17.000000 fairbalance-0.1.1/fairbalance/metrics/tests/test_dataset_metrics.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:38:54.000000 fairbalance-0.1.1/fairbalance/metrics/tests/test_model_metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:29.754673 fairbalance-0.1.1/fairbalance/mitigation_strategies/
+-rw-rw-rw-   0        0        0      324 2024-05-21 13:42:52.000000 fairbalance-0.1.1/fairbalance/mitigation_strategies/__init__.py
+-rw-rw-rw-   0        0        0     4834 2024-05-21 13:45:35.000000 fairbalance-0.1.1/fairbalance/mitigation_strategies/_mitigation_strategies.py
+-rw-rw-rw-   0        0        0     2972 2024-05-21 13:45:22.000000 fairbalance-0.1.1/fairbalance/mitigation_strategies/base.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:29.798148 fairbalance-0.1.1/fairbalance/processors/
+-rw-rw-rw-   0        0        0        0 2024-05-21 13:43:44.000000 fairbalance-0.1.1/fairbalance/processors/__init__.py
+-rw-rw-rw-   0        0        0     1352 2024-05-21 13:48:02.000000 fairbalance-0.1.1/fairbalance/processors/_processors.py
+-rw-rw-rw-   0        0        0     7246 2024-05-21 13:47:39.000000 fairbalance-0.1.1/fairbalance/processors/base.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:29.968811 fairbalance-0.1.1/fairbalance/tools/
+-rw-rw-rw-   0        0        0      605 2024-05-21 13:28:32.000000 fairbalance-0.1.1/fairbalance/tools/__init__.py
+-rw-rw-rw-   0        0        0    10474 2024-05-17 08:27:03.000000 fairbalance-0.1.1/fairbalance/tools/_fairness_analysis.py
+-rw-rw-rw-   0        0        0    23251 2024-05-21 13:35:16.000000 fairbalance-0.1.1/fairbalance/tools/_mitigator.py
+-rw-rw-rw-   0        0        0    10322 2024-05-21 13:01:40.000000 fairbalance-0.1.1/fairbalance/tools/_processor.py
+-rw-rw-rw-   0        0        0     2115 2024-05-21 07:39:27.000000 fairbalance-0.1.1/fairbalance/tools/_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:30.043215 fairbalance-0.1.1/fairbalance/tools/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:11.000000 fairbalance-0.1.1/fairbalance/tools/tests/__init__.py
+-rw-rw-rw-   0        0        0     4296 2024-05-21 09:28:03.000000 fairbalance-0.1.1/fairbalance/tools/tests/test_fairness_analysis.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:32.000000 fairbalance-0.1.1/fairbalance/tools/tests/test_mitigator.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:43:17.000000 fairbalance-0.1.1/fairbalance/tools/tests/test_processor.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:56.000000 fairbalance-0.1.1/fairbalance/tools/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:29.544848 fairbalance-0.1.1/fairbalance.egg-info/
+-rw-rw-rw-   0        0        0      602 2024-05-21 13:51:25.000000 fairbalance-0.1.1/fairbalance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1279 2024-05-21 13:51:28.000000 fairbalance-0.1.1/fairbalance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 13:51:25.000000 fairbalance-0.1.1/fairbalance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-05-21 13:51:25.000000 fairbalance-0.1.1/fairbalance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 13:51:25.000000 fairbalance-0.1.1/fairbalance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2024-05-17 11:08:16.000000 fairbalance-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 13:51:30.067652 fairbalance-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      765 2024-05-21 13:50:53.000000 fairbalance-0.1.1/setup.py
```

### Comparing `fairbalance-0.0.4/PKG-INFO` & `fairbalance-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbalance
-Version: 0.0.4
+Version: 0.1.1
 Summary: bias mitigation by balancing target and/or protected attributes using resampling techniques
 Author: Pierre-Antoine Lequeu @ Fujitsu Luxembourg
 Author-email: pierre-antoine.lequeu@fujitsu.com
 Description-Content-Type: text/markdown
 Requires-Dist: folktables>=0.0.12
 Requires-Dist: imbalanced_learn==0.9.1
 Requires-Dist: numpy>=1.24.3
```

### Comparing `fairbalance-0.0.4/fairbalance/datasets/_datasets_loader.py` & `fairbalance-0.1.1/fairbalance/datasets/_datasets_loader.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.0.4/fairbalance/metrics/_dataset_metrics.py` & `fairbalance-0.1.1/fairbalance/metrics/_dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.0.4/fairbalance/metrics/_model_metrics.py` & `fairbalance-0.1.1/fairbalance/metrics/_model_metrics.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.0.4/fairbalance/tools/_fairness_analysis.py` & `fairbalance-0.1.1/fairbalance/tools/_fairness_analysis.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.0.4/fairbalance/tools/_mitigator.py` & `fairbalance-0.1.1/fairbalance/tools/_mitigator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,1324 +1,1454 @@
 00000000: 0d0a 696d 706f 7274 2070 616e 6461 7320  ..import pandas 
 00000010: 6173 2070 640d 0a66 726f 6d20 696d 626c  as pd..from imbl
-00000020: 6561 726e 2e62 6173 6520 696d 706f 7274  earn.base import
-00000030: 2042 6173 6553 616d 706c 6572 0d0a 6672   BaseSampler..fr
-00000040: 6f6d 2069 6d62 6c65 6172 6e2e 6f76 6572  om imblearn.over
-00000050: 5f73 616d 706c 696e 6720 696d 706f 7274  _sampling import
-00000060: 2052 616e 646f 6d4f 7665 7253 616d 706c   RandomOverSampl
-00000070: 6572 2c20 534d 4f54 454e 430d 0a66 726f  er, SMOTENC..fro
-00000080: 6d20 696d 626c 6561 726e 2e75 6e64 6572  m imblearn.under
-00000090: 5f73 616d 706c 696e 6720 696d 706f 7274  _sampling import
-000000a0: 2052 616e 646f 6d55 6e64 6572 5361 6d70   RandomUnderSamp
-000000b0: 6c65 720d 0a66 726f 6d20 736b 6c65 6172  ler..from sklear
-000000c0: 6e2e 6261 7365 2069 6d70 6f72 7420 4261  n.base import Ba
-000000d0: 7365 4573 7469 6d61 746f 722c 2043 6c61  seEstimator, Cla
-000000e0: 7373 6966 6965 724d 6978 696e 2c20 5472  ssifierMixin, Tr
-000000f0: 616e 7366 6f72 6d65 724d 6978 696e 2c20  ansformerMixin, 
-00000100: 5f66 6974 5f63 6f6e 7465 7874 0d0a 696d  _fit_context..im
-00000110: 706f 7274 2066 756e 6374 6f6f 6c73 0d0a  port functools..
-00000120: 0d0a 6672 6f6d 202e 5f75 7469 6c73 2069  ..from ._utils i
-00000130: 6d70 6f72 7420 7361 6e69 7479 5f63 6865  mport sanity_che
-00000140: 636b 6572 0d0a 6672 6f6d 202e 5f70 726f  cker..from ._pro
-00000150: 6365 7373 6f72 2069 6d70 6f72 7420 5072  cessor import Pr
-00000160: 6f63 6573 736f 720d 0a0d 0a53 414d 504c  ocessor....SAMPL
-00000170: 494e 475f 4655 4e43 5449 4f4e 5320 3d20  ING_FUNCTIONS = 
-00000180: 5b22 5261 6e64 6f6d 4f76 6572 5361 6d70  ["RandomOverSamp
-00000190: 6c65 7222 2c20 2253 4d4f 5445 4e43 222c  ler", "SMOTENC",
-000001a0: 2022 5261 6e64 6f6d 556e 6465 7253 616d   "RandomUnderSam
-000001b0: 706c 6572 225d 0d0a 0d0a 0d0a 636c 6173  pler"]......clas
-000001c0: 7320 4d69 7469 6761 7469 6f6e 5374 7261  s MitigationStra
-000001d0: 7465 6779 203a 0d0a 2020 2020 6465 6620  tegy :..    def 
-000001e0: 5f5f 696e 6974 5f5f 2873 656c 662c 2073  __init__(self, s
-000001f0: 616d 706c 696e 675f 6d65 7468 6f64 3a20  ampling_method: 
-00000200: 4261 7365 5361 6d70 6c65 722c 2074 6172  BaseSampler, tar
-00000210: 6765 743a 2073 7472 203d 204e 6f6e 652c  get: str = None,
-00000220: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
-00000230: 6275 7465 733a 206c 6973 7420 3d20 4e6f  butes: list = No
-00000240: 6e65 2c20 0d0a 2020 2020 2020 2020 2020  ne, ..          
-00000250: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00000260: 745f 636f 6c75 6d6e 733a 206c 6973 7420  t_columns: list 
-00000270: 3d20 4e6f 6e65 2c20 6361 745f 636f 6c75  = None, cat_colu
-00000280: 6d6e 733a 206c 6973 7420 3d20 4e6f 6e65  mns: list = None
-00000290: 2920 3a0d 0a20 2020 2020 2020 2073 656c  ) :..        sel
-000002a0: 662e 7461 7267 6574 203d 2074 6172 6765  f.target = targe
-000002b0: 740d 0a20 2020 2020 2020 2073 656c 662e  t..        self.
-000002c0: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
-000002d0: 7574 6573 203d 2070 726f 7465 6374 6564  utes = protected
-000002e0: 5f61 7474 7269 6275 7465 730d 0a20 2020  _attributes..   
-000002f0: 2020 2020 2073 656c 662e 636f 6e74 5f63       self.cont_c
-00000300: 6f6c 756d 6e73 203d 2063 6f6e 745f 636f  olumns = cont_co
-00000310: 6c75 6d6e 730d 0a20 2020 2020 2020 2073  lumns..        s
-00000320: 656c 662e 6361 745f 636f 6c75 6d6e 7320  elf.cat_columns 
-00000330: 3d20 6361 745f 636f 6c75 6d6e 730d 0a20  = cat_columns.. 
-00000340: 2020 2020 2020 2073 656c 662e 7361 6d70         self.samp
-00000350: 6c69 6e67 5f6d 6574 686f 6420 3d20 7361  ling_method = sa
-00000360: 6d70 6c69 6e67 5f6d 6574 686f 640d 0a0d  mpling_method...
-00000370: 0a63 6c61 7373 2042 616c 616e 6365 4f75  .class BalanceOu
-00000380: 7470 7574 2854 7261 6e73 666f 726d 6572  tput(Transformer
-00000390: 4d69 7869 6e2c 2042 6173 6545 7374 696d  Mixin, BaseEstim
-000003a0: 6174 6f72 2c20 4d69 7469 6761 7469 6f6e  ator, Mitigation
-000003b0: 5374 7261 7465 6779 293a 0d0a 2020 2020  Strategy):..    
-000003c0: 2222 2241 6e20 6578 616d 706c 6520 7472  """An example tr
-000003d0: 616e 7366 6f72 6d65 7220 7468 6174 2072  ansformer that r
-000003e0: 6574 7572 6e73 2074 6865 2065 6c65 6d65  eturns the eleme
-000003f0: 6e74 2d77 6973 6520 7371 7561 7265 2072  nt-wise square r
-00000400: 6f6f 742e 0d0a 0d0a 2020 2020 466f 7220  oot.....    For 
-00000410: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
-00000420: 2072 6567 6172 6469 6e67 2068 6f77 2074   regarding how t
-00000430: 6f20 6275 696c 6420 796f 7572 206f 776e  o build your own
-00000440: 2074 7261 6e73 666f 726d 6572 2c20 7265   transformer, re
-00000450: 6164 206d 6f72 650d 0a20 2020 2069 6e20  ad more..    in 
-00000460: 7468 6520 3a72 6566 3a60 5573 6572 2047  the :ref:`User G
-00000470: 7569 6465 203c 7573 6572 5f67 7569 6465  uide <user_guide
-00000480: 3e60 2e0d 0a0d 0a20 2020 2050 6172 616d  >`.....    Param
-00000490: 6574 6572 730d 0a20 2020 202d 2d2d 2d2d  eters..    -----
-000004a0: 2d2d 2d2d 2d0d 0a20 2020 2064 656d 6f5f  -----..    demo_
-000004b0: 7061 7261 6d20 3a20 7374 722c 2064 6566  param : str, def
-000004c0: 6175 6c74 3d27 6465 6d6f 270d 0a20 2020  ault='demo'..   
-000004d0: 2020 2020 2041 2070 6172 616d 6574 6572       A parameter
-000004e0: 2075 7365 6420 666f 7220 6465 6d6f 6e73   used for demons
-000004f0: 7461 7469 6f6e 206f 6620 686f 7720 746f  tation of how to
-00000500: 2070 6173 7320 616e 6420 7374 6f72 6520   pass and store 
-00000510: 7061 7261 6d74 6572 732e 0d0a 0d0a 2020  paramters.....  
-00000520: 2020 4174 7472 6962 7574 6573 0d0a 2020    Attributes..  
-00000530: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
-00000540: 2020 6e5f 6665 6174 7572 6573 5f69 6e5f    n_features_in_
-00000550: 203a 2069 6e74 0d0a 2020 2020 2020 2020   : int..        
-00000560: 4e75 6d62 6572 206f 6620 6665 6174 7572  Number of featur
-00000570: 6573 2073 6565 6e20 6475 7269 6e67 203a  es seen during :
-00000580: 7465 726d 3a60 6669 7460 2e0d 0a0d 0a20  term:`fit`..... 
-00000590: 2020 2066 6561 7475 7265 5f6e 616d 6573     feature_names
-000005a0: 5f69 6e5f 203a 206e 6461 7272 6179 206f  _in_ : ndarray o
-000005b0: 6620 7368 6170 6520 2860 6e5f 6665 6174  f shape (`n_feat
-000005c0: 7572 6573 5f69 6e5f 602c 290d 0a20 2020  ures_in_`,)..   
-000005d0: 2020 2020 204e 616d 6573 206f 6620 6665       Names of fe
-000005e0: 6174 7572 6573 2073 6565 6e20 6475 7269  atures seen duri
-000005f0: 6e67 203a 7465 726d 3a60 6669 7460 2e20  ng :term:`fit`. 
-00000600: 4465 6669 6e65 6420 6f6e 6c79 2077 6865  Defined only whe
-00000610: 6e20 6058 600d 0a20 2020 2020 2020 2068  n `X`..        h
-00000620: 6173 2066 6561 7475 7265 206e 616d 6573  as feature names
-00000630: 2074 6861 7420 6172 6520 616c 6c20 7374   that are all st
-00000640: 7269 6e67 732e 0d0a 2020 2020 2222 220d  rings...    """.
-00000650: 0a0d 0a20 2020 2023 2054 6869 7320 6973  ...    # This is
-00000660: 2061 2064 6963 7469 6f6e 6172 7920 616c   a dictionary al
-00000670: 6c6f 7769 6e67 2074 6f20 6465 6669 6e65  lowing to define
-00000680: 2074 6865 2074 7970 6520 6f66 2070 6172   the type of par
-00000690: 616d 6574 6572 732e 0d0a 2020 2020 2320  ameters...    # 
-000006a0: 4974 2075 7365 6420 746f 2076 616c 6964  It used to valid
-000006b0: 6174 6520 7061 7261 6d65 7465 7220 7769  ate parameter wi
-000006c0: 7468 696e 2074 6865 2060 5f66 6974 5f63  thin the `_fit_c
-000006d0: 6f6e 7465 7874 6020 6465 636f 7261 746f  ontext` decorato
-000006e0: 722e 0d0a 2020 2020 5f70 6172 616d 6574  r...    _paramet
-000006f0: 6572 5f63 6f6e 7374 7261 696e 7473 203d  er_constraints =
-00000700: 207b 0d0a 2020 2020 2020 2020 2264 656d   {..        "dem
-00000710: 6f5f 7061 7261 6d22 3a20 5b73 7472 5d2c  o_param": [str],
-00000720: 0d0a 2020 2020 7d0d 0a0d 0a20 2020 2040  ..    }....    @
-00000730: 5f66 6974 5f63 6f6e 7465 7874 2870 7265  _fit_context(pre
-00000740: 6665 725f 736b 6970 5f6e 6573 7465 645f  fer_skip_nested_
-00000750: 7661 6c69 6461 7469 6f6e 3d54 7275 6529  validation=True)
-00000760: 0d0a 2020 2020 6465 6620 6669 7428 7365  ..    def fit(se
-00000770: 6c66 2c20 582c 2079 3d4e 6f6e 6529 3a0d  lf, X, y=None):.
-00000780: 0a20 2020 2020 2020 2022 2222 4120 7265  .        """A re
-00000790: 6665 7265 6e63 6520 696d 706c 656d 656e  ference implemen
-000007a0: 7461 7469 6f6e 206f 6620 6120 6669 7474  tation of a fitt
-000007b0: 696e 6720 6675 6e63 7469 6f6e 2066 6f72  ing function for
-000007c0: 2061 2074 7261 6e73 666f 726d 6572 2e0d   a transformer..
-000007d0: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-000007e0: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
-000007f0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
-00000800: 2020 2058 203a 207b 6172 7261 792d 6c69     X : {array-li
-00000810: 6b65 2c20 7370 6172 7365 206d 6174 7269  ke, sparse matri
-00000820: 787d 2c20 7368 6170 6520 286e 5f73 616d  x}, shape (n_sam
-00000830: 706c 6573 2c20 6e5f 6665 6174 7572 6573  ples, n_features
-00000840: 290d 0a20 2020 2020 2020 2020 2020 2054  )..            T
-00000850: 6865 2074 7261 696e 696e 6720 696e 7075  he training inpu
-00000860: 7420 7361 6d70 6c65 732e 0d0a 0d0a 2020  t samples.....  
-00000870: 2020 2020 2020 7920 3a20 4e6f 6e65 0d0a        y : None..
-00000880: 2020 2020 2020 2020 2020 2020 5468 6572              Ther
-00000890: 6520 6973 206e 6f20 6e65 6564 206f 6620  e is no need of 
-000008a0: 6120 7461 7267 6574 2069 6e20 6120 7472  a target in a tr
-000008b0: 616e 7366 6f72 6d65 722c 2079 6574 2074  ansformer, yet t
-000008c0: 6865 2070 6970 656c 696e 6520 4150 490d  he pipeline API.
-000008d0: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-000008e0: 7569 7265 7320 7468 6973 2070 6172 616d  uires this param
-000008f0: 6574 6572 2e0d 0a0d 0a20 2020 2020 2020  eter.....       
-00000900: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
-00000910: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
-00000920: 2020 2073 656c 6620 3a20 6f62 6a65 6374     self : object
-00000930: 0d0a 2020 2020 2020 2020 2020 2020 5265  ..            Re
-00000940: 7475 726e 7320 7365 6c66 2e0d 0a20 2020  turns self...   
-00000950: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00000960: 2020 5820 3d20 7365 6c66 2e5f 7661 6c69    X = self._vali
-00000970: 6461 7465 5f64 6174 6128 582c 2061 6363  date_data(X, acc
-00000980: 6570 745f 7370 6172 7365 3d54 7275 6529  ept_sparse=True)
-00000990: 0d0a 0d0a 2020 2020 2020 2020 2320 5265  ....        # Re
-000009a0: 7475 726e 2074 6865 2074 7261 6e73 666f  turn the transfo
-000009b0: 726d 6572 0d0a 2020 2020 2020 2020 7265  rmer..        re
-000009c0: 7475 726e 2073 656c 660d 0a0d 0a20 2020  turn self....   
-000009d0: 2064 6566 2074 7261 6e73 666f 726d 2873   def transform(s
-000009e0: 656c 662c 2058 293a 0d0a 2020 2020 2020  elf, X):..      
-000009f0: 2020 2222 2241 2072 6566 6572 656e 6365    """A reference
-00000a00: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
-00000a10: 6f66 2061 2074 7261 6e73 666f 726d 2066  of a transform f
-00000a20: 756e 6374 696f 6e2e 0d0a 0d0a 2020 2020  unction.....    
-00000a30: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
-00000a40: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00000a50: 2d2d 0d0a 2020 2020 2020 2020 5820 3a20  --..        X : 
-00000a60: 7b61 7272 6179 2d6c 696b 652c 2073 7061  {array-like, spa
-00000a70: 7273 652d 6d61 7472 6978 7d2c 2073 6861  rse-matrix}, sha
-00000a80: 7065 2028 6e5f 7361 6d70 6c65 732c 206e  pe (n_samples, n
-00000a90: 5f66 6561 7475 7265 7329 0d0a 2020 2020  _features)..    
-00000aa0: 2020 2020 2020 2020 5468 6520 696e 7075          The inpu
-00000ab0: 7420 7361 6d70 6c65 732e 0d0a 0d0a 2020  t samples.....  
-00000ac0: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
-00000ad0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
-00000ae0: 2020 2020 2020 2020 585f 7472 616e 7366          X_transf
-00000af0: 6f72 6d65 6420 3a20 6172 7261 792c 2073  ormed : array, s
-00000b00: 6861 7065 2028 6e5f 7361 6d70 6c65 732c  hape (n_samples,
-00000b10: 206e 5f66 6561 7475 7265 7329 0d0a 2020   n_features)..  
-00000b20: 2020 2020 2020 2020 2020 5468 6520 6172            The ar
-00000b30: 7261 7920 636f 6e74 6169 6e69 6e67 2074  ray containing t
-00000b40: 6865 2065 6c65 6d65 6e74 2d77 6973 6520  he element-wise 
-00000b50: 7371 7561 7265 2072 6f6f 7473 206f 6620  square roots of 
-00000b60: 7468 6520 7661 6c75 6573 0d0a 2020 2020  the values..    
-00000b70: 2020 2020 2020 2020 696e 2060 6058 6060          in ``X``
-00000b80: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-00000b90: 2020 2020 2020 2020 2320 5369 6e63 6520          # Since 
-00000ba0: 7468 6973 2069 7320 6120 7374 6174 656c  this is a statel
-00000bb0: 6573 7320 7472 616e 7366 6f72 6d65 722c  ess transformer,
-00000bc0: 2077 6520 7368 6f75 6c64 206e 6f74 2063   we should not c
-00000bd0: 616c 6c20 6063 6865 636b 5f69 735f 6669  all `check_is_fi
-00000be0: 7474 6564 602e 0d0a 2020 2020 2020 2020  tted`...        
-00000bf0: 2320 436f 6d6d 6f6e 2074 6573 7420 7769  # Common test wi
-00000c00: 6c6c 2063 6865 636b 2066 6f72 2074 6869  ll check for thi
-00000c10: 7320 7061 7274 6963 756c 6172 6c79 2e0d  s particularly..
-00000c20: 0a0d 0a20 2020 2020 2020 2023 2049 6e70  ...        # Inp
-00000c30: 7574 2076 616c 6964 6174 696f 6e0d 0a20  ut validation.. 
-00000c40: 2020 2020 2020 2023 2057 6520 6e65 6564         # We need
-00000c50: 2074 6f20 7365 7420 7265 7365 743d 4661   to set reset=Fa
-00000c60: 6c73 6520 6265 6361 7573 6520 7765 2064  lse because we d
-00000c70: 6f6e 2774 2077 616e 7420 746f 206f 7665  on't want to ove
-00000c80: 7277 7269 7465 2060 6e5f 6665 6174 7572  rwrite `n_featur
-00000c90: 6573 5f69 6e5f 600d 0a20 2020 2020 2020  es_in_`..       
-00000ca0: 2023 2060 6665 6174 7572 655f 6e61 6d65   # `feature_name
-00000cb0: 735f 696e 5f60 2062 7574 206f 6e6c 7920  s_in_` but only 
-00000cc0: 6368 6563 6b20 7468 6174 2074 6865 2073  check that the s
-00000cd0: 6861 7065 2069 7320 636f 6e73 6973 7465  hape is consiste
-00000ce0: 6e74 2e0d 0a20 2020 2020 2020 2058 203d  nt...        X =
-00000cf0: 2073 656c 662e 5f76 616c 6964 6174 655f   self._validate_
-00000d00: 6461 7461 2858 2c20 6163 6365 7074 5f73  data(X, accept_s
-00000d10: 7061 7273 653d 5472 7565 2c20 7265 7365  parse=True, rese
-00000d20: 743d 4661 6c73 6529 0d0a 2020 2020 2020  t=False)..      
-00000d30: 2020 7265 7475 726e 206e 702e 7371 7274    return np.sqrt
-00000d40: 2858 290d 0a0d 0a20 2020 2064 6566 205f  (X)....    def _
-00000d50: 6d6f 7265 5f74 6167 7328 7365 6c66 293a  more_tags(self):
-00000d60: 0d0a 2020 2020 2020 2020 2320 5468 6973  ..        # This
-00000d70: 2069 7320 6120 7175 6963 6b20 6578 616d   is a quick exam
-00000d80: 706c 6520 746f 2073 686f 7720 7468 6520  ple to show the 
-00000d90: 7461 6773 2041 5049 3a5c 0d0a 2020 2020  tags API:\..    
-00000da0: 2020 2020 2320 6874 7470 733a 2f2f 7363      # https://sc
-00000db0: 696b 6974 2d6c 6561 726e 2e6f 7267 2f64  ikit-learn.org/d
-00000dc0: 6576 2f64 6576 656c 6f70 6572 732f 6465  ev/developers/de
-00000dd0: 7665 6c6f 702e 6874 6d6c 2365 7374 696d  velop.html#estim
-00000de0: 6174 6f72 2d74 6167 730d 0a20 2020 2020  ator-tags..     
-00000df0: 2020 2023 2048 6572 652c 206f 7572 2074     # Here, our t
-00000e00: 7261 6e73 666f 726d 6572 2064 6f65 7320  ransformer does 
-00000e10: 6e6f 7420 646f 2061 6e79 206f 7065 7261  not do any opera
-00000e20: 7469 6f6e 2069 6e20 6066 6974 6020 616e  tion in `fit` an
-00000e30: 6420 6f6e 6c79 2076 616c 6964 6174 650d  d only validate.
-00000e40: 0a20 2020 2020 2020 2023 2074 6865 2070  .        # the p
-00000e50: 6172 616d 6574 6572 732e 2054 6875 732c  arameters. Thus,
-00000e60: 2069 7420 6973 2073 7461 7465 6c65 7373   it is stateless
-00000e70: 2e0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-00000e80: 6e20 7b22 7374 6174 656c 6573 7322 3a20  n {"stateless": 
-00000e90: 5472 7565 7d0d 0a20 2020 2020 2020 200d  True}..        .
-00000ea0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00000eb0: 2020 200d 0a20 2020 2020 2020 200d 0a63     ..        ..c
-00000ec0: 6c61 7373 204d 6974 6967 6174 6f72 2873  lass Mitigator(s
-00000ed0: 616e 6974 795f 6368 6563 6b65 7229 203a  anity_checker) :
-00000ee0: 0d0a 0d0a 2020 2020 6465 6620 5f5f 696e  ....    def __in
-00000ef0: 6974 5f5f 2873 656c 662c 206d 6574 686f  it__(self, metho
-00000f00: 6420 3d20 2252 616e 646f 6d4f 7665 7253  d = "RandomOverS
-00000f10: 616d 706c 6572 2229 203a 0d0a 2020 2020  ampler") :..    
-00000f20: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00000f30: 204d 6974 6967 6174 6f72 2069 6d70 6c65   Mitigator imple
-00000f40: 6d65 6e74 2064 6966 6665 7265 6e74 2074  ment different t
-00000f50: 7970 6573 206f 6620 6269 6169 7320 6d69  ypes of biais mi
-00000f60: 7469 6761 7469 6f6e 2062 7920 7265 7361  tigation by resa
-00000f70: 6d70 6c69 6e67 2e0d 0a0d 0a20 2020 2020  mpling.....     
-00000f80: 2020 2041 7267 733a 0d0a 2020 2020 2020     Args:..      
-00000f90: 2020 2020 2020 6d65 7468 6f64 2028 7374        method (st
-00000fa0: 722c 206f 7074 696f 6e61 6c29 3a20 7265  r, optional): re
-00000fb0: 7361 6d70 6c69 6e67 206d 6574 686f 6473  sampling methods
-00000fc0: 2069 6d70 6c65 6d65 6e74 6564 2062 7920   implemented by 
-00000fd0: 696d 626c 6561 726e 2e20 506f 7373 6962  imblearn. Possib
-00000fe0: 6c65 2076 616c 7565 7320 6172 6520 2252  le values are "R
-00000ff0: 616e 646f 6d4f 7665 7253 616d 706c 6572  andomOverSampler
-00001000: 222c 200d 0a20 2020 2020 2020 2020 2020  ", ..           
-00001010: 2022 534d 4f54 454e 4322 2061 6e64 2022   "SMOTENC" and "
-00001020: 5261 6e64 6f6d 556e 6465 7253 616d 706c  RandomUnderSampl
-00001030: 6572 222e 2020 4465 6661 756c 7473 2074  er".  Defaults t
-00001040: 6f20 2252 616e 646f 6d4f 7665 7253 616d  o "RandomOverSam
-00001050: 706c 6572 222e 0d0a 2020 2020 2020 2020  pler"...        
-00001060: 2222 220d 0a20 2020 2020 2020 200d 0a20  """..        .. 
-00001070: 2020 2020 2020 2073 656c 662e 5f69 6e69         self._ini
-00001080: 745f 7361 6e69 7479 5f63 6865 636b 286d  t_sanity_check(m
-00001090: 6574 686f 6429 0d0a 2020 2020 2020 2020  ethod)..        
-000010a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
-000010b0: 6574 686f 6420 3d20 6d65 7468 6f64 0d0a  ethod = method..
-000010c0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-000010d0: 6967 6174 6f72 5f66 756e 6374 696f 6e20  igator_function 
-000010e0: 3d20 7b0d 0a20 2020 2020 2020 2020 2020  = {..           
-000010f0: 2022 5261 6e64 6f6d 4f76 6572 5361 6d70   "RandomOverSamp
-00001100: 6c65 7222 203a 2052 616e 646f 6d4f 7665  ler" : RandomOve
-00001110: 7253 616d 706c 6572 2c0d 0a20 2020 2020  rSampler,..     
-00001120: 2020 2020 2020 2020 2253 4d4f 5445 4e43          "SMOTENC
-00001130: 2220 3a20 534d 4f54 454e 432c 0d0a 2020  " : SMOTENC,..  
-00001140: 2020 2020 2020 2020 2020 2022 5261 6e64             "Rand
-00001150: 6f6d 556e 6465 7253 616d 706c 6572 2220  omUnderSampler" 
-00001160: 3a20 5261 6e64 6f6d 556e 6465 7253 616d  : RandomUnderSam
-00001170: 706c 6572 0d0a 2020 2020 2020 2020 7d0d  pler..        }.
-00001180: 0a20 2020 200d 0a20 2020 2064 6566 205f  .    ..    def _
-00001190: 696e 6974 5f73 616e 6974 795f 6368 6563  init_sanity_chec
-000011a0: 6b28 7365 6c66 2c20 6d65 7468 6f64 2920  k(self, method) 
-000011b0: 3a0d 0a20 2020 2020 2020 2061 7373 6572  :..        asser
-000011c0: 7420 6d65 7468 6f64 2069 6e20 5341 4d50  t method in SAMP
-000011d0: 4c49 4e47 5f46 554e 4354 494f 4e53 2c20  LING_FUNCTIONS, 
-000011e0: 6622 6d65 7468 6f64 206e 6565 6420 746f  f"method need to
-000011f0: 2062 6520 696e 207b 5341 4d50 4c49 4e47   be in {SAMPLING
-00001200: 5f46 554e 4354 494f 4e53 7d22 0d0a 0d0a  _FUNCTIONS}"....
-00001210: 2020 2020 0d0a 2020 2020 6465 6620 6d69      ..    def mi
-00001220: 7469 6761 7465 2873 656c 662c 206d 6974  tigate(self, mit
-00001230: 6967 6174 696f 6e5f 7374 7261 7465 6779  igation_strategy
-00001240: 3a20 7374 722c 2064 6174 6173 6574 3a20  : str, dataset: 
-00001250: 7064 2e44 6174 6146 7261 6d65 2c20 7461  pd.DataFrame, ta
-00001260: 7267 6574 3a20 7374 722c 200d 0a20 2020  rget: str, ..   
-00001270: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00001280: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
-00001290: 6573 3a20 6c69 7374 203d 204e 6f6e 652c  es: list = None,
-000012a0: 2063 6f6e 745f 636f 6c75 6d6e 733a 206c   cont_columns: l
-000012b0: 6973 7420 3d20 4e6f 6e65 2c20 6361 745f  ist = None, cat_
-000012c0: 636f 6c75 6d6e 733a 206c 6973 7420 3d20  columns: list = 
-000012d0: 4e6f 6e65 2920 3a0d 0a20 2020 2020 2020  None) :..       
-000012e0: 2022 2222 0d0a 2020 2020 2020 2020 4d69   """..        Mi
-000012f0: 7469 6761 7465 2062 6961 7320 7573 696e  tigate bias usin
-00001300: 6720 7468 6520 6769 7665 6e20 6d69 7469  g the given miti
-00001310: 6761 7469 6f6e 2073 7472 6174 6567 790d  gation strategy.
-00001320: 0a0d 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00001330: 0d0a 2020 2020 2020 2020 2020 2020 6d69  ..            mi
-00001340: 7469 6761 7469 6f6e 5f73 7472 6174 6567  tigation_strateg
-00001350: 7920 2873 7472 293a 2074 6865 206d 6974  y (str): the mit
-00001360: 6967 6174 696f 6e20 7374 7261 7465 6779  igation strategy
-00001370: 2074 6f20 7573 652e 2050 6f73 7369 626c   to use. Possibl
-00001380: 6520 7661 6c75 6573 2061 7265 2022 6261  e values are "ba
-00001390: 6c61 6e65 5f6f 7574 7075 7422 2c20 2262  lane_output", "b
-000013a0: 616c 616e 6365 5f70 726f 7465 6374 6564  alance_protected
-000013b0: 5f61 7474 7269 6275 7465 222c 2022 6261  _attribute", "ba
-000013c0: 6c61 6e63 655f 6f75 7470 7574 2066 6f72  lance_output for
-000013d0: 2061 7474 7269 6275 7465 2220 616e 6420   attribute" and 
-000013e0: 2262 616c 616e 6365 5f61 6c6c 222e 200d  "balance_all". .
-000013f0: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
-00001400: 6e65 2220 6973 2061 6c73 6f20 696d 706c  ne" is also impl
-00001410: 656d 656e 7465 6420 666f 7220 6265 6e63  emented for benc
-00001420: 686d 6172 6b69 6e67 2063 6f6e 7369 7374  hmarking consist
-00001430: 656e 6379 2061 6e64 2073 696d 706c 7920  ency and simply 
-00001440: 7265 7475 726e 2074 6865 2069 6e69 7469  return the initi
-00001450: 616c 2064 6174 6173 6574 2061 6e64 2074  al dataset and t
-00001460: 6172 6765 742e 200d 0a20 2020 2020 2020  arget. ..       
-00001470: 2020 2020 2064 6174 6173 6574 2028 7064       dataset (pd
-00001480: 2e44 6174 6146 7261 6d65 293a 2064 6174  .DataFrame): dat
-00001490: 6173 6574 2074 6f20 6d69 7469 6761 7465  aset to mitigate
-000014a0: 2c20 7468 6174 2069 6e63 6c75 6465 7320  , that includes 
-000014b0: 7468 6520 7461 7267 6574 2063 6f6c 756d  the target colum
-000014c0: 6e2e 0d0a 2020 2020 2020 2020 2020 2020  n...            
-000014d0: 7461 7267 6574 2028 7374 7229 3a20 7468  target (str): th
-000014e0: 6520 7461 7267 6574 2063 6f6c 756d 6e20  e target column 
-000014f0: 6e61 6d65 0d0a 2020 2020 2020 2020 2020  name..          
-00001500: 2020 7072 6f74 6563 7465 645f 6174 7472    protected_attr
-00001510: 6962 7574 6573 2028 6c69 7374 2c20 6f70  ibutes (list, op
-00001520: 7469 6f6e 616c 293a 2054 6865 2061 7474  tional): The att
-00001530: 7269 6275 7465 2873 2920 746f 2062 616c  ribute(s) to bal
-00001540: 616e 6365 2e20 4f6e 6c79 206e 6563 6573  ance. Only neces
-00001550: 7361 7279 2066 6f72 2062 616c 616e 6365  sary for balance
-00001560: 5f70 726f 7465 6374 6564 5f61 7474 7269  _protected_attri
-00001570: 6275 7465 2061 6e64 2062 616c 616e 6365  bute and balance
-00001580: 5f6f 7574 7075 745f 666f 725f 6174 7472  _output_for_attr
-00001590: 6962 7574 652e 2044 6566 6175 6c74 7320  ibute. Defaults 
-000015a0: 746f 204e 6f6e 652e 0d0a 2020 2020 2020  to None...      
-000015b0: 2020 2020 2020 636f 6e74 5f63 6f6c 756d        cont_colum
-000015c0: 6e73 2028 6c69 7374 2c20 6f70 7469 6f6e  ns (list, option
-000015d0: 616c 293a 2054 6865 2063 6f6e 7469 6e75  al): The continu
-000015e0: 6f75 7320 636f 6c75 6d6e 7320 696e 2074  ous columns in t
-000015f0: 6865 2064 6174 6173 6574 2e20 4f6e 6c79  he dataset. Only
-00001600: 204e 6563 6573 7361 7279 2069 6620 7468   Necessary if th
-00001610: 6520 7361 6d70 6c69 6e67 2073 7472 6174  e sampling strat
-00001620: 6567 7920 6973 2053 4d4f 5445 4e43 2e20  egy is SMOTENC. 
-00001630: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
-00001640: 2e0d 0a20 2020 2020 2020 2020 2020 2063  ...            c
-00001650: 6174 5f63 6f6c 756d 6e73 2028 6c69 7374  at_columns (list
-00001660: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
-00001670: 2063 6174 6567 6f72 6963 616c 2063 6f6c   categorical col
-00001680: 756d 6e73 2069 6e20 7468 6520 6461 7461  umns in the data
-00001690: 7365 742e 204f 6e6c 7920 4e65 6365 7373  set. Only Necess
-000016a0: 6172 7920 6966 2074 6865 2073 616d 706c  ary if the sampl
-000016b0: 696e 6720 7374 7261 7465 6779 2069 7320  ing strategy is 
-000016c0: 534d 4f54 454e 432e 2044 6566 6175 6c74  SMOTENC. Default
-000016d0: 7320 746f 204e 6f6e 652e 0d0a 0d0a 2020  s to None.....  
-000016e0: 2020 2020 2020 5261 6973 6573 3a0d 0a20        Raises:.. 
-000016f0: 2020 2020 2020 2020 2020 2056 616c 7565             Value
-00001700: 4572 726f 723a 2049 6620 7468 6520 6d69  Error: If the mi
-00001710: 7469 6761 7469 6f6e 2073 7472 6174 6567  tigation strateg
-00001720: 7920 646f 6573 206e 6f74 2065 7869 7374  y does not exist
-00001730: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-00001740: 726e 733a 0d0a 2020 2020 2020 2020 2020  rns:..          
-00001750: 2020 285b 7064 2e44 6174 6146 7261 6d65    ([pd.DataFrame
-00001760: 2c20 7064 2e44 6174 6146 7261 6d65 5d29  , pd.DataFrame])
-00001770: 3a20 7468 6520 6261 6c61 6e63 6564 2064  : the balanced d
-00001780: 6174 6166 7261 6d65 7320 666f 7220 7468  ataframes for th
-00001790: 6520 6461 7461 7365 7420 616e 6420 7468  e dataset and th
-000017a0: 6520 7461 7267 6574 0d0a 2020 2020 2020  e target..      
-000017b0: 2020 2222 220d 0a20 2020 2020 2020 2069    """..        i
-000017c0: 6620 6d69 7469 6761 7469 6f6e 5f73 7472  f mitigation_str
-000017d0: 6174 6567 7920 3d3d 2022 6261 6c61 6e63  ategy == "balanc
-000017e0: 655f 6f75 7470 7574 2220 3a0d 0a20 2020  e_output" :..   
-000017f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00001800: 7365 6c66 2e62 616c 616e 6365 5f6f 7574  self.balance_out
-00001810: 7075 7428 6461 7461 7365 742c 2074 6172  put(dataset, tar
-00001820: 6765 742c 2070 726f 7465 6374 6564 5f61  get, protected_a
-00001830: 7474 7269 6275 7465 732c 2063 6f6e 745f  ttributes, cont_
-00001840: 636f 6c75 6d6e 732c 2063 6174 5f63 6f6c  columns, cat_col
-00001850: 756d 6e73 290d 0a20 2020 2020 2020 2065  umns)..        e
-00001860: 6c69 6620 6d69 7469 6761 7469 6f6e 5f73  lif mitigation_s
-00001870: 7472 6174 6567 7920 3d3d 2022 6261 6c61  trategy == "bala
-00001880: 6e63 655f 7072 6f74 6563 7465 645f 6174  nce_protected_at
-00001890: 7472 6962 7574 6522 203a 0d0a 2020 2020  tribute" :..    
-000018a0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000018b0: 656c 662e 6261 6c61 6e63 655f 7072 6f74  elf.balance_prot
-000018c0: 6563 7465 645f 6174 7472 6962 7574 6528  ected_attribute(
-000018d0: 6461 7461 7365 742c 2074 6172 6765 742c  dataset, target,
-000018e0: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
-000018f0: 6275 7465 732c 2063 6f6e 745f 636f 6c75  butes, cont_colu
-00001900: 6d6e 732c 2063 6174 5f63 6f6c 756d 6e73  mns, cat_columns
-00001910: 290d 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
-00001920: 6d69 7469 6761 7469 6f6e 5f73 7472 6174  mitigation_strat
-00001930: 6567 7920 3d3d 2022 6261 6c61 6e63 655f  egy == "balance_
-00001940: 6f75 7470 7574 5f66 6f72 5f61 7474 7269  output_for_attri
-00001950: 6275 7465 2220 3a0d 0a20 2020 2020 2020  bute" :..       
-00001960: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00001970: 2e62 616c 616e 6365 5f6f 7574 7075 745f  .balance_output_
-00001980: 666f 725f 6174 7472 6962 7574 6528 6461  for_attribute(da
-00001990: 7461 7365 742c 2074 6172 6765 742c 2070  taset, target, p
-000019a0: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
-000019b0: 7465 732c 2063 6f6e 745f 636f 6c75 6d6e  tes, cont_column
-000019c0: 732c 2063 6174 5f63 6f6c 756d 6e73 290d  s, cat_columns).
-000019d0: 0a20 2020 2020 2020 2065 6c69 6620 6d69  .        elif mi
-000019e0: 7469 6761 7469 6f6e 5f73 7472 6174 6567  tigation_strateg
-000019f0: 7920 3d3d 2022 6261 6c61 6e63 655f 616c  y == "balance_al
-00001a00: 6c22 203a 0d0a 2020 2020 2020 2020 2020  l" :..          
-00001a10: 2020 7265 7475 726e 2073 656c 662e 6261    return self.ba
-00001a20: 6c61 6e63 655f 616c 6c28 6461 7461 7365  lance_all(datase
-00001a30: 742c 2074 6172 6765 742c 2070 726f 7465  t, target, prote
-00001a40: 6374 6564 5f61 7474 7269 6275 7465 732c  cted_attributes,
-00001a50: 2063 6f6e 745f 636f 6c75 6d6e 732c 2063   cont_columns, c
-00001a60: 6174 5f63 6f6c 756d 6e73 290d 0a20 2020  at_columns)..   
-00001a70: 2020 2020 2065 6c69 6620 6d69 7469 6761       elif mitiga
-00001a80: 7469 6f6e 5f73 7472 6174 6567 7920 3d3d  tion_strategy ==
-00001a90: 2022 6e6f 6e65 2220 3a0d 0a20 2020 2020   "none" :..     
-00001aa0: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
-00001ab0: 7461 7365 742c 2074 6172 6765 740d 0a20  taset, target.. 
-00001ac0: 2020 2020 2020 2065 6c73 6520 3a0d 0a20         else :.. 
-00001ad0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00001ae0: 2056 616c 7565 4572 726f 720d 0a20 2020   ValueError..   
-00001af0: 2020 2020 200d 0a20 2020 2064 6566 2062       ..    def b
-00001b00: 616c 616e 6365 5f6f 7574 7075 7428 7365  alance_output(se
-00001b10: 6c66 2c20 6461 7461 7365 743a 2070 642e  lf, dataset: pd.
-00001b20: 4461 7461 4672 616d 652c 2074 6172 6765  DataFrame, targe
-00001b30: 743a 2073 7472 2c20 7072 6f74 6563 7465  t: str, protecte
-00001b40: 645f 6174 7472 6962 7574 6573 3a20 6c69  d_attributes: li
-00001b50: 7374 203d 204e 6f6e 652c 200d 0a20 2020  st = None, ..   
-00001b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b70: 2020 2020 636f 6e74 5f63 6f6c 756d 6e73      cont_columns
-00001b80: 3a20 6c69 7374 203d 204e 6f6e 652c 2063  : list = None, c
-00001b90: 6174 5f63 6f6c 756d 6e73 3a20 6c69 7374  at_columns: list
-00001ba0: 203d 204e 6f6e 6529 203a 0d0a 2020 2020   = None) :..    
-00001bb0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00001bc0: 2042 616c 616e 6365 2074 6865 206f 7574   Balance the out
-00001bd0: 7075 7420 7769 7468 206e 6f20 7265 6761  put with no rega
-00001be0: 7264 7320 746f 2074 6865 2070 726f 7465  rds to the prote
-00001bf0: 6374 6564 2061 7474 7269 6275 7465 732e  cted attributes.
-00001c00: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00001c10: 2020 2020 4172 6773 3a20 0d0a 2020 2020      Args: ..    
-00001c20: 2020 2020 2020 2020 6461 7461 7365 7420          dataset 
-00001c30: 2870 642e 4461 7461 4672 616d 6529 3a20  (pd.DataFrame): 
-00001c40: 6461 7461 7365 7420 746f 206d 6974 6967  dataset to mitig
-00001c50: 6174 652c 2074 6861 7420 696e 636c 7564  ate, that includ
-00001c60: 6573 2074 6865 2074 6172 6765 7420 636f  es the target co
-00001c70: 6c75 6d6e 2e0d 0a20 2020 2020 2020 2020  lumn...         
-00001c80: 2020 2074 6172 6765 7420 2873 7472 293a     target (str):
-00001c90: 2074 6865 2074 6172 6765 7420 636f 6c75   the target colu
-00001ca0: 6d6e 206e 616d 650d 0a20 2020 2020 2020  mn name..       
-00001cb0: 2020 2020 2070 726f 7465 6374 6564 5f61       protected_a
-00001cc0: 7474 7269 6275 7465 7320 286c 6973 742c  ttributes (list,
-00001cd0: 206f 7074 696f 6e61 6c29 3a20 5573 656c   optional): Usel
-00001ce0: 6573 7320 666f 7220 7468 6973 206d 6974  ess for this mit
-00001cf0: 6967 6174 696f 6e20 7374 7261 7465 6779  igation strategy
-00001d00: 2c20 6275 7420 696d 706c 656d 656e 7465  , but implemente
-00001d10: 6420 666f 7220 4150 4920 636f 6e73 6973  d for API consis
-00001d20: 7465 6e63 792e 2044 6566 6175 6c74 7320  tency. Defaults 
-00001d30: 746f 204e 6f6e 652e 0d0a 2020 2020 2020  to None...      
-00001d40: 2020 2020 2020 636f 6e74 5f63 6f6c 756d        cont_colum
-00001d50: 6e73 2028 6c69 7374 2c20 6f70 7469 6f6e  ns (list, option
-00001d60: 616c 293a 2054 6865 2063 6f6e 7469 6e75  al): The continu
-00001d70: 6f75 7320 636f 6c75 6d6e 7320 696e 2074  ous columns in t
-00001d80: 6865 2064 6174 6173 6574 2e20 4f6e 6c79  he dataset. Only
-00001d90: 204e 6563 6573 7361 7279 2069 6620 7468   Necessary if th
-00001da0: 6520 7361 6d70 6c69 6e67 2073 7472 6174  e sampling strat
-00001db0: 6567 7920 6973 2053 4d4f 5445 4e43 2e20  egy is SMOTENC. 
-00001dc0: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
-00001dd0: 2e0d 0a20 2020 2020 2020 2020 2020 2063  ...            c
-00001de0: 6174 5f63 6f6c 756d 6e73 2028 6c69 7374  at_columns (list
-00001df0: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
-00001e00: 2063 6174 6567 6f72 6963 616c 2063 6f6c   categorical col
-00001e10: 756d 6e73 2069 6e20 7468 6520 6461 7461  umns in the data
-00001e20: 7365 742e 204f 6e6c 7920 4e65 6365 7373  set. Only Necess
-00001e30: 6172 7920 6966 2074 6865 2073 616d 706c  ary if the sampl
-00001e40: 696e 6720 7374 7261 7465 6779 2069 7320  ing strategy is 
-00001e50: 534d 4f54 454e 432e 2044 6566 6175 6c74  SMOTENC. Default
-00001e60: 7320 746f 204e 6f6e 652e 0d0a 0d0a 2020  s to None.....  
-00001e70: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
-00001e80: 2020 2020 2020 2020 2020 2020 285b 7064              ([pd
-00001e90: 2e44 6174 6146 7261 6d65 2c20 7064 2e44  .DataFrame, pd.D
-00001ea0: 6174 6146 7261 6d65 5d29 3a20 7468 6520  ataFrame]): the 
-00001eb0: 6261 6c61 6e63 6564 2064 6174 6166 7261  balanced datafra
-00001ec0: 6d65 7320 666f 7220 7468 6520 6461 7461  mes for the data
-00001ed0: 7365 7420 616e 6420 7468 6520 7461 7267  set and the targ
-00001ee0: 6574 0d0a 2020 2020 2020 2020 2222 220d  et..        """.
-00001ef0: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-00001f00: 2e5f 7361 6e69 7479 5f63 6865 636b 2864  ._sanity_check(d
-00001f10: 6174 6173 6574 2c20 7461 7267 6574 2c20  ataset, target, 
-00001f20: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
-00001f30: 7574 6573 3d70 726f 7465 6374 6564 5f61  utes=protected_a
-00001f40: 7474 7269 6275 7465 7329 0d0a 2020 2020  ttributes)..    
-00001f50: 2020 2020 0d0a 2020 2020 2020 2020 2369      ..        #i
-00001f60: 6620 6e6f 7420 5261 6e64 6f6d 4f76 6572  f not RandomOver
-00001f70: 5361 6d70 6c65 722c 206e 6565 6420 746f  Sampler, need to
-00001f80: 206f 6e65 2d68 6f74 2065 6e63 6f64 6520   one-hot encode 
-00001f90: 6576 6572 7920 6361 7465 676f 7269 6361  every categorica
-00001fa0: 6c0d 0a20 2020 2020 2020 2064 6620 3d20  l..        df = 
-00001fb0: 6461 7461 7365 742e 636f 7079 2829 0d0a  dataset.copy()..
-00001fc0: 2020 2020 2020 2020 7461 7267 6574 5f64          target_d
-00001fd0: 6620 3d20 6466 5b74 6172 6765 745d 0d0a  f = df[target]..
-00001fe0: 2020 2020 2020 2020 6466 203d 2064 662e          df = df.
-00001ff0: 6472 6f70 2863 6f6c 756d 6e73 3d74 6172  drop(columns=tar
-00002000: 6765 7429 0d0a 2020 2020 2020 2020 0d0a  get)..        ..
-00002010: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00002020: 2020 6966 2070 726f 7465 6374 6564 5f61    if protected_a
-00002030: 7474 7269 6275 7465 7320 616e 6420 6c65  ttributes and le
-00002040: 6e28 7072 6f74 6563 7465 645f 6174 7472  n(protected_attr
-00002050: 6962 7574 6573 2920 3e20 3120 3a0d 0a20  ibutes) > 1 :.. 
-00002060: 2020 2020 2020 2020 2020 2064 662c 2070             df, p
-00002070: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
-00002080: 7465 203d 2073 656c 662e 5f6d 616b 655f  te = self._make_
-00002090: 7375 7065 725f 7072 6f74 6563 7465 6428  super_protected(
-000020a0: 6461 7461 7365 742c 2070 726f 7465 6374  dataset, protect
-000020b0: 6564 5f61 7474 7269 6275 7465 7329 0d0a  ed_attributes)..
-000020c0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000020d0: 2020 6966 2073 656c 662e 6d65 7468 6f64    if self.method
-000020e0: 2069 6e20 5b22 534d 4f54 454e 4322 5d20   in ["SMOTENC"] 
-000020f0: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
-00002100: 7072 6f63 6573 730d 0a20 2020 2020 2020  process..       
-00002110: 2020 2020 2070 726f 6365 7373 6f72 203d       processor =
-00002120: 2050 726f 6365 7373 6f72 2829 0d0a 2020   Processor()..  
-00002130: 2020 2020 2020 2020 2020 7072 6f63 6573            proces
-00002140: 7365 645f 6466 3d20 7072 6f63 6573 736f  sed_df= processo
-00002150: 722e 7072 6f63 6573 7328 6466 2c20 7363  r.process(df, sc
-00002160: 616c 655f 636f 6c73 3d63 6f6e 745f 636f  ale_cols=cont_co
-00002170: 6c75 6d6e 732c 2065 6e63 6f64 655f 636f  lumns, encode_co
-00002180: 6c73 3d63 6174 5f63 6f6c 756d 6e73 290d  ls=cat_columns).
-00002190: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
-000021a0: 2054 6865 6e20 7265 7361 6d70 6c65 0d0a   Then resample..
-000021b0: 2020 2020 2020 2020 2020 2020 6361 745f              cat_
-000021c0: 636f 6c75 6d6e 735f 6964 7320 3d20 5b70  columns_ids = [p
-000021d0: 726f 6365 7373 6564 5f64 662e 636f 6c75  rocessed_df.colu
-000021e0: 6d6e 732e 6765 745f 6c6f 6328 636f 6c5f  mns.get_loc(col_
-000021f0: 6e61 6d65 2920 666f 7220 636f 6c5f 6e61  name) for col_na
-00002200: 6d65 2069 6e20 6361 745f 636f 6c75 6d6e  me in cat_column
-00002210: 735d 0d0a 2020 2020 2020 2020 2020 2020  s]..            
-00002220: 7361 6d70 6c65 7220 3d20 7365 6c66 2e6d  sampler = self.m
-00002230: 6974 6967 6174 6f72 5f66 756e 6374 696f  itigator_functio
-00002240: 6e5b 7365 6c66 2e6d 6574 686f 645d 2863  n[self.method](c
-00002250: 6174 5f63 6f6c 756d 6e73 5f69 6473 290d  at_columns_ids).
-00002260: 0a20 2020 2020 2020 2020 2020 2058 5f72  .            X_r
-00002270: 6573 616d 706c 6564 2c20 795f 7265 7361  esampled, y_resa
-00002280: 6d70 6c65 6420 3d20 7361 6d70 6c65 722e  mpled = sampler.
-00002290: 6669 745f 7265 7361 6d70 6c65 2870 726f  fit_resample(pro
-000022a0: 6365 7373 6564 5f64 662c 2074 6172 6765  cessed_df, targe
-000022b0: 745f 6466 290d 0a20 2020 2020 2020 2020  t_df)..         
-000022c0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000022d0: 2023 2054 6865 6e20 756e 7072 6f63 6573   # Then unproces
-000022e0: 7320 6974 0d0a 2020 2020 2020 2020 2020  s it..          
-000022f0: 2020 6466 5f66 696e 616c 203d 2070 726f    df_final = pro
-00002300: 6365 7373 6f72 2e75 6e70 726f 6365 7373  cessor.unprocess
-00002310: 2858 5f72 6573 616d 706c 6564 290d 0a20  (X_resampled).. 
-00002320: 2020 2020 2020 2020 2020 2074 6172 6765             targe
-00002330: 745f 6669 6e61 6c20 3d20 795f 7265 7361  t_final = y_resa
-00002340: 6d70 6c65 640d 0a0d 0a20 2020 2020 2020  mpled....       
-00002350: 2065 6c73 6520 3a0d 0a20 2020 2020 2020   else :..       
-00002360: 2020 2020 2023 6a75 7374 2072 6573 616d       #just resam
-00002370: 706c 6572 0d0a 2020 2020 2020 2020 2020  pler..          
-00002380: 2020 7361 6d70 6c65 7220 3d20 7365 6c66    sampler = self
-00002390: 2e6d 6974 6967 6174 6f72 5f66 756e 6374  .mitigator_funct
-000023a0: 696f 6e5b 7365 6c66 2e6d 6574 686f 645d  ion[self.method]
-000023b0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-000023c0: 6466 5f66 696e 616c 2c20 7461 7267 6574  df_final, target
-000023d0: 5f66 696e 616c 203d 2073 616d 706c 6572  _final = sampler
-000023e0: 2e66 6974 5f72 6573 616d 706c 6528 6466  .fit_resample(df
-000023f0: 2c20 7461 7267 6574 5f64 6629 0d0a 2020  , target_df)..  
-00002400: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00002410: 6966 2070 726f 7465 6374 6564 5f61 7474  if protected_att
-00002420: 7269 6275 7465 7320 616e 6420 6c65 6e28  ributes and len(
-00002430: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
-00002440: 7574 6573 2920 3e20 3120 3a0d 0a20 2020  utes) > 1 :..   
-00002450: 2020 2020 2020 2020 2064 665f 6669 6e61           df_fina
-00002460: 6c20 3d20 6466 5f66 696e 616c 2e64 726f  l = df_final.dro
-00002470: 7028 636f 6c75 6d6e 7320 3d20 7072 6f74  p(columns = prot
-00002480: 6563 7465 645f 6174 7472 6962 7574 6529  ected_attribute)
-00002490: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-000024a0: 2020 2020 7265 7475 726e 2064 665f 6669      return df_fi
-000024b0: 6e61 6c2c 2074 6172 6765 745f 6669 6e61  nal, target_fina
-000024c0: 6c0d 0a20 2020 2020 2020 2020 2020 200d  l..            .
-000024d0: 0a20 2020 2064 6566 2062 616c 616e 6365  .    def balance
-000024e0: 5f70 726f 7465 6374 6564 5f61 7474 7269  _protected_attri
-000024f0: 6275 7465 2873 656c 662c 2064 6174 6173  bute(self, datas
-00002500: 6574 3a20 7064 2e44 6174 6146 7261 6d65  et: pd.DataFrame
-00002510: 2c20 7461 7267 6574 3a20 7374 722c 2070  , target: str, p
-00002520: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
-00002530: 7465 733a 206c 6973 742c 200d 0a20 2020  tes: list, ..   
-00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002560: 2063 6f6e 745f 636f 6c75 6d6e 733a 206c   cont_columns: l
-00002570: 6973 7420 3d20 4e6f 6e65 2c20 6361 745f  ist = None, cat_
-00002580: 636f 6c75 6d6e 733a 206c 6973 7420 3d20  columns: list = 
-00002590: 4e6f 6e65 2920 3a0d 0a20 2020 2020 2020  None) :..       
-000025a0: 2022 2222 0d0a 2020 2020 2020 2020 4261   """..        Ba
-000025b0: 6c61 6e63 6520 7468 6520 636c 6173 7365  lance the classe
-000025c0: 7320 6f66 2061 2070 726f 7465 6374 6564  s of a protected
-000025d0: 2061 7474 7269 6275 7465 2077 6974 6820   attribute with 
-000025e0: 6e6f 2072 6567 6172 6473 2074 6f20 7468  no regards to th
-000025f0: 6520 6f75 7470 7574 2e20 5c6e 0d0a 2020  e output. \n..  
-00002600: 2020 2020 2020 5368 6f75 6c64 2069 6d70        Should imp
-00002610: 726f 7665 2074 6865 2062 616c 616e 6365  rove the balance
-00002620: 2066 6f72 2074 6865 2070 726f 7465 6374   for the protect
-00002630: 6564 2061 7474 7269 6275 7465 2e0d 0a20  ed attribute... 
-00002640: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00002650: 2041 7267 733a 200d 0a20 2020 2020 2020   Args: ..       
-00002660: 2020 2020 2064 6174 6173 6574 2028 7064       dataset (pd
-00002670: 2e44 6174 6146 7261 6d65 293a 2064 6174  .DataFrame): dat
-00002680: 6173 6574 2074 6f20 6d69 7469 6761 7465  aset to mitigate
-00002690: 2c20 7468 6174 2069 6e63 6c75 6465 7320  , that includes 
-000026a0: 7468 6520 7461 7267 6574 2063 6f6c 756d  the target colum
-000026b0: 6e2e 0d0a 2020 2020 2020 2020 2020 2020  n...            
-000026c0: 7461 7267 6574 2028 7374 7229 3a20 7468  target (str): th
-000026d0: 6520 7461 7267 6574 2063 6f6c 756d 6e20  e target column 
-000026e0: 6e61 6d65 0d0a 2020 2020 2020 2020 2020  name..          
-000026f0: 2020 7072 6f74 6563 7465 645f 6174 7472    protected_attr
-00002700: 6962 7574 6573 2028 6c69 7374 2c20 6f70  ibutes (list, op
-00002710: 7469 6f6e 616c 293a 2054 6865 2061 7474  tional): The att
-00002720: 7269 6275 7465 2873 2920 746f 2062 616c  ribute(s) to bal
-00002730: 616e 6365 2e20 4465 6661 756c 7473 2074  ance. Defaults t
-00002740: 6f20 4e6f 6e65 2e0d 0a20 2020 2020 2020  o None...       
-00002750: 2020 2020 2063 6f6e 745f 636f 6c75 6d6e       cont_column
-00002760: 7320 286c 6973 742c 206f 7074 696f 6e61  s (list, optiona
-00002770: 6c29 3a20 5468 6520 636f 6e74 696e 756f  l): The continuo
-00002780: 7573 2063 6f6c 756d 6e73 2069 6e20 7468  us columns in th
-00002790: 6520 6461 7461 7365 742e 204f 6e6c 7920  e dataset. Only 
-000027a0: 4e65 6365 7373 6172 7920 6966 2074 6865  Necessary if the
-000027b0: 2073 616d 706c 696e 6720 7374 7261 7465   sampling strate
-000027c0: 6779 2069 7320 534d 4f54 454e 432e 2044  gy is SMOTENC. D
-000027d0: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
-000027e0: 0d0a 2020 2020 2020 2020 2020 2020 6361  ..            ca
-000027f0: 745f 636f 6c75 6d6e 7320 286c 6973 742c  t_columns (list,
-00002800: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
-00002810: 6361 7465 676f 7269 6361 6c20 636f 6c75  categorical colu
-00002820: 6d6e 7320 696e 2074 6865 2064 6174 6173  mns in the datas
-00002830: 6574 2e20 4f6e 6c79 204e 6563 6573 7361  et. Only Necessa
-00002840: 7279 2069 6620 7468 6520 7361 6d70 6c69  ry if the sampli
-00002850: 6e67 2073 7472 6174 6567 7920 6973 2053  ng strategy is S
-00002860: 4d4f 5445 4e43 2e20 4465 6661 756c 7473  MOTENC. Defaults
-00002870: 2074 6f20 4e6f 6e65 2e0d 0a0d 0a20 2020   to None.....   
-00002880: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
-00002890: 2020 2020 2020 2020 2020 2028 5b70 642e             ([pd.
-000028a0: 4461 7461 4672 616d 652c 2070 642e 4461  DataFrame, pd.Da
-000028b0: 7461 4672 616d 655d 293a 2074 6865 2062  taFrame]): the b
-000028c0: 616c 616e 6365 6420 6461 7461 6672 616d  alanced datafram
-000028d0: 6573 2066 6f72 2074 6865 2064 6174 6173  es for the datas
-000028e0: 6574 2061 6e64 2074 6865 2074 6172 6765  et and the targe
-000028f0: 740d 0a20 2020 2020 2020 2022 2222 0d0a  t..        """..
-00002900: 2020 2020 2020 2020 7375 7065 7228 292e          super().
-00002910: 5f73 616e 6974 795f 6368 6563 6b28 6461  _sanity_check(da
-00002920: 7461 7365 742c 2074 6172 6765 742c 2070  taset, target, p
-00002930: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
-00002940: 7465 733d 7072 6f74 6563 7465 645f 6174  tes=protected_at
-00002950: 7472 6962 7574 6573 290d 0a20 2020 2020  tributes)..     
-00002960: 2020 2064 6620 3d20 6461 7461 7365 742e     df = dataset.
-00002970: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
-00002980: 7461 7267 6574 5f64 6620 3d20 6466 5b74  target_df = df[t
-00002990: 6172 6765 745d 0d0a 2020 2020 2020 2020  arget]..        
-000029a0: 6466 203d 2064 662e 6472 6f70 2863 6f6c  df = df.drop(col
-000029b0: 756d 6e73 3d74 6172 6765 7429 0d0a 0d0a  umns=target)....
-000029c0: 2020 2020 2020 2020 6966 206c 656e 2870          if len(p
-000029d0: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
-000029e0: 7465 7329 203e 2031 203a 0d0a 2020 2020  tes) > 1 :..    
-000029f0: 2020 2020 2020 2020 6466 2c20 7072 6f74          df, prot
-00002a00: 6563 7465 645f 6174 7472 6962 7574 6520  ected_attribute 
-00002a10: 3d20 7365 6c66 2e5f 6d61 6b65 5f73 7570  = self._make_sup
-00002a20: 6572 5f70 726f 7465 6374 6564 2864 6174  er_protected(dat
-00002a30: 6173 6574 2c20 7072 6f74 6563 7465 645f  aset, protected_
-00002a40: 6174 7472 6962 7574 6573 290d 0a20 2020  attributes)..   
-00002a50: 2020 2020 2065 6c73 6520 3a0d 0a20 2020       else :..   
-00002a60: 2020 2020 2020 2020 2070 726f 7465 6374           protect
-00002a70: 6564 5f61 7474 7269 6275 7465 203d 2070  ed_attribute = p
-00002a80: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
-00002a90: 7465 735b 305d 0d0a 0d0a 2020 2020 2020  tes[0]....      
-00002aa0: 2020 6966 2073 656c 662e 6d65 7468 6f64    if self.method
-00002ab0: 2069 6e20 5b22 534d 4f54 454e 4322 5d20   in ["SMOTENC"] 
-00002ac0: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
-00002ad0: 7072 6570 726f 6365 7373 2075 7369 6e67  preprocess using
-00002ae0: 2074 6865 2070 726f 7465 6374 6564 2061   the protected a
-00002af0: 7474 7269 6275 7465 2061 7320 6120 7461  ttribute as a ta
-00002b00: 7267 6574 0d0a 2020 2020 2020 2020 2020  rget..          
-00002b10: 2020 636f 6e74 5f63 6f6c 5f62 7566 6620    cont_col_buff 
-00002b20: 3d20 5b66 6561 7475 7265 2066 6f72 2066  = [feature for f
-00002b30: 6561 7475 7265 2069 6e20 636f 6e74 5f63  eature in cont_c
-00002b40: 6f6c 756d 6e73 2069 6620 6665 6174 7572  olumns if featur
-00002b50: 6520 213d 2070 726f 7465 6374 6564 5f61  e != protected_a
-00002b60: 7474 7269 6275 7465 5d0d 0a20 2020 2020  ttribute]..     
-00002b70: 2020 2020 2020 2063 6174 5f63 6f6c 5f62         cat_col_b
-00002b80: 7566 6620 3d20 5b66 6561 7475 7265 2066  uff = [feature f
-00002b90: 6f72 2066 6561 7475 7265 2069 6e20 6361  or feature in ca
-00002ba0: 745f 636f 6c75 6d6e 7320 6966 2066 6561  t_columns if fea
-00002bb0: 7475 7265 2021 3d20 7072 6f74 6563 7465  ture != protecte
-00002bc0: 645f 6174 7472 6962 7574 655d 0d0a 2020  d_attribute]..  
-00002bd0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00002be0: 2020 2020 2020 2020 7072 6f63 6573 736f          processo
-00002bf0: 7220 3d20 5072 6f63 6573 736f 7228 290d  r = Processor().
-00002c00: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-00002c10: 2020 2020 2020 2020 2020 2070 726f 6365             proce
-00002c20: 7373 6564 5f64 6620 3d20 7072 6f63 6573  ssed_df = proces
-00002c30: 736f 722e 7072 6f63 6573 7328 6466 2c20  sor.process(df, 
-00002c40: 7363 616c 655f 636f 6c73 3d63 6f6e 745f  scale_cols=cont_
-00002c50: 636f 6c5f 6275 6666 2c20 656e 636f 6465  col_buff, encode
-00002c60: 5f63 6f6c 733d 2863 6174 5f63 6f6c 5f62  _cols=(cat_col_b
-00002c70: 7566 6620 2b20 5b70 726f 7465 6374 6564  uff + [protected
-00002c80: 5f61 7474 7269 6275 7465 5d29 290d 0a0d  _attribute]))...
-00002c90: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00002ca0: 7465 6374 6564 5f61 7474 7269 6275 7465  tected_attribute
-00002cb0: 5f63 6f6c 756d 6e20 3d20 7072 6f63 6573  _column = proces
-00002cc0: 7365 645f 6466 5b70 726f 7465 6374 6564  sed_df[protected
-00002cd0: 5f61 7474 7269 6275 7465 5d0d 0a20 2020  _attribute]..   
-00002ce0: 2020 2020 2020 2020 2070 726f 6365 7373           process
-00002cf0: 6564 5f64 662e 6472 6f70 2863 6f6c 756d  ed_df.drop(colum
-00002d00: 6e73 203d 205b 7072 6f74 6563 7465 645f  ns = [protected_
-00002d10: 6174 7472 6962 7574 655d 2c20 696e 706c  attribute], inpl
-00002d20: 6163 6520 3d20 5472 7565 290d 0a20 2020  ace = True)..   
-00002d30: 2020 2020 2020 2020 2070 726f 6365 7373           process
-00002d40: 6564 5f64 662e 6c6f 635b 3a2c 7461 7267  ed_df.loc[:,targ
-00002d50: 6574 5d20 3d20 7461 7267 6574 5f64 660d  et] = target_df.
-00002d60: 0a0d 0a20 2020 2020 2020 2020 2020 2063  ...            c
-00002d70: 6174 5f63 6f6c 756d 6e5f 6275 6666 203d  at_column_buff =
-00002d80: 2063 6174 5f63 6f6c 5f62 7566 662e 636f   cat_col_buff.co
-00002d90: 7079 2829 0d0a 2020 2020 2020 2020 2020  py()..          
-00002da0: 2020 6361 745f 636f 6c75 6d6e 5f62 7566    cat_column_buf
-00002db0: 662e 6170 7065 6e64 2874 6172 6765 7429  f.append(target)
-00002dc0: 0d0a 2020 2020 2020 2020 2020 2020 6361  ..            ca
-00002dd0: 745f 636f 6c75 6d6e 5f69 6473 203d 205b  t_column_ids = [
-00002de0: 7072 6f63 6573 7365 645f 6466 2e63 6f6c  processed_df.col
-00002df0: 756d 6e73 2e67 6574 5f6c 6f63 2863 6f6c  umns.get_loc(col
-00002e00: 5f6e 616d 6529 2066 6f72 2063 6f6c 5f6e  _name) for col_n
-00002e10: 616d 6520 696e 2063 6174 5f63 6f6c 756d  ame in cat_colum
-00002e20: 6e5f 6275 6666 5d0d 0a0d 0a20 2020 2020  n_buff]....     
-00002e30: 2020 2020 2020 2073 616d 706c 6572 203d         sampler =
-00002e40: 2073 656c 662e 6d69 7469 6761 746f 725f   self.mitigator_
-00002e50: 6675 6e63 7469 6f6e 5b73 656c 662e 6d65  function[self.me
-00002e60: 7468 6f64 5d28 6361 7465 676f 7269 6361  thod](categorica
-00002e70: 6c5f 6665 6174 7572 6573 3d63 6174 5f63  l_features=cat_c
-00002e80: 6f6c 756d 6e5f 6964 7329 0d0a 0d0a 2020  olumn_ids)....  
-00002e90: 2020 2020 2020 2020 2020 585f 7265 7361            X_resa
-00002ea0: 6d70 6c65 642c 2061 7474 7269 6275 7465  mpled, attribute
-00002eb0: 5f72 6573 616d 706c 6564 203d 2073 616d  _resampled = sam
-00002ec0: 706c 6572 2e66 6974 5f72 6573 616d 706c  pler.fit_resampl
-00002ed0: 6528 7072 6f63 6573 7365 645f 6466 2c20  e(processed_df, 
-00002ee0: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
-00002ef0: 7574 655f 636f 6c75 6d6e 290d 0a20 2020  ute_column)..   
-00002f00: 2020 2020 2020 2020 2058 5f72 6573 616d           X_resam
-00002f10: 706c 6564 2e6c 6f63 5b3a 2c20 7072 6f74  pled.loc[:, prot
-00002f20: 6563 7465 645f 6174 7472 6962 7574 655d  ected_attribute]
-00002f30: 203d 2061 7474 7269 6275 7465 5f72 6573   = attribute_res
-00002f40: 616d 706c 6564 0d0a 2020 2020 2020 2020  ampled..        
-00002f50: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00002f60: 2064 665f 6669 6e61 6c20 3d20 7072 6f63   df_final = proc
-00002f70: 6573 736f 722e 756e 7072 6f63 6573 7328  essor.unprocess(
-00002f80: 585f 7265 7361 6d70 6c65 6429 0d0a 2020  X_resampled)..  
-00002f90: 2020 2020 2020 2020 2020 7461 7267 6574            target
-00002fa0: 5f66 696e 616c 203d 2064 665f 6669 6e61  _final = df_fina
-00002fb0: 6c5b 7461 7267 6574 5d0d 0a20 2020 2020  l[target]..     
-00002fc0: 2020 2020 2020 2064 665f 6669 6e61 6c2e         df_final.
-00002fd0: 6472 6f70 2863 6f6c 756d 6e73 3d5b 7461  drop(columns=[ta
-00002fe0: 7267 6574 5d2c 2069 6e70 6c61 6365 3d54  rget], inplace=T
-00002ff0: 7275 6529 0d0a 0d0a 2020 2020 2020 2020  rue)....        
-00003000: 656c 7365 203a 200d 0a20 2020 2020 2020  else : ..       
-00003010: 2020 2020 2070 726f 7465 6374 6564 5f61       protected_a
-00003020: 7474 7269 6275 7465 5f63 6f6c 756d 6e20  ttribute_column 
-00003030: 3d20 6466 5b70 726f 7465 6374 6564 5f61  = df[protected_a
-00003040: 7474 7269 6275 7465 5d0d 0a20 2020 2020  ttribute]..     
-00003050: 2020 2020 2020 2064 662e 6472 6f70 2863         df.drop(c
-00003060: 6f6c 756d 6e73 203d 205b 7072 6f74 6563  olumns = [protec
-00003070: 7465 645f 6174 7472 6962 7574 655d 2c20  ted_attribute], 
-00003080: 696e 706c 6163 6520 3d20 5472 7565 290d  inplace = True).
-00003090: 0a20 2020 2020 2020 2020 2020 2064 662e  .            df.
-000030a0: 6c6f 635b 3a2c 7461 7267 6574 5d20 3d20  loc[:,target] = 
-000030b0: 7461 7267 6574 5f64 660d 0a0d 0a20 2020  target_df....   
-000030c0: 2020 2020 2020 2020 2073 616d 706c 6572           sampler
-000030d0: 203d 2073 656c 662e 6d69 7469 6761 746f   = self.mitigato
-000030e0: 725f 6675 6e63 7469 6f6e 5b73 656c 662e  r_function[self.
-000030f0: 6d65 7468 6f64 5d28 290d 0a20 2020 2020  method]()..     
-00003100: 2020 2020 2020 2058 5f72 6573 616d 706c         X_resampl
-00003110: 6564 2c20 6174 7472 6962 7574 655f 7265  ed, attribute_re
-00003120: 7361 6d70 6c65 6420 3d20 7361 6d70 6c65  sampled = sample
-00003130: 722e 6669 745f 7265 7361 6d70 6c65 2864  r.fit_resample(d
-00003140: 662c 2070 726f 7465 6374 6564 5f61 7474  f, protected_att
-00003150: 7269 6275 7465 5f63 6f6c 756d 6e29 0d0a  ribute_column)..
-00003160: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00003170: 2020 2020 2020 2020 2020 585f 7265 7361            X_resa
-00003180: 6d70 6c65 642e 6c6f 635b 3a2c 2070 726f  mpled.loc[:, pro
-00003190: 7465 6374 6564 5f61 7474 7269 6275 7465  tected_attribute
-000031a0: 5d20 3d20 6174 7472 6962 7574 655f 7265  ] = attribute_re
-000031b0: 7361 6d70 6c65 640d 0a20 2020 2020 2020  sampled..       
-000031c0: 2020 2020 2074 6172 6765 745f 6669 6e61       target_fina
-000031d0: 6c20 3d20 585f 7265 7361 6d70 6c65 645b  l = X_resampled[
-000031e0: 7461 7267 6574 5d0d 0a20 2020 2020 2020  target]..       
-000031f0: 2020 2020 2064 665f 6669 6e61 6c20 3d20       df_final = 
-00003200: 585f 7265 7361 6d70 6c65 642e 6472 6f70  X_resampled.drop
-00003210: 2863 6f6c 756d 6e73 3d5b 7461 7267 6574  (columns=[target
-00003220: 5d29 0d0a 2020 2020 2020 2020 0d0a 2020  ])..        ..  
-00003230: 2020 2020 2020 6966 206c 656e 2870 726f        if len(pro
-00003240: 7465 6374 6564 5f61 7474 7269 6275 7465  tected_attribute
-00003250: 7329 203e 2031 203a 0d0a 2020 2020 2020  s) > 1 :..      
-00003260: 2020 2020 2020 6466 5f66 696e 616c 203d        df_final =
-00003270: 2064 665f 6669 6e61 6c2e 6472 6f70 2863   df_final.drop(c
-00003280: 6f6c 756d 6e73 203d 2070 726f 7465 6374  olumns = protect
-00003290: 6564 5f61 7474 7269 6275 7465 2920 2020  ed_attribute)   
-000032a0: 200d 0a20 2020 200d 0a20 2020 2020 2020   ..    ..       
-000032b0: 2072 6574 7572 6e20 6466 5f66 696e 616c   return df_final
-000032c0: 2c20 7461 7267 6574 5f66 696e 616c 0d0a  , target_final..
-000032d0: 2020 2020 0d0a 2020 2020 6465 6620 6261      ..    def ba
-000032e0: 6c61 6e63 655f 6f75 7470 7574 5f66 6f72  lance_output_for
-000032f0: 5f61 7474 7269 6275 7465 2873 656c 662c  _attribute(self,
-00003300: 2064 6174 6173 6574 3a20 7064 2e44 6174   dataset: pd.Dat
-00003310: 6146 7261 6d65 2c20 7461 7267 6574 3a20  aFrame, target: 
-00003320: 7374 722c 2070 726f 7465 6374 6564 5f61  str, protected_a
-00003330: 7474 7269 6275 7465 733a 206c 6973 742c  ttributes: list,
-00003340: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00003350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003360: 2020 2020 2020 2020 636f 6e74 5f63 6f6c          cont_col
-00003370: 756d 6e73 3a20 6c69 7374 203d 204e 6f6e  umns: list = Non
-00003380: 652c 2063 6174 5f63 6f6c 756d 6e73 3a20  e, cat_columns: 
-00003390: 6c69 7374 203d 204e 6f6e 6529 203a 0d0a  list = None) :..
-000033a0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-000033b0: 2020 2020 2042 616c 616e 6365 2074 6865       Balance the
-000033c0: 206f 7574 7075 7420 6f66 2074 6865 2063   output of the c
-000033d0: 6c61 7373 6573 2066 6f72 2061 2067 6976  lasses for a giv
-000033e0: 656e 2070 726f 7465 6374 6564 2061 7474  en protected att
-000033f0: 7269 6275 7465 2e20 5c6e 0d0a 2020 2020  ribute. \n..    
-00003400: 2020 2020 5368 6f75 6c64 2069 6d70 726f      Should impro
-00003410: 7665 2074 6865 2044 4952 2066 6f72 2074  ve the DIR for t
-00003420: 6865 2070 726f 7465 6374 6564 2061 7474  he protected att
-00003430: 7269 6275 7465 2e0d 0a20 2020 2020 2020  ribute...       
-00003440: 200d 0a20 2020 2020 2020 2041 7267 733a   ..        Args:
-00003450: 200d 0a20 2020 2020 2020 2020 2020 2064   ..            d
-00003460: 6174 6173 6574 2028 7064 2e44 6174 6146  ataset (pd.DataF
-00003470: 7261 6d65 293a 2064 6174 6173 6574 2074  rame): dataset t
-00003480: 6f20 6d69 7469 6761 7465 2c20 7468 6174  o mitigate, that
-00003490: 2069 6e63 6c75 6465 7320 7468 6520 7461   includes the ta
-000034a0: 7267 6574 2063 6f6c 756d 6e2e 0d0a 2020  rget column...  
-000034b0: 2020 2020 2020 2020 2020 7461 7267 6574            target
-000034c0: 2028 7374 7229 3a20 7468 6520 7461 7267   (str): the targ
-000034d0: 6574 2063 6f6c 756d 6e20 6e61 6d65 0d0a  et column name..
-000034e0: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
-000034f0: 6563 7465 645f 6174 7472 6962 7574 6573  ected_attributes
-00003500: 2028 6c69 7374 2c20 6f70 7469 6f6e 616c   (list, optional
-00003510: 293a 2054 6865 2061 7474 7269 6275 7465  ): The attribute
-00003520: 2873 2920 746f 2062 616c 616e 6365 2e20  (s) to balance. 
-00003530: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
-00003540: 2e0d 0a20 2020 2020 2020 2020 2020 2063  ...            c
-00003550: 6f6e 745f 636f 6c75 6d6e 7320 286c 6973  ont_columns (lis
-00003560: 742c 206f 7074 696f 6e61 6c29 3a20 5468  t, optional): Th
-00003570: 6520 636f 6e74 696e 756f 7573 2063 6f6c  e continuous col
-00003580: 756d 6e73 2069 6e20 7468 6520 6461 7461  umns in the data
-00003590: 7365 742e 204f 6e6c 7920 4e65 6365 7373  set. Only Necess
-000035a0: 6172 7920 6966 2074 6865 2073 616d 706c  ary if the sampl
-000035b0: 696e 6720 7374 7261 7465 6779 2069 7320  ing strategy is 
-000035c0: 534d 4f54 454e 432e 2044 6566 6175 6c74  SMOTENC. Default
-000035d0: 7320 746f 204e 6f6e 652e 0d0a 2020 2020  s to None...    
-000035e0: 2020 2020 2020 2020 6361 745f 636f 6c75          cat_colu
-000035f0: 6d6e 7320 286c 6973 742c 206f 7074 696f  mns (list, optio
-00003600: 6e61 6c29 3a20 5468 6520 6361 7465 676f  nal): The catego
-00003610: 7269 6361 6c20 636f 6c75 6d6e 7320 696e  rical columns in
-00003620: 2074 6865 2064 6174 6173 6574 2e20 4f6e   the dataset. On
-00003630: 6c79 204e 6563 6573 7361 7279 2069 6620  ly Necessary if 
-00003640: 7468 6520 7361 6d70 6c69 6e67 2073 7472  the sampling str
-00003650: 6174 6567 7920 6973 2053 4d4f 5445 4e43  ategy is SMOTENC
-00003660: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
-00003670: 6e65 2e0d 0a0d 0a20 2020 2020 2020 2052  ne.....        R
-00003680: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-00003690: 2020 2020 2028 5b70 642e 4461 7461 4672       ([pd.DataFr
-000036a0: 616d 652c 2070 642e 4461 7461 4672 616d  ame, pd.DataFram
-000036b0: 655d 293a 2074 6865 2062 616c 616e 6365  e]): the balance
-000036c0: 6420 6461 7461 6672 616d 6573 2066 6f72  d dataframes for
-000036d0: 2074 6865 2064 6174 6173 6574 2061 6e64   the dataset and
-000036e0: 2074 6865 2074 6172 6765 740d 0a20 2020   the target..   
-000036f0: 2020 2020 2022 2222 0d0a 0d0a 2020 2020       """....    
-00003700: 2020 2020 7375 7065 7228 292e 5f73 616e      super()._san
-00003710: 6974 795f 6368 6563 6b28 6461 7461 7365  ity_check(datase
-00003720: 742c 2074 6172 6765 742c 2070 726f 7465  t, target, prote
-00003730: 6374 6564 5f61 7474 7269 6275 7465 733d  cted_attributes=
-00003740: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
-00003750: 7574 6573 290d 0a20 2020 2020 2020 2064  utes)..        d
-00003760: 6620 3d20 6461 7461 7365 742e 636f 7079  f = dataset.copy
-00003770: 2829 0d0a 0d0a 2020 2020 2020 2020 0d0a  ()....        ..
-00003780: 2020 2020 2020 2020 6966 206c 656e 2870          if len(p
-00003790: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
-000037a0: 7465 7329 203e 2031 203a 0d0a 2020 2020  tes) > 1 :..    
-000037b0: 2020 2020 2020 2020 6466 2c20 7072 6f74          df, prot
-000037c0: 6563 7465 645f 6174 7472 6962 7574 6520  ected_attribute 
-000037d0: 3d20 7365 6c66 2e5f 6d61 6b65 5f73 7570  = self._make_sup
-000037e0: 6572 5f70 726f 7465 6374 6564 2864 6174  er_protected(dat
-000037f0: 6173 6574 2c20 7072 6f74 6563 7465 645f  aset, protected_
-00003800: 6174 7472 6962 7574 6573 290d 0a20 2020  attributes)..   
-00003810: 2020 2020 2065 6c73 6520 3a0d 0a20 2020       else :..   
-00003820: 2020 2020 2020 2020 2070 726f 7465 6374           protect
-00003830: 6564 5f61 7474 7269 6275 7465 203d 2070  ed_attribute = p
-00003840: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
-00003850: 7465 735b 305d 0d0a 2020 2020 0d0a 2020  tes[0]..    ..  
-00003860: 2020 2020 2020 636c 6173 7365 7320 3d20        classes = 
-00003870: 6c69 7374 2864 665b 7072 6f74 6563 7465  list(df[protecte
-00003880: 645f 6174 7472 6962 7574 655d 2e75 6e69  d_attribute].uni
-00003890: 7175 6528 2929 0d0a 2020 2020 2020 2020  que())..        
-000038a0: 722c 206d 6178 5f63 6c61 7373 203d 2073  r, max_class = s
-000038b0: 656c 662e 5f68 6967 6865 7374 5f72 6174  elf._highest_rat
-000038c0: 696f 2864 662c 2074 6172 6765 742c 2063  io(df, target, c
-000038d0: 6c61 7373 6573 2c20 7072 6f74 6563 7465  lasses, protecte
-000038e0: 645f 6174 7472 6962 7574 6529 0d0a 2020  d_attribute)..  
-000038f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00003900: 666f 7220 6320 696e 2063 6c61 7373 6573  for c in classes
-00003910: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
-00003920: 6966 2063 2021 3d20 6d61 785f 636c 6173  if c != max_clas
-00003930: 7320 3a0d 0a20 2020 2020 2020 2020 2020  s :..           
-00003940: 2020 2020 2023 206b 6565 7020 6f6e 6c79       # keep only
-00003950: 2074 6865 2072 6f77 7320 7769 7468 2067   the rows with g
-00003960: 6976 656e 2063 6c61 7373 0d0a 2020 2020  iven class..    
-00003970: 2020 2020 2020 2020 2020 2020 636c 6173              clas
-00003980: 735f 6466 203d 2064 665b 6466 5b70 726f  s_df = df[df[pro
-00003990: 7465 6374 6564 5f61 7474 7269 6275 7465  tected_attribute
-000039a0: 5d20 3d3d 2063 5d0d 0a20 2020 2020 2020  ] == c]..       
-000039b0: 2020 2020 2020 2020 2063 6c61 7373 5f74           class_t
-000039c0: 6172 6765 7420 3d20 636c 6173 735f 6466  arget = class_df
-000039d0: 5b74 6172 6765 745d 0d0a 2020 2020 2020  [target]..      
-000039e0: 2020 2020 2020 2020 2020 636c 6173 735f            class_
-000039f0: 6466 203d 2063 6c61 7373 5f64 662e 6472  df = class_df.dr
-00003a00: 6f70 2863 6f6c 756d 6e73 3d5b 7461 7267  op(columns=[targ
-00003a10: 6574 5d29 0d0a 2020 2020 2020 2020 2020  et])..          
-00003a20: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00003a30: 2020 2020 2320 7265 7361 6d70 6c65 2074      # resample t
-00003a40: 6865 2074 6172 6765 7420 666f 7220 7468  he target for th
-00003a50: 6973 2063 6c61 7373 0d0a 2020 2020 2020  is class..      
-00003a60: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-00003a70: 286c 6973 7428 636c 6173 735f 7461 7267  (list(class_targ
-00003a80: 6574 2e75 6e69 7175 6528 2929 2920 213d  et.unique())) !=
-00003a90: 2031 203a 0d0a 2020 2020 2020 2020 2020   1 :..          
-00003aa0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00003ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ac0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003ad0: 2020 2020 2020 6966 2073 656c 662e 6d65        if self.me
-00003ae0: 7468 6f64 2069 6e20 5b22 534d 4f54 454e  thod in ["SMOTEN
-00003af0: 4322 5d20 3a0d 0a20 2020 2020 2020 2020  C"] :..         
-00003b00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00003b10: 6f6e 745f 636f 6c5f 6275 6666 203d 205b  ont_col_buff = [
-00003b20: 6665 6174 7572 6520 666f 7220 6665 6174  feature for feat
-00003b30: 7572 6520 696e 2063 6f6e 745f 636f 6c75  ure in cont_colu
-00003b40: 6d6e 7320 6966 2066 6561 7475 7265 2021  mns if feature !
-00003b50: 3d20 7072 6f74 6563 7465 645f 6174 7472  = protected_attr
-00003b60: 6962 7574 655d 0d0a 2020 2020 2020 2020  ibute]..        
-00003b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b80: 6361 745f 636f 6c5f 6275 6666 203d 205b  cat_col_buff = [
-00003b90: 6665 6174 7572 6520 666f 7220 6665 6174  feature for feat
-00003ba0: 7572 6520 696e 2063 6174 5f63 6f6c 756d  ure in cat_colum
-00003bb0: 6e73 2069 6620 6665 6174 7572 6520 213d  ns if feature !=
-00003bc0: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
-00003bd0: 6275 7465 5d0d 0a20 2020 2020 2020 2020  bute]..         
-00003be0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00003bf0: 2020 2020 2020 2020 2020 2020 2023 7072               #pr
-00003c00: 6570 726f 6365 7373 2075 7369 6e67 2074  eprocess using t
-00003c10: 6865 2070 726f 7465 6374 6564 2061 7474  he protected att
-00003c20: 7269 6275 7465 2061 7320 6120 7461 7267  ribute as a targ
-00003c30: 6574 0d0a 2020 2020 2020 2020 2020 2020  et..            
-00003c40: 2020 2020 2020 2020 2020 2020 7072 6f63              proc
-00003c50: 6573 736f 7220 3d20 5072 6f63 6573 736f  essor = Processo
-00003c60: 7228 290d 0a20 2020 2020 2020 2020 2020  r()..           
-00003c70: 2020 2020 2020 2020 2020 2020 2070 726f               pro
-00003c80: 6365 7373 6564 5f64 6620 3d20 7072 6f63  cessed_df = proc
-00003c90: 6573 736f 722e 7072 6f63 6573 7328 636c  essor.process(cl
-00003ca0: 6173 735f 6466 2c20 7363 616c 655f 636f  ass_df, scale_co
-00003cb0: 6c73 3d63 6f6e 745f 636f 6c5f 6275 6666  ls=cont_col_buff
-00003cc0: 2c20 656e 636f 6465 5f63 6f6c 733d 2863  , encode_cols=(c
-00003cd0: 6174 5f63 6f6c 5f62 7566 6620 2b20 5b70  at_col_buff + [p
-00003ce0: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
-00003cf0: 7465 5d29 290d 0a0d 0a20 2020 2020 2020  te]))....       
-00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d10: 2063 6174 5f63 6f6c 756d 6e73 5f69 6473   cat_columns_ids
-00003d20: 203d 205b 7072 6f63 6573 7365 645f 6466   = [processed_df
-00003d30: 2e63 6f6c 756d 6e73 2e67 6574 5f6c 6f63  .columns.get_loc
-00003d40: 2863 6f6c 5f6e 616d 6529 2066 6f72 2063  (col_name) for c
-00003d50: 6f6c 5f6e 616d 6520 696e 2063 6174 5f63  ol_name in cat_c
-00003d60: 6f6c 756d 6e73 5d0d 0a20 2020 2020 2020  olumns]..       
-00003d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d80: 2073 616d 706c 6572 203d 2053 4d4f 5445   sampler = SMOTE
-00003d90: 4e43 2873 616d 706c 696e 675f 7374 7261  NC(sampling_stra
-00003da0: 7465 6779 3d72 2c20 6361 7465 676f 7269  tegy=r, categori
-00003db0: 6361 6c5f 6665 6174 7572 6573 3d63 6174  cal_features=cat
-00003dc0: 5f63 6f6c 756d 6e73 5f69 6473 290d 0a20  _columns_ids).. 
-00003dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003de0: 2020 2020 2020 2058 5f72 6573 616d 706c         X_resampl
-00003df0: 6564 2c20 636c 6173 735f 7461 7267 6574  ed, class_target
-00003e00: 5f72 6573 616d 706c 6564 203d 2073 616d  _resampled = sam
-00003e10: 706c 6572 2e66 6974 5f72 6573 616d 706c  pler.fit_resampl
-00003e20: 6528 7072 6f63 6573 7365 645f 6466 2c20  e(processed_df, 
-00003e30: 636c 6173 735f 7461 7267 6574 290d 0a20  class_target).. 
-00003e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e50: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00003e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e70: 2063 6c61 7373 5f72 6573 616d 706c 6564   class_resampled
-00003e80: 203d 2070 726f 6365 7373 6f72 2e75 6e70   = processor.unp
-00003e90: 726f 6365 7373 2858 5f72 6573 616d 706c  rocess(X_resampl
-00003ea0: 6564 290d 0a20 2020 2020 2020 2020 2020  ed)..           
-00003eb0: 2020 2020 2020 2020 2020 2020 2063 6c61               cla
-00003ec0: 7373 5f72 6573 616d 706c 6564 2e6c 6f63  ss_resampled.loc
-00003ed0: 5b3a 2c20 7461 7267 6574 5d20 3d20 636c  [:, target] = cl
-00003ee0: 6173 735f 7461 7267 6574 5f72 6573 616d  ass_target_resam
-00003ef0: 706c 6564 0d0a 2020 2020 2020 2020 2020  pled..          
-00003f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f10: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00003f20: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00003f30: 2073 656c 662e 6d65 7468 6f64 2069 6e20   self.method in 
-00003f40: 5b22 5261 6e64 6f6d 4f76 6572 5361 6d70  ["RandomOverSamp
-00003f50: 6c65 7222 5d20 3a0d 0a20 2020 2020 2020  ler"] :..       
-00003f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f70: 2073 616d 706c 6572 203d 2052 616e 646f   sampler = Rando
-00003f80: 6d4f 7665 7253 616d 706c 6572 2873 616d  mOverSampler(sam
-00003f90: 706c 696e 675f 7374 7261 7465 6779 3d72  pling_strategy=r
-00003fa0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00003fb0: 2020 2020 2020 2020 2020 2063 6c61 7373             class
-00003fc0: 5f72 6573 616d 706c 6564 2c20 636c 6173  _resampled, clas
-00003fd0: 735f 7461 7267 6574 5f72 6573 616d 706c  s_target_resampl
-00003fe0: 6564 203d 2073 616d 706c 6572 2e66 6974  ed = sampler.fit
-00003ff0: 5f72 6573 616d 706c 6528 636c 6173 735f  _resample(class_
-00004000: 6466 2c20 636c 6173 735f 7461 7267 6574  df, class_target
-00004010: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00004020: 2020 2020 2020 2020 2020 2063 6c61 7373             class
-00004030: 5f72 6573 616d 706c 6564 2e6c 6f63 5b3a  _resampled.loc[:
-00004040: 2c20 7461 7267 6574 5d20 3d20 636c 6173  , target] = clas
-00004050: 735f 7461 7267 6574 5f72 6573 616d 706c  s_target_resampl
-00004060: 6564 0d0a 2020 2020 2020 2020 2020 2020  ed..            
-00004070: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00004080: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00004090: 6966 2073 656c 662e 6d65 7468 6f64 2069  if self.method i
-000040a0: 6e20 5b22 5261 6e64 6f6d 556e 6465 7253  n ["RandomUnderS
-000040b0: 616d 706c 6572 225d 203a 0d0a 2020 2020  ampler"] :..    
-000040c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040d0: 2020 2020 7361 6d70 6c65 7220 3d20 5261      sampler = Ra
-000040e0: 6e64 6f6d 556e 6465 7253 616d 706c 6572  ndomUnderSampler
-000040f0: 2873 616d 706c 696e 675f 7374 7261 7465  (sampling_strate
-00004100: 6779 3d72 290d 0a20 2020 2020 2020 2020  gy=r)..         
-00004110: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00004120: 6c61 7373 5f72 6573 616d 706c 6564 2c20  lass_resampled, 
-00004130: 636c 6173 735f 7461 7267 6574 5f72 6573  class_target_res
-00004140: 616d 706c 6564 203d 2073 616d 706c 6572  ampled = sampler
-00004150: 2e66 6974 5f72 6573 616d 706c 6528 636c  .fit_resample(cl
-00004160: 6173 735f 6466 2c20 636c 6173 735f 7461  ass_df, class_ta
-00004170: 7267 6574 290d 0a20 2020 2020 2020 2020  rget)..         
-00004180: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00004190: 6c61 7373 5f72 6573 616d 706c 6564 2e6c  lass_resampled.l
-000041a0: 6f63 5b3a 2c20 7461 7267 6574 5d20 3d20  oc[:, target] = 
-000041b0: 636c 6173 735f 7461 7267 6574 5f72 6573  class_target_res
-000041c0: 616d 706c 6564 2020 2020 2020 0d0a 2020  ampled      ..  
-000041d0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000041e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041f0: 656c 7365 203a 0d0a 2020 2020 2020 2020  else :..        
-00004200: 2020 2020 2020 2020 2020 2020 2369 6620              #if 
-00004210: 7468 6572 6520 6973 206f 6e6c 7920 6f6e  there is only on
-00004220: 6520 6f75 7470 7574 2066 6f72 2074 6865  e output for the
-00004230: 2063 6c61 7373 2c20 7468 6572 6520 6973   class, there is
-00004240: 206e 6f20 7761 7920 746f 2072 6573 616d   no way to resam
-00004250: 706c 6520 6974 0d0a 2020 2020 2020 2020  ple it..        
-00004260: 2020 2020 2020 2020 2020 2020 636c 6173              clas
-00004270: 735f 7265 7361 6d70 6c65 6420 3d20 636c  s_resampled = cl
-00004280: 6173 735f 6466 2e63 6f70 7928 290d 0a20  ass_df.copy().. 
-00004290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042a0: 2020 2063 6c61 7373 5f72 6573 616d 706c     class_resampl
-000042b0: 6564 2e6c 6f63 5b3a 2c74 6172 6765 745d  ed.loc[:,target]
-000042c0: 203d 2063 6c61 7373 5f74 6172 6765 740d   = class_target.
-000042d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000042e0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000042f0: 2020 2020 2020 2023 2061 7070 656e 6420         # append 
-00004300: 7468 6520 7265 7361 6d70 6c65 6420 636c  the resampled cl
-00004310: 6173 7320 696e 2066 696e 616c 2064 660d  ass in final df.
-00004320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004330: 2023 2028 6472 6f70 2074 6865 2072 6f77   # (drop the row
-00004340: 7320 7769 7468 2074 6869 7320 636c 6173  s with this clas
-00004350: 7320 6669 7273 7420 746f 206e 6f74 2064  s first to not d
-00004360: 7570 6c69 6361 7465 6420 7468 656d 290d  uplicated them).
-00004370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004380: 2064 6620 3d20 6466 5b64 665b 7072 6f74   df = df[df[prot
-00004390: 6563 7465 645f 6174 7472 6962 7574 655d  ected_attribute]
-000043a0: 2021 3d20 635d 0d0a 2020 2020 2020 2020   != c]..        
-000043b0: 2020 2020 2020 2020 6466 203d 2070 642e          df = pd.
-000043c0: 636f 6e63 6174 285b 6466 2c20 636c 6173  concat([df, clas
-000043d0: 735f 7265 7361 6d70 6c65 645d 2c20 6967  s_resampled], ig
-000043e0: 6e6f 7265 5f69 6e64 6578 3d54 7275 6529  nore_index=True)
-000043f0: 0d0a 0d0a 0d0a 2020 2020 2020 2020 7461  ......        ta
-00004400: 7267 6574 5f64 6620 3d20 6466 5b74 6172  rget_df = df[tar
-00004410: 6765 745d 0d0a 2020 2020 2020 2020 6466  get]..        df
-00004420: 2e64 726f 7028 636f 6c75 6d6e 733d 5b74  .drop(columns=[t
-00004430: 6172 6765 745d 2c20 696e 706c 6163 653d  arget], inplace=
-00004440: 5472 7565 290d 0a20 2020 2020 2020 200d  True)..        .
-00004450: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00004460: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
-00004470: 7574 6573 2920 3e20 3120 3a0d 0a20 2020  utes) > 1 :..   
-00004480: 2020 2020 2020 2020 2064 6620 3d20 6466           df = df
-00004490: 2e64 726f 7028 636f 6c75 6d6e 7320 3d20  .drop(columns = 
-000044a0: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
-000044b0: 7574 6529 0d0a 2020 2020 2020 2020 2020  ute)..          
-000044c0: 2020 2020 0d0a 2020 2020 2020 2020 7265      ..        re
-000044d0: 7475 726e 2064 662c 2074 6172 6765 745f  turn df, target_
-000044e0: 6466 0d0a 2020 2020 0d0a 2020 2020 6465  df..    ..    de
-000044f0: 6620 6261 6c61 6e63 655f 616c 6c28 7365  f balance_all(se
-00004500: 6c66 2c20 6461 7461 7365 743a 2070 642e  lf, dataset: pd.
-00004510: 4461 7461 4672 616d 652c 2074 6172 6765  DataFrame, targe
-00004520: 743a 2073 7472 2c20 7072 6f74 6563 7465  t: str, protecte
-00004530: 645f 6174 7472 6962 7574 6573 3a20 6c69  d_attributes: li
-00004540: 7374 2c20 0d0a 2020 2020 2020 2020 2020  st, ..          
-00004550: 2020 2020 2020 2020 2020 636f 6e74 5f63            cont_c
-00004560: 6f6c 756d 6e73 3a20 6c69 7374 203d 204e  olumns: list = N
-00004570: 6f6e 652c 2063 6174 5f63 6f6c 756d 6e73  one, cat_columns
-00004580: 3a20 6c69 7374 203d 204e 6f6e 6529 203a  : list = None) :
-00004590: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-000045a0: 2020 2020 2020 2046 6972 7374 2062 616c         First bal
-000045b0: 616e 6365 7320 7468 6520 7072 6f74 6563  ances the protec
-000045c0: 7465 6420 6174 7472 6962 7574 6528 7329  ted attribute(s)
-000045d0: 2c20 616e 6420 7468 656e 2062 616c 616e  , and then balan
-000045e0: 6365 2074 6865 6972 206f 7574 7075 742e  ce their output.
-000045f0: 2047 6976 6573 2061 6e20 616c 6d6f 7374   Gives an almost
-00004600: 2070 6572 6665 6374 6c79 2062 616c 616e   perfectly balan
-00004610: 6365 6420 6461 7461 7365 7420 666f 7220  ced dataset for 
-00004620: 7468 6520 7072 6f74 6563 7465 6420 6174  the protected at
-00004630: 7472 6962 7574 6528 7329 2e0d 0a0d 0a20  tribute(s)..... 
-00004640: 2020 2020 2020 2041 7267 733a 200d 0a20         Args: .. 
-00004650: 2020 2020 2020 2020 2020 2064 6174 6173             datas
-00004660: 6574 2028 7064 2e44 6174 6146 7261 6d65  et (pd.DataFrame
-00004670: 293a 2064 6174 6173 6574 2074 6f20 6d69  ): dataset to mi
-00004680: 7469 6761 7465 2c20 7468 6174 2069 6e63  tigate, that inc
-00004690: 6c75 6465 7320 7468 6520 7461 7267 6574  ludes the target
-000046a0: 2063 6f6c 756d 6e2e 0d0a 2020 2020 2020   column...      
-000046b0: 2020 2020 2020 7461 7267 6574 2028 7374        target (st
-000046c0: 7229 3a20 7468 6520 7461 7267 6574 2063  r): the target c
-000046d0: 6f6c 756d 6e20 6e61 6d65 0d0a 2020 2020  olumn name..    
-000046e0: 2020 2020 2020 2020 7072 6f74 6563 7465          protecte
-000046f0: 645f 6174 7472 6962 7574 6573 2028 6c69  d_attributes (li
-00004700: 7374 2c20 6f70 7469 6f6e 616c 293a 2054  st, optional): T
-00004710: 6865 2061 7474 7269 6275 7465 2873 2920  he attribute(s) 
-00004720: 746f 2062 616c 616e 6365 2e20 4465 6661  to balance. Defa
-00004730: 756c 7473 2074 6f20 4e6f 6e65 2e0d 0a20  ults to None... 
-00004740: 2020 2020 2020 2020 2020 2063 6f6e 745f             cont_
-00004750: 636f 6c75 6d6e 7320 286c 6973 742c 206f  columns (list, o
-00004760: 7074 696f 6e61 6c29 3a20 5468 6520 636f  ptional): The co
-00004770: 6e74 696e 756f 7573 2063 6f6c 756d 6e73  ntinuous columns
-00004780: 2069 6e20 7468 6520 6461 7461 7365 742e   in the dataset.
-00004790: 204f 6e6c 7920 4e65 6365 7373 6172 7920   Only Necessary 
-000047a0: 6966 2074 6865 2073 616d 706c 696e 6720  if the sampling 
-000047b0: 7374 7261 7465 6779 2069 7320 534d 4f54  strategy is SMOT
-000047c0: 454e 432e 2044 6566 6175 6c74 7320 746f  ENC. Defaults to
-000047d0: 204e 6f6e 652e 0d0a 2020 2020 2020 2020   None...        
-000047e0: 2020 2020 6361 745f 636f 6c75 6d6e 7320      cat_columns 
-000047f0: 286c 6973 742c 206f 7074 696f 6e61 6c29  (list, optional)
-00004800: 3a20 5468 6520 6361 7465 676f 7269 6361  : The categorica
-00004810: 6c20 636f 6c75 6d6e 7320 696e 2074 6865  l columns in the
-00004820: 2064 6174 6173 6574 2e20 4f6e 6c79 204e   dataset. Only N
-00004830: 6563 6573 7361 7279 2069 6620 7468 6520  ecessary if the 
-00004840: 7361 6d70 6c69 6e67 2073 7472 6174 6567  sampling strateg
-00004850: 7920 6973 2053 4d4f 5445 4e43 2e20 4465  y is SMOTENC. De
-00004860: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0d  faults to None..
-00004870: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00004880: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
-00004890: 2028 5b70 642e 4461 7461 4672 616d 652c   ([pd.DataFrame,
-000048a0: 2070 642e 4461 7461 4672 616d 655d 293a   pd.DataFrame]):
-000048b0: 2074 6865 2062 616c 616e 6365 6420 6461   the balanced da
-000048c0: 7461 6672 616d 6573 2066 6f72 2074 6865  taframes for the
-000048d0: 2064 6174 6173 6574 2061 6e64 2074 6865   dataset and the
-000048e0: 2074 6172 6765 740d 0a20 2020 2020 2020   target..       
-000048f0: 2022 2222 0d0a 2020 2020 2020 2020 6466   """..        df
-00004900: 2c20 7420 3d20 7365 6c66 2e62 616c 616e  , t = self.balan
-00004910: 6365 5f70 726f 7465 6374 6564 5f61 7474  ce_protected_att
-00004920: 7269 6275 7465 2864 6174 6173 6574 2c20  ribute(dataset, 
-00004930: 7461 7267 6574 2c20 7072 6f74 6563 7465  target, protecte
-00004940: 645f 6174 7472 6962 7574 6573 2c20 636f  d_attributes, co
-00004950: 6e74 5f63 6f6c 756d 6e73 2c20 6361 745f  nt_columns, cat_
-00004960: 636f 6c75 6d6e 7329 200d 0a20 2020 2020  columns) ..     
-00004970: 2020 2064 662e 6c6f 635b 3a2c 2074 6172     df.loc[:, tar
-00004980: 6765 745d 203d 2074 0d0a 2020 2020 2020  get] = t..      
-00004990: 2020 6466 2c20 7420 3d20 7365 6c66 2e62    df, t = self.b
-000049a0: 616c 616e 6365 5f6f 7574 7075 745f 666f  alance_output_fo
-000049b0: 725f 6174 7472 6962 7574 6528 6466 2c20  r_attribute(df, 
-000049c0: 7461 7267 6574 2c20 7072 6f74 6563 7465  target, protecte
-000049d0: 645f 6174 7472 6962 7574 6573 2c20 636f  d_attributes, co
-000049e0: 6e74 5f63 6f6c 756d 6e73 2c20 6361 745f  nt_columns, cat_
-000049f0: 636f 6c75 6d6e 7329 0d0a 2020 2020 2020  columns)..      
-00004a00: 2020 0d0a 2020 2020 2020 2020 7265 7475    ..        retu
-00004a10: 726e 2064 662c 2074 2020 2020 0d0a 2020  rn df, t    ..  
-00004a20: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00004a30: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
-00004a40: 6620 5f68 6967 6865 7374 5f72 6174 696f  f _highest_ratio
-00004a50: 2873 656c 662c 2064 6174 6173 6574 3a20  (self, dataset: 
-00004a60: 7064 2e44 6174 6146 7261 6d65 2c20 7461  pd.DataFrame, ta
-00004a70: 7267 6574 3a20 7374 722c 2063 6c61 7373  rget: str, class
-00004a80: 6573 3a20 6469 6374 2c20 7072 6f74 6563  es: dict, protec
-00004a90: 7465 645f 6174 7472 6962 7574 653a 2073  ted_attribute: s
-00004aa0: 7472 2920 3a0d 0a20 2020 2020 2020 2022  tr) :..        "
-00004ab0: 2222 0d0a 2020 2020 2020 2020 4769 7665  ""..        Give
-00004ac0: 2074 6865 2068 6967 6865 7374 2072 6174   the highest rat
-00004ad0: 696f 206f 6620 706f 7369 7469 7665 206f  io of positive o
-00004ae0: 7574 7075 7420 6f6e 206e 6567 6174 6976  utput on negativ
-00004af0: 6520 6f75 7470 7574 206f 6620 616c 6c20  e output of all 
-00004b00: 7468 6520 636c 6173 7365 7320 6f66 2074  the classes of t
-00004b10: 6865 2070 726f 7465 6374 6564 2061 7474  he protected att
-00004b20: 7269 6275 7465 2e20 4e65 6365 7373 6172  ribute. Necessar
-00004b30: 7920 666f 7220 6261 6c61 6e63 655f 6f75  y for balance_ou
-00004b40: 7470 7574 5f66 6f72 5f61 7474 7269 6275  tput_for_attribu
-00004b50: 7465 2e0d 0a0d 0a20 2020 2020 2020 2041  te.....        A
-00004b60: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
-00004b70: 2020 6461 7461 7365 7420 2870 642e 4461    dataset (pd.Da
-00004b80: 7461 4672 616d 6529 3a20 6461 7461 7365  taFrame): datase
-00004b90: 7420 746f 206d 6974 6967 6174 652c 2074  t to mitigate, t
-00004ba0: 6861 7420 696e 636c 7564 6573 2074 6865  hat includes the
-00004bb0: 2074 6172 6765 7420 636f 6c75 6d6e 2e0d   target column..
-00004bc0: 0a20 2020 2020 2020 2020 2020 2074 6172  .            tar
-00004bd0: 6765 7420 2873 7472 293a 2074 6865 2074  get (str): the t
-00004be0: 6172 6765 7420 636f 6c75 6d6e 206e 616d  arget column nam
-00004bf0: 650d 0a20 2020 2020 2020 2020 2020 2063  e..            c
-00004c00: 6c61 7373 6573 2028 6469 6374 293a 2074  lasses (dict): t
-00004c10: 6865 2063 6c61 7373 6573 206f 6620 7468  he classes of th
-00004c20: 6520 7072 6f74 6563 7465 6420 6174 7472  e protected attr
-00004c30: 6962 7574 650d 0a20 2020 2020 2020 2020  ibute..         
-00004c40: 2020 2070 726f 7465 6374 6564 5f61 7474     protected_att
-00004c50: 7269 6275 7465 2028 7374 7229 3a20 7468  ribute (str): th
-00004c60: 6520 7072 6f74 6563 7465 6420 6174 7472  e protected attr
-00004c70: 6962 7574 6520 746f 2063 616c 6375 6c61  ibute to calcula
-00004c80: 7465 2074 6865 2068 6967 6865 7374 2072  te the highest r
-00004c90: 6174 696f 2066 6f72 2e0d 0a0d 0a20 2020  atio for.....   
-00004ca0: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
-00004cb0: 2020 2020 2020 2020 2020 2028 5b66 6c6f             ([flo
-00004cc0: 6174 2c20 7374 725d 293a 2074 6865 2068  at, str]): the h
-00004cd0: 6967 6865 7374 2072 6174 696f 2061 6e64  ighest ratio and
-00004ce0: 2074 6865 2061 7373 6f63 6961 7465 6420   the associated 
-00004cf0: 636c 6173 730d 0a20 2020 2020 2020 2022  class..        "
-00004d00: 2222 0d0a 2020 2020 2020 2020 0d0a 2020  ""..        ..  
-00004d10: 2020 2020 2020 725f 6d61 7820 3d20 300d        r_max = 0.
-00004d20: 0a20 2020 2020 2020 2063 5f6d 6178 203d  .        c_max =
-00004d30: 2063 6c61 7373 6573 5b30 5d0d 0a20 2020   classes[0]..   
-00004d40: 2020 2020 2066 6f72 2063 2069 6e20 636c       for c in cl
-00004d50: 6173 7365 7320 3a0d 0a20 2020 2020 2020  asses :..       
-00004d60: 2020 2020 2072 203d 2064 6174 6173 6574       r = dataset
-00004d70: 5b64 6174 6173 6574 5b70 726f 7465 6374  [dataset[protect
-00004d80: 6564 5f61 7474 7269 6275 7465 5d20 3d3d  ed_attribute] ==
-00004d90: 2063 5d5b 7461 7267 6574 5d2e 7661 6c75   c][target].valu
-00004da0: 655f 636f 756e 7473 2829 5b31 5d2f 6461  e_counts()[1]/da
-00004db0: 7461 7365 745b 6461 7461 7365 745b 7072  taset[dataset[pr
-00004dc0: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
-00004dd0: 655d 203d 3d20 635d 5b74 6172 6765 745d  e] == c][target]
-00004de0: 2e76 616c 7565 5f63 6f75 6e74 7328 295b  .value_counts()[
-00004df0: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
-00004e00: 6966 2072 203e 2031 203a 0d0a 2020 2020  if r > 1 :..    
-00004e10: 2020 2020 2020 2020 2020 2020 7220 3d20              r = 
-00004e20: 312f 720d 0a20 2020 2020 2020 2020 2020  1/r..           
-00004e30: 2069 6620 7220 3e20 725f 6d61 7820 3a0d   if r > r_max :.
-00004e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004e50: 2072 5f6d 6178 203d 2072 0d0a 2020 2020   r_max = r..    
-00004e60: 2020 2020 2020 2020 2020 2020 635f 6d61              c_ma
-00004e70: 7820 3d20 630d 0a20 2020 2020 2020 2072  x = c..        r
-00004e80: 6574 7572 6e20 725f 6d61 782c 2063 5f6d  eturn r_max, c_m
-00004e90: 6178 0d0a 2020 200d 0a20 2020 0d0a 2020  ax..   ..   ..  
-00004ea0: 2020 6465 6620 5f6d 616b 655f 7375 7065    def _make_supe
-00004eb0: 725f 7072 6f74 6563 7465 6428 7365 6c66  r_protected(self
-00004ec0: 2c20 6461 7461 7365 743a 2070 642e 4461  , dataset: pd.Da
-00004ed0: 7461 4672 616d 652c 2070 726f 7465 6374  taFrame, protect
-00004ee0: 6564 5f61 7474 7269 6275 7465 733a 206c  ed_attributes: l
-00004ef0: 6973 7429 203a 0d0a 2020 2020 2020 2020  ist) :..        
-00004f00: 2222 220d 0a20 2020 2020 2020 204d 616b  """..        Mak
-00004f10: 6520 6120 7375 7065 7220 7072 6f74 6563  e a super protec
-00004f20: 7465 6420 6174 7472 6962 7574 6520 7468  ted attribute th
-00004f30: 6174 2069 7320 7468 6520 636f 6d62 696e  at is the combin
-00004f40: 6174 696f 6e20 6f66 2061 6c6c 2067 6976  ation of all giv
-00004f50: 656e 2070 726f 7465 6374 6564 2061 7474  en protected att
-00004f60: 7269 6275 7465 7320 6361 6c6c 6564 2022  ributes called "
-00004f70: 7072 6f74 6563 7465 645f 7375 7065 7263  protected_superc
-00004f80: 6c61 7373 220d 0a0d 0a20 2020 2020 2020  lass"....       
-00004f90: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
-00004fa0: 2020 2020 6461 7461 7365 7420 2870 642e      dataset (pd.
-00004fb0: 4461 7461 4672 616d 6529 3a20 6461 7461  DataFrame): data
-00004fc0: 7365 7420 746f 206d 6974 6967 6174 652c  set to mitigate,
-00004fd0: 2074 6861 7420 696e 636c 7564 6573 2074   that includes t
-00004fe0: 6865 2074 6172 6765 7420 636f 6c75 6d6e  he target column
-00004ff0: 2e0d 0a20 2020 2020 2020 2020 2020 2070  ...            p
-00005000: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
-00005010: 7465 7320 286c 6973 7429 3a20 7072 6f74  tes (list): prot
-00005020: 6563 7465 6420 6174 7472 6962 7574 6573  ected attributes
-00005030: 2074 6f20 636f 6d62 696e 650d 0a20 2020   to combine..   
-00005040: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00005050: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
-00005060: 2020 2020 2020 2020 2028 5b70 642e 4461           ([pd.Da
-00005070: 7461 4672 616d 652c 2073 7472 5d29 3a20  taFrame, str]): 
-00005080: 7468 6520 7472 616e 7366 6f72 6d65 6420  the transformed 
-00005090: 6461 7461 7365 7420 616e 6420 7468 6520  dataset and the 
-000050a0: 6e61 6d65 2022 7375 7065 7220 7072 6f74  name "super prot
-000050b0: 6563 7465 6422 2063 6f6c 756d 6e0d 0a20  ected" column.. 
-000050c0: 2020 2020 2020 2022 2222 0d0a 0d0a 2020         """....  
-000050d0: 2020 2020 2020 6466 203d 2064 6174 6173        df = datas
-000050e0: 6574 2e63 6f70 7928 290d 0a20 2020 2020  et.copy()..     
-000050f0: 2020 2073 7570 6572 7072 6f74 6563 7465     superprotecte
-00005100: 645f 636f 6c75 6d6e 203d 2066 756e 6374  d_column = funct
-00005110: 6f6f 6c73 2e72 6564 7563 6528 6c61 6d62  ools.reduce(lamb
-00005120: 6461 2061 2c20 6220 3a20 6120 2b20 225f  da a, b : a + "_
-00005130: 2220 2b20 622c 2070 726f 7465 6374 6564  " + b, protected
-00005140: 5f61 7474 7269 6275 7465 7329 0d0a 2020  _attributes)..  
-00005150: 2020 2020 2020 6466 5b73 7570 6572 7072        df[superpr
-00005160: 6f74 6563 7465 645f 636f 6c75 6d6e 5d20  otected_column] 
-00005170: 3d20 2222 0d0a 2020 2020 2020 2020 666f  = ""..        fo
-00005180: 7220 7072 6f74 6563 7465 645f 6174 7472  r protected_attr
-00005190: 6962 7574 6520 696e 2070 726f 7465 6374  ibute in protect
-000051a0: 6564 5f61 7474 7269 6275 7465 7320 3a0d  ed_attributes :.
-000051b0: 0a0d 0a20 2020 2020 2020 2020 2020 2064  ...            d
-000051c0: 665b 7375 7065 7270 726f 7465 6374 6564  f[superprotected
-000051d0: 5f63 6f6c 756d 6e5d 202b 3d20 6466 5b70  _column] += df[p
-000051e0: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
-000051f0: 7465 5d2e 6170 706c 7928 7374 7229 2020  te].apply(str)  
-00005200: 2b20 225f 220d 0a20 2020 2020 2020 2020  + "_"..         
-00005210: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00005220: 2020 2020 2020 2020 6466 5b73 7570 6572          df[super
-00005230: 7072 6f74 6563 7465 645f 636f 6c75 6d6e  protected_column
-00005240: 5d20 3d20 6466 5b73 7570 6572 7072 6f74  ] = df[superprot
-00005250: 6563 7465 645f 636f 6c75 6d6e 5d2e 6170  ected_column].ap
-00005260: 706c 7928 6c61 6d62 6461 2078 203a 2078  ply(lambda x : x
-00005270: 5b3a 2d31 5d29 0d0a 2020 2020 2020 2020  [:-1])..        
-00005280: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00005290: 2020 2020 7265 7475 726e 2064 662c 2073      return df, s
-000052a0: 7570 6572 7072 6f74 6563 7465 645f 636f  uperprotected_co
-000052b0: 6c75 6d6e                                lumn
+00000020: 6561 726e 2e6f 7665 725f 7361 6d70 6c69  earn.over_sampli
+00000030: 6e67 2069 6d70 6f72 7420 5261 6e64 6f6d  ng import Random
+00000040: 4f76 6572 5361 6d70 6c65 722c 2053 4d4f  OverSampler, SMO
+00000050: 5445 4e43 0d0a 6672 6f6d 2069 6d62 6c65  TENC..from imble
+00000060: 6172 6e2e 756e 6465 725f 7361 6d70 6c69  arn.under_sampli
+00000070: 6e67 2069 6d70 6f72 7420 5261 6e64 6f6d  ng import Random
+00000080: 556e 6465 7253 616d 706c 6572 0d0a 696d  UnderSampler..im
+00000090: 706f 7274 2066 756e 6374 6f6f 6c73 0d0a  port functools..
+000000a0: 0d0a 6672 6f6d 2074 6f72 6368 2069 6d70  ..from torch imp
+000000b0: 6f72 7420 6361 740d 0a66 726f 6d20 2e5f  ort cat..from ._
+000000c0: 7072 6f63 6573 736f 7220 696d 706f 7274  processor import
+000000d0: 2053 4d4f 5445 4e43 5072 6f63 6573 736f   SMOTENCProcesso
+000000e0: 722c 205f 5072 6f63 6573 736f 720d 0a0d  r, _Processor...
+000000f0: 0a66 726f 6d20 2e62 6173 6520 696d 706f  .from .base impo
+00000100: 7274 2042 6173 654d 6974 6967 6174 696f  rt BaseMitigatio
+00000110: 6e53 7472 6174 6567 792c 2042 6173 6550  nStrategy, BaseP
+00000120: 726f 6365 7373 6f72 0d0a 6672 6f6d 202e  rocessor..from .
+00000130: 5f75 7469 6c73 2069 6d70 6f72 7420 7361  _utils import sa
+00000140: 6e69 7479 5f63 6865 636b 6572 0d0a 0d0a  nity_checker....
+00000150: 0d0a 5341 4d50 4c49 4e47 5f46 554e 4354  ..SAMPLING_FUNCT
+00000160: 494f 4e53 203d 205b 2252 616e 646f 6d4f  IONS = ["RandomO
+00000170: 7665 7253 616d 706c 6572 222c 2022 534d  verSampler", "SM
+00000180: 4f54 454e 4322 2c20 2252 616e 646f 6d55  OTENC", "RandomU
+00000190: 6e64 6572 5361 6d70 6c65 7222 5d0d 0a0d  nderSampler"]...
+000001a0: 0a20 2020 0d0a 0d0a 636c 6173 7320 4261  .   ....class Ba
+000001b0: 6c61 6e63 654f 7574 7075 7428 4261 7365  lanceOutput(Base
+000001c0: 4d69 7469 6761 7469 6f6e 5374 7261 7465  MitigationStrate
+000001d0: 6779 2920 3a0d 0a20 2020 2022 2222 5465  gy) :..    """Te
+000001e0: 7374 0d0a 0d0a 2020 2020 4172 6773 3a0d  st....    Args:.
+000001f0: 0a20 2020 2020 2020 2042 6173 654d 6974  .        BaseMit
+00000200: 6967 6174 696f 6e53 7472 6174 6567 7920  igationStrategy 
+00000210: 285f 7479 7065 5f29 3a20 5f64 6573 6372  (_type_): _descr
+00000220: 6970 7469 6f6e 5f0d 0a20 2020 2022 2222  iption_..    """
+00000230: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00000240: 5f5f 2873 656c 662c 2073 616d 706c 6572  __(self, sampler
+00000250: 3a20 4261 7365 5072 6f63 6573 736f 7229  : BaseProcessor)
+00000260: 203a 0d0a 2020 2020 2020 2020 7375 7065   :..        supe
+00000270: 7228 292e 5f5f 696e 6974 5f5f 2873 616d  r().__init__(sam
+00000280: 706c 6572 290d 0a20 2020 200d 0a20 2020  pler)..    ..   
+00000290: 2064 6566 2062 616c 616e 6365 2873 656c   def balance(sel
+000002a0: 662c 2064 6174 6173 6574 3a20 7064 2e44  f, dataset: pd.D
+000002b0: 6174 6146 7261 6d65 2c20 7461 7267 6574  ataFrame, target
+000002c0: 3a20 7064 2e44 6174 6146 7261 6d65 203d  : pd.DataFrame =
+000002d0: 204e 6f6e 652c 2070 726f 7465 6374 6564   None, protected
+000002e0: 5f61 7474 7269 6275 7465 733a 206c 6973  _attributes: lis
+000002f0: 7420 3d20 4e6f 6e65 2c20 0d0a 2020 2020  t = None, ..    
+00000300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000310: 2020 2063 6f6e 745f 636f 6c75 6d6e 733a     cont_columns:
+00000320: 206c 6973 7420 3d20 4e6f 6e65 2c20 6361   list = None, ca
+00000330: 745f 636f 6c75 6d6e 733a 206c 6973 7420  t_columns: list 
+00000340: 3d20 4e6f 6e65 2920 3a0d 0a20 2020 2020  = None) :..     
+00000350: 2020 200d 0a20 2020 2020 2020 2064 662c     ..        df,
+00000360: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
+00000370: 6275 7465 203d 2073 656c 662e 5f67 6574  bute = self._get
+00000380: 5f64 6174 6166 7261 6d65 5f61 6e64 5f70  _dataframe_and_p
+00000390: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
+000003a0: 7465 2864 6174 6173 6574 2c20 7072 6f74  te(dataset, prot
+000003b0: 6563 7465 645f 6174 7472 6962 7574 6573  ected_attributes
+000003c0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
+000003d0: 2020 2020 2058 5f70 726f 6365 7373 6564       X_processed
+000003e0: 2c20 795f 7072 6f63 6573 7365 6420 3d20  , y_processed = 
+000003f0: 7365 6c66 2e73 616d 706c 6572 2e5f 7072  self.sampler._pr
+00000400: 6f63 6573 7328 6466 2c20 7461 7267 6574  ocess(df, target
+00000410: 2c20 636f 6e74 5f63 6f6c 756d 6e73 2c20  , cont_columns, 
+00000420: 6361 745f 636f 6c75 6d6e 7329 0d0a 2020  cat_columns)..  
+00000430: 2020 2020 2020 585f 7265 7361 6d70 6c65        X_resample
+00000440: 642c 2079 5f72 6573 616d 706c 6564 203d  d, y_resampled =
+00000450: 2073 656c 662e 7361 6d70 6c65 722e 6669   self.sampler.fi
+00000460: 745f 7265 7361 6d70 6c65 2858 5f70 726f  t_resample(X_pro
+00000470: 6365 7373 6564 2c20 795f 7072 6f63 6573  cessed, y_proces
+00000480: 7365 6429 0d0a 2020 2020 2020 2020 585f  sed)..        X_
+00000490: 6669 6e61 6c2c 2079 5f66 696e 616c 203d  final, y_final =
+000004a0: 2073 656c 662e 7361 6d70 6c65 722e 5f75   self.sampler._u
+000004b0: 6e70 726f 6365 7373 2858 5f72 6573 616d  nprocess(X_resam
+000004c0: 706c 6564 2c20 795f 7265 7361 6d70 6c65  pled, y_resample
+000004d0: 6429 0d0a 2020 2020 2020 2020 0d0a 2020  d)..        ..  
+000004e0: 2020 2020 2020 585f 6669 6e61 6c20 3d20        X_final = 
+000004f0: 7365 6c66 2e5f 6765 745f 6669 6e61 6c5f  self._get_final_
+00000500: 6461 7461 6672 616d 6528 585f 6669 6e61  dataframe(X_fina
+00000510: 6c2c 2070 726f 7465 6374 6564 5f61 7474  l, protected_att
+00000520: 7269 6275 7465 732c 2070 726f 7465 6374  ributes, protect
+00000530: 6564 5f61 7474 7269 6275 7465 290d 0a20  ed_attribute).. 
+00000540: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00000550: 2072 6574 7572 6e20 585f 6669 6e61 6c2c   return X_final,
+00000560: 2079 5f66 696e 616c 2020 2020 200d 0a0d   y_final     ...
+00000570: 0a0d 0a63 6c61 7373 2042 616c 616e 6365  ...class Balance
+00000580: 4174 7472 6962 7574 6573 2842 6173 654d  Attributes(BaseM
+00000590: 6974 6967 6174 696f 6e53 7472 6174 6567  itigationStrateg
+000005a0: 7929 203a 0d0a 2020 2020 6465 6620 5f5f  y) :..    def __
+000005b0: 696e 6974 5f5f 2873 656c 662c 2073 616d  init__(self, sam
+000005c0: 706c 6572 3a20 4261 7365 5072 6f63 6573  pler: BaseProces
+000005d0: 736f 7229 203a 0d0a 2020 2020 2020 2020  sor) :..        
+000005e0: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+000005f0: 2873 616d 706c 6572 290d 0a0d 0a20 2020  (sampler)....   
+00000600: 2064 6566 2062 616c 616e 6365 2873 656c   def balance(sel
+00000610: 662c 2064 6174 6173 6574 3a20 7064 2e44  f, dataset: pd.D
+00000620: 6174 6146 7261 6d65 2c20 7461 7267 6574  ataFrame, target
+00000630: 3a20 7064 2e44 6174 6146 7261 6d65 203d  : pd.DataFrame =
+00000640: 204e 6f6e 652c 2070 726f 7465 6374 6564   None, protected
+00000650: 5f61 7474 7269 6275 7465 733a 206c 6973  _attributes: lis
+00000660: 7420 3d20 4e6f 6e65 2c20 0d0a 2020 2020  t = None, ..    
+00000670: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00000680: 5f63 6f6c 756d 6e73 3a20 6c69 7374 203d  _columns: list =
+00000690: 204e 6f6e 652c 2063 6174 5f63 6f6c 756d   None, cat_colum
+000006a0: 6e73 3a20 6c69 7374 203d 204e 6f6e 6529  ns: list = None)
+000006b0: 203a 0d0a 2020 2020 2020 2020 0d0a 2020   :..        ..  
+000006c0: 2020 2020 2020 6466 2c20 7072 6f74 6563        df, protec
+000006d0: 7465 645f 6174 7472 6962 7574 6520 3d20  ted_attribute = 
+000006e0: 7365 6c66 2e5f 6765 745f 6461 7461 6672  self._get_datafr
+000006f0: 616d 655f 616e 645f 7072 6f74 6563 7465  ame_and_protecte
+00000700: 645f 6174 7472 6962 7574 6528 6461 7461  d_attribute(data
+00000710: 7365 742c 2070 726f 7465 6374 6564 5f61  set, protected_a
+00000720: 7474 7269 6275 7465 7329 0d0a 0d0a 2020  ttributes)....  
+00000730: 2020 2020 2020 585f 7072 6f63 6573 7365        X_processe
+00000740: 642c 2079 5f70 726f 6365 7373 6564 203d  d, y_processed =
+00000750: 2073 656c 662e 7361 6d70 6c65 722e 5f70   self.sampler._p
+00000760: 726f 6365 7373 2864 662c 2074 6172 6765  rocess(df, targe
+00000770: 742c 2063 6f6e 745f 636f 6c75 6d6e 732c  t, cont_columns,
+00000780: 2063 6174 5f63 6f6c 756d 6e73 290d 0a20   cat_columns).. 
+00000790: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000007a0: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
+000007b0: 6275 7465 5f63 6f6c 756d 6e20 3d20 585f  bute_column = X_
+000007c0: 7072 6f63 6573 7365 645b 7072 6f74 6563  processed[protec
+000007d0: 7465 645f 6174 7472 6962 7574 655d 0d0a  ted_attribute]..
+000007e0: 2020 2020 2020 2020 585f 7072 6f63 6573          X_proces
+000007f0: 7365 6420 3d20 585f 7072 6f63 6573 7365  sed = X_processe
+00000800: 642e 6472 6f70 2863 6f6c 756d 6e73 3d5b  d.drop(columns=[
+00000810: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
+00000820: 7574 655d 290d 0a20 2020 2020 2020 2058  ute])..        X
+00000830: 5f70 726f 6365 7373 6564 2e6c 6f63 5b3a  _processed.loc[:
+00000840: 2c22 7461 7267 6574 225d 203d 2079 5f70  ,"target"] = y_p
+00000850: 726f 6365 7373 6564 0d0a 2020 2020 2020  rocessed..      
+00000860: 2020 6e65 775f 6361 745f 636f 6c75 6d6e    new_cat_column
+00000870: 7320 3d20 5b63 6f6c 756d 6e20 666f 7220  s = [column for 
+00000880: 636f 6c75 6d6e 2069 6e20 6361 745f 636f  column in cat_co
+00000890: 6c75 6d6e 7320 6966 2063 6f6c 756d 6e20  lumns if column 
+000008a0: 213d 2070 726f 7465 6374 6564 5f61 7474  != protected_att
+000008b0: 7269 6275 7465 5d20 2b20 5b22 7461 7267  ribute] + ["targ
+000008c0: 6574 225d 0d0a 2020 2020 2020 2020 6361  et"]..        ca
+000008d0: 745f 636f 6c75 6d6e 735f 6964 7320 3d20  t_columns_ids = 
+000008e0: 5b58 5f70 726f 6365 7373 6564 2e63 6f6c  [X_processed.col
+000008f0: 756d 6e73 2e67 6574 5f6c 6f63 2863 6f6c  umns.get_loc(col
+00000900: 5f6e 616d 6529 2066 6f72 2063 6f6c 5f6e  _name) for col_n
+00000910: 616d 6520 696e 206e 6577 5f63 6174 5f63  ame in new_cat_c
+00000920: 6f6c 756d 6e73 5d0d 0a20 2020 2020 2020  olumns]..       
+00000930: 2073 656c 662e 7361 6d70 6c65 722e 7365   self.sampler.se
+00000940: 745f 6361 7465 676f 7269 6361 6c5f 6665  t_categorical_fe
+00000950: 6174 7572 6573 2863 6174 5f63 6f6c 756d  atures(cat_colum
+00000960: 6e73 5f69 6473 290d 0a0d 0a20 2020 2020  ns_ids)....     
+00000970: 2020 2058 5f72 6573 616d 706c 6564 2c20     X_resampled, 
+00000980: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
+00000990: 7574 655f 7265 7361 6d70 6c65 6420 3d20  ute_resampled = 
+000009a0: 7365 6c66 2e73 616d 706c 6572 2e66 6974  self.sampler.fit
+000009b0: 5f72 6573 616d 706c 6528 585f 7072 6f63  _resample(X_proc
+000009c0: 6573 7365 642c 2070 726f 7465 6374 6564  essed, protected
+000009d0: 5f61 7474 7269 6275 7465 5f63 6f6c 756d  _attribute_colum
+000009e0: 6e29 0d0a 2020 2020 2020 2020 585f 7265  n)..        X_re
+000009f0: 7361 6d70 6c65 642e 6c6f 635b 3a2c 2070  sampled.loc[:, p
+00000a00: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
+00000a10: 7465 5d20 3d20 7072 6f74 6563 7465 645f  te] = protected_
+00000a20: 6174 7472 6962 7574 655f 7265 7361 6d70  attribute_resamp
+00000a30: 6c65 640d 0a20 2020 2020 2020 2079 5f72  led..        y_r
+00000a40: 6573 616d 706c 6564 203d 2058 5f72 6573  esampled = X_res
+00000a50: 616d 706c 6564 5b22 7461 7267 6574 225d  ampled["target"]
+00000a60: 0d0a 2020 2020 2020 2020 585f 7265 7361  ..        X_resa
+00000a70: 6d70 6c65 6420 3d20 585f 7265 7361 6d70  mpled = X_resamp
+00000a80: 6c65 642e 6472 6f70 2863 6f6c 756d 6e73  led.drop(columns
+00000a90: 3d5b 2274 6172 6765 7422 5d29 0d0a 2020  =["target"])..  
+00000aa0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00000ab0: 585f 6669 6e61 6c2c 2079 5f66 696e 616c  X_final, y_final
+00000ac0: 203d 2073 656c 662e 7361 6d70 6c65 722e   = self.sampler.
+00000ad0: 5f75 6e70 726f 6365 7373 2858 5f72 6573  _unprocess(X_res
+00000ae0: 616d 706c 6564 2c20 795f 7265 7361 6d70  ampled, y_resamp
+00000af0: 6c65 6429 0d0a 2020 2020 2020 2020 585f  led)..        X_
+00000b00: 6669 6e61 6c20 3d20 7365 6c66 2e5f 6765  final = self._ge
+00000b10: 745f 6669 6e61 6c5f 6461 7461 6672 616d  t_final_datafram
+00000b20: 6528 585f 6669 6e61 6c2c 2070 726f 7465  e(X_final, prote
+00000b30: 6374 6564 5f61 7474 7269 6275 7465 732c  cted_attributes,
+00000b40: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
+00000b50: 6275 7465 290d 0a0d 0a20 2020 2020 2020  bute)....       
+00000b60: 2072 6574 7572 6e20 585f 6669 6e61 6c2c   return X_final,
+00000b70: 2079 5f66 696e 616c 0d0a 2020 2020 2020   y_final..      
+00000b80: 2020 0d0a 636c 6173 7320 4261 6c61 6e63    ..class Balanc
+00000b90: 654f 7574 7075 7446 6f72 4174 7472 6962  eOutputForAttrib
+00000ba0: 7574 6573 2842 6173 654d 6974 6967 6174  utes(BaseMitigat
+00000bb0: 696f 6e53 7472 6174 6567 7929 203a 0d0a  ionStrategy) :..
+00000bc0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00000bd0: 2873 656c 662c 2073 616d 706c 6572 3a20  (self, sampler: 
+00000be0: 4261 7365 5072 6f63 6573 736f 7229 203a  BaseProcessor) :
+00000bf0: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
+00000c00: 292e 5f5f 696e 6974 5f5f 2873 616d 706c  ).__init__(sampl
+00000c10: 6572 290d 0a20 2020 200d 0a20 2020 2064  er)..    ..    d
+00000c20: 6566 2062 616c 616e 6365 2873 656c 662c  ef balance(self,
+00000c30: 2064 6174 6173 6574 3a20 7064 2e44 6174   dataset: pd.Dat
+00000c40: 6146 7261 6d65 2c20 7461 7267 6574 3a20  aFrame, target: 
+00000c50: 7064 2e44 6174 6146 7261 6d65 203d 204e  pd.DataFrame = N
+00000c60: 6f6e 652c 2070 726f 7465 6374 6564 5f61  one, protected_a
+00000c70: 7474 7269 6275 7465 733a 206c 6973 7420  ttributes: list 
+00000c80: 3d20 4e6f 6e65 2c20 0d0a 2020 2020 2020  = None, ..      
+00000c90: 2020 2020 2020 2020 2020 636f 6e74 5f63            cont_c
+00000ca0: 6f6c 756d 6e73 3a20 6c69 7374 203d 204e  olumns: list = N
+00000cb0: 6f6e 652c 2063 6174 5f63 6f6c 756d 6e73  one, cat_columns
+00000cc0: 3a20 6c69 7374 203d 204e 6f6e 6529 203a  : list = None) :
+00000cd0: 0d0a 0d0a 2020 2020 2020 2020 6466 2c20  ....        df, 
+00000ce0: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
+00000cf0: 7574 6520 3d20 7365 6c66 2e5f 6765 745f  ute = self._get_
+00000d00: 6461 7461 6672 616d 655f 616e 645f 7072  dataframe_and_pr
+00000d10: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
+00000d20: 6528 6461 7461 7365 742c 2070 726f 7465  e(dataset, prote
+00000d30: 6374 6564 5f61 7474 7269 6275 7465 7329  cted_attributes)
+00000d40: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00000d50: 2020 2020 636c 6173 7365 7320 3d20 6c69      classes = li
+00000d60: 7374 2864 665b 7072 6f74 6563 7465 645f  st(df[protected_
+00000d70: 6174 7472 6962 7574 655d 2e75 6e69 7175  attribute].uniqu
+00000d80: 6528 2929 0d0a 2020 2020 2020 2020 6869  e())..        hi
+00000d90: 6768 6573 745f 722c 2063 6c61 7373 5f77  ghest_r, class_w
+00000da0: 6974 685f 6869 6768 6573 745f 7220 3d20  ith_highest_r = 
+00000db0: 7365 6c66 2e5f 6869 6768 6573 745f 7261  self._highest_ra
+00000dc0: 7469 6f28 6466 2c20 7461 7267 6574 2c20  tio(df, target, 
+00000dd0: 636c 6173 7365 732c 2070 726f 7465 6374  classes, protect
+00000de0: 6564 5f61 7474 7269 6275 7465 290d 0a20  ed_attribute).. 
+00000df0: 2020 2020 2020 2073 656c 662e 7361 6d70         self.samp
+00000e00: 6c65 722e 7361 6d70 6c69 6e67 5f73 7472  ler.sampling_str
+00000e10: 6174 6567 7920 3d20 6869 6768 6573 745f  ategy = highest_
+00000e20: 720d 0a20 2020 2020 2020 2058 5f66 696e  r..        X_fin
+00000e30: 616c 203d 2070 642e 4461 7461 4672 616d  al = pd.DataFram
+00000e40: 6528 636f 6c75 6d6e 7320 3d20 6466 2e63  e(columns = df.c
+00000e50: 6f6c 756d 6e73 290d 0a20 2020 2020 2020  olumns)..       
+00000e60: 2079 5f66 696e 616c 203d 2070 642e 5365   y_final = pd.Se
+00000e70: 7269 6573 2829 0d0a 2020 2020 2020 2020  ries()..        
+00000e80: 666f 7220 636c 6173 735f 2069 6e20 636c  for class_ in cl
+00000e90: 6173 7365 7320 3a0d 0a20 2020 2020 2020  asses :..       
+00000ea0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00000eb0: 2020 2020 2020 2023 206b 6565 7020 6f6e         # keep on
+00000ec0: 6c79 2074 6865 2072 6f77 7320 7769 7468  ly the rows with
+00000ed0: 2067 6976 656e 2063 6c61 7373 0d0a 2020   given class..  
+00000ee0: 2020 2020 2020 2020 2020 636c 6173 735f            class_
+00000ef0: 6466 203d 2064 665b 6466 5b70 726f 7465  df = df[df[prote
+00000f00: 6374 6564 5f61 7474 7269 6275 7465 5d20  cted_attribute] 
+00000f10: 3d3d 2063 6c61 7373 5f5d 0d0a 2020 2020  == class_]..    
+00000f20: 2020 2020 2020 2020 636c 6173 735f 7461          class_ta
+00000f30: 7267 6574 203d 2074 6172 6765 745b 6466  rget = target[df
+00000f40: 5b70 726f 7465 6374 6564 5f61 7474 7269  [protected_attri
+00000f50: 6275 7465 5d20 3d3d 2063 6c61 7373 5f5d  bute] == class_]
+00000f60: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+00000f70: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00000f80: 6c61 7373 5f20 213d 2063 6c61 7373 5f77  lass_ != class_w
+00000f90: 6974 685f 6869 6768 6573 745f 7220 3a20  ith_highest_r : 
+00000fa0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00000fb0: 2020 2023 2072 6573 616d 706c 6520 7468     # resample th
+00000fc0: 6520 7461 7267 6574 2066 6f72 2074 6869  e target for thi
+00000fd0: 7320 636c 6173 730d 0a20 2020 2020 2020  s class..       
+00000fe0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+00000ff0: 636c 6173 735f 7461 7267 6574 2e75 6e69  class_target.uni
+00001000: 7175 6528 2929 203e 2031 203a 0d0a 2020  que()) > 1 :..  
+00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001020: 2020 585f 7072 6f63 6573 7365 642c 2079    X_processed, y
+00001030: 5f70 726f 6365 7373 6564 203d 2073 656c  _processed = sel
+00001040: 662e 7361 6d70 6c65 722e 5f70 726f 6365  f.sampler._proce
+00001050: 7373 2863 6c61 7373 5f64 662c 2063 6c61  ss(class_df, cla
+00001060: 7373 5f74 6172 6765 742c 2063 6f6e 745f  ss_target, cont_
+00001070: 636f 6c75 6d6e 732c 2063 6174 5f63 6f6c  columns, cat_col
+00001080: 756d 6e73 290d 0a20 2020 2020 2020 2020  umns)..         
+00001090: 2020 2020 2020 2020 2020 2058 5f72 6573             X_res
+000010a0: 616d 706c 6564 2c20 795f 7265 7361 6d70  ampled, y_resamp
+000010b0: 6c65 6420 3d20 7365 6c66 2e73 616d 706c  led = self.sampl
+000010c0: 6572 2e66 6974 5f72 6573 616d 706c 6528  er.fit_resample(
+000010d0: 585f 7072 6f63 6573 7365 642c 2079 5f70  X_processed, y_p
+000010e0: 726f 6365 7373 6564 290d 0a20 2020 2020  rocessed)..     
+000010f0: 2020 2020 2020 2020 2020 2020 2020 2058                 X
+00001100: 5f63 6c61 7373 5f66 696e 616c 2c20 795f  _class_final, y_
+00001110: 636c 6173 735f 6669 6e61 6c20 3d20 7365  class_final = se
+00001120: 6c66 2e73 616d 706c 6572 2e5f 756e 7072  lf.sampler._unpr
+00001130: 6f63 6573 7328 585f 7265 7361 6d70 6c65  ocess(X_resample
+00001140: 642c 2079 5f72 6573 616d 706c 6564 290d  d, y_resampled).
+00001150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001160: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00001170: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
+00001180: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001190: 2020 2020 2020 2058 5f63 6c61 7373 5f66         X_class_f
+000011a0: 696e 616c 203d 2063 6c61 7373 5f64 660d  inal = class_df.
+000011b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000011c0: 2020 2020 2079 5f63 6c61 7373 5f66 696e       y_class_fin
+000011d0: 616c 203d 2063 6c61 7373 5f74 6172 6765  al = class_targe
+000011e0: 740d 0a20 2020 2020 2020 2020 2020 200d  t..            .
+000011f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001200: 2023 2061 7070 656e 6420 7468 6520 7265   # append the re
+00001210: 7361 6d70 6c65 6420 636c 6173 7320 696e  sampled class in
+00001220: 2066 696e 616c 2064 6673 0d0a 2020 2020   final dfs..    
+00001230: 2020 2020 2020 2020 2020 2020 585f 6669              X_fi
+00001240: 6e61 6c20 3d20 7064 2e63 6f6e 6361 7428  nal = pd.concat(
+00001250: 5b58 5f66 696e 616c 2c20 585f 636c 6173  [X_final, X_clas
+00001260: 735f 6669 6e61 6c5d 2c20 6967 6e6f 7265  s_final], ignore
+00001270: 5f69 6e64 6578 3d54 7275 6529 0d0a 2020  _index=True)..  
+00001280: 2020 2020 2020 2020 2020 2020 2020 795f                y_
+00001290: 6669 6e61 6c20 3d20 7064 2e63 6f6e 6361  final = pd.conca
+000012a0: 7428 5b79 5f66 696e 616c 2c20 795f 636c  t([y_final, y_cl
+000012b0: 6173 735f 6669 6e61 6c5d 290d 0a20 2020  ass_final])..   
+000012c0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000012d0: 2020 2020 2020 2065 6c73 6520 3a0d 0a20         else :.. 
+000012e0: 2020 2020 2020 2020 2020 2020 2020 2058                 X
+000012f0: 5f66 696e 616c 203d 2070 642e 636f 6e63  _final = pd.conc
+00001300: 6174 285b 585f 6669 6e61 6c2c 2063 6c61  at([X_final, cla
+00001310: 7373 5f64 665d 2c20 6967 6e6f 7265 5f69  ss_df], ignore_i
+00001320: 6e64 6578 3d54 7275 6529 0d0a 2020 2020  ndex=True)..    
+00001330: 2020 2020 2020 2020 2020 2020 795f 6669              y_fi
+00001340: 6e61 6c20 3d20 7064 2e63 6f6e 6361 7428  nal = pd.concat(
+00001350: 5b79 5f66 696e 616c 2c20 636c 6173 735f  [y_final, class_
+00001360: 7461 7267 6574 5d29 0d0a 2020 2020 2020  target])..      
+00001370: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00001380: 2020 2020 0d0a 2020 2020 2020 2020 0d0a      ..        ..
+00001390: 2020 2020 2020 2020 585f 6669 6e61 6c20          X_final 
+000013a0: 3d20 7365 6c66 2e5f 6765 745f 6669 6e61  = self._get_fina
+000013b0: 6c5f 6461 7461 6672 616d 6528 585f 6669  l_dataframe(X_fi
+000013c0: 6e61 6c2c 2070 726f 7465 6374 6564 5f61  nal, protected_a
+000013d0: 7474 7269 6275 7465 732c 2070 726f 7465  ttributes, prote
+000013e0: 6374 6564 5f61 7474 7269 6275 7465 290d  cted_attribute).
+000013f0: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+00001400: 6e20 585f 6669 6e61 6c2c 2079 5f66 696e  n X_final, y_fin
+00001410: 616c 0d0a 2020 2020 2020 2020 2020 2020  al..            
+00001420: 2020 2020 0d0a 636c 6173 7320 4d69 7469      ..class Miti
+00001430: 6761 746f 7228 7361 6e69 7479 5f63 6865  gator(sanity_che
+00001440: 636b 6572 2920 3a0d 0a0d 0a20 2020 2064  cker) :....    d
+00001450: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00001460: 2c20 6d65 7468 6f64 203d 2022 5261 6e64  , method = "Rand
+00001470: 6f6d 4f76 6572 5361 6d70 6c65 7222 2920  omOverSampler") 
+00001480: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00001490: 2020 2020 2020 2020 4d69 7469 6761 746f          Mitigato
+000014a0: 7220 696d 706c 656d 656e 7420 6469 6666  r implement diff
+000014b0: 6572 656e 7420 7479 7065 7320 6f66 2062  erent types of b
+000014c0: 6961 6973 206d 6974 6967 6174 696f 6e20  iais mitigation 
+000014d0: 6279 2072 6573 616d 706c 696e 672e 0d0a  by resampling...
+000014e0: 0d0a 2020 2020 2020 2020 4172 6773 3a0d  ..        Args:.
+000014f0: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+00001500: 686f 6420 2873 7472 2c20 6f70 7469 6f6e  hod (str, option
+00001510: 616c 293a 2072 6573 616d 706c 696e 6720  al): resampling 
+00001520: 6d65 7468 6f64 7320 696d 706c 656d 656e  methods implemen
+00001530: 7465 6420 6279 2069 6d62 6c65 6172 6e2e  ted by imblearn.
+00001540: 2050 6f73 7369 626c 6520 7661 6c75 6573   Possible values
+00001550: 2061 7265 2022 5261 6e64 6f6d 4f76 6572   are "RandomOver
+00001560: 5361 6d70 6c65 7222 2c20 0d0a 2020 2020  Sampler", ..    
+00001570: 2020 2020 2020 2020 2253 4d4f 5445 4e43          "SMOTENC
+00001580: 2220 616e 6420 2252 616e 646f 6d55 6e64  " and "RandomUnd
+00001590: 6572 5361 6d70 6c65 7222 2e20 2044 6566  erSampler".  Def
+000015a0: 6175 6c74 7320 746f 2022 5261 6e64 6f6d  aults to "Random
+000015b0: 4f76 6572 5361 6d70 6c65 7222 2e0d 0a20  OverSampler"... 
+000015c0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+000015d0: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
+000015e0: 6c66 2e5f 696e 6974 5f73 616e 6974 795f  lf._init_sanity_
+000015f0: 6368 6563 6b28 6d65 7468 6f64 290d 0a20  check(method).. 
+00001600: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00001610: 2073 656c 662e 6d65 7468 6f64 203d 206d   self.method = m
+00001620: 6574 686f 640d 0a20 2020 2020 2020 2073  ethod..        s
+00001630: 656c 662e 6d69 7469 6761 746f 725f 6675  elf.mitigator_fu
+00001640: 6e63 7469 6f6e 203d 207b 0d0a 2020 2020  nction = {..    
+00001650: 2020 2020 2020 2020 2252 616e 646f 6d4f          "RandomO
+00001660: 7665 7253 616d 706c 6572 2220 3a20 5261  verSampler" : Ra
+00001670: 6e64 6f6d 4f76 6572 5361 6d70 6c65 722c  ndomOverSampler,
+00001680: 0d0a 2020 2020 2020 2020 2020 2020 2022  ..             "
+00001690: 534d 4f54 454e 4322 203a 2053 4d4f 5445  SMOTENC" : SMOTE
+000016a0: 4e43 2c0d 0a20 2020 2020 2020 2020 2020  NC,..           
+000016b0: 2020 2252 616e 646f 6d55 6e64 6572 5361    "RandomUnderSa
+000016c0: 6d70 6c65 7222 203a 2052 616e 646f 6d55  mpler" : RandomU
+000016d0: 6e64 6572 5361 6d70 6c65 720d 0a20 2020  nderSampler..   
+000016e0: 2020 2020 207d 0d0a 2020 2020 0d0a 2020       }..    ..  
+000016f0: 2020 6465 6620 5f69 6e69 745f 7361 6e69    def _init_sani
+00001700: 7479 5f63 6865 636b 2873 656c 662c 206d  ty_check(self, m
+00001710: 6574 686f 6429 203a 0d0a 2020 2020 2020  ethod) :..      
+00001720: 2020 6173 7365 7274 206d 6574 686f 6420    assert method 
+00001730: 696e 2053 414d 504c 494e 475f 4655 4e43  in SAMPLING_FUNC
+00001740: 5449 4f4e 532c 2066 226d 6574 686f 6420  TIONS, f"method 
+00001750: 6e65 6564 2074 6f20 6265 2069 6e20 7b53  need to be in {S
+00001760: 414d 504c 494e 475f 4655 4e43 5449 4f4e  AMPLING_FUNCTION
+00001770: 537d 220d 0a0d 0a20 2020 200d 0a20 2020  S}"....    ..   
+00001780: 2064 6566 206d 6974 6967 6174 6528 7365   def mitigate(se
+00001790: 6c66 2c20 6d69 7469 6761 7469 6f6e 5f73  lf, mitigation_s
+000017a0: 7472 6174 6567 793a 2073 7472 2c20 6461  trategy: str, da
+000017b0: 7461 7365 743a 2070 642e 4461 7461 4672  taset: pd.DataFr
+000017c0: 616d 652c 2074 6172 6765 743a 2073 7472  ame, target: str
+000017d0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+000017e0: 2020 2020 2070 726f 7465 6374 6564 5f61       protected_a
+000017f0: 7474 7269 6275 7465 733a 206c 6973 7420  ttributes: list 
+00001800: 3d20 4e6f 6e65 2c20 636f 6e74 5f63 6f6c  = None, cont_col
+00001810: 756d 6e73 3a20 6c69 7374 203d 204e 6f6e  umns: list = Non
+00001820: 652c 2063 6174 5f63 6f6c 756d 6e73 3a20  e, cat_columns: 
+00001830: 6c69 7374 203d 204e 6f6e 6529 203a 0d0a  list = None) :..
+00001840: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00001850: 2020 2020 204d 6974 6967 6174 6520 6269       Mitigate bi
+00001860: 6173 2075 7369 6e67 2074 6865 2067 6976  as using the giv
+00001870: 656e 206d 6974 6967 6174 696f 6e20 7374  en mitigation st
+00001880: 7261 7465 6779 0d0a 0d0a 2020 2020 2020  rategy....      
+00001890: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
+000018a0: 2020 2020 206d 6974 6967 6174 696f 6e5f       mitigation_
+000018b0: 7374 7261 7465 6779 2028 7374 7229 3a20  strategy (str): 
+000018c0: 7468 6520 6d69 7469 6761 7469 6f6e 2073  the mitigation s
+000018d0: 7472 6174 6567 7920 746f 2075 7365 2e20  trategy to use. 
+000018e0: 506f 7373 6962 6c65 2076 616c 7565 7320  Possible values 
+000018f0: 6172 6520 2262 616c 616e 655f 6f75 7470  are "balane_outp
+00001900: 7574 222c 2022 6261 6c61 6e63 655f 7072  ut", "balance_pr
+00001910: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
+00001920: 6522 2c20 2262 616c 616e 6365 5f6f 7574  e", "balance_out
+00001930: 7075 7420 666f 7220 6174 7472 6962 7574  put for attribut
+00001940: 6522 2061 6e64 2022 6261 6c61 6e63 655f  e" and "balance_
+00001950: 616c 6c22 2e20 0d0a 2020 2020 2020 2020  all". ..        
+00001960: 2020 2020 226e 6f6e 6522 2069 7320 616c      "none" is al
+00001970: 736f 2069 6d70 6c65 6d65 6e74 6564 2066  so implemented f
+00001980: 6f72 2062 656e 6368 6d61 726b 696e 6720  or benchmarking 
+00001990: 636f 6e73 6973 7465 6e63 7920 616e 6420  consistency and 
+000019a0: 7369 6d70 6c79 2072 6574 7572 6e20 7468  simply return th
+000019b0: 6520 696e 6974 6961 6c20 6461 7461 7365  e initial datase
+000019c0: 7420 616e 6420 7461 7267 6574 2e20 0d0a  t and target. ..
+000019d0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+000019e0: 7365 7420 2870 642e 4461 7461 4672 616d  set (pd.DataFram
+000019f0: 6529 3a20 6461 7461 7365 7420 746f 206d  e): dataset to m
+00001a00: 6974 6967 6174 652c 2074 6861 7420 696e  itigate, that in
+00001a10: 636c 7564 6573 2074 6865 2074 6172 6765  cludes the targe
+00001a20: 7420 636f 6c75 6d6e 2e0d 0a20 2020 2020  t column...     
+00001a30: 2020 2020 2020 2074 6172 6765 7420 2873         target (s
+00001a40: 7472 293a 2074 6865 2074 6172 6765 7420  tr): the target 
+00001a50: 636f 6c75 6d6e 206e 616d 650d 0a20 2020  column name..   
+00001a60: 2020 2020 2020 2020 2070 726f 7465 6374           protect
+00001a70: 6564 5f61 7474 7269 6275 7465 7320 286c  ed_attributes (l
+00001a80: 6973 742c 206f 7074 696f 6e61 6c29 3a20  ist, optional): 
+00001a90: 5468 6520 6174 7472 6962 7574 6528 7329  The attribute(s)
+00001aa0: 2074 6f20 6261 6c61 6e63 652e 204f 6e6c   to balance. Onl
+00001ab0: 7920 6e65 6365 7373 6172 7920 666f 7220  y necessary for 
+00001ac0: 6261 6c61 6e63 655f 7072 6f74 6563 7465  balance_protecte
+00001ad0: 645f 6174 7472 6962 7574 6520 616e 6420  d_attribute and 
+00001ae0: 6261 6c61 6e63 655f 6f75 7470 7574 5f66  balance_output_f
+00001af0: 6f72 5f61 7474 7269 6275 7465 2e20 4465  or_attribute. De
+00001b00: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0d  faults to None..
+00001b10: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00001b20: 745f 636f 6c75 6d6e 7320 286c 6973 742c  t_columns (list,
+00001b30: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+00001b40: 636f 6e74 696e 756f 7573 2063 6f6c 756d  continuous colum
+00001b50: 6e73 2069 6e20 7468 6520 6461 7461 7365  ns in the datase
+00001b60: 742e 204f 6e6c 7920 4e65 6365 7373 6172  t. Only Necessar
+00001b70: 7920 6966 2074 6865 2073 616d 706c 696e  y if the samplin
+00001b80: 6720 7374 7261 7465 6779 2069 7320 534d  g strategy is SM
+00001b90: 4f54 454e 432e 2044 6566 6175 6c74 7320  OTENC. Defaults 
+00001ba0: 746f 204e 6f6e 652e 0d0a 2020 2020 2020  to None...      
+00001bb0: 2020 2020 2020 6361 745f 636f 6c75 6d6e        cat_column
+00001bc0: 7320 286c 6973 742c 206f 7074 696f 6e61  s (list, optiona
+00001bd0: 6c29 3a20 5468 6520 6361 7465 676f 7269  l): The categori
+00001be0: 6361 6c20 636f 6c75 6d6e 7320 696e 2074  cal columns in t
+00001bf0: 6865 2064 6174 6173 6574 2e20 4f6e 6c79  he dataset. Only
+00001c00: 204e 6563 6573 7361 7279 2069 6620 7468   Necessary if th
+00001c10: 6520 7361 6d70 6c69 6e67 2073 7472 6174  e sampling strat
+00001c20: 6567 7920 6973 2053 4d4f 5445 4e43 2e20  egy is SMOTENC. 
+00001c30: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
+00001c40: 2e0d 0a0d 0a20 2020 2020 2020 2052 6169  .....        Rai
+00001c50: 7365 733a 0d0a 2020 2020 2020 2020 2020  ses:..          
+00001c60: 2020 5661 6c75 6545 7272 6f72 3a20 4966    ValueError: If
+00001c70: 2074 6865 206d 6974 6967 6174 696f 6e20   the mitigation 
+00001c80: 7374 7261 7465 6779 2064 6f65 7320 6e6f  strategy does no
+00001c90: 7420 6578 6973 740d 0a0d 0a20 2020 2020  t exist....     
+00001ca0: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
+00001cb0: 2020 2020 2020 2020 2028 5b70 642e 4461           ([pd.Da
+00001cc0: 7461 4672 616d 652c 2070 642e 4461 7461  taFrame, pd.Data
+00001cd0: 4672 616d 655d 293a 2074 6865 2062 616c  Frame]): the bal
+00001ce0: 616e 6365 6420 6461 7461 6672 616d 6573  anced dataframes
+00001cf0: 2066 6f72 2074 6865 2064 6174 6173 6574   for the dataset
+00001d00: 2061 6e64 2074 6865 2074 6172 6765 740d   and the target.
+00001d10: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00001d20: 2020 2020 2020 6966 206d 6974 6967 6174        if mitigat
+00001d30: 696f 6e5f 7374 7261 7465 6779 203d 3d20  ion_strategy == 
+00001d40: 2262 616c 616e 6365 5f6f 7574 7075 7422  "balance_output"
+00001d50: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
+00001d60: 7265 7475 726e 2073 656c 662e 6261 6c61  return self.bala
+00001d70: 6e63 655f 6f75 7470 7574 2864 6174 6173  nce_output(datas
+00001d80: 6574 2c20 7461 7267 6574 2c20 7072 6f74  et, target, prot
+00001d90: 6563 7465 645f 6174 7472 6962 7574 6573  ected_attributes
+00001da0: 2c20 636f 6e74 5f63 6f6c 756d 6e73 2c20  , cont_columns, 
+00001db0: 6361 745f 636f 6c75 6d6e 7329 0d0a 2020  cat_columns)..  
+00001dc0: 2020 2020 2020 656c 6966 206d 6974 6967        elif mitig
+00001dd0: 6174 696f 6e5f 7374 7261 7465 6779 203d  ation_strategy =
+00001de0: 3d20 2262 616c 616e 6365 5f70 726f 7465  = "balance_prote
+00001df0: 6374 6564 5f61 7474 7269 6275 7465 2220  cted_attribute" 
+00001e00: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00001e10: 6574 7572 6e20 7365 6c66 2e62 616c 616e  eturn self.balan
+00001e20: 6365 5f70 726f 7465 6374 6564 5f61 7474  ce_protected_att
+00001e30: 7269 6275 7465 2864 6174 6173 6574 2c20  ribute(dataset, 
+00001e40: 7461 7267 6574 2c20 7072 6f74 6563 7465  target, protecte
+00001e50: 645f 6174 7472 6962 7574 6573 2c20 636f  d_attributes, co
+00001e60: 6e74 5f63 6f6c 756d 6e73 2c20 6361 745f  nt_columns, cat_
+00001e70: 636f 6c75 6d6e 7329 0d0a 2020 2020 2020  columns)..      
+00001e80: 2020 656c 6966 206d 6974 6967 6174 696f    elif mitigatio
+00001e90: 6e5f 7374 7261 7465 6779 203d 3d20 2262  n_strategy == "b
+00001ea0: 616c 616e 6365 5f6f 7574 7075 745f 666f  alance_output_fo
+00001eb0: 725f 6174 7472 6962 7574 6522 203a 0d0a  r_attribute" :..
+00001ec0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00001ed0: 726e 2073 656c 662e 6261 6c61 6e63 655f  rn self.balance_
+00001ee0: 6f75 7470 7574 5f66 6f72 5f61 7474 7269  output_for_attri
+00001ef0: 6275 7465 2864 6174 6173 6574 2c20 7461  bute(dataset, ta
+00001f00: 7267 6574 2c20 7072 6f74 6563 7465 645f  rget, protected_
+00001f10: 6174 7472 6962 7574 6573 2c20 636f 6e74  attributes, cont
+00001f20: 5f63 6f6c 756d 6e73 2c20 6361 745f 636f  _columns, cat_co
+00001f30: 6c75 6d6e 7329 0d0a 2020 2020 2020 2020  lumns)..        
+00001f40: 656c 6966 206d 6974 6967 6174 696f 6e5f  elif mitigation_
+00001f50: 7374 7261 7465 6779 203d 3d20 2262 616c  strategy == "bal
+00001f60: 616e 6365 5f61 6c6c 2220 3a0d 0a20 2020  ance_all" :..   
+00001f70: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001f80: 7365 6c66 2e62 616c 616e 6365 5f61 6c6c  self.balance_all
+00001f90: 2864 6174 6173 6574 2c20 7461 7267 6574  (dataset, target
+00001fa0: 2c20 7072 6f74 6563 7465 645f 6174 7472  , protected_attr
+00001fb0: 6962 7574 6573 2c20 636f 6e74 5f63 6f6c  ibutes, cont_col
+00001fc0: 756d 6e73 2c20 6361 745f 636f 6c75 6d6e  umns, cat_column
+00001fd0: 7329 0d0a 2020 2020 2020 2020 656c 6966  s)..        elif
+00001fe0: 206d 6974 6967 6174 696f 6e5f 7374 7261   mitigation_stra
+00001ff0: 7465 6779 203d 3d20 226e 6f6e 6522 203a  tegy == "none" :
+00002000: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00002010: 7475 726e 2064 6174 6173 6574 2c20 7461  turn dataset, ta
+00002020: 7267 6574 0d0a 2020 2020 2020 2020 656c  rget..        el
+00002030: 7365 203a 0d0a 2020 2020 2020 2020 2020  se :..          
+00002040: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00002050: 6f72 0d0a 2020 2020 2020 2020 0d0a 2020  or..        ..  
+00002060: 2020 6465 6620 6261 6c61 6e63 655f 6f75    def balance_ou
+00002070: 7470 7574 2873 656c 662c 2064 6174 6173  tput(self, datas
+00002080: 6574 3a20 7064 2e44 6174 6146 7261 6d65  et: pd.DataFrame
+00002090: 2c20 7461 7267 6574 3a20 7374 722c 2070  , target: str, p
+000020a0: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
+000020b0: 7465 733a 206c 6973 7420 3d20 4e6f 6e65  tes: list = None
+000020c0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+000020d0: 2020 2020 2020 2020 2020 2063 6f6e 745f             cont_
+000020e0: 636f 6c75 6d6e 733a 206c 6973 7420 3d20  columns: list = 
+000020f0: 4e6f 6e65 2c20 6361 745f 636f 6c75 6d6e  None, cat_column
+00002100: 733a 206c 6973 7420 3d20 4e6f 6e65 2920  s: list = None) 
+00002110: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00002120: 2020 2020 2020 2020 4261 6c61 6e63 6520          Balance 
+00002130: 7468 6520 6f75 7470 7574 2077 6974 6820  the output with 
+00002140: 6e6f 2072 6567 6172 6473 2074 6f20 7468  no regards to th
+00002150: 6520 7072 6f74 6563 7465 6420 6174 7472  e protected attr
+00002160: 6962 7574 6573 2e0d 0a20 2020 2020 2020  ibutes...       
+00002170: 200d 0a20 2020 2020 2020 2041 7267 733a   ..        Args:
+00002180: 200d 0a20 2020 2020 2020 2020 2020 2064   ..            d
+00002190: 6174 6173 6574 2028 7064 2e44 6174 6146  ataset (pd.DataF
+000021a0: 7261 6d65 293a 2064 6174 6173 6574 2074  rame): dataset t
+000021b0: 6f20 6d69 7469 6761 7465 2c20 7468 6174  o mitigate, that
+000021c0: 2069 6e63 6c75 6465 7320 7468 6520 7461   includes the ta
+000021d0: 7267 6574 2063 6f6c 756d 6e2e 0d0a 2020  rget column...  
+000021e0: 2020 2020 2020 2020 2020 7461 7267 6574            target
+000021f0: 2028 7374 7229 3a20 7468 6520 7461 7267   (str): the targ
+00002200: 6574 2063 6f6c 756d 6e20 6e61 6d65 0d0a  et column name..
+00002210: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
+00002220: 6563 7465 645f 6174 7472 6962 7574 6573  ected_attributes
+00002230: 2028 6c69 7374 2c20 6f70 7469 6f6e 616c   (list, optional
+00002240: 293a 2055 7365 6c65 7373 2066 6f72 2074  ): Useless for t
+00002250: 6869 7320 6d69 7469 6761 7469 6f6e 2073  his mitigation s
+00002260: 7472 6174 6567 792c 2062 7574 2069 6d70  trategy, but imp
+00002270: 6c65 6d65 6e74 6564 2066 6f72 2041 5049  lemented for API
+00002280: 2063 6f6e 7369 7374 656e 6379 2e20 4465   consistency. De
+00002290: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0d  faults to None..
+000022a0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+000022b0: 745f 636f 6c75 6d6e 7320 286c 6973 742c  t_columns (list,
+000022c0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+000022d0: 636f 6e74 696e 756f 7573 2063 6f6c 756d  continuous colum
+000022e0: 6e73 2069 6e20 7468 6520 6461 7461 7365  ns in the datase
+000022f0: 742e 204f 6e6c 7920 4e65 6365 7373 6172  t. Only Necessar
+00002300: 7920 6966 2074 6865 2073 616d 706c 696e  y if the samplin
+00002310: 6720 7374 7261 7465 6779 2069 7320 534d  g strategy is SM
+00002320: 4f54 454e 432e 2044 6566 6175 6c74 7320  OTENC. Defaults 
+00002330: 746f 204e 6f6e 652e 0d0a 2020 2020 2020  to None...      
+00002340: 2020 2020 2020 6361 745f 636f 6c75 6d6e        cat_column
+00002350: 7320 286c 6973 742c 206f 7074 696f 6e61  s (list, optiona
+00002360: 6c29 3a20 5468 6520 6361 7465 676f 7269  l): The categori
+00002370: 6361 6c20 636f 6c75 6d6e 7320 696e 2074  cal columns in t
+00002380: 6865 2064 6174 6173 6574 2e20 4f6e 6c79  he dataset. Only
+00002390: 204e 6563 6573 7361 7279 2069 6620 7468   Necessary if th
+000023a0: 6520 7361 6d70 6c69 6e67 2073 7472 6174  e sampling strat
+000023b0: 6567 7920 6973 2053 4d4f 5445 4e43 2e20  egy is SMOTENC. 
+000023c0: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
+000023d0: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
+000023e0: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
+000023f0: 2020 2028 5b70 642e 4461 7461 4672 616d     ([pd.DataFram
+00002400: 652c 2070 642e 4461 7461 4672 616d 655d  e, pd.DataFrame]
+00002410: 293a 2074 6865 2062 616c 616e 6365 6420  ): the balanced 
+00002420: 6461 7461 6672 616d 6573 2066 6f72 2074  dataframes for t
+00002430: 6865 2064 6174 6173 6574 2061 6e64 2074  he dataset and t
+00002440: 6865 2074 6172 6765 740d 0a20 2020 2020  he target..     
+00002450: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00002460: 7375 7065 7228 292e 5f73 616e 6974 795f  super()._sanity_
+00002470: 6368 6563 6b28 6461 7461 7365 742c 2074  check(dataset, t
+00002480: 6172 6765 742c 2070 726f 7465 6374 6564  arget, protected
+00002490: 5f61 7474 7269 6275 7465 733d 7072 6f74  _attributes=prot
+000024a0: 6563 7465 645f 6174 7472 6962 7574 6573  ected_attributes
+000024b0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
+000024c0: 2020 2020 2023 6966 206e 6f74 2052 616e       #if not Ran
+000024d0: 646f 6d4f 7665 7253 616d 706c 6572 2c20  domOverSampler, 
+000024e0: 6e65 6564 2074 6f20 6f6e 652d 686f 7420  need to one-hot 
+000024f0: 656e 636f 6465 2065 7665 7279 2063 6174  encode every cat
+00002500: 6567 6f72 6963 616c 0d0a 2020 2020 2020  egorical..      
+00002510: 2020 6466 203d 2064 6174 6173 6574 2e63    df = dataset.c
+00002520: 6f70 7928 290d 0a20 2020 2020 2020 2074  opy()..        t
+00002530: 6172 6765 745f 6466 203d 2064 665b 7461  arget_df = df[ta
+00002540: 7267 6574 5d0d 0a20 2020 2020 2020 2064  rget]..        d
+00002550: 6620 3d20 6466 2e64 726f 7028 636f 6c75  f = df.drop(colu
+00002560: 6d6e 733d 7461 7267 6574 290d 0a20 2020  mns=target)..   
+00002570: 2020 2020 200d 0a20 2020 2020 2020 200d       ..        .
+00002580: 0a20 2020 2020 2020 2069 6620 7072 6f74  .        if prot
+00002590: 6563 7465 645f 6174 7472 6962 7574 6573  ected_attributes
+000025a0: 2061 6e64 206c 656e 2870 726f 7465 6374   and len(protect
+000025b0: 6564 5f61 7474 7269 6275 7465 7329 203e  ed_attributes) >
+000025c0: 2031 203a 0d0a 2020 2020 2020 2020 2020   1 :..          
+000025d0: 2020 6466 2c20 7072 6f74 6563 7465 645f    df, protected_
+000025e0: 6174 7472 6962 7574 6520 3d20 7365 6c66  attribute = self
+000025f0: 2e5f 6d61 6b65 5f73 7570 6572 5f70 726f  ._make_super_pro
+00002600: 7465 6374 6564 2864 6174 6173 6574 2c20  tected(dataset, 
+00002610: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
+00002620: 7574 6573 290d 0a20 2020 2020 2020 200d  utes)..        .
+00002630: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00002640: 2e6d 6574 686f 6420 696e 205b 2253 4d4f  .method in ["SMO
+00002650: 5445 4e43 225d 203a 0d0a 2020 2020 2020  TENC"] :..      
+00002660: 2020 2020 2020 2370 726f 6365 7373 0d0a        #process..
+00002670: 2020 2020 2020 2020 2020 2020 7072 6f63              proc
+00002680: 6573 736f 7220 3d20 5f50 726f 6365 7373  essor = _Process
+00002690: 6f72 2829 0d0a 2020 2020 2020 2020 2020  or()..          
+000026a0: 2020 7072 6f63 6573 7365 645f 6466 3d20    processed_df= 
+000026b0: 7072 6f63 6573 736f 722e 7072 6f63 6573  processor.proces
+000026c0: 7328 6466 2c20 7363 616c 655f 636f 6c73  s(df, scale_cols
+000026d0: 3d63 6f6e 745f 636f 6c75 6d6e 732c 2065  =cont_columns, e
+000026e0: 6e63 6f64 655f 636f 6c73 3d63 6174 5f63  ncode_cols=cat_c
+000026f0: 6f6c 756d 6e73 290d 0a0d 0a20 2020 2020  olumns)....     
+00002700: 2020 2020 2020 2023 2054 6865 6e20 7265         # Then re
+00002710: 7361 6d70 6c65 0d0a 2020 2020 2020 2020  sample..        
+00002720: 2020 2020 6361 745f 636f 6c75 6d6e 735f      cat_columns_
+00002730: 6964 7320 3d20 5b70 726f 6365 7373 6564  ids = [processed
+00002740: 5f64 662e 636f 6c75 6d6e 732e 6765 745f  _df.columns.get_
+00002750: 6c6f 6328 636f 6c5f 6e61 6d65 2920 666f  loc(col_name) fo
+00002760: 7220 636f 6c5f 6e61 6d65 2069 6e20 6361  r col_name in ca
+00002770: 745f 636f 6c75 6d6e 735d 0d0a 2020 2020  t_columns]..    
+00002780: 2020 2020 2020 2020 7361 6d70 6c65 7220          sampler 
+00002790: 3d20 7365 6c66 2e6d 6974 6967 6174 6f72  = self.mitigator
+000027a0: 5f66 756e 6374 696f 6e5b 7365 6c66 2e6d  _function[self.m
+000027b0: 6574 686f 645d 2863 6174 5f63 6f6c 756d  ethod](cat_colum
+000027c0: 6e73 5f69 6473 290d 0a20 2020 2020 2020  ns_ids)..       
+000027d0: 2020 2020 2058 5f72 6573 616d 706c 6564       X_resampled
+000027e0: 2c20 795f 7265 7361 6d70 6c65 6420 3d20  , y_resampled = 
+000027f0: 7361 6d70 6c65 722e 6669 745f 7265 7361  sampler.fit_resa
+00002800: 6d70 6c65 2870 726f 6365 7373 6564 5f64  mple(processed_d
+00002810: 662c 2074 6172 6765 745f 6466 290d 0a20  f, target_df).. 
+00002820: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00002830: 2020 2020 2020 2020 2023 2054 6865 6e20           # Then 
+00002840: 756e 7072 6f63 6573 7320 6974 0d0a 2020  unprocess it..  
+00002850: 2020 2020 2020 2020 2020 6466 5f66 696e            df_fin
+00002860: 616c 203d 2070 726f 6365 7373 6f72 2e75  al = processor.u
+00002870: 6e70 726f 6365 7373 2858 5f72 6573 616d  nprocess(X_resam
+00002880: 706c 6564 290d 0a20 2020 2020 2020 2020  pled)..         
+00002890: 2020 2074 6172 6765 745f 6669 6e61 6c20     target_final 
+000028a0: 3d20 795f 7265 7361 6d70 6c65 640d 0a0d  = y_resampled...
+000028b0: 0a20 2020 2020 2020 2065 6c73 6520 3a0d  .        else :.
+000028c0: 0a20 2020 2020 2020 2020 2020 2023 6a75  .            #ju
+000028d0: 7374 2072 6573 616d 706c 6572 0d0a 2020  st resampler..  
+000028e0: 2020 2020 2020 2020 2020 7361 6d70 6c65            sample
+000028f0: 7220 3d20 7365 6c66 2e6d 6974 6967 6174  r = self.mitigat
+00002900: 6f72 5f66 756e 6374 696f 6e5b 7365 6c66  or_function[self
+00002910: 2e6d 6574 686f 645d 2829 0d0a 2020 2020  .method]()..    
+00002920: 2020 2020 2020 2020 6466 5f66 696e 616c          df_final
+00002930: 2c20 7461 7267 6574 5f66 696e 616c 203d  , target_final =
+00002940: 2073 616d 706c 6572 2e66 6974 5f72 6573   sampler.fit_res
+00002950: 616d 706c 6528 6466 2c20 7461 7267 6574  ample(df, target
+00002960: 5f64 6629 0d0a 2020 2020 2020 2020 0d0a  _df)..        ..
+00002970: 2020 2020 2020 2020 6966 2070 726f 7465          if prote
+00002980: 6374 6564 5f61 7474 7269 6275 7465 7320  cted_attributes 
+00002990: 616e 6420 6c65 6e28 7072 6f74 6563 7465  and len(protecte
+000029a0: 645f 6174 7472 6962 7574 6573 2920 3e20  d_attributes) > 
+000029b0: 3120 3a0d 0a20 2020 2020 2020 2020 2020  1 :..           
+000029c0: 2064 665f 6669 6e61 6c20 3d20 6466 5f66   df_final = df_f
+000029d0: 696e 616c 2e64 726f 7028 636f 6c75 6d6e  inal.drop(column
+000029e0: 7320 3d20 7072 6f74 6563 7465 645f 6174  s = protected_at
+000029f0: 7472 6962 7574 6529 0d0a 2020 2020 2020  tribute)..      
+00002a00: 2020 0d0a 2020 2020 2020 2020 7265 7475    ..        retu
+00002a10: 726e 2064 665f 6669 6e61 6c2c 2074 6172  rn df_final, tar
+00002a20: 6765 745f 6669 6e61 6c0d 0a20 2020 2020  get_final..     
+00002a30: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
+00002a40: 2062 616c 616e 6365 5f70 726f 7465 6374   balance_protect
+00002a50: 6564 5f61 7474 7269 6275 7465 2873 656c  ed_attribute(sel
+00002a60: 662c 2064 6174 6173 6574 3a20 7064 2e44  f, dataset: pd.D
+00002a70: 6174 6146 7261 6d65 2c20 7461 7267 6574  ataFrame, target
+00002a80: 3a20 7374 722c 2070 726f 7465 6374 6564  : str, protected
+00002a90: 5f61 7474 7269 6275 7465 733a 206c 6973  _attributes: lis
+00002aa0: 742c 200d 0a20 2020 2020 2020 2020 2020  t, ..           
+00002ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ac0: 2020 2020 2020 2020 2063 6f6e 745f 636f           cont_co
+00002ad0: 6c75 6d6e 733a 206c 6973 7420 3d20 4e6f  lumns: list = No
+00002ae0: 6e65 2c20 6361 745f 636f 6c75 6d6e 733a  ne, cat_columns:
+00002af0: 206c 6973 7420 3d20 4e6f 6e65 2920 3a0d   list = None) :.
+00002b00: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00002b10: 2020 2020 2020 4261 6c61 6e63 6520 7468        Balance th
+00002b20: 6520 636c 6173 7365 7320 6f66 2061 2070  e classes of a p
+00002b30: 726f 7465 6374 6564 2061 7474 7269 6275  rotected attribu
+00002b40: 7465 2077 6974 6820 6e6f 2072 6567 6172  te with no regar
+00002b50: 6473 2074 6f20 7468 6520 6f75 7470 7574  ds to the output
+00002b60: 2e20 5c6e 0d0a 2020 2020 2020 2020 5368  . \n..        Sh
+00002b70: 6f75 6c64 2069 6d70 726f 7665 2074 6865  ould improve the
+00002b80: 2062 616c 616e 6365 2066 6f72 2074 6865   balance for the
+00002b90: 2070 726f 7465 6374 6564 2061 7474 7269   protected attri
+00002ba0: 6275 7465 2e0d 0a20 2020 2020 2020 200d  bute...        .
+00002bb0: 0a20 2020 2020 2020 2041 7267 733a 200d  .        Args: .
+00002bc0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00002bd0: 6173 6574 2028 7064 2e44 6174 6146 7261  aset (pd.DataFra
+00002be0: 6d65 293a 2064 6174 6173 6574 2074 6f20  me): dataset to 
+00002bf0: 6d69 7469 6761 7465 2c20 7468 6174 2069  mitigate, that i
+00002c00: 6e63 6c75 6465 7320 7468 6520 7461 7267  ncludes the targ
+00002c10: 6574 2063 6f6c 756d 6e2e 0d0a 2020 2020  et column...    
+00002c20: 2020 2020 2020 2020 7461 7267 6574 2028          target (
+00002c30: 7374 7229 3a20 7468 6520 7461 7267 6574  str): the target
+00002c40: 2063 6f6c 756d 6e20 6e61 6d65 0d0a 2020   column name..  
+00002c50: 2020 2020 2020 2020 2020 7072 6f74 6563            protec
+00002c60: 7465 645f 6174 7472 6962 7574 6573 2028  ted_attributes (
+00002c70: 6c69 7374 2c20 6f70 7469 6f6e 616c 293a  list, optional):
+00002c80: 2054 6865 2061 7474 7269 6275 7465 2873   The attribute(s
+00002c90: 2920 746f 2062 616c 616e 6365 2e20 4465  ) to balance. De
+00002ca0: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0d  faults to None..
+00002cb0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00002cc0: 745f 636f 6c75 6d6e 7320 286c 6973 742c  t_columns (list,
+00002cd0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+00002ce0: 636f 6e74 696e 756f 7573 2063 6f6c 756d  continuous colum
+00002cf0: 6e73 2069 6e20 7468 6520 6461 7461 7365  ns in the datase
+00002d00: 742e 204f 6e6c 7920 4e65 6365 7373 6172  t. Only Necessar
+00002d10: 7920 6966 2074 6865 2073 616d 706c 696e  y if the samplin
+00002d20: 6720 7374 7261 7465 6779 2069 7320 534d  g strategy is SM
+00002d30: 4f54 454e 432e 2044 6566 6175 6c74 7320  OTENC. Defaults 
+00002d40: 746f 204e 6f6e 652e 0d0a 2020 2020 2020  to None...      
+00002d50: 2020 2020 2020 6361 745f 636f 6c75 6d6e        cat_column
+00002d60: 7320 286c 6973 742c 206f 7074 696f 6e61  s (list, optiona
+00002d70: 6c29 3a20 5468 6520 6361 7465 676f 7269  l): The categori
+00002d80: 6361 6c20 636f 6c75 6d6e 7320 696e 2074  cal columns in t
+00002d90: 6865 2064 6174 6173 6574 2e20 4f6e 6c79  he dataset. Only
+00002da0: 204e 6563 6573 7361 7279 2069 6620 7468   Necessary if th
+00002db0: 6520 7361 6d70 6c69 6e67 2073 7472 6174  e sampling strat
+00002dc0: 6567 7920 6973 2053 4d4f 5445 4e43 2e20  egy is SMOTENC. 
+00002dd0: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
+00002de0: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
+00002df0: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
+00002e00: 2020 2028 5b70 642e 4461 7461 4672 616d     ([pd.DataFram
+00002e10: 652c 2070 642e 4461 7461 4672 616d 655d  e, pd.DataFrame]
+00002e20: 293a 2074 6865 2062 616c 616e 6365 6420  ): the balanced 
+00002e30: 6461 7461 6672 616d 6573 2066 6f72 2074  dataframes for t
+00002e40: 6865 2064 6174 6173 6574 2061 6e64 2074  he dataset and t
+00002e50: 6865 2074 6172 6765 740d 0a20 2020 2020  he target..     
+00002e60: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00002e70: 7375 7065 7228 292e 5f73 616e 6974 795f  super()._sanity_
+00002e80: 6368 6563 6b28 6461 7461 7365 742c 2074  check(dataset, t
+00002e90: 6172 6765 742c 2070 726f 7465 6374 6564  arget, protected
+00002ea0: 5f61 7474 7269 6275 7465 733d 7072 6f74  _attributes=prot
+00002eb0: 6563 7465 645f 6174 7472 6962 7574 6573  ected_attributes
+00002ec0: 290d 0a20 2020 2020 2020 2064 6620 3d20  )..        df = 
+00002ed0: 6461 7461 7365 742e 636f 7079 2829 0d0a  dataset.copy()..
+00002ee0: 2020 2020 2020 2020 7461 7267 6574 5f64          target_d
+00002ef0: 6620 3d20 6466 5b74 6172 6765 745d 0d0a  f = df[target]..
+00002f00: 2020 2020 2020 2020 6466 203d 2064 662e          df = df.
+00002f10: 6472 6f70 2863 6f6c 756d 6e73 3d74 6172  drop(columns=tar
+00002f20: 6765 7429 0d0a 0d0a 2020 2020 2020 2020  get)....        
+00002f30: 6966 206c 656e 2870 726f 7465 6374 6564  if len(protected
+00002f40: 5f61 7474 7269 6275 7465 7329 203e 2031  _attributes) > 1
+00002f50: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
+00002f60: 6466 2c20 7072 6f74 6563 7465 645f 6174  df, protected_at
+00002f70: 7472 6962 7574 6520 3d20 7365 6c66 2e5f  tribute = self._
+00002f80: 6d61 6b65 5f73 7570 6572 5f70 726f 7465  make_super_prote
+00002f90: 6374 6564 2864 6174 6173 6574 2c20 7072  cted(dataset, pr
+00002fa0: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
+00002fb0: 6573 290d 0a20 2020 2020 2020 2065 6c73  es)..        els
+00002fc0: 6520 3a0d 0a20 2020 2020 2020 2020 2020  e :..           
+00002fd0: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
+00002fe0: 6275 7465 203d 2070 726f 7465 6374 6564  bute = protected
+00002ff0: 5f61 7474 7269 6275 7465 735b 305d 0d0a  _attributes[0]..
+00003000: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00003010: 662e 6d65 7468 6f64 2069 6e20 5b22 534d  f.method in ["SM
+00003020: 4f54 454e 4322 5d20 3a0d 0a20 2020 2020  OTENC"] :..     
+00003030: 2020 2020 2020 2023 7072 6570 726f 6365         #preproce
+00003040: 7373 2075 7369 6e67 2074 6865 2070 726f  ss using the pro
+00003050: 7465 6374 6564 2061 7474 7269 6275 7465  tected attribute
+00003060: 2061 7320 6120 7461 7267 6574 0d0a 2020   as a target..  
+00003070: 2020 2020 2020 2020 2020 636f 6e74 5f63            cont_c
+00003080: 6f6c 5f62 7566 6620 3d20 5b66 6561 7475  ol_buff = [featu
+00003090: 7265 2066 6f72 2066 6561 7475 7265 2069  re for feature i
+000030a0: 6e20 636f 6e74 5f63 6f6c 756d 6e73 2069  n cont_columns i
+000030b0: 6620 6665 6174 7572 6520 213d 2070 726f  f feature != pro
+000030c0: 7465 6374 6564 5f61 7474 7269 6275 7465  tected_attribute
+000030d0: 5d0d 0a20 2020 2020 2020 2020 2020 2063  ]..            c
+000030e0: 6174 5f63 6f6c 5f62 7566 6620 3d20 5b66  at_col_buff = [f
+000030f0: 6561 7475 7265 2066 6f72 2066 6561 7475  eature for featu
+00003100: 7265 2069 6e20 6361 745f 636f 6c75 6d6e  re in cat_column
+00003110: 7320 6966 2066 6561 7475 7265 2021 3d20  s if feature != 
+00003120: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
+00003130: 7574 655d 0d0a 2020 2020 2020 2020 2020  ute]..          
+00003140: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00003150: 7072 6f63 6573 736f 7220 3d20 5f50 726f  processor = _Pro
+00003160: 6365 7373 6f72 2829 0d0a 2020 2020 2020  cessor()..      
+00003170: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00003180: 2020 2020 7072 6f63 6573 7365 645f 6466      processed_df
+00003190: 203d 2070 726f 6365 7373 6f72 2e70 726f   = processor.pro
+000031a0: 6365 7373 2864 662c 2073 6361 6c65 5f63  cess(df, scale_c
+000031b0: 6f6c 733d 636f 6e74 5f63 6f6c 5f62 7566  ols=cont_col_buf
+000031c0: 662c 2065 6e63 6f64 655f 636f 6c73 3d28  f, encode_cols=(
+000031d0: 6361 745f 636f 6c5f 6275 6666 202b 205b  cat_col_buff + [
+000031e0: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
+000031f0: 7574 655d 2929 0d0a 0d0a 2020 2020 2020  ute]))....      
+00003200: 2020 2020 2020 7072 6f74 6563 7465 645f        protected_
+00003210: 6174 7472 6962 7574 655f 636f 6c75 6d6e  attribute_column
+00003220: 203d 2070 726f 6365 7373 6564 5f64 665b   = processed_df[
+00003230: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
+00003240: 7574 655d 0d0a 2020 2020 2020 2020 2020  ute]..          
+00003250: 2020 7072 6f63 6573 7365 645f 6466 2e64    processed_df.d
+00003260: 726f 7028 636f 6c75 6d6e 7320 3d20 5b70  rop(columns = [p
+00003270: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
+00003280: 7465 5d2c 2069 6e70 6c61 6365 203d 2054  te], inplace = T
+00003290: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
+000032a0: 2020 7072 6f63 6573 7365 645f 6466 2e6c    processed_df.l
+000032b0: 6f63 5b3a 2c74 6172 6765 745d 203d 2074  oc[:,target] = t
+000032c0: 6172 6765 745f 6466 0d0a 0d0a 2020 2020  arget_df....    
+000032d0: 2020 2020 2020 2020 6361 745f 636f 6c75          cat_colu
+000032e0: 6d6e 5f62 7566 6620 3d20 6361 745f 636f  mn_buff = cat_co
+000032f0: 6c5f 6275 6666 2e63 6f70 7928 290d 0a20  l_buff.copy().. 
+00003300: 2020 2020 2020 2020 2020 2063 6174 5f63             cat_c
+00003310: 6f6c 756d 6e5f 6275 6666 2e61 7070 656e  olumn_buff.appen
+00003320: 6428 7461 7267 6574 290d 0a20 2020 2020  d(target)..     
+00003330: 2020 2020 2020 2063 6174 5f63 6f6c 756d         cat_colum
+00003340: 6e5f 6964 7320 3d20 5b70 726f 6365 7373  n_ids = [process
+00003350: 6564 5f64 662e 636f 6c75 6d6e 732e 6765  ed_df.columns.ge
+00003360: 745f 6c6f 6328 636f 6c5f 6e61 6d65 2920  t_loc(col_name) 
+00003370: 666f 7220 636f 6c5f 6e61 6d65 2069 6e20  for col_name in 
+00003380: 6361 745f 636f 6c75 6d6e 5f62 7566 665d  cat_column_buff]
+00003390: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000033a0: 7361 6d70 6c65 7220 3d20 7365 6c66 2e6d  sampler = self.m
+000033b0: 6974 6967 6174 6f72 5f66 756e 6374 696f  itigator_functio
+000033c0: 6e5b 7365 6c66 2e6d 6574 686f 645d 2863  n[self.method](c
+000033d0: 6174 6567 6f72 6963 616c 5f66 6561 7475  ategorical_featu
+000033e0: 7265 733d 6361 745f 636f 6c75 6d6e 5f69  res=cat_column_i
+000033f0: 6473 290d 0a0d 0a20 2020 2020 2020 2020  ds)....         
+00003400: 2020 2058 5f72 6573 616d 706c 6564 2c20     X_resampled, 
+00003410: 6174 7472 6962 7574 655f 7265 7361 6d70  attribute_resamp
+00003420: 6c65 6420 3d20 7361 6d70 6c65 722e 6669  led = sampler.fi
+00003430: 745f 7265 7361 6d70 6c65 2870 726f 6365  t_resample(proce
+00003440: 7373 6564 5f64 662c 2070 726f 7465 6374  ssed_df, protect
+00003450: 6564 5f61 7474 7269 6275 7465 5f63 6f6c  ed_attribute_col
+00003460: 756d 6e29 0d0a 2020 2020 2020 2020 2020  umn)..          
+00003470: 2020 585f 7265 7361 6d70 6c65 642e 6c6f    X_resampled.lo
+00003480: 635b 3a2c 2070 726f 7465 6374 6564 5f61  c[:, protected_a
+00003490: 7474 7269 6275 7465 5d20 3d20 6174 7472  ttribute] = attr
+000034a0: 6962 7574 655f 7265 7361 6d70 6c65 640d  ibute_resampled.
+000034b0: 0a20 2020 2020 2020 2020 2020 0d0a 2020  .           ..  
+000034c0: 2020 2020 2020 2020 2020 6466 5f66 696e            df_fin
+000034d0: 616c 203d 2070 726f 6365 7373 6f72 2e75  al = processor.u
+000034e0: 6e70 726f 6365 7373 2858 5f72 6573 616d  nprocess(X_resam
+000034f0: 706c 6564 290d 0a20 2020 2020 2020 2020  pled)..         
+00003500: 2020 2074 6172 6765 745f 6669 6e61 6c20     target_final 
+00003510: 3d20 6466 5f66 696e 616c 5b74 6172 6765  = df_final[targe
+00003520: 745d 0d0a 2020 2020 2020 2020 2020 2020  t]..            
+00003530: 6466 5f66 696e 616c 2e64 726f 7028 636f  df_final.drop(co
+00003540: 6c75 6d6e 733d 5b74 6172 6765 745d 2c20  lumns=[target], 
+00003550: 696e 706c 6163 653d 5472 7565 290d 0a0d  inplace=True)...
+00003560: 0a20 2020 2020 2020 2065 6c73 6520 3a20  .        else : 
+00003570: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00003580: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
+00003590: 655f 636f 6c75 6d6e 203d 2064 665b 7072  e_column = df[pr
+000035a0: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
+000035b0: 655d 0d0a 2020 2020 2020 2020 2020 2020  e]..            
+000035c0: 6466 2e64 726f 7028 636f 6c75 6d6e 7320  df.drop(columns 
+000035d0: 3d20 5b70 726f 7465 6374 6564 5f61 7474  = [protected_att
+000035e0: 7269 6275 7465 5d2c 2069 6e70 6c61 6365  ribute], inplace
+000035f0: 203d 2054 7275 6529 0d0a 2020 2020 2020   = True)..      
+00003600: 2020 2020 2020 6466 2e6c 6f63 5b3a 2c74        df.loc[:,t
+00003610: 6172 6765 745d 203d 2074 6172 6765 745f  arget] = target_
+00003620: 6466 0d0a 0d0a 2020 2020 2020 2020 2020  df....          
+00003630: 2020 7361 6d70 6c65 7220 3d20 7365 6c66    sampler = self
+00003640: 2e6d 6974 6967 6174 6f72 5f66 756e 6374  .mitigator_funct
+00003650: 696f 6e5b 7365 6c66 2e6d 6574 686f 645d  ion[self.method]
+00003660: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00003670: 585f 7265 7361 6d70 6c65 642c 2061 7474  X_resampled, att
+00003680: 7269 6275 7465 5f72 6573 616d 706c 6564  ribute_resampled
+00003690: 203d 2073 616d 706c 6572 2e66 6974 5f72   = sampler.fit_r
+000036a0: 6573 616d 706c 6528 6466 2c20 7072 6f74  esample(df, prot
+000036b0: 6563 7465 645f 6174 7472 6962 7574 655f  ected_attribute_
+000036c0: 636f 6c75 6d6e 290d 0a20 2020 2020 2020  column)..       
+000036d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000036e0: 2020 2058 5f72 6573 616d 706c 6564 2e6c     X_resampled.l
+000036f0: 6f63 5b3a 2c20 7072 6f74 6563 7465 645f  oc[:, protected_
+00003700: 6174 7472 6962 7574 655d 203d 2061 7474  attribute] = att
+00003710: 7269 6275 7465 5f72 6573 616d 706c 6564  ribute_resampled
+00003720: 0d0a 2020 2020 2020 2020 2020 2020 7461  ..            ta
+00003730: 7267 6574 5f66 696e 616c 203d 2058 5f72  rget_final = X_r
+00003740: 6573 616d 706c 6564 5b74 6172 6765 745d  esampled[target]
+00003750: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
+00003760: 5f66 696e 616c 203d 2058 5f72 6573 616d  _final = X_resam
+00003770: 706c 6564 2e64 726f 7028 636f 6c75 6d6e  pled.drop(column
+00003780: 733d 5b74 6172 6765 745d 290d 0a20 2020  s=[target])..   
+00003790: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
+000037a0: 6620 6c65 6e28 7072 6f74 6563 7465 645f  f len(protected_
+000037b0: 6174 7472 6962 7574 6573 2920 3e20 3120  attributes) > 1 
+000037c0: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
+000037d0: 665f 6669 6e61 6c20 3d20 6466 5f66 696e  f_final = df_fin
+000037e0: 616c 2e64 726f 7028 636f 6c75 6d6e 7320  al.drop(columns 
+000037f0: 3d20 7072 6f74 6563 7465 645f 6174 7472  = protected_attr
+00003800: 6962 7574 6529 2020 2020 0d0a 2020 2020  ibute)    ..    
+00003810: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00003820: 2064 665f 6669 6e61 6c2c 2074 6172 6765   df_final, targe
+00003830: 745f 6669 6e61 6c0d 0a20 2020 200d 0a20  t_final..    .. 
+00003840: 2020 2064 6566 2062 616c 616e 6365 5f6f     def balance_o
+00003850: 7574 7075 745f 666f 725f 6174 7472 6962  utput_for_attrib
+00003860: 7574 6528 7365 6c66 2c20 6461 7461 7365  ute(self, datase
+00003870: 743a 2070 642e 4461 7461 4672 616d 652c  t: pd.DataFrame,
+00003880: 2074 6172 6765 743a 2073 7472 2c20 7072   target: str, pr
+00003890: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
+000038a0: 6573 3a20 6c69 7374 2c20 0d0a 2020 2020  es: list, ..    
+000038b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038d0: 2063 6f6e 745f 636f 6c75 6d6e 733a 206c   cont_columns: l
+000038e0: 6973 7420 3d20 4e6f 6e65 2c20 6361 745f  ist = None, cat_
+000038f0: 636f 6c75 6d6e 733a 206c 6973 7420 3d20  columns: list = 
+00003900: 4e6f 6e65 2920 3a0d 0a20 2020 2020 2020  None) :..       
+00003910: 2022 2222 0d0a 2020 2020 2020 2020 4261   """..        Ba
+00003920: 6c61 6e63 6520 7468 6520 6f75 7470 7574  lance the output
+00003930: 206f 6620 7468 6520 636c 6173 7365 7320   of the classes 
+00003940: 666f 7220 6120 6769 7665 6e20 7072 6f74  for a given prot
+00003950: 6563 7465 6420 6174 7472 6962 7574 652e  ected attribute.
+00003960: 205c 6e0d 0a20 2020 2020 2020 2053 686f   \n..        Sho
+00003970: 756c 6420 696d 7072 6f76 6520 7468 6520  uld improve the 
+00003980: 4449 5220 666f 7220 7468 6520 7072 6f74  DIR for the prot
+00003990: 6563 7465 6420 6174 7472 6962 7574 652e  ected attribute.
+000039a0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+000039b0: 2020 2020 4172 6773 3a20 0d0a 2020 2020      Args: ..    
+000039c0: 2020 2020 2020 2020 6461 7461 7365 7420          dataset 
+000039d0: 2870 642e 4461 7461 4672 616d 6529 3a20  (pd.DataFrame): 
+000039e0: 6461 7461 7365 7420 746f 206d 6974 6967  dataset to mitig
+000039f0: 6174 652c 2074 6861 7420 696e 636c 7564  ate, that includ
+00003a00: 6573 2074 6865 2074 6172 6765 7420 636f  es the target co
+00003a10: 6c75 6d6e 2e0d 0a20 2020 2020 2020 2020  lumn...         
+00003a20: 2020 2074 6172 6765 7420 2873 7472 293a     target (str):
+00003a30: 2074 6865 2074 6172 6765 7420 636f 6c75   the target colu
+00003a40: 6d6e 206e 616d 650d 0a20 2020 2020 2020  mn name..       
+00003a50: 2020 2020 2070 726f 7465 6374 6564 5f61       protected_a
+00003a60: 7474 7269 6275 7465 7320 286c 6973 742c  ttributes (list,
+00003a70: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+00003a80: 6174 7472 6962 7574 6528 7329 2074 6f20  attribute(s) to 
+00003a90: 6261 6c61 6e63 652e 2044 6566 6175 6c74  balance. Default
+00003aa0: 7320 746f 204e 6f6e 652e 0d0a 2020 2020  s to None...    
+00003ab0: 2020 2020 2020 2020 636f 6e74 5f63 6f6c          cont_col
+00003ac0: 756d 6e73 2028 6c69 7374 2c20 6f70 7469  umns (list, opti
+00003ad0: 6f6e 616c 293a 2054 6865 2063 6f6e 7469  onal): The conti
+00003ae0: 6e75 6f75 7320 636f 6c75 6d6e 7320 696e  nuous columns in
+00003af0: 2074 6865 2064 6174 6173 6574 2e20 4f6e   the dataset. On
+00003b00: 6c79 204e 6563 6573 7361 7279 2069 6620  ly Necessary if 
+00003b10: 7468 6520 7361 6d70 6c69 6e67 2073 7472  the sampling str
+00003b20: 6174 6567 7920 6973 2053 4d4f 5445 4e43  ategy is SMOTENC
+00003b30: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
+00003b40: 6e65 2e0d 0a20 2020 2020 2020 2020 2020  ne...           
+00003b50: 2063 6174 5f63 6f6c 756d 6e73 2028 6c69   cat_columns (li
+00003b60: 7374 2c20 6f70 7469 6f6e 616c 293a 2054  st, optional): T
+00003b70: 6865 2063 6174 6567 6f72 6963 616c 2063  he categorical c
+00003b80: 6f6c 756d 6e73 2069 6e20 7468 6520 6461  olumns in the da
+00003b90: 7461 7365 742e 204f 6e6c 7920 4e65 6365  taset. Only Nece
+00003ba0: 7373 6172 7920 6966 2074 6865 2073 616d  ssary if the sam
+00003bb0: 706c 696e 6720 7374 7261 7465 6779 2069  pling strategy i
+00003bc0: 7320 534d 4f54 454e 432e 2044 6566 6175  s SMOTENC. Defau
+00003bd0: 6c74 7320 746f 204e 6f6e 652e 0d0a 0d0a  lts to None.....
+00003be0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00003bf0: 0d0a 2020 2020 2020 2020 2020 2020 285b  ..            ([
+00003c00: 7064 2e44 6174 6146 7261 6d65 2c20 7064  pd.DataFrame, pd
+00003c10: 2e44 6174 6146 7261 6d65 5d29 3a20 7468  .DataFrame]): th
+00003c20: 6520 6261 6c61 6e63 6564 2064 6174 6166  e balanced dataf
+00003c30: 7261 6d65 7320 666f 7220 7468 6520 6461  rames for the da
+00003c40: 7461 7365 7420 616e 6420 7468 6520 7461  taset and the ta
+00003c50: 7267 6574 0d0a 2020 2020 2020 2020 2222  rget..        ""
+00003c60: 220d 0a0d 0a20 2020 2020 2020 2073 7570  "....        sup
+00003c70: 6572 2829 2e5f 7361 6e69 7479 5f63 6865  er()._sanity_che
+00003c80: 636b 2864 6174 6173 6574 2c20 7461 7267  ck(dataset, targ
+00003c90: 6574 2c20 7072 6f74 6563 7465 645f 6174  et, protected_at
+00003ca0: 7472 6962 7574 6573 3d70 726f 7465 6374  tributes=protect
+00003cb0: 6564 5f61 7474 7269 6275 7465 7329 0d0a  ed_attributes)..
+00003cc0: 2020 2020 2020 2020 6466 203d 2064 6174          df = dat
+00003cd0: 6173 6574 2e63 6f70 7928 290d 0a0d 0a20  aset.copy().... 
+00003ce0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00003cf0: 2069 6620 6c65 6e28 7072 6f74 6563 7465   if len(protecte
+00003d00: 645f 6174 7472 6962 7574 6573 2920 3e20  d_attributes) > 
+00003d10: 3120 3a0d 0a20 2020 2020 2020 2020 2020  1 :..           
+00003d20: 2064 662c 2070 726f 7465 6374 6564 5f61   df, protected_a
+00003d30: 7474 7269 6275 7465 203d 2073 656c 662e  ttribute = self.
+00003d40: 5f6d 616b 655f 7375 7065 725f 7072 6f74  _make_super_prot
+00003d50: 6563 7465 6428 6461 7461 7365 742c 2070  ected(dataset, p
+00003d60: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
+00003d70: 7465 7329 0d0a 2020 2020 2020 2020 656c  tes)..        el
+00003d80: 7365 203a 0d0a 2020 2020 2020 2020 2020  se :..          
+00003d90: 2020 7072 6f74 6563 7465 645f 6174 7472    protected_attr
+00003da0: 6962 7574 6520 3d20 7072 6f74 6563 7465  ibute = protecte
+00003db0: 645f 6174 7472 6962 7574 6573 5b30 5d0d  d_attributes[0].
+00003dc0: 0a20 2020 200d 0a20 2020 2020 2020 2063  .    ..        c
+00003dd0: 6c61 7373 6573 203d 206c 6973 7428 6466  lasses = list(df
+00003de0: 5b70 726f 7465 6374 6564 5f61 7474 7269  [protected_attri
+00003df0: 6275 7465 5d2e 756e 6971 7565 2829 290d  bute].unique()).
+00003e00: 0a20 2020 2020 2020 2072 2c20 6d61 785f  .        r, max_
+00003e10: 636c 6173 7320 3d20 7365 6c66 2e5f 6869  class = self._hi
+00003e20: 6768 6573 745f 7261 7469 6f28 6466 2c20  ghest_ratio(df, 
+00003e30: 7461 7267 6574 2c20 636c 6173 7365 732c  target, classes,
+00003e40: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
+00003e50: 6275 7465 290d 0a20 2020 2020 2020 200d  bute)..        .
+00003e60: 0a20 2020 2020 2020 2066 6f72 2063 2069  .        for c i
+00003e70: 6e20 636c 6173 7365 7320 3a0d 0a20 2020  n classes :..   
+00003e80: 2020 2020 2020 2020 2069 6620 6320 213d           if c !=
+00003e90: 206d 6178 5f63 6c61 7373 203a 0d0a 2020   max_class :..  
+00003ea0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00003eb0: 6b65 6570 206f 6e6c 7920 7468 6520 726f  keep only the ro
+00003ec0: 7773 2077 6974 6820 6769 7665 6e20 636c  ws with given cl
+00003ed0: 6173 730d 0a20 2020 2020 2020 2020 2020  ass..           
+00003ee0: 2020 2020 2063 6c61 7373 5f64 6620 3d20       class_df = 
+00003ef0: 6466 5b64 665b 7072 6f74 6563 7465 645f  df[df[protected_
+00003f00: 6174 7472 6962 7574 655d 203d 3d20 635d  attribute] == c]
+00003f10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003f20: 2020 636c 6173 735f 7461 7267 6574 203d    class_target =
+00003f30: 2063 6c61 7373 5f64 665b 7461 7267 6574   class_df[target
+00003f40: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00003f50: 2020 2063 6c61 7373 5f64 6620 3d20 636c     class_df = cl
+00003f60: 6173 735f 6466 2e64 726f 7028 636f 6c75  ass_df.drop(colu
+00003f70: 6d6e 733d 5b74 6172 6765 745d 290d 0a20  mns=[target]).. 
+00003f80: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00003f90: 2020 2020 2020 2020 2020 2020 2023 2072               # r
+00003fa0: 6573 616d 706c 6520 7468 6520 7461 7267  esample the targ
+00003fb0: 6574 2066 6f72 2074 6869 7320 636c 6173  et for this clas
+00003fc0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00003fd0: 2020 2069 6620 6c65 6e28 6c69 7374 2863     if len(list(c
+00003fe0: 6c61 7373 5f74 6172 6765 742e 756e 6971  lass_target.uniq
+00003ff0: 7565 2829 2929 2021 3d20 3120 3a0d 0a20  ue())) != 1 :.. 
+00004000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004010: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00004020: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00004030: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00004040: 6620 7365 6c66 2e6d 6574 686f 6420 696e  f self.method in
+00004050: 205b 2253 4d4f 5445 4e43 225d 203a 0d0a   ["SMOTENC"] :..
+00004060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004070: 2020 2020 2020 2020 636f 6e74 5f63 6f6c          cont_col
+00004080: 5f62 7566 6620 3d20 5b66 6561 7475 7265  _buff = [feature
+00004090: 2066 6f72 2066 6561 7475 7265 2069 6e20   for feature in 
+000040a0: 636f 6e74 5f63 6f6c 756d 6e73 2069 6620  cont_columns if 
+000040b0: 6665 6174 7572 6520 213d 2070 726f 7465  feature != prote
+000040c0: 6374 6564 5f61 7474 7269 6275 7465 5d0d  cted_attribute].
+000040d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000040e0: 2020 2020 2020 2020 2063 6174 5f63 6f6c           cat_col
+000040f0: 5f62 7566 6620 3d20 5b66 6561 7475 7265  _buff = [feature
+00004100: 2066 6f72 2066 6561 7475 7265 2069 6e20   for feature in 
+00004110: 6361 745f 636f 6c75 6d6e 7320 6966 2066  cat_columns if f
+00004120: 6561 7475 7265 2021 3d20 7072 6f74 6563  eature != protec
+00004130: 7465 645f 6174 7472 6962 7574 655d 0d0a  ted_attribute]..
+00004140: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00004150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004160: 2020 2020 2020 2370 7265 7072 6f63 6573        #preproces
+00004170: 7320 7573 696e 6720 7468 6520 7072 6f74  s using the prot
+00004180: 6563 7465 6420 6174 7472 6962 7574 6520  ected attribute 
+00004190: 6173 2061 2074 6172 6765 740d 0a20 2020  as a target..   
+000041a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041b0: 2020 2020 2070 726f 6365 7373 6f72 203d       processor =
+000041c0: 205f 5072 6f63 6573 736f 7228 290d 0a20   _Processor().. 
+000041d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041e0: 2020 2020 2020 2070 726f 6365 7373 6564         processed
+000041f0: 5f64 6620 3d20 7072 6f63 6573 736f 722e  _df = processor.
+00004200: 7072 6f63 6573 7328 636c 6173 735f 6466  process(class_df
+00004210: 2c20 7363 616c 655f 636f 6c73 3d63 6f6e  , scale_cols=con
+00004220: 745f 636f 6c5f 6275 6666 2c20 656e 636f  t_col_buff, enco
+00004230: 6465 5f63 6f6c 733d 2863 6174 5f63 6f6c  de_cols=(cat_col
+00004240: 5f62 7566 6620 2b20 5b70 726f 7465 6374  _buff + [protect
+00004250: 6564 5f61 7474 7269 6275 7465 5d29 290d  ed_attribute])).
+00004260: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00004270: 2020 2020 2020 2020 2020 2063 6174 5f63             cat_c
+00004280: 6f6c 756d 6e73 5f69 6473 203d 205b 7072  olumns_ids = [pr
+00004290: 6f63 6573 7365 645f 6466 2e63 6f6c 756d  ocessed_df.colum
+000042a0: 6e73 2e67 6574 5f6c 6f63 2863 6f6c 5f6e  ns.get_loc(col_n
+000042b0: 616d 6529 2066 6f72 2063 6f6c 5f6e 616d  ame) for col_nam
+000042c0: 6520 696e 2063 6174 5f63 6f6c 756d 6e73  e in cat_columns
+000042d0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000042e0: 2020 2020 2020 2020 2020 2073 616d 706c             sampl
+000042f0: 6572 203d 2053 4d4f 5445 4e43 2873 616d  er = SMOTENC(sam
+00004300: 706c 696e 675f 7374 7261 7465 6779 3d72  pling_strategy=r
+00004310: 2c20 6361 7465 676f 7269 6361 6c5f 6665  , categorical_fe
+00004320: 6174 7572 6573 3d63 6174 5f63 6f6c 756d  atures=cat_colum
+00004330: 6e73 5f69 6473 290d 0a20 2020 2020 2020  ns_ids)..       
+00004340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004350: 2058 5f72 6573 616d 706c 6564 2c20 636c   X_resampled, cl
+00004360: 6173 735f 7461 7267 6574 5f72 6573 616d  ass_target_resam
+00004370: 706c 6564 203d 2073 616d 706c 6572 2e66  pled = sampler.f
+00004380: 6974 5f72 6573 616d 706c 6528 7072 6f63  it_resample(proc
+00004390: 6573 7365 645f 6466 2c20 636c 6173 735f  essed_df, class_
+000043a0: 7461 7267 6574 290d 0a20 2020 2020 2020  target)..       
+000043b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043c0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000043d0: 2020 2020 2020 2020 2020 2063 6c61 7373             class
+000043e0: 5f72 6573 616d 706c 6564 203d 2070 726f  _resampled = pro
+000043f0: 6365 7373 6f72 2e75 6e70 726f 6365 7373  cessor.unprocess
+00004400: 2858 5f72 6573 616d 706c 6564 290d 0a20  (X_resampled).. 
+00004410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004420: 2020 2020 2020 2063 6c61 7373 5f72 6573         class_res
+00004430: 616d 706c 6564 2e6c 6f63 5b3a 2c20 7461  ampled.loc[:, ta
+00004440: 7267 6574 5d20 3d20 636c 6173 735f 7461  rget] = class_ta
+00004450: 7267 6574 5f72 6573 616d 706c 6564 0d0a  rget_resampled..
+00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004490: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
+000044a0: 6d65 7468 6f64 2069 6e20 5b22 5261 6e64  method in ["Rand
+000044b0: 6f6d 4f76 6572 5361 6d70 6c65 7222 5d20  omOverSampler"] 
+000044c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000044d0: 2020 2020 2020 2020 2020 2073 616d 706c             sampl
+000044e0: 6572 203d 2052 616e 646f 6d4f 7665 7253  er = RandomOverS
+000044f0: 616d 706c 6572 2873 616d 706c 696e 675f  ampler(sampling_
+00004500: 7374 7261 7465 6779 3d72 290d 0a20 2020  strategy=r)..   
+00004510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004520: 2020 2020 2063 6c61 7373 5f72 6573 616d       class_resam
+00004530: 706c 6564 2c20 636c 6173 735f 7461 7267  pled, class_targ
+00004540: 6574 5f72 6573 616d 706c 6564 203d 2073  et_resampled = s
+00004550: 616d 706c 6572 2e66 6974 5f72 6573 616d  ampler.fit_resam
+00004560: 706c 6528 636c 6173 735f 6466 2c20 636c  ple(class_df, cl
+00004570: 6173 735f 7461 7267 6574 290d 0a20 2020  ass_target)..   
+00004580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004590: 2020 2020 2063 6c61 7373 5f72 6573 616d       class_resam
+000045a0: 706c 6564 2e6c 6f63 5b3a 2c20 7461 7267  pled.loc[:, targ
+000045b0: 6574 5d20 3d20 636c 6173 735f 7461 7267  et] = class_targ
+000045c0: 6574 5f72 6573 616d 706c 6564 0d0a 2020  et_resampled..  
+000045d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045e0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000045f0: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
+00004600: 662e 6d65 7468 6f64 2069 6e20 5b22 5261  f.method in ["Ra
+00004610: 6e64 6f6d 556e 6465 7253 616d 706c 6572  ndomUnderSampler
+00004620: 225d 203a 0d0a 2020 2020 2020 2020 2020  "] :..          
+00004630: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00004640: 6d70 6c65 7220 3d20 5261 6e64 6f6d 556e  mpler = RandomUn
+00004650: 6465 7253 616d 706c 6572 2873 616d 706c  derSampler(sampl
+00004660: 696e 675f 7374 7261 7465 6779 3d72 290d  ing_strategy=r).
+00004670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004680: 2020 2020 2020 2020 2063 6c61 7373 5f72           class_r
+00004690: 6573 616d 706c 6564 2c20 636c 6173 735f  esampled, class_
+000046a0: 7461 7267 6574 5f72 6573 616d 706c 6564  target_resampled
+000046b0: 203d 2073 616d 706c 6572 2e66 6974 5f72   = sampler.fit_r
+000046c0: 6573 616d 706c 6528 636c 6173 735f 6466  esample(class_df
+000046d0: 2c20 636c 6173 735f 7461 7267 6574 290d  , class_target).
+000046e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000046f0: 2020 2020 2020 2020 2063 6c61 7373 5f72           class_r
+00004700: 6573 616d 706c 6564 2e6c 6f63 5b3a 2c20  esampled.loc[:, 
+00004710: 7461 7267 6574 5d20 3d20 636c 6173 735f  target] = class_
+00004720: 7461 7267 6574 5f72 6573 616d 706c 6564  target_resampled
+00004730: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00004740: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00004750: 2020 2020 2020 2020 2020 656c 7365 203a            else :
+00004760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004770: 2020 2020 2020 2369 6620 7468 6572 6520        #if there 
+00004780: 6973 206f 6e6c 7920 6f6e 6520 6f75 7470  is only one outp
+00004790: 7574 2066 6f72 2074 6865 2063 6c61 7373  ut for the class
+000047a0: 2c20 7468 6572 6520 6973 206e 6f20 7761  , there is no wa
+000047b0: 7920 746f 2072 6573 616d 706c 6520 6974  y to resample it
+000047c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000047d0: 2020 2020 2020 636c 6173 735f 7265 7361        class_resa
+000047e0: 6d70 6c65 6420 3d20 636c 6173 735f 6466  mpled = class_df
+000047f0: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
+00004800: 2020 2020 2020 2020 2020 2020 2063 6c61               cla
+00004810: 7373 5f72 6573 616d 706c 6564 2e6c 6f63  ss_resampled.loc
+00004820: 5b3a 2c74 6172 6765 745d 203d 2063 6c61  [:,target] = cla
+00004830: 7373 5f74 6172 6765 740d 0a20 2020 2020  ss_target..     
+00004840: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00004850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004860: 2023 2061 7070 656e 6420 7468 6520 7265   # append the re
+00004870: 7361 6d70 6c65 6420 636c 6173 7320 696e  sampled class in
+00004880: 2066 696e 616c 2064 660d 0a20 2020 2020   final df..     
+00004890: 2020 2020 2020 2020 2020 2023 2028 6472             # (dr
+000048a0: 6f70 2074 6865 2072 6f77 7320 7769 7468  op the rows with
+000048b0: 2074 6869 7320 636c 6173 7320 6669 7273   this class firs
+000048c0: 7420 746f 206e 6f74 2064 7570 6c69 6361  t to not duplica
+000048d0: 7465 6420 7468 656d 290d 0a20 2020 2020  ted them)..     
+000048e0: 2020 2020 2020 2020 2020 2064 6620 3d20             df = 
+000048f0: 6466 5b64 665b 7072 6f74 6563 7465 645f  df[df[protected_
+00004900: 6174 7472 6962 7574 655d 2021 3d20 635d  attribute] != c]
+00004910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004920: 2020 6466 203d 2070 642e 636f 6e63 6174    df = pd.concat
+00004930: 285b 6466 2c20 636c 6173 735f 7265 7361  ([df, class_resa
+00004940: 6d70 6c65 645d 2c20 6967 6e6f 7265 5f69  mpled], ignore_i
+00004950: 6e64 6578 3d54 7275 6529 0d0a 0d0a 0d0a  ndex=True)......
+00004960: 2020 2020 2020 2020 7461 7267 6574 5f64          target_d
+00004970: 6620 3d20 6466 5b74 6172 6765 745d 0d0a  f = df[target]..
+00004980: 2020 2020 2020 2020 6466 2e64 726f 7028          df.drop(
+00004990: 636f 6c75 6d6e 733d 5b74 6172 6765 745d  columns=[target]
+000049a0: 2c20 696e 706c 6163 653d 5472 7565 290d  , inplace=True).
+000049b0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+000049c0: 2020 2069 6620 6c65 6e28 7072 6f74 6563     if len(protec
+000049d0: 7465 645f 6174 7472 6962 7574 6573 2920  ted_attributes) 
+000049e0: 3e20 3120 3a0d 0a20 2020 2020 2020 2020  > 1 :..         
+000049f0: 2020 2064 6620 3d20 6466 2e64 726f 7028     df = df.drop(
+00004a00: 636f 6c75 6d6e 7320 3d20 7072 6f74 6563  columns = protec
+00004a10: 7465 645f 6174 7472 6962 7574 6529 0d0a  ted_attribute)..
+00004a20: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00004a30: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+00004a40: 662c 2074 6172 6765 745f 6466 0d0a 2020  f, target_df..  
+00004a50: 2020 0d0a 2020 2020 6465 6620 6261 6c61    ..    def bala
+00004a60: 6e63 655f 616c 6c28 7365 6c66 2c20 6461  nce_all(self, da
+00004a70: 7461 7365 743a 2070 642e 4461 7461 4672  taset: pd.DataFr
+00004a80: 616d 652c 2074 6172 6765 743a 2073 7472  ame, target: str
+00004a90: 2c20 7072 6f74 6563 7465 645f 6174 7472  , protected_attr
+00004aa0: 6962 7574 6573 3a20 6c69 7374 2c20 0d0a  ibutes: list, ..
+00004ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ac0: 2020 2020 636f 6e74 5f63 6f6c 756d 6e73      cont_columns
+00004ad0: 3a20 6c69 7374 203d 204e 6f6e 652c 2063  : list = None, c
+00004ae0: 6174 5f63 6f6c 756d 6e73 3a20 6c69 7374  at_columns: list
+00004af0: 203d 204e 6f6e 6529 203a 0d0a 2020 2020   = None) :..    
+00004b00: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00004b10: 2046 6972 7374 2062 616c 616e 6365 7320   First balances 
+00004b20: 7468 6520 7072 6f74 6563 7465 6420 6174  the protected at
+00004b30: 7472 6962 7574 6528 7329 2c20 616e 6420  tribute(s), and 
+00004b40: 7468 656e 2062 616c 616e 6365 2074 6865  then balance the
+00004b50: 6972 206f 7574 7075 742e 2047 6976 6573  ir output. Gives
+00004b60: 2061 6e20 616c 6d6f 7374 2070 6572 6665   an almost perfe
+00004b70: 6374 6c79 2062 616c 616e 6365 6420 6461  ctly balanced da
+00004b80: 7461 7365 7420 666f 7220 7468 6520 7072  taset for the pr
+00004b90: 6f74 6563 7465 6420 6174 7472 6962 7574  otected attribut
+00004ba0: 6528 7329 2e0d 0a0d 0a20 2020 2020 2020  e(s).....       
+00004bb0: 2041 7267 733a 200d 0a20 2020 2020 2020   Args: ..       
+00004bc0: 2020 2020 2064 6174 6173 6574 2028 7064       dataset (pd
+00004bd0: 2e44 6174 6146 7261 6d65 293a 2064 6174  .DataFrame): dat
+00004be0: 6173 6574 2074 6f20 6d69 7469 6761 7465  aset to mitigate
+00004bf0: 2c20 7468 6174 2069 6e63 6c75 6465 7320  , that includes 
+00004c00: 7468 6520 7461 7267 6574 2063 6f6c 756d  the target colum
+00004c10: 6e2e 0d0a 2020 2020 2020 2020 2020 2020  n...            
+00004c20: 7461 7267 6574 2028 7374 7229 3a20 7468  target (str): th
+00004c30: 6520 7461 7267 6574 2063 6f6c 756d 6e20  e target column 
+00004c40: 6e61 6d65 0d0a 2020 2020 2020 2020 2020  name..          
+00004c50: 2020 7072 6f74 6563 7465 645f 6174 7472    protected_attr
+00004c60: 6962 7574 6573 2028 6c69 7374 2c20 6f70  ibutes (list, op
+00004c70: 7469 6f6e 616c 293a 2054 6865 2061 7474  tional): The att
+00004c80: 7269 6275 7465 2873 2920 746f 2062 616c  ribute(s) to bal
+00004c90: 616e 6365 2e20 4465 6661 756c 7473 2074  ance. Defaults t
+00004ca0: 6f20 4e6f 6e65 2e0d 0a20 2020 2020 2020  o None...       
+00004cb0: 2020 2020 2063 6f6e 745f 636f 6c75 6d6e       cont_column
+00004cc0: 7320 286c 6973 742c 206f 7074 696f 6e61  s (list, optiona
+00004cd0: 6c29 3a20 5468 6520 636f 6e74 696e 756f  l): The continuo
+00004ce0: 7573 2063 6f6c 756d 6e73 2069 6e20 7468  us columns in th
+00004cf0: 6520 6461 7461 7365 742e 204f 6e6c 7920  e dataset. Only 
+00004d00: 4e65 6365 7373 6172 7920 6966 2074 6865  Necessary if the
+00004d10: 2073 616d 706c 696e 6720 7374 7261 7465   sampling strate
+00004d20: 6779 2069 7320 534d 4f54 454e 432e 2044  gy is SMOTENC. D
+00004d30: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
+00004d40: 0d0a 2020 2020 2020 2020 2020 2020 6361  ..            ca
+00004d50: 745f 636f 6c75 6d6e 7320 286c 6973 742c  t_columns (list,
+00004d60: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+00004d70: 6361 7465 676f 7269 6361 6c20 636f 6c75  categorical colu
+00004d80: 6d6e 7320 696e 2074 6865 2064 6174 6173  mns in the datas
+00004d90: 6574 2e20 4f6e 6c79 204e 6563 6573 7361  et. Only Necessa
+00004da0: 7279 2069 6620 7468 6520 7361 6d70 6c69  ry if the sampli
+00004db0: 6e67 2073 7472 6174 6567 7920 6973 2053  ng strategy is S
+00004dc0: 4d4f 5445 4e43 2e20 4465 6661 756c 7473  MOTENC. Defaults
+00004dd0: 2074 6f20 4e6f 6e65 2e0d 0a0d 0a20 2020   to None.....   
+00004de0: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
+00004df0: 2020 2020 2020 2020 2020 2028 5b70 642e             ([pd.
+00004e00: 4461 7461 4672 616d 652c 2070 642e 4461  DataFrame, pd.Da
+00004e10: 7461 4672 616d 655d 293a 2074 6865 2062  taFrame]): the b
+00004e20: 616c 616e 6365 6420 6461 7461 6672 616d  alanced datafram
+00004e30: 6573 2066 6f72 2074 6865 2064 6174 6173  es for the datas
+00004e40: 6574 2061 6e64 2074 6865 2074 6172 6765  et and the targe
+00004e50: 740d 0a20 2020 2020 2020 2022 2222 0d0a  t..        """..
+00004e60: 2020 2020 2020 2020 6466 2c20 7420 3d20          df, t = 
+00004e70: 7365 6c66 2e62 616c 616e 6365 5f70 726f  self.balance_pro
+00004e80: 7465 6374 6564 5f61 7474 7269 6275 7465  tected_attribute
+00004e90: 2864 6174 6173 6574 2c20 7461 7267 6574  (dataset, target
+00004ea0: 2c20 7072 6f74 6563 7465 645f 6174 7472  , protected_attr
+00004eb0: 6962 7574 6573 2c20 636f 6e74 5f63 6f6c  ibutes, cont_col
+00004ec0: 756d 6e73 2c20 6361 745f 636f 6c75 6d6e  umns, cat_column
+00004ed0: 7329 200d 0a20 2020 2020 2020 2064 662e  s) ..        df.
+00004ee0: 6c6f 635b 3a2c 2074 6172 6765 745d 203d  loc[:, target] =
+00004ef0: 2074 0d0a 2020 2020 2020 2020 6466 2c20   t..        df, 
+00004f00: 7420 3d20 7365 6c66 2e62 616c 616e 6365  t = self.balance
+00004f10: 5f6f 7574 7075 745f 666f 725f 6174 7472  _output_for_attr
+00004f20: 6962 7574 6528 6466 2c20 7461 7267 6574  ibute(df, target
+00004f30: 2c20 7072 6f74 6563 7465 645f 6174 7472  , protected_attr
+00004f40: 6962 7574 6573 2c20 636f 6e74 5f63 6f6c  ibutes, cont_col
+00004f50: 756d 6e73 2c20 6361 745f 636f 6c75 6d6e  umns, cat_column
+00004f60: 7329 0d0a 2020 2020 2020 2020 0d0a 2020  s)..        ..  
+00004f70: 2020 2020 2020 7265 7475 726e 2064 662c        return df,
+00004f80: 2074 2020 2020 0d0a 2020 2020 2020 2020   t    ..        
+00004f90: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00004fa0: 2020 0d0a 2020 2020 6465 6620 5f68 6967    ..    def _hig
+00004fb0: 6865 7374 5f72 6174 696f 2873 656c 662c  hest_ratio(self,
+00004fc0: 2064 6174 6173 6574 3a20 7064 2e44 6174   dataset: pd.Dat
+00004fd0: 6146 7261 6d65 2c20 7461 7267 6574 3a20  aFrame, target: 
+00004fe0: 7374 722c 2063 6c61 7373 6573 3a20 6469  str, classes: di
+00004ff0: 6374 2c20 7072 6f74 6563 7465 645f 6174  ct, protected_at
+00005000: 7472 6962 7574 653a 2073 7472 2920 3a0d  tribute: str) :.
+00005010: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00005020: 2020 2020 2020 4769 7665 2074 6865 2068        Give the h
+00005030: 6967 6865 7374 2072 6174 696f 206f 6620  ighest ratio of 
+00005040: 706f 7369 7469 7665 206f 7574 7075 7420  positive output 
+00005050: 6f6e 206e 6567 6174 6976 6520 6f75 7470  on negative outp
+00005060: 7574 206f 6620 616c 6c20 7468 6520 636c  ut of all the cl
+00005070: 6173 7365 7320 6f66 2074 6865 2070 726f  asses of the pro
+00005080: 7465 6374 6564 2061 7474 7269 6275 7465  tected attribute
+00005090: 2e20 4e65 6365 7373 6172 7920 666f 7220  . Necessary for 
+000050a0: 6261 6c61 6e63 655f 6f75 7470 7574 5f66  balance_output_f
+000050b0: 6f72 5f61 7474 7269 6275 7465 2e0d 0a0d  or_attribute....
+000050c0: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
+000050d0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+000050e0: 7365 7420 2870 642e 4461 7461 4672 616d  set (pd.DataFram
+000050f0: 6529 3a20 6461 7461 7365 7420 746f 206d  e): dataset to m
+00005100: 6974 6967 6174 652c 2074 6861 7420 696e  itigate, that in
+00005110: 636c 7564 6573 2074 6865 2074 6172 6765  cludes the targe
+00005120: 7420 636f 6c75 6d6e 2e0d 0a20 2020 2020  t column...     
+00005130: 2020 2020 2020 2074 6172 6765 7420 2873         target (s
+00005140: 7472 293a 2074 6865 2074 6172 6765 7420  tr): the target 
+00005150: 636f 6c75 6d6e 206e 616d 650d 0a20 2020  column name..   
+00005160: 2020 2020 2020 2020 2063 6c61 7373 6573           classes
+00005170: 2028 6469 6374 293a 2074 6865 2063 6c61   (dict): the cla
+00005180: 7373 6573 206f 6620 7468 6520 7072 6f74  sses of the prot
+00005190: 6563 7465 6420 6174 7472 6962 7574 650d  ected attribute.
+000051a0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+000051b0: 7465 6374 6564 5f61 7474 7269 6275 7465  tected_attribute
+000051c0: 2028 7374 7229 3a20 7468 6520 7072 6f74   (str): the prot
+000051d0: 6563 7465 6420 6174 7472 6962 7574 6520  ected attribute 
+000051e0: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
+000051f0: 2068 6967 6865 7374 2072 6174 696f 2066   highest ratio f
+00005200: 6f72 2e0d 0a0d 0a20 2020 2020 2020 2052  or.....        R
+00005210: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+00005220: 2020 2020 2028 5b66 6c6f 6174 2c20 7374       ([float, st
+00005230: 725d 293a 2074 6865 2068 6967 6865 7374  r]): the highest
+00005240: 2072 6174 696f 2061 6e64 2074 6865 2061   ratio and the a
+00005250: 7373 6f63 6961 7465 6420 636c 6173 730d  ssociated class.
+00005260: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00005270: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00005280: 725f 6d61 7820 3d20 300d 0a20 2020 2020  r_max = 0..     
+00005290: 2020 2063 5f6d 6178 203d 2063 6c61 7373     c_max = class
+000052a0: 6573 5b30 5d0d 0a20 2020 2020 2020 2066  es[0]..        f
+000052b0: 6f72 2063 2069 6e20 636c 6173 7365 7320  or c in classes 
+000052c0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+000052d0: 203d 2064 6174 6173 6574 5b64 6174 6173   = dataset[datas
+000052e0: 6574 5b70 726f 7465 6374 6564 5f61 7474  et[protected_att
+000052f0: 7269 6275 7465 5d20 3d3d 2063 5d5b 7461  ribute] == c][ta
+00005300: 7267 6574 5d2e 7661 6c75 655f 636f 756e  rget].value_coun
+00005310: 7473 2829 5b31 5d2f 6461 7461 7365 745b  ts()[1]/dataset[
+00005320: 6461 7461 7365 745b 7072 6f74 6563 7465  dataset[protecte
+00005330: 645f 6174 7472 6962 7574 655d 203d 3d20  d_attribute] == 
+00005340: 635d 5b74 6172 6765 745d 2e76 616c 7565  c][target].value
+00005350: 5f63 6f75 6e74 7328 295b 305d 0d0a 2020  _counts()[0]..  
+00005360: 2020 2020 2020 2020 2020 6966 2072 203e            if r >
+00005370: 2031 203a 0d0a 2020 2020 2020 2020 2020   1 :..          
+00005380: 2020 2020 2020 7220 3d20 312f 720d 0a20        r = 1/r.. 
+00005390: 2020 2020 2020 2020 2020 2069 6620 7220             if r 
+000053a0: 3e20 725f 6d61 7820 3a0d 0a20 2020 2020  > r_max :..     
+000053b0: 2020 2020 2020 2020 2020 2072 5f6d 6178             r_max
+000053c0: 203d 2072 0d0a 2020 2020 2020 2020 2020   = r..          
+000053d0: 2020 2020 2020 635f 6d61 7820 3d20 630d        c_max = c.
+000053e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000053f0: 725f 6d61 782c 2063 5f6d 6178 0d0a 2020  r_max, c_max..  
+00005400: 200d 0a20 2020 0d0a 2020 2020 6465 6620   ..   ..    def 
+00005410: 5f6d 616b 655f 7375 7065 725f 7072 6f74  _make_super_prot
+00005420: 6563 7465 6428 7365 6c66 2c20 6461 7461  ected(self, data
+00005430: 7365 743a 2070 642e 4461 7461 4672 616d  set: pd.DataFram
+00005440: 652c 2070 726f 7465 6374 6564 5f61 7474  e, protected_att
+00005450: 7269 6275 7465 733a 206c 6973 7429 203a  ributes: list) :
+00005460: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00005470: 2020 2020 2020 204d 616b 6520 6120 7375         Make a su
+00005480: 7065 7220 7072 6f74 6563 7465 6420 6174  per protected at
+00005490: 7472 6962 7574 6520 7468 6174 2069 7320  tribute that is 
+000054a0: 7468 6520 636f 6d62 696e 6174 696f 6e20  the combination 
+000054b0: 6f66 2061 6c6c 2067 6976 656e 2070 726f  of all given pro
+000054c0: 7465 6374 6564 2061 7474 7269 6275 7465  tected attribute
+000054d0: 7320 6361 6c6c 6564 2022 7072 6f74 6563  s called "protec
+000054e0: 7465 645f 7375 7065 7263 6c61 7373 220d  ted_superclass".
+000054f0: 0a0d 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00005500: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
+00005510: 7461 7365 7420 2870 642e 4461 7461 4672  taset (pd.DataFr
+00005520: 616d 6529 3a20 6461 7461 7365 7420 746f  ame): dataset to
+00005530: 206d 6974 6967 6174 652c 2074 6861 7420   mitigate, that 
+00005540: 696e 636c 7564 6573 2074 6865 2074 6172  includes the tar
+00005550: 6765 7420 636f 6c75 6d6e 2e0d 0a20 2020  get column...   
+00005560: 2020 2020 2020 2020 2070 726f 7465 6374           protect
+00005570: 6564 5f61 7474 7269 6275 7465 7320 286c  ed_attributes (l
+00005580: 6973 7429 3a20 7072 6f74 6563 7465 6420  ist): protected 
+00005590: 6174 7472 6962 7574 6573 2074 6f20 636f  attributes to co
+000055a0: 6d62 696e 650d 0a20 2020 2020 2020 2020  mbine..         
+000055b0: 2020 200d 0a20 2020 2020 2020 2052 6574     ..        Ret
+000055c0: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
+000055d0: 2020 2028 5b70 642e 4461 7461 4672 616d     ([pd.DataFram
+000055e0: 652c 2073 7472 5d29 3a20 7468 6520 7472  e, str]): the tr
+000055f0: 616e 7366 6f72 6d65 6420 6461 7461 7365  ansformed datase
+00005600: 7420 616e 6420 7468 6520 6e61 6d65 2022  t and the name "
+00005610: 7375 7065 7220 7072 6f74 6563 7465 6422  super protected"
+00005620: 2063 6f6c 756d 6e0d 0a20 2020 2020 2020   column..       
+00005630: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
+00005640: 6466 203d 2064 6174 6173 6574 2e63 6f70  df = dataset.cop
+00005650: 7928 290d 0a20 2020 2020 2020 2073 7570  y()..        sup
+00005660: 6572 7072 6f74 6563 7465 645f 636f 6c75  erprotected_colu
+00005670: 6d6e 203d 2066 756e 6374 6f6f 6c73 2e72  mn = functools.r
+00005680: 6564 7563 6528 6c61 6d62 6461 2061 2c20  educe(lambda a, 
+00005690: 6220 3a20 6120 2b20 225f 2220 2b20 622c  b : a + "_" + b,
+000056a0: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
+000056b0: 6275 7465 7329 0d0a 2020 2020 2020 2020  butes)..        
+000056c0: 6466 5b73 7570 6572 7072 6f74 6563 7465  df[superprotecte
+000056d0: 645f 636f 6c75 6d6e 5d20 3d20 2222 0d0a  d_column] = ""..
+000056e0: 2020 2020 2020 2020 666f 7220 7072 6f74          for prot
+000056f0: 6563 7465 645f 6174 7472 6962 7574 6520  ected_attribute 
+00005700: 696e 2070 726f 7465 6374 6564 5f61 7474  in protected_att
+00005710: 7269 6275 7465 7320 3a0d 0a0d 0a20 2020  ributes :....   
+00005720: 2020 2020 2020 2020 2064 665b 7375 7065           df[supe
+00005730: 7270 726f 7465 6374 6564 5f63 6f6c 756d  rprotected_colum
+00005740: 6e5d 202b 3d20 6466 5b70 726f 7465 6374  n] += df[protect
+00005750: 6564 5f61 7474 7269 6275 7465 5d2e 6170  ed_attribute].ap
+00005760: 706c 7928 7374 7229 2020 2b20 225f 220d  ply(str)  + "_".
+00005770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005780: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00005790: 2020 6466 5b73 7570 6572 7072 6f74 6563    df[superprotec
+000057a0: 7465 645f 636f 6c75 6d6e 5d20 3d20 6466  ted_column] = df
+000057b0: 5b73 7570 6572 7072 6f74 6563 7465 645f  [superprotected_
+000057c0: 636f 6c75 6d6e 5d2e 6170 706c 7928 6c61  column].apply(la
+000057d0: 6d62 6461 2078 203a 2078 5b3a 2d31 5d29  mbda x : x[:-1])
+000057e0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+000057f0: 2020 2020 0d0a 2020 2020 2020 2020 7265      ..        re
+00005800: 7475 726e 2064 662c 2073 7570 6572 7072  turn df, superpr
+00005810: 6f74 6563 7465 645f 636f 6c75 6d6e 0d0a  otected_column..
+00005820: 2020 2020 0d0a 6966 205f 5f6e 616d 655f      ..if __name_
+00005830: 5f20 3d3d 2022 5f5f 6d61 696e 5f5f 2220  _ == "__main__" 
+00005840: 3a20 0d0a 2020 2020 6461 7461 203d 207b  : ..    data = {
+00005850: 0d0a 2020 2020 2766 6561 7475 7265 3127  ..    'feature1'
+00005860: 3a20 5b31 2c20 302c 2031 2c20 302c 2031  : [1, 0, 1, 0, 1
+00005870: 2c20 302c 2031 2c20 302c 2031 2c20 302c  , 0, 1, 0, 1, 0,
+00005880: 2031 2c20 302c 2031 2c20 302c 2031 2c20   1, 0, 1, 0, 1, 
+00005890: 302c 2031 2c20 302c 2031 2c20 305d 2c0d  0, 1, 0, 1, 0],.
+000058a0: 0a20 2020 2027 6665 6174 7572 6532 273a  .    'feature2':
+000058b0: 205b 352c 2036 2c20 372c 2038 2c20 392c   [5, 6, 7, 8, 9,
+000058c0: 2031 302c 2031 312c 2031 322c 2031 332c   10, 11, 12, 13,
+000058d0: 2031 342c 2031 352c 2031 362c 2031 372c   14, 15, 16, 17,
+000058e0: 2031 382c 2031 392c 2032 302c 2032 312c   18, 19, 20, 21,
+000058f0: 2032 322c 2032 332c 2032 345d 2c0d 0a20   22, 23, 24],.. 
+00005900: 2020 2027 7072 6f74 6563 7465 645f 6174     'protected_at
+00005910: 7472 6962 7574 6527 3a20 5b27 4127 2c20  tribute': ['A', 
+00005920: 2741 272c 2027 4127 2c20 2741 272c 2027  'A', 'A', 'A', '
+00005930: 4127 2c20 2742 272c 2027 4127 2c20 2742  A', 'B', 'A', 'B
+00005940: 272c 2027 4127 2c20 2742 272c 2027 4127  ', 'A', 'B', 'A'
+00005950: 2c20 2742 272c 2027 4127 2c20 2742 272c  , 'B', 'A', 'B',
+00005960: 2027 4127 2c20 2742 272c 2027 4127 2c20   'A', 'B', 'A', 
+00005970: 2742 272c 2027 4127 2c20 2742 275d 2c0d  'B', 'A', 'B'],.
+00005980: 0a20 2020 207d 0d0a 0d0a 2020 2020 6461  .    }....    da
+00005990: 7461 7365 7420 3d20 7064 2e44 6174 6146  taset = pd.DataF
+000059a0: 7261 6d65 2864 6174 6129 0d0a 2020 2020  rame(data)..    
+000059b0: 7461 7267 6574 203d 2070 642e 5365 7269  target = pd.Seri
+000059c0: 6573 285b 312c 2030 2c20 312c 2030 2c20  es([1, 0, 1, 0, 
+000059d0: 312c 2030 2c20 312c 2030 2c20 312c 2030  1, 0, 1, 0, 1, 0
+000059e0: 2c20 312c 2031 2c20 302c 2030 2c20 312c  , 1, 1, 0, 0, 1,
+000059f0: 2030 2c20 312c 2030 2c20 302c 2030 5d29   0, 1, 0, 0, 0])
+00005a00: 0d0a 2020 2020 0d0a 2020 2020 6261 6c61  ..    ..    bala
+00005a10: 6e63 6520 3d20 4261 6c61 6e63 6541 7474  nce = BalanceAtt
+00005a20: 7269 6275 7465 7328 534d 4f54 454e 4350  ributes(SMOTENCP
+00005a30: 726f 6365 7373 6f72 2829 290d 0a20 2020  rocessor())..   
+00005a40: 200d 0a20 2020 2058 2c20 793d 2062 616c   ..    X, y= bal
+00005a50: 616e 6365 2e62 616c 616e 6365 2864 6174  ance.balance(dat
+00005a60: 6173 6574 2c20 7461 7267 6574 2c20 5b22  aset, target, ["
+00005a70: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
+00005a80: 7574 6522 5d2c 2063 6f6e 745f 636f 6c75  ute"], cont_colu
+00005a90: 6d6e 733d 5b22 6665 6174 7572 6532 225d  mns=["feature2"]
+00005aa0: 2c20 6361 745f 636f 6c75 6d6e 733d 5b22  , cat_columns=["
+00005ab0: 6665 6174 7572 6531 222c 2022 7072 6f74  feature1", "prot
+00005ac0: 6563 7465 645f 6174 7472 6962 7574 6522  ected_attribute"
+00005ad0: 5d20 29                                  ] )
```

### Comparing `fairbalance-0.0.4/fairbalance/tools/_utils.py` & `fairbalance-0.1.1/fairbalance/tools/_utils.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.0.4/fairbalance.egg-info/PKG-INFO` & `fairbalance-0.1.1/fairbalance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbalance
-Version: 0.0.4
+Version: 0.1.1
 Summary: bias mitigation by balancing target and/or protected attributes using resampling techniques
 Author: Pierre-Antoine Lequeu @ Fujitsu Luxembourg
 Author-email: pierre-antoine.lequeu@fujitsu.com
 Description-Content-Type: text/markdown
 Requires-Dist: folktables>=0.0.12
 Requires-Dist: imbalanced_learn==0.9.1
 Requires-Dist: numpy>=1.24.3
```

### Comparing `fairbalance-0.0.4/setup.py` & `fairbalance-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "fairbalance",
-    version = "0.0.4",
+    version = "0.1.1",
     author = "Pierre-Antoine Lequeu @ Fujitsu Luxembourg",
     author_email = "pierre-antoine.lequeu@fujitsu.com",
     description = "bias mitigation by balancing target and/or protected attributes using resampling techniques",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = setuptools.find_packages(),
     install_requires=[
```

