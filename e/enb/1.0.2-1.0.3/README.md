# Comparing `tmp/enb-1.0.2.tar.gz` & `tmp/enb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enb-1.0.2.tar", last modified: Tue Feb  6 16:28:20 2024, max compression
+gzip compressed data, was "enb-1.0.3.tar", last modified: Tue May 21 15:15:34 2024, max compression
```

## Comparing `enb-1.0.2.tar` & `enb-1.0.3.tar`

### file list

```diff
@@ -1,367 +1,370 @@
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.085866 enb-1.0.2/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1405 2021-10-06 09:19:32.000000 enb-1.0.2/LICENSE.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    13887 2024-02-06 16:27:53.000000 enb-1.0.2/MANIFEST.in
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     3536 2024-02-06 16:28:20.085866 enb-1.0.2/PKG-INFO
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2215 2022-12-02 09:46:00.000000 enb-1.0.2/README.md
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.061866 enb-1.0.2/enb/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     5684 2024-02-06 16:27:53.000000 enb-1.0.2/enb/__init__.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)    11909 2024-02-06 16:27:53.000000 enb-1.0.2/enb/__main__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   185172 2024-02-06 16:27:53.000000 enb-1.0.2/enb/aanalysis.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    94029 2024-02-06 16:27:53.000000 enb-1.0.2/enb/atable.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.061866 enb-1.0.2/enb/config/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     4692 2024-02-06 16:27:53.000000 enb-1.0.2/enb/config/__init__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     9156 2024-02-06 16:27:53.000000 enb-1.0.2/enb/config/aini.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    19042 2024-02-06 16:27:53.000000 enb-1.0.2/enb/config/aoptions.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1381 2024-02-06 16:27:45.000000 enb-1.0.2/enb/config/contrib_sha256.csv
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    11317 2024-02-06 16:27:53.000000 enb-1.0.2/enb/config/enb.ini
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.061866 enb-1.0.2/enb/config/mpl_styles/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      215 2022-05-23 13:58:55.000000 enb-1.0.2/enb/config/mpl_styles/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      226 2022-05-23 13:58:55.000000 enb-1.0.2/enb/config/mpl_styles/single_column
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      193 2022-05-23 13:58:55.000000 enb-1.0.2/enb/config/mpl_styles/slides
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      232 2022-05-23 13:58:55.000000 enb-1.0.2/enb/config/mpl_styles/two_columns
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    23890 2024-02-06 16:27:53.000000 enb-1.0.2/enb/config/singleton_cli.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    19298 2024-02-06 16:27:53.000000 enb-1.0.2/enb/experiment.py
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    12039 2023-12-07 15:45:59.000000 enb-1.0.2/enb/fits.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    73954 2024-02-06 16:27:53.000000 enb-1.0.2/enb/icompression.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    41042 2024-02-06 16:27:53.000000 enb-1.0.2/enb/isets.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      467 2024-01-01 12:38:20.000000 enb-1.0.2/enb/jpg.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    24405 2024-02-06 16:27:53.000000 enb-1.0.2/enb/log.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     9459 2024-02-06 16:27:53.000000 enb-1.0.2/enb/misc.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    10904 2024-02-06 16:27:53.000000 enb-1.0.2/enb/parallel.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    27513 2024-02-06 16:27:53.000000 enb-1.0.2/enb/parallel_ray.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     8096 2024-01-01 12:38:20.000000 enb-1.0.2/enb/pgm.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    29734 2024-01-01 12:38:20.000000 enb-1.0.2/enb/plotdata.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.061866 enb-1.0.2/enb/plugins/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      904 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/__init__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    17872 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/installable.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     8126 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/plugin.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.061866 enb-1.0.2/enb/plugins/plugin_ac/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      356 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/plugin_ac/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      540 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/plugin_ac/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1518 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/plugin_ac/arithmetic_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.061866 enb-1.0.2/enb/plugins/plugin_bwt/
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    35147 2023-02-15 10:23:26.000000 enb-1.0.2/enb/plugins/plugin_bwt/COPYING
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     7639 2023-02-15 10:23:26.000000 enb-1.0.2/enb/plugins/plugin_bwt/COPYING.LESSER
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      977 2023-02-15 10:23:26.000000 enb-1.0.2/enb/plugins/plugin_bwt/Makefile
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     4662 2023-02-15 10:23:26.000000 enb-1.0.2/enb/plugins/plugin_bwt/README
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      571 2023-02-15 10:28:33.000000 enb-1.0.2/enb/plugins/plugin_bwt/__plugin__.py
--rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)     1249 2023-02-15 10:31:51.000000 enb-1.0.2/enb/plugins/plugin_bwt/bwt_codec.py
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    22418 2023-02-15 10:23:26.000000 enb-1.0.2/enb/plugins/plugin_bwt/bwxform.c
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2488 2023-02-15 10:23:26.000000 enb-1.0.2/enb/plugins/plugin_bwt/bwxform.h
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.065866 enb-1.0.2/enb/plugins/plugin_bwt/optlist/
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)       11 2023-09-15 14:24:43.000000 enb-1.0.2/enb/plugins/plugin_bwt/optlist/.bzrignore
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)       63 2023-09-15 14:24:43.000000 enb-1.0.2/enb/plugins/plugin_bwt/optlist/.gitignore
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    35147 2023-09-15 14:24:43.000000 enb-1.0.2/enb/plugins/plugin_bwt/optlist/COPYING
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     7639 2023-09-15 14:24:43.000000 enb-1.0.2/enb/plugins/plugin_bwt/optlist/COPYING.LESSER
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1080 2023-09-15 14:24:43.000000 enb-1.0.2/enb/plugins/plugin_bwt/optlist/Makefile
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     3212 2023-09-15 14:24:43.000000 enb-1.0.2/enb/plugins/plugin_bwt/optlist/README
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    10880 2023-09-15 14:24:43.000000 enb-1.0.2/enb/plugins/plugin_bwt/optlist/optlist.c
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     3199 2023-09-15 14:24:43.000000 enb-1.0.2/enb/plugins/plugin_bwt/optlist/optlist.h
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     3916 2023-09-15 14:24:43.000000 enb-1.0.2/enb/plugins/plugin_bwt/optlist/sample.c
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     4135 2023-09-15 14:24:43.000000 enb-1.0.2/enb/plugins/plugin_bwt/optlist/sample.cpp
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     6961 2023-02-15 10:23:26.000000 enb-1.0.2/enb/plugins/plugin_bwt/sample.c
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.065866 enb-1.0.2/enb/plugins/plugin_ccsds122/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      131 2021-07-14 12:07:01.000000 enb-1.0.2/enb/plugins/plugin_ccsds122/.gitignore
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       75 2021-07-14 12:07:01.000000 enb-1.0.2/enb/plugins/plugin_ccsds122/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)        0 2023-06-06 14:03:27.000000 enb-1.0.2/enb/plugins/plugin_ccsds122/__init__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      350 2022-12-02 09:46:00.000000 enb-1.0.2/enb/plugins/plugin_ccsds122/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     4508 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_ccsds122/ccsds122_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.065866 enb-1.0.2/enb/plugins/plugin_ccsds124/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      114 2021-11-29 16:18:18.000000 enb-1.0.2/enb/plugins/plugin_ccsds124/.gitignore
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      176 2021-11-29 16:18:18.000000 enb-1.0.2/enb/plugins/plugin_ccsds124/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      432 2024-01-01 12:38:20.000000 enb-1.0.2/enb/plugins/plugin_ccsds124/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2898 2024-01-31 17:56:24.000000 enb-1.0.2/enb/plugins/plugin_ccsds124/ccsds124_codecs.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.065866 enb-1.0.2/enb/plugins/plugin_emporda/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      372 2022-12-02 09:46:00.000000 enb-1.0.2/enb/plugins/plugin_emporda/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   126747 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/plugin_emporda/emporda.jar
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     4775 2022-06-14 16:14:05.000000 enb-1.0.2/enb/plugins/plugin_emporda/emporda_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.065866 enb-1.0.2/enb/plugins/plugin_fapec/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       89 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/plugin_fapec/.gitignore
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      391 2021-07-14 12:07:01.000000 enb-1.0.2/enb/plugins/plugin_fapec/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      296 2022-12-02 09:46:00.000000 enb-1.0.2/enb/plugins/plugin_fapec/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    10058 2024-01-01 12:38:20.000000 enb-1.0.2/enb/plugins/plugin_fapec/fapec_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.065866 enb-1.0.2/enb/plugins/plugin_flif/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      424 2021-07-14 12:07:01.000000 enb-1.0.2/enb/plugins/plugin_flif/.gitignore
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1258 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_flif/Makefile.darwin
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     8635 2021-07-14 12:07:01.000000 enb-1.0.2/enb/plugins/plugin_flif/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     6140 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_flif/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1114 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_flif/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1284 2023-02-17 13:23:43.000000 enb-1.0.2/enb/plugins/plugin_flif/flif_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.065866 enb-1.0.2/enb/plugins/plugin_fpack/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      191 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/plugin_fpack/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       26 2023-06-06 14:56:57.000000 enb-1.0.2/enb/plugins/plugin_fpack/__init__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      869 2024-01-01 12:38:20.000000 enb-1.0.2/enb/plugins/plugin_fpack/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     3953 2023-02-19 11:01:26.000000 enb-1.0.2/enb/plugins/plugin_fpack/fpack_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.065866 enb-1.0.2/enb/plugins/plugin_fpc/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      152 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_fpc/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1084 2021-07-14 12:07:01.000000 enb-1.0.2/enb/plugins/plugin_fpc/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      318 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/plugin_fpc/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    12012 2021-07-14 12:07:01.000000 enb-1.0.2/enb/plugins/plugin_fpc/fpc.c
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1211 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_fpc/fpc_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.065866 enb-1.0.2/enb/plugins/plugin_fpzip/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      144 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_fpzip/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      600 2021-07-14 12:07:01.000000 enb-1.0.2/enb/plugins/plugin_fpzip/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      498 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_fpzip/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1366 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_fpzip/fpzip_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.065866 enb-1.0.2/enb/plugins/plugin_fse_huffman/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     4855 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_fse_huffman/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1405 2021-07-14 12:07:01.000000 enb-1.0.2/enb/plugins/plugin_fse_huffman/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      504 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/plugin_fse_huffman/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      944 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_fse_huffman/fse_codec.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1380 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/plugin_fse_huffman/huffman_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.069866 enb-1.0.2/enb/plugins/plugin_hdf5/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      349 2022-12-02 09:46:00.000000 enb-1.0.2/enb/plugins/plugin_hdf5/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     3987 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_hdf5/hdf5_codecs.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.069866 enb-1.0.2/enb/plugins/plugin_hevc/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2394 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_hevc/Makefile.darwin
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1414 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_hevc/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1872 2021-07-14 12:07:02.000000 enb-1.0.2/enb/plugins/plugin_hevc/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      810 2024-01-01 12:38:20.000000 enb-1.0.2/enb/plugins/plugin_hevc/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     5083 2024-01-01 12:38:20.000000 enb-1.0.2/enb/plugins/plugin_hevc/hevc_codec.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     8493 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/plugin_hevc/hevc_lossless_400.cfg
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     8481 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/plugin_hevc/hevc_lossy_400.cfg
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.069866 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2782 2023-05-18 12:37:50.000000 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/AdaptiveHuffmanCompress.cpp
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2097 2023-05-18 12:37:50.000000 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/AdaptiveHuffmanDecompress.cpp
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1655 2023-05-18 12:37:50.000000 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/BitIoStream.cpp
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2600 2023-05-18 12:37:50.000000 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/BitIoStream.hpp
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     4066 2023-05-18 12:37:50.000000 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/CanonicalCode.cpp
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2895 2023-05-18 12:37:50.000000 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/CanonicalCode.hpp
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1944 2023-05-18 12:37:50.000000 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/CodeTree.cpp
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2711 2023-05-18 12:37:50.000000 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/CodeTree.hpp
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     3217 2023-05-18 12:37:50.000000 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/FrequencyTable.cpp
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2671 2023-05-18 12:37:50.000000 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/FrequencyTable.hpp
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1288 2023-05-18 12:37:50.000000 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/HuffmanCoder.cpp
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1823 2023-05-18 12:37:50.000000 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/HuffmanCoder.hpp
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2996 2023-05-18 12:37:50.000000 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/HuffmanCompress.cpp
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1784 2023-05-18 12:37:50.000000 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/HuffmanDecompress.cpp
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      732 2023-05-18 12:38:12.000000 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      321 2023-05-18 12:42:06.000000 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1422 2023-05-18 12:54:04.000000 enb-1.0.2/enb/plugins/plugin_huffman_nayuki/huffman_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.069866 enb-1.0.2/enb/plugins/plugin_iraf_photometry/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)        6 2022-12-02 09:46:00.000000 enb-1.0.2/enb/plugins/plugin_iraf_photometry/.gitignore
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       30 2023-06-06 14:56:57.000000 enb-1.0.2/enb/plugins/plugin_iraf_photometry/__init__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      898 2022-12-02 09:46:00.000000 enb-1.0.2/enb/plugins/plugin_iraf_photometry/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     5605 2023-12-07 15:46:12.000000 enb-1.0.2/enb/plugins/plugin_iraf_photometry/iraf_photometry.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     5106 2022-12-02 09:46:00.000000 enb-1.0.2/enb/plugins/plugin_iraf_photometry/iraf_photometry_slave.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.069866 enb-1.0.2/enb/plugins/plugin_jpeg/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      154 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_jpeg/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       97 2021-07-14 12:07:02.000000 enb-1.0.2/enb/plugins/plugin_jpeg/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      510 2022-12-02 09:46:00.000000 enb-1.0.2/enb/plugins/plugin_jpeg/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    14924 2023-01-16 16:00:24.000000 enb-1.0.2/enb/plugins/plugin_jpeg/jpeg_codecs.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.069866 enb-1.0.2/enb/plugins/plugin_jpeg_xl/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1615 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_jpeg_xl/Makefile.darwin
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1594 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_jpeg_xl/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     8841 2022-01-04 15:31:31.000000 enb-1.0.2/enb/plugins/plugin_jpeg_xl/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1155 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/plugin_jpeg_xl/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2500 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/plugin_jpeg_xl/jpegxl_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.069866 enb-1.0.2/enb/plugins/plugin_kakadu/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       95 2022-06-09 11:53:47.000000 enb-1.0.2/enb/plugins/plugin_kakadu/.gitignore
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1022 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_kakadu/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      326 2022-12-02 09:46:00.000000 enb-1.0.2/enb/plugins/plugin_kakadu/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    15198 2024-01-01 12:38:20.000000 enb-1.0.2/enb/plugins/plugin_kakadu/kakadu_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.069866 enb-1.0.2/enb/plugins/plugin_lcnl/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      231 2021-07-14 12:07:02.000000 enb-1.0.2/enb/plugins/plugin_lcnl/.gitignore
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      271 2021-11-29 16:18:18.000000 enb-1.0.2/enb/plugins/plugin_lcnl/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      830 2023-01-25 11:55:23.000000 enb-1.0.2/enb/plugins/plugin_lcnl/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    21509 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/plugin_lcnl/lcnl_codecs.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.073866 enb-1.0.2/enb/plugins/plugin_lpaq8/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       94 2023-01-12 11:02:40.000000 enb-1.0.2/enb/plugins/plugin_lpaq8/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      334 2023-01-12 10:19:30.000000 enb-1.0.2/enb/plugins/plugin_lpaq8/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    55595 2023-01-19 12:34:54.000000 enb-1.0.2/enb/plugins/plugin_lpaq8/lpaq8.cpp
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1578 2023-01-12 10:27:09.000000 enb-1.0.2/enb/plugins/plugin_lpaq8/lpaq8_codec.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2566 2008-02-15 21:45:22.000000 enb-1.0.2/enb/plugins/plugin_lpaq8/readme.txt
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.073866 enb-1.0.2/enb/plugins/plugin_lz4/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      110 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_lz4/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2011 2021-07-14 12:07:02.000000 enb-1.0.2/enb/plugins/plugin_lz4/README.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      448 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/plugin_lz4/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1483 2023-01-16 16:00:24.000000 enb-1.0.2/enb/plugins/plugin_lz4/lz4_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.073866 enb-1.0.2/enb/plugins/plugin_marlin/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      424 2021-07-14 12:07:02.000000 enb-1.0.2/enb/plugins/plugin_marlin/.gitignore
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1351 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_marlin/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      918 2024-01-01 12:38:20.000000 enb-1.0.2/enb/plugins/plugin_marlin/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1739 2023-02-17 13:23:43.000000 enb-1.0.2/enb/plugins/plugin_marlin/marlin_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.073866 enb-1.0.2/enb/plugins/plugin_mcalic/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2358 2021-07-14 12:07:02.000000 enb-1.0.2/enb/plugins/plugin_mcalic/README.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1020 2023-01-16 16:00:24.000000 enb-1.0.2/enb/plugins/plugin_mcalic/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    18029 2023-02-07 16:50:55.000000 enb-1.0.2/enb/plugins/plugin_mcalic/mcalic_codecs.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.073866 enb-1.0.2/enb/plugins/plugin_mhdc_transforms/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    14291 2022-01-04 15:31:31.000000 enb-1.0.2/enb/plugins/plugin_mhdc_transforms/abstract_mhdc_transform.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     3309 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_mhdc_transforms/iwt.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     3162 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_mhdc_transforms/pot.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.073866 enb-1.0.2/enb/plugins/plugin_montsec/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      358 2024-01-01 12:38:20.000000 enb-1.0.2/enb/plugins/plugin_montsec/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    96904 2024-01-01 12:38:20.000000 enb-1.0.2/enb/plugins/plugin_montsec/montsec.jar
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     3366 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/plugin_montsec/montsec_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.073866 enb-1.0.2/enb/plugins/plugin_ndzip/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      159 2022-04-18 12:35:34.000000 enb-1.0.2/enb/plugins/plugin_ndzip/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1244 2021-07-14 12:07:02.000000 enb-1.0.2/enb/plugins/plugin_ndzip/README.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      750 2024-01-01 12:38:20.000000 enb-1.0.2/enb/plugins/plugin_ndzip/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1988 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/plugin_ndzip/ndzip_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.073866 enb-1.0.2/enb/plugins/plugin_rle/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       65 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/plugin_rle/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     5273 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/plugin_rle/README
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      672 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/plugin_rle/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    35745 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/plugin_rle/rle.zip
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1694 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/plugin_rle/rle_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.073866 enb-1.0.2/enb/plugins/plugin_spdp/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      158 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_spdp/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      874 2021-07-14 12:07:02.000000 enb-1.0.2/enb/plugins/plugin_spdp/README.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     7920 2021-07-14 12:07:02.000000 enb-1.0.2/enb/plugins/plugin_spdp/SPDP_11.c
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      332 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_spdp/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1201 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_spdp/spdp_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.073866 enb-1.0.2/enb/plugins/plugin_speck/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   351672 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/plugin_speck/SpeckCode.jar
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   351673 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/plugin_speck/SpeckDecode.jar
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      422 2023-12-14 14:08:09.000000 enb-1.0.2/enb/plugins/plugin_speck/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     3257 2023-01-19 11:50:46.000000 enb-1.0.2/enb/plugins/plugin_speck/speck_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.073866 enb-1.0.2/enb/plugins/plugin_v2f/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      456 2022-01-04 15:31:31.000000 enb-1.0.2/enb/plugins/plugin_v2f/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    15998 2022-06-09 11:53:47.000000 enb-1.0.2/enb/plugins/plugin_v2f/v2f_codecs.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.077866 enb-1.0.2/enb/plugins/plugin_vvc/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1454 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_vvc/Makefile.darwin
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1515 2022-02-16 15:17:31.000000 enb-1.0.2/enb/plugins/plugin_vvc/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1869 2021-07-14 12:07:02.000000 enb-1.0.2/enb/plugins/plugin_vvc/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      883 2024-01-01 12:38:20.000000 enb-1.0.2/enb/plugins/plugin_vvc/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     8366 2024-01-01 12:38:20.000000 enb-1.0.2/enb/plugins/plugin_vvc/vvc_codec.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     9217 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/plugin_vvc/vvc_lossless_400_inter.cfg
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     6705 2022-04-26 10:10:15.000000 enb-1.0.2/enb/plugins/plugin_vvc/vvc_lossless_400_intra.cfg
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     6653 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/plugin_vvc/vvc_lossless_400_onecomponent.cfg
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     5760 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/plugin_vvc/vvc_lossy_400_onecomponent.cfg
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.077866 enb-1.0.2/enb/plugins/plugin_zfp/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      121 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_zfp/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     5458 2022-01-04 15:31:31.000000 enb-1.0.2/enb/plugins/plugin_zfp/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      500 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_zfp/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2489 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/plugin_zfp/zfp_codec.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.077866 enb-1.0.2/enb/plugins/plugin_zip/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      516 2022-02-16 15:17:31.000000 enb-1.0.2/enb/plugins/plugin_zip/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     3093 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/plugin_zip/zip_codecs.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.077866 enb-1.0.2/enb/plugins/plugin_zstandard/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      132 2022-06-09 11:53:47.000000 enb-1.0.2/enb/plugins/plugin_zstandard/Makefile.darwin
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      132 2022-06-09 11:53:47.000000 enb-1.0.2/enb/plugins/plugin_zstandard/Makefile.linux
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2268 2021-08-31 17:20:37.000000 enb-1.0.2/enb/plugins/plugin_zstandard/README.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      498 2022-06-14 16:14:05.000000 enb-1.0.2/enb/plugins/plugin_zstandard/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     5280 2023-05-08 11:41:21.000000 enb-1.0.2/enb/plugins/plugin_zstandard/zstd_codec.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     9937 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/template.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.077866 enb-1.0.2/enb/plugins/template_analysis_gallery_example/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      356 2022-02-16 15:17:31.000000 enb-1.0.2/enb/plugins/template_analysis_gallery_example/__plugin__.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)    11280 2024-01-01 12:38:20.000000 enb-1.0.2/enb/plugins/template_analysis_gallery_example/generate_gallery.py.enbt
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.077866 enb-1.0.2/enb/plugins/template_analysis_gallery_example/input_csv/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   230049 2022-05-23 13:58:55.000000 enb-1.0.2/enb/plugins/template_analysis_gallery_example/input_csv/2d_data_example.csv
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      704 2024-01-01 12:38:20.000000 enb-1.0.2/enb/plugins/template_analysis_gallery_example/input_csv/continent_data_example.csv
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      800 2024-01-01 12:38:20.000000 enb-1.0.2/enb/plugins/template_analysis_gallery_example/input_csv/function.csv
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    89946 2022-05-23 13:58:55.000000 enb-1.0.2/enb/plugins/template_analysis_gallery_example/input_csv/hevc_frame_prediction.csv
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     4606 2022-05-23 13:58:55.000000 enb-1.0.2/enb/plugins/template_analysis_gallery_example/input_csv/iris_dataset.csv
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.077866 enb-1.0.2/enb/plugins/template_base_experiment/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      826 2023-02-16 11:53:26.000000 enb-1.0.2/enb/plugins/template_base_experiment/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1446 2023-02-16 12:45:43.000000 enb-1.0.2/enb/plugins/template_base_experiment/__plugin__.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.077866 enb-1.0.2/enb/plugins/template_base_experiment/datasets/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    32768 2023-09-15 14:24:43.000000 enb-1.0.2/enb/plugins/template_base_experiment/datasets/data.bin
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     4199 2023-02-16 12:27:10.000000 enb-1.0.2/enb/plugins/template_base_experiment/experiment.py.enbt
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.077866 enb-1.0.2/enb/plugins/template_base_experiment/plugins/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      499 2023-09-15 14:24:43.000000 enb-1.0.2/enb/plugins/template_base_experiment/plugins/__init__.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.077866 enb-1.0.2/enb/plugins/template_basic_workflow_example/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      372 2022-02-16 15:17:31.000000 enb-1.0.2/enb/plugins/template_basic_workflow_example/__plugin__.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     2546 2023-02-13 16:17:41.000000 enb-1.0.2/enb/plugins/template_basic_workflow_example/basic_workflow.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.057866 enb-1.0.2/enb/plugins/template_basic_workflow_example/data/
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_basic_workflow_example/data/wiki/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   134471 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_basic_workflow_example/data/wiki/a_turing.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    49578 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_basic_workflow_example/data/wiki/c_shannon.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    62336 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_basic_workflow_example/data/wiki/d_knuth.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   108445 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_basic_workflow_example/data/wiki/k_popper.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   112486 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_basic_workflow_example/data/wiki/m_curie.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   159578 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_basic_workflow_example/data/wiki/n_chomsky.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   136828 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_basic_workflow_example/data/wiki/r_franklin.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    44597 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_basic_workflow_example/data/wiki/s_beauvoir.txt
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_cluster_config/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      628 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/template_cluster_config/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       94 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/template_cluster_config/enb_cluster.csv
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_colors/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2653 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/template_colors/__plugin__.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2789 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/template_colors/colors-dark.ini
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2790 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/template_colors/colors-default.ini
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_enb_ini/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      771 2022-02-16 15:17:31.000000 enb-1.0.2/enb/plugins/template_enb_ini/__plugin__.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_entropy_codec_comparison/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       89 2022-04-20 12:24:12.000000 enb-1.0.2/enb/plugins/template_entropy_codec_comparison/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2063 2023-02-07 16:50:55.000000 enb-1.0.2/enb/plugins/template_entropy_codec_comparison/__plugin__.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_entropy_codec_comparison/datasets/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    32768 2022-05-23 13:58:55.000000 enb-1.0.2/enb/plugins/template_entropy_codec_comparison/datasets/image_u8be-1x256x128.raw
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     3043 2023-02-16 12:28:01.000000 enb-1.0.2/enb/plugins/template_entropy_codec_comparison/entropy_codec_comparison.py.enbt
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_entropy_codec_comparison/plugins/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      499 2022-05-23 13:58:55.000000 enb-1.0.2/enb/plugins/template_entropy_codec_comparison/plugins/__init__.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_file_version_lowercase_example/
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      379 2022-10-26 12:47:36.000000 enb-1.0.2/enb/plugins/template_file_version_lowercase_example/__plugin__.py
--rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)      867 2022-10-26 12:47:36.000000 enb-1.0.2/enb/plugins/template_file_version_lowercase_example/file_version_example_lowercase.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_file_version_lowercase_example/original_data/
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)   174752 2022-10-26 12:48:17.000000 enb-1.0.2/enb/plugins/template_file_version_lowercase_example/original_data/god_and_state_bakunin.txt
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    34900 2022-10-26 12:48:17.000000 enb-1.0.2/enb/plugins/template_file_version_lowercase_example/original_data/kitten_garden_of_verses_oliver_herford.txt
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_lossless_compression/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      826 2022-10-26 12:47:36.000000 enb-1.0.2/enb/plugins/template_lossless_compression/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1454 2022-12-02 09:46:00.000000 enb-1.0.2/enb/plugins/template_lossless_compression/__plugin__.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_lossless_compression/datasets/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    32768 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_lossless_compression/datasets/image_u8be-2x128x128.raw
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     5109 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/template_lossless_compression/lossless_compression_experiment.py.enbt
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_lossless_compression/plugins/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      499 2021-10-06 09:19:32.000000 enb-1.0.2/enb/plugins/template_lossless_compression/plugins/__init__.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_lossy_compression/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      826 2022-10-26 12:47:36.000000 enb-1.0.2/enb/plugins/template_lossy_compression/README.md
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1445 2022-12-02 09:46:00.000000 enb-1.0.2/enb/plugins/template_lossy_compression/__plugin__.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_lossy_compression/datasets/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    32768 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_lossy_compression/datasets/image1_u8be-1x128x256.raw
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    32768 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_lossy_compression/datasets/image2_u8be-1x128x256.raw
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     5210 2023-02-16 12:28:34.000000 enb-1.0.2/enb/plugins/template_lossy_compression/lossy_compression_experiment.py.enbt
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_lossy_compression/plugins/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      499 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_lossy_compression/plugins/__init__.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_matplotlibrc/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      950 2022-02-16 15:17:31.000000 enb-1.0.2/enb/plugins/template_matplotlibrc/__plugin__.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_montecarlo_pi/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      607 2022-02-16 15:17:31.000000 enb-1.0.2/enb/plugins/template_montecarlo_pi/__plugin__.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     2260 2022-06-09 11:53:47.000000 enb-1.0.2/enb/plugins/template_montecarlo_pi/montecarlo_pi_experiment.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_port_experiment_example/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      360 2022-02-16 15:17:31.000000 enb-1.0.2/enb/plugins/template_port_experiment_example/__plugin__.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.057866 enb-1.0.2/enb/plugins/template_port_experiment_example/data/
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_port_experiment_example/data/ips/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       12 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_port_experiment_example/data/ips/ip1.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       12 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_port_experiment_example/data/ips/ip2.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       12 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_port_experiment_example/data/ips/ip3.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       12 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_port_experiment_example/data/ips/ip4.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       12 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_port_experiment_example/data/ips/ip5.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       12 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_port_experiment_example/data/ips/ip6.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       12 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_port_experiment_example/data/ips/ip7.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       12 2022-05-23 13:57:04.000000 enb-1.0.2/enb/plugins/template_port_experiment_example/data/ips/ip8.txt
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     2031 2023-06-26 12:11:47.000000 enb-1.0.2/enb/plugins/template_port_experiment_example/experiment_example.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.081866 enb-1.0.2/enb/plugins/template_test_all_codecs/
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     3349 2024-01-01 12:38:20.000000 enb-1.0.2/enb/plugins/template_test_all_codecs/__plugin__.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     5209 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/template_test_all_codecs/generate_test_images.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)    10230 2024-02-06 16:27:53.000000 enb-1.0.2/enb/plugins/template_test_all_codecs/test_all_codecs.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     8487 2024-01-01 12:38:20.000000 enb-1.0.2/enb/png.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    18337 2024-02-06 16:27:53.000000 enb-1.0.2/enb/progress.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    41754 2024-02-06 16:27:53.000000 enb-1.0.2/enb/render.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    17050 2024-02-06 16:27:53.000000 enb-1.0.2/enb/sets.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     3348 2023-12-07 15:45:23.000000 enb-1.0.2/enb/tarlite.py
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     4187 2024-02-06 16:27:53.000000 enb-1.0.2/enb/tcall.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.085866 enb-1.0.2/enb.egg-info/
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     3536 2024-02-06 16:28:20.000000 enb-1.0.2/enb.egg-info/PKG-INFO
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    12249 2024-02-06 16:28:20.000000 enb-1.0.2/enb.egg-info/SOURCES.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)        1 2024-02-06 16:28:20.000000 enb-1.0.2/enb.egg-info/dependency_links.txt
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)       42 2024-02-06 16:28:20.000000 enb-1.0.2/enb.egg-info/entry_points.txt
--rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      163 2024-02-06 16:28:20.000000 enb-1.0.2/enb.egg-info/requires.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)        4 2024-02-06 16:28:20.000000 enb-1.0.2/enb.egg-info/top_level.txt
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      100 2021-04-27 15:27:58.000000 enb-1.0.2/pyproject.toml
--rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       38 2024-02-06 16:28:20.085866 enb-1.0.2/setup.cfg
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     3506 2024-02-06 16:27:53.000000 enb-1.0.2/setup.py
-drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-02-06 16:28:20.085866 enb-1.0.2/test/
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     1225 2022-01-04 15:31:31.000000 enb-1.0.2/test/test_aanalysis.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     1328 2023-02-17 10:50:54.000000 enb-1.0.2/test/test_all.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     8108 2023-03-29 09:44:27.000000 enb-1.0.2/test/test_atable.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     1964 2021-10-06 09:19:32.000000 enb-1.0.2/test/test_bitstream.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     2332 2021-10-06 09:19:32.000000 enb-1.0.2/test/test_codec.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     2235 2023-02-17 10:49:26.000000 enb-1.0.2/test/test_experiment.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)    10079 2024-02-06 16:27:53.000000 enb-1.0.2/test/test_icompression.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     3016 2023-03-07 09:28:14.000000 enb-1.0.2/test/test_isets.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     2210 2021-10-06 09:19:32.000000 enb-1.0.2/test/test_log.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     1827 2022-12-02 09:46:00.000000 enb-1.0.2/test/test_pgm.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     1402 2022-06-09 11:53:47.000000 enb-1.0.2/test/test_ray.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     5398 2023-02-17 11:53:45.000000 enb-1.0.2/test/test_sets.py
--rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     1163 2021-10-06 09:19:32.000000 enb-1.0.2/test/test_tarlite.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.031584 enb-1.0.3/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1405 2021-10-06 09:19:32.000000 enb-1.0.3/LICENSE.txt
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    14001 2024-05-19 08:59:35.000000 enb-1.0.3/MANIFEST.in
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     3536 2024-05-21 15:15:34.031584 enb-1.0.3/PKG-INFO
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2215 2024-05-19 08:59:35.000000 enb-1.0.3/README.md
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:33.991584 enb-1.0.3/enb/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     5684 2024-05-19 06:42:49.000000 enb-1.0.3/enb/__init__.py
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)    11909 2024-05-19 06:42:49.000000 enb-1.0.3/enb/__main__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)   187388 2024-05-19 08:59:35.000000 enb-1.0.3/enb/aanalysis.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    94029 2024-05-19 06:42:49.000000 enb-1.0.3/enb/atable.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:33.991584 enb-1.0.3/enb/config/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     4692 2024-05-19 06:42:49.000000 enb-1.0.3/enb/config/__init__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     9156 2024-05-19 06:42:49.000000 enb-1.0.3/enb/config/aini.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    19042 2024-05-19 06:42:49.000000 enb-1.0.3/enb/config/aoptions.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1549 2024-05-19 08:59:35.000000 enb-1.0.3/enb/config/contrib_sha256.csv
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    11317 2024-05-21 15:15:27.000000 enb-1.0.3/enb/config/enb.ini
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:33.995584 enb-1.0.3/enb/config/mpl_styles/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      215 2022-05-23 13:58:55.000000 enb-1.0.3/enb/config/mpl_styles/README.md
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      226 2022-05-23 13:58:55.000000 enb-1.0.3/enb/config/mpl_styles/single_column
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      193 2022-05-23 13:58:55.000000 enb-1.0.3/enb/config/mpl_styles/slides
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      232 2022-05-23 13:58:55.000000 enb-1.0.3/enb/config/mpl_styles/two_columns
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    23890 2024-05-19 06:42:49.000000 enb-1.0.3/enb/config/singleton_cli.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    19298 2024-05-19 06:42:49.000000 enb-1.0.3/enb/experiment.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    12039 2024-05-19 06:42:49.000000 enb-1.0.3/enb/fits.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    73954 2024-05-19 06:42:49.000000 enb-1.0.3/enb/icompression.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    41042 2024-05-19 06:42:49.000000 enb-1.0.3/enb/isets.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      467 2024-05-19 06:42:49.000000 enb-1.0.3/enb/jpg.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    24405 2024-05-19 06:42:49.000000 enb-1.0.3/enb/log.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     9459 2024-05-19 06:42:49.000000 enb-1.0.3/enb/misc.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    10904 2024-05-19 06:42:49.000000 enb-1.0.3/enb/parallel.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    27513 2024-05-19 06:42:49.000000 enb-1.0.3/enb/parallel_ray.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     8096 2024-05-19 06:42:49.000000 enb-1.0.3/enb/pgm.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    29734 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plotdata.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:33.995584 enb-1.0.3/enb/plugins/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      904 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/__init__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    18766 2024-05-19 08:59:35.000000 enb-1.0.3/enb/plugins/installable.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     8184 2024-05-19 08:59:35.000000 enb-1.0.3/enb/plugins/plugin.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:33.995584 enb-1.0.3/enb/plugins/plugin_ac/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      356 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_ac/Makefile.linux
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      540 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_ac/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1518 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_ac/arithmetic_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:33.995584 enb-1.0.3/enb/plugins/plugin_bwt/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    35147 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/COPYING
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     7639 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/COPYING.LESSER
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      977 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/Makefile
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     4662 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/README
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      571 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/__plugin__.py
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)     1249 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/bwt_codec.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    22418 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/bwxform.c
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2488 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/bwxform.h
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:33.999584 enb-1.0.3/enb/plugins/plugin_bwt/optlist/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)       11 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/optlist/.bzrignore
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)       63 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/optlist/.gitignore
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    35147 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/optlist/COPYING
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     7639 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/optlist/COPYING.LESSER
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1080 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/optlist/Makefile
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     3212 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/optlist/README
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    10880 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/optlist/optlist.c
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     3199 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/optlist/optlist.h
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     3916 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/optlist/sample.c
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     4135 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/optlist/sample.cpp
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     6961 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_bwt/sample.c
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:33.999584 enb-1.0.3/enb/plugins/plugin_ccsds122/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      131 2021-07-12 13:17:26.000000 enb-1.0.3/enb/plugins/plugin_ccsds122/.gitignore
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)       75 2021-07-12 12:54:02.000000 enb-1.0.3/enb/plugins/plugin_ccsds122/README.md
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)        0 2023-06-06 14:03:27.000000 enb-1.0.3/enb/plugins/plugin_ccsds122/__init__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      350 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_ccsds122/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     4508 2021-08-31 17:17:48.000000 enb-1.0.3/enb/plugins/plugin_ccsds122/ccsds122_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:33.999584 enb-1.0.3/enb/plugins/plugin_ccsds124/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      114 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_ccsds124/.gitignore
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      176 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_ccsds124/README.md
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      432 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_ccsds124/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2898 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_ccsds124/ccsds124_codecs.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:33.999584 enb-1.0.3/enb/plugins/plugin_emporda/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      906 2024-05-19 08:59:35.000000 enb-1.0.3/enb/plugins/plugin_emporda/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     9570 2024-05-19 08:59:35.000000 enb-1.0.3/enb/plugins/plugin_emporda/emporda_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:33.999584 enb-1.0.3/enb/plugins/plugin_fapec/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       89 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_fapec/.gitignore
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      391 2021-07-12 16:03:45.000000 enb-1.0.3/enb/plugins/plugin_fapec/README.md
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      296 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_fapec/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    10058 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_fapec/fapec_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:33.999584 enb-1.0.3/enb/plugins/plugin_flif/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      424 2021-07-12 11:24:51.000000 enb-1.0.3/enb/plugins/plugin_flif/.gitignore
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1258 2021-08-30 10:31:08.000000 enb-1.0.3/enb/plugins/plugin_flif/Makefile.darwin
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     8635 2021-07-12 11:24:51.000000 enb-1.0.3/enb/plugins/plugin_flif/Makefile.linux
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     6140 2021-08-30 10:31:08.000000 enb-1.0.3/enb/plugins/plugin_flif/README.md
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1114 2021-08-31 17:17:48.000000 enb-1.0.3/enb/plugins/plugin_flif/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1284 2023-02-17 13:23:43.000000 enb-1.0.3/enb/plugins/plugin_flif/flif_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:33.999584 enb-1.0.3/enb/plugins/plugin_fpack/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      191 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_fpack/Makefile.linux
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)       26 2023-06-06 14:56:57.000000 enb-1.0.3/enb/plugins/plugin_fpack/__init__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      869 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_fpack/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     3953 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_fpack/fpack_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.003584 enb-1.0.3/enb/plugins/plugin_fpc/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      152 2021-08-30 10:31:08.000000 enb-1.0.3/enb/plugins/plugin_fpc/Makefile.linux
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1084 2021-07-12 11:24:51.000000 enb-1.0.3/enb/plugins/plugin_fpc/README.md
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      318 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_fpc/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    12012 2021-07-12 11:24:51.000000 enb-1.0.3/enb/plugins/plugin_fpc/fpc.c
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1211 2021-08-31 17:17:48.000000 enb-1.0.3/enb/plugins/plugin_fpc/fpc_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.003584 enb-1.0.3/enb/plugins/plugin_fpzip/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      144 2021-08-30 10:31:08.000000 enb-1.0.3/enb/plugins/plugin_fpzip/Makefile.linux
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      600 2021-07-12 11:24:51.000000 enb-1.0.3/enb/plugins/plugin_fpzip/README.md
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      498 2021-08-31 17:17:48.000000 enb-1.0.3/enb/plugins/plugin_fpzip/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1366 2021-08-31 17:17:48.000000 enb-1.0.3/enb/plugins/plugin_fpzip/fpzip_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.003584 enb-1.0.3/enb/plugins/plugin_fse_huffman/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     4855 2021-08-30 10:31:08.000000 enb-1.0.3/enb/plugins/plugin_fse_huffman/Makefile.linux
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1405 2021-07-12 11:24:51.000000 enb-1.0.3/enb/plugins/plugin_fse_huffman/README.md
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      504 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_fse_huffman/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      944 2021-08-31 17:17:48.000000 enb-1.0.3/enb/plugins/plugin_fse_huffman/fse_codec.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1380 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_fse_huffman/huffman_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.003584 enb-1.0.3/enb/plugins/plugin_hdf5/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      349 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_hdf5/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     3987 2021-08-31 17:17:48.000000 enb-1.0.3/enb/plugins/plugin_hdf5/hdf5_codecs.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.003584 enb-1.0.3/enb/plugins/plugin_hevc/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2394 2021-08-30 10:31:08.000000 enb-1.0.3/enb/plugins/plugin_hevc/Makefile.darwin
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1414 2021-08-30 10:31:08.000000 enb-1.0.3/enb/plugins/plugin_hevc/Makefile.linux
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1872 2021-07-12 11:24:52.000000 enb-1.0.3/enb/plugins/plugin_hevc/README.md
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      810 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_hevc/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     5083 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_hevc/hevc_codec.py
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     8493 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_hevc/hevc_lossless_400.cfg
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     8481 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_hevc/hevc_lossy_400.cfg
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.007584 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2782 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/AdaptiveHuffmanCompress.cpp
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2097 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/AdaptiveHuffmanDecompress.cpp
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1655 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/BitIoStream.cpp
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2600 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/BitIoStream.hpp
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     4066 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/CanonicalCode.cpp
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2895 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/CanonicalCode.hpp
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1944 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/CodeTree.cpp
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2711 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/CodeTree.hpp
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     3217 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/FrequencyTable.cpp
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2671 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/FrequencyTable.hpp
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1288 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/HuffmanCoder.cpp
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1823 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/HuffmanCoder.hpp
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2996 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/HuffmanCompress.cpp
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1784 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/HuffmanDecompress.cpp
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      732 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/Makefile.linux
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      321 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1422 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_huffman_nayuki/huffman_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.007584 enb-1.0.3/enb/plugins/plugin_iraf_photometry/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)        6 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_iraf_photometry/.gitignore
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)       30 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_iraf_photometry/__init__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      898 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_iraf_photometry/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     5605 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_iraf_photometry/iraf_photometry.py
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)     5106 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_iraf_photometry/iraf_photometry_slave.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.007584 enb-1.0.3/enb/plugins/plugin_jpeg/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      154 2021-08-30 10:31:08.000000 enb-1.0.3/enb/plugins/plugin_jpeg/Makefile.linux
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)       97 2021-07-12 15:04:01.000000 enb-1.0.3/enb/plugins/plugin_jpeg/README.md
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      510 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_jpeg/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    14924 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_jpeg/jpeg_codecs.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.007584 enb-1.0.3/enb/plugins/plugin_jpeg_xl/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1615 2021-08-30 10:31:08.000000 enb-1.0.3/enb/plugins/plugin_jpeg_xl/Makefile.darwin
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1594 2021-08-31 17:17:48.000000 enb-1.0.3/enb/plugins/plugin_jpeg_xl/Makefile.linux
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     8841 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_jpeg_xl/README.md
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1155 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_jpeg_xl/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2500 2024-01-15 11:27:42.000000 enb-1.0.3/enb/plugins/plugin_jpeg_xl/jpegxl_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.007584 enb-1.0.3/enb/plugins/plugin_kakadu/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       95 2022-05-30 13:02:26.000000 enb-1.0.3/enb/plugins/plugin_kakadu/.gitignore
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1022 2021-08-30 10:31:08.000000 enb-1.0.3/enb/plugins/plugin_kakadu/README.md
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      326 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_kakadu/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    15198 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_kakadu/kakadu_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.007584 enb-1.0.3/enb/plugins/plugin_lc_framework/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      251 2024-05-19 08:59:35.000000 enb-1.0.3/enb/plugins/plugin_lc_framework/Makefile.linux
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      557 2024-05-19 08:59:35.000000 enb-1.0.3/enb/plugins/plugin_lc_framework/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     9317 2024-05-19 08:59:35.000000 enb-1.0.3/enb/plugins/plugin_lc_framework/lc_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.011584 enb-1.0.3/enb/plugins/plugin_lcnl/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      231 2021-07-12 12:50:16.000000 enb-1.0.3/enb/plugins/plugin_lcnl/.gitignore
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      271 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_lcnl/README.md
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      830 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_lcnl/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    21509 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_lcnl/lcnl_codecs.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.011584 enb-1.0.3/enb/plugins/plugin_lpaq8/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)       94 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_lpaq8/Makefile.linux
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      334 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_lpaq8/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    55595 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_lpaq8/lpaq8.cpp
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1578 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_lpaq8/lpaq8_codec.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2566 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_lpaq8/readme.txt
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.011584 enb-1.0.3/enb/plugins/plugin_lz4/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      110 2021-08-30 10:31:08.000000 enb-1.0.3/enb/plugins/plugin_lz4/Makefile.linux
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2011 2021-07-12 11:24:51.000000 enb-1.0.3/enb/plugins/plugin_lz4/README.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      448 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_lz4/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1483 2023-01-16 16:00:24.000000 enb-1.0.3/enb/plugins/plugin_lz4/lz4_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.011584 enb-1.0.3/enb/plugins/plugin_marlin/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      424 2021-07-12 11:24:52.000000 enb-1.0.3/enb/plugins/plugin_marlin/.gitignore
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1351 2021-08-30 10:31:08.000000 enb-1.0.3/enb/plugins/plugin_marlin/Makefile.linux
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      918 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/plugin_marlin/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1739 2023-02-17 13:23:43.000000 enb-1.0.3/enb/plugins/plugin_marlin/marlin_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.011584 enb-1.0.3/enb/plugins/plugin_mcalic/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2358 2021-07-12 11:24:52.000000 enb-1.0.3/enb/plugins/plugin_mcalic/README.txt
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1020 2023-01-16 16:00:24.000000 enb-1.0.3/enb/plugins/plugin_mcalic/__plugin__.py
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    18029 2023-09-15 14:24:43.000000 enb-1.0.3/enb/plugins/plugin_mcalic/mcalic_codecs.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.011584 enb-1.0.3/enb/plugins/plugin_mhdc_transforms/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    14291 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_mhdc_transforms/abstract_mhdc_transform.py
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)     3309 2021-08-31 17:17:48.000000 enb-1.0.3/enb/plugins/plugin_mhdc_transforms/iwt.py
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)     3162 2021-08-31 17:17:48.000000 enb-1.0.3/enb/plugins/plugin_mhdc_transforms/pot.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.011584 enb-1.0.3/enb/plugins/plugin_montsec/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      358 2023-12-14 14:09:04.000000 enb-1.0.3/enb/plugins/plugin_montsec/__plugin__.py
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    96904 2023-12-14 14:01:21.000000 enb-1.0.3/enb/plugins/plugin_montsec/montsec.jar
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     3366 2024-01-15 11:27:42.000000 enb-1.0.3/enb/plugins/plugin_montsec/montsec_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.011584 enb-1.0.3/enb/plugins/plugin_ndzip/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      159 2022-04-18 12:35:34.000000 enb-1.0.3/enb/plugins/plugin_ndzip/Makefile.linux
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1244 2021-07-13 18:03:11.000000 enb-1.0.3/enb/plugins/plugin_ndzip/README.txt
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      750 2023-11-18 08:55:51.000000 enb-1.0.3/enb/plugins/plugin_ndzip/__plugin__.py
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1988 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_ndzip/ndzip_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.015584 enb-1.0.3/enb/plugins/plugin_rle/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)       65 2024-01-15 11:27:42.000000 enb-1.0.3/enb/plugins/plugin_rle/Makefile.linux
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     5273 2024-01-15 11:27:42.000000 enb-1.0.3/enb/plugins/plugin_rle/README
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      672 2024-01-15 11:27:42.000000 enb-1.0.3/enb/plugins/plugin_rle/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    35745 2024-01-15 11:27:42.000000 enb-1.0.3/enb/plugins/plugin_rle/rle.zip
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1694 2024-01-15 11:27:42.000000 enb-1.0.3/enb/plugins/plugin_rle/rle_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.015584 enb-1.0.3/enb/plugins/plugin_spdp/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      158 2021-08-30 10:31:08.000000 enb-1.0.3/enb/plugins/plugin_spdp/Makefile.linux
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      874 2021-07-12 16:08:12.000000 enb-1.0.3/enb/plugins/plugin_spdp/README.txt
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     7920 2021-07-12 11:24:51.000000 enb-1.0.3/enb/plugins/plugin_spdp/SPDP_11.c
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      332 2021-08-31 17:17:48.000000 enb-1.0.3/enb/plugins/plugin_spdp/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1201 2021-08-31 17:17:48.000000 enb-1.0.3/enb/plugins/plugin_spdp/spdp_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.015584 enb-1.0.3/enb/plugins/plugin_speck/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   351672 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_speck/SpeckCode.jar
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   351673 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_speck/SpeckDecode.jar
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      422 2023-12-14 14:08:09.000000 enb-1.0.3/enb/plugins/plugin_speck/__plugin__.py
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     3257 2023-09-15 14:24:43.000000 enb-1.0.3/enb/plugins/plugin_speck/speck_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.015584 enb-1.0.3/enb/plugins/plugin_v2f/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      456 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_v2f/__plugin__.py
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    15998 2022-05-30 13:02:26.000000 enb-1.0.3/enb/plugins/plugin_v2f/v2f_codecs.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.015584 enb-1.0.3/enb/plugins/plugin_vvc/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1454 2021-08-30 10:31:08.000000 enb-1.0.3/enb/plugins/plugin_vvc/Makefile.darwin
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1515 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_vvc/Makefile.linux
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1869 2021-07-12 11:24:52.000000 enb-1.0.3/enb/plugins/plugin_vvc/README.md
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      883 2023-11-18 08:56:36.000000 enb-1.0.3/enb/plugins/plugin_vvc/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     8366 2023-11-18 10:54:42.000000 enb-1.0.3/enb/plugins/plugin_vvc/vvc_codec.py
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     9217 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_vvc/vvc_lossless_400_inter.cfg
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     6705 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_vvc/vvc_lossless_400_intra.cfg
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     6653 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_vvc/vvc_lossless_400_onecomponent.cfg
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     5760 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_vvc/vvc_lossy_400_onecomponent.cfg
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.015584 enb-1.0.3/enb/plugins/plugin_zfp/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      121 2021-08-30 10:31:08.000000 enb-1.0.3/enb/plugins/plugin_zfp/Makefile.linux
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     5458 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_zfp/README.md
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      500 2021-08-31 17:17:48.000000 enb-1.0.3/enb/plugins/plugin_zfp/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2489 2021-08-31 17:17:48.000000 enb-1.0.3/enb/plugins/plugin_zfp/zfp_codec.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.015584 enb-1.0.3/enb/plugins/plugin_zip/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      516 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_zip/__plugin__.py
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     3093 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/plugin_zip/zip_codecs.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.019584 enb-1.0.3/enb/plugins/plugin_zstandard/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      132 2022-05-30 13:02:30.000000 enb-1.0.3/enb/plugins/plugin_zstandard/Makefile.darwin
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      132 2022-05-30 13:02:30.000000 enb-1.0.3/enb/plugins/plugin_zstandard/Makefile.linux
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2268 2021-08-30 10:31:08.000000 enb-1.0.3/enb/plugins/plugin_zstandard/README.txt
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      498 2022-06-14 16:14:05.000000 enb-1.0.3/enb/plugins/plugin_zstandard/__plugin__.py
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     5280 2023-09-15 14:24:43.000000 enb-1.0.3/enb/plugins/plugin_zstandard/zstd_codec.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     9937 2024-01-15 11:27:42.000000 enb-1.0.3/enb/plugins/template.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.019584 enb-1.0.3/enb/plugins/template_analysis_gallery_example/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      356 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_analysis_gallery_example/__plugin__.py
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)    11280 2024-01-01 11:35:30.000000 enb-1.0.3/enb/plugins/template_analysis_gallery_example/generate_gallery.py.enbt
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.019584 enb-1.0.3/enb/plugins/template_analysis_gallery_example/input_csv/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   230049 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_analysis_gallery_example/input_csv/2d_data_example.csv
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      704 2023-12-02 21:07:15.000000 enb-1.0.3/enb/plugins/template_analysis_gallery_example/input_csv/continent_data_example.csv
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      800 2023-12-20 09:43:23.000000 enb-1.0.3/enb/plugins/template_analysis_gallery_example/input_csv/function.csv
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    89946 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_analysis_gallery_example/input_csv/hevc_frame_prediction.csv
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     4606 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_analysis_gallery_example/input_csv/iris_dataset.csv
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.019584 enb-1.0.3/enb/plugins/template_base_experiment/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      826 2023-09-15 14:24:43.000000 enb-1.0.3/enb/plugins/template_base_experiment/README.md
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     1446 2023-09-15 14:24:43.000000 enb-1.0.3/enb/plugins/template_base_experiment/__plugin__.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.019584 enb-1.0.3/enb/plugins/template_base_experiment/datasets/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    32768 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/template_base_experiment/datasets/data.bin
+-rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     4199 2023-09-15 14:24:43.000000 enb-1.0.3/enb/plugins/template_base_experiment/experiment.py.enbt
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.019584 enb-1.0.3/enb/plugins/template_base_experiment/plugins/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      499 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/template_base_experiment/plugins/__init__.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.019584 enb-1.0.3/enb/plugins/template_basic_workflow_example/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      372 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_basic_workflow_example/__plugin__.py
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)     2546 2023-02-13 16:17:41.000000 enb-1.0.3/enb/plugins/template_basic_workflow_example/basic_workflow.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:33.983584 enb-1.0.3/enb/plugins/template_basic_workflow_example/data/
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.019584 enb-1.0.3/enb/plugins/template_basic_workflow_example/data/wiki/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   134471 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_basic_workflow_example/data/wiki/a_turing.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    49578 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_basic_workflow_example/data/wiki/c_shannon.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    62336 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_basic_workflow_example/data/wiki/d_knuth.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   108445 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_basic_workflow_example/data/wiki/k_popper.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   112486 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_basic_workflow_example/data/wiki/m_curie.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   159578 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_basic_workflow_example/data/wiki/n_chomsky.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)   136828 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_basic_workflow_example/data/wiki/r_franklin.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    44597 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_basic_workflow_example/data/wiki/s_beauvoir.txt
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.023584 enb-1.0.3/enb/plugins/template_cluster_config/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      628 2024-01-15 11:27:42.000000 enb-1.0.3/enb/plugins/template_cluster_config/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)       94 2024-01-15 11:27:42.000000 enb-1.0.3/enb/plugins/template_cluster_config/enb_cluster.csv
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.023584 enb-1.0.3/enb/plugins/template_colors/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2653 2024-01-15 11:27:42.000000 enb-1.0.3/enb/plugins/template_colors/__plugin__.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2789 2024-01-15 11:27:42.000000 enb-1.0.3/enb/plugins/template_colors/colors-dark.ini
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     2790 2024-01-15 11:27:42.000000 enb-1.0.3/enb/plugins/template_colors/colors-default.ini
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.023584 enb-1.0.3/enb/plugins/template_enb_ini/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      771 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_enb_ini/__plugin__.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.023584 enb-1.0.3/enb/plugins/template_entropy_codec_comparison/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       89 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_entropy_codec_comparison/README.md
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)     2063 2023-09-15 14:24:43.000000 enb-1.0.3/enb/plugins/template_entropy_codec_comparison/__plugin__.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.023584 enb-1.0.3/enb/plugins/template_entropy_codec_comparison/datasets/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    32768 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_entropy_codec_comparison/datasets/image_u8be-1x256x128.raw
+-rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     3043 2023-09-15 14:24:43.000000 enb-1.0.3/enb/plugins/template_entropy_codec_comparison/entropy_codec_comparison.py.enbt
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.023584 enb-1.0.3/enb/plugins/template_entropy_codec_comparison/plugins/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      499 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_entropy_codec_comparison/plugins/__init__.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.023584 enb-1.0.3/enb/plugins/template_file_version_lowercase_example/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      379 2022-10-26 12:48:17.000000 enb-1.0.3/enb/plugins/template_file_version_lowercase_example/__plugin__.py
+-rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)      867 2022-10-26 12:48:17.000000 enb-1.0.3/enb/plugins/template_file_version_lowercase_example/file_version_example_lowercase.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.023584 enb-1.0.3/enb/plugins/template_file_version_lowercase_example/original_data/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)   174752 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/template_file_version_lowercase_example/original_data/god_and_state_bakunin.txt
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    34900 2024-05-19 06:42:49.000000 enb-1.0.3/enb/plugins/template_file_version_lowercase_example/original_data/kitten_garden_of_verses_oliver_herford.txt
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.023584 enb-1.0.3/enb/plugins/template_lossless_compression/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      826 2022-10-26 12:48:17.000000 enb-1.0.3/enb/plugins/template_lossless_compression/README.md
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1454 2022-11-07 13:00:43.000000 enb-1.0.3/enb/plugins/template_lossless_compression/__plugin__.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.023584 enb-1.0.3/enb/plugins/template_lossless_compression/datasets/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    32768 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_lossless_compression/datasets/image_u8be-2x128x128.raw
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)     5109 2024-01-15 11:27:42.000000 enb-1.0.3/enb/plugins/template_lossless_compression/lossless_compression_experiment.py.enbt
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.023584 enb-1.0.3/enb/plugins/template_lossless_compression/plugins/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      499 2021-09-10 07:14:09.000000 enb-1.0.3/enb/plugins/template_lossless_compression/plugins/__init__.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.023584 enb-1.0.3/enb/plugins/template_lossy_compression/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      826 2022-10-26 12:48:17.000000 enb-1.0.3/enb/plugins/template_lossy_compression/README.md
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     1445 2022-11-07 13:00:54.000000 enb-1.0.3/enb/plugins/template_lossy_compression/__plugin__.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.023584 enb-1.0.3/enb/plugins/template_lossy_compression/datasets/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    32768 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_lossy_compression/datasets/image1_u8be-1x128x256.raw
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    32768 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_lossy_compression/datasets/image2_u8be-1x128x256.raw
+-rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     5210 2023-09-15 14:24:43.000000 enb-1.0.3/enb/plugins/template_lossy_compression/lossy_compression_experiment.py.enbt
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.023584 enb-1.0.3/enb/plugins/template_lossy_compression/plugins/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      499 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_lossy_compression/plugins/__init__.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.023584 enb-1.0.3/enb/plugins/template_matplotlibrc/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      950 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_matplotlibrc/__plugin__.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.027584 enb-1.0.3/enb/plugins/template_montecarlo_pi/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      607 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_montecarlo_pi/__plugin__.py
+-rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     2260 2022-05-30 13:02:26.000000 enb-1.0.3/enb/plugins/template_montecarlo_pi/montecarlo_pi_experiment.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.027584 enb-1.0.3/enb/plugins/template_port_experiment_example/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      360 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_port_experiment_example/__plugin__.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:33.987584 enb-1.0.3/enb/plugins/template_port_experiment_example/data/
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.027584 enb-1.0.3/enb/plugins/template_port_experiment_example/data/ips/
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       12 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_port_experiment_example/data/ips/ip1.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       12 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_port_experiment_example/data/ips/ip2.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       12 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_port_experiment_example/data/ips/ip3.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       12 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_port_experiment_example/data/ips/ip4.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       12 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_port_experiment_example/data/ips/ip5.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       12 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_port_experiment_example/data/ips/ip6.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       12 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_port_experiment_example/data/ips/ip7.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       12 2022-05-23 13:58:55.000000 enb-1.0.3/enb/plugins/template_port_experiment_example/data/ips/ip8.txt
+-rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     2031 2023-09-15 14:24:43.000000 enb-1.0.3/enb/plugins/template_port_experiment_example/experiment_example.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.027584 enb-1.0.3/enb/plugins/template_test_all_codecs/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     3349 2023-11-18 10:54:42.000000 enb-1.0.3/enb/plugins/template_test_all_codecs/__plugin__.py
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)     5209 2024-01-15 11:27:42.000000 enb-1.0.3/enb/plugins/template_test_all_codecs/generate_test_images.py
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)    10230 2024-01-31 16:24:04.000000 enb-1.0.3/enb/plugins/template_test_all_codecs/test_all_codecs.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     8487 2023-12-07 15:45:28.000000 enb-1.0.3/enb/png.py
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    18337 2024-01-15 13:00:38.000000 enb-1.0.3/enb/progress.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    41754 2024-02-02 13:25:53.000000 enb-1.0.3/enb/render.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)    16675 2024-05-19 08:59:35.000000 enb-1.0.3/enb/sets.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     3348 2023-12-07 15:45:23.000000 enb-1.0.3/enb/tarlite.py
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     4187 2024-02-01 15:15:14.000000 enb-1.0.3/enb/tcall.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.031584 enb-1.0.3/enb.egg-info/
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)     3536 2024-05-21 15:15:33.000000 enb-1.0.3/enb.egg-info/PKG-INFO
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)    12347 2024-05-21 15:15:33.000000 enb-1.0.3/enb.egg-info/SOURCES.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)        1 2024-05-21 15:15:33.000000 enb-1.0.3/enb.egg-info/dependency_links.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       42 2024-05-21 15:15:33.000000 enb-1.0.3/enb.egg-info/entry_points.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)      163 2024-05-21 15:15:33.000000 enb-1.0.3/enb.egg-info/requires.txt
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)        4 2024-05-21 15:15:33.000000 enb-1.0.3/enb.egg-info/top_level.txt
+-rw-r--r--   0 miguelinux  (1000) miguelinux  (1000)      100 2021-04-27 11:15:00.000000 enb-1.0.3/pyproject.toml
+-rw-rw-r--   0 miguelinux  (1000) miguelinux  (1000)       38 2024-05-21 15:15:34.031584 enb-1.0.3/setup.cfg
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)     3506 2024-01-31 16:25:22.000000 enb-1.0.3/setup.py
+drwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)        0 2024-05-21 15:15:34.027584 enb-1.0.3/test/
+-rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     1225 2022-05-23 13:58:55.000000 enb-1.0.3/test/test_aanalysis.py
+-rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     1328 2023-09-15 14:24:43.000000 enb-1.0.3/test/test_all.py
+-rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     8108 2023-09-15 14:24:43.000000 enb-1.0.3/test/test_atable.py
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)     1964 2021-08-31 17:17:48.000000 enb-1.0.3/test/test_bitstream.py
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)     2332 2021-08-31 17:17:48.000000 enb-1.0.3/test/test_codec.py
+-rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     2235 2023-09-15 14:24:43.000000 enb-1.0.3/test/test_experiment.py
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)    10079 2024-02-01 15:05:30.000000 enb-1.0.3/test/test_icompression.py
+-rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     3016 2023-09-15 14:24:43.000000 enb-1.0.3/test/test_isets.py
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)     2210 2021-08-31 17:17:48.000000 enb-1.0.3/test/test_log.py
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)     1827 2022-11-10 17:11:27.000000 enb-1.0.3/test/test_pgm.py
+-rwxrwxr-x   0 miguelinux  (1000) miguelinux  (1000)     1402 2022-05-30 13:02:26.000000 enb-1.0.3/test/test_ray.py
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)     5408 2024-05-19 08:59:35.000000 enb-1.0.3/test/test_sets.py
+-rwxr--r--   0 miguelinux  (1000) miguelinux  (1000)     1163 2021-08-31 17:17:48.000000 enb-1.0.3/test/test_tarlite.py
```

### Comparing `enb-1.0.2/LICENSE.txt` & `enb-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/MANIFEST.in` & `enb-1.0.3/MANIFEST.in`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 include enb/plugins/plugin_ccsds122/__plugin__.py
 include enb/plugins/plugin_ccsds122/README.md
 include enb/plugins/plugin_ccsds124/ccsds124_codecs.py
 include enb/plugins/plugin_ccsds124/.gitignore
 include enb/plugins/plugin_ccsds124/__plugin__.py
 include enb/plugins/plugin_ccsds124/README.md
 include enb/plugins/plugin_emporda/emporda_codec.py
-include enb/plugins/plugin_emporda/emporda.jar
 include enb/plugins/plugin_emporda/__plugin__.py
 include enb/plugins/plugin_fapec/fapec_codec.py
 include enb/plugins/plugin_fapec/.gitignore
 include enb/plugins/plugin_fapec/__plugin__.py
 include enb/plugins/plugin_fapec/README.md
 include enb/plugins/plugin_flif/flif_codec.py
 include enb/plugins/plugin_flif/.gitignore
@@ -126,14 +125,17 @@
 include enb/plugins/plugin_jpeg_xl/Makefile.linux
 include enb/plugins/plugin_jpeg_xl/__plugin__.py
 include enb/plugins/plugin_jpeg_xl/README.md
 include enb/plugins/plugin_kakadu/.gitignore
 include enb/plugins/plugin_kakadu/kakadu_codec.py
 include enb/plugins/plugin_kakadu/__plugin__.py
 include enb/plugins/plugin_kakadu/README.md
+include enb/plugins/plugin_lc_framework/lc_codec.py
+include enb/plugins/plugin_lc_framework/Makefile.linux
+include enb/plugins/plugin_lc_framework/__plugin__.py
 include enb/plugins/plugin_lcnl/.gitignore
 include enb/plugins/plugin_lcnl/lcnl_codecs.py
 include enb/plugins/plugin_lcnl/__plugin__.py
 include enb/plugins/plugin_lcnl/README.md
 include enb/plugins/plugin_lpaq8/lpaq8_codec.py
 include enb/plugins/plugin_lpaq8/lpaq8.cpp
 include enb/plugins/plugin_lpaq8/Makefile.linux
```

### Comparing `enb-1.0.2/PKG-INFO` & `enb-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: enb
-Version: 1.0.2
+Version: 1.0.3
 Summary: Experiment NoteBook (enb): efficient and reproducible science.
 Home-page: https://github.com/miguelinux314/experiment-notebook
-Download-URL: https://github.com/miguelinux314/experiment-notebook/archive/v1.0.2.tar.gz
+Download-URL: https://github.com/miguelinux314/experiment-notebook/archive/v1.0.3.tar.gz
 Author: Miguel Hernández Cabronero, et al.
 Author-email: miguel.hernandez@uab.cat
 License: MIT License
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
@@ -37,15 +37,15 @@
 Requires-Dist: astropy
 Requires-Dist: natsort
 Requires-Dist: rich
 Requires-Dist: h5py
 
 # Experiment Notebook (`enb`)
 
-The `enb` Python (>= 3.6) library is a table-based framework designed to define, run and report computer-based
+The `enb` Python (>= 3.7) library is a table-based framework designed to define, run and report computer-based
 experiments.
 
 - Your can create and run any type of (computer-based) experiment. Quickly.
 - You can analyze and plot results produced with your enb experiments. Clearly. You can also reuse previously existing
   data (e.g., in CSV format).
 - You can easily create reproducible, redistributable software to be shared with others, e.g., as supplementary
   materials in your publication or project.
```

### Comparing `enb-1.0.2/README.md` & `enb-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Experiment Notebook (`enb`)
 
-The `enb` Python (>= 3.6) library is a table-based framework designed to define, run and report computer-based
+The `enb` Python (>= 3.7) library is a table-based framework designed to define, run and report computer-based
 experiments.
 
 - Your can create and run any type of (computer-based) experiment. Quickly.
 - You can analyze and plot results produced with your enb experiments. Clearly. You can also reuse previously existing
   data (e.g., in CSV format).
 - You can easily create reproducible, redistributable software to be shared with others, e.g., as supplementary
   materials in your publication or project.
```

### Comparing `enb-1.0.2/enb/__init__.py` & `enb-1.0.3/enb/__init__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/__main__.py` & `enb-1.0.3/enb/__main__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/aanalysis.py` & `enb-1.0.3/enb/aanalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,14 +260,15 @@
                 self.save_analysis_tables(
                     group_by=group_by,
                     reference_group=reference_group,
                     selected_render_modes=selected_render_modes,
                     summary_df=summary_df,
                     summary_table=summary_table,
                     target_columns=target_columns,
+                    column_to_properties=column_to_properties,
                     **render_kwargs)
 
                 # Return the summary result dataframe
                 return summary_df
 
             normalized_wrapper = self.__class__.normalize_parameters(
                 fun=normalized_wrapper,
@@ -349,23 +350,25 @@
                         id_list=render_ids,
                         iteration_period=self.progress_report_period,
                         alive_bar=None):
                     pass
                 enb.parallel.get(render_ids)
             else:
                 # Rich progress reporting
-                with enb.progress.ProgressTracker(self, len(render_ids), len(render_ids)) as progress_tracker:
+                with enb.progress.ProgressTracker(self, len(render_ids),
+                                                  len(render_ids)) as progress_tracker:
                     progressive_getter = enb.parallel.ProgressiveGetter(
                         id_list=render_ids,
                         iteration_period=self.progress_report_period,
                         alive_bar=None)
                     for _ in progressive_getter:
-                        progress_tracker.update_chunk_completed_rows(len(progressive_getter.completed_ids))
+                        progress_tracker.update_chunk_completed_rows(
+                            len(progressive_getter.completed_ids))
                     enb.parallel.get(render_ids)
-                    progress_tracker.complete_chunk() # A single chunk is employed
+                    progress_tracker.complete_chunk()  # A single chunk is employed
                     progress_tracker.update_chunk_completed_rows(0)
 
     def update_render_kwargs_one_case(
             self, column_selection, reference_group, render_mode,
             # Dynamic arguments with every call
             summary_df, output_plot_dir,
             group_by, column_to_properties,
@@ -492,15 +495,14 @@
         try:
             column_kwargs["group_name_order"] = [
                 n for n in column_kwargs["group_name_order"]
                 if n != reference_group]
         except KeyError:
             pass
 
-
     def get_output_pdf_path(self, column_selection, group_by, reference_group,
                             output_plot_dir, render_mode):
         """Get the path of the PDF file to be created for a single
         parameter selection.
         """
         # pylint: disable=too-many-arguments
         if isinstance(column_selection, str):
@@ -531,15 +533,17 @@
             (f"-groupby__{get_groupby_str(group_by=group_by)}" if group_by else "") +
             (f"-referencegroup__{reference_group}" if reference_group else "") +
             ".pdf")
 
     def save_analysis_tables(
             self, group_by, reference_group,
             selected_render_modes, summary_df, summary_table,
-            target_columns, **render_kwargs):
+            target_columns,
+            column_to_properties,
+            **render_kwargs):
         """Save csv and tex files into enb.config.options.analysis_dir that
         summarize the results of one target_columns element. If
         enb.config.options.analysis_dir is None or empty, no analysis is
         performed.
 
         By default, the CSV contains the min, max, avg, std, and median of each
         group. Subclasses may overwrite this behavior.
@@ -557,34 +561,43 @@
                 reference_group=reference_group,
                 output_plot_dir=options.analysis_dir,
                 render_mode=render_mode_str)[:-4] + ".csv"
             enb.logger.debug(
                 f"Saving analysis results to {analysis_output_path}")
             os.makedirs(os.path.dirname(analysis_output_path), exist_ok=True)
 
+            column_rename_dict = {"group_label": "Group"}
+            for c in summary_df:
+                if c.endswith("_avg"):
+                    try:
+                        column_rename_dict[c] = column_to_properties[c[:-len("_avg")]].label
+                    except KeyError:
+                        pass
+
             # Save CSV analysis
             summary_df[list(
                 c for c in summary_df.columns
                 if c not in summary_table.render_column_names
                 and c not in ["row_created", "row_updated",
-                              enb.atable.ATable.private_index_column])].to_csv(
-                analysis_output_path, index=False)
+                              enb.atable.ATable.private_index_column])].copy().rename(
+                columns=column_rename_dict).to_csv(analysis_output_path, index=False)
 
             # Generate tex summary
             show_count = "show_count" in render_kwargs and render_kwargs["show_count"] is True
             summary_df[list(
                 c for c in summary_df.columns
                 if c not in summary_table.render_column_names
                 and c not in ["row_created", "row_updated",
                               enb.atable.ATable.private_index_column]
                 and (c in ("group_label", "group_size" if show_count else "")
-                     or c.endswith("_avg")))].style.format(
+                     or c.endswith("_avg")))].copy().rename(
+                columns=column_rename_dict).style.format(
                 escape="latex",
                 precision=self.latex_decimal_count).format_index(
-                r"\textbf{{ {} }}", escape="latex", axis=1).hide(
+                r"\textbf{{{}}}", escape="latex", axis=1).hide(
                 axis="index").to_latex(
                 analysis_output_path[:-4] + ".tex")
 
     @classmethod
     def normalize_parameters(cls, fun, group_by, column_to_properties,
                              target_columns, reference_group,
                              output_plot_dir, selected_render_modes):
@@ -1426,18 +1439,19 @@
 
     def set_scalar_description(self, *args, **kwargs):
         """Set basic descriptive statistics for the target column
         """
         _self, group_label, row = args
         column_name = kwargs["column_selection"]
         full_series = _self.label_to_df[group_label][column_name]
-        for stat, value in _self.numeric_series_to_stat_dict(full_series, group_label=group_label).items():
+        for stat, value in _self.numeric_series_to_stat_dict(full_series,
+                                                             group_label=group_label).items():
             row[f"{column_name}_{stat}"] = value
 
-    def numeric_series_to_stat_dict(self, series: pd.Series, group_label: str=None):
+    def numeric_series_to_stat_dict(self, series: pd.Series, group_label: str = None):
         """Convert a series of numeric data into a dictionary of
         stats ('avg', 'min', 'max', 'std', 'count').
 
         :param series: series of numeric scalar data to be analyzed.
           Infinite and nan values are removed before processing.
         :return: a dictionary of stats for `series`.
         """
@@ -1944,15 +1958,15 @@
                                  reference_group=reference_group,
                                  target_columns=target_columns,
                                  group_by=group_by,
                                  include_all_group=include_all_group)
 
     def save_analysis_tables(
             self, group_by, reference_group, selected_render_modes, summary_df,
-            summary_table, target_columns, **render_kwargs):
+            summary_table, target_columns, column_to_properties, **render_kwargs):
         """Save csv and tex files into enb.config.options.analysis_dir that
         summarize the results of one target_columns element. If
         enb.config.options.analysis_dir is None or empty, no analysis is
         performed.
 
         By default, the CSV contains the min, max, avg, std, and median of
         each group. Subclasses may overwrite this behavior.
@@ -1963,14 +1977,15 @@
                 super().save_analysis_tables(
                     group_by=group_by,
                     reference_group=reference_group,
                     selected_render_modes={render_mode},
                     summary_df=summary_df,
                     summary_table=summary_table,
                     target_columns=target_columns,
+                    column_to_properties=column_to_properties,
                     **render_kwargs)
             elif options.analysis_dir:
                 for column_pair in target_columns:
                     analysis_output_path = self.get_output_pdf_path(
                         column_selection=[column_pair],
                         group_by=group_by,
                         reference_group=reference_group,
@@ -2116,28 +2131,29 @@
                         processed_y_to_x_columns[y_column] = x_column
                     except KeyError:
                         pass
 
                 reference_count_by_xvalue = dict()
                 for x_value in group_df[x_column].unique():
                     reference_filtered_df = group_df.loc[group_df[x_column] == x_value]
-                    reference_filtered_df = reference_filtered_df.loc[reference_filtered_df[y_column].notna()]
+                    reference_filtered_df = reference_filtered_df.loc[
+                        reference_filtered_df[y_column].notna()]
                     reference_count_by_xvalue[x_value] = len(reference_filtered_df)
                     self.reference_df.loc[self.reference_df[x_column] == x_value, y_column] \
                         -= reference_filtered_df[y_column].mean()
 
-
                 warning_shown = False
                 for target_group_label, target_group_df in self.split_groups():
                     for y_column, x_column in processed_y_to_x_columns.items():
                         for x_value in target_group_df[x_column].unique():
                             target_filtered_df = target_group_df[
                                 target_group_df[x_column] == x_value].notna()
                             target_count = len(target_filtered_df)
-                            if not warning_shown and target_count != reference_count_by_xvalue[x_value]:
+                            if not warning_shown and target_count != reference_count_by_xvalue[
+                                x_value]:
                                 enb.logger.warn(
                                     "Warning: when applying group reference bias, it was found that "
                                     f"group {repr(target_group_label)} contained {target_count} elements "
                                     f"for {x_column}={x_value} but the reference group ({self.reference_group}) "
                                     f"contained {reference_count_by_xvalue[x_value]}. This message is shown "
                                     f"only once per call: other columns and/or x values might have the same "
                                     f"problem.")
@@ -3143,18 +3159,20 @@
         :param show_global_row: if True, or if None and self.show_global is True, an extra row is
           added to the analysis, corresponding to not splitting the data into the y categories
           (i.e., considering the average for all possible y categories). Note that if y_header_list is selected,
           averages are considered only for those categories.
         :param show_global_column: like show_global_row, but adds a new column corresponding to not splitting
           into x categories. Note that if x_header_list is selected, averages are considered only for those categories.
         """
-        if highlight_best_column is not None and str(highlight_best_column).lower() not in ("low", "high"):
+        if highlight_best_column is not None and str(highlight_best_column).lower() not in (
+                "low", "high"):
             raise ValueError(
                 f"Invalid {highlight_best_column=}. Must be one of {('low', 'high', None)}")
-        if highlight_best_row is not None and str(highlight_best_row).lower() not in ("low", "high"):
+        if highlight_best_row is not None and str(highlight_best_row).lower() not in (
+                "low", "high"):
             raise ValueError(
                 f"Invalid {highlight_best_row=}. Must be one of {('low', 'high', None)}")
 
         if "show_global" in render_kwargs:
             enb.logger.warn(f"Warning: `show_global` is ignored in {self.__class__.__name__}; "
                             f"use `show_global_row` and/or `show_global_column` instead.")
 
@@ -3235,20 +3253,21 @@
                                          reference_group=reference_group,
                                          group_by=group_by,
                                          show_global_row=render_kwargs["show_global_row"],
                                          show_global_column=render_kwargs["show_global_column"],
                                          x_header_list=render_kwargs["x_header_list"],
                                          y_header_list=render_kwargs["y_header_list"],
                                          highlight_best_row=render_kwargs["highlight_best_row"],
-                                         highlight_best_column=render_kwargs["highlight_best_column"])
+                                         highlight_best_column=render_kwargs[
+                                             "highlight_best_column"])
 
     def save_analysis_tables(
             self, group_by, reference_group,
             selected_render_modes, summary_df, summary_table,
-            target_columns, **render_kwargs):
+            target_columns, column_to_properties, **render_kwargs):
         """
         Store the joint analysis results in CSV and latex formats.
 
         If enb.config.options.analysis_dir is None or empty, no analysis is
         performed.
         """
         # pylint: disable=too-many-arguments
@@ -3270,16 +3289,31 @@
 
             assert set(selected_render_modes) == {"table"}, \
                 f"Only the table render mode is currently supported by {self.__class__.__name__}"
 
             # Generate CSV tables
             with open(analysis_output_path, "w") as csv_file:
                 for x_column, y_column, data_column in target_columns:
-                    csv_file.write(f"\n\n# Column selection: "
-                                   f"{repr(x_column)} {repr(y_column)} {repr(data_column)}\n")
+
+                    try:
+                        x_column_name = column_to_properties[x_column].label
+                    except KeyError:
+                        x_column_name = str(x_column)
+                    try:
+                        y_column_name = column_to_properties[y_column].label
+                    except KeyError:
+                        y_column_name = str(y_column)
+                    try:
+                        data_column_name = column_to_properties[data_column].label
+                    except KeyError:
+                        data_column_name = str(data_column)
+
+                    csv_file.write(
+                        f"\n\n# Column selection: "
+                        f"{repr(x_column_name)} {repr(y_column_name)} {repr(data_column_name)}\n")
 
                     for stat in ["avg", "count", "min", "max", "std", "median"]:
                         csv_file.write(f"\n## Statistic: {stat}\n")
 
                         for group_name, group_df in summary_df.iterrows():
                             summary_dict = group_df[f"{x_column}_{y_column}_{data_column}_{stat}"]
 
@@ -3317,24 +3351,35 @@
                                     except KeyError:
                                         csv_file.write(",")
                                 csv_file.write("\n")
 
             # Generate latex tables
             with (open(analysis_output_path[:-4] + ".tex", "w") as latex_file):
                 for x_column, y_column, data_column in target_columns:
+                    try:
+                        x_column_name = column_to_properties[x_column].label
+                    except KeyError:
+                        x_column_name = str(x_column)
+                    try:
+                        y_column_name = column_to_properties[y_column].label
+                    except KeyError:
+                        y_column_name = str(y_column)
+
                     column_header_count = len(summary_table.category_to_values[x_column])
+                    if summary_table.show_global_column and len(x_categories) > 1:
+                        column_header_count += 1
                     longest_row_header = max(
                         len(str(y)) for y in summary_table.category_to_values[y_column])
                     if summary_table.include_all_group and len(
                             summary_table.category_to_values[y_column]) > 1:
                         longest_row_header = max(len(self.global_group_name), longest_row_header)
                     longest_row_header += len(r"\textbf{}")
 
                     latex_file.write(f"\n\n% Column selection: "
-                                     f"{repr(x_column)} {repr(y_column)} {repr(data_column)}\n")
+                                     f"{repr(x_column_name)} {repr(y_column_name)} {repr(data_column)}\n")
                     for stat in ["avg", "count", "min", "max", "std", "median"]:
                         latex_file.write(f"\n% Statistic: {enb.misc.escape_latex(stat)}\n")
                         latex_file.write(
                             r"\begin{tabular}{l" + "c" * column_header_count + r"}" + "\n")
                         latex_file.write(r"\toprule" + "\n")
 
                         for group_name, group_df in summary_df.iterrows():
@@ -3342,15 +3387,16 @@
                                 x_categories=summary_table.category_to_values[x_column],
                                 y_categories=summary_table.category_to_values[y_column],
                                 reference_group=summary_table.reference_group)
 
                             summary_dict = group_df[f"{x_column}_{y_column}_{data_column}_{stat}"]
                             number_format = self.number_format if stat != "count" else "{:d}"
                             longest_cell_length = max(
-                                max(len(number_format.format(val)) for val in summary_dict.values()),
+                                max(len(number_format.format(val)) for val in
+                                    summary_dict.values()),
                                 max(len(str(x)) for x in x_categories)) + len(r"\textbf{}")
                             row_header_format = f"{{:{longest_row_header}s}}"
                             cell_format = f"{{:{longest_cell_length}s}}"
 
                             # Write group separator if there is more than one group
                             if len(summary_df) > 1:
                                 group_label = " ".join(
@@ -3365,15 +3411,16 @@
                                 y_categories.append(None)
                             if summary_table.show_global_column and len(x_categories) > 1:
                                 x_categories.append(None)
 
                             # Write the (sub) table headers
                             latex_file.write(
                                 " " * longest_row_header + " & "
-                                + " & ".join(cell_format.format(r"\textbf{" + str(x or self.global_group_name) + r"}")
+                                + " & ".join(cell_format.format(
+                                    r"\textbf{" + str(x or self.global_group_name) + r"}")
                                              for x in x_categories)
                                 + " \\\\\n")
                             latex_file.write("\\toprule\n")
 
                             # Write data rows
                             for y_category in y_categories:
                                 latex_file.write(row_header_format.format(
@@ -3391,15 +3438,16 @@
                                                     summary_dict[(x_category, y_category)])
                                                 + ("}" if highlight else "")))
                                     except KeyError:
                                         latex_file.write(" & " + " " * longest_cell_length)
                                 latex_file.write(" \\\\\n")
                             if summary_table.show_global_row and len(y_categories) > 1:
                                 latex_file.write("\\midrule\n")
-                                latex_file.write(row_header_format.format(f"\\textbf{{{self.global_group_name}}}"))
+                                latex_file.write(row_header_format.format(
+                                    f"\\textbf{{{self.global_group_name}}}"))
                                 for x_category in x_categories:
                                     highlight = self.should_highlight_cell(
                                         summary_dict=summary_dict, summary_table=summary_table,
                                         x_categories=x_categories, x_category=x_category,
                                         y_categories=y_categories, y_category=None)
                                     try:
                                         latex_file.write(
@@ -3600,27 +3648,29 @@
         # Add the (x,y) cell values
         for (x_category, y_category), split_df in full_df.groupby([x_column, y_column]):
             if _self.x_header_list and str(x_category) not in _self.x_header_list:
                 continue
             if _self.y_header_list and str(y_category) not in _self.y_header_list:
                 continue
             for stat, value in _self.numeric_series_to_stat_dict(split_df[data_column]).items():
-                row[f"{x_column}_{y_column}_{data_column}_{stat}"][(str(x_category), str(y_category))] = value
+                row[f"{x_column}_{y_column}_{data_column}_{stat}"][
+                    (str(x_category), str(y_category))] = value
 
         # Add the "All" row
         if _self.show_global_row:
             # If a list of y categories is specified, only those are used for the global row "All"
             if _self.y_header_list:
                 global_df = full_df[full_df[y_column].apply(str).isin(_self.y_header_list)]
             else:
                 global_df = full_df
 
             for x_category, split_df in global_df.groupby(x_column):
                 for stat, value in _self.numeric_series_to_stat_dict(split_df[data_column]).items():
-                    row[f"{x_column}_{y_column}_{data_column}_{stat}"][(str(x_category), None)] = value
+                    row[f"{x_column}_{y_column}_{data_column}_{stat}"][
+                        (str(x_category), None)] = value
 
         # Add the "All" column
         if _self.show_global_column:
             # If a list of x categories is specified, only those are used for the global column "All"
             if _self.x_header_list:
                 global_df = full_df[full_df[x_column].apply(str).isin(_self.x_header_list)]
             else:
```

### Comparing `enb-1.0.2/enb/atable.py` & `enb-1.0.3/enb/atable.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/config/__init__.py` & `enb-1.0.3/enb/config/__init__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/config/aini.py` & `enb-1.0.3/enb/config/aini.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/config/aoptions.py` & `enb-1.0.3/enb/config/aoptions.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/config/contrib_sha256.csv` & `enb-1.0.3/enb/config/contrib_sha256.csv`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 file,sha256
 cfitsio-3.49.tar.gz,8c3a8ed1a3577c0036cd0ddeaee881953c6801c981d2937b6a60b303b7d2d5fb
+emporda_20240419.zip,f2a6777decb6be8c525be9ba0723abd22a036f77f303ea4a5e8ca64394437f86
 flif_0.3_2017.zip,14161b4d49e2c53691117361a5344ca69d982212bd5a1d343b33f1294895afa5
 fpzip-1.3.0.tar.gz,248df7d84259e3feaa4c4797956b2a77c3fcd734e8f8fdc51ce171dcf4f0136c
 fse_git.zip,75de8836f4f932b93feefaa41d80a543039e80edf4ffbe196d2d7ad26920aff7
 HM-master.zip,53846388572596910e4577e218e987a7d429bf9091e51bb4a524f2661d03b006
 jpegxl_git.zip,49858126381419794317d928416a2087f36872298247074312e9171115c6afd2
+lc-framework.zip,b49387e6f91e34b4862150b276c5b6e3b5db001a8e7062317e690f34223ba600
 libjpeg-master-1.59.zip,2cf73babbec228705e01d14a1f5fd3958a16639419edf6cf1bdc6d0dfadbe413
 lz4-1.9.2.zip,0b8bf249fd54a0b974de1a50f0a13ba809a78fd48f90c465c240ee28a9e4784d
 marlin_ubuntu20_git.zip,c5a368cf98ac694a0cb0884c53718a33145f261d9a6929153fddd7eb257bb371
 nayuki_arithmetic_coder_reference.zip,0b9e332e9cdd234773cc63a945bdf03e7603cc7eedc259d5ba8159ba53faeecd
 ndzip-master-enb.zip,0459096eb8e780c492921f235e0fbbe025076411188f2a214c036129ff8ab571
 SPModule_20220804.zip,7eb56af65a8b1ca08fba6242fcf38100eb8b8bcf2cbbd1c71af91fd1d3d32fa8
 VVCSoftware_VTM-master.zip,8c64e84d0cf626cc78b1ec09f649e713180784887dfff9cb90f1291cd5b82b69
```

### Comparing `enb-1.0.2/enb/config/enb.ini` & `enb-1.0.3/enb/config/enb.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # General variables related to the enb project itself, passed to the setup() method.
 [enb]
 name = enb
 description = Experiment NoteBook (%(name)s): efficient and reproducible science.
-version = 1.0.2
+version = 1.0.3
 url = https://github.com/miguelinux314/experiment-notebook
 download_url = https://github.com/miguelinux314/experiment-notebook/archive/v%(version)s.tar.gz
 license = MIT License
 author = Miguel Hernández Cabronero, et al.
 author_email = miguel.hernandez@uab.cat
 platforms = any
 python_requires = >=3.7
```

### Comparing `enb-1.0.2/enb/config/singleton_cli.py` & `enb-1.0.3/enb/config/singleton_cli.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/experiment.py` & `enb-1.0.3/enb/experiment.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/fits.py` & `enb-1.0.3/enb/fits.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/icompression.py` & `enb-1.0.3/enb/icompression.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/isets.py` & `enb-1.0.3/enb/isets.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/log.py` & `enb-1.0.3/enb/log.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/misc.py` & `enb-1.0.3/enb/misc.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/parallel.py` & `enb-1.0.3/enb/parallel.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/parallel_ray.py` & `enb-1.0.3/enb/parallel_ray.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/pgm.py` & `enb-1.0.3/enb/pgm.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plotdata.py` & `enb-1.0.3/enb/plotdata.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/__init__.py` & `enb-1.0.3/enb/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/installable.py` & `enb-1.0.3/enb/plugins/installable.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,18 +177,30 @@
                 shutil.copyfile(cached_path, output_path)
 
             # Custom building of the Installable
             print(f"Building plugin {repr(cls.name)} into {repr(installation_dir)}...")
             cls.build(installation_dir=installation_dir)
             cls.report_successful_installation(installation_dir=installation_dir)
         except Exception as ex:
+            enb.logger.error(f"{ex}")
             if not installation_dir_existed:
-                enb.logger.verbose(f"Removing incomplete installation dir {repr(installation_dir)}.")
+                copy_dir = os.path.abspath(os.path.join(
+                    enb.config.options.base_tmp_dir, os.path.basename(installation_dir)))
+                shutil.rmtree(copy_dir, ignore_errors=True)
+                shutil.copytree(installation_dir, copy_dir)
+                enb.logger.warn(f"Removing incomplete installation dir {repr(installation_dir)}.\n"
+                                 f"A copy has been made into {repr(copy_dir)} in case you want "
+                                 f"to attempt manual building of the plugin.\n"
+                                 f"You would then need to copy that folder into "
+                                f"{repr(installation_dir)} to complete the installation.")
                 shutil.rmtree(installation_dir, ignore_errors=True)
-            raise ex
+            else:
+                enb.logger.warn(f"The destination dir {repr(installation_dir)} already existed, "
+                                "so the incomplete installation files have to be manually removed "
+                                "if needed.")
 
     @classmethod
     def build(cls, installation_dir):
         """Method called after the main installation body, that allows further building customization
         by Installable subclasses. By default, nothing is done.
 
         Note that the installation dir is created before calling build.
```

### Comparing `enb-1.0.2/enb/plugins/plugin.py` & `enb-1.0.3/enb/plugins/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import os
 import glob
 import inspect
 import shutil
 import platform
 import subprocess
+import textwrap
 import enb
 
 from .installable import Installable
 
 
 class Plugin(Installable):
     """Plugins are self-contained, python modules that may assume enb is installed.
@@ -138,17 +139,17 @@
                                 "Makefile.")
         if os.path.exists(make_path):
             invocation = (f"cd {os.path.dirname(os.path.abspath(make_path))} "
                           f"&& {shutil.which('make')} -f {os.path.basename(make_path)}")
             status, output = subprocess.getstatusoutput(invocation)
             if status != 0:
                 raise Exception(f"Error building plugin {repr(cls.name)} with "
-                                f"the Makefile at {make_path}!\n\n"
-                                f"Status = {status} != 0.\n"
-                                f"Input=[{invocation}].\nOutput=[{output}]")
+                                f"the Makefile at {make_path} ({status=})!\n"
+                                f"Failing command:\n{textwrap.indent(invocation, ' '*3)}\n"
+                                f"Output:\n{textwrap.indent(output, ' '*3)}")
         else:
             raise ValueError(f"Cannot build {repr(cls.name)}: no valid makefile "
                              f"in {installation_dir}.")
 
 
 class PluginJava(Plugin):
     @classmethod
```

### Comparing `enb-1.0.2/enb/plugins/plugin_ac/__plugin__.py` & `enb-1.0.3/enb/plugins/plugin_ac/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_ac/arithmetic_codec.py` & `enb-1.0.3/enb/plugins/plugin_ac/arithmetic_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_bwt/COPYING` & `enb-1.0.3/enb/plugins/plugin_bwt/COPYING`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_bwt/COPYING.LESSER` & `enb-1.0.3/enb/plugins/plugin_bwt/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_bwt/Makefile` & `enb-1.0.3/enb/plugins/plugin_bwt/Makefile`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_bwt/README` & `enb-1.0.3/enb/plugins/plugin_bwt/README`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_bwt/__plugin__.py` & `enb-1.0.3/enb/plugins/plugin_bwt/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_bwt/bwt_codec.py` & `enb-1.0.3/enb/plugins/plugin_bwt/bwt_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_bwt/bwxform.c` & `enb-1.0.3/enb/plugins/plugin_bwt/bwxform.c`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_bwt/bwxform.h` & `enb-1.0.3/enb/plugins/plugin_bwt/bwxform.h`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_bwt/optlist/COPYING` & `enb-1.0.3/enb/plugins/plugin_bwt/optlist/COPYING`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_bwt/optlist/COPYING.LESSER` & `enb-1.0.3/enb/plugins/plugin_bwt/optlist/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_bwt/optlist/Makefile` & `enb-1.0.3/enb/plugins/plugin_bwt/optlist/Makefile`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_bwt/optlist/README` & `enb-1.0.3/enb/plugins/plugin_bwt/optlist/README`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_bwt/optlist/optlist.c` & `enb-1.0.3/enb/plugins/plugin_bwt/optlist/optlist.c`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_bwt/optlist/optlist.h` & `enb-1.0.3/enb/plugins/plugin_bwt/optlist/optlist.h`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_bwt/optlist/sample.c` & `enb-1.0.3/enb/plugins/plugin_bwt/optlist/sample.c`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_bwt/optlist/sample.cpp` & `enb-1.0.3/enb/plugins/plugin_bwt/optlist/sample.cpp`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_bwt/sample.c` & `enb-1.0.3/enb/plugins/plugin_bwt/sample.c`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_ccsds122/ccsds122_codec.py` & `enb-1.0.3/enb/plugins/plugin_ccsds122/ccsds122_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_ccsds124/ccsds124_codecs.py` & `enb-1.0.3/enb/plugins/plugin_ccsds124/ccsds124_codecs.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_emporda/emporda_codec.py` & `enb-1.0.3/enb/plugins/plugin_hevc/hevc_codec.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,135 @@
 #!/usr/bin/env python3
-"""Codec wrapper for the emporda software (https://gici.uab.cat/GiciWebPage/downloads.php#emporda)
+"""Wrapper for the HEVC codec, using the reference implementation from
+
+https://vcgit.hhi.fraunhofer.de/jvet/HM
 """
-__author__ = "Miguel Hernández-Cabronero"
-__since__ = "2022/04/08"
+__author__ = "Natalia Blasco, Ester Jara, Artemis Llabrés and Miguel Hernández-Cabronero"
+__since__ = "2021/09/01"
 
 import os
-import enb.icompression
-import shutil
+import math
+from enb import icompression
+
+
+class HEVC(icompression.LittleEndianWrapper):
+    default_qp = 0
+
+    """
+    Base class for HEVC coder
+    """
+
+    def __init__(self, config_path, chroma_format="400", qp=None):
+        """
+        :param chroma_format: Specifies the chroma format used in the input file (only 400 supported).
+        :param qp: Specifies the base value of the quantization parameter (0-51).
+        """
+        chroma_format = str(chroma_format)
+        assert chroma_format in ["400"], f"Chroma format {chroma_format} not supported."
+        qp = int(qp) if qp is not None else self.default_qp
+        assert 0 <= qp <= 51
+
+        param_dict = dict(chroma_format=chroma_format, QP=qp)
+
+        icompression.WrapperCodec.__init__(
+            self,
+            compressor_path=os.path.join(os.path.dirname(
+                os.path.abspath(__file__)), "TAppEncoderStatic"),
+            decompressor_path=os.path.join(os.path.dirname(
+                os.path.abspath(__file__)), "TAppDecoderStatic"),
+            param_dict=param_dict)
+
+        self.config_path = config_path
+
+    def get_compression_params(self, original_path, compressed_path, original_file_info):
+        if original_file_info["float"]:
+            raise ValueError("This codec does not support floating point data")
+
+        return f"-i {original_path} " \
+               f"-c {self.config_path} " \
+               f"-b {compressed_path} " \
+               f"-wdt {original_file_info['width']} " \
+               f"-hgt {original_file_info['height']} " \
+               f"-f {original_file_info['component_count']} " \
+               f"-cf {self.param_dict['chroma_format']} " \
+               f"--InputChromaFormat={self.param_dict['chroma_format']} " \
+               f"--InputBitDepth={8 * original_file_info['bytes_per_sample']} "
+
+    def get_decompression_params(self, compressed_path, reconstructed_path, original_file_info):
+        return f"-b {compressed_path} " \
+               f"-o {reconstructed_path} " \
+               f"-d {8 * original_file_info['bytes_per_sample']}"
+
+    @property
+    def label(self):
+        raise NotImplementedError("Subclasses must implement their own label.")
+
 
+class HEVC_lossless(icompression.LosslessCodec, HEVC):
+    """
+    HEVC subclass for lossless compression
+    """
 
-class Emporda(enb.icompression.LosslessCodec, enb.icompression.NearLosslessCodec,
-              enb.icompression.JavaWrapperCodec, enb.icompression.GiciLibHelper):
-    """Wrapper for the emporda codec (https://gici.uab.cat/GiciWebPage/downloads.php#emporda)
-    """
-
-    def __init__(self,
-                 compressor_jar=os.path.join(os.path.dirname(__file__), "emporda.jar"),
-                 decompressor_jar=os.path.join(os.path.dirname(__file__), "emporda.jar"),
-                 qs=0, ec=1, cm=1, pm=0, wp=2048, up=2):
-        """
-        :param qs: sets the quantization step.
-        :param ec: The encoder type that will encode the image.
-            0.- Lossless without predictor + entropy encoder.
-            1.- Lossless with predictor + entropy encoder.
-            2.- Lossless and near-lossless with predictor predictor + entropy encoder.
-            3.- Lossless and near-lossless with state-of-the-art predictor + entropy encoder.
-        :param cm: context model
-            0.- No context model is used.
-            1.- Context modelling is used during the encoding process.
-        :param pm: Probability model employed for the entropy coder.
-            0.- The probability is estimated using a full division operation.
-            1.- The probability is estimated using a division implemented through a quantized Look Up Table.
-                This option must be used with -qlut option.
-            2.- The probability is estimated using only bitwise operators and witout division.
-                When this option is used -wp and -up parameters must be the same value of form 2^X.
-        :param wp: Indicates the maximum number of symbols within the variable-size sliding windows
-          that are employed for the Entropy Coder to compute the probability of the context.
-          Must be of the form 2^X.
-        :param up: Indicates the number of symbols coded before updating the context probability in the Entropy Coder.
-            Must be of the form 2^X.
-        """
-        assert shutil.which("java") is not None, \
-            f"The 'java' program was not found in the path, but is required by {self.__class__.__name__}. " \
-            f"Please (re)install a JRE in the path and try again."
-        super().__init__(compressor_jar=compressor_jar,
-                         decompressor_jar=decompressor_jar,
-                         param_dict=dict(qs=qs, ec=ec, cm=cm, pm=pm, wp=wp, up=up))
+    def __init__(self, config_path=None, chroma_format="400"):
+        """
+        :param chroma_format: Specifies the chroma format used in the input file
+        (only 400 supported).
+        """
+        config_path = config_path if config_path is not None \
+            else os.path.join(os.path.dirname(os.path.abspath(__file__)),
+                              f"hevc_lossless_{chroma_format}.cfg")
+        HEVC.__init__(self, config_path, chroma_format, qp=0)
 
     @property
     def label(self):
-        return "Emporda"
+        return "HEVC lossless"
+
+
+class HEVC_lossy(icompression.LossyCodec, HEVC):
+    """
+    HEVC subclass for lossy compression
+    """
+
+    rate_decimals = 3
+
+    def __init__(self, config_path=None, chroma_format="400", qp=25, bit_rate=None):
+        """
+        :param chroma_format: Specifies the chroma format used in the input file
+          (only 400 supported).
+        :param qp: Specifies the base value of the quantization parameter (0-51).
+        :param bit_rate: target bitrate in bps.
+        """
+        bit_rate = round(float(bit_rate), self.rate_decimals) if bit_rate is not None else bit_rate
+
+        config_path = config_path if config_path is not None \
+            else os.path.join(os.path.dirname(os.path.abspath(__file__)),
+                              f"hevc_lossy_{chroma_format}.cfg")
+        HEVC.__init__(
+            self, config_path=config_path, chroma_format=chroma_format, qp=qp)
+
+        self.param_dict['bit_rate'] = bit_rate
 
     def get_compression_params(self, original_path, compressed_path, original_file_info):
-        assert original_file_info["bytes_per_sample"] == 2, \
-            f"Only 16-bit samples are currently supported by {self.__class__.__name__}"
-        assert not original_file_info["float"], \
-            f"Only integer samples are currently supported by {self.__class__.__name__}"
-        assert original_file_info["big_endian"], \
-            f"Only big-endian samples are currently supported by {self.__class__.__name__}"
-
-        return f"-Xmx256g -jar {self.compressor_jar} -c -i {original_path} -o {compressed_path} " \
-               f"-ig {self.get_gici_geometry_str(original_file_info=original_file_info)} " \
-               f"-qs {self.param_dict['qs']} " \
-               f"-ec {self.param_dict['ec']} " \
-               f"-cm {self.param_dict['cm']} " \
-               f"-pm {self.param_dict['pm']} " \
-               f"-wp {self.param_dict['wp']} " \
-               f"-up {self.param_dict['up']}"
+        params = super().get_compression_params(
+            original_path=original_path,
+            compressed_path=compressed_path,
+            original_file_info=original_file_info)
+
+        if self.param_dict['bit_rate'] is not None:
+            target_rate = math.ceil(self.param_dict['bit_rate']
+                                    * original_file_info['width'] * original_file_info['height'])
+            params += " --RateControl "
+            params += f" --TargetBitrate={target_rate} "
+        else:
+            params += f" --QP={self.param_dict['QP']} --InitialQP={self.param_dict['QP']}"
 
-    def get_decompression_params(self, compressed_path, reconstructed_path, original_file_info):
-        assert original_file_info["bytes_per_sample"] == 2, \
-            f"Only 16-bit samples are currently supported by {self.__class__.__name__}"
-        assert not original_file_info["float"], \
-            f"Only integer samples are currently supported by {self.__class__.__name__}"
-        assert original_file_info["big_endian"], \
-            f"Only big-endian samples are currently supported by {self.__class__.__name__}"
-        
-        return f"-Xmx256g -jar {self.decompressor_jar} -d -i {compressed_path} -o {reconstructed_path} " \
-               f"-ig {self.get_gici_geometry_str(original_file_info=original_file_info)} " \
-               f"-qs {self.param_dict['qs']} " \
-               f"-ec {self.param_dict['ec']} " \
-               f"-cm {self.param_dict['cm']} " \
-               f"-pm {self.param_dict['pm']} " \
-               f"-wp {self.param_dict['wp']} " \
-               f"-up {self.param_dict['up']}"
+        return params
+
+    @property
+    def label(self):
+        if self.param_dict["bit_rate"] is not None:
+            rate_format = "{0:." + str(self.rate_decimals) + "f}"
+            s = f"HEVC {rate_format.format(self.param_dict['bit_rate'])}bps"
+        else:
+            s = f"HEVC QP{self.param_dict['QP']}"
+
+        return s
```

### Comparing `enb-1.0.2/enb/plugins/plugin_fapec/fapec_codec.py` & `enb-1.0.3/enb/plugins/plugin_fapec/fapec_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_flif/Makefile.darwin` & `enb-1.0.3/enb/plugins/plugin_flif/Makefile.darwin`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_flif/Makefile.linux` & `enb-1.0.3/enb/plugins/plugin_flif/Makefile.linux`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_flif/README.md` & `enb-1.0.3/enb/plugins/plugin_flif/README.md`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_flif/__plugin__.py` & `enb-1.0.3/enb/plugins/plugin_flif/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_flif/flif_codec.py` & `enb-1.0.3/enb/plugins/plugin_flif/flif_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_fpack/__plugin__.py` & `enb-1.0.3/enb/plugins/plugin_fpack/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_fpack/fpack_codec.py` & `enb-1.0.3/enb/plugins/plugin_fpack/fpack_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_fpc/README.md` & `enb-1.0.3/enb/plugins/plugin_fpc/README.md`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_fpc/fpc.c` & `enb-1.0.3/enb/plugins/plugin_fpc/fpc.c`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_fpc/fpc_codec.py` & `enb-1.0.3/enb/plugins/plugin_fpc/fpc_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_fpzip/README.md` & `enb-1.0.3/enb/plugins/plugin_fpzip/README.md`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_fpzip/fpzip_codec.py` & `enb-1.0.3/enb/plugins/plugin_fpzip/fpzip_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_fse_huffman/Makefile.linux` & `enb-1.0.3/enb/plugins/plugin_fse_huffman/Makefile.linux`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_fse_huffman/README.md` & `enb-1.0.3/enb/plugins/plugin_fse_huffman/README.md`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_fse_huffman/fse_codec.py` & `enb-1.0.3/enb/plugins/plugin_fse_huffman/fse_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_fse_huffman/huffman_codec.py` & `enb-1.0.3/enb/plugins/plugin_fse_huffman/huffman_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_hdf5/hdf5_codecs.py` & `enb-1.0.3/enb/plugins/plugin_hdf5/hdf5_codecs.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_hevc/Makefile.darwin` & `enb-1.0.3/enb/plugins/plugin_hevc/Makefile.darwin`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_hevc/Makefile.linux` & `enb-1.0.3/enb/plugins/plugin_hevc/Makefile.linux`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_hevc/README.md` & `enb-1.0.3/enb/plugins/plugin_hevc/README.md`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_hevc/__plugin__.py` & `enb-1.0.3/enb/plugins/plugin_hevc/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_hevc/hevc_codec.py` & `enb-1.0.3/enb/plugins/plugin_zstandard/zstd_codec.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,135 +1,108 @@
 #!/usr/bin/env python3
-"""Wrapper for the HEVC codec, using the reference implementation from
-
-https://vcgit.hhi.fraunhofer.de/jvet/HM
+"""Codec wrapper for the Zstandard lossless image coder
 """
-__author__ = "Natalia Blasco, Ester Jara, Artemis Llabrés and Miguel Hernández-Cabronero"
-__since__ = "2021/09/01"
+__author__ = "Miguel Hernández-Cabronero"
+__since__ = "2021/07/12"
 
 import os
-import math
-from enb import icompression
-
-
-class HEVC(icompression.LittleEndianWrapper):
-    default_qp = 0
-
-    """
-    Base class for HEVC coder
-    """
-
-    def __init__(self, config_path, chroma_format="400", qp=None):
-        """
-        :param chroma_format: Specifies the chroma format used in the input file (only 400 supported).
-        :param qp: Specifies the base value of the quantization parameter (0-51).
-        """
-        chroma_format = str(chroma_format)
-        assert chroma_format in ["400"], f"Chroma format {chroma_format} not supported."
-        qp = int(qp) if qp is not None else self.default_qp
-        assert 0 <= qp <= 51
-
-        param_dict = dict(chroma_format=chroma_format, QP=qp)
-
-        icompression.WrapperCodec.__init__(
-            self,
-            compressor_path=os.path.join(os.path.dirname(
-                os.path.abspath(__file__)), "TAppEncoderStatic"),
-            decompressor_path=os.path.join(os.path.dirname(
-                os.path.abspath(__file__)), "TAppDecoderStatic"),
-            param_dict=param_dict)
-
-        self.config_path = config_path
-
-    def get_compression_params(self, original_path, compressed_path, original_file_info):
-        if original_file_info["float"]:
-            raise ValueError("This codec does not support floating point data")
-
-        return f"-i {original_path} " \
-               f"-c {self.config_path} " \
-               f"-b {compressed_path} " \
-               f"-wdt {original_file_info['width']} " \
-               f"-hgt {original_file_info['height']} " \
-               f"-f {original_file_info['component_count']} " \
-               f"-cf {self.param_dict['chroma_format']} " \
-               f"--InputChromaFormat={self.param_dict['chroma_format']} " \
-               f"--InputBitDepth={8 * original_file_info['bytes_per_sample']} "
-
-    def get_decompression_params(self, compressed_path, reconstructed_path, original_file_info):
-        return f"-b {compressed_path} " \
-               f"-o {reconstructed_path} " \
-               f"-d {8 * original_file_info['bytes_per_sample']}"
+import enb
+from enb import tarlite
+import tempfile
+import subprocess
 
-    @property
-    def label(self):
-        raise NotImplementedError("Subclasses must implement their own label.")
-
-
-class HEVC_lossless(icompression.LosslessCodec, HEVC):
-    """
-    HEVC subclass for lossless compression
+class Zstandard(enb.icompression.LosslessCodec, enb.icompression.NearLosslessCodec, enb.fits.FITSWrapperCodec):
+    """Wrapper for the Zstandard codec
+    All data types integer and float 16, 32, 64 can be compressed
     """
 
-    def __init__(self, config_path=None, chroma_format="400"):
+    def __init__(self, compression_level=19, zstd_binary=os.path.join(os.path.dirname(__file__), "zstd")):
         """
-        :param chroma_format: Specifies the chroma format used in the input file
-        (only 400 supported).
+        :param compression_level: 1-22, being 22 the maximum data reduction
         """
-        config_path = config_path if config_path is not None \
-            else os.path.join(os.path.dirname(os.path.abspath(__file__)),
-                              f"hevc_lossless_{chroma_format}.cfg")
-        HEVC.__init__(self, config_path, chroma_format, qp=0)
+        assert 1 <= int(compression_level) <= 22, f"Invalid compression level {compression_level}"
+        super().__init__(compressor_path=zstd_binary,
+                         decompressor_path=zstd_binary,
+                         param_dict=dict(compression_level=compression_level))
 
     @property
     def label(self):
-        return "HEVC lossless"
-
+        return f"Zstandard {self.param_dict['compression_level']}"
 
-class HEVC_lossy(icompression.LossyCodec, HEVC):
-    """
-    HEVC subclass for lossy compression
-    """
-
-    rate_decimals = 3
-
-    def __init__(self, config_path=None, chroma_format="400", qp=25, bit_rate=None):
+    def assert_valid_data_type(self, original_file_info):
+        """Verify that the input data type is supported, else raise an exception
         """
-        :param chroma_format: Specifies the chroma format used in the input file
-          (only 400 supported).
-        :param qp: Specifies the base value of the quantization parameter (0-51).
-        :param bit_rate: target bitrate in bps.
-        """
-        bit_rate = round(float(bit_rate), self.rate_decimals) if bit_rate is not None else bit_rate
+        assert not original_file_info["float"], f"Only integer samples are supported by {self.__class__.__name__}"
+        assert original_file_info["big_endian"], f"Only big-endian samples are supported by {self.__class__.__name__}"
 
-        config_path = config_path if config_path is not None \
-            else os.path.join(os.path.dirname(os.path.abspath(__file__)),
-                              f"hevc_lossy_{chroma_format}.cfg")
-        HEVC.__init__(
-            self, config_path=config_path, chroma_format=chroma_format, qp=qp)
+    def get_compression_params(self, original_path, compressed_path, original_file_info):
+        self.assert_valid_data_type(original_file_info=original_file_info)
+        return f"-{self.param_dict['compression_level']} " \
+               f"{'--ultra ' if self.param_dict['compression_level'] > 19 else ''}" \
+               f"-f {original_path}  -o {compressed_path}"
 
-        self.param_dict['bit_rate'] = bit_rate
+    def get_decompression_params(self, compressed_path, reconstructed_path, original_file_info):
+        return f"-d  -f {compressed_path} -o {reconstructed_path}"
 
-    def get_compression_params(self, original_path, compressed_path, original_file_info):
-        params = super().get_compression_params(
-            original_path=original_path,
-            compressed_path=compressed_path,
-            original_file_info=original_file_info)
-
-        if self.param_dict['bit_rate'] is not None:
-            target_rate = math.ceil(self.param_dict['bit_rate']
-                                    * original_file_info['width'] * original_file_info['height'])
-            params += " --RateControl "
-            params += f" --TargetBitrate={target_rate} "
-        else:
-            params += f" --QP={self.param_dict['QP']} --InitialQP={self.param_dict['QP']}"
 
-        return params
+class Zstandard_train(Zstandard):
+    """Wrapper for the Zstandard codec, which produces a dictionary file for the input data and then employs
+    it for compression. The generated dictionary is included in the compressed data size measurements.
+
+    All data types integer and float 16, 32, 64 can be compressed
+    """
+
+    def assert_valid_data_type(self, original_file_info):
+        """Verify that the input data type is supported, else raise an exception
+        """
+        super().assert_valid_data_type(original_file_info=original_file_info)
+        assert original_file_info["bytes_per_sample"] == 4, \
+            f"Only 32-bit samples are supported by {self.__class__.__name__}"
+
+    def compress(self, original_path, compressed_path, original_file_info):
+        self.assert_valid_data_type(original_file_info=original_file_info)
+
+        with tempfile.TemporaryDirectory(dir=enb.config.options.base_tmp_dir) as tmp_dir:
+            dict_path = os.path.join(tmp_dir, "dict.zstd")
+            dict_compressed_path = os.path.join(tmp_dir, "compressed.zstd")
+
+            # Generate dictionary
+            invocation = f"{self.compressor_path} --train {original_path} --optimize-cover -o {dict_path}"
+            status, output = subprocess.getstatusoutput(invocation)
+            if status != 0:
+                raise Exception(f"Status = {status} != 0.\n"
+                                f"Input=[{invocation}].\n"
+                                f"Output=[{output}]")
+
+            # Compress using that dictionary
+            invocation = f" {self.compressor_path} " \
+                         f"{'--ultra ' if int(self.param_dict['compression_level']) > 19 else ''}" \
+                         f"-{self.param_dict['compression_level']} -D {dict_path} -f {original_path} " \
+                         f"-o {dict_compressed_path}"
+            status, output = subprocess.getstatusoutput(invocation)
+            if status != 0:
+                raise Exception(f"Status = {status} != 0.\n"
+                                f"Input=[{invocation}].\n"
+                                f"Output=[{output}]")
+
+            # Unite the compressed data and the side information
+            tarlite.tarlite_files(input_paths=(dict_path, dict_compressed_path), output_tarlite_path=compressed_path)
+
+    def decompress(self, compressed_path, reconstructed_path, original_file_info):
+        with tempfile.TemporaryDirectory(dir=enb.config.options.base_tmp_dir) as tmp_dir:
+            dict_path = os.path.join(tmp_dir, "dict.zstd")
+            dict_compressed_path = os.path.join(tmp_dir, "compressed.zstd")
+
+            # Separate the compressed data from the side information
+            tarlite.untarlite_files(input_tarlite_path=compressed_path, output_dir_path=tmp_dir)
+
+            # Decompress
+            invocation = f"{self.compressor_path} -d -D {dict_path} -f {dict_compressed_path} -o {reconstructed_path}"
+            status, output = subprocess.getstatusoutput(invocation)
+            if status != 0:
+                raise Exception(f"Status = {status} != 0.\n"
+                                f"Input=[{invocation}].\n"
+                                f"Output=[{output}]")
 
     @property
     def label(self):
-        if self.param_dict["bit_rate"] is not None:
-            rate_format = "{0:." + str(self.rate_decimals) + "f}"
-            s = f"HEVC {rate_format.format(self.param_dict['bit_rate'])}bps"
-        else:
-            s = f"HEVC QP{self.param_dict['QP']}"
-
-        return s
+        return f"Zstandard pretrain {self.param_dict['compression_level']}"
```

### Comparing `enb-1.0.2/enb/plugins/plugin_hevc/hevc_lossless_400.cfg` & `enb-1.0.3/enb/plugins/plugin_hevc/hevc_lossless_400.cfg`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_hevc/hevc_lossy_400.cfg` & `enb-1.0.3/enb/plugins/plugin_hevc/hevc_lossy_400.cfg`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_huffman_nayuki/AdaptiveHuffmanCompress.cpp` & `enb-1.0.3/enb/plugins/plugin_huffman_nayuki/AdaptiveHuffmanCompress.cpp`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_huffman_nayuki/AdaptiveHuffmanDecompress.cpp` & `enb-1.0.3/enb/plugins/plugin_huffman_nayuki/AdaptiveHuffmanDecompress.cpp`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_huffman_nayuki/BitIoStream.cpp` & `enb-1.0.3/enb/plugins/plugin_huffman_nayuki/BitIoStream.cpp`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_huffman_nayuki/BitIoStream.hpp` & `enb-1.0.3/enb/plugins/plugin_huffman_nayuki/BitIoStream.hpp`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_huffman_nayuki/CanonicalCode.cpp` & `enb-1.0.3/enb/plugins/plugin_huffman_nayuki/CanonicalCode.cpp`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_huffman_nayuki/CanonicalCode.hpp` & `enb-1.0.3/enb/plugins/plugin_huffman_nayuki/CanonicalCode.hpp`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_huffman_nayuki/CodeTree.cpp` & `enb-1.0.3/enb/plugins/plugin_huffman_nayuki/CodeTree.cpp`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_huffman_nayuki/CodeTree.hpp` & `enb-1.0.3/enb/plugins/plugin_huffman_nayuki/CodeTree.hpp`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_huffman_nayuki/FrequencyTable.cpp` & `enb-1.0.3/enb/plugins/plugin_huffman_nayuki/FrequencyTable.cpp`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_huffman_nayuki/FrequencyTable.hpp` & `enb-1.0.3/enb/plugins/plugin_huffman_nayuki/FrequencyTable.hpp`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_huffman_nayuki/HuffmanCoder.cpp` & `enb-1.0.3/enb/plugins/plugin_huffman_nayuki/HuffmanCoder.cpp`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_huffman_nayuki/HuffmanCoder.hpp` & `enb-1.0.3/enb/plugins/plugin_huffman_nayuki/HuffmanCoder.hpp`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_huffman_nayuki/HuffmanCompress.cpp` & `enb-1.0.3/enb/plugins/plugin_huffman_nayuki/HuffmanCompress.cpp`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_huffman_nayuki/HuffmanDecompress.cpp` & `enb-1.0.3/enb/plugins/plugin_huffman_nayuki/HuffmanDecompress.cpp`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_huffman_nayuki/Makefile.linux` & `enb-1.0.3/enb/plugins/plugin_huffman_nayuki/Makefile.linux`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_huffman_nayuki/huffman_codec.py` & `enb-1.0.3/enb/plugins/plugin_huffman_nayuki/huffman_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_iraf_photometry/__plugin__.py` & `enb-1.0.3/enb/plugins/plugin_iraf_photometry/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_iraf_photometry/iraf_photometry.py` & `enb-1.0.3/enb/plugins/plugin_iraf_photometry/iraf_photometry.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_iraf_photometry/iraf_photometry_slave.py` & `enb-1.0.3/enb/plugins/plugin_iraf_photometry/iraf_photometry_slave.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_jpeg/jpeg_codecs.py` & `enb-1.0.3/enb/plugins/plugin_jpeg/jpeg_codecs.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_jpeg_xl/Makefile.darwin` & `enb-1.0.3/enb/plugins/plugin_jpeg_xl/Makefile.darwin`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_jpeg_xl/Makefile.linux` & `enb-1.0.3/enb/plugins/plugin_jpeg_xl/Makefile.linux`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_jpeg_xl/README.md` & `enb-1.0.3/enb/plugins/plugin_jpeg_xl/README.md`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_jpeg_xl/__plugin__.py` & `enb-1.0.3/enb/plugins/plugin_jpeg_xl/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_jpeg_xl/jpegxl_codec.py` & `enb-1.0.3/enb/plugins/plugin_jpeg_xl/jpegxl_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_kakadu/README.md` & `enb-1.0.3/enb/plugins/plugin_kakadu/README.md`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_kakadu/kakadu_codec.py` & `enb-1.0.3/enb/plugins/plugin_kakadu/kakadu_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_lcnl/__plugin__.py` & `enb-1.0.3/enb/plugins/plugin_lcnl/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_lcnl/lcnl_codecs.py` & `enb-1.0.3/enb/plugins/plugin_lcnl/lcnl_codecs.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_lpaq8/lpaq8.cpp` & `enb-1.0.3/enb/plugins/plugin_lpaq8/lpaq8.cpp`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_lpaq8/lpaq8_codec.py` & `enb-1.0.3/enb/plugins/plugin_lpaq8/lpaq8_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_lpaq8/readme.txt` & `enb-1.0.3/enb/plugins/plugin_lpaq8/readme.txt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_lz4/README.txt` & `enb-1.0.3/enb/plugins/plugin_lz4/README.txt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_lz4/lz4_codec.py` & `enb-1.0.3/enb/plugins/plugin_lz4/lz4_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_marlin/Makefile.linux` & `enb-1.0.3/enb/plugins/plugin_marlin/Makefile.linux`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_marlin/__plugin__.py` & `enb-1.0.3/enb/plugins/plugin_marlin/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_marlin/marlin_codec.py` & `enb-1.0.3/enb/plugins/plugin_marlin/marlin_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_mcalic/README.txt` & `enb-1.0.3/enb/plugins/plugin_mcalic/README.txt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_mcalic/__plugin__.py` & `enb-1.0.3/enb/plugins/plugin_mcalic/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_mcalic/mcalic_codecs.py` & `enb-1.0.3/enb/plugins/plugin_mcalic/mcalic_codecs.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_mhdc_transforms/abstract_mhdc_transform.py` & `enb-1.0.3/enb/plugins/plugin_mhdc_transforms/abstract_mhdc_transform.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_mhdc_transforms/iwt.py` & `enb-1.0.3/enb/plugins/plugin_mhdc_transforms/iwt.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_mhdc_transforms/pot.py` & `enb-1.0.3/enb/plugins/plugin_mhdc_transforms/pot.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_montsec/montsec.jar` & `enb-1.0.3/enb/plugins/plugin_montsec/montsec.jar`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_montsec/montsec_codec.py` & `enb-1.0.3/enb/plugins/plugin_montsec/montsec_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_ndzip/README.txt` & `enb-1.0.3/enb/plugins/plugin_ndzip/README.txt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_ndzip/__plugin__.py` & `enb-1.0.3/enb/plugins/plugin_ndzip/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_ndzip/ndzip_codec.py` & `enb-1.0.3/enb/plugins/plugin_ndzip/ndzip_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_rle/README` & `enb-1.0.3/enb/plugins/plugin_rle/README`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_rle/__plugin__.py` & `enb-1.0.3/enb/plugins/plugin_rle/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_rle/rle.zip` & `enb-1.0.3/enb/plugins/plugin_rle/rle.zip`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_rle/rle_codec.py` & `enb-1.0.3/enb/plugins/plugin_rle/rle_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_spdp/README.txt` & `enb-1.0.3/enb/plugins/plugin_spdp/README.txt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_spdp/SPDP_11.c` & `enb-1.0.3/enb/plugins/plugin_spdp/SPDP_11.c`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_spdp/spdp_codec.py` & `enb-1.0.3/enb/plugins/plugin_spdp/spdp_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_speck/SpeckCode.jar` & `enb-1.0.3/enb/plugins/plugin_speck/SpeckCode.jar`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_speck/SpeckDecode.jar` & `enb-1.0.3/enb/plugins/plugin_speck/SpeckDecode.jar`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_speck/speck_codec.py` & `enb-1.0.3/enb/plugins/plugin_speck/speck_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_v2f/v2f_codecs.py` & `enb-1.0.3/enb/plugins/plugin_v2f/v2f_codecs.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_vvc/Makefile.darwin` & `enb-1.0.3/enb/plugins/plugin_vvc/Makefile.darwin`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_vvc/Makefile.linux` & `enb-1.0.3/enb/plugins/plugin_vvc/Makefile.linux`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_vvc/README.md` & `enb-1.0.3/enb/plugins/plugin_vvc/README.md`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_vvc/__plugin__.py` & `enb-1.0.3/enb/plugins/plugin_vvc/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_vvc/vvc_codec.py` & `enb-1.0.3/enb/plugins/plugin_vvc/vvc_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_vvc/vvc_lossless_400_inter.cfg` & `enb-1.0.3/enb/plugins/plugin_vvc/vvc_lossless_400_inter.cfg`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_vvc/vvc_lossless_400_intra.cfg` & `enb-1.0.3/enb/plugins/plugin_vvc/vvc_lossless_400_intra.cfg`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_vvc/vvc_lossless_400_onecomponent.cfg` & `enb-1.0.3/enb/plugins/plugin_vvc/vvc_lossless_400_onecomponent.cfg`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_vvc/vvc_lossy_400_onecomponent.cfg` & `enb-1.0.3/enb/plugins/plugin_vvc/vvc_lossy_400_onecomponent.cfg`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_zfp/README.md` & `enb-1.0.3/enb/plugins/plugin_zfp/README.md`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_zfp/zfp_codec.py` & `enb-1.0.3/enb/plugins/plugin_zfp/zfp_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_zip/__plugin__.py` & `enb-1.0.3/enb/plugins/plugin_zip/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_zip/zip_codecs.py` & `enb-1.0.3/enb/plugins/plugin_zip/zip_codecs.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/plugin_zstandard/README.txt` & `enb-1.0.3/enb/plugins/plugin_zstandard/README.txt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template.py` & `enb-1.0.3/enb/plugins/template.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_analysis_gallery_example/generate_gallery.py.enbt` & `enb-1.0.3/enb/plugins/template_analysis_gallery_example/generate_gallery.py.enbt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_analysis_gallery_example/input_csv/2d_data_example.csv` & `enb-1.0.3/enb/plugins/template_analysis_gallery_example/input_csv/2d_data_example.csv`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_analysis_gallery_example/input_csv/continent_data_example.csv` & `enb-1.0.3/enb/plugins/template_analysis_gallery_example/input_csv/continent_data_example.csv`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_analysis_gallery_example/input_csv/function.csv` & `enb-1.0.3/enb/plugins/template_analysis_gallery_example/input_csv/function.csv`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_analysis_gallery_example/input_csv/hevc_frame_prediction.csv` & `enb-1.0.3/enb/plugins/template_analysis_gallery_example/input_csv/hevc_frame_prediction.csv`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_analysis_gallery_example/input_csv/iris_dataset.csv` & `enb-1.0.3/enb/plugins/template_analysis_gallery_example/input_csv/iris_dataset.csv`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_base_experiment/README.md` & `enb-1.0.3/enb/plugins/template_base_experiment/README.md`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_base_experiment/__plugin__.py` & `enb-1.0.3/enb/plugins/template_base_experiment/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_base_experiment/datasets/data.bin` & `enb-1.0.3/enb/plugins/template_base_experiment/datasets/data.bin`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_base_experiment/experiment.py.enbt` & `enb-1.0.3/enb/plugins/template_base_experiment/experiment.py.enbt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_basic_workflow_example/basic_workflow.py` & `enb-1.0.3/enb/plugins/template_basic_workflow_example/basic_workflow.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_basic_workflow_example/data/wiki/a_turing.txt` & `enb-1.0.3/enb/plugins/template_basic_workflow_example/data/wiki/a_turing.txt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_basic_workflow_example/data/wiki/c_shannon.txt` & `enb-1.0.3/enb/plugins/template_basic_workflow_example/data/wiki/c_shannon.txt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_basic_workflow_example/data/wiki/d_knuth.txt` & `enb-1.0.3/enb/plugins/template_basic_workflow_example/data/wiki/d_knuth.txt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_basic_workflow_example/data/wiki/k_popper.txt` & `enb-1.0.3/enb/plugins/template_basic_workflow_example/data/wiki/k_popper.txt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_basic_workflow_example/data/wiki/m_curie.txt` & `enb-1.0.3/enb/plugins/template_basic_workflow_example/data/wiki/m_curie.txt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_basic_workflow_example/data/wiki/n_chomsky.txt` & `enb-1.0.3/enb/plugins/template_basic_workflow_example/data/wiki/n_chomsky.txt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_basic_workflow_example/data/wiki/r_franklin.txt` & `enb-1.0.3/enb/plugins/template_basic_workflow_example/data/wiki/r_franklin.txt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_basic_workflow_example/data/wiki/s_beauvoir.txt` & `enb-1.0.3/enb/plugins/template_basic_workflow_example/data/wiki/s_beauvoir.txt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_cluster_config/__plugin__.py` & `enb-1.0.3/enb/plugins/template_cluster_config/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_colors/__plugin__.py` & `enb-1.0.3/enb/plugins/template_colors/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_colors/colors-dark.ini` & `enb-1.0.3/enb/plugins/template_colors/colors-dark.ini`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_colors/colors-default.ini` & `enb-1.0.3/enb/plugins/template_colors/colors-default.ini`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_enb_ini/__plugin__.py` & `enb-1.0.3/enb/plugins/template_enb_ini/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_entropy_codec_comparison/__plugin__.py` & `enb-1.0.3/enb/plugins/template_entropy_codec_comparison/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_entropy_codec_comparison/datasets/image_u8be-1x256x128.raw` & `enb-1.0.3/enb/plugins/template_entropy_codec_comparison/datasets/image_u8be-1x256x128.raw`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_entropy_codec_comparison/entropy_codec_comparison.py.enbt` & `enb-1.0.3/enb/plugins/template_entropy_codec_comparison/entropy_codec_comparison.py.enbt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_file_version_lowercase_example/file_version_example_lowercase.py` & `enb-1.0.3/enb/plugins/template_file_version_lowercase_example/file_version_example_lowercase.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_file_version_lowercase_example/original_data/god_and_state_bakunin.txt` & `enb-1.0.3/enb/plugins/template_file_version_lowercase_example/original_data/god_and_state_bakunin.txt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_file_version_lowercase_example/original_data/kitten_garden_of_verses_oliver_herford.txt` & `enb-1.0.3/enb/plugins/template_file_version_lowercase_example/original_data/kitten_garden_of_verses_oliver_herford.txt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_lossless_compression/README.md` & `enb-1.0.3/enb/plugins/template_lossless_compression/README.md`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_lossless_compression/__plugin__.py` & `enb-1.0.3/enb/plugins/template_lossless_compression/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_lossless_compression/datasets/image_u8be-2x128x128.raw` & `enb-1.0.3/enb/plugins/template_lossless_compression/datasets/image_u8be-2x128x128.raw`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_lossless_compression/lossless_compression_experiment.py.enbt` & `enb-1.0.3/enb/plugins/template_lossless_compression/lossless_compression_experiment.py.enbt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_lossy_compression/README.md` & `enb-1.0.3/enb/plugins/template_lossy_compression/README.md`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_lossy_compression/__plugin__.py` & `enb-1.0.3/enb/plugins/template_lossy_compression/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_lossy_compression/datasets/image1_u8be-1x128x256.raw` & `enb-1.0.3/enb/plugins/template_lossy_compression/datasets/image1_u8be-1x128x256.raw`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_lossy_compression/datasets/image2_u8be-1x128x256.raw` & `enb-1.0.3/enb/plugins/template_lossy_compression/datasets/image2_u8be-1x128x256.raw`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_lossy_compression/lossy_compression_experiment.py.enbt` & `enb-1.0.3/enb/plugins/template_lossy_compression/lossy_compression_experiment.py.enbt`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_matplotlibrc/__plugin__.py` & `enb-1.0.3/enb/plugins/template_matplotlibrc/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_montecarlo_pi/__plugin__.py` & `enb-1.0.3/enb/plugins/template_montecarlo_pi/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_montecarlo_pi/montecarlo_pi_experiment.py` & `enb-1.0.3/enb/plugins/template_montecarlo_pi/montecarlo_pi_experiment.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_port_experiment_example/experiment_example.py` & `enb-1.0.3/enb/plugins/template_port_experiment_example/experiment_example.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_test_all_codecs/__plugin__.py` & `enb-1.0.3/enb/plugins/template_test_all_codecs/__plugin__.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_test_all_codecs/generate_test_images.py` & `enb-1.0.3/enb/plugins/template_test_all_codecs/generate_test_images.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/plugins/template_test_all_codecs/test_all_codecs.py` & `enb-1.0.3/enb/plugins/template_test_all_codecs/test_all_codecs.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/png.py` & `enb-1.0.3/enb/png.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/progress.py` & `enb-1.0.3/enb/progress.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/render.py` & `enb-1.0.3/enb/render.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/sets.py` & `enb-1.0.3/enb/sets.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,32 +74,21 @@
         file_path = file_path[1:]
         return file_path
 
     @atable.column_function("corpus", label="Corpus name")
     def set_corpus(self, file_path, row):
         """Store the corpus name of a data sample.
         By default, it is the name of the folder in which the sample is stored.
-        """
-        file_path = os.path.abspath(os.path.realpath(file_path))
-        if options.base_dataset_dir is not None \
-                and os.path.dirname(file_path) != os.path.abspath(os.path.realpath(options.base_dataset_dir)):
-            file_dir = os.path.dirname(file_path)
-            if self.base_dir is not None:
-                file_dir = file_dir.replace(self.base_dir, "")
-            while file_dir and file_dir[0] == os.sep:
-                file_dir = file_dir[1:]
-        else:
-            file_dir = os.path.basename(
-                os.path.dirname(file_path))
-
-        if not file_dir:
-            file_dir = os.path.basename(
-                os.path.dirname(file_path))
 
-        row[_column_name] = os.path.basename(os.path.abspath(file_dir))
+        Symbolic links can be used within the base dataset dir (./datasets by default).
+        In that case, they are treated as a regular file with the path relative to the project.
+        """
+        row[_column_name] = os.path.basename(os.path.dirname(file_path)) \
+            if os.path.dirname(file_path) \
+            else os.path.basename(os.path.dirname(os.path.abspath(file_path)))
 
     @atable.column_function("size_bytes", label="File size (bytes)")
     def set_file_size(self, file_path, row):
         """Store the original file size in row.
         :param file_path: path to the file to analyze
         :param row: dictionary of previously computed values for this file_path
           (to speed up derived values).
```

### Comparing `enb-1.0.2/enb/tarlite.py` & `enb-1.0.3/enb/tarlite.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb/tcall.py` & `enb-1.0.3/enb/tcall.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/enb.egg-info/PKG-INFO` & `enb-1.0.3/enb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: enb
-Version: 1.0.2
+Version: 1.0.3
 Summary: Experiment NoteBook (enb): efficient and reproducible science.
 Home-page: https://github.com/miguelinux314/experiment-notebook
-Download-URL: https://github.com/miguelinux314/experiment-notebook/archive/v1.0.2.tar.gz
+Download-URL: https://github.com/miguelinux314/experiment-notebook/archive/v1.0.3.tar.gz
 Author: Miguel Hernández Cabronero, et al.
 Author-email: miguel.hernandez@uab.cat
 License: MIT License
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
@@ -37,15 +37,15 @@
 Requires-Dist: astropy
 Requires-Dist: natsort
 Requires-Dist: rich
 Requires-Dist: h5py
 
 # Experiment Notebook (`enb`)
 
-The `enb` Python (>= 3.6) library is a table-based framework designed to define, run and report computer-based
+The `enb` Python (>= 3.7) library is a table-based framework designed to define, run and report computer-based
 experiments.
 
 - Your can create and run any type of (computer-based) experiment. Quickly.
 - You can analyze and plot results produced with your enb experiments. Clearly. You can also reuse previously existing
   data (e.g., in CSV format).
 - You can easily create reproducible, redistributable software to be shared with others, e.g., as supplementary
   materials in your publication or project.
```

### Comparing `enb-1.0.2/enb.egg-info/SOURCES.txt` & `enb-1.0.3/enb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 enb/plugins/plugin_ccsds122/__plugin__.py
 enb/plugins/plugin_ccsds122/ccsds122_codec.py
 enb/plugins/plugin_ccsds124/.gitignore
 enb/plugins/plugin_ccsds124/README.md
 enb/plugins/plugin_ccsds124/__plugin__.py
 enb/plugins/plugin_ccsds124/ccsds124_codecs.py
 enb/plugins/plugin_emporda/__plugin__.py
-enb/plugins/plugin_emporda/emporda.jar
 enb/plugins/plugin_emporda/emporda_codec.py
 enb/plugins/plugin_fapec/.gitignore
 enb/plugins/plugin_fapec/README.md
 enb/plugins/plugin_fapec/__plugin__.py
 enb/plugins/plugin_fapec/fapec_codec.py
 enb/plugins/plugin_flif/.gitignore
 enb/plugins/plugin_flif/Makefile.darwin
@@ -146,14 +145,17 @@
 enb/plugins/plugin_jpeg_xl/README.md
 enb/plugins/plugin_jpeg_xl/__plugin__.py
 enb/plugins/plugin_jpeg_xl/jpegxl_codec.py
 enb/plugins/plugin_kakadu/.gitignore
 enb/plugins/plugin_kakadu/README.md
 enb/plugins/plugin_kakadu/__plugin__.py
 enb/plugins/plugin_kakadu/kakadu_codec.py
+enb/plugins/plugin_lc_framework/Makefile.linux
+enb/plugins/plugin_lc_framework/__plugin__.py
+enb/plugins/plugin_lc_framework/lc_codec.py
 enb/plugins/plugin_lcnl/.gitignore
 enb/plugins/plugin_lcnl/README.md
 enb/plugins/plugin_lcnl/__plugin__.py
 enb/plugins/plugin_lcnl/lcnl_codecs.py
 enb/plugins/plugin_lpaq8/Makefile.linux
 enb/plugins/plugin_lpaq8/__plugin__.py
 enb/plugins/plugin_lpaq8/lpaq8.cpp
```

### Comparing `enb-1.0.2/setup.py` & `enb-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/test/test_aanalysis.py` & `enb-1.0.3/test/test_aanalysis.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/test/test_all.py` & `enb-1.0.3/test/test_all.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/test/test_atable.py` & `enb-1.0.3/test/test_atable.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/test/test_bitstream.py` & `enb-1.0.3/test/test_bitstream.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/test/test_codec.py` & `enb-1.0.3/test/test_codec.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/test/test_experiment.py` & `enb-1.0.3/test/test_experiment.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/test/test_icompression.py` & `enb-1.0.3/test/test_icompression.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/test/test_isets.py` & `enb-1.0.3/test/test_isets.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/test/test_log.py` & `enb-1.0.3/test/test_log.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/test/test_pgm.py` & `enb-1.0.3/test/test_pgm.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/test/test_ray.py` & `enb-1.0.3/test/test_ray.py`

 * *Files identical despite different names*

### Comparing `enb-1.0.2/test/test_sets.py` & `enb-1.0.3/test/test_sets.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 
 
 class TestSets(unittest.TestCase):
 
     def test_file_properties(self):
         """Test that file properties are correctly obtained and retrieved.
         """
-        target_indices = [p for p in glob.glob(
-            os.path.join(enb.calling_script_dir, "*.py"))
+        target_indices = [p for p in glob.glob(os.path.join(enb.calling_script_dir, "*.py"))
                           if os.path.isfile(p)]
 
         # dataset_df = get_result_df()
         with tempfile.NamedTemporaryFile(suffix=".csv") as tmp_file:
             dataset_properties_table = sets.FilePropertiesTable(
                 csv_support_path=tmp_file.name)
 
@@ -53,16 +52,16 @@
             assert (dataset_properties_df.columns == new_df.columns).all()
 
             for c in dataset_properties_df.columns:
                 try:
                     if not (dataset_properties_df[c] == new_df[c]).all():
                         # Floating point values might be unstable
                         try:
-                            assert np.abs(dataset_properties_df[c] - new_df[
-                                c]).max() < 1e-12
+                            assert np.abs(dataset_properties_df[c] - new_df[c]).max() < 1e-12, (
+                            dataset_properties_df[c], new_df[c])
                         except TypeError:
                             # Stability within dictionaries is not verified,
                             # but only dictionaries can raise this error
                             assert (dataset_properties_df[c].apply(
                                 lambda c: isinstance(c, dict))).all()
                 except ValueError as ex:
                     raise RuntimeError(
@@ -95,19 +94,18 @@
             tvt = TrivialVersionTable(version_base_dir=tmp_dir,
                                       version_name="trivial",
                                       original_base_dir=options.project_root)
             tvt_df = tvt.get_df()
             for input_path in (
                     p for p in glob.glob(
                 os.path.join(options.project_root, "**", "*.py"), recursive=True)
-                               if os.path.isfile(p)):
+                    if os.path.isfile(p)):
                 assert filecmp.cmp(input_path,
                                    tvt.original_to_versioned_path(input_path))
 
-
             lsuffix = "_original"
             rsuffix = f"_{tvt.version_name}"
             joint_df = fpt_df.set_index("original_file_path").join(
                 tvt_df.set_index("original_file_path"),
                 lsuffix=lsuffix, rsuffix=rsuffix)
 
             assert not np.any(joint_df.applymap(lambda x: x is None))
```

### Comparing `enb-1.0.2/test/test_tarlite.py` & `enb-1.0.3/test/test_tarlite.py`

 * *Files identical despite different names*

