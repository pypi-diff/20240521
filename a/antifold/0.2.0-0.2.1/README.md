# Comparing `tmp/antifold-0.2.0.tar.gz` & `tmp/antifold-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antifold-0.2.0.tar", last modified: Tue May 21 14:24:43 2024, max compression
+gzip compressed data, was "antifold-0.2.1.tar", last modified: Tue May 21 16:14:59 2024, max compression
```

## Comparing `antifold-0.2.0.tar` & `antifold-0.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 14:24:43.433695 antifold-0.2.0/
--rw-r--r--   0 maghoi     (502) staff       (20)     1512 2024-05-13 11:41:55.000000 antifold-0.2.0/LICENSE
--rw-r--r--   0 maghoi     (502) staff       (20)       25 2024-05-21 13:44:49.000000 antifold-0.2.0/MANIFEST.in
--rw-r--r--   0 maghoi     (502) staff       (20)      480 2024-05-21 14:24:43.433342 antifold-0.2.0/PKG-INFO
--rw-r--r--   0 maghoi     (502) staff       (20)    12485 2024-05-21 13:02:22.000000 antifold-0.2.0/README.md
-drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 14:24:43.398627 antifold-0.2.0/antifold/
--rw-r--r--   0 maghoi     (502) staff       (20)        0 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/__init__.py
--rw-r--r--   0 maghoi     (502) staff       (20)    25829 2024-05-21 14:18:55.000000 antifold-0.2.0/antifold/antiscripts.py
-drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 14:24:43.408734 antifold-0.2.0/antifold/esm/
--rw-r--r--   0 maghoi     (502) staff       (20)      238 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/__init__.py
--rw-r--r--   0 maghoi     (502) staff       (20)      371 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/constants.py
--rw-r--r--   0 maghoi     (502) staff       (20)    17438 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/data.py
-drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 14:24:43.432783 antifold-0.2.0/antifold/esm/inverse_folding/
--rw-r--r--   0 maghoi     (502) staff       (20)      231 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/inverse_folding/__init__.py
--rw-r--r--   0 maghoi     (502) staff       (20)    14800 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/inverse_folding/features.py
--rw-r--r--   0 maghoi     (502) staff       (20)     1790 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/inverse_folding/gvp_encoder.py
--rw-r--r--   0 maghoi     (502) staff       (20)    18774 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/inverse_folding/gvp_modules.py
--rw-r--r--   0 maghoi     (502) staff       (20)     5140 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/inverse_folding/gvp_transformer.py
--rw-r--r--   0 maghoi     (502) staff       (20)     7232 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/inverse_folding/gvp_transformer_encoder.py
--rw-r--r--   0 maghoi     (502) staff       (20)     2966 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/inverse_folding/gvp_utils.py
--rw-r--r--   0 maghoi     (502) staff       (20)     6113 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/inverse_folding/multichain_util.py
--rw-r--r--   0 maghoi     (502) staff       (20)     7569 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/inverse_folding/transformer_decoder.py
--rw-r--r--   0 maghoi     (502) staff       (20)    10679 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/inverse_folding/transformer_layer.py
--rw-r--r--   0 maghoi     (502) staff       (20)    11715 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/inverse_folding/util.py
--rw-r--r--   0 maghoi     (502) staff       (20)     1883 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/modules.py
--rw-r--r--   0 maghoi     (502) staff       (20)    20748 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/multihead_attention.py
--rw-r--r--   0 maghoi     (502) staff       (20)    14213 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/pretrained.py
--rw-r--r--   0 maghoi     (502) staff       (20)     2785 2024-05-13 11:41:55.000000 antifold-0.2.0/antifold/esm/rotary_embedding.py
--rwxr-xr-x   0 maghoi     (502) staff       (20)    13995 2024-05-21 14:18:58.000000 antifold-0.2.0/antifold/esm_multichain_util_custom.py
--rwxr-xr-x   0 maghoi     (502) staff       (20)    21670 2024-05-21 14:18:54.000000 antifold-0.2.0/antifold/esm_util_custom.py
--rwxr-xr-x   0 maghoi     (502) staff       (20)     9255 2024-05-21 14:18:58.000000 antifold-0.2.0/antifold/if1_dataset.py
--rw-r--r--   0 maghoi     (502) staff       (20)    15379 2024-05-21 14:18:58.000000 antifold-0.2.0/antifold/main.py
-drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 14:24:43.402985 antifold-0.2.0/antifold.egg-info/
--rw-r--r--   0 maghoi     (502) staff       (20)      480 2024-05-21 14:24:43.000000 antifold-0.2.0/antifold.egg-info/PKG-INFO
--rw-r--r--   0 maghoi     (502) staff       (20)     1062 2024-05-21 14:24:43.000000 antifold-0.2.0/antifold.egg-info/SOURCES.txt
--rw-r--r--   0 maghoi     (502) staff       (20)        1 2024-05-21 14:24:43.000000 antifold-0.2.0/antifold.egg-info/dependency_links.txt
--rw-r--r--   0 maghoi     (502) staff       (20)       94 2024-05-21 14:24:43.000000 antifold-0.2.0/antifold.egg-info/requires.txt
--rw-r--r--   0 maghoi     (502) staff       (20)        9 2024-05-21 14:24:43.000000 antifold-0.2.0/antifold.egg-info/top_level.txt
--rw-r--r--   0 maghoi     (502) staff       (20)       94 2024-05-13 11:41:55.000000 antifold-0.2.0/requirements.txt
--rw-r--r--   0 maghoi     (502) staff       (20)       38 2024-05-21 14:24:43.433840 antifold-0.2.0/setup.cfg
--rw-r--r--   0 maghoi     (502) staff       (20)      708 2024-05-21 14:24:11.000000 antifold-0.2.0/setup.py
+drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 16:14:58.997236 antifold-0.2.1/
+-rw-r--r--   0 maghoi     (502) staff       (20)     1512 2024-05-13 11:41:55.000000 antifold-0.2.1/LICENSE
+-rw-r--r--   0 maghoi     (502) staff       (20)       24 2024-05-21 14:41:16.000000 antifold-0.2.1/MANIFEST.in
+-rw-r--r--   0 maghoi     (502) staff       (20)    11944 2024-05-21 16:14:58.996816 antifold-0.2.1/PKG-INFO
+-rw-r--r--   0 maghoi     (502) staff       (20)    11465 2024-05-21 16:13:33.000000 antifold-0.2.1/README.md
+drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 16:14:58.975656 antifold-0.2.1/antifold/
+-rw-r--r--   0 maghoi     (502) staff       (20)        0 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/__init__.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    26394 2024-05-21 15:01:46.000000 antifold-0.2.1/antifold/antiscripts.py
+drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 16:14:58.987221 antifold-0.2.1/antifold/esm/
+-rw-r--r--   0 maghoi     (502) staff       (20)      238 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/__init__.py
+-rw-r--r--   0 maghoi     (502) staff       (20)      371 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/constants.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    17438 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/data.py
+drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 16:14:58.995991 antifold-0.2.1/antifold/esm/inverse_folding/
+-rw-r--r--   0 maghoi     (502) staff       (20)      231 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/__init__.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    14800 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/features.py
+-rw-r--r--   0 maghoi     (502) staff       (20)     1790 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/gvp_encoder.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    18774 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/gvp_modules.py
+-rw-r--r--   0 maghoi     (502) staff       (20)     5140 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/gvp_transformer.py
+-rw-r--r--   0 maghoi     (502) staff       (20)     7232 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/gvp_transformer_encoder.py
+-rw-r--r--   0 maghoi     (502) staff       (20)     2966 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/gvp_utils.py
+-rw-r--r--   0 maghoi     (502) staff       (20)     6113 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/multichain_util.py
+-rw-r--r--   0 maghoi     (502) staff       (20)     7569 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/transformer_decoder.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    10679 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/transformer_layer.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    11715 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/util.py
+-rw-r--r--   0 maghoi     (502) staff       (20)     1883 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/modules.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    20748 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/multihead_attention.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    14213 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/pretrained.py
+-rw-r--r--   0 maghoi     (502) staff       (20)     2785 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/rotary_embedding.py
+-rwxr-xr-x   0 maghoi     (502) staff       (20)    13995 2024-05-21 14:18:58.000000 antifold-0.2.1/antifold/esm_multichain_util_custom.py
+-rwxr-xr-x   0 maghoi     (502) staff       (20)    21670 2024-05-21 14:18:54.000000 antifold-0.2.1/antifold/esm_util_custom.py
+-rwxr-xr-x   0 maghoi     (502) staff       (20)     9255 2024-05-21 14:18:58.000000 antifold-0.2.1/antifold/if1_dataset.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    15248 2024-05-21 15:06:53.000000 antifold-0.2.1/antifold/main.py
+drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 16:14:58.979258 antifold-0.2.1/antifold.egg-info/
+-rw-r--r--   0 maghoi     (502) staff       (20)    11944 2024-05-21 16:14:58.000000 antifold-0.2.1/antifold.egg-info/PKG-INFO
+-rw-r--r--   0 maghoi     (502) staff       (20)     1062 2024-05-21 16:14:58.000000 antifold-0.2.1/antifold.egg-info/SOURCES.txt
+-rw-r--r--   0 maghoi     (502) staff       (20)        1 2024-05-21 16:14:58.000000 antifold-0.2.1/antifold.egg-info/dependency_links.txt
+-rw-r--r--   0 maghoi     (502) staff       (20)       94 2024-05-21 16:14:58.000000 antifold-0.2.1/antifold.egg-info/requires.txt
+-rw-r--r--   0 maghoi     (502) staff       (20)        9 2024-05-21 16:14:58.000000 antifold-0.2.1/antifold.egg-info/top_level.txt
+-rw-r--r--   0 maghoi     (502) staff       (20)       94 2024-05-13 11:41:55.000000 antifold-0.2.1/requirements.txt
+-rw-r--r--   0 maghoi     (502) staff       (20)       38 2024-05-21 16:14:58.997435 antifold-0.2.1/setup.cfg
+-rw-r--r--   0 maghoi     (502) staff       (20)      938 2024-05-21 15:09:28.000000 antifold-0.2.1/setup.py
```

### Comparing `antifold-0.2.0/LICENSE` & `antifold-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/README.md` & `antifold-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,781 +1,747 @@
-00000000: 416e 7469 466f 6c64 0a3d 3d3d 3d3d 3d3d  AntiFold.=======
-00000010: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000020: 3d3d 3d3d 3d3d 3d0a 0a41 6e74 6946 6f6c  =======..AntiFol
-00000030: 6420 7072 6564 6963 7473 2073 6571 7565  d predicts seque
-00000040: 6e63 6573 2077 6869 6368 2066 6974 2069  nces which fit i
-00000050: 6e74 6f20 616e 2069 6e70 7574 2061 6e74  nto an input ant
-00000060: 6962 6f64 7920 7661 7269 6162 6c65 2064  ibody variable d
-00000070: 6f6d 6169 6e20 7374 7275 6374 7572 652e  omain structure.
-00000080: 2054 6865 2074 6f6f 6c20 6f75 7470 7574   The tool output
-00000090: 7320 7265 7369 6475 6520 6c6f 672d 6c69  s residue log-li
-000000a0: 6b65 6c69 686f 6f64 7320 696e 2043 5356  kelihoods in CSV
-000000b0: 2066 6f72 6d61 742c 2061 6e64 2063 616e   format, and can
-000000c0: 2073 616d 706c 6520 7365 7175 656e 6365   sample sequence
-000000d0: 7320 746f 2061 2046 4153 5441 2066 6f72  s to a FASTA for
-000000e0: 6d61 7420 6469 7265 6374 6c79 2e20 5361  mat directly. Sa
-000000f0: 6d70 6c65 6420 7365 7175 656e 6365 7320  mpled sequences 
-00000100: 7368 6f77 2068 6967 6820 7374 7275 6374  show high struct
-00000110: 7572 616c 2061 6772 6565 6d65 6e74 2077  ural agreement w
-00000120: 6974 6820 6578 7065 7269 6d65 6e74 616c  ith experimental
-00000130: 2073 7472 7563 7475 7265 732e 0a0a 416e   structures...An
-00000140: 7469 466f 6c64 2069 7320 6261 7365 6420  tiFold is based 
-00000150: 6f6e 2074 6865 2045 534d 2d49 4631 206d  on the ESM-IF1 m
-00000160: 6f64 656c 2061 6e64 2069 7320 6669 6e65  odel and is fine
-00000170: 2d74 756e 6564 206f 6e20 736f 6c76 6564  -tuned on solved
-00000180: 2061 6e64 2070 7265 6469 6374 6564 2061   and predicted a
-00000190: 6e74 6962 6f64 7920 7374 7275 6374 7572  ntibody structur
-000001a0: 6573 2066 726f 6d20 5341 6244 6162 2061  es from SAbDab a
-000001b0: 6e64 204f 4153 2e0a 0a2d 2050 6170 6572  nd OAS...- Paper
-000001c0: 3a20 5b61 7258 6976 2070 7265 2d70 7269  : [arXiv pre-pri
-000001d0: 6e74 5d28 6874 7470 733a 2f2f 6172 7869  nt](https://arxi
-000001e0: 762e 6f72 672f 6162 732f 3234 3035 2e30  v.org/abs/2405.0
-000001f0: 3333 3730 290a 2d20 5765 6273 6572 7665  3370).- Webserve
-00000200: 723a 205b 4f50 4947 2077 6562 7365 7276  r: [OPIG webserv
-00000210: 6572 5d28 6874 7470 733a 2f2f 6f70 6967  er](https://opig
-00000220: 2e73 7461 7473 2e6f 782e 6163 2e75 6b2f  .stats.ox.ac.uk/
-00000230: 7765 6261 7070 732f 616e 7469 666f 6c64  webapps/antifold
-00000240: 2f29 0a2d 2043 6f6c 6162 2028 6f75 7464  /).- Colab (outd
-00000250: 6174 6564 293a 205b 215b 4f70 656e 2049  ated): [![Open I
-00000260: 6e20 436f 6c61 625d 2869 6d61 6765 732f  n Colab](images/
-00000270: 636f 6c61 622d 6261 6467 652e 7376 6729  colab-badge.svg)
-00000280: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
-00000290: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
-000002a0: 636f 6d2f 6472 6976 652f 3154 5466 676a  com/drive/1TTfgj
-000002b0: 6f5a 7833 6d7a 4635 7534 6539 6234 556e  oZx3mzF5u4e9b4Un
-000002c0: 3959 3762 5f72 7158 635f 3429 0a2d 204d  9Y7b_rqXc_4).- M
-000002d0: 6f64 656c 3a20 5b6d 6f64 656c 2e70 745d  odel: [model.pt]
-000002e0: 2868 7474 7073 3a2f 2f6f 7069 672e 7374  (https://opig.st
-000002f0: 6174 732e 6f78 2e61 632e 756b 2f64 6174  ats.ox.ac.uk/dat
-00000300: 612f 646f 776e 6c6f 6164 732f 416e 7469  a/downloads/Anti
-00000310: 466f 6c64 2f6d 6f64 656c 732f 6d6f 6465  Fold/models/mode
-00000320: 6c2e 7074 290a 2d20 4c69 6365 6e73 653a  l.pt).- License:
-00000330: 205b 4253 4420 332d 436c 6175 7365 5d28   [BSD 3-Clause](
-00000340: 6874 7470 733a 2f2f 6f70 6967 2e73 7461  https://opig.sta
-00000350: 7473 2e6f 782e 6163 2e75 6b2f 6461 7461  ts.ox.ac.uk/data
-00000360: 2f64 6f77 6e6c 6f61 6473 2f41 6e74 6946  /downloads/AntiF
-00000370: 6f6c 642f 4c49 4345 4e53 4529 0a0a 2323  old/LICENSE)..##
-00000380: 2057 6562 7365 7276 6572 0a0a 546f 2074   Webserver..To t
-00000390: 7279 2041 6e74 6946 6f6c 6420 7769 7468  ry AntiFold with
-000003a0: 6f75 7420 696e 7374 616c 6c69 6e67 2069  out installing i
-000003b0: 742c 2070 6c65 6173 6520 7365 6520 6f75  t, please see ou
-000003c0: 7220 4f50 4947 2077 6562 7365 7276 6572  r OPIG webserver
-000003d0: 3a0a 5b68 7474 7073 3a2f 2f6f 7069 672e  :.[https://opig.
-000003e0: 7374 6174 732e 6f78 2e61 632e 756b 2f77  stats.ox.ac.uk/w
-000003f0: 6562 6170 7073 2f61 6e74 6966 6f6c 642f  ebapps/antifold/
-00000400: 5d28 6874 7470 733a 2f2f 6f70 6967 2e73  ](https://opig.s
-00000410: 7461 7473 2e6f 782e 6163 2e75 6b2f 7765  tats.ox.ac.uk/we
-00000420: 6261 7070 732f 616e 7469 666f 6c64 2f29  bapps/antifold/)
-00000430: 0a0a 2323 2049 6e73 7461 6c6c 2061 6e64  ..## Install and
-00000440: 2072 756e 2041 6e74 6946 6f6c 640a 0a23   run AntiFold..#
-00000450: 2323 2044 6f77 6e6c 6f61 6420 416e 7469  ## Download Anti
-00000460: 466f 6c64 2063 6f64 6520 616e 6420 6d6f  Fold code and mo
-00000470: 6465 6c0a 6060 6062 6173 680a 2320 446f  del.```bash.# Do
-00000480: 776e 6c6f 6164 2063 6f64 6520 616e 6420  wnload code and 
-00000490: 6d6f 6465 6c0a 6769 7420 636c 6f6e 6520  model.git clone 
-000004a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000004b0: 6f6d 2f6f 7870 6967 2f41 6e74 6946 6f6c  om/oxpig/AntiFol
-000004c0: 640a 6364 2041 6e74 6946 6f6c 640a 7767  d.cd AntiFold.wg
-000004d0: 6574 202d 5020 6d6f 6465 6c73 2f20 6874  et -P models/ ht
-000004e0: 7470 733a 2f2f 6f70 6967 2e73 7461 7473  tps://opig.stats
-000004f0: 2e6f 782e 6163 2e75 6b2f 6461 7461 2f64  .ox.ac.uk/data/d
-00000500: 6f77 6e6c 6f61 6473 2f41 6e74 6946 6f6c  ownloads/AntiFol
-00000510: 642f 6d6f 6465 6c73 2f6d 6f64 656c 2e70  d/models/model.p
-00000520: 740a 6060 600a 0a23 2323 2049 6e73 7461  t.```..### Insta
-00000530: 6c6c 2041 6e74 6946 6f6c 6420 2843 5055  ll AntiFold (CPU
-00000540: 290a 6060 6062 6173 680a 636f 6e64 6120  ).```bash.conda 
-00000550: 6372 6561 7465 202d 2d6e 616d 6520 616e  create --name an
-00000560: 7469 666f 6c64 2070 7974 686f 6e3d 332e  tifold python=3.
-00000570: 3130 202d 790a 636f 6e64 6120 6163 7469  10 -y.conda acti
-00000580: 7661 7465 2061 6e74 6966 6f6c 640a 636f  vate antifold.co
-00000590: 6e64 6120 696e 7374 616c 6c20 2d63 2070  nda install -c p
-000005a0: 7974 6f72 6368 2070 7974 6f72 6368 0a63  ytorch pytorch.c
-000005b0: 6f6e 6461 2069 6e73 7461 6c6c 202d 6320  onda install -c 
-000005c0: 7079 6720 7079 6720 2d79 0a63 6f6e 6461  pyg pyg -y.conda
-000005d0: 2069 6e73 7461 6c6c 202d 6320 636f 6e64   install -c cond
-000005e0: 612d 666f 7267 6520 7069 7020 2d79 0a23  a-forge pip -y.#
-000005f0: 2049 6e73 7461 6c6c 2041 6e74 6946 6f6c   Install AntiFol
-00000600: 6420 6672 6f6d 2061 6e74 6966 6f6c 645f  d from antifold_
-00000610: 636f 6465 2064 6972 6563 746f 7279 0a70  code directory.p
-00000620: 6970 2069 6e73 7461 6c6c 202e 0a70 6970  ip install ..pip
-00000630: 2069 6e73 7461 6c6c 2074 6f72 6368 2d67   install torch-g
-00000640: 656f 6d65 7472 6963 3d3d 322e 342e 300a  eometric==2.4.0.
-00000650: 6060 600a 0a23 2323 2049 6e73 7461 6c6c  ```..### Install
-00000660: 2041 6e74 6946 6f6c 6420 2847 5055 290a   AntiFold (GPU).
-00000670: 6060 6062 6173 680a 636f 6e64 6120 6372  ```bash.conda cr
-00000680: 6561 7465 202d 2d6e 616d 6520 616e 7469  eate --name anti
-00000690: 666f 6c64 2070 7974 686f 6e3d 332e 3130  fold python=3.10
-000006a0: 202d 790a 636f 6e64 6120 6163 7469 7661   -y.conda activa
-000006b0: 7465 2061 6e74 6966 6f6c 640a 636f 6e64  te antifold.cond
-000006c0: 6120 696e 7374 616c 6c20 2d63 2063 6f6e  a install -c con
-000006d0: 6461 2d66 6f72 6765 2070 7974 6f72 6368  da-forge pytorch
-000006e0: 2d67 7075 0a63 6f6e 6461 2069 6e73 7461  -gpu.conda insta
-000006f0: 6c6c 202d 6320 7079 6720 7079 6720 2d79  ll -c pyg pyg -y
-00000700: 0a63 6f6e 6461 2069 6e73 7461 6c6c 202d  .conda install -
-00000710: 6320 636f 6e64 612d 666f 7267 6520 7069  c conda-forge pi
-00000720: 7020 2d79 0a23 2049 6e73 7461 6c6c 2041  p -y.# Install A
-00000730: 6e74 6946 6f6c 6420 6672 6f6d 2061 6e74  ntiFold from ant
-00000740: 6966 6f6c 645f 636f 6465 2064 6972 6563  ifold_code direc
-00000750: 746f 7279 0a70 6970 2069 6e73 7461 6c6c  tory.pip install
-00000760: 202e 0a70 6970 2069 6e73 7461 6c6c 2074   ..pip install t
-00000770: 6f72 6368 2d67 656f 6d65 7472 6963 3d3d  orch-geometric==
-00000780: 322e 342e 300a 6060 600a 0a23 2323 2052  2.4.0.```..### R
-00000790: 756e 2041 6e74 6946 6f6c 6420 2869 6e76  un AntiFold (inv
-000007a0: 6572 7365 2d66 6f6c 6469 6e67 2070 726f  erse-folding pro
-000007b0: 6261 6269 6c69 7469 6573 2c20 7361 6d70  babilities, samp
-000007c0: 6c65 2073 6571 7565 6e63 6573 290a 6060  le sequences).``
-000007d0: 6062 6173 680a 2320 5275 6e20 416e 7469  `bash.# Run Anti
-000007e0: 466f 6c64 206f 6e20 7369 6e67 6c65 2050  Fold on single P
-000007f0: 4442 2f43 4946 2066 696c 650a 2320 4e62  DB/CIF file.# Nb
-00000800: 3a20 4173 7375 6d65 7320 6669 7273 7420  : Assumes first 
-00000810: 6368 6169 6e20 6865 6176 792c 2073 6563  chain heavy, sec
-00000820: 6f6e 6420 6368 6169 6e20 6c69 6768 740a  ond chain light.
-00000830: 7079 7468 6f6e 2061 6e74 6966 6f6c 642f  python antifold/
-00000840: 6d61 696e 2e70 7920 5c0a 2020 2020 2d2d  main.py \.    --
-00000850: 7064 625f 6669 6c65 2064 6174 612f 7064  pdb_file data/pd
-00000860: 6273 2f36 7931 6c5f 696d 6774 2e70 6462  bs/6y1l_imgt.pdb
-00000870: 0a0a 2320 5275 6e20 416e 7469 466f 6c64  ..# Run AntiFold
-00000880: 206f 6e20 616e 2061 6e74 6962 6f64 792d   on an antibody-
-00000890: 616e 7469 6765 6e20 636f 6d70 6c65 780a  antigen complex.
-000008a0: 7079 7468 6f6e 2061 6e74 6966 6f6c 642f  python antifold/
-000008b0: 6d61 696e 2e70 7920 5c0a 2020 2020 2d2d  main.py \.    --
-000008c0: 7064 625f 6669 6c65 2064 6174 612f 616e  pdb_file data/an
-000008d0: 7469 626f 6479 5f61 6e74 6967 656e 2f33  tibody_antigen/3
-000008e0: 6866 6d2e 7064 6220 5c0a 2020 2020 2d2d  hfm.pdb \.    --
-000008f0: 6865 6176 795f 6368 6169 6e20 4820 5c0a  heavy_chain H \.
-00000900: 2020 2020 2d2d 6c69 6768 745f 6368 6169      --light_chai
-00000910: 6e20 4c20 5c0a 2020 2020 2d2d 616e 7469  n L \.    --anti
-00000920: 6765 6e5f 6368 6169 6e20 590a 0a23 2052  gen_chain Y..# R
-00000930: 756e 2041 6e74 6946 6f6c 6420 6f6e 2061  un AntiFold on a
-00000940: 2066 6f6c 6465 7220 6f66 2050 4442 2f43   folder of PDB/C
-00000950: 4946 730a 2320 4e62 3a20 4173 7375 6d65  IFs.# Nb: Assume
-00000960: 7320 6669 7273 7420 6368 6169 6e20 6865  s first chain he
-00000970: 6176 792c 2073 6563 6f6e 6420 6c69 6768  avy, second ligh
-00000980: 740a 7079 7468 6f6e 2061 6e74 6966 6f6c  t.python antifol
-00000990: 642f 6d61 696e 2e70 7920 5c0a 2020 2020  d/main.py \.    
-000009a0: 2d2d 7064 625f 6469 7220 6461 7461 2f70  --pdb_dir data/p
-000009b0: 6462 730a 0a23 2053 7065 6369 6679 2063  dbs..# Specify c
-000009c0: 6861 696e 7320 746f 2072 756e 2069 6e20  hains to run in 
-000009d0: 6120 4353 5620 6669 6c65 2028 652e 672e  a CSV file (e.g.
-000009e0: 2061 6e74 6962 6f64 792d 616e 7469 6765   antibody-antige
-000009f0: 6e20 636f 6d70 6c65 7829 0a70 7974 686f  n complex).pytho
-00000a00: 6e20 616e 7469 666f 6c64 2f6d 6169 6e2e  n antifold/main.
-00000a10: 7079 205c 0a20 2020 202d 2d70 6462 5f64  py \.    --pdb_d
-00000a20: 6972 2064 6174 612f 616e 7469 626f 6479  ir data/antibody
-00000a30: 5f61 6e74 6967 656e 205c 0a20 2020 202d  _antigen \.    -
-00000a40: 2d70 6462 735f 6373 7620 6461 7461 2f61  -pdbs_csv data/a
-00000a50: 6e74 6962 6f64 795f 616e 7469 6765 6e2e  ntibody_antigen.
-00000a60: 6373 760a 0a23 2053 616d 706c 6520 7365  csv..# Sample se
-00000a70: 7175 656e 6365 7320 3130 780a 7079 7468  quences 10x.pyth
-00000a80: 6f6e 2061 6e74 6966 6f6c 642f 6d61 696e  on antifold/main
-00000a90: 2e70 7920 5c0a 2020 2020 2d2d 7064 625f  .py \.    --pdb_
-00000aa0: 6669 6c65 2064 6174 612f 7064 6273 2f36  file data/pdbs/6
-00000ab0: 7931 6c5f 696d 6774 2e70 6462 205c 0a20  y1l_imgt.pdb \. 
-00000ac0: 2020 202d 2d68 6561 7679 5f63 6861 696e     --heavy_chain
-00000ad0: 2048 205c 0a20 2020 202d 2d6c 6967 6874   H \.    --light
-00000ae0: 5f63 6861 696e 204c 205c 0a20 2020 202d  _chain L \.    -
-00000af0: 2d6e 756d 5f73 6571 5f70 6572 5f74 6172  -num_seq_per_tar
-00000b00: 6765 7420 3130 205c 0a20 2020 202d 2d73  get 10 \.    --s
-00000b10: 616d 706c 696e 675f 7465 6d70 2022 302e  ampling_temp "0.
-00000b20: 3222 205c 0a20 2020 202d 2d72 6567 696f  2" \.    --regio
-00000b30: 6e73 2022 4344 5231 2043 4452 3220 4344  ns "CDR1 CDR2 CD
-00000b40: 5233 220a 0a23 2052 756e 2061 6c6c 2063  R3"..# Run all c
-00000b50: 6861 696e 7320 7769 7468 2045 534d 2d49  hains with ESM-I
-00000b60: 4631 0a70 7974 686f 6e20 616e 7469 666f  F1.python antifo
-00000b70: 6c64 2f6d 6169 6e2e 7079 205c 0a20 2020  ld/main.py \.   
-00000b80: 202d 2d70 6462 5f64 6972 2064 6174 612f   --pdb_dir data/
-00000b90: 7064 6273 205c 0a20 2020 202d 2d65 736d  pdbs \.    --esm
-00000ba0: 5f69 6631 5f6d 6f64 650a 6060 600a 0a23  _if1_mode.```..#
-00000bb0: 2320 496e 7075 7420 7061 7261 6d65 7465  # Input paramete
-00000bc0: 7273 0a52 6571 7569 7265 6420 7061 7261  rs.Required para
-00000bd0: 6d65 7465 7273 3a0a 6060 6074 6578 740a  meters:.```text.
-00000be0: 496e 7075 7420 5044 4273 2073 686f 756c  Input PDBs shoul
-00000bf0: 6420 6265 2061 6e74 6962 6f64 7920 7661  d be antibody va
-00000c00: 7269 6162 6c65 2064 6f6d 6169 6e20 7374  riable domain st
-00000c10: 7275 6374 7572 6573 2028 494d 4754 2070  ructures (IMGT p
-00000c20: 6f73 6974 696f 6e73 2031 2d31 3238 292e  ositions 1-128).
-00000c30: 0a0a 4966 206e 6f20 6368 6169 6e73 2061  ..If no chains a
-00000c40: 7265 2073 7065 6369 6669 6564 2c20 7468  re specified, th
-00000c50: 6520 6669 7273 7420 7477 6f20 6368 6169  e first two chai
-00000c60: 6e73 2077 696c 6c20 6265 2061 7373 756d  ns will be assum
-00000c70: 6564 2074 6f20 6265 2068 6561 7679 206c  ed to be heavy l
-00000c80: 6967 6874 2e0a 4966 2063 7573 746f 6d5f  ight..If custom_
-00000c90: 6368 6169 6e5f 6d6f 6465 2069 7320 7365  chain_mode is se
-00000ca0: 742c 2061 6c6c 2028 3130 2920 6368 6169  t, all (10) chai
-00000cb0: 6e73 2077 696c 6c20 6265 2072 756e 2e0a  ns will be run..
-00000cc0: 0a2d 204f 7074 696f 6e20 313a 2050 4442  .- Option 1: PDB
-00000cd0: 2066 696c 6520 282d 2d70 6462 5f66 696c   file (--pdb_fil
-00000ce0: 6529 2e20 5765 2072 6563 6f6d 6d65 6e64  e). We recommend
-00000cf0: 2073 7065 6369 6679 696e 6720 6865 6176   specifying heav
-00000d00: 7920 616e 6420 6c69 6768 7420 6368 6169  y and light chai
-00000d10: 6e20 282d 2d68 6561 7679 5f63 6861 696e  n (--heavy_chain
-00000d20: 2061 6e64 202d 2d6c 6967 6874 5f63 6861   and --light_cha
-00000d30: 696e 290a 2d20 4f70 7469 6f6e 2032 3a20  in).- Option 2: 
-00000d40: 5044 4220 666f 6c64 6572 2028 2d2d 7064  PDB folder (--pd
-00000d50: 625f 6469 7229 202b 2043 5356 2066 696c  b_dir) + CSV fil
-00000d60: 6520 7370 6563 6966 7969 6e67 2063 6861  e specifying cha
-00000d70: 696e 7320 282d 2d70 6462 735f 6373 7629  ins (--pdbs_csv)
-00000d80: 0a2d 204f 7074 696f 6e20 333a 2050 4442  .- Option 3: PDB
-00000d90: 2066 6f6c 6465 722c 2069 6e66 6572 2031   folder, infer 1
-00000da0: 7374 2063 6861 696e 2068 6561 7679 2c20  st chain heavy, 
-00000db0: 326e 6420 6368 6169 6e20 6c69 6768 740a  2nd chain light.
-00000dc0: 6060 600a 0a50 6172 616d 6574 6572 7320  ```..Parameters 
-00000dd0: 666f 7220 6765 6e65 7261 7469 6e67 206e  for generating n
-00000de0: 6577 2073 6571 7565 6e63 6573 3a0a 6060  ew sequences:.``
-00000df0: 6074 6578 740a 5044 4273 2073 686f 756c  `text.PDBs shoul
-00000e00: 6420 6265 2049 4d47 5420 616e 6e6f 7461  d be IMGT annota
-00000e10: 7465 6420 666f 7220 7468 6520 7365 7175  ted for the sequ
-00000e20: 656e 6365 2073 616d 706c 696e 6720 7265  ence sampling re
-00000e30: 6769 6f6e 7320 746f 2062 6520 7661 6c69  gions to be vali
-00000e40: 642e 0a0a 2d20 4e75 6d62 6572 206f 6620  d...- Number of 
-00000e50: 7365 7175 656e 6365 7320 746f 2067 656e  sequences to gen
-00000e60: 6572 6174 6520 282d 2d6e 756d 5f73 6571  erate (--num_seq
-00000e70: 5f70 6572 5f74 6172 6765 7429 0a2d 2052  _per_target).- R
-00000e80: 6567 696f 6e20 746f 206d 7574 6174 6520  egion to mutate 
-00000e90: 282d 2d72 6567 696f 6e29 2062 6173 6564  (--region) based
-00000ea0: 206f 6e20 696e 7665 7273 6520 666f 6c64   on inverse fold
-00000eb0: 696e 6720 7072 6f62 6162 696c 6974 6965  ing probabilitie
-00000ec0: 732e 2053 656c 6563 7420 6672 6f6d 206c  s. Select from l
-00000ed0: 6973 7420 696e 2049 4d47 545f 6469 6374  ist in IMGT_dict
-00000ee0: 2028 652e 672e 2027 4344 5248 3120 4344   (e.g. 'CDRH1 CD
-00000ef0: 5248 3220 4344 5248 3327 290a 2d20 5361  RH2 CDRH3').- Sa
-00000f00: 6d70 6c69 6e67 2074 656d 7065 7261 7475  mpling temperatu
-00000f10: 7265 2028 2d2d 7361 6d70 6c69 6e67 5f74  re (--sampling_t
-00000f20: 656d 7029 2063 6f6e 7472 6f6c 7320 6765  emp) controls ge
-00000f30: 6e65 7261 7465 6420 7365 7175 656e 6365  nerated sequence
-00000f40: 2064 6976 6572 7369 7479 2c20 6279 2073   diversity, by s
-00000f50: 6361 6c69 6e67 2074 6865 2069 6e76 6572  caling the inver
-00000f60: 7365 2066 6f6c 6469 6e67 2070 726f 6261  se folding proba
-00000f70: 6269 6c69 7469 6573 2062 6566 6f72 6520  bilities before 
-00000f80: 7361 6d70 6c69 6e67 2e20 5465 6d70 6572  sampling. Temper
-00000f90: 6174 7572 6520 3d20 3120 6d65 616e 7320  ature = 1 means 
-00000fa0: 6e6f 2063 6861 6e67 652c 2077 6869 6c65  no change, while
-00000fb0: 2074 656d 7065 7261 7475 7265 207e 2030   temperature ~ 0
-00000fc0: 206f 6e6c 7920 7361 6d70 6c65 7320 7468   only samples th
-00000fd0: 6520 6d6f 7374 206c 696b 656c 7920 616d  e most likely am
-00000fe0: 696e 6f2d 6163 6964 2061 7420 6561 6368  ino-acid at each
-00000ff0: 2070 6f73 6974 696f 6e20 2861 6374 7320   position (acts 
-00001000: 6173 2061 7267 6d61 7829 2e0a 6060 600a  as argmax)..```.
-00001010: 0a4f 7074 696f 6e61 6c20 7061 7261 6d65  .Optional parame
-00001020: 7465 7273 3a0a 6060 6074 6578 740a 2d20  ters:.```text.- 
-00001030: 4d75 6c74 692d 6368 6169 6e20 6d6f 6465  Multi-chain mode
-00001040: 2066 6f72 2069 6e63 6c75 6469 6e67 2061   for including a
-00001050: 6e74 6967 656e 206f 7220 6f74 6865 7220  ntigen or other 
-00001060: 6368 6169 6e73 2028 2d2d 6375 7374 6f6d  chains (--custom
-00001070: 5f63 6861 696e 5f6d 6f64 6529 0a2d 2045  _chain_mode).- E
-00001080: 7874 7261 6374 206c 6174 656e 7420 7265  xtract latent re
-00001090: 7072 6573 656e 7461 7469 6f6e 7320 6f66  presentations of
-000010a0: 2050 4442 2077 6974 6869 6e20 6d6f 6465   PDB within mode
-000010b0: 6c20 282d 2d65 7874 7261 6374 5f65 6d62  l (--extract_emb
-000010c0: 6564 6469 6e67 7329 0a2d 2055 7365 2045  eddings).- Use E
-000010d0: 534d 2d49 4631 2069 6e73 7465 6164 206f  SM-IF1 instead o
-000010e0: 6620 416e 7469 466f 6c64 206d 6f64 656c  f AntiFold model
-000010f0: 2077 6569 6768 7473 2028 2d2d 6573 6d5f   weights (--esm_
-00001100: 6966 315f 6d6f 6465 292c 2065 6e61 626c  if1_mode), enabl
-00001110: 6573 2063 7573 746f 6d5f 6368 6169 6e5f  es custom_chain_
-00001120: 6d6f 6465 0a60 6060 0a0a 2323 2045 7861  mode.```..## Exa
-00001130: 6d70 6c65 206f 7574 7075 740a 466f 7220  mple output.For 
-00001140: 6578 616d 706c 6520 7765 6273 6572 7665  example webserve
-00001150: 7220 6f75 7470 7574 2c20 7365 653a 0a5b  r output, see:.[
-00001160: 6874 7470 733a 2f2f 6f70 6967 2e73 7461  https://opig.sta
-00001170: 7473 2e6f 782e 6163 2e75 6b2f 7765 6261  ts.ox.ac.uk/weba
-00001180: 7070 732f 616e 7469 666f 6c64 2f72 6573  pps/antifold/res
-00001190: 756c 7473 2f65 7861 6d70 6c65 5f6a 6f62  ults/example_job
-000011a0: 2f5d 2868 7474 7073 3a2f 2f6f 7069 672e  /](https://opig.
-000011b0: 7374 6174 732e 6f78 2e61 632e 756b 2f77  stats.ox.ac.uk/w
-000011c0: 6562 6170 7073 2f61 6e74 6966 6f6c 642f  ebapps/antifold/
-000011d0: 7265 7375 6c74 732f 6578 616d 706c 655f  results/example_
-000011e0: 6a6f 622f 290a 0a4f 7574 7075 7420 4353  job/)..Output CS
-000011f0: 5620 7769 7468 2072 6573 6964 7565 206c  V with residue l
-00001200: 6f67 2d70 726f 6261 6269 6c69 7469 6573  og-probabilities
-00001210: 3a20 5265 7369 6475 6520 7072 6f62 6162  : Residue probab
-00001220: 696c 6974 6965 733a 203c 6120 6872 6566  ilities: <a href
-00001230: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00001240: 2e63 6f6d 2f6f 7870 6967 2f41 6e74 6946  .com/oxpig/AntiF
-00001250: 6f6c 642f 626c 6f62 2f6d 6173 7465 722f  old/blob/master/
-00001260: 6f75 7470 7574 2f65 7861 6d70 6c65 5f70  output/example_p
-00001270: 6462 732f 3679 316c 5f69 6d67 742e 6373  dbs/6y1l_imgt.cs
-00001280: 7622 3e36 7931 6c5f 696d 6774 2e63 7376  v">6y1l_imgt.csv
-00001290: 3c2f 613e 0a2d 2070 6462 5f70 6f73 202d  </a>.- pdb_pos -
-000012a0: 2050 4442 2072 6573 6964 7565 206e 756d   PDB residue num
-000012b0: 6265 720a 2d20 7064 625f 6368 6169 6e20  ber.- pdb_chain 
-000012c0: 2d20 5044 4220 6368 6169 6e0a 2d20 6161  - PDB chain.- aa
-000012d0: 5f6f 7269 6720 2d20 5044 4220 7265 7369  _orig - PDB resi
-000012e0: 6475 6520 2865 2e67 2e20 3131 3229 0a2d  due (e.g. 112).-
-000012f0: 2061 615f 7072 6564 202d 2054 6f70 2070   aa_pred - Top p
-00001300: 7265 6469 6374 6564 2072 6573 6964 7565  redicted residue
-00001310: 2062 7920 416e 7469 466f 6c64 2028 692e   by AntiFold (i.
-00001320: 652e 2061 7267 6d61 7829 2066 6f72 2074  e. argmax) for t
-00001330: 6869 7320 706f 7369 7469 6f6e 0a2d 2070  his position.- p
-00001340: 6462 5f70 6f73 696e 7320 2d20 5044 4220  db_posins - PDB 
-00001350: 7265 7369 6475 6520 6e75 6d62 6572 2077  residue number w
-00001360: 6974 6820 696e 7365 7274 696f 6e20 636f  ith insertion co
-00001370: 6465 2028 652e 672e 2031 3132 4129 0a2d  de (e.g. 112A).-
-00001380: 2070 6572 706c 6578 6974 7920 2d20 496e   perplexity - In
-00001390: 7665 7273 6520 666f 6c64 696e 6720 746f  verse folding to
-000013a0: 6c65 7261 6e63 6520 2868 6967 6865 7220  lerance (higher 
-000013b0: 6973 206d 6f72 6520 746f 6c65 7261 6e74  is more tolerant
-000013c0: 2920 746f 206d 7574 6174 696f 6e73 2e20  ) to mutations. 
-000013d0: 5365 6520 7061 7065 7220 666f 7220 6d6f  See paper for mo
-000013e0: 7265 2064 6574 6169 6c73 2e0a 2d20 416d  re details..- Am
-000013f0: 696e 6f2d 6163 6964 7320 2d20 496e 7665  ino-acids - Inve
-00001400: 7273 6520 666f 6c64 696e 6720 7363 6f72  rse folding scor
-00001410: 6573 2028 6c6f 672d 6c69 6b65 6c69 686f  es (log-likeliho
-00001420: 6f64 2920 666f 7220 7468 6520 6769 7665  od) for the give
-00001430: 6e20 706f 7369 7469 6f6e 0a60 6060 6373  n position.```cs
-00001440: 760a 7064 625f 706f 732c 7064 625f 6368  v.pdb_pos,pdb_ch
-00001450: 6169 6e2c 6161 5f6f 7269 672c 6161 5f70  ain,aa_orig,aa_p
-00001460: 7265 642c 7064 625f 706f 7369 6e73 2c70  red,pdb_posins,p
-00001470: 6572 706c 6578 6974 792c 412c 432c 442c  erplexity,A,C,D,
-00001480: 452c 462c 472c 482c 492c 4b2c 4c2c 4d2c  E,F,G,H,I,K,L,M,
-00001490: 4e2c 502c 512c 522c 532c 542c 562c 572c  N,P,Q,R,S,T,V,W,
-000014a0: 590a 322c 482c 562c 4d2c 322c 312e 3634  Y.2,H,V,M,2,1.64
-000014b0: 3838 2c2d 342e 3939 3633 2c2d 362e 3631  88,-4.9963,-6.61
-000014c0: 3137 2c2d 362e 3331 3831 2c2d 362e 3332  17,-6.3181,-6.32
-000014d0: 3433 2c2d 362e 3735 3730 2c2d 342e 3235  43,-6.7570,-4.25
-000014e0: 3138 2c2d 362e 3735 3134 2c2d 352e 3235  18,-6.7514,-5.25
-000014f0: 3430 2c2d 362e 3830 3637 2c2d 352e 3836  40,-6.8067,-5.86
-00001500: 3139 2c2d 302e 3039 3034 2c2d 362e 3534  19,-0.0904,-6.54
-00001510: 3933 2c2d 342e 3836 3339 2c2d 362e 3633  93,-4.8639,-6.63
-00001520: 3136 2c2d 362e 3330 3834 2c2d 352e 3139  16,-6.3084,-5.19
-00001530: 3030 2c2d 352e 3039 3838 2c2d 332e 3732  00,-5.0988,-3.72
-00001540: 3935 2c2d 382e 3034 3830 2c2d 372e 3332  95,-8.0480,-7.32
-00001550: 3336 0a33 2c48 2c51 2c51 2c33 2c31 2e33  36.3,H,Q,Q,3,1.3
-00001560: 3838 392c 2d31 302e 3532 3538 2c2d 3132  889,-10.5258,-12
-00001570: 2e38 3436 332c 2d38 2e34 3830 302c 2d34  .8463,-8.4800,-4
-00001580: 2e37 3633 302c 2d31 322e 3930 3934 2c2d  .7630,-12.9094,-
-00001590: 3131 2e30 3932 342c 2d35 2e36 3133 362c  11.0924,-5.6136,
-000015a0: 2d31 302e 3938 3730 2c2d 332e 3131 3139  -10.9870,-3.1119
-000015b0: 2c2d 382e 3131 3133 2c2d 392e 3433 3832  ,-8.1113,-9.4382
-000015c0: 2c2d 362e 3232 3436 2c2d 3133 2e33 3636  ,-6.2246,-13.366
-000015d0: 302c 2d30 2e30 3730 312c 2d34 2e39 3935  0,-0.0701,-4.995
-000015e0: 372c 2d31 302e 3033 3031 2c2d 362e 3836  7,-10.0301,-6.86
-000015f0: 3138 2c2d 372e 3538 3130 2c2d 3133 2e36  18,-7.5810,-13.6
-00001600: 3732 312c 2d31 312e 3431 3537 0a34 2c48  721,-11.4157.4,H
-00001610: 2c4c 2c4c 2c34 2c31 2e30 3032 312c 2d31  ,L,L,4,1.0021,-1
-00001620: 332e 3335 3831 2c2d 3132 2e36 3230 362c  3.3581,-12.6206,
-00001630: 2d31 372e 3534 3834 2c2d 3132 2e34 3830  -17.5484,-12.480
-00001640: 312c 2d39 2e38 3739 322c 2d31 332e 3633  1,-9.8792,-13.63
-00001650: 3832 2c2d 3134 2e38 3630 392c 2d31 332e  82,-14.8609,-13.
-00001660: 3933 3434 2c2d 3136 2e34 3038 302c 2d30  9344,-16.4080,-0
-00001670: 2e30 3030 322c 2d39 2e32 3732 372c 2d31  .0002,-9.2727,-1
-00001680: 362e 3635 3332 2c2d 3134 2e30 3437 362c  6.6532,-14.0476,
-00001690: 2d31 322e 3539 3433 2c2d 3135 2e34 3535  -12.5943,-15.455
-000016a0: 392c 2d31 362e 3931 3033 2c2d 3137 2e30  9,-16.9103,-17.0
-000016b0: 3830 392c 2d31 302e 3536 3730 2c2d 3133  809,-10.5670,-13
-000016c0: 2e35 3333 342c 2d31 332e 3433 3234 0a2e  .5334,-13.4324..
-000016d0: 2e2e 0a60 6060 0a0a 4f75 7470 7574 2046  ...```..Output F
-000016e0: 4153 5441 2066 696c 6520 7769 7468 2073  ASTA file with s
-000016f0: 616d 706c 6564 2073 6571 7565 6e63 6573  ampled sequences
-00001700: 3a20 3c61 2068 7265 663d 2268 7474 7073  : <a href="https
-00001710: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f78  ://github.com/ox
-00001720: 7069 672f 416e 7469 466f 6c64 2f62 6c6f  pig/AntiFold/blo
-00001730: 622f 6d61 7374 6572 2f6f 7574 7075 742f  b/master/output/
-00001740: 6578 616d 706c 655f 7064 6273 2f36 7931  example_pdbs/6y1
-00001750: 6c5f 696d 6774 2e66 6173 7461 223e 3679  l_imgt.fasta">6y
-00001760: 316c 5f69 6d67 742e 6661 7374 613c 2f61  1l_imgt.fasta</a
-00001770: 3e0a 2d20 543a 2054 656d 7065 7261 7475  >.- T: Temperatu
-00001780: 7265 2075 7365 6420 666f 7220 6465 7369  re used for desi
-00001790: 676e 0a2d 2073 636f 7265 3a20 6176 6572  gn.- score: aver
-000017a0: 6167 6520 6c6f 672d 6f64 6473 206f 6620  age log-odds of 
-000017b0: 7265 7369 6475 6573 2069 6e20 7468 6520  residues in the 
-000017c0: 7361 6d70 6c65 6420 7265 6769 6f6e 0a2d  sampled region.-
-000017d0: 2067 6c6f 6261 6c5f 7363 6f72 653a 2061   global_score: a
-000017e0: 7665 7261 6765 206c 6f67 2d6f 6464 7320  verage log-odds 
-000017f0: 6f66 2061 6c6c 2072 6573 6964 7565 7320  of all residues 
-00001800: 2849 4d47 5420 706f 7369 7469 6f6e 7320  (IMGT positions 
-00001810: 312d 3132 3829 0a2d 2072 6567 696f 6e73  1-128).- regions
-00001820: 3a20 7265 6769 6f6e 7320 7365 6c65 6374  : regions select
-00001830: 6564 2066 6f72 2064 6573 6967 6e0a 2d20  ed for design.- 
-00001840: 7365 715f 7265 636f 7665 7279 3a20 2320  seq_recovery: # 
-00001850: 6d75 7461 7469 6f6e 7320 2f20 746f 7461  mutations / tota
-00001860: 6c20 7365 7175 656e 6365 206c 656e 6774  l sequence lengt
-00001870: 680a 2d20 6d75 7461 7469 6f6e 733a 2023  h.- mutations: #
-00001880: 206d 7574 6174 696f 6e73 2066 726f 6d20   mutations from 
-00001890: 6f72 6967 696e 616c 2050 4442 2073 6571  original PDB seq
-000018a0: 7565 6e63 650a 6060 6066 6173 7461 0a3e  uence.```fasta.>
-000018b0: 3679 316c 5f69 6d67 7420 2c20 7363 6f72  6y1l_imgt , scor
-000018c0: 653d 302e 3239 3334 2c20 676c 6f62 616c  e=0.2934, global
-000018d0: 5f73 636f 7265 3d30 2e32 3933 342c 2072  _score=0.2934, r
-000018e0: 6567 696f 6e73 3d5b 2743 4452 3127 2c20  egions=['CDR1', 
-000018f0: 2743 4452 3227 2c20 2743 4452 4833 275d  'CDR2', 'CDRH3']
-00001900: 2c20 6d6f 6465 6c5f 6e61 6d65 3d41 6e74  , model_name=Ant
-00001910: 6946 6f6c 642c 2073 6565 643d 3432 0a56  iFold, seed=42.V
-00001920: 514c 5145 5347 5047 4c56 4b50 5345 544c  QLQESGPGLVKPSETL
-00001930: 534c 5443 4156 5347 5953 4953 5347 5959  SLTCAVSGYSISSGYY
-00001940: 5747 5749 5251 5050 474b 474c 4557 4947  WGWIRQPPGKGLEWIG
-00001950: 5349 5948 5347 5354 5959 4e0a 5053 4c4b  SIYHSGSTYYN.PSLK
-00001960: 5352 5654 4953 5644 5453 4b4e 5146 534c  SRVTISVDTSKNQFSL
-00001970: 4b4c 5353 5654 4141 4454 4156 5959 4341  KLSSVTAADTAVYYCA
-00001980: 474c 5451 5353 484e 4441 4e57 4751 4754  GLTQSSHNDANWGQGT
-00001990: 4c56 5456 5353 2f56 0a4c 5451 5050 5356  LVTVSS/V.LTQPPSV
-000019a0: 5341 4150 4751 4b56 5449 5343 5347 5353  SAAPGQKVTISCSGSS
-000019b0: 534e 4947 4e4e 5956 5357 5951 514c 5047  SNIGNNYVSWYQQLPG
-000019c0: 5441 504b 524c 4959 444e 4e4b 5250 5347  TAPKRLIYDNNKRPSG
-000019d0: 4950 4452 460a 5347 534b 5347 5453 4154  IPDRF.SGSKSGTSAT
-000019e0: 4c47 4954 474c 5154 4744 4541 4459 5943  LGITGLQTGDEADYYC
-000019f0: 4754 5744 5353 4c4e 5056 4647 4747 544b  GTWDSSLNPVFGGGTK
-00001a00: 4c45 494b 520a 3e20 543d 302e 3230 2c20  LEIKR.> T=0.20, 
-00001a10: 7361 6d70 6c65 3d31 2c20 7363 6f72 653d  sample=1, score=
-00001a20: 302e 3339 3330 2c20 676c 6f62 616c 5f73  0.3930, global_s
-00001a30: 636f 7265 3d30 2e31 3836 392c 2073 6571  core=0.1869, seq
-00001a40: 5f72 6563 6f76 6572 793d 302e 3839 3833  _recovery=0.8983
-00001a50: 2c20 6d75 7461 7469 6f6e 733d 3132 0a56  , mutations=12.V
-00001a60: 514c 5145 5347 5047 4c56 4b50 5345 544c  QLQESGPGLVKPSETL
-00001a70: 534c 5443 4156 5347 4153 4954 5353 5959  SLTCAVSGASITSSYY
-00001a80: 5747 5749 5251 5050 474b 474c 4557 4947  WGWIRQPPGKGLEWIG
-00001a90: 5349 5959 5347 5354 5959 4e0a 5053 4c4b  SIYYSGSTYYN.PSLK
-00001aa0: 5352 5654 4953 5644 5453 4b4e 5146 534c  SRVTISVDTSKNQFSL
-00001ab0: 4b4c 5353 5654 4141 4454 4156 5959 4341  KLSSVTAADTAVYYCA
-00001ac0: 474c 5947 5350 5753 4e50 5957 4751 4754  GLYGSPWSNPYWGQGT
-00001ad0: 4c56 5456 5353 2f56 0a4c 5451 5050 5356  LVTVSS/V.LTQPPSV
-00001ae0: 5341 4150 4751 4b56 5449 5343 5347 5353  SAAPGQKVTISCSGSS
-00001af0: 534e 4947 4e4e 5956 5357 5951 514c 5047  SNIGNNYVSWYQQLPG
-00001b00: 5441 504b 524c 4959 444e 4e4b 5250 5347  TAPKRLIYDNNKRPSG
-00001b10: 4950 4452 460a 5347 534b 5347 5453 4154  IPDRF.SGSKSGTSAT
-00001b20: 4c47 4954 474c 5154 4744 4541 4459 5943  LGITGLQTGDEADYYC
-00001b30: 4754 5744 5353 4c4e 5056 4647 4747 544b  GTWDSSLNPVFGGGTK
-00001b40: 4c45 494b 520a 2e2e 2e0a 6060 600a 2323  LEIKR.....```.##
-00001b50: 2045 7861 6d70 6c65 206e 6f74 6562 6f6f   Example noteboo
-00001b60: 6b0a 4e6f 7465 626f 6f6b 3a20 3c61 2068  k.Notebook: <a h
-00001b70: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00001b80: 6875 622e 636f 6d2f 6f78 7069 672f 416e  hub.com/oxpig/An
-00001b90: 7469 466f 6c64 2f62 6c6f 622f 6d61 7374  tiFold/blob/mast
-00001ba0: 6572 2f6e 6f74 6562 6f6f 6b2e 6970 796e  er/notebook.ipyn
-00001bb0: 6222 3e6e 6f74 6562 6f6f 6b2e 6970 796e  b">notebook.ipyn
-00001bc0: 623c 2f61 3e0a 0a60 6060 7079 7468 6f6e  b</a>..```python
-00001bd0: 0a69 6d70 6f72 7420 7061 6e64 6173 2061  .import pandas a
-00001be0: 7320 7064 0a0a 2320 5075 7420 494d 4754  s pd..# Put IMGT
-00001bf0: 206e 756d 6265 7265 6420 5044 4273 2028   numbered PDBs (
-00001c00: 4676 206f 6e6c 792c 2049 4d47 5420 706f  Fv only, IMGT po
-00001c10: 7369 7469 6f6e 2031 2d31 3238 2920 746f  sition 1-128) to
-00001c20: 2070 726f 6365 7373 2061 6e64 206c 6f61   process and loa
-00001c30: 6420 6120 4353 5620 6669 6c65 2077 6974  d a CSV file wit
-00001c40: 6820 5044 4220 6e61 6d65 7320 616e 6420  h PDB names and 
-00001c50: 6865 6176 792f 6c69 6768 7420 6368 6169  heavy/light chai
-00001c60: 6e73 0a23 2044 6566 696e 6520 7468 6520  ns.# Define the 
-00001c70: 5044 4220 616e 6420 6368 6169 6e73 2069  PDB and chains i
-00001c80: 6e20 4461 7461 4672 616d 650a 7064 625f  n DataFrame.pdb_
-00001c90: 6469 7220 3d20 2264 6174 612f 7064 6273  dir = "data/pdbs
-00001ca0: 220a 6466 5f70 6462 7320 3d20 7064 2e72  ".df_pdbs = pd.r
-00001cb0: 6561 645f 6373 7628 2264 6174 612f 6578  ead_csv("data/ex
-00001cc0: 616d 706c 655f 7064 6273 2e63 7376 2229  ample_pdbs.csv")
-00001cd0: 0a0a 2320 5265 6769 6f6e 7320 746f 206d  ..# Regions to m
-00001ce0: 7574 6174 6520 2849 4d47 5429 0a72 6567  utate (IMGT).reg
-00001cf0: 696f 6e73 5f74 6f5f 6d75 7461 7465 203d  ions_to_mutate =
-00001d00: 205b 2243 4452 3122 2c20 2243 4452 3222   ["CDR1", "CDR2"
-00001d10: 2c20 2243 4452 3348 225d 0a0a 2320 4c6f  , "CDR3H"]..# Lo
-00001d20: 6164 206d 6f64 656c 0a69 6d70 6f72 7420  ad model.import 
-00001d30: 616e 7469 666f 6c64 2e6d 6169 6e20 6173  antifold.main as
-00001d40: 2061 6e74 6966 6f6c 640a 6d6f 6465 6c20   antifold.model 
-00001d50: 3d20 616e 7469 666f 6c64 2e6c 6f61 645f  = antifold.load_
-00001d60: 4946 315f 6d6f 6465 6c28 226d 6f64 656c  IF1_model("model
-00001d70: 732f 6d6f 6465 6c2e 7074 2229 0a0a 2320  s/model.pt")..# 
-00001d80: 5361 6d70 6c65 2066 726f 6d20 5044 4273  Sample from PDBs
-00001d90: 2c20 3130 2073 6571 7565 6e63 6573 2065  , 10 sequences e
-00001da0: 6163 6820 6174 2074 656d 7065 7261 7475  ach at temperatu
-00001db0: 7265 2030 2e35 3020 696e 2072 6567 696f  re 0.50 in regio
-00001dc0: 6e73 2043 4452 312c 2043 4452 322c 2043  ns CDR1, CDR2, C
-00001dd0: 4452 3348 0a70 6462 5f6f 7574 7075 745f  DR3H.pdb_output_
-00001de0: 6469 6374 203d 2061 6e74 6966 6f6c 642e  dict = antifold.
-00001df0: 7361 6d70 6c65 5f70 6462 7328 0a20 2020  sample_pdbs(.   
-00001e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e10: 206d 6f64 656c 2c0a 2020 2020 2020 2020   model,.        
-00001e20: 2020 2020 2020 2020 2020 2020 7064 6273              pdbs
-00001e30: 5f63 7376 5f6f 725f 6461 7461 6672 616d  _csv_or_datafram
-00001e40: 653d 6466 5f70 6462 732c 2023 2050 6174  e=df_pdbs, # Pat
-00001e50: 6820 746f 2043 5356 2066 696c 652c 206f  h to CSV file, o
-00001e60: 7220 6120 4461 7461 4672 616d 650a 2020  r a DataFrame.  
-00001e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e80: 2020 7265 6769 6f6e 735f 746f 5f6d 7574    regions_to_mut
-00001e90: 6174 653d 7265 6769 6f6e 735f 746f 5f6d  ate=regions_to_m
-00001ea0: 7574 6174 652c 0a20 2020 2020 2020 2020  utate,.         
-00001eb0: 2020 2020 2020 2020 2020 2070 6462 5f64             pdb_d
-00001ec0: 6972 3d22 6461 7461 2f70 6462 7322 2c0a  ir="data/pdbs",.
-00001ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ee0: 2020 2020 7361 6d70 6c65 5f6e 3d31 302c      sample_n=10,
-00001ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001f00: 2020 2020 2073 616d 706c 696e 675f 7465       sampling_te
-00001f10: 6d70 3d30 2e35 302c 0a20 2020 2020 2020  mp=0.50,.       
-00001f20: 2020 2020 2020 2020 2020 2020 206c 696d               lim
-00001f30: 6974 5f65 7870 6563 7465 645f 7661 7269  it_expected_vari
-00001f40: 6174 696f 6e3d 4661 6c73 650a 2020 2020  ation=False.    
-00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f60: 290a 0a23 204f 7574 7075 7420 6469 6374  )..# Output dict
-00001f70: 696f 6e61 7279 2077 6974 6820 7365 7175  ionary with sequ
-00001f80: 656e 6365 732c 2061 6e64 2072 6573 6964  ences, and resid
-00001f90: 7565 2070 726f 6261 6269 6c69 7469 6573  ue probabilities
-00001fa0: 206f 7220 6c6f 672d 6f64 6473 0a70 6462   or log-odds.pdb
-00001fb0: 7320 3d20 7064 625f 6f75 7470 7574 5f64  s = pdb_output_d
-00001fc0: 6963 742e 6b65 7973 2829 0a0a 2320 5265  ict.keys()..# Re
-00001fd0: 7369 6475 6520 6c6f 6720 7072 6f62 6162  sidue log probab
-00001fe0: 696c 6974 6965 730a 6466 5f6c 6f67 7072  ilities.df_logpr
-00001ff0: 6f62 7320 3d20 7064 625f 6f75 7470 7574  obs = pdb_output
-00002000: 5f64 6963 745b 2236 7931 6c5f 696d 6774  _dict["6y1l_imgt
-00002010: 225d 5b22 6c6f 6770 726f 6273 225d 0a0a  "]["logprobs"]..
-00002020: 2320 5361 6d70 6c65 6420 7365 7175 656e  # Sampled sequen
-00002030: 6365 730a 6661 7374 615f 6469 6374 203d  ces.fasta_dict =
-00002040: 2070 6462 5f6f 7574 7075 745f 6469 6374   pdb_output_dict
-00002050: 5b22 3679 316c 5f69 6d67 7422 5d5b 2273  ["6y1l_imgt"]["s
-00002060: 6571 7565 6e63 6573 225d 0a60 6060 0a0a  equences"].```..
-00002070: 2323 2055 7361 6765 0a60 6060 6261 7368  ## Usage.```bash
-00002080: 0a75 7361 6765 3a20 0a20 2020 2023 2050  .usage: .    # P
-00002090: 7265 6469 6374 206f 6e20 6578 616d 706c  redict on exampl
-000020a0: 6520 5044 4273 2069 6e20 666f 6c64 6572  e PDBs in folder
-000020b0: 0a70 7974 686f 6e20 616e 7469 666f 6c64  .python antifold
-000020c0: 2f6d 6169 6e2e 7079 205c 0a20 2020 202d  /main.py \.    -
-000020d0: 2d70 6462 5f66 696c 6520 6461 7461 2f61  -pdb_file data/a
-000020e0: 6e74 6962 6f64 795f 616e 7469 6765 6e2f  ntibody_antigen/
-000020f0: 3368 666d 2e70 6462 205c 0a20 2020 202d  3hfm.pdb \.    -
-00002100: 2d68 6561 7679 5f63 6861 696e 2048 205c  -heavy_chain H \
-00002110: 0a20 2020 202d 2d6c 6967 6874 5f63 6861  .    --light_cha
-00002120: 696e 204c 205c 0a20 2020 202d 2d61 6e74  in L \.    --ant
-00002130: 6967 656e 5f63 6861 696e 2059 2023 204f  igen_chain Y # O
-00002140: 7074 696f 6e61 6c0a 0a50 7265 6469 6374  ptional..Predict
-00002150: 2069 6e76 6572 7365 2066 6f6c 6469 6e67   inverse folding
-00002160: 2070 726f 6261 6269 6c69 7469 6573 2066   probabilities f
-00002170: 6f72 2061 6e74 6962 6f64 7920 7661 7269  or antibody vari
-00002180: 6162 6c65 2064 6f6d 6169 6e2c 2061 6e64  able domain, and
-00002190: 2073 616d 706c 6520 7365 7175 656e 6365   sample sequence
-000021a0: 7320 7769 7468 206d 6169 6e74 6169 6e65  s with maintaine
-000021b0: 6420 666f 6c64 2e0a 5044 4220 7374 7275  d fold..PDB stru
-000021c0: 6374 7572 6573 2073 686f 756c 6420 6265  ctures should be
-000021d0: 2049 4d47 542d 6e75 6d62 6572 6564 2c20   IMGT-numbered, 
-000021e0: 7061 6972 6564 2068 6561 7679 2061 6e64  paired heavy and
-000021f0: 206c 6967 6874 2063 6861 696e 2076 6172   light chain var
-00002200: 6961 626c 6520 646f 6d61 696e 7320 2870  iable domains (p
-00002210: 6f73 6974 696f 6e73 2031 2d31 3238 292e  ositions 1-128).
-00002220: 0a0a 466f 7220 494d 4754 206e 756d 6265  ..For IMGT numbe
-00002230: 7269 6e67 2050 4442 7320 7573 6520 5341  ring PDBs use SA
-00002240: 6244 6162 206f 7220 6874 7470 733a 2f2f  bDab or https://
-00002250: 6f70 6967 2e73 7461 7473 2e6f 782e 6163  opig.stats.ox.ac
-00002260: 2e75 6b2f 7765 6261 7070 732f 7361 6264  .uk/webapps/sabd
-00002270: 6162 2d73 6162 7072 6564 2f73 6162 7072  ab-sabpred/sabpr
-00002280: 6564 2f61 6e61 7263 692f 0a0a 6f70 7469  ed/anarci/..opti
-00002290: 6f6e 733a 0a20 202d 682c 202d 2d68 656c  ons:.  -h, --hel
-000022a0: 7020 2020 2020 2020 2020 2020 2073 686f  p            sho
-000022b0: 7720 7468 6973 2068 656c 7020 6d65 7373  w this help mess
-000022c0: 6167 6520 616e 6420 6578 6974 0a20 202d  age and exit.  -
-000022d0: 2d70 6462 5f66 696c 6520 5044 425f 4649  -pdb_file PDB_FI
-000022e0: 4c45 2020 2049 6e70 7574 2050 4442 2066  LE   Input PDB f
-000022f0: 696c 6520 2866 6f72 2073 696e 676c 6520  ile (for single 
-00002300: 5044 4220 7072 6564 6963 7469 6f6e 7329  PDB predictions)
-00002310: 0a20 202d 2d68 6561 7679 5f63 6861 696e  .  --heavy_chain
-00002320: 2048 4541 5659 5f43 4841 494e 0a20 2020   HEAVY_CHAIN.   
-00002330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002340: 2020 2020 2041 6220 6865 6176 7920 6368       Ab heavy ch
-00002350: 6169 6e20 2866 6f72 2073 696e 676c 6520  ain (for single 
-00002360: 5044 4220 7072 6564 6963 7469 6f6e 7329  PDB predictions)
-00002370: 0a20 202d 2d6c 6967 6874 5f63 6861 696e  .  --light_chain
-00002380: 204c 4947 4854 5f43 4841 494e 0a20 2020   LIGHT_CHAIN.   
-00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023a0: 2020 2020 2041 6220 6c69 6768 7420 6368       Ab light ch
-000023b0: 6169 6e20 2866 6f72 2073 696e 676c 6520  ain (for single 
-000023c0: 5044 4220 7072 6564 6963 7469 6f6e 7329  PDB predictions)
-000023d0: 0a20 202d 2d61 6e74 6967 656e 5f63 6861  .  --antigen_cha
-000023e0: 696e 2041 4e54 4947 454e 5f43 4841 494e  in ANTIGEN_CHAIN
-000023f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002400: 2020 2020 2020 2020 2041 6e74 6967 656e           Antigen
-00002410: 2063 6861 696e 2028 6f70 7469 6f6e 616c   chain (optional
-00002420: 290a 2020 2d2d 7064 6273 5f63 7376 2050  ).  --pdbs_csv P
-00002430: 4442 535f 4353 5620 2020 496e 7075 7420  DBS_CSV   Input 
-00002440: 4353 5620 6669 6c65 2077 6974 6820 5044  CSV file with PD
-00002450: 4220 6e61 6d65 7320 616e 6420 482f 4c20  B names and H/L 
-00002460: 6368 6169 6e73 2028 6d75 6c74 692d 5044  chains (multi-PD
-00002470: 4220 7072 6564 6963 7469 6f6e 7329 0a20  B predictions). 
-00002480: 202d 2d70 6462 5f64 6972 2050 4442 5f44   --pdb_dir PDB_D
-00002490: 4952 2020 2020 2044 6972 6563 746f 7279  IR     Directory
-000024a0: 2077 6974 6820 696e 7075 7420 5044 4220   with input PDB 
-000024b0: 6669 6c65 7320 286d 756c 7469 2d50 4442  files (multi-PDB
-000024c0: 2070 7265 6469 6374 696f 6e73 290a 2020   predictions).  
-000024d0: 2d2d 6f75 745f 6469 7220 4f55 545f 4449  --out_dir OUT_DI
-000024e0: 5220 2020 2020 4f75 7470 7574 2064 6972  R     Output dir
-000024f0: 6563 746f 7279 0a20 202d 2d72 6567 696f  ectory.  --regio
-00002500: 6e73 2052 4547 494f 4e53 2020 2020 2053  ns REGIONS     S
-00002510: 7061 6365 2d73 6570 6172 6174 6564 2072  pace-separated r
-00002520: 6567 696f 6e73 2074 6f20 6d75 7461 7465  egions to mutate
-00002530: 2e20 4465 6661 756c 7420 2743 4452 3120  . Default 'CDR1 
-00002540: 4344 5232 2043 4452 3348 270a 2020 2d2d  CDR2 CDR3H'.  --
-00002550: 6e75 6d5f 7365 715f 7065 725f 7461 7267  num_seq_per_targ
-00002560: 6574 204e 554d 5f53 4551 5f50 4552 5f54  et NUM_SEQ_PER_T
-00002570: 4152 4745 540a 2020 2020 2020 2020 2020  ARGET.          
-00002580: 2020 2020 2020 2020 2020 2020 2020 4e75                Nu
-00002590: 6d62 6572 206f 6620 7365 7175 656e 6365  mber of sequence
-000025a0: 7320 746f 2073 616d 706c 6520 6672 6f6d  s to sample from
-000025b0: 2065 6163 6820 616e 7469 626f 6479 2050   each antibody P
-000025c0: 4442 2028 6465 6661 756c 7420 3029 0a20  DB (default 0). 
-000025d0: 202d 2d73 616d 706c 696e 675f 7465 6d70   --sampling_temp
-000025e0: 2053 414d 504c 494e 475f 5445 4d50 0a20   SAMPLING_TEMP. 
-000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002600: 2020 2020 2020 2041 2073 7472 696e 6720         A string 
-00002610: 6f66 2074 656d 7065 7261 7475 7265 7320  of temperatures 
-00002620: 652e 672e 2027 302e 3230 2030 2e32 3520  e.g. '0.20 0.25 
-00002630: 302e 3530 2720 2864 6566 6175 6c74 2030  0.50' (default 0
-00002640: 2e32 3029 2e20 5361 6d70 6c69 6e67 2074  .20). Sampling t
-00002650: 656d 7065 7261 7475 7265 2066 6f72 2061  emperature for a
-00002660: 6d69 6e6f 2061 6369 6473 2e20 5375 6767  mino acids. Sugg
-00002670: 6573 7465 6420 7661 6c75 6573 2030 2e31  ested values 0.1
-00002680: 302c 2030 2e31 352c 2030 2e32 302c 2030  0, 0.15, 0.20, 0
-00002690: 2e32 352c 2030 2e33 302e 2048 6967 6865  .25, 0.30. Highe
-000026a0: 7220 7661 6c75 6573 2077 696c 6c20 6c65  r values will le
-000026b0: 6164 2074 6f20 6d6f 7265 2064 6976 6572  ad to more diver
-000026c0: 7369 7479 2e0a 2020 2d2d 6c69 6d69 745f  sity..  --limit_
-000026d0: 7661 7269 6174 696f 6e20 2020 2020 4c69  variation     Li
-000026e0: 6d69 7420 7661 7269 6174 696f 6e20 746f  mit variation to
-000026f0: 2061 7320 6d61 6e79 206d 7574 6174 696f   as many mutatio
-00002700: 6e73 2061 7320 6578 7065 6374 6564 2066  ns as expected f
-00002710: 726f 6d20 7465 6d70 6572 6174 7572 6520  rom temperature 
-00002720: 7361 6d70 6c69 6e67 0a20 202d 2d65 7874  sampling.  --ext
-00002730: 7261 6374 5f65 6d62 6564 6469 6e67 7320  ract_embeddings 
-00002740: 2045 7874 7261 6374 2070 6572 2d72 6573   Extract per-res
-00002750: 6964 7565 2065 6d62 6564 6469 6e67 7320  idue embeddings 
-00002760: 6672 6f6d 2041 6e74 6946 6f6c 6420 2f20  from AntiFold / 
-00002770: 4553 4d2d 4946 310a 2020 2d2d 6375 7374  ESM-IF1.  --cust
-00002780: 6f6d 5f63 6861 696e 5f6d 6f64 6520 2020  om_chain_mode   
-00002790: 5275 6e20 616c 6c20 7370 6563 6966 6965  Run all specifie
-000027a0: 6420 6368 6169 6e73 2028 666f 7220 616e  d chains (for an
-000027b0: 7469 626f 6479 2d61 6e74 6967 656e 2063  tibody-antigen c
-000027c0: 6f6d 706c 6578 6573 206f 7220 616e 7920  omplexes or any 
-000027d0: 636f 6d62 696e 6174 696f 6e20 6f66 2063  combination of c
-000027e0: 6861 696e 7329 0a20 202d 2d65 7863 6c75  hains).  --exclu
-000027f0: 6465 5f68 6561 7679 2020 2020 2020 2045  de_heavy       E
-00002800: 7863 6c75 6465 2068 6561 7679 2063 6861  xclude heavy cha
-00002810: 696e 2066 726f 6d20 7361 6d70 6c69 6e67  in from sampling
-00002820: 0a20 202d 2d65 7863 6c75 6465 5f6c 6967  .  --exclude_lig
-00002830: 6874 2020 2020 2020 2045 7863 6c75 6465  ht       Exclude
-00002840: 206c 6967 6874 2063 6861 696e 2066 726f   light chain fro
-00002850: 6d20 7361 6d70 6c69 6e67 0a20 202d 2d62  m sampling.  --b
-00002860: 6174 6368 5f73 697a 6520 4241 5443 485f  atch_size BATCH_
-00002870: 5349 5a45 0a20 2020 2020 2020 2020 2020  SIZE.           
-00002880: 2020 2020 2020 2020 2020 2020 2042 6174               Bat
-00002890: 6368 2d73 697a 6520 746f 2075 7365 0a20  ch-size to use. 
-000028a0: 202d 2d6e 756d 5f74 6872 6561 6473 204e   --num_threads N
-000028b0: 554d 5f54 4852 4541 4453 0a20 2020 2020  UM_THREADS.     
-000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028d0: 2020 204e 756d 6265 7220 6f66 2043 5055     Number of CPU
-000028e0: 2074 6872 6561 6473 2074 6f20 7573 6520   threads to use 
-000028f0: 666f 7220 7061 7261 6c6c 656c 2070 726f  for parallel pro
-00002900: 6365 7373 696e 6720 2830 203d 2061 6c6c  cessing (0 = all
-00002910: 2061 7661 696c 6162 6c65 290a 2020 2d2d   available).  --
-00002920: 7365 6564 2053 4545 4420 2020 2020 2020  seed SEED       
-00002930: 2020 2020 5365 6564 2066 6f72 2072 6570      Seed for rep
-00002940: 726f 6475 6369 6269 6c69 7479 0a20 202d  roducibility.  -
-00002950: 2d6d 6f64 656c 5f70 6174 6820 4d4f 4445  -model_path MODE
-00002960: 4c5f 5041 5448 0a20 2020 2020 2020 2020  L_PATH.         
-00002970: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-00002980: 6c74 6572 6e61 7469 7665 206d 6f64 656c  lternative model
-00002990: 2077 6569 6768 7473 2028 6465 6661 756c   weights (defaul
-000029a0: 7420 6d6f 6465 6c73 2f6d 6f64 656c 2e70  t models/model.p
-000029b0: 7429 2e20 5365 6520 2d2d 7573 655f 6573  t). See --use_es
-000029c0: 6d5f 6966 315f 7765 6967 6874 7320 666c  m_if1_weights fl
-000029d0: 6167 2074 6f20 7573 6520 4553 4d2d 4946  ag to use ESM-IF
-000029e0: 3120 7765 6967 6874 7320 696e 7374 6561  1 weights instea
-000029f0: 6420 6f66 2041 6e74 6946 6f6c 640a 2020  d of AntiFold.  
-00002a00: 2d2d 6573 6d5f 6966 315f 6d6f 6465 2020  --esm_if1_mode  
-00002a10: 2020 2020 2020 5573 6520 4553 4d2d 4946        Use ESM-IF
-00002a20: 3120 7765 6967 6874 7320 696e 7374 6561  1 weights instea
-00002a30: 6420 6f66 2041 6e74 6946 6f6c 640a 2020  d of AntiFold.  
-00002a40: 2d2d 7665 7262 6f73 6520 5645 5242 4f53  --verbose VERBOS
-00002a50: 4520 2020 2020 5665 7262 6f73 6520 7072  E     Verbose pr
-00002a60: 696e 7469 6e67 0a60 6060 0a0a 2323 2049  inting.```..## I
-00002a70: 4d47 5420 7265 6769 6f6e 7320 6469 6374  MGT regions dict
-00002a80: 0a55 7365 6420 746f 2073 7065 6369 6679  .Used to specify
-00002a90: 2077 6869 6368 2072 6567 696f 6e73 2074   which regions t
-00002aa0: 6f20 6d75 7461 7465 2069 6e20 616e 2049  o mutate in an I
-00002ab0: 4d47 5420 6e75 6d62 6572 6564 2050 4442  MGT numbered PDB
-00002ac0: 0a2d 2049 4d47 5420 6e75 6d62 6572 6564  .- IMGT numbered
-00002ad0: 2050 4442 733a 205b 6874 7470 733a 2f2f   PDBs: [https://
-00002ae0: 6f70 6967 2e73 7461 7473 2e6f 782e 6163  opig.stats.ox.ac
-00002af0: 2e75 6b2f 7765 6261 7070 732f 7361 6264  .uk/webapps/sabd
-00002b00: 6162 2d73 6162 7072 6564 2f73 6162 6461  ab-sabpred/sabda
-00002b10: 625d 2868 7474 7073 3a2f 2f6f 7069 672e  b](https://opig.
-00002b20: 7374 6174 732e 6f78 2e61 632e 756b 2f77  stats.ox.ac.uk/w
-00002b30: 6562 6170 7073 2f73 6162 6461 622d 7361  ebapps/sabdab-sa
-00002b40: 6270 7265 642f 7361 6264 6162 290a 2d20  bpred/sabdab).- 
-00002b50: 5265 6e75 6d62 6572 2065 7869 7374 696e  Renumber existin
-00002b60: 6720 5044 4273 2077 6974 6820 414e 4152  g PDBs with ANAR
-00002b70: 4349 3a20 5b68 7474 7073 3a2f 2f67 6974  CI: [https://git
-00002b80: 6875 622e 636f 6d2f 6f78 7069 672f 414e  hub.com/oxpig/AN
-00002b90: 4152 4349 5d28 6874 7470 733a 2f2f 6769  ARCI](https://gi
-00002ba0: 7468 7562 2e63 6f6d 2f6f 7870 6967 2f41  thub.com/oxpig/A
-00002bb0: 4e41 5243 4929 0a2d 2052 6561 6420 6d6f  NARCI).- Read mo
-00002bc0: 7265 3a20 5b68 7474 7073 3a2f 2f77 7777  re: [https://www
-00002bd0: 2e69 6d67 742e 6f72 672f 494d 4754 5363  .imgt.org/IMGTSc
-00002be0: 6965 6e74 6966 6963 4368 6172 742f 4e75  ientificChart/Nu
-00002bf0: 6d62 6572 696e 672f 494d 4754 4947 564c  mbering/IMGTIGVL
-00002c00: 7375 7065 7266 616d 696c 792e 6874 6d6c  superfamily.html
-00002c10: 5d28 6874 7470 733a 2f2f 7777 772e 696d  ](https://www.im
-00002c20: 6774 2e6f 7267 2f49 4d47 5453 6369 656e  gt.org/IMGTScien
-00002c30: 7469 6669 6343 6861 7274 2f4e 756d 6265  tificChart/Numbe
-00002c40: 7269 6e67 2f49 4d47 5449 4756 4c73 7570  ring/IMGTIGVLsup
-00002c50: 6572 6661 6d69 6c79 2e68 746d 6c29 0a0a  erfamily.html)..
-00002c60: 6060 6070 7974 686f 6e0a 494d 4754 5f64  ```python.IMGT_d
-00002c70: 6963 7420 3d20 7b0a 2020 2020 2261 6c6c  ict = {.    "all
-00002c80: 223a 2072 616e 6765 2831 2c20 3132 3820  ": range(1, 128 
-00002c90: 2b20 3129 2c0a 2020 2020 2261 6c6c 4822  + 1),.    "allH"
-00002ca0: 3a20 7261 6e67 6528 312c 2031 3238 202b  : range(1, 128 +
-00002cb0: 2031 292c 0a20 2020 2022 616c 6c4c 223a   1),.    "allL":
-00002cc0: 2072 616e 6765 2831 2c20 3132 3820 2b20   range(1, 128 + 
-00002cd0: 3129 2c0a 2020 2020 2246 5748 223a 206c  1),.    "FWH": l
-00002ce0: 6973 7428 7261 6e67 6528 312c 2032 3620  ist(range(1, 26 
-00002cf0: 2b20 3129 2920 2b20 6c69 7374 2872 616e  + 1)) + list(ran
-00002d00: 6765 2834 302c 2035 3520 2b20 3129 2920  ge(40, 55 + 1)) 
-00002d10: 2b20 6c69 7374 2872 616e 6765 2836 362c  + list(range(66,
-00002d20: 2031 3034 202b 2031 2929 2c0a 2020 2020   104 + 1)),.    
-00002d30: 2246 574c 223a 206c 6973 7428 7261 6e67  "FWL": list(rang
-00002d40: 6528 312c 2032 3620 2b20 3129 2920 2b20  e(1, 26 + 1)) + 
-00002d50: 6c69 7374 2872 616e 6765 2834 302c 2035  list(range(40, 5
-00002d60: 3520 2b20 3129 2920 2b20 6c69 7374 2872  5 + 1)) + list(r
-00002d70: 616e 6765 2836 362c 2031 3034 202b 2031  ange(66, 104 + 1
-00002d80: 2929 2c0a 2020 2020 2243 4452 4822 3a20  )),.    "CDRH": 
-00002d90: 6c69 7374 2872 616e 6765 2832 372c 2033  list(range(27, 3
-00002da0: 3929 2920 2b20 6c69 7374 2872 616e 6765  9)) + list(range
-00002db0: 2835 362c 2036 3520 2b20 3129 2920 2b20  (56, 65 + 1)) + 
-00002dc0: 6c69 7374 2872 616e 6765 2831 3035 2c20  list(range(105, 
-00002dd0: 3131 3720 2b20 3129 292c 0a20 2020 2022  117 + 1)),.    "
-00002de0: 4344 524c 223a 206c 6973 7428 7261 6e67  CDRL": list(rang
-00002df0: 6528 3237 2c20 3339 2929 202b 206c 6973  e(27, 39)) + lis
-00002e00: 7428 7261 6e67 6528 3536 2c20 3635 202b  t(range(56, 65 +
-00002e10: 2031 2929 202b 206c 6973 7428 7261 6e67   1)) + list(rang
-00002e20: 6528 3130 352c 2031 3137 202b 2031 2929  e(105, 117 + 1))
-00002e30: 2c0a 2020 2020 2246 5731 223a 2072 616e  ,.    "FW1": ran
-00002e40: 6765 2831 2c20 3236 202b 2031 292c 0a20  ge(1, 26 + 1),. 
-00002e50: 2020 2022 4657 4831 223a 2072 616e 6765     "FWH1": range
-00002e60: 2831 2c20 3236 202b 2031 292c 0a20 2020  (1, 26 + 1),.   
-00002e70: 2022 4657 4c31 223a 2072 616e 6765 2831   "FWL1": range(1
-00002e80: 2c20 3236 202b 2031 292c 0a20 2020 2022  , 26 + 1),.    "
-00002e90: 4344 5231 223a 2072 616e 6765 2832 372c  CDR1": range(27,
-00002ea0: 2033 3929 2c0a 2020 2020 2243 4452 4831   39),.    "CDRH1
-00002eb0: 223a 2072 616e 6765 2832 372c 2033 3929  ": range(27, 39)
-00002ec0: 2c0a 2020 2020 2243 4452 4c31 223a 2072  ,.    "CDRL1": r
-00002ed0: 616e 6765 2832 372c 2033 3929 2c0a 2020  ange(27, 39),.  
-00002ee0: 2020 2246 5732 223a 2072 616e 6765 2834    "FW2": range(4
-00002ef0: 302c 2035 3520 2b20 3129 2c0a 2020 2020  0, 55 + 1),.    
-00002f00: 2246 5748 3222 3a20 7261 6e67 6528 3430  "FWH2": range(40
-00002f10: 2c20 3535 202b 2031 292c 0a20 2020 2022  , 55 + 1),.    "
-00002f20: 4657 4c32 223a 2072 616e 6765 2834 302c  FWL2": range(40,
-00002f30: 2035 3520 2b20 3129 2c0a 2020 2020 2243   55 + 1),.    "C
-00002f40: 4452 3222 3a20 7261 6e67 6528 3536 2c20  DR2": range(56, 
-00002f50: 3635 202b 2031 292c 0a20 2020 2022 4344  65 + 1),.    "CD
-00002f60: 5248 3222 3a20 7261 6e67 6528 3536 2c20  RH2": range(56, 
-00002f70: 3635 202b 2031 292c 0a20 2020 2022 4344  65 + 1),.    "CD
-00002f80: 524c 3222 3a20 7261 6e67 6528 3536 2c20  RL2": range(56, 
-00002f90: 3635 202b 2031 292c 0a20 2020 2022 4657  65 + 1),.    "FW
-00002fa0: 3322 3a20 7261 6e67 6528 3636 2c20 3130  3": range(66, 10
-00002fb0: 3420 2b20 3129 2c0a 2020 2020 2246 5748  4 + 1),.    "FWH
-00002fc0: 3322 3a20 7261 6e67 6528 3636 2c20 3130  3": range(66, 10
-00002fd0: 3420 2b20 3129 2c0a 2020 2020 2246 574c  4 + 1),.    "FWL
-00002fe0: 3322 3a20 7261 6e67 6528 3636 2c20 3130  3": range(66, 10
-00002ff0: 3420 2b20 3129 2c0a 2020 2020 2243 4452  4 + 1),.    "CDR
-00003000: 3322 3a20 7261 6e67 6528 3130 352c 2031  3": range(105, 1
-00003010: 3137 202b 2031 292c 0a20 2020 2022 4344  17 + 1),.    "CD
-00003020: 5248 3322 3a20 7261 6e67 6528 3130 352c  RH3": range(105,
-00003030: 2031 3137 202b 2031 292c 0a20 2020 2022   117 + 1),.    "
-00003040: 4344 524c 3322 3a20 7261 6e67 6528 3130  CDRL3": range(10
-00003050: 352c 2031 3137 202b 2031 292c 0a20 2020  5, 117 + 1),.   
-00003060: 2022 4657 3422 3a20 7261 6e67 6528 3131   "FW4": range(11
-00003070: 382c 2031 3238 202b 2031 292c 0a20 2020  8, 128 + 1),.   
-00003080: 2022 4657 4834 223a 2072 616e 6765 2831   "FWH4": range(1
-00003090: 3138 2c20 3132 3820 2b20 3129 2c0a 2020  18, 128 + 1),.  
-000030a0: 2020 2246 574c 3422 3a20 7261 6e67 6528    "FWL4": range(
-000030b0: 3131 382c 2031 3238 202b 2031 292c 0a7d  118, 128 + 1),.}
-000030c0: 0a60 6060 0a                             .```.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 616e 7469  : 2.1.Name: anti
+00000020: 666f 6c64 0a56 6572 7369 6f6e 3a20 302e  fold.Version: 0.
+00000030: 322e 310a 5375 6d6d 6172 793a 2049 6e76  2.1.Summary: Inv
+00000040: 6572 7365 2066 6f6c 6469 6e67 206f 6620  erse folding of 
+00000050: 616e 7469 626f 6469 6573 0a48 6f6d 652d  antibodies.Home-
+00000060: 7061 6765 3a20 6874 7470 733a 2f2f 6769  page: https://gi
+00000070: 7468 7562 2e63 6f6d 2f6f 7870 6967 2f41  thub.com/oxpig/A
+00000080: 6e74 6946 6f6c 642f 0a41 7574 686f 723a  ntiFold/.Author:
+00000090: 204d 6167 6e75 7320 4861 7261 6c64 736f   Magnus Haraldso
+000000a0: 6e20 48c3 b869 6520 2620 416c 6973 7361  n H..ie & Alissa
+000000b0: 2048 756d 6d65 720a 4175 7468 6f72 2d65   Hummer.Author-e
+000000c0: 6d61 696c 3a20 6d61 6768 6f69 4064 7475  mail: maghoi@dtu
+000000d0: 2e64 6b0a 436c 6173 7369 6669 6572 3a20  .dk.Classifier: 
+000000e0: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
+000000f0: 7573 203a 3a20 3520 2d20 5072 6f64 7563  us :: 5 - Produc
+00000100: 7469 6f6e 2f53 7461 626c 650a 436c 6173  tion/Stable.Clas
+00000110: 7369 6669 6572 3a20 496e 7465 6e64 6564  sifier: Intended
+00000120: 2041 7564 6965 6e63 6520 3a3a 2053 6369   Audience :: Sci
+00000130: 656e 6365 2f52 6573 6561 7263 680a 436c  ence/Research.Cl
+00000140: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
+00000150: 696e 6720 5379 7374 656d 203a 3a20 504f  ing System :: PO
+00000160: 5349 5820 3a3a 204c 696e 7578 0a43 6c61  SIX :: Linux.Cla
+00000170: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000180: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000190: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
+000001a0: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
+000001b0: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
+000001c0: 6172 6b64 6f77 6e0a 4c69 6365 6e73 652d  arkdown.License-
+000001d0: 4669 6c65 3a20 4c49 4345 4e53 450a 0a41  File: LICENSE..A
+000001e0: 6e74 6946 6f6c 640a 3d3d 3d3d 3d3d 3d3d  ntiFold.========
+000001f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000200: 3d3d 3d3d 3d3d 0a0a 416e 7469 466f 6c64  ======..AntiFold
+00000210: 2070 7265 6469 6374 7320 7365 7175 656e   predicts sequen
+00000220: 6365 7320 7768 6963 6820 6669 7420 696e  ces which fit in
+00000230: 746f 2061 6e20 696e 7075 7420 616e 7469  to an input anti
+00000240: 626f 6479 2076 6172 6961 626c 6520 646f  body variable do
+00000250: 6d61 696e 2073 7472 7563 7475 7265 2e20  main structure. 
+00000260: 5468 6520 746f 6f6c 206f 7574 7075 7473  The tool outputs
+00000270: 2072 6573 6964 7565 206c 6f67 2d6c 696b   residue log-lik
+00000280: 656c 6968 6f6f 6473 2069 6e20 4353 5620  elihoods in CSV 
+00000290: 666f 726d 6174 2c20 616e 6420 6361 6e20  format, and can 
+000002a0: 7361 6d70 6c65 2073 6571 7565 6e63 6573  sample sequences
+000002b0: 2074 6f20 6120 4641 5354 4120 666f 726d   to a FASTA form
+000002c0: 6174 2064 6972 6563 746c 792e 2053 616d  at directly. Sam
+000002d0: 706c 6564 2073 6571 7565 6e63 6573 2073  pled sequences s
+000002e0: 686f 7720 6869 6768 2073 7472 7563 7475  how high structu
+000002f0: 7261 6c20 6167 7265 656d 656e 7420 7769  ral agreement wi
+00000300: 7468 2065 7870 6572 696d 656e 7461 6c20  th experimental 
+00000310: 7374 7275 6374 7572 6573 2e0a 0a41 6e74  structures...Ant
+00000320: 6946 6f6c 6420 6973 2062 6173 6564 206f  iFold is based o
+00000330: 6e20 7468 6520 4553 4d2d 4946 3120 6d6f  n the ESM-IF1 mo
+00000340: 6465 6c20 616e 6420 6973 2066 696e 652d  del and is fine-
+00000350: 7475 6e65 6420 6f6e 2073 6f6c 7665 6420  tuned on solved 
+00000360: 616e 6420 7072 6564 6963 7465 6420 616e  and predicted an
+00000370: 7469 626f 6479 2073 7472 7563 7475 7265  tibody structure
+00000380: 7320 6672 6f6d 2053 4162 4461 6220 616e  s from SAbDab an
+00000390: 6420 4f41 532e 0a0a 2d20 5061 7065 723a  d OAS...- Paper:
+000003a0: 205b 6172 5869 7620 7072 652d 7072 696e   [arXiv pre-prin
+000003b0: 745d 2868 7474 7073 3a2f 2f61 7278 6976  t](https://arxiv
+000003c0: 2e6f 7267 2f61 6273 2f32 3430 352e 3033  .org/abs/2405.03
+000003d0: 3337 3029 0a2d 2057 6562 7365 7276 6572  370).- Webserver
+000003e0: 3a20 5b4f 5049 4720 7765 6273 6572 7665  : [OPIG webserve
+000003f0: 725d 2868 7474 7073 3a2f 2f6f 7069 672e  r](https://opig.
+00000400: 7374 6174 732e 6f78 2e61 632e 756b 2f77  stats.ox.ac.uk/w
+00000410: 6562 6170 7073 2f61 6e74 6966 6f6c 642f  ebapps/antifold/
+00000420: 290a 2d20 436f 6c61 6220 286f 7574 6461  ).- Colab (outda
+00000430: 7465 6429 3a20 5b21 5b4f 7065 6e20 496e  ted): [![Open In
+00000440: 2043 6f6c 6162 5d28 696d 6167 6573 2f63   Colab](images/c
+00000450: 6f6c 6162 2d62 6164 6765 2e73 7667 295d  olab-badge.svg)]
+00000460: 2868 7474 7073 3a2f 2f63 6f6c 6162 2e72  (https://colab.r
+00000470: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
+00000480: 6f6d 2f64 7269 7665 2f31 5454 6667 6a6f  om/drive/1TTfgjo
+00000490: 5a78 336d 7a46 3575 3465 3962 3455 6e39  Zx3mzF5u4e9b4Un9
+000004a0: 5937 625f 7271 5863 5f34 290a 2d20 4d6f  Y7b_rqXc_4).- Mo
+000004b0: 6465 6c3a 205b 6d6f 6465 6c2e 7074 5d28  del: [model.pt](
+000004c0: 6874 7470 733a 2f2f 6f70 6967 2e73 7461  https://opig.sta
+000004d0: 7473 2e6f 782e 6163 2e75 6b2f 6461 7461  ts.ox.ac.uk/data
+000004e0: 2f64 6f77 6e6c 6f61 6473 2f41 6e74 6946  /downloads/AntiF
+000004f0: 6f6c 642f 6d6f 6465 6c73 2f6d 6f64 656c  old/models/model
+00000500: 2e70 7429 0a2d 204c 6963 656e 7365 3a20  .pt).- License: 
+00000510: 5b42 5344 2033 2d43 6c61 7573 655d 2868  [BSD 3-Clause](h
+00000520: 7474 7073 3a2f 2f6f 7069 672e 7374 6174  ttps://opig.stat
+00000530: 732e 6f78 2e61 632e 756b 2f64 6174 612f  s.ox.ac.uk/data/
+00000540: 646f 776e 6c6f 6164 732f 416e 7469 466f  downloads/AntiFo
+00000550: 6c64 2f4c 4943 454e 5345 290a 0a23 2320  ld/LICENSE)..## 
+00000560: 5765 6273 6572 7665 720a 0a54 6f20 7472  Webserver..To tr
+00000570: 7920 416e 7469 466f 6c64 2077 6974 686f  y AntiFold witho
+00000580: 7574 2069 6e73 7461 6c6c 696e 6720 6974  ut installing it
+00000590: 2c20 706c 6561 7365 2073 6565 206f 7572  , please see our
+000005a0: 204f 5049 4720 7765 6273 6572 7665 723a   OPIG webserver:
+000005b0: 0a5b 6874 7470 733a 2f2f 6f70 6967 2e73  .[https://opig.s
+000005c0: 7461 7473 2e6f 782e 6163 2e75 6b2f 7765  tats.ox.ac.uk/we
+000005d0: 6261 7070 732f 616e 7469 666f 6c64 2f5d  bapps/antifold/]
+000005e0: 2868 7474 7073 3a2f 2f6f 7069 672e 7374  (https://opig.st
+000005f0: 6174 732e 6f78 2e61 632e 756b 2f77 6562  ats.ox.ac.uk/web
+00000600: 6170 7073 2f61 6e74 6966 6f6c 642f 290a  apps/antifold/).
+00000610: 0a23 2320 496e 7374 616c 6c20 616e 6420  .## Install and 
+00000620: 7275 6e20 416e 7469 466f 6c64 0a0a 0a23  run AntiFold...#
+00000630: 2323 2049 6e73 7461 6c6c 2041 6e74 6946  ## Install AntiF
+00000640: 6f6c 6420 7769 7468 2070 6970 2028 4350  old with pip (CP
+00000650: 5529 0a60 6060 6261 7368 0a63 6f6e 6461  U).```bash.conda
+00000660: 2063 7265 6174 6520 2d2d 6e61 6d65 2061   create --name a
+00000670: 6e74 6966 6f6c 6420 7079 7468 6f6e 3d33  ntifold python=3
+00000680: 2e31 3020 2d79 2026 2620 6163 7469 7661  .10 -y && activa
+00000690: 7465 2061 6e74 6966 6f6c 640a 7069 7020  te antifold.pip 
+000006a0: 696e 7374 616c 6c20 616e 7469 666f 6c64  install antifold
+000006b0: 0a60 6060 0a0a 2323 2320 496e 7374 616c  .```..### Instal
+000006c0: 6c20 416e 7469 466f 6c64 2077 6974 6820  l AntiFold with 
+000006d0: 7069 7020 2847 5055 290a 6060 6062 6173  pip (GPU).```bas
+000006e0: 680a 636f 6e64 6120 6372 6561 7465 202d  h.conda create -
+000006f0: 2d6e 616d 6520 616e 7469 666f 6c64 2070  -name antifold p
+00000700: 7974 686f 6e3d 332e 3130 202d 7920 2626  ython=3.10 -y &&
+00000710: 2061 6374 6976 6174 6520 616e 7469 666f   activate antifo
+00000720: 6c64 0a63 6f6e 6461 2069 6e73 7461 6c6c  ld.conda install
+00000730: 202d 6320 636f 6e64 612d 666f 7267 6520   -c conda-forge 
+00000740: 7079 746f 7263 682d 6770 750a 7069 7020  pytorch-gpu.pip 
+00000750: 696e 7374 616c 6c20 616e 7469 666f 6c64  install antifold
+00000760: 0a60 6060 0a0a 2323 2320 446f 776e 6c6f  .```..### Downlo
+00000770: 6164 2061 6e64 2069 6e73 7461 6c6c 2066  ad and install f
+00000780: 726f 6d20 4769 7468 7562 2073 6f75 7263  rom Github sourc
+00000790: 6520 286c 6174 6573 7420 7265 6c65 6173  e (latest releas
+000007a0: 6529 0a60 6060 6261 7368 0a23 2044 6f77  e).```bash.# Dow
+000007b0: 6e6c 6f61 6420 636f 6465 2061 6e64 206d  nload code and m
+000007c0: 6f64 656c 0a67 6974 2063 6c6f 6e65 2068  odel.git clone h
+000007d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000007e0: 6d2f 6f78 7069 672f 416e 7469 466f 6c64  m/oxpig/AntiFold
+000007f0: 2026 2620 6364 2041 6e74 6946 6f6c 640a   && cd AntiFold.
+00000800: 636f 6e64 6120 6372 6561 7465 202d 2d6e  conda create --n
+00000810: 616d 6520 616e 7469 666f 6c64 2070 7974  ame antifold pyt
+00000820: 686f 6e3d 332e 3130 202d 7920 2626 2063  hon=3.10 -y && c
+00000830: 6f6e 6461 2061 6374 6976 6174 6520 616e  onda activate an
+00000840: 7469 666f 6c64 0a70 6970 2069 6e73 7461  tifold.pip insta
+00000850: 6c6c 202e 0a60 6060 0a0a 2323 2320 5275  ll ..```..### Ru
+00000860: 6e20 416e 7469 466f 6c64 2028 696e 7665  n AntiFold (inve
+00000870: 7273 652d 666f 6c64 696e 6720 7072 6f62  rse-folding prob
+00000880: 6162 696c 6974 6965 732c 2073 616d 706c  abilities, sampl
+00000890: 6520 7365 7175 656e 6365 7329 0a60 6060  e sequences).```
+000008a0: 6261 7368 0a23 2052 756e 2041 6e74 6946  bash.# Run AntiF
+000008b0: 6f6c 6420 6f6e 2073 696e 676c 6520 5044  old on single PD
+000008c0: 422f 4349 4620 6669 6c65 0a23 204e 623a  B/CIF file.# Nb:
+000008d0: 2041 7373 756d 6573 2066 6972 7374 2063   Assumes first c
+000008e0: 6861 696e 2068 6561 7679 2c20 7365 636f  hain heavy, seco
+000008f0: 6e64 2063 6861 696e 206c 6967 6874 0a70  nd chain light.p
+00000900: 7974 686f 6e20 616e 7469 666f 6c64 2f6d  ython antifold/m
+00000910: 6169 6e2e 7079 205c 0a20 2020 202d 2d70  ain.py \.    --p
+00000920: 6462 5f66 696c 6520 6461 7461 2f70 6462  db_file data/pdb
+00000930: 732f 3679 316c 5f69 6d67 742e 7064 620a  s/6y1l_imgt.pdb.
+00000940: 0a23 2052 756e 2041 6e74 6946 6f6c 6420  .# Run AntiFold 
+00000950: 6f6e 2061 6e20 616e 7469 626f 6479 2d61  on an antibody-a
+00000960: 6e74 6967 656e 2063 6f6d 706c 6578 0a70  ntigen complex.p
+00000970: 7974 686f 6e20 616e 7469 666f 6c64 2f6d  ython antifold/m
+00000980: 6169 6e2e 7079 205c 0a20 2020 202d 2d70  ain.py \.    --p
+00000990: 6462 5f66 696c 6520 6461 7461 2f61 6e74  db_file data/ant
+000009a0: 6962 6f64 795f 616e 7469 6765 6e2f 3368  ibody_antigen/3h
+000009b0: 666d 2e70 6462 205c 0a20 2020 202d 2d68  fm.pdb \.    --h
+000009c0: 6561 7679 5f63 6861 696e 2048 205c 0a20  eavy_chain H \. 
+000009d0: 2020 202d 2d6c 6967 6874 5f63 6861 696e     --light_chain
+000009e0: 204c 205c 0a20 2020 202d 2d61 6e74 6967   L \.    --antig
+000009f0: 656e 5f63 6861 696e 2059 0a0a 2320 5275  en_chain Y..# Ru
+00000a00: 6e20 416e 7469 466f 6c64 206f 6e20 6120  n AntiFold on a 
+00000a10: 666f 6c64 6572 206f 6620 5044 422f 4349  folder of PDB/CI
+00000a20: 4673 0a23 204e 623a 2041 7373 756d 6573  Fs.# Nb: Assumes
+00000a30: 2066 6972 7374 2063 6861 696e 2068 6561   first chain hea
+00000a40: 7679 2c20 7365 636f 6e64 206c 6967 6874  vy, second light
+00000a50: 0a70 7974 686f 6e20 616e 7469 666f 6c64  .python antifold
+00000a60: 2f6d 6169 6e2e 7079 205c 0a20 2020 202d  /main.py \.    -
+00000a70: 2d70 6462 5f64 6972 2064 6174 612f 7064  -pdb_dir data/pd
+00000a80: 6273 0a0a 2320 5370 6563 6966 7920 6368  bs..# Specify ch
+00000a90: 6169 6e73 2074 6f20 7275 6e20 696e 2061  ains to run in a
+00000aa0: 2043 5356 2066 696c 6520 2865 2e67 2e20   CSV file (e.g. 
+00000ab0: 616e 7469 626f 6479 2d61 6e74 6967 656e  antibody-antigen
+00000ac0: 2063 6f6d 706c 6578 290a 7079 7468 6f6e   complex).python
+00000ad0: 2061 6e74 6966 6f6c 642f 6d61 696e 2e70   antifold/main.p
+00000ae0: 7920 5c0a 2020 2020 2d2d 7064 625f 6469  y \.    --pdb_di
+00000af0: 7220 6461 7461 2f61 6e74 6962 6f64 795f  r data/antibody_
+00000b00: 616e 7469 6765 6e20 5c0a 2020 2020 2d2d  antigen \.    --
+00000b10: 7064 6273 5f63 7376 2064 6174 612f 616e  pdbs_csv data/an
+00000b20: 7469 626f 6479 5f61 6e74 6967 656e 2e63  tibody_antigen.c
+00000b30: 7376 0a0a 2320 5361 6d70 6c65 2073 6571  sv..# Sample seq
+00000b40: 7565 6e63 6573 2031 3078 0a70 7974 686f  uences 10x.pytho
+00000b50: 6e20 616e 7469 666f 6c64 2f6d 6169 6e2e  n antifold/main.
+00000b60: 7079 205c 0a20 2020 202d 2d70 6462 5f66  py \.    --pdb_f
+00000b70: 696c 6520 6461 7461 2f70 6462 732f 3679  ile data/pdbs/6y
+00000b80: 316c 5f69 6d67 742e 7064 6220 5c0a 2020  1l_imgt.pdb \.  
+00000b90: 2020 2d2d 6865 6176 795f 6368 6169 6e20    --heavy_chain 
+00000ba0: 4820 5c0a 2020 2020 2d2d 6c69 6768 745f  H \.    --light_
+00000bb0: 6368 6169 6e20 4c20 5c0a 2020 2020 2d2d  chain L \.    --
+00000bc0: 6e75 6d5f 7365 715f 7065 725f 7461 7267  num_seq_per_targ
+00000bd0: 6574 2031 3020 5c0a 2020 2020 2d2d 7361  et 10 \.    --sa
+00000be0: 6d70 6c69 6e67 5f74 656d 7020 2230 2e32  mpling_temp "0.2
+00000bf0: 2220 5c0a 2020 2020 2d2d 7265 6769 6f6e  " \.    --region
+00000c00: 7320 2243 4452 3120 4344 5232 2043 4452  s "CDR1 CDR2 CDR
+00000c10: 3322 0a0a 2320 5275 6e20 616c 6c20 6368  3"..# Run all ch
+00000c20: 6169 6e73 2077 6974 6820 4553 4d2d 4946  ains with ESM-IF
+00000c30: 310a 7079 7468 6f6e 2061 6e74 6966 6f6c  1.python antifol
+00000c40: 642f 6d61 696e 2e70 7920 5c0a 2020 2020  d/main.py \.    
+00000c50: 2d2d 7064 625f 6469 7220 6461 7461 2f70  --pdb_dir data/p
+00000c60: 6462 7320 5c0a 2020 2020 2d2d 6573 6d5f  dbs \.    --esm_
+00000c70: 6966 315f 6d6f 6465 0a60 6060 0a0a 2323  if1_mode.```..##
+00000c80: 2045 7861 6d70 6c65 206e 6f74 6562 6f6f   Example noteboo
+00000c90: 6b0a 4e6f 7465 626f 6f6b 3a20 3c61 2068  k.Notebook: <a h
+00000ca0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000cb0: 6875 622e 636f 6d2f 6f78 7069 672f 416e  hub.com/oxpig/An
+00000cc0: 7469 466f 6c64 2f62 6c6f 622f 6d61 7374  tiFold/blob/mast
+00000cd0: 6572 2f6e 6f74 6562 6f6f 6b2e 6970 796e  er/notebook.ipyn
+00000ce0: 6222 3e6e 6f74 6562 6f6f 6b2e 6970 796e  b">notebook.ipyn
+00000cf0: 623c 2f61 3e0a 0a60 6060 7079 7468 6f6e  b</a>..```python
+00000d00: 0a69 6d70 6f72 7420 616e 7469 666f 6c64  .import antifold
+00000d10: 0a69 6d70 6f72 7420 616e 7469 666f 6c64  .import antifold
+00000d20: 2e6d 6169 6e0a 0a23 204c 6f61 6420 6d6f  .main..# Load mo
+00000d30: 6465 6c0a 6d6f 6465 6c20 3d20 616e 7469  del.model = anti
+00000d40: 666f 6c64 2e6d 6169 6e2e 6c6f 6164 5f6d  fold.main.load_m
+00000d50: 6f64 656c 2829 0a0a 2320 5044 4220 6469  odel()..# PDB di
+00000d60: 7265 6374 6f72 790a 7064 625f 6469 7220  rectory.pdb_dir 
+00000d70: 3d20 2264 6174 612f 7064 6273 220a 0a23  = "data/pdbs"..#
+00000d80: 2041 7373 756d 6573 2066 6972 7374 2063   Assumes first c
+00000d90: 6861 696e 2068 6561 7679 2c20 7365 636f  hain heavy, seco
+00000da0: 6e64 2063 6861 696e 206c 6967 6874 0a70  nd chain light.p
+00000db0: 6462 735f 6373 7620 3d20 616e 7469 666f  dbs_csv = antifo
+00000dc0: 6c64 2e6d 6169 6e2e 6765 6e65 7261 7465  ld.main.generate
+00000dd0: 5f70 6462 735f 6373 7628 7064 625f 6469  _pdbs_csv(pdb_di
+00000de0: 722c 206d 6178 5f63 6861 696e 733d 3229  r, max_chains=2)
+00000df0: 0a0a 2320 5361 6d70 6c65 2066 726f 6d20  ..# Sample from 
+00000e00: 5044 4273 0a64 665f 6c6f 6769 7473 5f6c  PDBs.df_logits_l
+00000e10: 6973 7420 3d20 616e 7469 666f 6c64 2e6d  ist = antifold.m
+00000e20: 6169 6e2e 6765 745f 7064 6273 5f6c 6f67  ain.get_pdbs_log
+00000e30: 6974 7328 0a20 2020 206d 6f64 656c 3d6d  its(.    model=m
+00000e40: 6f64 656c 2c0a 2020 2020 7064 6273 5f63  odel,.    pdbs_c
+00000e50: 7376 5f6f 725f 6461 7461 6672 616d 653d  sv_or_dataframe=
+00000e60: 7064 6273 5f63 7376 2c0a 2020 2020 7064  pdbs_csv,.    pd
+00000e70: 625f 6469 723d 7064 625f 6469 722c 0a29  b_dir=pdb_dir,.)
+00000e80: 0a0a 2320 4f75 7470 7574 206c 6f67 2070  ..# Output log p
+00000e90: 726f 6261 6269 6c69 7465 730a 6466 5f6c  robabilites.df_l
+00000ea0: 6f67 6974 735f 6c69 7374 5b30 5d0a 6060  ogits_list[0].``
+00000eb0: 600a 0a23 2320 496e 7075 7420 7061 7261  `..## Input para
+00000ec0: 6d65 7465 7273 0a52 6571 7569 7265 6420  meters.Required 
+00000ed0: 7061 7261 6d65 7465 7273 3a0a 6060 6074  parameters:.```t
+00000ee0: 6578 740a 496e 7075 7420 5044 4273 2073  ext.Input PDBs s
+00000ef0: 686f 756c 6420 6265 2061 6e74 6962 6f64  hould be antibod
+00000f00: 7920 7661 7269 6162 6c65 2064 6f6d 6169  y variable domai
+00000f10: 6e20 7374 7275 6374 7572 6573 2028 494d  n structures (IM
+00000f20: 4754 2070 6f73 6974 696f 6e73 2031 2d31  GT positions 1-1
+00000f30: 3238 292e 0a0a 4966 206e 6f20 6368 6169  28)...If no chai
+00000f40: 6e73 2061 7265 2073 7065 6369 6669 6564  ns are specified
+00000f50: 2c20 7468 6520 6669 7273 7420 7477 6f20  , the first two 
+00000f60: 6368 6169 6e73 2077 696c 6c20 6265 2061  chains will be a
+00000f70: 7373 756d 6564 2074 6f20 6265 2068 6561  ssumed to be hea
+00000f80: 7679 206c 6967 6874 2e0a 4966 2063 7573  vy light..If cus
+00000f90: 746f 6d5f 6368 6169 6e5f 6d6f 6465 2069  tom_chain_mode i
+00000fa0: 7320 7365 742c 2061 6c6c 2028 3130 2920  s set, all (10) 
+00000fb0: 6368 6169 6e73 2077 696c 6c20 6265 2072  chains will be r
+00000fc0: 756e 2e0a 0a2d 204f 7074 696f 6e20 313a  un...- Option 1:
+00000fd0: 2050 4442 2066 696c 6520 282d 2d70 6462   PDB file (--pdb
+00000fe0: 5f66 696c 6529 2e20 5765 2072 6563 6f6d  _file). We recom
+00000ff0: 6d65 6e64 2073 7065 6369 6679 696e 6720  mend specifying 
+00001000: 6865 6176 7920 616e 6420 6c69 6768 7420  heavy and light 
+00001010: 6368 6169 6e20 282d 2d68 6561 7679 5f63  chain (--heavy_c
+00001020: 6861 696e 2061 6e64 202d 2d6c 6967 6874  hain and --light
+00001030: 5f63 6861 696e 290a 2d20 4f70 7469 6f6e  _chain).- Option
+00001040: 2032 3a20 5044 4220 666f 6c64 6572 2028   2: PDB folder (
+00001050: 2d2d 7064 625f 6469 7229 202b 2043 5356  --pdb_dir) + CSV
+00001060: 2066 696c 6520 7370 6563 6966 7969 6e67   file specifying
+00001070: 2063 6861 696e 7320 282d 2d70 6462 735f   chains (--pdbs_
+00001080: 6373 7629 0a2d 204f 7074 696f 6e20 333a  csv).- Option 3:
+00001090: 2050 4442 2066 6f6c 6465 722c 2069 6e66   PDB folder, inf
+000010a0: 6572 2031 7374 2063 6861 696e 2068 6561  er 1st chain hea
+000010b0: 7679 2c20 326e 6420 6368 6169 6e20 6c69  vy, 2nd chain li
+000010c0: 6768 740a 6060 600a 0a50 6172 616d 6574  ght.```..Paramet
+000010d0: 6572 7320 666f 7220 6765 6e65 7261 7469  ers for generati
+000010e0: 6e67 206e 6577 2073 6571 7565 6e63 6573  ng new sequences
+000010f0: 3a0a 6060 6074 6578 740a 5044 4273 2073  :.```text.PDBs s
+00001100: 686f 756c 6420 6265 2049 4d47 5420 616e  hould be IMGT an
+00001110: 6e6f 7461 7465 6420 666f 7220 7468 6520  notated for the 
+00001120: 7365 7175 656e 6365 2073 616d 706c 696e  sequence samplin
+00001130: 6720 7265 6769 6f6e 7320 746f 2062 6520  g regions to be 
+00001140: 7661 6c69 642e 0a0a 2d20 4e75 6d62 6572  valid...- Number
+00001150: 206f 6620 7365 7175 656e 6365 7320 746f   of sequences to
+00001160: 2067 656e 6572 6174 6520 282d 2d6e 756d   generate (--num
+00001170: 5f73 6571 5f70 6572 5f74 6172 6765 7429  _seq_per_target)
+00001180: 0a2d 2052 6567 696f 6e20 746f 206d 7574  .- Region to mut
+00001190: 6174 6520 282d 2d72 6567 696f 6e29 2062  ate (--region) b
+000011a0: 6173 6564 206f 6e20 696e 7665 7273 6520  ased on inverse 
+000011b0: 666f 6c64 696e 6720 7072 6f62 6162 696c  folding probabil
+000011c0: 6974 6965 732e 2053 656c 6563 7420 6672  ities. Select fr
+000011d0: 6f6d 206c 6973 7420 696e 2049 4d47 545f  om list in IMGT_
+000011e0: 6469 6374 2028 652e 672e 2027 4344 5248  dict (e.g. 'CDRH
+000011f0: 3120 4344 5248 3220 4344 5248 3327 290a  1 CDRH2 CDRH3').
+00001200: 2d20 5361 6d70 6c69 6e67 2074 656d 7065  - Sampling tempe
+00001210: 7261 7475 7265 2028 2d2d 7361 6d70 6c69  rature (--sampli
+00001220: 6e67 5f74 656d 7029 2063 6f6e 7472 6f6c  ng_temp) control
+00001230: 7320 6765 6e65 7261 7465 6420 7365 7175  s generated sequ
+00001240: 656e 6365 2064 6976 6572 7369 7479 2c20  ence diversity, 
+00001250: 6279 2073 6361 6c69 6e67 2074 6865 2069  by scaling the i
+00001260: 6e76 6572 7365 2066 6f6c 6469 6e67 2070  nverse folding p
+00001270: 726f 6261 6269 6c69 7469 6573 2062 6566  robabilities bef
+00001280: 6f72 6520 7361 6d70 6c69 6e67 2e20 5465  ore sampling. Te
+00001290: 6d70 6572 6174 7572 6520 3d20 3120 6d65  mperature = 1 me
+000012a0: 616e 7320 6e6f 2063 6861 6e67 652c 2077  ans no change, w
+000012b0: 6869 6c65 2074 656d 7065 7261 7475 7265  hile temperature
+000012c0: 207e 2030 206f 6e6c 7920 7361 6d70 6c65   ~ 0 only sample
+000012d0: 7320 7468 6520 6d6f 7374 206c 696b 656c  s the most likel
+000012e0: 7920 616d 696e 6f2d 6163 6964 2061 7420  y amino-acid at 
+000012f0: 6561 6368 2070 6f73 6974 696f 6e20 2861  each position (a
+00001300: 6374 7320 6173 2061 7267 6d61 7829 2e0a  cts as argmax)..
+00001310: 6060 600a 0a4f 7074 696f 6e61 6c20 7061  ```..Optional pa
+00001320: 7261 6d65 7465 7273 3a0a 6060 6074 6578  rameters:.```tex
+00001330: 740a 2d20 4d75 6c74 692d 6368 6169 6e20  t.- Multi-chain 
+00001340: 6d6f 6465 2066 6f72 2069 6e63 6c75 6469  mode for includi
+00001350: 6e67 2061 6e74 6967 656e 206f 7220 6f74  ng antigen or ot
+00001360: 6865 7220 6368 6169 6e73 2028 2d2d 6375  her chains (--cu
+00001370: 7374 6f6d 5f63 6861 696e 5f6d 6f64 6529  stom_chain_mode)
+00001380: 0a2d 2045 7874 7261 6374 206c 6174 656e  .- Extract laten
+00001390: 7420 7265 7072 6573 656e 7461 7469 6f6e  t representation
+000013a0: 7320 6f66 2050 4442 2077 6974 6869 6e20  s of PDB within 
+000013b0: 6d6f 6465 6c20 282d 2d65 7874 7261 6374  model (--extract
+000013c0: 5f65 6d62 6564 6469 6e67 7329 0a2d 2055  _embeddings).- U
+000013d0: 7365 2045 534d 2d49 4631 2069 6e73 7465  se ESM-IF1 inste
+000013e0: 6164 206f 6620 416e 7469 466f 6c64 206d  ad of AntiFold m
+000013f0: 6f64 656c 2077 6569 6768 7473 2028 2d2d  odel weights (--
+00001400: 6573 6d5f 6966 315f 6d6f 6465 292c 2065  esm_if1_mode), e
+00001410: 6e61 626c 6573 2063 7573 746f 6d5f 6368  nables custom_ch
+00001420: 6169 6e5f 6d6f 6465 0a60 6060 0a0a 2323  ain_mode.```..##
+00001430: 2045 7861 6d70 6c65 206f 7574 7075 740a   Example output.
+00001440: 466f 7220 6578 616d 706c 6520 7765 6273  For example webs
+00001450: 6572 7665 7220 6f75 7470 7574 2c20 7365  erver output, se
+00001460: 653a 0a5b 6874 7470 733a 2f2f 6f70 6967  e:.[https://opig
+00001470: 2e73 7461 7473 2e6f 782e 6163 2e75 6b2f  .stats.ox.ac.uk/
+00001480: 7765 6261 7070 732f 616e 7469 666f 6c64  webapps/antifold
+00001490: 2f72 6573 756c 7473 2f65 7861 6d70 6c65  /results/example
+000014a0: 5f6a 6f62 2f5d 2868 7474 7073 3a2f 2f6f  _job/](https://o
+000014b0: 7069 672e 7374 6174 732e 6f78 2e61 632e  pig.stats.ox.ac.
+000014c0: 756b 2f77 6562 6170 7073 2f61 6e74 6966  uk/webapps/antif
+000014d0: 6f6c 642f 7265 7375 6c74 732f 6578 616d  old/results/exam
+000014e0: 706c 655f 6a6f 622f 290a 0a4f 7574 7075  ple_job/)..Outpu
+000014f0: 7420 4353 5620 7769 7468 2072 6573 6964  t CSV with resid
+00001500: 7565 206c 6f67 2d70 726f 6261 6269 6c69  ue log-probabili
+00001510: 7469 6573 3a20 5265 7369 6475 6520 7072  ties: Residue pr
+00001520: 6f62 6162 696c 6974 6965 733a 203c 6120  obabilities: <a 
+00001530: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00001540: 7468 7562 2e63 6f6d 2f6f 7870 6967 2f41  thub.com/oxpig/A
+00001550: 6e74 6946 6f6c 642f 626c 6f62 2f6d 6173  ntiFold/blob/mas
+00001560: 7465 722f 6f75 7470 7574 2f65 7861 6d70  ter/output/examp
+00001570: 6c65 5f70 6462 732f 3679 316c 5f69 6d67  le_pdbs/6y1l_img
+00001580: 742e 6373 7622 3e36 7931 6c5f 696d 6774  t.csv">6y1l_imgt
+00001590: 2e63 7376 3c2f 613e 0a2d 2070 6462 5f70  .csv</a>.- pdb_p
+000015a0: 6f73 202d 2050 4442 2072 6573 6964 7565  os - PDB residue
+000015b0: 206e 756d 6265 720a 2d20 7064 625f 6368   number.- pdb_ch
+000015c0: 6169 6e20 2d20 5044 4220 6368 6169 6e0a  ain - PDB chain.
+000015d0: 2d20 6161 5f6f 7269 6720 2d20 5044 4220  - aa_orig - PDB 
+000015e0: 7265 7369 6475 6520 2865 2e67 2e20 3131  residue (e.g. 11
+000015f0: 3229 0a2d 2061 615f 7072 6564 202d 2054  2).- aa_pred - T
+00001600: 6f70 2070 7265 6469 6374 6564 2072 6573  op predicted res
+00001610: 6964 7565 2062 7920 416e 7469 466f 6c64  idue by AntiFold
+00001620: 2028 692e 652e 2061 7267 6d61 7829 2066   (i.e. argmax) f
+00001630: 6f72 2074 6869 7320 706f 7369 7469 6f6e  or this position
+00001640: 0a2d 2070 6462 5f70 6f73 696e 7320 2d20  .- pdb_posins - 
+00001650: 5044 4220 7265 7369 6475 6520 6e75 6d62  PDB residue numb
+00001660: 6572 2077 6974 6820 696e 7365 7274 696f  er with insertio
+00001670: 6e20 636f 6465 2028 652e 672e 2031 3132  n code (e.g. 112
+00001680: 4129 0a2d 2070 6572 706c 6578 6974 7920  A).- perplexity 
+00001690: 2d20 496e 7665 7273 6520 666f 6c64 696e  - Inverse foldin
+000016a0: 6720 746f 6c65 7261 6e63 6520 2868 6967  g tolerance (hig
+000016b0: 6865 7220 6973 206d 6f72 6520 746f 6c65  her is more tole
+000016c0: 7261 6e74 2920 746f 206d 7574 6174 696f  rant) to mutatio
+000016d0: 6e73 2e20 5365 6520 7061 7065 7220 666f  ns. See paper fo
+000016e0: 7220 6d6f 7265 2064 6574 6169 6c73 2e0a  r more details..
+000016f0: 2d20 416d 696e 6f2d 6163 6964 7320 2d20  - Amino-acids - 
+00001700: 496e 7665 7273 6520 666f 6c64 696e 6720  Inverse folding 
+00001710: 7363 6f72 6573 2028 6c6f 672d 6c69 6b65  scores (log-like
+00001720: 6c69 686f 6f64 2920 666f 7220 7468 6520  lihood) for the 
+00001730: 6769 7665 6e20 706f 7369 7469 6f6e 0a60  given position.`
+00001740: 6060 6373 760a 7064 625f 706f 732c 7064  ``csv.pdb_pos,pd
+00001750: 625f 6368 6169 6e2c 6161 5f6f 7269 672c  b_chain,aa_orig,
+00001760: 6161 5f70 7265 642c 7064 625f 706f 7369  aa_pred,pdb_posi
+00001770: 6e73 2c70 6572 706c 6578 6974 792c 412c  ns,perplexity,A,
+00001780: 432c 442c 452c 462c 472c 482c 492c 4b2c  C,D,E,F,G,H,I,K,
+00001790: 4c2c 4d2c 4e2c 502c 512c 522c 532c 542c  L,M,N,P,Q,R,S,T,
+000017a0: 562c 572c 590a 322c 482c 562c 4d2c 322c  V,W,Y.2,H,V,M,2,
+000017b0: 312e 3634 3838 2c2d 342e 3939 3633 2c2d  1.6488,-4.9963,-
+000017c0: 362e 3631 3137 2c2d 362e 3331 3831 2c2d  6.6117,-6.3181,-
+000017d0: 362e 3332 3433 2c2d 362e 3735 3730 2c2d  6.3243,-6.7570,-
+000017e0: 342e 3235 3138 2c2d 362e 3735 3134 2c2d  4.2518,-6.7514,-
+000017f0: 352e 3235 3430 2c2d 362e 3830 3637 2c2d  5.2540,-6.8067,-
+00001800: 352e 3836 3139 2c2d 302e 3039 3034 2c2d  5.8619,-0.0904,-
+00001810: 362e 3534 3933 2c2d 342e 3836 3339 2c2d  6.5493,-4.8639,-
+00001820: 362e 3633 3136 2c2d 362e 3330 3834 2c2d  6.6316,-6.3084,-
+00001830: 352e 3139 3030 2c2d 352e 3039 3838 2c2d  5.1900,-5.0988,-
+00001840: 332e 3732 3935 2c2d 382e 3034 3830 2c2d  3.7295,-8.0480,-
+00001850: 372e 3332 3336 0a33 2c48 2c51 2c51 2c33  7.3236.3,H,Q,Q,3
+00001860: 2c31 2e33 3838 392c 2d31 302e 3532 3538  ,1.3889,-10.5258
+00001870: 2c2d 3132 2e38 3436 332c 2d38 2e34 3830  ,-12.8463,-8.480
+00001880: 302c 2d34 2e37 3633 302c 2d31 322e 3930  0,-4.7630,-12.90
+00001890: 3934 2c2d 3131 2e30 3932 342c 2d35 2e36  94,-11.0924,-5.6
+000018a0: 3133 362c 2d31 302e 3938 3730 2c2d 332e  136,-10.9870,-3.
+000018b0: 3131 3139 2c2d 382e 3131 3133 2c2d 392e  1119,-8.1113,-9.
+000018c0: 3433 3832 2c2d 362e 3232 3436 2c2d 3133  4382,-6.2246,-13
+000018d0: 2e33 3636 302c 2d30 2e30 3730 312c 2d34  .3660,-0.0701,-4
+000018e0: 2e39 3935 372c 2d31 302e 3033 3031 2c2d  .9957,-10.0301,-
+000018f0: 362e 3836 3138 2c2d 372e 3538 3130 2c2d  6.8618,-7.5810,-
+00001900: 3133 2e36 3732 312c 2d31 312e 3431 3537  13.6721,-11.4157
+00001910: 0a34 2c48 2c4c 2c4c 2c34 2c31 2e30 3032  .4,H,L,L,4,1.002
+00001920: 312c 2d31 332e 3335 3831 2c2d 3132 2e36  1,-13.3581,-12.6
+00001930: 3230 362c 2d31 372e 3534 3834 2c2d 3132  206,-17.5484,-12
+00001940: 2e34 3830 312c 2d39 2e38 3739 322c 2d31  .4801,-9.8792,-1
+00001950: 332e 3633 3832 2c2d 3134 2e38 3630 392c  3.6382,-14.8609,
+00001960: 2d31 332e 3933 3434 2c2d 3136 2e34 3038  -13.9344,-16.408
+00001970: 302c 2d30 2e30 3030 322c 2d39 2e32 3732  0,-0.0002,-9.272
+00001980: 372c 2d31 362e 3635 3332 2c2d 3134 2e30  7,-16.6532,-14.0
+00001990: 3437 362c 2d31 322e 3539 3433 2c2d 3135  476,-12.5943,-15
+000019a0: 2e34 3535 392c 2d31 362e 3931 3033 2c2d  .4559,-16.9103,-
+000019b0: 3137 2e30 3830 392c 2d31 302e 3536 3730  17.0809,-10.5670
+000019c0: 2c2d 3133 2e35 3333 342c 2d31 332e 3433  ,-13.5334,-13.43
+000019d0: 3234 0a2e 2e2e 0a60 6060 0a0a 4f75 7470  24.....```..Outp
+000019e0: 7574 2046 4153 5441 2066 696c 6520 7769  ut FASTA file wi
+000019f0: 7468 2073 616d 706c 6564 2073 6571 7565  th sampled seque
+00001a00: 6e63 6573 3a20 3c61 2068 7265 663d 2268  nces: <a href="h
+00001a10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001a20: 6d2f 6f78 7069 672f 416e 7469 466f 6c64  m/oxpig/AntiFold
+00001a30: 2f62 6c6f 622f 6d61 7374 6572 2f6f 7574  /blob/master/out
+00001a40: 7075 742f 6578 616d 706c 655f 7064 6273  put/example_pdbs
+00001a50: 2f36 7931 6c5f 696d 6774 2e66 6173 7461  /6y1l_imgt.fasta
+00001a60: 223e 3679 316c 5f69 6d67 742e 6661 7374  ">6y1l_imgt.fast
+00001a70: 613c 2f61 3e0a 2d20 543a 2054 656d 7065  a</a>.- T: Tempe
+00001a80: 7261 7475 7265 2075 7365 6420 666f 7220  rature used for 
+00001a90: 6465 7369 676e 0a2d 2073 636f 7265 3a20  design.- score: 
+00001aa0: 6176 6572 6167 6520 6c6f 672d 6f64 6473  average log-odds
+00001ab0: 206f 6620 7265 7369 6475 6573 2069 6e20   of residues in 
+00001ac0: 7468 6520 7361 6d70 6c65 6420 7265 6769  the sampled regi
+00001ad0: 6f6e 0a2d 2067 6c6f 6261 6c5f 7363 6f72  on.- global_scor
+00001ae0: 653a 2061 7665 7261 6765 206c 6f67 2d6f  e: average log-o
+00001af0: 6464 7320 6f66 2061 6c6c 2072 6573 6964  dds of all resid
+00001b00: 7565 7320 2849 4d47 5420 706f 7369 7469  ues (IMGT positi
+00001b10: 6f6e 7320 312d 3132 3829 0a2d 2072 6567  ons 1-128).- reg
+00001b20: 696f 6e73 3a20 7265 6769 6f6e 7320 7365  ions: regions se
+00001b30: 6c65 6374 6564 2066 6f72 2064 6573 6967  lected for desig
+00001b40: 6e0a 2d20 7365 715f 7265 636f 7665 7279  n.- seq_recovery
+00001b50: 3a20 2320 6d75 7461 7469 6f6e 7320 2f20  : # mutations / 
+00001b60: 746f 7461 6c20 7365 7175 656e 6365 206c  total sequence l
+00001b70: 656e 6774 680a 2d20 6d75 7461 7469 6f6e  ength.- mutation
+00001b80: 733a 2023 206d 7574 6174 696f 6e73 2066  s: # mutations f
+00001b90: 726f 6d20 6f72 6967 696e 616c 2050 4442  rom original PDB
+00001ba0: 2073 6571 7565 6e63 650a 6060 6066 6173   sequence.```fas
+00001bb0: 7461 0a3e 3679 316c 5f69 6d67 7420 2c20  ta.>6y1l_imgt , 
+00001bc0: 7363 6f72 653d 302e 3239 3334 2c20 676c  score=0.2934, gl
+00001bd0: 6f62 616c 5f73 636f 7265 3d30 2e32 3933  obal_score=0.293
+00001be0: 342c 2072 6567 696f 6e73 3d5b 2743 4452  4, regions=['CDR
+00001bf0: 3127 2c20 2743 4452 3227 2c20 2743 4452  1', 'CDR2', 'CDR
+00001c00: 4833 275d 2c20 6d6f 6465 6c5f 6e61 6d65  H3'], model_name
+00001c10: 3d41 6e74 6946 6f6c 642c 2073 6565 643d  =AntiFold, seed=
+00001c20: 3432 0a56 514c 5145 5347 5047 4c56 4b50  42.VQLQESGPGLVKP
+00001c30: 5345 544c 534c 5443 4156 5347 5953 4953  SETLSLTCAVSGYSIS
+00001c40: 5347 5959 5747 5749 5251 5050 474b 474c  SGYYWGWIRQPPGKGL
+00001c50: 4557 4947 5349 5948 5347 5354 5959 4e0a  EWIGSIYHSGSTYYN.
+00001c60: 5053 4c4b 5352 5654 4953 5644 5453 4b4e  PSLKSRVTISVDTSKN
+00001c70: 5146 534c 4b4c 5353 5654 4141 4454 4156  QFSLKLSSVTAADTAV
+00001c80: 5959 4341 474c 5451 5353 484e 4441 4e57  YYCAGLTQSSHNDANW
+00001c90: 4751 4754 4c56 5456 5353 2f56 0a4c 5451  GQGTLVTVSS/V.LTQ
+00001ca0: 5050 5356 5341 4150 4751 4b56 5449 5343  PPSVSAAPGQKVTISC
+00001cb0: 5347 5353 534e 4947 4e4e 5956 5357 5951  SGSSSNIGNNYVSWYQ
+00001cc0: 514c 5047 5441 504b 524c 4959 444e 4e4b  QLPGTAPKRLIYDNNK
+00001cd0: 5250 5347 4950 4452 460a 5347 534b 5347  RPSGIPDRF.SGSKSG
+00001ce0: 5453 4154 4c47 4954 474c 5154 4744 4541  TSATLGITGLQTGDEA
+00001cf0: 4459 5943 4754 5744 5353 4c4e 5056 4647  DYYCGTWDSSLNPVFG
+00001d00: 4747 544b 4c45 494b 520a 3e20 543d 302e  GGTKLEIKR.> T=0.
+00001d10: 3230 2c20 7361 6d70 6c65 3d31 2c20 7363  20, sample=1, sc
+00001d20: 6f72 653d 302e 3339 3330 2c20 676c 6f62  ore=0.3930, glob
+00001d30: 616c 5f73 636f 7265 3d30 2e31 3836 392c  al_score=0.1869,
+00001d40: 2073 6571 5f72 6563 6f76 6572 793d 302e   seq_recovery=0.
+00001d50: 3839 3833 2c20 6d75 7461 7469 6f6e 733d  8983, mutations=
+00001d60: 3132 0a56 514c 5145 5347 5047 4c56 4b50  12.VQLQESGPGLVKP
+00001d70: 5345 544c 534c 5443 4156 5347 4153 4954  SETLSLTCAVSGASIT
+00001d80: 5353 5959 5747 5749 5251 5050 474b 474c  SSYYWGWIRQPPGKGL
+00001d90: 4557 4947 5349 5959 5347 5354 5959 4e0a  EWIGSIYYSGSTYYN.
+00001da0: 5053 4c4b 5352 5654 4953 5644 5453 4b4e  PSLKSRVTISVDTSKN
+00001db0: 5146 534c 4b4c 5353 5654 4141 4454 4156  QFSLKLSSVTAADTAV
+00001dc0: 5959 4341 474c 5947 5350 5753 4e50 5957  YYCAGLYGSPWSNPYW
+00001dd0: 4751 4754 4c56 5456 5353 2f56 0a4c 5451  GQGTLVTVSS/V.LTQ
+00001de0: 5050 5356 5341 4150 4751 4b56 5449 5343  PPSVSAAPGQKVTISC
+00001df0: 5347 5353 534e 4947 4e4e 5956 5357 5951  SGSSSNIGNNYVSWYQ
+00001e00: 514c 5047 5441 504b 524c 4959 444e 4e4b  QLPGTAPKRLIYDNNK
+00001e10: 5250 5347 4950 4452 460a 5347 534b 5347  RPSGIPDRF.SGSKSG
+00001e20: 5453 4154 4c47 4954 474c 5154 4744 4541  TSATLGITGLQTGDEA
+00001e30: 4459 5943 4754 5744 5353 4c4e 5056 4647  DYYCGTWDSSLNPVFG
+00001e40: 4747 544b 4c45 494b 520a 2e2e 2e0a 6060  GGTKLEIKR.....``
+00001e50: 600a 0a23 2320 5573 6167 650a 6060 6062  `..## Usage.```b
+00001e60: 6173 680a 7573 6167 653a 200a 2020 2020  ash.usage: .    
+00001e70: 2320 5072 6564 6963 7420 6f6e 2065 7861  # Predict on exa
+00001e80: 6d70 6c65 2050 4442 7320 696e 2066 6f6c  mple PDBs in fol
+00001e90: 6465 720a 7079 7468 6f6e 2061 6e74 6966  der.python antif
+00001ea0: 6f6c 642f 6d61 696e 2e70 7920 5c0a 2020  old/main.py \.  
+00001eb0: 2020 2d2d 7064 625f 6669 6c65 2064 6174    --pdb_file dat
+00001ec0: 612f 616e 7469 626f 6479 5f61 6e74 6967  a/antibody_antig
+00001ed0: 656e 2f33 6866 6d2e 7064 6220 5c0a 2020  en/3hfm.pdb \.  
+00001ee0: 2020 2d2d 6865 6176 795f 6368 6169 6e20    --heavy_chain 
+00001ef0: 4820 5c0a 2020 2020 2d2d 6c69 6768 745f  H \.    --light_
+00001f00: 6368 6169 6e20 4c20 5c0a 2020 2020 2d2d  chain L \.    --
+00001f10: 616e 7469 6765 6e5f 6368 6169 6e20 5920  antigen_chain Y 
+00001f20: 2320 4f70 7469 6f6e 616c 0a0a 5072 6564  # Optional..Pred
+00001f30: 6963 7420 696e 7665 7273 6520 666f 6c64  ict inverse fold
+00001f40: 696e 6720 7072 6f62 6162 696c 6974 6965  ing probabilitie
+00001f50: 7320 666f 7220 616e 7469 626f 6479 2076  s for antibody v
+00001f60: 6172 6961 626c 6520 646f 6d61 696e 2c20  ariable domain, 
+00001f70: 616e 6420 7361 6d70 6c65 2073 6571 7565  and sample seque
+00001f80: 6e63 6573 2077 6974 6820 6d61 696e 7461  nces with mainta
+00001f90: 696e 6564 2066 6f6c 642e 0a50 4442 2073  ined fold..PDB s
+00001fa0: 7472 7563 7475 7265 7320 7368 6f75 6c64  tructures should
+00001fb0: 2062 6520 494d 4754 2d6e 756d 6265 7265   be IMGT-numbere
+00001fc0: 642c 2070 6169 7265 6420 6865 6176 7920  d, paired heavy 
+00001fd0: 616e 6420 6c69 6768 7420 6368 6169 6e20  and light chain 
+00001fe0: 7661 7269 6162 6c65 2064 6f6d 6169 6e73  variable domains
+00001ff0: 2028 706f 7369 7469 6f6e 7320 312d 3132   (positions 1-12
+00002000: 3829 2e0a 0a46 6f72 2049 4d47 5420 6e75  8)...For IMGT nu
+00002010: 6d62 6572 696e 6720 5044 4273 2075 7365  mbering PDBs use
+00002020: 2053 4162 4461 6220 6f72 2068 7474 7073   SAbDab or https
+00002030: 3a2f 2f6f 7069 672e 7374 6174 732e 6f78  ://opig.stats.ox
+00002040: 2e61 632e 756b 2f77 6562 6170 7073 2f73  .ac.uk/webapps/s
+00002050: 6162 6461 622d 7361 6270 7265 642f 7361  abdab-sabpred/sa
+00002060: 6270 7265 642f 616e 6172 6369 2f0a 0a6f  bpred/anarci/..o
+00002070: 7074 696f 6e73 3a0a 2020 2d68 2c20 2d2d  ptions:.  -h, --
+00002080: 6865 6c70 2020 2020 2020 2020 2020 2020  help            
+00002090: 7368 6f77 2074 6869 7320 6865 6c70 206d  show this help m
+000020a0: 6573 7361 6765 2061 6e64 2065 7869 740a  essage and exit.
+000020b0: 2020 2d2d 7064 625f 6669 6c65 2050 4442    --pdb_file PDB
+000020c0: 5f46 494c 4520 2020 496e 7075 7420 5044  _FILE   Input PD
+000020d0: 4220 6669 6c65 2028 666f 7220 7369 6e67  B file (for sing
+000020e0: 6c65 2050 4442 2070 7265 6469 6374 696f  le PDB predictio
+000020f0: 6e73 290a 2020 2d2d 6865 6176 795f 6368  ns).  --heavy_ch
+00002100: 6169 6e20 4845 4156 595f 4348 4149 4e0a  ain HEAVY_CHAIN.
+00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002120: 2020 2020 2020 2020 4162 2068 6561 7679          Ab heavy
+00002130: 2063 6861 696e 2028 666f 7220 7369 6e67   chain (for sing
+00002140: 6c65 2050 4442 2070 7265 6469 6374 696f  le PDB predictio
+00002150: 6e73 290a 2020 2d2d 6c69 6768 745f 6368  ns).  --light_ch
+00002160: 6169 6e20 4c49 4748 545f 4348 4149 4e0a  ain LIGHT_CHAIN.
+00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002180: 2020 2020 2020 2020 4162 206c 6967 6874          Ab light
+00002190: 2063 6861 696e 2028 666f 7220 7369 6e67   chain (for sing
+000021a0: 6c65 2050 4442 2070 7265 6469 6374 696f  le PDB predictio
+000021b0: 6e73 290a 2020 2d2d 616e 7469 6765 6e5f  ns).  --antigen_
+000021c0: 6368 6169 6e20 414e 5449 4745 4e5f 4348  chain ANTIGEN_CH
+000021d0: 4149 4e0a 2020 2020 2020 2020 2020 2020  AIN.            
+000021e0: 2020 2020 2020 2020 2020 2020 416e 7469              Anti
+000021f0: 6765 6e20 6368 6169 6e20 286f 7074 696f  gen chain (optio
+00002200: 6e61 6c29 0a20 202d 2d70 6462 735f 6373  nal).  --pdbs_cs
+00002210: 7620 5044 4253 5f43 5356 2020 2049 6e70  v PDBS_CSV   Inp
+00002220: 7574 2043 5356 2066 696c 6520 7769 7468  ut CSV file with
+00002230: 2050 4442 206e 616d 6573 2061 6e64 2048   PDB names and H
+00002240: 2f4c 2063 6861 696e 7320 286d 756c 7469  /L chains (multi
+00002250: 2d50 4442 2070 7265 6469 6374 696f 6e73  -PDB predictions
+00002260: 290a 2020 2d2d 7064 625f 6469 7220 5044  ).  --pdb_dir PD
+00002270: 425f 4449 5220 2020 2020 4469 7265 6374  B_DIR     Direct
+00002280: 6f72 7920 7769 7468 2069 6e70 7574 2050  ory with input P
+00002290: 4442 2066 696c 6573 2028 6d75 6c74 692d  DB files (multi-
+000022a0: 5044 4220 7072 6564 6963 7469 6f6e 7329  PDB predictions)
+000022b0: 0a20 202d 2d6f 7574 5f64 6972 204f 5554  .  --out_dir OUT
+000022c0: 5f44 4952 2020 2020 204f 7574 7075 7420  _DIR     Output 
+000022d0: 6469 7265 6374 6f72 790a 2020 2d2d 7265  directory.  --re
+000022e0: 6769 6f6e 7320 5245 4749 4f4e 5320 2020  gions REGIONS   
+000022f0: 2020 5370 6163 652d 7365 7061 7261 7465    Space-separate
+00002300: 6420 7265 6769 6f6e 7320 746f 206d 7574  d regions to mut
+00002310: 6174 652e 2044 6566 6175 6c74 2027 4344  ate. Default 'CD
+00002320: 5231 2043 4452 3220 4344 5233 4827 0a20  R1 CDR2 CDR3H'. 
+00002330: 202d 2d6e 756d 5f73 6571 5f70 6572 5f74   --num_seq_per_t
+00002340: 6172 6765 7420 4e55 4d5f 5345 515f 5045  arget NUM_SEQ_PE
+00002350: 525f 5441 5247 4554 0a20 2020 2020 2020  R_TARGET.       
+00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002370: 204e 756d 6265 7220 6f66 2073 6571 7565   Number of seque
+00002380: 6e63 6573 2074 6f20 7361 6d70 6c65 2066  nces to sample f
+00002390: 726f 6d20 6561 6368 2061 6e74 6962 6f64  rom each antibod
+000023a0: 7920 5044 4220 2864 6566 6175 6c74 2030  y PDB (default 0
+000023b0: 290a 2020 2d2d 7361 6d70 6c69 6e67 5f74  ).  --sampling_t
+000023c0: 656d 7020 5341 4d50 4c49 4e47 5f54 454d  emp SAMPLING_TEM
+000023d0: 500a 2020 2020 2020 2020 2020 2020 2020  P.              
+000023e0: 2020 2020 2020 2020 2020 4120 7374 7269            A stri
+000023f0: 6e67 206f 6620 7465 6d70 6572 6174 7572  ng of temperatur
+00002400: 6573 2065 2e67 2e20 2730 2e32 3020 302e  es e.g. '0.20 0.
+00002410: 3235 2030 2e35 3027 2028 6465 6661 756c  25 0.50' (defaul
+00002420: 7420 302e 3230 292e 2053 616d 706c 696e  t 0.20). Samplin
+00002430: 6720 7465 6d70 6572 6174 7572 6520 666f  g temperature fo
+00002440: 7220 616d 696e 6f20 6163 6964 732e 2053  r amino acids. S
+00002450: 7567 6765 7374 6564 2076 616c 7565 7320  uggested values 
+00002460: 302e 3130 2c20 302e 3135 2c20 302e 3230  0.10, 0.15, 0.20
+00002470: 2c20 302e 3235 2c20 302e 3330 2e20 4869  , 0.25, 0.30. Hi
+00002480: 6768 6572 2076 616c 7565 7320 7769 6c6c  gher values will
+00002490: 206c 6561 6420 746f 206d 6f72 6520 6469   lead to more di
+000024a0: 7665 7273 6974 792e 0a20 202d 2d6c 696d  versity..  --lim
+000024b0: 6974 5f76 6172 6961 7469 6f6e 2020 2020  it_variation    
+000024c0: 204c 696d 6974 2076 6172 6961 7469 6f6e   Limit variation
+000024d0: 2074 6f20 6173 206d 616e 7920 6d75 7461   to as many muta
+000024e0: 7469 6f6e 7320 6173 2065 7870 6563 7465  tions as expecte
+000024f0: 6420 6672 6f6d 2074 656d 7065 7261 7475  d from temperatu
+00002500: 7265 2073 616d 706c 696e 670a 2020 2d2d  re sampling.  --
+00002510: 6578 7472 6163 745f 656d 6265 6464 696e  extract_embeddin
+00002520: 6773 2020 4578 7472 6163 7420 7065 722d  gs  Extract per-
+00002530: 7265 7369 6475 6520 656d 6265 6464 696e  residue embeddin
+00002540: 6773 2066 726f 6d20 416e 7469 466f 6c64  gs from AntiFold
+00002550: 202f 2045 534d 2d49 4631 0a20 202d 2d63   / ESM-IF1.  --c
+00002560: 7573 746f 6d5f 6368 6169 6e5f 6d6f 6465  ustom_chain_mode
+00002570: 2020 2052 756e 2061 6c6c 2073 7065 6369     Run all speci
+00002580: 6669 6564 2063 6861 696e 7320 2866 6f72  fied chains (for
+00002590: 2061 6e74 6962 6f64 792d 616e 7469 6765   antibody-antige
+000025a0: 6e20 636f 6d70 6c65 7865 7320 6f72 2061  n complexes or a
+000025b0: 6e79 2063 6f6d 6269 6e61 7469 6f6e 206f  ny combination o
+000025c0: 6620 6368 6169 6e73 290a 2020 2d2d 6578  f chains).  --ex
+000025d0: 636c 7564 655f 6865 6176 7920 2020 2020  clude_heavy     
+000025e0: 2020 4578 636c 7564 6520 6865 6176 7920    Exclude heavy 
+000025f0: 6368 6169 6e20 6672 6f6d 2073 616d 706c  chain from sampl
+00002600: 696e 670a 2020 2d2d 6578 636c 7564 655f  ing.  --exclude_
+00002610: 6c69 6768 7420 2020 2020 2020 4578 636c  light       Excl
+00002620: 7564 6520 6c69 6768 7420 6368 6169 6e20  ude light chain 
+00002630: 6672 6f6d 2073 616d 706c 696e 670a 2020  from sampling.  
+00002640: 2d2d 6261 7463 685f 7369 7a65 2042 4154  --batch_size BAT
+00002650: 4348 5f53 495a 450a 2020 2020 2020 2020  CH_SIZE.        
+00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002670: 4261 7463 682d 7369 7a65 2074 6f20 7573  Batch-size to us
+00002680: 650a 2020 2d2d 6e75 6d5f 7468 7265 6164  e.  --num_thread
+00002690: 7320 4e55 4d5f 5448 5245 4144 530a 2020  s NUM_THREADS.  
+000026a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026b0: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
+000026c0: 4350 5520 7468 7265 6164 7320 746f 2075  CPU threads to u
+000026d0: 7365 2066 6f72 2070 6172 616c 6c65 6c20  se for parallel 
+000026e0: 7072 6f63 6573 7369 6e67 2028 3020 3d20  processing (0 = 
+000026f0: 616c 6c20 6176 6169 6c61 626c 6529 0a20  all available). 
+00002700: 202d 2d73 6565 6420 5345 4544 2020 2020   --seed SEED    
+00002710: 2020 2020 2020 2053 6565 6420 666f 7220         Seed for 
+00002720: 7265 7072 6f64 7563 6962 696c 6974 790a  reproducibility.
+00002730: 2020 2d2d 6d6f 6465 6c5f 7061 7468 204d    --model_path M
+00002740: 4f44 454c 5f50 4154 480a 2020 2020 2020  ODEL_PATH.      
+00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002760: 2020 416c 7465 726e 6174 6976 6520 6d6f    Alternative mo
+00002770: 6465 6c20 7765 6967 6874 7320 2864 6566  del weights (def
+00002780: 6175 6c74 206d 6f64 656c 732f 6d6f 6465  ault models/mode
+00002790: 6c2e 7074 292e 2053 6565 202d 2d75 7365  l.pt). See --use
+000027a0: 5f65 736d 5f69 6631 5f77 6569 6768 7473  _esm_if1_weights
+000027b0: 2066 6c61 6720 746f 2075 7365 2045 534d   flag to use ESM
+000027c0: 2d49 4631 2077 6569 6768 7473 2069 6e73  -IF1 weights ins
+000027d0: 7465 6164 206f 6620 416e 7469 466f 6c64  tead of AntiFold
+000027e0: 0a20 202d 2d65 736d 5f69 6631 5f6d 6f64  .  --esm_if1_mod
+000027f0: 6520 2020 2020 2020 2055 7365 2045 534d  e        Use ESM
+00002800: 2d49 4631 2077 6569 6768 7473 2069 6e73  -IF1 weights ins
+00002810: 7465 6164 206f 6620 416e 7469 466f 6c64  tead of AntiFold
+00002820: 0a20 202d 2d76 6572 626f 7365 2056 4552  .  --verbose VER
+00002830: 424f 5345 2020 2020 2056 6572 626f 7365  BOSE     Verbose
+00002840: 2070 7269 6e74 696e 670a 6060 600a 0a23   printing.```..#
+00002850: 2320 494d 4754 2072 6567 696f 6e73 2064  # IMGT regions d
+00002860: 6963 740a 5573 6564 2074 6f20 7370 6563  ict.Used to spec
+00002870: 6966 7920 7768 6963 6820 7265 6769 6f6e  ify which region
+00002880: 7320 746f 206d 7574 6174 6520 696e 2061  s to mutate in a
+00002890: 6e20 494d 4754 206e 756d 6265 7265 6420  n IMGT numbered 
+000028a0: 5044 420a 2d20 494d 4754 206e 756d 6265  PDB.- IMGT numbe
+000028b0: 7265 6420 5044 4273 3a20 5b68 7474 7073  red PDBs: [https
+000028c0: 3a2f 2f6f 7069 672e 7374 6174 732e 6f78  ://opig.stats.ox
+000028d0: 2e61 632e 756b 2f77 6562 6170 7073 2f73  .ac.uk/webapps/s
+000028e0: 6162 6461 622d 7361 6270 7265 642f 7361  abdab-sabpred/sa
+000028f0: 6264 6162 5d28 6874 7470 733a 2f2f 6f70  bdab](https://op
+00002900: 6967 2e73 7461 7473 2e6f 782e 6163 2e75  ig.stats.ox.ac.u
+00002910: 6b2f 7765 6261 7070 732f 7361 6264 6162  k/webapps/sabdab
+00002920: 2d73 6162 7072 6564 2f73 6162 6461 6229  -sabpred/sabdab)
+00002930: 0a2d 2052 656e 756d 6265 7220 6578 6973  .- Renumber exis
+00002940: 7469 6e67 2050 4442 7320 7769 7468 2041  ting PDBs with A
+00002950: 4e41 5243 493a 205b 6874 7470 733a 2f2f  NARCI: [https://
+00002960: 6769 7468 7562 2e63 6f6d 2f6f 7870 6967  github.com/oxpig
+00002970: 2f41 4e41 5243 495d 2868 7474 7073 3a2f  /ANARCI](https:/
+00002980: 2f67 6974 6875 622e 636f 6d2f 6f78 7069  /github.com/oxpi
+00002990: 672f 414e 4152 4349 290a 2d20 5265 6164  g/ANARCI).- Read
+000029a0: 206d 6f72 653a 205b 6874 7470 733a 2f2f   more: [https://
+000029b0: 7777 772e 696d 6774 2e6f 7267 2f49 4d47  www.imgt.org/IMG
+000029c0: 5453 6369 656e 7469 6669 6343 6861 7274  TScientificChart
+000029d0: 2f4e 756d 6265 7269 6e67 2f49 4d47 5449  /Numbering/IMGTI
+000029e0: 4756 4c73 7570 6572 6661 6d69 6c79 2e68  GVLsuperfamily.h
+000029f0: 746d 6c5d 2868 7474 7073 3a2f 2f77 7777  tml](https://www
+00002a00: 2e69 6d67 742e 6f72 672f 494d 4754 5363  .imgt.org/IMGTSc
+00002a10: 6965 6e74 6966 6963 4368 6172 742f 4e75  ientificChart/Nu
+00002a20: 6d62 6572 696e 672f 494d 4754 4947 564c  mbering/IMGTIGVL
+00002a30: 7375 7065 7266 616d 696c 792e 6874 6d6c  superfamily.html
+00002a40: 290a 0a60 6060 7079 7468 6f6e 0a49 4d47  )..```python.IMG
+00002a50: 545f 6469 6374 203d 207b 0a20 2020 2022  T_dict = {.    "
+00002a60: 616c 6c22 3a20 7261 6e67 6528 312c 2031  all": range(1, 1
+00002a70: 3238 202b 2031 292c 0a20 2020 2022 616c  28 + 1),.    "al
+00002a80: 6c48 223a 2072 616e 6765 2831 2c20 3132  lH": range(1, 12
+00002a90: 3820 2b20 3129 2c0a 2020 2020 2261 6c6c  8 + 1),.    "all
+00002aa0: 4c22 3a20 7261 6e67 6528 312c 2031 3238  L": range(1, 128
+00002ab0: 202b 2031 292c 0a20 2020 2022 4657 4822   + 1),.    "FWH"
+00002ac0: 3a20 6c69 7374 2872 616e 6765 2831 2c20  : list(range(1, 
+00002ad0: 3236 202b 2031 2929 202b 206c 6973 7428  26 + 1)) + list(
+00002ae0: 7261 6e67 6528 3430 2c20 3535 202b 2031  range(40, 55 + 1
+00002af0: 2929 202b 206c 6973 7428 7261 6e67 6528  )) + list(range(
+00002b00: 3636 2c20 3130 3420 2b20 3129 292c 0a20  66, 104 + 1)),. 
+00002b10: 2020 2022 4657 4c22 3a20 6c69 7374 2872     "FWL": list(r
+00002b20: 616e 6765 2831 2c20 3236 202b 2031 2929  ange(1, 26 + 1))
+00002b30: 202b 206c 6973 7428 7261 6e67 6528 3430   + list(range(40
+00002b40: 2c20 3535 202b 2031 2929 202b 206c 6973  , 55 + 1)) + lis
+00002b50: 7428 7261 6e67 6528 3636 2c20 3130 3420  t(range(66, 104 
+00002b60: 2b20 3129 292c 0a20 2020 2022 4344 5248  + 1)),.    "CDRH
+00002b70: 223a 206c 6973 7428 7261 6e67 6528 3237  ": list(range(27
+00002b80: 2c20 3339 2929 202b 206c 6973 7428 7261  , 39)) + list(ra
+00002b90: 6e67 6528 3536 2c20 3635 202b 2031 2929  nge(56, 65 + 1))
+00002ba0: 202b 206c 6973 7428 7261 6e67 6528 3130   + list(range(10
+00002bb0: 352c 2031 3137 202b 2031 2929 2c0a 2020  5, 117 + 1)),.  
+00002bc0: 2020 2243 4452 4c22 3a20 6c69 7374 2872    "CDRL": list(r
+00002bd0: 616e 6765 2832 372c 2033 3929 2920 2b20  ange(27, 39)) + 
+00002be0: 6c69 7374 2872 616e 6765 2835 362c 2036  list(range(56, 6
+00002bf0: 3520 2b20 3129 2920 2b20 6c69 7374 2872  5 + 1)) + list(r
+00002c00: 616e 6765 2831 3035 2c20 3131 3720 2b20  ange(105, 117 + 
+00002c10: 3129 292c 0a20 2020 2022 4657 3122 3a20  1)),.    "FW1": 
+00002c20: 7261 6e67 6528 312c 2032 3620 2b20 3129  range(1, 26 + 1)
+00002c30: 2c0a 2020 2020 2246 5748 3122 3a20 7261  ,.    "FWH1": ra
+00002c40: 6e67 6528 312c 2032 3620 2b20 3129 2c0a  nge(1, 26 + 1),.
+00002c50: 2020 2020 2246 574c 3122 3a20 7261 6e67      "FWL1": rang
+00002c60: 6528 312c 2032 3620 2b20 3129 2c0a 2020  e(1, 26 + 1),.  
+00002c70: 2020 2243 4452 3122 3a20 7261 6e67 6528    "CDR1": range(
+00002c80: 3237 2c20 3339 292c 0a20 2020 2022 4344  27, 39),.    "CD
+00002c90: 5248 3122 3a20 7261 6e67 6528 3237 2c20  RH1": range(27, 
+00002ca0: 3339 292c 0a20 2020 2022 4344 524c 3122  39),.    "CDRL1"
+00002cb0: 3a20 7261 6e67 6528 3237 2c20 3339 292c  : range(27, 39),
+00002cc0: 0a20 2020 2022 4657 3222 3a20 7261 6e67  .    "FW2": rang
+00002cd0: 6528 3430 2c20 3535 202b 2031 292c 0a20  e(40, 55 + 1),. 
+00002ce0: 2020 2022 4657 4832 223a 2072 616e 6765     "FWH2": range
+00002cf0: 2834 302c 2035 3520 2b20 3129 2c0a 2020  (40, 55 + 1),.  
+00002d00: 2020 2246 574c 3222 3a20 7261 6e67 6528    "FWL2": range(
+00002d10: 3430 2c20 3535 202b 2031 292c 0a20 2020  40, 55 + 1),.   
+00002d20: 2022 4344 5232 223a 2072 616e 6765 2835   "CDR2": range(5
+00002d30: 362c 2036 3520 2b20 3129 2c0a 2020 2020  6, 65 + 1),.    
+00002d40: 2243 4452 4832 223a 2072 616e 6765 2835  "CDRH2": range(5
+00002d50: 362c 2036 3520 2b20 3129 2c0a 2020 2020  6, 65 + 1),.    
+00002d60: 2243 4452 4c32 223a 2072 616e 6765 2835  "CDRL2": range(5
+00002d70: 362c 2036 3520 2b20 3129 2c0a 2020 2020  6, 65 + 1),.    
+00002d80: 2246 5733 223a 2072 616e 6765 2836 362c  "FW3": range(66,
+00002d90: 2031 3034 202b 2031 292c 0a20 2020 2022   104 + 1),.    "
+00002da0: 4657 4833 223a 2072 616e 6765 2836 362c  FWH3": range(66,
+00002db0: 2031 3034 202b 2031 292c 0a20 2020 2022   104 + 1),.    "
+00002dc0: 4657 4c33 223a 2072 616e 6765 2836 362c  FWL3": range(66,
+00002dd0: 2031 3034 202b 2031 292c 0a20 2020 2022   104 + 1),.    "
+00002de0: 4344 5233 223a 2072 616e 6765 2831 3035  CDR3": range(105
+00002df0: 2c20 3131 3720 2b20 3129 2c0a 2020 2020  , 117 + 1),.    
+00002e00: 2243 4452 4833 223a 2072 616e 6765 2831  "CDRH3": range(1
+00002e10: 3035 2c20 3131 3720 2b20 3129 2c0a 2020  05, 117 + 1),.  
+00002e20: 2020 2243 4452 4c33 223a 2072 616e 6765    "CDRL3": range
+00002e30: 2831 3035 2c20 3131 3720 2b20 3129 2c0a  (105, 117 + 1),.
+00002e40: 2020 2020 2246 5734 223a 2072 616e 6765      "FW4": range
+00002e50: 2831 3138 2c20 3132 3820 2b20 3129 2c0a  (118, 128 + 1),.
+00002e60: 2020 2020 2246 5748 3422 3a20 7261 6e67      "FWH4": rang
+00002e70: 6528 3131 382c 2031 3238 202b 2031 292c  e(118, 128 + 1),
+00002e80: 0a20 2020 2022 4657 4c34 223a 2072 616e  .    "FWL4": ran
+00002e90: 6765 2831 3138 2c20 3132 3820 2b20 3129  ge(118, 128 + 1)
+00002ea0: 2c0a 7d0a 6060 600a                      ,.}.```.
```

### Comparing `antifold-0.2.0/antifold/antiscripts.py` & `antifold-0.2.1/antifold/antiscripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import glob
 import logging
 import os
 import sys
 import warnings
+import urllib.request
 from pathlib import Path
 
 ROOT_PATH = Path(os.path.dirname(__file__)).parent
 sys.path.insert(0, ROOT_PATH)
 
 import re
 from collections import OrderedDict
@@ -127,18 +128,30 @@
 
     # Load pretrained weights
     model.load_state_dict(pretrained_dict)
 
     return model
 
 
-def load_IF1_model(checkpoint_path: str = ""):
+def load_model(checkpoint_path: str = ""):
     """Load raw/FT IF1 model"""
 
-    if not os.path.exists(checkpoint_path) and not checkpoint_path == "ESM-IF1":
+    # Check that AntiFold weights are downloaded
+    root_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+    model_path = f"{root_dir}/models/model.pt"
+
+    if not os.path.exists(model_path):
+        log.warning(
+            f"Downloading AntiFold model weights to models/model.pt from https://opig.stats.ox.ac.uk/data/downloads/AntiFold/models/model.pt"
+        )
+        url = "https://opig.stats.ox.ac.uk/data/downloads/AntiFold/models/model.pt"
+        filename = "models/model.pt"
+        urllib.request.urlretrieve(url, filename)
+
+    if not os.path.exists(model_path) and not checkpoint_path == "ESM-IF1":
         raise Exception(
             f"Unable to find model weights. File does not exist: {checkpoint_path}"
         )
 
     # Download IF1 weights
     if checkpoint_path == "ESM-IF1":
         log.info(
@@ -148,15 +161,15 @@
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             model, _ = antifold.esm.pretrained.esm_if1_gvp4_t16_142M_UR50()
 
     # Load AntiFold weights locally
     else:
         model, _ = antifold.esm.pretrained._load_IF1_local()
-        model = load_IF1_checkpoint(model, checkpoint_path)
+        model = load_IF1_checkpoint(model, model_path)
 
     # Evaluation mode when predicting
     model = model.eval()
 
     # Send to CPU/GPU
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     _ = model.to(device)
@@ -422,15 +435,15 @@
     pdbs_csv_or_dataframe,
     pdb_dir,
     out_dir=False,
     batch_size=1,
     extract_embeddings=False,
     custom_chain_mode=False,
     num_threads=0,
-    save_flag=True,
+    save_flag=False,
     float_format="%.4f",
     seed=42,
 ):
     """Predict PDBs from a CSV file"""
 
     # if save_flag:
     #    log.info(f"Saving prediction CSVs to {out_dir}")
```

### Comparing `antifold-0.2.0/antifold/esm/data.py` & `antifold-0.2.1/antifold/esm/data.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/esm/inverse_folding/features.py` & `antifold-0.2.1/antifold/esm/inverse_folding/features.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/esm/inverse_folding/gvp_encoder.py` & `antifold-0.2.1/antifold/esm/inverse_folding/gvp_encoder.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/esm/inverse_folding/gvp_modules.py` & `antifold-0.2.1/antifold/esm/inverse_folding/gvp_modules.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/esm/inverse_folding/gvp_transformer.py` & `antifold-0.2.1/antifold/esm/inverse_folding/gvp_transformer.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/esm/inverse_folding/gvp_transformer_encoder.py` & `antifold-0.2.1/antifold/esm/inverse_folding/gvp_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/esm/inverse_folding/gvp_utils.py` & `antifold-0.2.1/antifold/esm/inverse_folding/gvp_utils.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/esm/inverse_folding/multichain_util.py` & `antifold-0.2.1/antifold/esm/inverse_folding/multichain_util.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/esm/inverse_folding/transformer_decoder.py` & `antifold-0.2.1/antifold/esm/inverse_folding/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/esm/inverse_folding/transformer_layer.py` & `antifold-0.2.1/antifold/esm/inverse_folding/transformer_layer.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/esm/inverse_folding/util.py` & `antifold-0.2.1/antifold/esm/inverse_folding/util.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/esm/modules.py` & `antifold-0.2.1/antifold/esm/modules.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/esm/multihead_attention.py` & `antifold-0.2.1/antifold/esm/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/esm/pretrained.py` & `antifold-0.2.1/antifold/esm/pretrained.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/esm/rotary_embedding.py` & `antifold-0.2.1/antifold/esm/rotary_embedding.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/esm_multichain_util_custom.py` & `antifold-0.2.1/antifold/esm_multichain_util_custom.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/esm_util_custom.py` & `antifold-0.2.1/antifold/esm_util_custom.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/if1_dataset.py` & `antifold-0.2.1/antifold/if1_dataset.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.0/antifold/main.py` & `antifold-0.2.1/antifold/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 
 from argparse import ArgumentParser, RawTextHelpFormatter
 
 import pandas as pd
 
 from antifold.antiscripts import (df_logits_to_logprobs,
                                   extract_chains_biotite, generate_pdbs_csv,
-                                  get_pdbs_logits, load_IF1_model,
-                                  sample_from_df_logits, write_fasta_to_dir)
+                                  get_pdbs_logits, load_model,
+                                  sample_from_df_logits, write_fasta_to_dir,
+                                  visualize_mutations)
 
 log = logging.getLogger(__name__)
 
 
 def cmdline_args():
     # Make parser object
     usage = f"""
@@ -409,18 +410,15 @@
     if args.num_seq_per_target >= 1:
         log.info(
             f"Will sample {args.num_seq_per_target} sequences from {len(pdbs_csv.values)} PDBs at temperature(s) {args.sampling_temp} and regions: {regions_to_mutate}"
         )
 
     # Load AntiFold or ESM-IF1 model
     # Infer model from file path
-    if not args.model_path:
-        root_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-        args.model_path = f"{root_dir}/models/model.pt"
-    model = load_IF1_model(args.model_path)
+    model = load_model()
 
     # Get dict with PDBs, sampled sequences and logits / log_odds DataFrame
     pdb_output_dict = sample_pdbs(
         model=model,
         pdbs_csv_or_dataframe=pdbs_csv,
         pdb_dir=pdb_dir,
         regions_to_mutate=regions_to_mutate,
```

### Comparing `antifold-0.2.0/antifold.egg-info/SOURCES.txt` & `antifold-0.2.1/antifold.egg-info/SOURCES.txt`

 * *Files identical despite different names*

